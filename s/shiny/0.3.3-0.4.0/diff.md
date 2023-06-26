# Comparing `tmp/shiny-0.3.3.tar.gz` & `tmp/shiny-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny-0.3.3.tar", last modified: Wed Apr 26 21:38:03 2023, max compression
+gzip compressed data, was "shiny-0.4.0.tar", last modified: Mon Jun 26 20:02:49 2023, max compression
```

## Comparing `shiny-0.3.3.tar` & `shiny-0.4.0.tar`

### file list

```diff
@@ -1,489 +1,579 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.931761 shiny-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 21:36:42.000000 shiny-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-26 21:36:42.000000 shiny-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-26 21:38:03.931761 shiny-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 21:36:42.000000 shiny-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-26 21:38:03.935761 shiny-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:36:42.000000 shiny-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.847760 shiny-0.3.3/shiny/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_fileupload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_hostenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_launchbrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_shinyenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.831760 shiny-0.3.3/shiny/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.847760 shiny-0.3.3/shiny/examples/Calc/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/Calc/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.847760 shiny-0.3.3/shiny/examples/Effect/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/Effect/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.847760 shiny-0.3.3/shiny/examples/Module/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/Module/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.847760 shiny-0.3.3/shiny/examples/Progress/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/Progress/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.847760 shiny-0.3.3/shiny/examples/SafeException/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/SafeException/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.847760 shiny-0.3.3/shiny/examples/SilentCancelOutputException/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/SilentCancelOutputException/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.847760 shiny-0.3.3/shiny/examples/SilentException/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/SilentException/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.847760 shiny-0.3.3/shiny/examples/Value/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/Value/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.847760 shiny-0.3.3/shiny/examples/close/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/close/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/download/
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/download/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/download/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/download_button/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/download_button/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/download_button/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/download_link/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/download_link/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/download_link/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/dynamic_route/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/dynamic_route/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/event/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/event/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/file_reader/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/file_reader/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/file_reader/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/input_action_button/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_action_button/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/input_action_link/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_action_link/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/input_checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_checkbox/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/input_checkbox_group/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_checkbox_group/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/input_date/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_date/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/input_date_range/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_date_range/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.851760 shiny-0.3.3/shiny/examples/input_file/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_file/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/input_numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_numeric/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/input_password/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_password/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/input_radio_buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_radio_buttons/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/input_select/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_select/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/input_selectize/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_selectize/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/input_slider/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_slider/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/input_switch/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_switch/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/input_text/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_text/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/input_text_area/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/input_text_area/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/insert_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/insert_ui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/invalidate_later/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/invalidate_later/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/isolate/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/isolate/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/layout_sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/layout_sidebar/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/markdown/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/modal/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/modal/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/nav/
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/nav/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.855760 shiny-0.3.3/shiny/examples/navset_hidden/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/navset_hidden/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/notification_show/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/notification_show/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/on_ended/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/on_ended/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/on_flush/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/on_flush/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/on_flushed/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/on_flushed/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/output_image/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/output_image/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/output_image/posit-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/output_plot/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/output_plot/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/output_table/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/output_table/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/output_table/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/output_text/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/output_text/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/output_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/output_ui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/page_fixed/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/page_fixed/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/page_fluid/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/page_fluid/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/panel_absolute/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/panel_absolute/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/panel_conditional/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/panel_conditional/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/panel_title/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/panel_title/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/poll/
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/poll/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.859760 shiny-0.3.3/shiny/examples/remove_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/remove_ui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/render_image/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/render_image/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/req/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/req/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/row/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/row/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/send_custom_message/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/send_custom_message/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/template/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/update_action_button/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/update_action_button/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/update_checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/update_checkbox/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/update_checkbox_group/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/update_checkbox_group/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/update_date/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/update_date/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/update_date_range/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/update_date_range/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/update_navs/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/update_navs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/update_numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/update_numeric/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/update_radio_buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/update_radio_buttons/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/update_select/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/update_select/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/update_selectize/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/update_selectize/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.863760 shiny-0.3.3/shiny/examples/update_slider/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/update_slider/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.867760 shiny-0.3.3/shiny/examples/update_text/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/update_text/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.867760 shiny-0.3.3/shiny/examples/www_dir/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/www_dir/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.831760 shiny-0.3.3/shiny/examples/www_dir/www/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.867760 shiny-0.3.3/shiny/examples/www_dir/www/css/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/www_dir/www/css/more-styles.css
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/www_dir/www/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.867760 shiny-0.3.3/shiny/examples/www_dir/www/js/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/examples/www_dir/www/js/changetext.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.867760 shiny-0.3.3/shiny/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.871760 shiny-0.3.3/shiny/experimental/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_card_full_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_card_item.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_css.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_htmldeps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_input_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_sidebar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/ui/_valuebox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.871760 shiny-0.3.3/shiny/experimental/www/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/www/card-full-screen.js
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/www/fill.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.871760 shiny-0.3.3/shiny/experimental/www/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/www/sidebar/sidebar.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/www/sidebar/sidebar.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/www/textarea-autoresize.css
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/experimental/www/textarea-autoresize.js
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/html_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/http_staticfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/input_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/plotutils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.871760 shiny-0.3.3/shiny/reactive/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/reactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/reactive/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/reactive/_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)    30436 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/reactive/_reactives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.871760 shiny-0.3.3/shiny/render/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/render/_coordmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    25137 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/render/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/render/_try_render_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.875760 shiny-0.3.3/shiny/session/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39788 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/session/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/session/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.879760 shiny-0.3.3/shiny/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_download_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_html_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_input_action_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_input_check_radio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_input_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_input_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_input_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_input_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_input_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_input_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_input_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    26041 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_input_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    27410 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_navs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_plot_output_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/ui/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.835760 shiny-0.3.3/shiny/www/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.887760 shiny-0.3.3/shiny/www/shared/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.887760 shiny-0.3.3/shiny/www/shared/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)    80496 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/bootstrap/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   333304 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   248284 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/bootstrap/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.835760 shiny-0.3.3/shiny/www/shared/bootstrap/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.891761 shiny-0.3.3/shiny/www/shared/bootstrap/fonts/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/bootstrap/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.891761 shiny-0.3.3/shiny/www/shared/datatables/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.891761 shiny-0.3.3/shiny/www/shared/datatables/css/
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datatables/css/dataTables.bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datatables/css/dataTables.extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.891761 shiny-0.3.3/shiny/www/shared/datatables/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datatables/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datatables/images/sort_asc_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datatables/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datatables/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datatables/images/sort_desc_disabled.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.891761 shiny-0.3.3/shiny/www/shared/datatables/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datatables/js/dataTables.bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)    78980 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datatables/js/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datatables/upgrade1.10.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.835760 shiny-0.3.3/shiny/www/shared/datepicker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.895761 shiny-0.3.3/shiny/www/shared/datepicker/css/
--rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/css/bootstrap-datepicker3.css
--rw-r--r--   0 runner    (1001) docker     (123)    21013 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.895761 shiny-0.3.3/shiny/www/shared/datepicker/js/
--rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/bootstrap-datepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)   106348 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.915761 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.az.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bm.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bn.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.br.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ca.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cy.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.da.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.de.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.el.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-AU.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-CA.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-GB.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-IE.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-NZ.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-ZA.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.es.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.et.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eu.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fa.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fi.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr-CH.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.gl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.he.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hi.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hu.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hy.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.id.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.is.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it-CH.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ja.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ka.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kh.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.km.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ko.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lt.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.me.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mn.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ms.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl-BE.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.no.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.oc.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pt-BR.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pt.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ro.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs-latin.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ru.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.si.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sq.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr-latin.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sw.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ta.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.th.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-cyrl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-latn.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.vi.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-CN.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-TW.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.915761 shiny-0.3.3/shiny/www/shared/datepicker/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/scss/build3.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/datepicker/scss/datepicker3.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.915761 shiny-0.3.3/shiny/www/shared/highlight/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/highlight/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22392 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/highlight/classref.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/highlight/highlight.pack.js
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/highlight/rstudio.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.835760 shiny-0.3.3/shiny/www/shared/ionrangeslider/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.915761 shiny-0.3.3/shiny/www/shared/ionrangeslider/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/ionrangeslider/css/ion.rangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.915761 shiny-0.3.3/shiny/www/shared/ionrangeslider/js/
--rw-r--r--   0 runner    (1001) docker     (123)    84989 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.js
--rw-r--r--   0 runner    (1001) docker     (123)    41631 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.915761 shiny-0.3.3/shiny/www/shared/ionrangeslider/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/ionrangeslider/scss/_base.scss
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/ionrangeslider/scss/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/ionrangeslider/scss/shiny.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.919761 shiny-0.3.3/shiny/www/shared/jquery/
--rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jquery/jquery-3.6.0.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jquery/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jquery/jquery-3.6.0.min.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.923761 shiny-0.3.3/shiny/www/shared/jqueryui/
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.923761 shiny-0.3.3/shiny/www/shared/jqueryui/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    32532 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    37452 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)   529159 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)    32130 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.structure.css
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.structure.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.theme.css
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.theme.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.923761 shiny-0.3.3/shiny/www/shared/requirejs/
--rw-r--r--   0 runner    (1001) docker     (123)    19715 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/requirejs/require.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.839760 shiny-0.3.3/shiny/www/shared/selectize/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.839760 shiny-0.3.3/shiny/www/shared/selectize/accessibility/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.923761 shiny-0.3.3/shiny/www/shared/selectize/accessibility/js/
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.js
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.923761 shiny-0.3.3/shiny/www/shared/selectize/css/
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/css/selectize.bootstrap3.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.923761 shiny-0.3.3/shiny/www/shared/selectize/js/
--rw-r--r--   0 runner    (1001) docker     (123)    45139 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/js/selectize.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.927761 shiny-0.3.3/shiny/www/shared/selectize/scss/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.927761 shiny-0.3.3/shiny/www/shared/selectize/scss/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/scss/plugins/drag_drop.scss
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/scss/plugins/dropdown_header.scss
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/scss/plugins/optgroup_columns.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/scss/plugins/remove_button.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/scss/selectize.bootstrap3.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/scss/selectize.bootstrap4.scss
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/scss/selectize.bootstrap5.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/scss/selectize.default.scss
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/selectize/scss/selectize.scss
--rw-r--r--   0 runner    (1001) docker     (123)    23760 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny-autoreload.js
--rw-r--r--   0 runner    (1001) docker     (123)   125989 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny-autoreload.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny-showcase.css
--rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny-showcase.js
--rw-r--r--   0 runner    (1001) docker     (123)   126645 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny-showcase.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny-testmode.js
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny-testmode.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   757524 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny.js
--rw-r--r--   0 runner    (1001) docker     (123)  1314664 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   306317 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1349172 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.927761 shiny-0.3.3/shiny/www/shared/shiny_scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny_scss/bootstrap.scss
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/shiny_scss/shiny.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.927761 shiny-0.3.3/shiny/www/shared/showdown/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.927761 shiny-0.3.3/shiny/www/shared/showdown/compressed/
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/showdown/compressed/showdown.js
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/showdown/license.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.927761 shiny-0.3.3/shiny/www/shared/showdown/src/
--rw-r--r--   0 runner    (1001) docker     (123)    37933 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/showdown/src/showdown.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.927761 shiny-0.3.3/shiny/www/shared/strftime/
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-04-26 21:36:42.000000 shiny-0.3.3/shiny/www/shared/strftime/strftime-min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.847760 shiny-0.3.3/shiny.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-26 21:38:03.000000 shiny-0.3.3/shiny.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15956 2023-04-26 21:38:03.000000 shiny-0.3.3/shiny.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:38:03.000000 shiny-0.3.3/shiny.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 21:38:03.000000 shiny-0.3.3/shiny.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:38:03.000000 shiny-0.3.3/shiny.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-26 21:38:03.000000 shiny-0.3.3/shiny.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 21:38:03.000000 shiny-0.3.3/shiny.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:38:03.931761 shiny-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/asyncio_prevent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/mocktime.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_e2e_regex_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_navs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)    31010 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_reactives.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_shinysession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_ui_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-04-26 21:36:42.000000 shiny-0.3.3/tests/test_utils_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.476434 shiny-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-26 20:01:07.000000 shiny-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 20:01:07.000000 shiny-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-26 20:02:49.476434 shiny-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-26 20:01:07.000000 shiny-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-26 20:02:49.480434 shiny-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:01:07.000000 shiny-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.372433 shiny-0.4.0/shiny/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14468 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_fileupload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_hostenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_launchbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_shinyenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.344432 shiny-0.4.0/shiny/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.372433 shiny-0.4.0/shiny/examples/Calc/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/Calc/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/Effect/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/Effect/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/Module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/Module/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/Progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/Progress/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/SafeException/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/SafeException/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/SilentCancelOutputException/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/SilentCancelOutputException/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/SilentException/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/SilentException/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/Value/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/Value/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/close/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/close/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/data_frame/
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/data_frame/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/download/
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/download/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/download/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/download_button/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/download_button/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/download_button/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/download_link/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/download_link/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/download_link/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/dynamic_route/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/dynamic_route/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/event/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/event/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/file_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/file_reader/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/file_reader/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/include_css/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/include_css/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/include_css/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/include_css/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/include_javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/include_javascript/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/include_javascript/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/include_javascript/js/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/input_action_button/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_action_button/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/input_action_link/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_action_link/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/input_checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_checkbox/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/input_checkbox_group/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_checkbox_group/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/input_date/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_date/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.376433 shiny-0.4.0/shiny/examples/input_date_range/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_date_range/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/input_file/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_file/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/input_numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_numeric/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/input_password/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_password/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/input_radio_buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_radio_buttons/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/input_select/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_select/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/input_selectize/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_selectize/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/input_slider/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_slider/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/input_switch/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_switch/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/input_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_text/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/input_text_area/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/input_text_area/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/insert_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/insert_ui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/invalidate_later/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/invalidate_later/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/isolate/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/isolate/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/layout_sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/layout_sidebar/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/markdown/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/modal/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/modal/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/nav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/nav/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/navset_hidden/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/navset_hidden/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/notification_show/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/notification_show/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.380433 shiny-0.4.0/shiny/examples/on_ended/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/on_ended/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.384433 shiny-0.4.0/shiny/examples/on_flush/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/on_flush/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.384433 shiny-0.4.0/shiny/examples/on_flushed/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/on_flushed/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.388433 shiny-0.4.0/shiny/examples/output_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/output_image/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/output_image/posit-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.388433 shiny-0.4.0/shiny/examples/output_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/output_plot/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.388433 shiny-0.4.0/shiny/examples/output_table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/output_table/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/output_table/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.388433 shiny-0.4.0/shiny/examples/output_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/output_text/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.388433 shiny-0.4.0/shiny/examples/output_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/output_ui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.392433 shiny-0.4.0/shiny/examples/page_fixed/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/page_fixed/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.392433 shiny-0.4.0/shiny/examples/page_fluid/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/page_fluid/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.392433 shiny-0.4.0/shiny/examples/panel_absolute/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/panel_absolute/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.392433 shiny-0.4.0/shiny/examples/panel_conditional/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/panel_conditional/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.392433 shiny-0.4.0/shiny/examples/panel_title/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/panel_title/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.392433 shiny-0.4.0/shiny/examples/poll/
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/poll/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.392433 shiny-0.4.0/shiny/examples/remove_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/remove_ui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.392433 shiny-0.4.0/shiny/examples/render_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/render_image/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.396433 shiny-0.4.0/shiny/examples/req/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/req/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.396433 shiny-0.4.0/shiny/examples/row/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/row/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.396433 shiny-0.4.0/shiny/examples/send_custom_message/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/send_custom_message/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.396433 shiny-0.4.0/shiny/examples/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.396433 shiny-0.4.0/shiny/examples/update_action_button/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/update_action_button/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.396433 shiny-0.4.0/shiny/examples/update_checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/update_checkbox/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.396433 shiny-0.4.0/shiny/examples/update_checkbox_group/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/update_checkbox_group/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.396433 shiny-0.4.0/shiny/examples/update_date/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/update_date/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.396433 shiny-0.4.0/shiny/examples/update_date_range/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/update_date_range/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.400433 shiny-0.4.0/shiny/examples/update_navs/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/update_navs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.400433 shiny-0.4.0/shiny/examples/update_numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/update_numeric/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.400433 shiny-0.4.0/shiny/examples/update_radio_buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/update_radio_buttons/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.400433 shiny-0.4.0/shiny/examples/update_select/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/update_select/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.400433 shiny-0.4.0/shiny/examples/update_selectize/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/update_selectize/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.400433 shiny-0.4.0/shiny/examples/update_slider/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/update_slider/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.400433 shiny-0.4.0/shiny/examples/update_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/update_text/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.400433 shiny-0.4.0/shiny/examples/www_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/www_dir/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.348432 shiny-0.4.0/shiny/examples/www_dir/www/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/examples/www_dir/www/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/www_dir/www/css/more-styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/www_dir/www/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/examples/www_dir/www/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/examples/www_dir/www/js/changetext.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.348432 shiny-0.4.0/shiny/experimental/e2e/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/e2e/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/e2e/accordion/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/e2e/navbar/
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/e2e/navbar/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/e2e/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/e2e/sidebar/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/e2e/sidebar/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.360432 shiny-0.4.0/shiny/experimental/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/examples/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/accordion/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/examples/accordion_panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/accordion_panel/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/examples/accordion_panel_close/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/accordion_panel_close/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/examples/accordion_panel_insert/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/accordion_panel_insert/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/examples/accordion_panel_open/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/accordion_panel_open/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/examples/accordion_panel_remove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/accordion_panel_remove/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/examples/accordion_panel_set/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/accordion_panel_set/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/examples/accordion_panel_update/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/accordion_panel_update/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/examples/as_fill_carrier/
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/as_fill_carrier/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.404433 shiny-0.4.0/shiny/experimental/examples/as_fill_item/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/as_fill_item/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/as_fillable_container/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/as_fillable_container/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/card/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/card/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/card_body/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/card_body/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/card_footer/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/card_footer/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/card_header/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/card_header/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/card_image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/card_image/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/card_title/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/card_title/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/layout_column_wrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/layout_column_wrap/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/layout_sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/layout_sidebar/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/page_sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/page_sidebar/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/showcase_left_center/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/showcase_left_center/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/showcase_top_right/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/showcase_top_right/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/sidebar/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/sidebar_toggle/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/sidebar_toggle/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.408433 shiny-0.4.0/shiny/experimental/examples/value_box/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/examples/value_box/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.412433 shiny-0.4.0/shiny/experimental/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21922 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_accordion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23675 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_css_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18563 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_htmldeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_input_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19808 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_navs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21327 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/ui/_valuebox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.412433 shiny-0.4.0/shiny/experimental/www/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.412433 shiny-0.4.0/shiny/experimental/www/bslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/www/bslib/_version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.412433 shiny-0.4.0/shiny/experimental/www/bslib/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/www/bslib/components/accordion.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/www/bslib/components/accordion.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/www/bslib/components/card.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26956 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/www/bslib/components/card.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/www/bslib/components/sidebar.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/www/bslib/components/sidebar.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.412433 shiny-0.4.0/shiny/experimental/www/htmltools/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/www/htmltools/_version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.412433 shiny-0.4.0/shiny/experimental/www/htmltools/fill/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/www/htmltools/fill/fill.css
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/www/textarea-autoresize.css
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/experimental/www/textarea-autoresize.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/html_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/http_staticfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/input_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/plotutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.416433 shiny-0.4.0/shiny/reactive/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/reactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/reactive/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/reactive/_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30454 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/reactive/_reactives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.416433 shiny-0.4.0/shiny/render/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/render/_coordmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/render/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24854 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/render/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/render/_try_render_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.416433 shiny-0.4.0/shiny/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39788 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/session/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/session/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.420433 shiny-0.4.0/shiny/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_download_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_html_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_include_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_input_action_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_input_check_radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_input_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_input_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_input_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_input_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_input_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_input_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_input_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26041 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_input_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27419 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_navs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_plot_output_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.420433 shiny-0.4.0/shiny/ui/_x/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_x/_css_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_x/_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_x/_htmldeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_x/_sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_x/_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/_x/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.420433 shiny-0.4.0/shiny/ui/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/dataframe/_dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.364432 shiny-0.4.0/shiny/ui/dataframe/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.420433 shiny-0.4.0/shiny/ui/dataframe/js/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    98259 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/dataframe/js/dist/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)   518230 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/ui/dataframe/js/dist/index.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.364432 shiny-0.4.0/shiny/www/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.428433 shiny-0.4.0/shiny/www/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/_version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.364432 shiny-0.4.0/shiny/www/shared/_x/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.364432 shiny-0.4.0/shiny/www/shared/_x/bslib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.428433 shiny-0.4.0/shiny/www/shared/_x/bslib/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/_x/bslib/components/sidebar.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/_x/bslib/components/sidebar.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.364432 shiny-0.4.0/shiny/www/shared/_x/htmltools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.428433 shiny-0.4.0/shiny/www/shared/_x/htmltools/fill/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/_x/htmltools/fill/fill.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.432433 shiny-0.4.0/shiny/www/shared/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/bootstrap/_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)    80496 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/bootstrap/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   333304 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   258637 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/bootstrap/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.364432 shiny-0.4.0/shiny/www/shared/bootstrap/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.432433 shiny-0.4.0/shiny/www/shared/bootstrap/fonts/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.364432 shiny-0.4.0/shiny/www/shared/datepicker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.432433 shiny-0.4.0/shiny/www/shared/datepicker/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/css/bootstrap-datepicker3.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21013 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.432433 shiny-0.4.0/shiny/www/shared/datepicker/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/bootstrap-datepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   106348 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.448433 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.az.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bm.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bn.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.br.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bs.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ca.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cs.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cy.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.da.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.de.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.el.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-AU.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-CA.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-GB.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-IE.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-NZ.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-ZA.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.es.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.et.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eu.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fa.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fi.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr-CH.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.gl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.he.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hi.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hu.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hy.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.id.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.is.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it-CH.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ja.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ka.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kh.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.km.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ko.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lt.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.me.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mn.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ms.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl-BE.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.no.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.oc.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pt-BR.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pt.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ro.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs-latin.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ru.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.si.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sq.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr-latin.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sw.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ta.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.th.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-cyrl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-latn.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.vi.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-CN.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-TW.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.448433 shiny-0.4.0/shiny/www/shared/datepicker/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/scss/build3.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/datepicker/scss/datepicker3.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.452434 shiny-0.4.0/shiny/www/shared/highlight/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/highlight/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22392 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/highlight/classref.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/highlight/highlight.pack.js
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/highlight/rstudio.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.364432 shiny-0.4.0/shiny/www/shared/ionrangeslider/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.452434 shiny-0.4.0/shiny/www/shared/ionrangeslider/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/ionrangeslider/css/ion.rangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.452434 shiny-0.4.0/shiny/www/shared/ionrangeslider/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    84989 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41631 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.452434 shiny-0.4.0/shiny/www/shared/ionrangeslider/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/ionrangeslider/scss/_base.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/ionrangeslider/scss/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/ionrangeslider/scss/shiny.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.452434 shiny-0.4.0/shiny/www/shared/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jquery/jquery-3.6.0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jquery/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jquery/jquery-3.6.0.min.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.464434 shiny-0.4.0/shiny/www/shared/jqueryui/
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.468434 shiny-0.4.0/shiny/www/shared/jqueryui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32532 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    37452 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)   529159 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32130 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.structure.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.structure.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.theme.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.468434 shiny-0.4.0/shiny/www/shared/requirejs/
+-rw-r--r--   0 runner    (1001) docker     (123)    19715 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/requirejs/require.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.364432 shiny-0.4.0/shiny/www/shared/selectize/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.364432 shiny-0.4.0/shiny/www/shared/selectize/accessibility/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.468434 shiny-0.4.0/shiny/www/shared/selectize/accessibility/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.468434 shiny-0.4.0/shiny/www/shared/selectize/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/css/selectize.bootstrap3.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.468434 shiny-0.4.0/shiny/www/shared/selectize/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    45139 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/js/selectize.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.468434 shiny-0.4.0/shiny/www/shared/selectize/scss/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.472434 shiny-0.4.0/shiny/www/shared/selectize/scss/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/scss/plugins/drag_drop.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/scss/plugins/dropdown_header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/scss/plugins/optgroup_columns.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/scss/plugins/remove_button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/scss/selectize.bootstrap3.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/scss/selectize.bootstrap4.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/scss/selectize.bootstrap5.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/scss/selectize.default.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/selectize/scss/selectize.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    23760 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny-autoreload.js
+-rw-r--r--   0 runner    (1001) docker     (123)   125989 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny-autoreload.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny-showcase.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny-showcase.js
+-rw-r--r--   0 runner    (1001) docker     (123)   126645 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny-showcase.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny-testmode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny-testmode.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   757524 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1314664 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   306317 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1349172 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.472434 shiny-0.4.0/shiny/www/shared/shiny_scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny_scss/bootstrap.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/shiny_scss/shiny.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.472434 shiny-0.4.0/shiny/www/shared/showdown/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.472434 shiny-0.4.0/shiny/www/shared/showdown/compressed/
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/showdown/compressed/showdown.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/showdown/license.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.472434 shiny-0.4.0/shiny/www/shared/showdown/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    37933 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/showdown/src/showdown.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.472434 shiny-0.4.0/shiny/www/shared/strftime/
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-26 20:01:07.000000 shiny-0.4.0/shiny/www/shared/strftime/strftime-min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.372433 shiny-0.4.0/shiny.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-26 20:02:49.000000 shiny-0.4.0/shiny.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17914 2023-06-26 20:02:49.000000 shiny-0.4.0/shiny.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:02:49.000000 shiny-0.4.0/shiny.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 20:02:49.000000 shiny-0.4.0/shiny.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:02:49.000000 shiny-0.4.0/shiny.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-26 20:02:49.000000 shiny-0.4.0/shiny.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 20:02:49.000000 shiny-0.4.0/shiny.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:02:49.476434 shiny-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/asyncio_prevent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/mocktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_e2e_regex_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_navs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31032 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_reactives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_shinysession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_ui_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_utils_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-26 20:01:07.000000 shiny-0.4.0/tests/test_x_sidebar.py
```

### Comparing `shiny-0.3.3/LICENSE` & `shiny-0.4.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 RStudio, PBC
+Copyright (c) 2023 Posit Software, PBC
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `shiny-0.3.3/setup.cfg` & `shiny-0.4.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 description = A web development framework for Python.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 platforms = any
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 project_urls = 
 	Bug Tracker = https://github.com/rstudio/py-shiny/issues
-	Documentation = https://shiny.rstudio.com/py/
+	Documentation = https://shiny.posit.co/py/
 	Source Code = https://github.com/rstudio/py-shiny
 
 [options]
 python_requires = >=3.7
-packages = find:
+packages = find_namespace:
 test_suite = tests
 include_package_data = True
 setup_requires = 
 	setuptools
 install_requires = 
 	typing-extensions>=4.0.1
 	uvicorn>=0.16.0
@@ -42,26 +42,29 @@
 	htmltools>=0.2.1
 	click>=8.0.3
 	markdown-it-py>=1.1.0
 	mdit-py-plugins>=0.3.0
 	linkify-it-py>=1.0
 	appdirs>=1.4.4
 	asgiref>=3.5.2
+	watchfiles>=0.18.0;platform_system!="Emscripten"
 	importlib-metadata>=1.1.0,<5;python_version<"3.8"
 tests_require = 
 	pytest>=3
 zip_safe = False
 
 [options.extras_require]
 test = 
 	pytest>=6.2.4
 	pytest-asyncio>=0.17.2
 	pytest-playwright>=0.3.0
 	pytest-xdist
 	pytest-timeout
+	pytest-rerunfailures
+	syrupy
 	psutil
 	astropy
 	suntime
 	timezonefinder
 	ipyleaflet
 	shinywidgets
 	seaborn
@@ -69,22 +72,22 @@
 	plotly
 dev = 
 	black>=23.1.0
 	flake8==3.9.2;python_version<="3.7"
 	flake8>=6.0.0;python_version>"3.7"
 	flake8-bugbear>=23.2.13
 	isort>=5.10.1
-	pyright>=1.1.244
+	pyright==1.1.311
 	pre-commit>=2.15.0
 	wheel
 	matplotlib
 	pandas
 	pandas-stubs
 	numpy
-	shinyswatch>=0.2.3
+	shinyswatch>=0.2.4
 
 [options.packages.find]
 include = shiny, shiny.*
 
 [options.package_data]
 shiny = py.typed
```

### Comparing `shiny-0.3.3/shiny/__init__.py` & `shiny-0.4.0/shiny/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A package for building reactive web applications."""
 
-__version__ = "0.3.3"
+__version__ = "0.4.0"
 
 from ._shinyenv import is_pyodide as _is_pyodide
 
 # User-facing subpackages that should be available on `from shiny import *`
 from . import reactive
 from . import render
 from .session import (
```

### Comparing `shiny-0.3.3/shiny/_app.py` & `shiny-0.4.0/shiny/_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         Whether to enable debug mode.
 
     Example
     -------
 
     .. code-block:: python
 
-        from shiny import *
+        from shiny import  App, Inputs, Outputs, Session, ui
 
         app_ui = ui.page_fluid("Hello Shiny!")
 
         def server(input: Inputs, output: Outputs, session: Session):
             pass
 
         app = App(app_ui, server)
```

### Comparing `shiny-0.3.3/shiny/_autoreload.py` & `shiny-0.4.0/shiny/_autoreload.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/_connection.py` & `shiny-0.4.0/shiny/_connection.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/_datastructures.py` & `shiny-0.4.0/shiny/_datastructures.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/_deprecated.py` & `shiny-0.4.0/shiny/_deprecated.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/_docstring.py` & `shiny-0.4.0/shiny/_docstring.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/_error.py` & `shiny-0.4.0/shiny/_error.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/_fileupload.py` & `shiny-0.4.0/shiny/_fileupload.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/_hostenv.py` & `shiny-0.4.0/shiny/_hostenv.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/_launchbrowser.py` & `shiny-0.4.0/shiny/_launchbrowser.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/_main.py` & `shiny-0.4.0/shiny/_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,20 @@
 @click.option(
     "--autoreload-port",
     type=int,
     default=0,
     help="Bind autoreload socket to this port. If 0, a random port will be used. Ignored if --reload is not used.",
     show_default=True,
 )
-@click.option("--reload", is_flag=True, default=False, help="Enable auto-reload.")
+@click.option(
+    "--reload",
+    is_flag=True,
+    default=False,
+    help="Enable auto-reload, when these types of files change: .py .css .js .html",
+)
 @click.option(
     "--ws-max-size",
     type=int,
     default=16777216,
     help="WebSocket max size message in bytes",
     show_default=True,
 )
@@ -212,47 +217,55 @@
         app, app_dir = resolve_app(app, app_dir)
 
     if app_dir:
         app_dir = os.path.realpath(app_dir)
 
     log_config: dict[str, Any] = copy.deepcopy(uvicorn.config.LOGGING_CONFIG)
 
-    if reload and app_dir is not None:
-        reload_dirs = [app_dir]
-    else:
-        reload_dirs = []
-
     if reload:
         if autoreload_port == 0:
             autoreload_port = _utils.random_port(host=host)
 
         if autoreload_port == port:
             sys.stderr.write(
                 "Autoreload port is already being used by the app; disabling autoreload\n"
             )
             reload = False
         else:
             setup_hot_reload(log_config, autoreload_port, port, launch_browser)
 
+    reload_args: dict[str, bool | str | list[str]] = {}
+    if reload:
+        reload_dirs = []
+        if app_dir is not None:
+            reload_dirs = [app_dir]
+
+        reload_args = {
+            "reload": reload,
+            # Adding `reload_includes` param while `reload=False` produces an warning
+            # https://github.com/encode/uvicorn/blob/d43afed1cfa018a85c83094da8a2dd29f656d676/uvicorn/config.py#L298-L304
+            "reload_includes": ["*.py", "*.css", "*.js", "*.html"],
+            "reload_dirs": reload_dirs,
+        }
+
     if launch_browser and not reload:
         setup_launch_browser(log_config)
 
     maybe_setup_rsw_proxying(log_config)
 
     uvicorn.run(  # pyright: ignore[reportUnknownMemberType]
         app,  # pyright: ignore[reportGeneralTypeIssues]
         host=host,
         port=port,
-        reload=reload,
-        reload_dirs=reload_dirs,
         ws_max_size=ws_max_size,
         log_level=log_level,
         log_config=log_config,
         app_dir=app_dir,
         factory=factory,
+        **reload_args,
     )
 
 
 def setup_hot_reload(
     log_config: dict[str, Any],
     autoreload_port: int,
     app_port: int,
```

### Comparing `shiny-0.3.3/shiny/_namespaces.py` & `shiny-0.4.0/shiny/_namespaces.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/_static.py` & `shiny-0.4.0/shiny/_static.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/_typing_extensions.py` & `shiny-0.4.0/shiny/_typing_extensions.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/_utils.py` & `shiny-0.4.0/shiny/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,18 +90,98 @@
     host
         Before returning a port number, ensure that we can successfully bind it on this
         host.
     n
         Number of times to attempt before giving up.
     """
 
-    # fmt: off
-    # From https://github.com/rstudio/httpuv/blob/main/R/random_port.R
-    unsafe_ports = [1, 7, 9, 11, 13, 15, 17, 19, 20, 21, 22, 23, 25, 37, 42, 43, 53, 77, 79, 87, 95, 101, 102, 103, 104, 109, 110, 111, 113, 115, 117, 119, 123, 135, 139, 143, 179, 389, 427, 465, 512, 513, 514, 515, 526, 530, 531, 532, 540, 548, 556, 563, 587, 601, 636, 993, 995, 2049, 3659, 4045, 6000, 6665, 6666, 6667, 6668, 6669, 6697]
-    # fmt: on
+    # From https://chromium.googlesource.com/chromium/src.git/+/refs/heads/master/net/base/port_util.cc
+    unsafe_ports = [
+        1,
+        7,
+        9,
+        11,
+        13,
+        15,
+        17,
+        19,
+        20,
+        21,
+        22,
+        23,
+        25,
+        37,
+        42,
+        43,
+        53,
+        69,
+        77,
+        79,
+        87,
+        95,
+        101,
+        102,
+        103,
+        104,
+        109,
+        110,
+        111,
+        113,
+        115,
+        117,
+        119,
+        123,
+        135,
+        137,
+        139,
+        143,
+        161,
+        179,
+        389,
+        427,
+        465,
+        512,
+        513,
+        514,
+        515,
+        526,
+        530,
+        531,
+        532,
+        540,
+        548,
+        554,
+        556,
+        563,
+        587,
+        601,
+        636,
+        989,
+        990,
+        993,
+        995,
+        1719,
+        1720,
+        1723,
+        2049,
+        3659,
+        4045,
+        5060,
+        5061,
+        6000,
+        6566,
+        6665,
+        6666,
+        6667,
+        6668,
+        6669,
+        6697,
+        10080,
+    ]
+
     unusable = set([x for x in unsafe_ports if x >= min and x <= max])
     while n > 0:
         if (max - min + 1) <= len(unusable):
             break
         port = random.randint(min, max)
         if port in unusable:
             continue
```

### Comparing `shiny-0.3.3/shiny/_validation.py` & `shiny-0.4.0/shiny/_validation.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/examples/Calc/app.py` & `shiny-0.4.0/shiny/examples/Calc/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 import time
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, render, ui
 
 app_ui = ui.page_fluid(
     ui.input_action_button("first", "Invalidate first (slow) computation"),
     " ",
     ui.input_action_button("second", "Invalidate second (fast) computation"),
     ui.br(),
     ui.output_ui("result"),
```

### Comparing `shiny-0.3.3/shiny/examples/Module/app.py` & `shiny-0.4.0/shiny/examples/Module/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, module, reactive, render, ui
 
 
 # ============================================================
 # Counter module
 # ============================================================
 @module.ui
 def counter_ui(label: str = "Increment counter") -> ui.TagChild:
```

### Comparing `shiny-0.3.3/shiny/examples/Progress/app.py` & `shiny-0.4.0/shiny/examples/Progress/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, render, ui
 
 app_ui = ui.page_fluid(
     ui.input_action_button("button", "Compute"),
     ui.output_text("compute"),
 )
```

### Comparing `shiny-0.3.3/shiny/examples/SilentCancelOutputException/app.py` & `shiny-0.4.0/shiny/examples/SilentCancelOutputException/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, ui
 from shiny.types import SilentCancelOutputException
 
 app_ui = ui.page_fluid(
     ui.input_text(
         "txt",
         "Delete the input text completely: it won't get removed below the input",
         "Some text",
```

### Comparing `shiny-0.3.3/shiny/examples/Value/app.py` & `shiny-0.4.0/shiny/examples/Value/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, render, ui
 
 app_ui = ui.page_fluid(
     ui.input_action_button("minus", "-1"),
     " ",
     ui.input_action_button("plus", "+1"),
     ui.br(),
     ui.output_text("value"),
```

### Comparing `shiny-0.3.3/shiny/examples/close/app.py` & `shiny-0.4.0/shiny/examples/close/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
 app_ui = ui.page_fluid(
     ui.input_action_button("close", "Close the session"),
     ui.p(
         """If this example is running on the browser (i.e., via shinylive),
         closing the session will log a message to the JavaScript console
         (open the browser's developer tools to see it).
```

### Comparing `shiny-0.3.3/shiny/examples/download/app.py` & `shiny-0.4.0/shiny/examples/download/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 import os
 from datetime import date
 from typing import Any
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-from shiny import *
-from shiny.ui import div, p
+from shiny import App, Inputs, Outputs, Session, ui
 
 
 def make_example(id: str, label: str, title: str, desc: str, extra: Any = None):
     return ui.column(
         4,
-        div(
+        ui.div(
             {"class": "card mb-4"},
-            div(title, class_="card-header"),
-            div(
+            ui.div(title, class_="card-header"),
+            ui.div(
                 {"class": "card-body"},
-                p(desc, class_="card-text text-muted"),
+                ui.p(desc, class_="card-text text-muted"),
                 extra,
                 ui.download_button(id, label, class_="btn-primary"),
             ),
         ),
     )
```

### Comparing `shiny-0.3.3/shiny/examples/download/mtcars.csv` & `shiny-0.4.0/shiny/examples/download/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/examples/download_button/app.py` & `shiny-0.4.0/shiny/examples/download_link/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import asyncio
 from datetime import date
 
 import numpy as np
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, ui
 
 app_ui = ui.page_fluid(
-    ui.download_button("downloadData", "Download"),
+    ui.download_link("downloadData", "Download"),
 )
 
 
-# For more examples of different types of download handlers, see:
-# https://github.com/rstudio/py-shiny/blob/68ffc27/examples/download/app.py#L90
 def server(input: Inputs, output: Outputs, session: Session):
     @session.download(
         filename=lambda: f"新型-{date.today().isoformat()}-{np.random.randint(100,999)}.csv"
     )
     async def downloadData():
         await asyncio.sleep(0.25)
         yield "one,two,three\n"
```

### Comparing `shiny-0.3.3/shiny/examples/download_button/mtcars.csv` & `shiny-0.4.0/shiny/examples/download_button/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/examples/download_link/mtcars.csv` & `shiny-0.4.0/shiny/examples/download_link/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/examples/dynamic_route/app.py` & `shiny-0.4.0/shiny/examples/dynamic_route/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from starlette.requests import Request
 from starlette.responses import JSONResponse
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
 app_ui = ui.page_fluid(
     ui.input_action_button("serve", "Click to serve"), ui.div(id="messages")
 )
 
 
 def server(input: Inputs, output: Outputs, session: Session):
```

### Comparing `shiny-0.3.3/shiny/examples/event/app.py` & `shiny-0.4.0/shiny/examples/event/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, render, ui
 
 app_ui = ui.page_fluid(
     ui.markdown(
         f"""
         This example demonstrates how `@reactive.event()` can be used to restrict
         execution of: (1) a `@render` function, (2) `@reactive.Calc`, or (3)
         `@reactive.Effect`.
```

### Comparing `shiny-0.3.3/shiny/examples/file_reader/mtcars.csv` & `shiny-0.4.0/shiny/examples/file_reader/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/examples/input_action_button/app.py` & `shiny-0.4.0/shiny/examples/input_action_button/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, render, ui
 
 app_ui = ui.page_fluid(
     ui.input_slider("n", "Number of observations", min=0, max=1000, value=500),
     ui.input_action_button("go", "Go!", class_="btn-success"),
     ui.output_plot("plot"),
 )
```

### Comparing `shiny-0.3.3/shiny/examples/input_action_link/app.py` & `shiny-0.4.0/shiny/examples/input_action_link/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, render, ui
 
 app_ui = ui.page_fluid(
     ui.input_slider("n", "Number of observations", min=0, max=1000, value=500),
     ui.input_action_link("go", "Go!"),
     ui.output_plot("plot"),
 )
```

### Comparing `shiny-0.3.3/shiny/examples/input_checkbox_group/app.py` & `shiny-0.4.0/shiny/examples/input_checkbox_group/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, req, ui
 
 app_ui = ui.page_fluid(
     ui.input_checkbox_group(
         "colors",
         "Choose color(s):",
         {
             "red": ui.span("Red", style="color: #FF0000;"),
```

### Comparing `shiny-0.3.3/shiny/examples/input_date/app.py` & `shiny-0.4.0/shiny/examples/input_date/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import date
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, ui
 
 app_ui = ui.page_fluid(
     ui.input_date("date1", "Date:", value="2016-02-29"),
     # Default value is the date in client's time zone
     ui.input_date("date2", "Date:"),
     # value is always yyyy-mm-dd, even if the display format is different
     ui.input_date("date3", "Date:", value="2016-02-29", format="mm/dd/yy"),
```

### Comparing `shiny-0.3.3/shiny/examples/input_date_range/app.py` & `shiny-0.4.0/shiny/examples/input_date_range/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import date
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, ui
 
 app_ui = ui.page_fluid(
     ui.input_date_range(
         "daterange1", "Date range:", start="2001-01-01", end="2010-12-31"
     ),
     # Default start and end is the current date in the client's time zone
     ui.input_date_range("daterange2", "Date range:"),
```

### Comparing `shiny-0.3.3/shiny/examples/input_file/app.py` & `shiny-0.4.0/shiny/examples/input_file/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import pandas as pd
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, ui
 from shiny.types import FileInfo
 
 app_ui = ui.page_fluid(
     ui.layout_sidebar(
         ui.panel_sidebar(
             ui.input_file("file1", "Choose CSV File", accept=[".csv"], multiple=False),
             ui.input_checkbox("header", "Header", True),
+            width=5,
         ),
-        ui.panel_main(ui.output_ui("contents")),
-    )
+        ui.panel_main(
+            ui.output_ui("contents"),
+        ),
+    ),
 )
 
 
 def server(input: Inputs, output: Outputs, session: Session):
     @output
     @render.ui
     def contents():
```

### Comparing `shiny-0.3.3/shiny/examples/input_select/app.py` & `shiny-0.4.0/shiny/examples/input_select/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, ui
 
 app_ui = ui.page_fluid(
     ui.input_select(
         "state",
         "Choose a state:",
         {
             "East Coast": {"NY": "New York", "NJ": "New Jersey", "CT": "Connecticut"},
```

### Comparing `shiny-0.3.3/shiny/examples/input_selectize/app.py` & `shiny-0.4.0/shiny/examples/input_selectize/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, ui
 
 app_ui = ui.page_fluid(
     ui.input_selectize(
         "state",
         "Choose a state:",
         {
             "East Coast": {"NY": "New York", "NJ": "New Jersey", "CT": "Connecticut"},
```

### Comparing `shiny-0.3.3/shiny/examples/input_slider/app.py` & `shiny-0.4.0/shiny/examples/input_slider/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, ui
 
 app_ui = ui.page_fluid(
     ui.input_slider("obs", "Number of bins:", min=10, max=100, value=30),
     ui.output_plot("distPlot"),
 )
```

### Comparing `shiny-0.3.3/shiny/examples/layout_sidebar/app.py` & `shiny-0.4.0/shiny/examples/row/app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, ui
 
 app_ui = ui.page_fluid(
-    ui.layout_sidebar(
-        ui.panel_sidebar(ui.input_slider("n", "N", min=0, max=100, value=20)),
-        ui.panel_main(ui.output_plot("plot")),
-    ),
+    ui.row(
+        ui.column(4, ui.input_slider("n", "N", min=0, max=100, value=20)),
+        ui.column(8, ui.output_plot("plot")),
+    )
 )
 
 
 def server(input: Inputs, output: Outputs, session: Session):
     @output
     @render.plot(alt="A histogram")
     def plot() -> object:
```

### Comparing `shiny-0.3.3/shiny/examples/nav/app.py` & `shiny-0.4.0/shiny/examples/nav/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import List
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 from shiny.types import NavSetArg
-from shiny.ui import h4
 
 
 def nav_controls(prefix: str) -> List[NavSetArg]:
     return [
         ui.nav("a", prefix + ": tab a content"),
         ui.nav("b", prefix + ": tab b content"),
         ui.nav_control(
@@ -46,23 +45,23 @@
         ui.tags.style(
             """
             h4 {
                 margin-top: 3em;
             }
             """
         ),
-        h4("navset_tab()"),
+        ui.h4("navset_tab()"),
         ui.navset_tab(*nav_controls("navset_tab()")),
-        h4("navset_pill()"),
+        ui.h4("navset_pill()"),
         ui.navset_pill(*nav_controls("navset_pill()")),
-        h4("navset_tab_card()"),
+        ui.h4("navset_tab_card()"),
         ui.navset_tab_card(*nav_controls("navset_tab_card()")),
-        h4("navset_pill_card()"),
+        ui.h4("navset_pill_card()"),
         ui.navset_pill_card(*nav_controls("navset_pill_card()")),
-        h4("navset_pill_list()"),
+        ui.h4("navset_pill_list()"),
         ui.navset_pill_list(*nav_controls("navset_pill_list()")),
     )
 )
 
 
 def server(input: Inputs, output: Outputs, session: Session):
     @reactive.Effect
```

### Comparing `shiny-0.3.3/shiny/examples/navset_hidden/app.py` & `shiny-0.4.0/shiny/examples/navset_hidden/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
 app_ui = ui.page_fluid(
     ui.layout_sidebar(
         ui.panel_sidebar(
             ui.input_radio_buttons(
                 "controller", "Controller", ["1", "2", "3"], selected="1"
             )
         ),
         ui.panel_main(
             ui.navset_hidden(
                 ui.nav(None, "Panel 1 content", value="panel1"),
                 ui.nav(None, "Panel 2 content", value="panel2"),
                 ui.nav(None, "Panel 3 content", value="panel3"),
                 id="hidden_tabs",
-            )
+            ),
         ),
     )
 )
 
 
 def server(input: Inputs, output: Outputs, session: Session):
     @reactive.Effect
```

### Comparing `shiny-0.3.3/shiny/examples/notification_show/app.py` & `shiny-0.4.0/shiny/examples/notification_show/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
 app_ui = ui.page_fluid(
     ui.input_action_button("show", "Show"),
     " ",
     ui.input_action_button("remove", "Remove"),
 )
```

### Comparing `shiny-0.3.3/shiny/examples/on_flush/app.py` & `shiny-0.4.0/shiny/examples/on_flush/app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, ui
 
 app_ui = ui.page_fluid(
     ui.input_action_button("flush", "Trigger flush"),
     ui.output_ui("n_clicks"),
     ui.div(id="flush_time"),
 )
```

### Comparing `shiny-0.3.3/shiny/examples/on_flushed/app.py` & `shiny-0.4.0/shiny/examples/on_flushed/app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, ui
 
 app_ui = ui.page_fluid(
     ui.input_action_button("flush", "Trigger flush"),
     ui.output_ui("n_clicks"),
     ui.div(id="flush_time"),
 )
```

### Comparing `shiny-0.3.3/shiny/examples/output_image/posit-logo.png` & `shiny-0.4.0/shiny/examples/output_image/posit-logo.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/examples/output_plot/app.py` & `shiny-0.4.0/shiny/examples/output_plot/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, ui
 
 app_ui = ui.page_fluid(
     ui.input_slider(
         "n", "input_slider()", min=10, max=100, value=50, step=5, animate=True
     ),
     ui.output_plot("p"),
 )
```

### Comparing `shiny-0.3.3/shiny/examples/output_table/app.py` & `shiny-0.4.0/shiny/examples/output_table/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathlib
 
 import pandas as pd
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, ui
 
 dir = pathlib.Path(__file__).parent
 mtcars = pd.read_csv(dir / "mtcars.csv")
 
 
 app_ui = ui.page_fluid(
     ui.input_checkbox("highlight", "Highlight min/max values"),
```

### Comparing `shiny-0.3.3/shiny/examples/output_table/mtcars.csv` & `shiny-0.4.0/shiny/examples/output_table/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/examples/output_text/app.py` & `shiny-0.4.0/shiny/examples/output_text/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, ui
 
 app_ui = ui.page_fluid(
     ui.input_text("txt", "Enter the text to display below:"),
     ui.row(
         ui.column(6, ui.output_text("text")),
         ui.column(6, ui.output_text_verbatim("verb", placeholder=True)),
     ),
```

### Comparing `shiny-0.3.3/shiny/examples/panel_conditional/app.py` & `shiny-0.4.0/shiny/examples/panel_conditional/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, ui
 
 app_ui = ui.page_fluid(
     ui.input_checkbox("show", "Show radio buttons", False),
     ui.panel_conditional(
         "input.show", ui.input_radio_buttons("radio", "Choose ", ["slider", "select"])
     ),
     ui.panel_conditional(
```

### Comparing `shiny-0.3.3/shiny/examples/poll/app.py` & `shiny-0.4.0/shiny/examples/poll/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import random
 import sqlite3
 from datetime import datetime
 from typing import Any, Awaitable
 
 import pandas as pd
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, render, ui
 
 SYMBOLS = ["AAA", "BBB", "CCC", "DDD", "EEE", "FFF"]
 
 
 def timestamp() -> str:
     return datetime.now().strftime("%x %X")
```

### Comparing `shiny-0.3.3/shiny/examples/req/app.py` & `shiny-0.4.0/shiny/examples/req/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, render, req, ui
 from shiny.types import SafeException
 
 app_ui = ui.page_fluid(
     ui.input_action_button("safe", "Throw a safe error"),
     ui.output_ui("safe"),
     ui.input_action_button("unsafe", "Throw an unsafe error"),
     ui.output_ui("unsafe"),
```

### Comparing `shiny-0.3.3/shiny/examples/row/app.py` & `shiny-0.4.0/shiny/examples/layout_sidebar/app.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, render, ui
 
 app_ui = ui.page_fluid(
-    ui.row(
-        ui.column(4, ui.input_slider("n", "N", min=0, max=100, value=20)),
-        ui.column(8, ui.output_plot("plot")),
-    )
+    ui.layout_sidebar(
+        ui.panel_sidebar(
+            ui.input_slider("n", "N", min=0, max=100, value=20),
+        ),
+        ui.panel_main(
+            ui.output_plot("plot"),
+        ),
+    ),
 )
 
 
 def server(input: Inputs, output: Outputs, session: Session):
     @output
     @render.plot(alt="A histogram")
     def plot() -> object:
```

### Comparing `shiny-0.3.3/shiny/examples/send_custom_message/app.py` & `shiny-0.4.0/shiny/examples/send_custom_message/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
 app_ui = ui.page_fluid(
     ui.input_text("msg", "Enter a message"),
     ui.input_action_button("submit", "Submit the message"),
     # It'd be better to use ui.insert_ui() in order to implement this kind of
     # functionality...this is just a basic demo of how custom message handling works.
     ui.tags.div(id="messages"),
```

### Comparing `shiny-0.3.3/shiny/examples/update_action_button/app.py` & `shiny-0.4.0/shiny/examples/update_action_button/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from htmltools import br
-
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, req, ui
 
 app_ui = ui.page_fluid(
     ui.input_action_button("update", "Update other buttons and link"),
-    br(),
+    ui.br(),
     ui.input_action_button("goButton", "Go"),
-    br(),
+    ui.br(),
     ui.input_action_button("goButton2", "Go 2", icon="🤩"),
-    br(),
+    ui.br(),
     ui.input_action_button("goButton3", "Go 3"),
-    br(),
+    ui.br(),
     ui.input_action_link("goLink", "Go Link"),
 )
 
 
 def server(input: Inputs, output: Outputs, session: Session):
     @reactive.Effect
     def _():
```

### Comparing `shiny-0.3.3/shiny/examples/update_checkbox_group/app.py` & `shiny-0.4.0/shiny/examples/update_checkbox_group/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
 app_ui = ui.page_fluid(
     ui.tags.p("The first checkbox group controls the second"),
     ui.input_checkbox_group(
         "inCheckboxGroup", "Input checkbox", ["Item A", "Item B", "Item C"]
     ),
     ui.input_checkbox_group(
```

### Comparing `shiny-0.3.3/shiny/examples/update_date/app.py` & `shiny-0.4.0/shiny/examples/update_date/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import date, timedelta
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
 app_ui = ui.page_fluid(
     ui.input_slider("n", "Day of month", min=1, max=30, value=10),
     ui.input_date("inDate", "Input date"),
 )
```

### Comparing `shiny-0.3.3/shiny/examples/update_date_range/app.py` & `shiny-0.4.0/shiny/examples/update_date_range/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import date, timedelta
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
 app_ui = ui.page_fluid(
     ui.input_slider("n", "Day of month", min=1, max=30, value=10),
     ui.input_date_range("inDateRange", "Input date"),
 )
```

### Comparing `shiny-0.3.3/shiny/examples/update_navs/app.py` & `shiny-0.4.0/shiny/examples/update_navs/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
-app_ui = ui.page_fluid(
+app_ui = ui.page_fixed(
     ui.layout_sidebar(
         ui.panel_sidebar(
             ui.input_slider("controller", "Controller", min=1, max=3, value=1)
         ),
         ui.panel_main(
             ui.navset_tab_card(
                 ui.nav("Panel 1", "Panel 1 content", value="panel1"),
                 ui.nav("Panel 2", "Panel 2 content", value="panel2"),
                 ui.nav("Panel 3", "Panel 3 content", value="panel3"),
                 id="inTabset",
-            )
+            ),
         ),
     )
 )
 
 
 def server(input: Inputs, output: Outputs, session: Session):
     @reactive.Effect
```

### Comparing `shiny-0.3.3/shiny/examples/update_numeric/app.py` & `shiny-0.4.0/shiny/examples/update_numeric/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
 app_ui = ui.page_fluid(
     ui.input_slider("controller", "Controller", min=0, max=20, value=10),
     ui.input_numeric("inNumber", "Input number", 0),
     ui.input_numeric("inNumber2", "Input number 2", 0),
 )
```

### Comparing `shiny-0.3.3/shiny/examples/update_radio_buttons/app.py` & `shiny-0.4.0/shiny/examples/update_radio_buttons/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
 app_ui = ui.page_fluid(
     ui.tags.p("The first radio button group controls the second"),
     ui.input_radio_buttons(
         "inRadioButtons", "Input radio buttons", ["Item A", "Item B", "Item C"]
     ),
     ui.input_radio_buttons(
```

### Comparing `shiny-0.3.3/shiny/examples/update_select/app.py` & `shiny-0.4.0/shiny/examples/update_select/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
 app_ui = ui.page_fluid(
     ui.tags.p("The checkbox group controls the select input"),
     ui.input_checkbox_group(
         "inCheckboxGroup", "Input checkbox", ["Item A", "Item B", "Item C"]
     ),
     ui.input_select("inSelect", "Select input", ["Item A", "Item B", "Item C"]),
```

### Comparing `shiny-0.3.3/shiny/examples/update_slider/app.py` & `shiny-0.4.0/shiny/examples/update_slider/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
-app_ui = ui.page_fluid(
+app_ui = ui.page_fixed(
     ui.layout_sidebar(
         ui.panel_sidebar(
             ui.tags.p("The first slider controls the second"),
             ui.input_slider("control", "Controller:", min=0, max=20, value=10, step=1),
             ui.input_slider("receive", "Receiver:", min=0, max=20, value=10, step=1),
         ),
-        ui.panel_main(),
+        ui.panel_main("Main app content"),
     )
 )
 
 
 def server(input: Inputs, output: Outputs, session: Session):
     @reactive.Effect
     def _():
```

### Comparing `shiny-0.3.3/shiny/examples/update_text/app.py` & `shiny-0.4.0/shiny/examples/update_text/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, reactive, ui
 
 app_ui = ui.page_fluid(
     ui.input_slider("controller", "Controller", min=0, max=20, value=10),
     ui.input_text("inText", "Input text"),
     ui.input_text("inText2", "Input text 2"),
 )
```

### Comparing `shiny-0.3.3/shiny/examples/www_dir/app.py` & `shiny-0.4.0/shiny/examples/www_dir/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, ui
 
 app_ui = ui.page_fluid(
     ui.tags.link(href="css/styles.css", rel="stylesheet"),
     ui.tags.div(
         "If you see this text, it failed",
         id="target",
         style="background-color: red;",
```

### Comparing `shiny-0.3.3/shiny/experimental/ui/_css.py` & `shiny-0.4.0/shiny/ui/_x/_css_unit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 from __future__ import annotations
 
-import numbers
 from typing import Union, overload
 
+__all__ = (
+    "CssUnit",
+    "as_css_unit",
+    "as_css_padding",
+)
+
 CssUnit = Union[
-    # TODO: pylance really doesn't like `numbers.Number`.
-    #       Instead, use `int` and `float`
     int,
     float,
     str,
 ]
 
 
 @overload
-def trinary(x: None) -> None:
+def as_css_unit(value: None) -> None:
     ...
 
 
 @overload
-def trinary(x: bool | str) -> str:
+def as_css_unit(value: CssUnit) -> str:
     ...
 
 
-def trinary(x: bool | str | None) -> None | str:
-    if x is None:
-        return None
-    elif x:
-        return "true"
+def as_css_unit(value: None | CssUnit) -> None | str:
+    # TODO-future: Actually validate. Or don't validate, but then change
+    # the function name to to_css_unit() or something.
+    if isinstance(value, (float, int)):
+        # Explicit check for 0 because floats may format to have many decimals.
+        if value == 0:
+            return "0"
+        return "{:f}px".format(value)
     else:
-        return "false"
+        return value
 
 
 @overload
-def validate_css_unit(value: None) -> None:
+def as_css_padding(padding: CssUnit | list[CssUnit]) -> str:
     ...
 
 
 @overload
-def validate_css_unit(value: CssUnit) -> str:
+def as_css_padding(padding: None) -> None:
     ...
 
 
-def validate_css_unit(value: None | CssUnit) -> None | str:
-    # TODO-future: Actually validate. Or don't validate, but then change
-    # the function name to to_css_unit() or something.
-    # TODO-future: pylance can't figure out if an `int` or `float` is a `numbers.Number` (which
-    # is it). For now, use the extra types
-    if (
-        isinstance(value, numbers.Number)
-        or isinstance(value, float)
-        or isinstance(value, int)
-    ):
-        # Explicit check for 0 because floats may format to have many decimals.
-        if value == 0:
-            return "0"
-        return "{:f}px".format(value)
-    else:
-        return value
+def as_css_padding(padding: CssUnit | list[CssUnit] | None) -> str | None:
+    if padding is None:
+        return None
+
+    if not isinstance(padding, list):
+        padding = [padding]
+
+    return " ".join(as_css_unit(p) for p in padding)
+
+
+# It seems to be to use % over fr here since there is no gap on the grid
+def to_width_unit(x: str | float | int) -> str:
+    if isinstance(x, (int, float)):
+        return as_css_unit(x)
+
+    if isinstance(x, str) and x.endswith("%") and x.count("%") == 1:
+        x1_num = float(x[:-1])
+        x2_num = 100 - x1_num
+        return f"{x1_num}% {x2_num}%"
+
+    # TODO-bslib: validateCssUnit() should maybe support fr units?
+    # return(paste(x, collapse = " "))
+    return as_css_unit(x)
```

### Comparing `shiny-0.3.3/shiny/experimental/ui/_htmldeps.py` & `shiny-0.4.0/shiny/ui/_x/_htmldeps.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 from __future__ import annotations
 
 from pathlib import PurePath
 
 from htmltools import HTMLDependency
 
-from shiny import __version__ as shiny_package_version
+from ..._versions import bslib as bslib_version
+from ..._versions import htmltools as htmltools_version
 
-ex_www_path = PurePath(__file__).parent.parent / "www"
+_x_www = PurePath(__file__).parent.parent.parent / "www" / "shared" / "_x"
+_x_components_path = str(_x_www / "bslib" / "components")
+_x_fill_path = str(_x_www / "htmltools" / "fill")
 
 
-def card_full_screen_dep() -> HTMLDependency:
-    return HTMLDependency(
-        name="bslib-card-full-screen",
-        version=shiny_package_version,
-        source={
-            "package": "shiny",
-            "subdir": str(ex_www_path),
-        },
-        script={"src": "card-full-screen.js"},
-    )
-
-
-def fill_dependencies() -> HTMLDependency:
+def fill_dependency() -> HTMLDependency:
     return HTMLDependency(
         "htmltools-fill",
-        "0.0.0.0",
+        htmltools_version,
         source={
             "package": "shiny",
-            "subdir": str(ex_www_path),
+            "subdir": _x_fill_path,
         },
         stylesheet={"href": "fill.css"},
     )
 
 
 def sidebar_dependency() -> HTMLDependency:
     return HTMLDependency(
-        "bslib-sidebar-x",
-        "0.0.0",
+        "bslib-sidebar",
+        bslib_version,
         source={
             "package": "shiny",
-            "subdir": str(ex_www_path / "sidebar"),
+            "subdir": _x_components_path,
         },
         script={"src": "sidebar.min.js"},
     )
```

### Comparing `shiny-0.3.3/shiny/experimental/ui/_input_text.py` & `shiny-0.4.0/shiny/experimental/ui/_input_text.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 __all__ = ("input_text_area",)
 
-from pathlib import PurePath
 from typing import Optional
 
-from htmltools import HTMLDependency, Tag, TagChild, css, div, tags
+from htmltools import Tag, TagChild, css, div, tags
 
-from ..._docstring import add_example
+# from ..._docstring import add_example
 from ..._namespaces import resolve_id
 from ..._typing_extensions import Literal
+from ...ui._utils import shiny_input_label
+from ._htmldeps import autoresize_dependency
 
 
-@add_example()
+# TODO-maindocs;
+# @add_example()
 def input_text_area(
     id: str,
     label: TagChild,
     value: str = "",
     *,
     width: Optional[str] = None,
     height: Optional[str] = None,
@@ -106,30 +108,11 @@
         autocomplete=autocomplete,
         spellcheck=spellcheck,
     )
 
     return div(
         shiny_input_label(id, label),
         area,
-        _autoresize_dependency() if autoresize else None,
+        autoresize_dependency() if autoresize else None,
         class_="form-group shiny-input-container",
         style=css(width=width),
     )
-
-
-ex_www_path = PurePath(__file__).parent.parent / "www"
-
-
-def _autoresize_dependency():
-    return HTMLDependency(
-        "shiny-textarea-autoresize",
-        "0.0.0",
-        source={"package": "shiny", "subdir": str(ex_www_path)},
-        script={"src": "textarea-autoresize.js"},
-        stylesheet={"href": "textarea-autoresize.css"},
-    )
-
-
-# Originally from ui._utils, but we can't seem to import ..ui._utils
-def shiny_input_label(id: str, label: TagChild = None) -> Tag:
-    cls = "control-label" + ("" if label else " shiny-label-null")
-    return tags.label(label, class_=cls, id=id + "-label", for_=id)
```

### Comparing `shiny-0.3.3/shiny/experimental/ui/_layout.py` & `shiny-0.4.0/shiny/experimental/ui/_layout.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,128 +1,127 @@
 from __future__ import annotations
 
-# import pdb
 from typing import Optional
 
-from htmltools import TagAttrValue, TagChild, css, div
+from htmltools import TagAttrs, TagAttrValue, TagChild, css, div
 
-from shiny._typing_extensions import Literal
+from ..._typing_extensions import Literal
+from ._css_unit import CssUnit, as_css_unit
+from ._fill import as_fill_item, as_fillable_container
+from ._utils import consolidate_attrs, is_01_scalar
 
-from ._css import CssUnit, validate_css_unit
-from ._fill import bind_fill_role
 
-
-# A grid-like, column-first, layout
-#
-# Wraps a 1d sequence of UI elements into a 2d grid. The number of columns (and
-# rows) in the grid dependent on the column `width` as well as the size of the
-# display. For more explanation and illustrative examples, see [here](https://rstudio.github.io/bslib/articles/cards.html#multiple-cards)
-#
-# @param ... Unnamed arguments should be UI elements (e.g., [card()])
-#   Named arguments become attributes on the containing [htmltools::tag] element.
-# @param width The desired width of each card, which can be any of the
-#  following:
-#   * A (unit-less) number between 0 and 1.
-#     * This should be specified as `1/num`, where `num` represents the number
-#       of desired columns.
-#   * A [CSS length unit][htmltools::validateCssUnit()]
-#     * Either the minimum (when `fixed_width=FALSE`) or fixed width
-#       (`fixed_width=TRUE`).
-#   * `NULL`
-#     * Allows power users to set the `grid-template-columns` CSS property
-#       manually, either via a `style` attribute or a CSS stylesheet.
-# @param fixed_width Whether or not to interpret the `width` as a minimum
-#   (`fixed_width=FALSE`) or fixed (`fixed_width=TRUE`) width when it is a CSS
-#   length unit.
-# @param heights_equal If `"all"` (the default), every card in every row of the
-#   grid will have the same height. If `"row"`, then every card in _each_ row
-#   of the grid will have the same height, but heights may vary between rows.
-# @param fill Whether or not to allow the layout to grow/shrink to fit a
-#   fillable container with an opinionated height (e.g., `page_fillable()`).
-# @param fillable Whether or not each element is wrapped in a fillable container.
-# @param height_mobile Any valid CSS unit to use for the height when on mobile
-#   devices (or narrow windows).
-# @inheritParams card
-# @inheritParams card_body
-#
-# @export
-# @examples
-#
-# x <- card("A simple card")
-# # Always has 2 columns (on non-mobile)
-# layout_column_wrap(1/2, x, x, x)
-# # Has three columns when viewport is wider than 750px
-# layout_column_wrap("250px", x, x, x)
-#
 def layout_column_wrap(
     width: Optional[CssUnit],
-    *args: TagChild,  # `TagAttrs` are not allowed here
+    *args: TagChild | TagAttrs,
     fixed_width: bool = False,
     heights_equal: Literal["all", "row"] = "all",
     fill: bool = True,
     fillable: bool = True,
     height: Optional[CssUnit] = None,
     height_mobile: Optional[CssUnit] = None,
     gap: Optional[CssUnit] = None,
-    class_: Optional[str] = None,  # Applies after `bind_fill_role()`
+    class_: Optional[str] = None,
     **kwargs: TagAttrValue,
 ):
-    attribs = kwargs
-    children = args
+    # For
+    # more explanation and illustrative examples, see
+    # [here](https://rstudio.github.io/bslib/articles/cards.html#multiple-cards)
+    """
+    A grid-like, column-first layout
+
+    Wraps a 1d sequence of UI elements into a 2d grid. The number of columns (and rows)
+    in the grid dependent on the column `width` as well as the size of the display.
+
+    Parameters
+    ----------
+    width
+        The desired width of each card, which can be any of the following:
+        * A (unit-less) number between 0 and 1.
+            * This should be specified as `1/num`, where `num` represents the number
+            of desired columns.
+        * A CSS length unit
+            * Either the minimum (when `fixed_width=False`) or fixed width
+            (`fixed_width=True`).
+        * `None`
+            * Allows power users to set the `grid-template-columns` CSS property
+            manually, either via a `style` attribute or a CSS stylesheet.
+    *args
+        Unnamed arguments should be UI elements (e.g., [card()]). Named arguments become
+        attributes on the containing [htmltools::tag] element.
+    fixed_width
+        Whether or not to interpret the `width` as a minimum (`fixed_width=False`) or
+        fixed (`fixed_width=True`) width when it is a CSS length unit.
+    heights_equal
+        If `"all"` (the default), every card in every row of the grid will have the same
+        height. If `"row"`, then every card in _each_ row of the grid will have the same
+        height, but heights may vary between rows.
+    fill
+        Whether or not to allow the layout to grow/shrink to fit a fillable container
+        with an opinionated height (e.g., `page_fillable()`).
+    fillable
+        Whether or not each element is wrapped in a fillable container.
+    height
+        Any valid CSS unit to use for the height.
+    height_mobile
+        Any valid CSS unit to use for the height when on mobile devices (or narrow
+        windows).
+    gap
+        Any valid CSS unit to use for the gap between columns.
+    class_
+        A CSS class to apply to the containing element.
+    **kwargs
+        Additional attributes to apply to the containing element.
+
+
+    """
+    attrs, children = consolidate_attrs(*args, class_=class_, **kwargs)
 
     colspec: str | None = None
     if width is not None:
-        width_num = float(width)
-        if width_num > 0.0 and width_num <= 1.0:
-            num_cols = 1.0 / width_num
+        if is_01_scalar(width) and width > 0.0:
+            num_cols = 1.0 / width
             if not num_cols.is_integer():
                 raise ValueError(
-                    "Could not interpret width argument; see ?layout_column_wrap"
+                    "Could not interpret `layout_column_wrap(width=)` argument"
                 )
             colspec = " ".join(["1fr" for _ in range(int(num_cols))])
         else:
-            width_css_unit = validate_css_unit(width)
+            width_css_unit = as_css_unit(width)
             if fixed_width:
                 colspec = f"repeat(auto-fit, minmax({width_css_unit}, 1fr))"
             else:
                 colspec = f"repeat(auto-fit, minmax(0, {width_css_unit}))"
 
     # Use a new dict so that we don't mutate the original `children` dict
     upgraded_children: list[TagChild] = []
     for child_value in children:
-        upgraded_children.append(
-            bind_fill_role(
-                div(bind_fill_role(div(child_value), container=fillable, item=True)),
-                container=True,
-            )
-        )
+        child = div({"class": "bslib-gap-spacing"}, child_value)
+        if fillable:
+            child = as_fillable_container(child)
+        upgraded_children.append(child)
+
     tag_style_css = {
         "grid-template-columns": colspec,
         "grid-auto-rows": "1fr" if (heights_equal == "all") else None,
         # Always provide the `height:auto` default so that the CSS variable
         # doesn't get inherited in a scenario like
         # layout_column_wrap(height=200, layout, layout_column_wrap(...))
-        "--bslib-column-wrap-height": validate_css_unit(
-            "auto" if height is None else height
-        ),
-        "--bslib-column-wrap-height-mobile": validate_css_unit(
+        "--bslib-grid-height": as_css_unit("auto" if height is None else height),
+        "--bslib-grid-height-mobile": as_css_unit(
             "auto" if height_mobile is None else height_mobile
         ),
-        "gap": validate_css_unit(gap),
+        "gap": as_css_unit(gap),
     }
 
     tag = div(
         {
-            "class": "bslib-column-wrap",
+            "class": "bslib-grid",
             "style": css(**tag_style_css),
         },
+        attrs,
         *upgraded_children,
-        **attribs,
     )
-    # pdb.set_trace()
-
-    tag = bind_fill_role(tag, item=fill)
-    # Give the user an opportunity to override the classes added by bind_fill_role()
-    if class_ is not None:
-        tag.add_class(class_)
+    if fill:
+        tag = as_fill_item(tag)
 
     return tag
```

### Comparing `shiny-0.3.3/shiny/experimental/ui/_output.py` & `shiny-0.4.0/shiny/experimental/ui/_output.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 
 from __future__ import annotations
 
 from typing import Optional
 
 from htmltools import Tag, TagAttrValue, TagFunction, css, div, tags
 
-from shiny._docstring import add_example
-from shiny._namespaces import resolve_id
-from shiny.types import MISSING, MISSING_TYPE
-from shiny.ui._plot_output_opts import (
+from ..._docstring import add_example
+from ..._namespaces import resolve_id
+from ...types import MISSING, MISSING_TYPE
+from ...ui._plot_output_opts import (
     BrushOpts,
     ClickOpts,
     DblClickOpts,
     HoverOpts,
     brush_opts,
     click_opts,
     dblclick_opts,
     format_opt_names,
     hover_opts,
 )
-
-from ._fill import bind_fill_role
+from ._fill import as_fill_item, as_fillable_container
 
 
 @add_example()
 def output_plot(
     id: str,
     width: str = "100%",
     height: str = "400px",
@@ -89,15 +88,16 @@
     Returns
     -------
     :
         A UI element
 
     See Also
     -------
-    ~shiny.render.plot ~shiny.ui.output_image
+    * :func:`~shiny.render.plot`
+    * :func:`~shiny.ui.output_image`
     """
 
     # NEW
     if isinstance(fill, MISSING_TYPE):
         fill = not inline
     # /NEW
 
@@ -219,17 +219,18 @@
 
     container = func(
         id=id_resolved,
         class_="shiny-image-output",
         style=style,
         **args,
     )
-    # NEW
-    return bind_fill_role(container, item=fill)
-    # /NEW
+    if fill:
+        container = as_fill_item(container)
+
+    return container
 
 
 @add_example()
 def output_ui(
     id: str,
     inline: bool = False,
     container: Optional[TagFunction] = None,
@@ -267,14 +268,14 @@
     if not container:
         container = tags.span if inline else tags.div
     res = container(
         {"class": "shiny-html-output"},
         id=resolve_id(id),
         **kwargs,
     )
-    return bind_fill_role(
-        res,
-        # NEW
-        item=bool(fill),
-        container=bool(fillable),
-        # /NEW
-    )
+
+    if fillable:
+        res = as_fillable_container(res)
+    if fill:
+        res = as_fill_item(res)
+
+    return res
```

### Comparing `shiny-0.3.3/shiny/experimental/ui/_sidebar.py` & `shiny-0.4.0/shiny/ui/_x/_sidebar.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,207 +1,250 @@
 from __future__ import annotations
 
-import numbers
 import random
 from typing import Optional
 
-from htmltools import Tag, TagAttrs, TagChild, css, div
+from htmltools import Tag, TagAttrs, TagAttrValue, TagChild, TagList, css, div
 from htmltools import svg as svgtags
 from htmltools import tags
 
-from shiny._typing_extensions import Literal
+from ..._typing_extensions import Literal
 
-from ._color import get_color_contrast
-from ._css import CssUnit, trinary, validate_css_unit
-from ._fill import bind_fill_role
+# from ._color import get_color_contrast
+from ._css_unit import CssUnit, as_css_padding, as_css_unit
+from ._fill import as_fill_item, as_fillable_container
 from ._htmldeps import sidebar_dependency
+from ._utils import consolidate_attrs, trinary
 
 
 class Sidebar:
     def __init__(
         self,
         tag: Tag,
         collapse_tag: Optional[Tag],
         position: Literal["left", "right"],
         open: Literal["desktop", "open", "closed", "always"],
-        width: int,
+        width: CssUnit,
         max_height_mobile: Optional[str | float],
+        color_fg: Optional[str],
+        color_bg: Optional[str],
     ):
         self.tag = tag
         self.collapse_tag = collapse_tag
         self.position = position
         self.open = open
         self.width = width
         self.max_height_mobile = max_height_mobile
+        self.color_fg = color_fg
+        self.color_bg = color_bg
+
+    # # This does not contain the `collapse_tag`
+    # # The `Sidebar` class should use it's fields, not this method
+    # def tagify(self) -> Tag:
+    #     return self.tag.tagify()
 
 
 def sidebar(
     *args: TagChild | TagAttrs,
-    width: int = 250,
+    width: CssUnit = 250,
     position: Literal["left", "right"] = "left",
     open: Literal["desktop", "open", "closed", "always"] = "desktop",
     id: Optional[str] = None,
-    title: TagChild | str | numbers.Number = None,
+    title: TagChild | str = None,
     bg: Optional[str] = None,
     fg: Optional[str] = None,
     class_: Optional[str] = None,  # TODO-future; Consider using `**kwargs` instead
     max_height_mobile: Optional[str | float] = None,
 ) -> Sidebar:
-    # TODO: validate `open`, bg, fg, class_, max_height_mobile
-    # TODO: Add type annotations
+    # See [this article](https://rstudio.github.io/bslib/articles/sidebars.html)
+    #   to learn more.
+    # TODO-future; If color contrast is implemented. Docs for `bg` and `fg`:
+    #     If only one of either is provided, an
+    #     accessible contrasting color is provided for the opposite color, e.g. setting
+    #     `bg` chooses an appropriate `fg` color.
+    # TODO-future; validate `open`, bg, fg, class_, max_height_mobile
 
     if id is None and open != "always":
         # but always provide id when collapsible for accessibility reasons
         id = f"bslib-sidebar-{random.randint(1000, 10000)}"
 
-    if fg is None and bg is not None:
-        fg = get_color_contrast(bg)
-    if bg is None and fg is not None:
-        bg = get_color_contrast(fg)
+    # TODO-future; implement
+    # if fg is None and bg is not None:
+    #     fg = get_color_contrast(bg)
+    # if bg is None and fg is not None:
+    #     bg = get_color_contrast(fg)
 
-    if isinstance(title, str) or isinstance(title, numbers.Number):
+    if isinstance(title, (str, int, float)):
         title = div(str(title), class_="sidebar-title")
 
     collapse_tag = None
+    # Code
     if open != "always":
         collapse_tag = tags.button(
-            collapse_icon(),
+            _collapse_icon(),
             class_="collapse-toggle",
             type="button",
             title="Toggle sidebar",
-            style=css(background_color=bg, color=fg),
             aria_expanded=trinary(open in ["open", "desktop"]),
             aria_controls=id,
         )
 
     tag = div(
-        div(title, *args, class_="sidebar-content"),
+        div(
+            title,
+            {"class": "sidebar-content"},
+            *args,
+        ),
         {"class": "bslib-sidebar-input"} if id is not None else None,
         {"class": "sidebar"},
         id=id,
         role="complementary",
         class_=class_,
-        style=css(background_color=bg, color=fg),
     )
 
     return Sidebar(
         tag=tag,
         collapse_tag=collapse_tag,
         position=position,
         open=open,
         width=width,
         max_height_mobile=max_height_mobile,
+        color_fg=fg,
+        color_bg=bg,
     )
 
 
-def collapse_icon() -> Tag:
-    return tags.svg(
-        svgtags.path(
-            fill_rule="evenodd",
-            d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z",
-        ),
-        xmlns="http://www.w3.org/2000/svg",
-        viewBox="0 0 16 16",
-        class_="bi bi-chevron-down collapse-icon",
-        style="fill:currentColor;",
-        aria_hidden="true",
-        role="img",
-    )
-
-
+# TODO-maindocs; @add_example()
 def layout_sidebar(
     sidebar: Sidebar,
-    *args: TagChild | TagAttrs,
-    fillable: bool = False,
+    content: PanelMain,
+    fillable: bool = True,
     fill: bool = True,
     bg: Optional[str] = None,
     fg: Optional[str] = None,
-    border: Optional[str] = None,
+    border: Optional[bool] = None,
     border_radius: Optional[bool] = None,
     border_color: Optional[str] = None,
+    gap: Optional[CssUnit] = None,
+    padding: Optional[CssUnit | list[CssUnit]] = None,
     height: Optional[CssUnit] = None,
+    **kwargs: TagAttrValue,
 ) -> Tag:
-    # TODO: validate sidebar object, border, border_radius, colors
-
-    if fg is None and bg is not None:
-        fg = get_color_contrast(bg)
-    if bg is None and fg is not None:
-        bg = get_color_contrast(fg)
+    attrs, _ = consolidate_attrs(**content.attrs, **kwargs)
 
     main = div(
-        *args,
-        role="main",
-        class_="main",
-        style=css(background_color=bg, color=fg),
+        {
+            "role": "main",
+            "class": f"main{' bslib-gap-spacing' if fillable else ''}",
+            ""
+            "style": css(
+                background_color=bg,
+                color=fg,
+                gap=as_css_unit(gap),
+                padding=as_css_padding(padding),
+            ),
+        },
+        attrs,
+        content,
     )
-
-    main = bind_fill_role(main, container=fillable)
-
-    contents = [main, sidebar.tag, sidebar.collapse_tag]
-
-    right = sidebar.position == "right"
+    if fillable:
+        main = as_fillable_container(main)
 
     max_height_mobile = sidebar.max_height_mobile or (
         "250px" if height is None else "50%"
     )
 
     res = div(
-        sidebar_dependency(),
-        sidebar_js_init(),
         {"class": "bslib-sidebar-layout"},
-        {"class": "sidebar-right"} if right else None,
+        {"class": "sidebar-right"} if sidebar.position == "right" else None,
         {"class": "sidebar-collapsed"} if sidebar.open == "closed" else None,
-        *contents,
-        data_sidebar_init_auto_collapse="true" if sidebar.open == "desktop" else None,
+        main,
+        sidebar.tag,
+        sidebar.collapse_tag,
+        sidebar_dependency(),
+        _sidebar_init_js(),
+        data_bslib_sidebar_init="true" if sidebar.open != "always" else None,
+        data_bslib_sidebar_open=sidebar.open,
         data_bslib_sidebar_border=trinary(border),
         data_bslib_sidebar_border_radius=trinary(border_radius),
         style=css(
-            __bslib_sidebar_width=validate_css_unit(sidebar.width),
+            __bslib_sidebar_width=as_css_unit(sidebar.width),
+            __bslib_sidebar_bg=as_css_unit(sidebar.color_bg),
+            __bslib_sidebar_fg=as_css_unit(sidebar.color_fg),
             __bs_card_border_color=border_color,
-            height=validate_css_unit(height),
-            __bslib_sidebar_max_height_mobile=validate_css_unit(max_height_mobile),
+            height=as_css_unit(height),
+            __bslib_sidebar_max_height_mobile=as_css_unit(max_height_mobile),
         ),
     )
+    if fill:
+        res = as_fill_item(res)
 
-    res = bind_fill_role(res, item=fill)
-
-    # res <- as.card_item(res)
-    # as_fragment(
-    #     tag_require(res, version = 5, caller = "layout_sidebar()")
-    # )
     return res
 
 
-def sidebar_js_init() -> Tag:
+# _sidebar_func = sidebar
+
+
+def _collapse_icon() -> Tag:
+    return tags.svg(
+        svgtags.path(
+            fill_rule="evenodd",
+            d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z",
+        ),
+        xmlns="http://www.w3.org/2000/svg",
+        viewBox="0 0 16 16",
+        class_="bi bi-chevron-down collapse-icon",
+        style="fill:currentColor;",
+        aria_hidden="true",
+        role="img",
+    )
+
+
+def _sidebar_init_js() -> Tag:
+    # Note: if we want to avoid inline `<script>` tags in the future for
+    # initialization code, we might be able to do so by turning the sidebar layout
+    # container into a web component
     return tags.script(
-        {"data_bslib_sidebar_init": True},
-        """
-        var thisScript = document.querySelector('script[data-bslib-sidebar-init]');
-        thisScript.removeAttribute('data-bslib-sidebar-init');
-
-        // If this layout is the innermost layout, then allow it to add CSS
-        // variables to it and its ancestors (counting how parent layouts there are)
-        var thisLayout = $(thisScript).parent();
-        var noChildLayouts = thisLayout.find('.bslib-sidebar-layout').length === 0;
-        if (noChildLayouts) {
-        var parentLayouts = thisLayout.parents('.bslib-sidebar-layout');
-        // .add() sorts the layouts in DOM order (i.e., innermost is last)
-        var layouts = thisLayout.add(parentLayouts);
-        var ctrs = {left: 0, right: 0};
-        layouts.each(function(i, x) {
-            $(x).css('--bslib-sidebar-counter', i);
-            var right = $(x).hasClass('sidebar-right');
-            $(x).css('--bslib-sidebar-overlap-counter', right ? ctrs.right : ctrs.left);
-            right ? ctrs.right++ : ctrs.left++;
-        });
-        }
-
-        // If sidebar is marked open='desktop', collapse sidebar if on mobile
-        if (thisLayout.data('sidebarInitAutoCollapse')) {
-        var initCollapsed = thisLayout.css('--bslib-sidebar-js-init-collapsed');
-        if (initCollapsed === 'true') {
-            thisLayout.addClass('sidebar-collapsed');
-            thisLayout.find('.collapse-toggle').attr('aria-expanded', 'false');
-        }
-        }
-        """,
+        {"data-bslib-sidebar-init": True},
+        "bslib.Sidebar.initCollapsibleAll()",
     )
+
+
+###################################################################
+
+
+class PanelSidebar:
+    # Store `attrs` for `layout_sidebar()` to retrieve
+    def __init__(
+        self, *args: TagChild | TagAttrs, width: int = 4, **kwargs: TagAttrValue
+    ) -> None:
+        self.args = args
+        self.kwargs = kwargs
+        self.width = width
+
+    def get_sidebar(self, position: Literal["left", "right"] = "left") -> Sidebar:
+        return sidebar(
+            *self.args,
+            width=f"{int(self.width / 12 * 100)}%",
+            position=position,
+            open="always",
+            **self.kwargs,
+        )
+
+    # Hopefully this is never used. But it makes it Tagifiable to allow us to not expose
+    # `Sidebar` and `PanelSidebar` classes
+    def tagify(self) -> Tag:
+        return self.get_sidebar().tag.tagify()
+
+
+class PanelMain:
+    # Store `attrs` for `layout_sidebar()` to retrieve
+    attrs: TagAttrs
+    # Return `children` in `layout_sidebar()` via `.tagify()` method
+    children: list[TagChild]
+
+    def __init__(self, *, attrs: TagAttrs, children: list[TagChild]) -> None:
+        self.attrs = attrs
+        self.children = children
+
+    def tagify(self) -> TagList:
+        return TagList(self.children).tagify()
```

### Comparing `shiny-0.3.3/shiny/experimental/ui/_valuebox.py` & `shiny-0.4.0/shiny/experimental/ui/_valuebox.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,206 @@
 from __future__ import annotations
 
-import numbers
 from typing import Callable, Optional
 
-from htmltools import Tag, TagAttrs, TagAttrValue, TagChild, css, div
+from htmltools import Tag, TagAttrs, TagAttrValue, TagChild, css, div, tags
 
-from shiny._typing_extensions import TypeGuard
-
-from ._card import card, card_body
-from ._card_item import CardItem
-from ._css import CssUnit, validate_css_unit
-from ._fill import bind_fill_role
+from ._card import CardItem, card, card_body
+from ._css_unit import CssUnit, as_css_unit, as_width_unit
+from ._fill import as_fill_carrier
 from ._layout import layout_column_wrap
+from ._utils import consolidate_attrs, is_01_scalar
 
-
-def is_01_scalar(x: object) -> TypeGuard[float]:
-    return isinstance(x, float) and x >= 0.0 and x <= 1.0
-
-
-# It seems to be to use % over fr here since there is no gap on the grid
-def to_width_unit(x: str | float) -> str:
-    if isinstance(x, float):
-        return validate_css_unit(x)
-
-    if isinstance(x, str) and x.endswith("%") and x.count("%") == 1:
-        x1_num = float(x[:-1])
-        x2_num = 100 - x1_num
-        return f"{x1_num}% {x2_num}%"
-
-    # TODO: validateCssUnit() should maybe support fr units?
-    # return(paste(x, collapse = " "))
-    return validate_css_unit(x)
+__all__ = (
+    "value_box",
+    "showcase_left_center",
+    "showcase_top_right",
+)
 
 
+# TODO-maindocs; @add_example()
 def value_box(
-    title: TagChild | str | numbers.Number,
-    value: TagChild | str | numbers.Number,
+    title: TagChild,
+    value: TagChild,
     *args: TagChild | TagAttrs,
     showcase: Optional[TagChild] = None,
     showcase_layout: Callable[[TagChild, Tag], CardItem] | None = None,
     full_screen: bool = False,
     theme_color: Optional[str] = "primary",
     height: Optional[CssUnit] = None,
     max_height: Optional[CssUnit] = None,
     fill: bool = True,
-    class_: Optional[str] = None,  # Applies after `bind_fill_role()` inside `card()`
+    class_: Optional[str] = None,
     **kwargs: TagAttrValue,
 ) -> Tag:
+    """
+    Value box
+
+    An opinionated (:func:`~shiny.experimental.ui.card`-powered) box, designed for
+    displaying a `value` and `title`. Optionally, a `showcase` can provide for context
+    for what the `value` represents (for example, it could hold an icon, or even a
+    :func:`~shiny.ui.output_plot`).
+
+    Parameters
+    ----------
+    title,value
+        A string, number, or :func:`~htmltools.tag` child to display as
+        the title or value of the value box. The `title` appears above the `value`.
+    *args
+        Unnamed arguments may be any :func:`~htmltools.tag` children to display below
+        `value`. Named arguments are passed to :func:`~shiny.experimental.ui.card` as
+        element attributes.
+    showcase
+        A :func:`~htmltools.tag` child to showcase (e.g., an icon, a
+        :func:`~shiny.ui.output_plot`, etc).
+    showcase_layout
+        Either :func:`~showcase_left_center` or :func:`~showcase_top_right`.
+    theme_color
+        A theme color to use for the background color. Should match a name in the
+        Bootstrap Sass variable `$theme-colors` (e.g., `"secondary"`, `"success"`,
+        `"danger"`, etc).
+    height,max_height
+        Any valid CSS unit (e.g., `height="200px"`). Doesn't apply when a card is made
+        `full_screen` (in this case, consider setting a `height` in
+        :func:`~shiny.experimental.ui.card_body()`).
+    fill
+        Whether to allow the value box to grow/shrink to fit a fillable container with
+        an opinionated height (e.g., :func:`~shiny.experimental.ui.page_fillable`).
+    class_
+        Utility classes for customizing the appearance of the summary card. Use `bg-*`
+        and `text-*` classes (e.g, `"bg-danger"` and `"text-light"`) to customize the
+        background/foreground colors.
+    **kwargs
+        Additional attributes to pass to :func:`~shiny.experimental.ui.card`.
+
+    Returns
+    -------
+    :
+        A :func:`~shiny.experimental.ui.card`
+
+    See Also
+    --------
+    * :func:`~shiny.experimental.ui.card`
+    """
+    attrs, children = consolidate_attrs(
+        # Must be before `attrs` so that `class_` is applied before any `attrs` values
+        {"class": "bslib-value-box border-0"},
+        {"class": f"bg-{theme_color}"} if theme_color else None,
+        *args,
+        class_=class_,
+        **kwargs,
+    )
+
     if showcase_layout is None:
         showcase_layout = showcase_left_center()
-    if isinstance(title, str) or isinstance(title, numbers.Number):
-        title = div(str(title), class_="h6 mb-1")
-    if isinstance(value, str) or isinstance(value, numbers.Number):
-        value = div(str(value), class_="h2 mb-2")
+    if isinstance(title, (str, int, float)):
+        title = tags.p(str(title), class_="h6 mb-1")
+    if isinstance(title, (str, int, float)):
+        value = tags.p(str(value), class_="h2 mb-2")
 
     contents = div(
         title,
         value,
-        *args,
+        *children,
         class_="value-box-area",
     )
-    contents = bind_fill_role(contents, container=True, item=True)
+    contents = as_fill_carrier(contents)
 
     if showcase is not None:
         contents = showcase_layout(showcase, contents)
 
-    # Must use `class_` in `card()` as it must be applied after `bind_fill_role()`
-    theme_class_str = f" bg-{theme_color}" if theme_color else ""
-    class_str = f" {class_}" if class_ is not None else ""
-
     return card(
         contents,
-        class_=f"bslib-value-box border-0{theme_class_str}{class_str}",
+        attrs,
         full_screen=full_screen,
         height=height,
         max_height=max_height,
         fill=fill,
-        **kwargs,
     )
 
 
-# @param width one of the following:
-#   * A proportion (i.e., a number between 0 and 1) of available width to
-#     allocate to the showcase.
-#   * A vector of length 2 valid [CSS unit][htmltools::validateCssUnit] defining
-#     the width of each column (for `showcase_left_center()` the 1st unit defines
-#     the showcase width and for `showcase_top_right` the 2nd unit defines the
-#     showcase width). Note that any units supported by the CSS grid
-#     `grid-template-columns` property may be used (e.g., `fr` units).
-# @param max_height,max_height_full_screen A proportion (i.e., a number between
-#   0 and 1) or any valid [CSS unit][htmltools::validateCssUnit] defining the
-#   showcase max_height.
-#
-# @export
-# @rdname value_box
+# TODO-maindocs; @add_example()
 def showcase_left_center(
     width: CssUnit = "30%",
     max_height: CssUnit = "100px",
     max_height_full_screen: CssUnit = "67%",
 ) -> Callable[[TagChild | TagAttrs, Tag], CardItem]:
-    return showcase_layout_(
+    """
+    Left center showcase for a value box
+
+    Gives the showcase a width and centers it vertically.
+
+    Parameters
+    ----------
+    width
+        one of the following:
+        * A proportion (i.e., a number between 0 and 1) of available width to allocate
+          to the showcase.
+        * A vector of length 2 valid CSS unit defining the width of each column (for
+          `showcase_left_center()` the 1st unit defines the showcase width and for
+          `showcase_top_right` the 2nd unit defines the showcase width). Note that any
+          units supported by the CSS grid `grid-template-columns` property may be used
+          (e.g., `fr` units).
+
+    max_height,max_height_full_screen
+        A proportion (i.e., a number between 0 and 1) or any valid CSS unit defining the
+        showcase max_height.
+
+    Returns
+    -------
+    :
+        A function that takes a showcase and contents and returns a :func:`~shiny.experimental.ui.card_body`
+    """
+    return _showcase_layout(
         width=width,
         max_height=max_height,
         max_height_full_screen=max_height_full_screen,
         top_right=False,
     )
 
 
-# @export
-# @rdname value_box
+# TODO-maindocs; @add_example()
 def showcase_top_right(
     width: CssUnit = "30%",
     max_height: CssUnit = "75px",
     max_height_full_screen: CssUnit = "67%",
 ) -> Callable[[TagChild | TagAttrs, Tag], CardItem]:
     if is_01_scalar(width):
         width = 1 - width
-    return showcase_layout_(
+    return _showcase_layout(
         width=width,
         max_height=max_height,
         max_height_full_screen=max_height_full_screen,
         top_right=True,
     )
 
 
-def showcase_layout_(
+def _showcase_layout(
     width: CssUnit,
     max_height: CssUnit,
     max_height_full_screen: CssUnit,
     top_right: bool,
 ) -> Callable[[TagChild | TagAttrs, Tag], CardItem]:
     # Do not "magically" turn `0.3` into `"30%"` as it is not clear to the user when it happens
-    width_css_unit = to_width_unit(width)
-    max_height_css_unit = validate_css_unit(max_height)
-    max_height_full_screen_css_unit = validate_css_unit(max_height_full_screen)
+    width_css_unit = as_width_unit(width)
+    max_height_css_unit = as_css_unit(max_height)
+    max_height_full_screen_css_unit = as_css_unit(max_height_full_screen)
 
-    def _showcase_layout(showcase: TagChild | TagAttrs, contents: Tag) -> CardItem:
+    def _layout(showcase: TagChild | TagAttrs, contents: Tag) -> CardItem:
         css_args = {
             "--bslib-value-box-max-height": max_height_css_unit,
             "--bslib-value-box-max-height-full-screen": max_height_full_screen_css_unit,
         }
         showcase_container = div(
             showcase,
             {"class": "value-box-showcase overflow-hidden"},
             {"class": "showcase-top-right"} if top_right else None,
             style=css(**css_args),
         )
-        showcase_container = bind_fill_role(
-            showcase_container, container=True, item=True
-        )
+        showcase_container = as_fill_carrier(showcase_container)
 
         if not top_right:
             contents.add_class("border-start")
 
         items = [showcase_container, contents]
         width_fs = ["1fr", "auto"]
         if top_right:
@@ -171,8 +219,8 @@
                 gap=0,
                 heights_equal="row",
                 class_="value-box-grid",
             ),
             style=css(padding=0),
         )
 
-    return _showcase_layout
+    return _layout
```

### Comparing `shiny-0.3.3/shiny/html_dependencies.py` & `shiny-0.4.0/shiny/html_dependencies.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/http_staticfiles.py` & `shiny-0.4.0/shiny/http_staticfiles.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/input_handler.py` & `shiny-0.4.0/shiny/input_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from datetime import date, datetime
 from typing import TYPE_CHECKING, Any, Callable, Dict
 
 if TYPE_CHECKING:
     from .session import Session
 
+
 from .types import ActionButtonValue
 
 InputHandlerType = Callable[[Any, str, "Session"], Any]
 
 
 class _InputHandlers(Dict[str, InputHandlerType]):
     def __init__(self):
@@ -43,16 +44,17 @@
 Manage Shiny input handlers.
 
 Add and/or remove input handlers of a given ``type``. Shiny uses these handlers to
 pre-process input values from the client (after being deserialized) before passing them
 to the ``input`` argument of an :func:`~shiny.App`'s ``server`` function.
 
 The ``type`` is based on the ``getType()`` JavaScript method on the relevant Shiny
-input binding. See `this article <https://shiny.rstudio.com/articles/js-custom-input.html>`_
-for more information on how to create custom input bindings.
+input binding. See `this article <https://shiny.posit.co/articles/js-custom-input.html>`_
+for more information on how to create custom input bindings. (The article is about
+Shiny for R, but the JavaScript and general principles are the same.)
 
 Methods
 --------
 add(type: str, force: bool = False) -> Callable[[InputHandlerType], None]
     Register an input handler. This method returns a decorator that registers the
     decorated function as the handler for the given ``type``. This handler should
     accept three arguments:
```

### Comparing `shiny-0.3.3/shiny/module.py` & `shiny-0.4.0/shiny/module.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/plotutils.py` & `shiny-0.4.0/shiny/plotutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         panelvar2 = coordinfo["mapping"]["panelvar2"]
         if panelvar2 not in new_df:
             raise ValueError(f"near_points: `panelvar2` ({panelvar2}) not in dataframe")
         keep_rows &= new_df[panelvar2] == coordinfo["panelvar2"]  # pyright: ignore
 
     # Track the row indices to keep (note this is the row position, 0, 1, 2, not the
     # pandas index column, which can have arbitrary values).
-    keep_idx = np.where(keep_rows)[0]  # pyright: ignore[reportUnknownMemberType]
+    keep_idx = np.where(keep_rows)[0]
 
     # Order by distance
     dists = dists.iloc[keep_idx]
     keep_idx: npt.NDArray[np.intp] = keep_idx[dists.argsort()]
 
     # Keep max number of rows
     if max_points is not None and len(keep_idx) > max_points:
```

### Comparing `shiny-0.3.3/shiny/reactive/__init__.py` & `shiny-0.4.0/shiny/reactive/__init__.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/reactive/_core.py` & `shiny-0.4.0/shiny/reactive/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     :
         A context manager that executes the given expression in a scope where reactive
         values can be read, but do not cause the reactive scope of the caller to be
         re-evaluated when they change.
 
     See Also
     --------
-    ~shiny.event
+    ~shiny.reactive.event
     """
     with _reactive_environment.isolate():
         yield
 
 
 def get_current_context() -> Context:
     """
```

### Comparing `shiny-0.3.3/shiny/reactive/_poll.py` & `shiny-0.4.0/shiny/reactive/_poll.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/reactive/_reactives.py` & `shiny-0.4.0/shiny/reactive/_reactives.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,15 +415,15 @@
 
     See Also
     --------
     ~shiny.Inputs
     ~shiny.reactive.Value
     ~shiny.reactive.Effect
     ~shiny.reactive.invalidate_later
-    ~shiny.event
+    ~shiny.reactive.event
     """
 
     def create_calc(fn: CalcFunction[T] | CalcFunctionAsync[T]) -> Calc_[T]:
         if _utils.is_async_callable(fn):
             return CalcAsync_(fn, session=session)
         else:
             fn = cast(CalcFunction[T], fn)
@@ -690,15 +690,15 @@
 
     See Also
     --------
     ~shiny.Inputs
     ~shiny.reactive.Value
     ~shiny.reactive.Effect
     ~shiny.reactive.invalidate_later
-    ~shiny.event
+    ~shiny.reactive.event
     """
 
     def create_effect(fn: EffectFunction | EffectFunctionAsync) -> Effect_:
         fn = cast(EffectFunction, fn)
         return Effect_(fn, suspended=suspended, priority=priority, session=session)
 
     if fn is None:
```

### Comparing `shiny-0.3.3/shiny/render/__init__.py` & `shiny-0.4.0/shiny/render/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,15 +18,26 @@
     RenderTableAsync,  # pyright: ignore[reportUnusedImport]
     table,
     RenderUI,  # pyright: ignore[reportUnusedImport]
     RenderUIAsync,  # pyright: ignore[reportUnusedImport]
     ui,
 )
 
+from ._dataframe import (  # noqa: F401
+    RenderDataFrame,  # pyright: ignore[reportUnusedImport]
+    RenderDataFrameAsync,  # pyright: ignore[reportUnusedImport]
+    DataGrid,
+    DataTable,
+    data_frame,
+)
+
 
 __all__ = (
+    "DataGrid",
+    "DataTable",
+    "data_frame",
     "text",
     "plot",
     "image",
     "table",
     "ui",
 )
```

### Comparing `shiny-0.3.3/shiny/render/_coordmap.py` & `shiny-0.4.0/shiny/render/_coordmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,18 @@
 def get_coordmap(fig: Figure) -> Coordmap | None:
     dims_ar = cast("npt.NDArray[np.double]", fig.get_size_inches() * fig.get_dpi())
     dims: CoordmapDims = {
         "width": dims_ar[0],
         "height": dims_ar[1],
     }
 
-    all_axes = cast("list[Axes]", fig.get_axes())
+    all_axes = cast(
+        "list[Axes]",  # pyright: ignore
+        fig.get_axes(),
+    )
 
     panels: list[CoordmapPanel] = []
     for i, axes in enumerate(all_axes):
         panel = get_coordmap_panel(axes, i + 1, dims["height"])
         panels.append(panel)
 
     coordmap: Coordmap = {
```

### Comparing `shiny-0.3.3/shiny/render/_render.py` & `shiny-0.4.0/shiny/render/_render.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,30 @@
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     Generic,
     Optional,
     TypeVar,
+    Union,
+    cast,
     overload,
 )
 
 # These aren't used directly in this file, but they seem necessary for Sphinx to work
 # cleanly.
 from htmltools import Tag  # pyright: ignore[reportUnusedImport] # noqa: F401
 from htmltools import Tagifiable  # pyright: ignore[reportUnusedImport] # noqa: F401
 from htmltools import TagList  # pyright: ignore[reportUnusedImport] # noqa: F401
 from htmltools import TagChild
 
 if TYPE_CHECKING:
     from ..session import Session
     from ..session._utils import RenderedDeps
+    import pandas as pd
 
 from .. import _utils
 from .._namespaces import ResolvedId
 from .._typing_extensions import Protocol, runtime_checkable
 from ..types import ImgData
 from ._try_render_plot import try_render_matplotlib, try_render_pil, try_render_plotnine
 
@@ -336,15 +339,15 @@
         1. A :class:`matplotlib.figure.Figure` instance.
         2. An :class:`matplotlib.artist.Artist` instance.
         3. A list/tuple of Figure/Artist instances.
         4. An object with a 'figure' attribute pointing to a
            :class:`matplotlib.figure.Figure` instance.
         5. A :class:`PIL.Image.Image` instance.
 
-    It's also possible to use the `matplotlib.pyplot` interface; in that case, your
+    It's also possible to use the ``matplotlib.pyplot`` interface; in that case, your
     function should just call pyplot functions and not return anything. (Note that if
     the decorated function is async, then it's not safe to use pyplot. Shiny will detect
     this case and throw an error asking you to use matplotlib's object-oriented
     interface instead.)
 
     Tip
     ----
@@ -484,29 +487,28 @@
     else:
         return wrapper(fn)
 
 
 # ======================================================================================
 # RenderTable
 # ======================================================================================
-# It would be nice to specify the return type of RenderPlotFunc to be something like:
-#   Union[pandas.DataFrame, <protocol with .to_pandas()>]
-# However, if we did that, we'd have to import pandas at load time, which adds
-# a nontrivial amount of overhead. So for now, we're just using `object`.
-RenderTableFunc = Callable[[], object]
-RenderTableFuncAsync = Callable[[], Awaitable[object]]
 
 
 @runtime_checkable
 class PandasCompatible(Protocol):
     # Signature doesn't matter, runtime_checkable won't look at it anyway
-    def to_pandas(self) -> object:
+    def to_pandas(self) -> "pd.DataFrame":
         ...
 
 
+TableResult = Union[None, "pd.DataFrame", PandasCompatible]
+RenderTableFunc = Callable[[], TableResult]
+RenderTableFuncAsync = Callable[[], Awaitable[TableResult]]
+
+
 class RenderTable(RenderFunction[object, "RenderedDeps | None"]):
     def __init__(
         self,
         fn: RenderTableFunc,
         *,
         index: bool = False,
         classes: str = "table shiny-table w-auto",
@@ -528,34 +530,31 @@
 
     async def _run(self) -> RenderedDeps | None:
         x = await self._fn()
 
         if x is None:
             return None
 
-        import pandas  # pyright: reportMissingTypeStubs=false,reportUnknownVariableType=false,reportMissingImports=false,reportMissingModuleSource=false
+        import pandas
         import pandas.io.formats.style
 
         html: str
-        if isinstance(
-            x, pandas.io.formats.style.Styler
-        ):  # pyright: reportUnknownMemberType=false
-            html = x.to_html(**self._kwargs)  # pyright: reportGeneralTypeIssues=false
+        if isinstance(x, pandas.io.formats.style.Styler):
+            html = x.to_html(**self._kwargs)  # pyright: ignore[reportUnknownMemberType]
         else:
             if not isinstance(x, pandas.DataFrame):
                 if not isinstance(x, PandasCompatible):
                     raise TypeError(
                         "@render.table doesn't know how to render objects of type "
                         f"'{str(type(x))}'. Return either a pandas.DataFrame, or an object "
                         "that has a .to_pandas() method."
                     )
                 x = x.to_pandas()
 
-            df = typing.cast(pandas.DataFrame, x)
-            html = df.to_html(
+            html = x.to_html(  # pyright: ignore[reportUnknownMemberType]
                 index=self._index,
                 classes=self._classes,
                 border=self._border,
                 **self._kwargs,
             )
         return {"deps": [], "html": html}
 
@@ -654,15 +653,19 @@
     def wrapper(fn: RenderTableFunc | RenderTableFuncAsync) -> RenderTable:
         if _utils.is_async_callable(fn):
             return RenderTableAsync(
                 fn, index=index, classes=classes, border=border, **kwargs
             )
         else:
             return RenderTable(
-                fn, index=index, classes=classes, border=border, **kwargs
+                cast(RenderTableFunc, fn),
+                index=index,
+                classes=classes,
+                border=border,
+                **kwargs,
             )
 
     if fn is None:
         return wrapper
     else:
         return wrapper(fn)
```

### Comparing `shiny-0.3.3/shiny/render/_try_render_plot.py` & `shiny-0.4.0/shiny/render/_try_render_plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,30 +25,34 @@
     height: float,
     pixelratio: float,
     ppi: float,
     allow_global: bool,
     alt: Optional[str],
     **kwargs: object,
 ) -> TryPlotResult:
-    fig = get_matplotlib_figure(x, allow_global)
+    fig = get_matplotlib_figure(  # pyright: ignore[reportUnknownVariableType]
+        x, allow_global
+    )
 
     if fig is None:
         return (False, None)
 
     try:
         import matplotlib.pyplot as plt
 
-        fig.set_size_inches(width / ppi, height / ppi)
-        fig.set_dpi(ppi * pixelratio)
+        fig.set_size_inches(  # pyright: ignore[reportUnknownMemberType]
+            width / ppi, height / ppi
+        )
+        fig.set_dpi(ppi * pixelratio)  # pyright: ignore[reportUnknownMemberType]
 
-        plt.tight_layout()
+        plt.tight_layout()  # pyright: ignore[reportUnknownMemberType]
         coordmap = get_coordmap(fig)
 
         with io.BytesIO() as buf:
-            fig.savefig(
+            fig.savefig(  # pyright: ignore[reportUnknownMemberType]
                 buf,
                 format="png",
                 dpi=ppi * pixelratio,
                 **kwargs,
             )
             buf.seek(0)
             data = base64.b64encode(buf.read())
@@ -65,37 +69,45 @@
 
         if coordmap is not None:
             res["coordmap"] = coordmap
 
         return (True, res)
 
     finally:
-        import matplotlib.pyplot  # pyright: ignore[reportMissingTypeStubs]
+        import matplotlib.pyplot
 
-        matplotlib.pyplot.close(fig)  # pyright: ignore[reportGeneralTypeIssues]
+        matplotlib.pyplot.close(fig)  # pyright: ignore[reportUnknownMemberType]
 
 
-def get_matplotlib_figure(x: object, allow_global: bool) -> Figure | None:
+def get_matplotlib_figure(
+    x: object, allow_global: bool
+) -> Figure | None:  # pyright: ignore
     import matplotlib.pyplot as plt
     from matplotlib.animation import Animation
     from matplotlib.artist import Artist
     from matplotlib.figure import Figure
 
     # Detect usage of pyplot global figure
     # TODO: Might be good to detect non-empty plt.get_fignums() before we call the user
     #   function, which would mean we will false-positive here. Maybe we warn in that
     #   case, maybe we ignore gcf(), maybe both.
     if (
-        x is None and len(plt.get_fignums()) > 0
-    ):  # pyright: reportUnknownArgumentType=false, reportUnknownMemberType=false
+        x is None
+        and len(
+            plt.get_fignums()  # pyright: ignore[reportUnknownArgumentType, reportUnknownMemberType]
+        )
+        > 0
+    ):
         if allow_global:
-            return plt.gcf()
+            return (
+                plt.gcf()  # pyright: ignore[reportUnknownVariableType, reportUnknownMemberType]
+            )
         else:
             # Must close the global figure so we don't stay in this state forever
-            plt.close(plt.gcf())
+            plt.close(plt.gcf())  # pyright: ignore[reportUnknownMemberType]
             raise RuntimeError(
                 "matplotlib.pyplot cannot be used from an async render function; "
                 "please use matplotlib's object-oriented interface instead"
             )
 
     if isinstance(x, Figure):
         return x
@@ -108,43 +120,47 @@
         )
 
     # Libraries like pandas, xarray, etc have plot() methods that can return a wide
     # array pf mpl classes, like Lines2D, Subplots, Axes, etc. The Artist ABC class
     # should cover most, if not all, of these (it doesn't cover Animation, though).
     # https://matplotlib.org/stable/api/artist_api.html
     if isinstance(x, Artist):
-        return x.get_figure()
+        return (
+            x.get_figure()  # pyright: ignore[reportUnknownMemberType, reportUnknownVariableType]
+        )
 
     # Some other custom figure-like classes such as seaborn.axisgrid.FacetGrid attach
     # their figure as an attribute
     fig = getattr(x, "figure", None)
     if isinstance(fig, Figure):
         return fig
 
     # Sometimes generic plot() methods will return an iterable of Artists,
     # If they all refer to the same figure, then it seems reasonable to use it
     # https://docs.xarray.dev/en/latest/user-guide/plotting.html#dimension-along-y-axis
     if isinstance(x, (list, tuple)):
-        figs = [get_matplotlib_figure(y, allow_global) for y in cast(List[Any], x)]
-        if len(set(figs)) == 1:
-            return figs[0]
+        figs = [  # pyright: ignore[reportUnknownVariableType]
+            get_matplotlib_figure(y, allow_global) for y in cast(List[Any], x)
+        ]
+        if len(set(figs)) == 1:  # pyright: ignore[reportUnknownArgumentType]
+            return figs[0]  # pyright: ignore[reportUnknownVariableType]
 
     return None
 
 
 def try_render_pil(
     x: object,
     width: float,
     height: float,
     pixelratio: float,
     ppi: float,
     alt: Optional[str] = None,
     **kwargs: object,
 ) -> TryPlotResult:
-    import PIL.Image  # pyright: ignore[reportMissingModuleSource]
+    import PIL.Image
 
     if not isinstance(x, PIL.Image.Image):
         return (False, None)
 
     with io.BytesIO() as buf:
         x.save(buf, format="PNG", **kwargs)
         buf.seek(0)
@@ -169,41 +185,45 @@
     width: float,
     height: float,
     pixelratio: float,
     ppi: float,
     alt: Optional[str] = None,
     **kwargs: object,
 ) -> TryPlotResult:
-    from plotnine.ggplot import (  # pyright: reportMissingTypeStubs=false,reportUnknownVariableType=false,reportMissingImports=false
-        ggplot,
-    )
+    # Must use `pyright: ignore` otherwise Black formats the comments into a single line
+    from plotnine.ggplot import ggplot  # pyright: ignore
 
     if not isinstance(x, ggplot):
         return (False, None)
 
     x = cast(PlotnineFigure, x)
 
     with io.BytesIO() as buf:
         # save_helper was added in plotnine 0.10.1-dev. If this method exists, we can
         # use it to get the matplotlib Figure object, which we can then use to get the
         # coordmap. Once this version of plotnine is released and in common use, we can
         # add a version dependency and remove the conditional code.
         if hasattr(x, "save_helper"):
-            res = x.save_helper(  # pyright: reportGeneralTypeIssues=false
+            res = x.save_helper(  # pyright: ignore[reportUnknownMemberType, reportGeneralTypeIssues, reportUnknownVariableType]
                 filename=buf,
                 format="png",
                 units="in",
                 dpi=ppi * pixelratio,
                 width=width / ppi,
                 height=height / ppi,
                 verbose=False,
                 **kwargs,
             )
-            coordmap = get_coordmap_plotnine(x, res.figure)
-            res.figure.savefig(**res.kwargs)
+            coordmap = get_coordmap_plotnine(
+                x,
+                res.figure,  # pyright: ignore[reportUnknownMemberType, reportGeneralTypeIssues]
+            )
+            res.figure.savefig(  # pyright: ignore[reportUnknownMemberType, reportGeneralTypeIssues]
+                **res.kwargs  # pyright: ignore[reportUnknownMemberType, reportGeneralTypeIssues]
+            )
         else:
             x.save(
                 filename=buf,
                 format="png",
                 units="in",
                 dpi=ppi * pixelratio,
                 width=width / ppi,
```

### Comparing `shiny-0.3.3/shiny/session/_session.py` & `shiny-0.4.0/shiny/session/_session.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/session/_utils.py` & `shiny-0.4.0/shiny/session/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Needed for types imported only during TYPE_CHECKING with Python 3.7 - 3.9
 # See https://www.python.org/dev/peps/pep-0655/#usage-in-python-3-11
 from __future__ import annotations
 
-__all__ = ("get_current_session", "session_context", "require_active_session")
+__all__ = (
+    "get_current_session",
+    "session_context",
+    "require_active_session",
+)
 
 from contextlib import contextmanager
 from contextvars import ContextVar, Token
 from typing import TYPE_CHECKING, Any, Callable, Optional, TypeVar
 
 if TYPE_CHECKING:
     from ._session import Session
```

### Comparing `shiny-0.3.3/shiny/types.py` & `shiny-0.4.0/shiny/types.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/__init__.py` & `shiny-0.4.0/shiny/ui/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     panel_title,
     panel_fixed,
     panel_absolute,
     help_text,
 )
 from ._download_button import download_button, download_link
 from ._plot_output_opts import brush_opts, click_opts, dblclick_opts, hover_opts
+from ._include_helpers import include_css, include_js
 from ._input_action_button import input_action_button, input_action_link
 from ._input_check_radio import (
     input_checkbox,
     input_checkbox_group,
     input_switch,
     input_radio_buttons,
 )
@@ -73,14 +74,16 @@
     output_text_verbatim,
     output_table,
     output_ui,
 )
 from ._page import page_navbar, page_fluid, page_fixed, page_bootstrap
 from ._progress import Progress
 
+from .dataframe._dataframe import output_data_frame
+
 from htmltools import (
     TagList,
     Tag,
     TagChild,
     TagAttrs,
     TagAttrValue,
     tags,
@@ -120,14 +123,16 @@
     "help_text",
     "download_button",
     "download_link",
     "brush_opts",
     "click_opts",
     "dblclick_opts",
     "hover_opts",
+    "include_css",
+    "include_js",
     "input_action_button",
     "input_action_link",
     "input_checkbox",
     "input_checkbox_group",
     "input_switch",
     "input_radio_buttons",
     "input_date",
@@ -174,14 +179,15 @@
     "navset_pill",
     "navset_pill_card",
     "navset_pill_list",
     "navset_hidden",
     "navset_bar",
     "notification_show",
     "notification_remove",
+    "output_data_frame",
     "output_plot",
     "output_image",
     "output_text",
     "output_text_verbatim",
     "output_table",
     "output_ui",
     "page_navbar",
```

### Comparing `shiny-0.3.3/shiny/ui/_bootstrap.py` & `shiny-0.4.0/shiny/ui/_bootstrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,49 +10,57 @@
     "panel_conditional",
     "panel_title",
     "panel_fixed",
     "panel_absolute",
     "help_text",
 )
 
+
 from typing import Optional
 
 from htmltools import (
     Tag,
     TagAttrs,
     TagAttrValue,
     TagChild,
+    Tagifiable,
     TagList,
     css,
     div,
     h2,
     span,
     tags,
 )
 
+from .._deprecated import warn_deprecated
 from .._docstring import add_example
 from .._typing_extensions import Literal
 from ..module import current_namespace
 from ..types import MISSING, MISSING_TYPE
 from ._html_dependencies import jqui_deps
 from ._utils import get_window_title
+from ._x._sidebar import PanelMain as XPanelMain
+from ._x._sidebar import PanelSidebar as XPanelSidebar
+from ._x._sidebar import layout_sidebar as x_layout_sidebar
+from ._x._utils import consolidate_attrs as x_consolidate_attrs
 
 
 # TODO: make a python version of the layout guide?
 @add_example()
 def row(*args: TagChild | TagAttrs, **kwargs: TagAttrValue) -> Tag:
     """
     Responsive row-column based layout
 
     Layout UI components using Bootstrap's grid layout system. Use ``row()`` to group
     elements that should appear on the same line (if the browser has adequate width) and
     :func:`~shiny.ui.column` to define how much horizontal space within a 12-unit wide
     grid each on of these elements should occupy. See the [layout
-    guide](https://shiny.rstudio.com/articles/layout-guide.html>) for more context and
+    guide](https://shiny.posit.co/articles/layout-guide.html>) for more context and
     examples.
+    (The article is about Shiny for R, but the general principles are the same.)
 
     Parameters
     ----------
     args
         Any number of child elements.
     kwargs
         Attributes to place on the row tag.
@@ -112,15 +120,15 @@
 
 @add_example()
 def layout_sidebar(
     # TODO: also accept a generic list (and wrap in panel in that case)?
     sidebar: TagChild,
     main: TagChild,
     position: Literal["left", "right"] = "left",
-) -> Tag:
+) -> Tagifiable:
     """
     Layout a sidebar and main area
 
     Create a layout with a sidebar (:func:`~shiny.ui.panel_sidebar`) and main area
     (:func:`~shiny.ui.panel_main`). The sidebar is displayed with a distinct background
     color and typically contains input controls. By default, the main area occupies 2/3
     of the horizontal width and typically contains outputs.
@@ -142,15 +150,25 @@
         A UI element
 
     See Also
     -------
     :func:`~shiny.ui.panel_sidebar`
     :func:`~shiny.ui.panel_main`
     """
-    return row(sidebar, main) if position == "left" else row(main, sidebar)
+
+    # Not requiring `XPanelSidebar`/`XPanelMain` to not expose the `_x` module if possible
+    if not isinstance(sidebar, XPanelSidebar):
+        sidebar = XPanelSidebar(sidebar)
+    if not isinstance(main, XPanelMain):
+        main = XPanelMain(attrs={}, children=[main])
+
+    return x_layout_sidebar(
+        sidebar.get_sidebar(position=position),
+        main,
+    )
 
 
 def panel_well(*args: TagChild | TagAttrs, **kwargs: TagAttrValue) -> Tag:
     """
     Create a well panel
 
     Creates a panel with a slightly inset border and grey background. Equivalent to
@@ -173,16 +191,18 @@
     :func:`~shiny.ui.panel_sidebar`
     :func:`~shiny.ui.panel_main`
     """
     return div({"class": "well"}, *args, **kwargs)
 
 
 def panel_sidebar(
-    *args: TagChild | TagAttrs, width: int = 4, **kwargs: TagAttrValue
-) -> Tag:
+    *args: TagChild | TagAttrs,
+    width: int = 4,
+    **kwargs: TagAttrValue,
+) -> Tagifiable:
     """
     Create a sidebar panel
 
     See :func:`~shiny.ui.layout_sidebar` for more information and an example.
 
     Parameters
     ----------
@@ -200,55 +220,57 @@
         A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.panel_sidebar`
     :func:`~shiny.ui.panel_main`
     """
-    return div(
-        {"class": "col-sm-" + str(width)},
-        # A11y semantic landmark for sidebar
-        tags.form({"class": "well"}, *args, role="complementary", **kwargs),
-    )
+    return XPanelSidebar(*args, width=width, **kwargs)
 
 
 def panel_main(
-    *args: TagChild | TagAttrs, width: int = 8, **kwargs: TagAttrValue
-) -> Tag:
+    *args: TagChild | TagAttrs,
+    **kwargs: TagAttrValue,
+) -> Tagifiable:
     """
     Create an main area panel
 
     See :func:`~shiny.ui.layout_sidebar` for more information and an example.
 
     Parameters
     ----------
     args
         UI elements to include inside the main area.
-    width
-        The width of the main area (an integer between 1 and 12).
     kwargs
         Attributes to place on the main area tag.
 
     Returns
     -------
     :
         A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.panel_sidebar`
     :func:`~shiny.ui.layout_sidebar`
     """
-    return div(
-        {"class": "col-sm-" + str(width)},
-        # A11y semantic landmark for main region
-        *args,
-        role="main",
-        **kwargs,
-    )
+    attrs, children = x_consolidate_attrs(*args, **kwargs)
+    if "width" in attrs:
+        if attrs["width"] != 8:
+            warn_deprecated(
+                "panel_main(width=)` is being ignored. Given the sidebar width, the main panel will take up the remaining horizontal space."
+            )
+        del attrs["width"]
+
+    if len(attrs) > 0:
+        # While we could return an `XPanelMain()` for empty attrs,
+        # let's try to limit the exposure of the class object
+        return XPanelMain(attrs=attrs, children=children)
+
+    return TagList(*children)
 
 
 # TODO: replace `flowLayout()`/`splitLayout()` with a flexbox wrapper?
 # def panel_input(*args: TagChild, **kwargs: TagAttr):
 #  return div(flowLayout(...), class_="shiny-input-panel")
```

### Comparing `shiny-0.3.3/shiny/ui/_download_button.py` & `shiny-0.4.0/shiny/ui/_download_button.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_html_dependencies.py` & `shiny-0.4.0/shiny/ui/_html_dependencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 def bootstrap_deps() -> list[HTMLDependency]:
     dep = HTMLDependency(
         name="bootstrap",
         version=bootstrap_version,
         source={"package": "shiny", "subdir": "www/shared/bootstrap/"},
         script={"src": "bootstrap.bundle.min.js"},
         stylesheet={"href": "bootstrap.min.css"},
+        meta={"name": "viewport", "content": "width=device-width, initial-scale=1"},
     )
     deps = [jquery_deps(), dep]
     return deps
 
 
 def ionrangeslider_deps() -> list[HTMLDependency]:
     return [
```

### Comparing `shiny-0.3.3/shiny/ui/_input_action_button.py` & `shiny-0.4.0/shiny/ui/_input_action_button.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     .. admonition:: Server value
 
         An integer representing the number of clicks.
 
     See Also
     -------
     ~shiny.ui.input_action_link
-    ~shiny.event
+    ~shiny.reactive.event
     """
 
     return tags.button(
         {"class": "btn btn-default action-button", "style": css(width=width)},
         icon,
         None if icon is None else " ",
         label,
@@ -95,15 +95,15 @@
     .. admonition:: Server value
 
         An integer representing the number of clicks.
 
     See Also
     -------
     ~shiny.ui.input_action_button
-    ~shiny.event
+    ~shiny.reactive.event
     """
 
     return tags.a(
         {"class": "action-button"},
         icon,
         label,
         id=resolve_id(id),
```

### Comparing `shiny-0.3.3/shiny/ui/_input_check_radio.py` & `shiny-0.4.0/shiny/ui/_input_check_radio.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_input_date.py` & `shiny-0.4.0/shiny/ui/_input_date.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_input_file.py` & `shiny-0.4.0/shiny/ui/_input_file.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_input_numeric.py` & `shiny-0.4.0/shiny/ui/_input_numeric.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_input_password.py` & `shiny-0.4.0/shiny/ui/_input_password.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_input_select.py` & `shiny-0.4.0/shiny/ui/_input_select.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_input_slider.py` & `shiny-0.4.0/shiny/ui/_input_slider.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         # integer multiple of the step size, e.g., min=1, max=10, step=4
         scale_factor = math.ceil(n_steps / 10)
         n_ticks = n_steps / scale_factor
 
     id = resolve_id(id)
 
     props: dict[str, TagAttrValue] = {
-        "class_": "js-range-slider",
+        "class": "js-range-slider",
         "id": id,
         "data_skin": "shiny",
         # TODO: do we need to worry about scientific notation (i.e., formatNoSci()?)
         "data_min": str(min_num),
         "data_max": str(max_num),
         "data_from": str(val_nums[0]),
         "data_step": str(step_num),
```

### Comparing `shiny-0.3.3/shiny/ui/_input_text.py` & `shiny-0.4.0/shiny/ui/_input_text.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_input_update.py` & `shiny-0.4.0/shiny/ui/_input_update.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_insert.py` & `shiny-0.4.0/shiny/ui/_insert.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_markdown.py` & `shiny-0.4.0/shiny/ui/_markdown.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_modal.py` & `shiny-0.4.0/shiny/ui/_modal.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_navs.py` & `shiny-0.4.0/shiny/ui/_navs.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
         ul_class = self.ul_class
         if id is not None:
             ul_class += " shiny-tab-input"
 
         nav, content = render_navset(
             *self.args, ul_class=ul_class, id=id, selected=self.selected, context={}
         )
-        return self.layout(nav, content)
+        return self.layout(nav, content).tagify()
 
     def layout(self, nav: TagChild, content: TagChild) -> TagList | Tag:
         return TagList(nav, self.header, content, self.footer)
 
 
 # -----------------------------------------------------------------------------
 # Navigation containers
```

### Comparing `shiny-0.3.3/shiny/ui/_notification.py` & `shiny-0.4.0/shiny/ui/_notification.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_output.py` & `shiny-0.4.0/shiny/ui/_output.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_page.py` & `shiny-0.4.0/shiny/ui/_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,10 +228,9 @@
         A UI element.
 
     See Also
     -------
     :func:`~shiny.ui.page_fluid`
     :func:`~shiny.ui.page_navbar`
     """
-
     head = tags.title(title) if title else None
     return tags.html(tags.head(head), tags.body(*bootstrap_deps(), *args), lang=lang)
```

### Comparing `shiny-0.3.3/shiny/ui/_plot_output_opts.py` & `shiny-0.4.0/shiny/ui/_plot_output_opts.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_progress.py` & `shiny-0.4.0/shiny/ui/_progress.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/ui/_utils.py` & `shiny-0.4.0/shiny/ui/_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Optional
+from typing import Optional, overload
 
 from htmltools import (
     HTMLDependency,
     Tag,
     TagChild,
     TagList,
     TagNode,
@@ -16,14 +16,38 @@
 
 
 def shiny_input_label(id: str, label: TagChild = None) -> Tag:
     cls = "control-label" + ("" if label else " shiny-label-null")
     return tags.label(label, class_=cls, id=id + "-label", for_=id)
 
 
+@overload
+def get_window_title(
+    title: None,
+    window_title: MISSING_TYPE,
+) -> None:
+    ...
+
+
+@overload
+def get_window_title(
+    title: None,
+    window_title: str,
+) -> HTMLDependency:
+    ...
+
+
+@overload
+def get_window_title(
+    title: str | Tag | TagList,
+    window_title: str | MISSING_TYPE,
+) -> HTMLDependency:
+    ...
+
+
 def get_window_title(
     title: Optional[str | Tag | TagList],
     window_title: str | MISSING_TYPE = MISSING,
 ) -> Optional[HTMLDependency]:
     if title is not None and isinstance(window_title, MISSING_TYPE):
         window_title = _find_child_strings(title)
```

### Comparing `shiny-0.3.3/shiny/www/shared/bootstrap/bootstrap.bundle.min.js` & `shiny-0.4.0/shiny/www/shared/bootstrap/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map` & `shiny-0.4.0/shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/bootstrap/bootstrap.min.css` & `shiny-0.4.0/shiny/www/shared/bootstrap/bootstrap.min.css`

 * *Files 6% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 /*!
    * Bootstrap  v5.2.2 (https://getbootstrap.com/)
    * Copyright 2011-2022 The Bootstrap Authors
    * Copyright 2011-2022 Twitter, Inc.
    * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE)
-   */:root{--bs-blue: #0d6efd;--bs-indigo: #6610f2;--bs-purple: #6f42c1;--bs-pink: #d63384;--bs-red: #dc3545;--bs-orange: #fd7e14;--bs-yellow: #ffc107;--bs-green: #198754;--bs-teal: #20c997;--bs-cyan: #0dcaf0;--bs-black: #000;--bs-white: #fff;--bs-gray: #6c757d;--bs-gray-dark: #343a40;--bs-gray-100: #f8f9fa;--bs-gray-200: #e9ecef;--bs-gray-300: #dee2e6;--bs-gray-400: #ced4da;--bs-gray-500: #adb5bd;--bs-gray-600: #6c757d;--bs-gray-700: #495057;--bs-gray-800: #343a40;--bs-gray-900: #212529;--bs-default: #dee2e6;--bs-primary: #0d6efd;--bs-secondary: #6c757d;--bs-success: #198754;--bs-info: #0dcaf0;--bs-warning: #ffc107;--bs-danger: #dc3545;--bs-light: #f8f9fa;--bs-dark: #212529;--bs-default-rgb: 222,226,230;--bs-primary-rgb: 13,110,253;--bs-secondary-rgb: 108,117,125;--bs-success-rgb: 25,135,84;--bs-info-rgb: 13,202,240;--bs-warning-rgb: 255,193,7;--bs-danger-rgb: 220,53,69;--bs-light-rgb: 248,249,250;--bs-dark-rgb: 33,37,41;--bs-white-rgb: 255,255,255;--bs-black-rgb: 0,0,0;--bs-body-color-rgb: 33,37,41;--bs-body-bg-rgb: 255,255,255;--bs-font-sans-serif: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", "Liberation Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";--bs-font-monospace: SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;--bs-gradient: linear-gradient(180deg, rgba(255,255,255,0.15), rgba(255,255,255,0));--bs-body-font-family: var(--bs-font-sans-serif);--bs-body-font-size:1rem;--bs-body-font-weight: 400;--bs-body-line-height: 1.5;--bs-body-color: #212529;--bs-body-bg: #fff;--bs-border-width: 1px;--bs-border-style: solid;--bs-border-color: #dee2e6;--bs-border-color-translucent: rgba(0,0,0,0.175);--bs-border-radius: .375rem;--bs-border-radius-sm: .25rem;--bs-border-radius-lg: .5rem;--bs-border-radius-xl: 1rem;--bs-border-radius-2xl: 2rem;--bs-border-radius-pill: 50rem;--bs-link-color: #0d6efd;--bs-link-hover-color: #0a58ca;--bs-code-color: #000;--bs-highlight-bg: #fff3cd}*,*::before,*::after{box-sizing:border-box}@media (prefers-reduced-motion: no-preference){:root{scroll-behavior:smooth}}body{margin:0;font-family:var(--bs-body-font-family);font-size:var(--bs-body-font-size);font-weight:var(--bs-body-font-weight);line-height:var(--bs-body-line-height);color:var(--bs-body-color);text-align:var(--bs-body-text-align);background-color:var(--bs-body-bg);-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:rgba(0,0,0,0)}hr{margin:1rem 0;color:inherit;border:0;border-top:1px solid;opacity:.25}h6,.h6,h5,.h5,h4,.h4,h3,.h3,h2,.h2,h1,.h1{margin-top:0;margin-bottom:.5rem;font-weight:500;line-height:1.2}h1,.h1{font-size:calc(1.375rem + 1.5vw)}@media (min-width: 1200px){h1,.h1{font-size:2.5rem}}h2,.h2{font-size:calc(1.325rem + .9vw)}@media (min-width: 1200px){h2,.h2{font-size:2rem}}h3,.h3{font-size:calc(1.3rem + .6vw)}@media (min-width: 1200px){h3,.h3{font-size:1.75rem}}h4,.h4{font-size:calc(1.275rem + .3vw)}@media (min-width: 1200px){h4,.h4{font-size:1.5rem}}h5,.h5{font-size:1.25rem}h6,.h6{font-size:1rem}p{margin-top:0;margin-bottom:1rem}abbr[title]{text-decoration:underline dotted;-webkit-text-decoration:underline dotted;-moz-text-decoration:underline dotted;-ms-text-decoration:underline dotted;-o-text-decoration:underline dotted;cursor:help;text-decoration-skip-ink:none}address{margin-bottom:1rem;font-style:normal;line-height:inherit}ol,ul{padding-left:2rem}ol,ul,dl{margin-top:0;margin-bottom:1rem}ol ol,ul ul,ol ul,ul ol{margin-bottom:0}dt{font-weight:700}dd{margin-bottom:.5rem;margin-left:0}blockquote{margin:0 0 1rem;padding:.625rem 1.25rem;border-left:.25rem solid #e9ecef}blockquote p:last-child,blockquote ul:last-child,blockquote ol:last-child{margin-bottom:0}b,strong{font-weight:bolder}small,.small{font-size:.875em}mark,.mark{padding:.1875em;background-color:var(--bs-highlight-bg)}sub,sup{position:relative;font-size:.75em;line-height:0;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}a{color:var(--bs-link-color);text-decoration:underline;-webkit-text-decoration:underline;-moz-text-decoration:underline;-ms-text-decoration:underline;-o-text-decoration:underline}a:hover{color:var(--bs-link-hover-color)}a:not([href]):not([class]),a:not([href]):not([class]):hover{color:inherit;text-decoration:none}pre,code,kbd,samp{font-family:var(--bs-font-monospace);font-size:1em}pre{display:block;margin-top:0;margin-bottom:1rem;overflow:auto;font-size:.875em;color:#000;background-color:#f6f6f6;padding:.5rem;border:1px solid #dee2e6;border-radius:.375rem}pre code{background-color:transparent;font-size:inherit;color:inherit;word-break:normal}code{font-size:.875em;color:var(--bs-code-color);background-color:#f6f6f6;border-radius:.375rem;padding:.125rem .25rem;word-wrap:break-word}a>code{color:inherit}kbd{padding:.1875rem .375rem;font-size:.875em;color:var(--bs-body-bg);background-color:var(--bs-body-color);border-radius:.25rem}kbd kbd{padding:0;font-size:1em}figure{margin:0 0 1rem}img,svg{vertical-align:middle}table{caption-side:bottom;border-collapse:collapse}caption{padding-top:.5rem;padding-bottom:.5rem;color:#6c757d;text-align:left}th{text-align:inherit;text-align:-webkit-match-parent}thead,tbody,tfoot,tr,td,th{border-color:inherit;border-style:solid;border-width:0}label{display:inline-block}button{border-radius:0}button:focus:not(:focus-visible){outline:0}input,button,select,optgroup,textarea{margin:0;font-family:inherit;font-size:inherit;line-height:inherit}button,select{text-transform:none}[role="button"]{cursor:pointer}select{word-wrap:normal}select:disabled{opacity:1}[list]:not([type="date"]):not([type="datetime-local"]):not([type="month"]):not([type="week"]):not([type="time"])::-webkit-calendar-picker-indicator{display:none !important}button,[type="button"],[type="reset"],[type="submit"]{-webkit-appearance:button}button:not(:disabled),[type="button"]:not(:disabled),[type="reset"]:not(:disabled),[type="submit"]:not(:disabled){cursor:pointer}::-moz-focus-inner{padding:0;border-style:none}textarea{resize:vertical}fieldset{min-width:0;padding:0;margin:0;border:0}legend{float:left;width:100%;padding:0;margin-bottom:.5rem;font-size:calc(1.275rem + .3vw);line-height:inherit}@media (min-width: 1200px){legend{font-size:1.5rem}}legend+*{clear:left}::-webkit-datetime-edit-fields-wrapper,::-webkit-datetime-edit-text,::-webkit-datetime-edit-minute,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-year-field{padding:0}::-webkit-inner-spin-button{height:auto}[type="search"]{outline-offset:-2px;-webkit-appearance:textfield}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-color-swatch-wrapper{padding:0}::file-selector-button{font:inherit;-webkit-appearance:button}output{display:inline-block}iframe{border:0}summary{display:list-item;cursor:pointer}progress{vertical-align:baseline}[hidden]{display:none !important}.lead{font-size:1.25rem;font-weight:300}.display-1{font-size:calc(1.625rem + 4.5vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-1{font-size:5rem}}.display-2{font-size:calc(1.575rem + 3.9vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-2{font-size:4.5rem}}.display-3{font-size:calc(1.525rem + 3.3vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-3{font-size:4rem}}.display-4{font-size:calc(1.475rem + 2.7vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-4{font-size:3.5rem}}.display-5{font-size:calc(1.425rem + 2.1vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-5{font-size:3rem}}.display-6{font-size:calc(1.375rem + 1.5vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-6{font-size:2.5rem}}.list-unstyled{padding-left:0;list-style:none}.list-inline{padding-left:0;list-style:none}.list-inline-item{display:inline-block}.list-inline-item:not(:last-child){margin-right:.5rem}.initialism{font-size:.875em;text-transform:uppercase}.blockquote{margin-bottom:1rem;font-size:1.25rem}.blockquote>:last-child{margin-bottom:0}.blockquote-footer{margin-top:-1rem;margin-bottom:1rem;font-size:.875em;color:#6c757d}.blockquote-footer::before{content:"\2014\00A0"}.img-fluid{max-width:100%;height:auto}.img-thumbnail{padding:.25rem;background-color:#fff;border:1px solid var(--bs-border-color);border-radius:.375rem;max-width:100%;height:auto}.figure{display:inline-block}.figure-img{margin-bottom:.5rem;line-height:1}.figure-caption{font-size:.875em;color:#6c757d}.container,.container-fluid,.container-xxl,.container-xl,.container-lg,.container-md,.container-sm{--bs-gutter-x: 1.5rem;--bs-gutter-y: 0;width:100%;padding-right:calc(var(--bs-gutter-x) * .5);padding-left:calc(var(--bs-gutter-x) * .5);margin-right:auto;margin-left:auto}@media (min-width: 576px){.container-sm,.container{max-width:540px}}@media (min-width: 768px){.container-md,.container-sm,.container{max-width:720px}}@media (min-width: 992px){.container-lg,.container-md,.container-sm,.container{max-width:960px}}@media (min-width: 1200px){.container-xl,.container-lg,.container-md,.container-sm,.container{max-width:1140px}}@media (min-width: 1400px){.container-xxl,.container-xl,.container-lg,.container-md,.container-sm,.container{max-width:1320px}}.row{--bs-gutter-x: 1.5rem;--bs-gutter-y: 0;display:flex;display:-webkit-flex;flex-wrap:wrap;-webkit-flex-wrap:wrap;margin-top:calc(-1 * var(--bs-gutter-y));margin-right:calc(-.5 * var(--bs-gutter-x));margin-left:calc(-.5 * var(--bs-gutter-x))}.row>*{flex-shrink:0;-webkit-flex-shrink:0;width:100%;max-width:100%;padding-right:calc(var(--bs-gutter-x) * .5);padding-left:calc(var(--bs-gutter-x) * .5);margin-top:var(--bs-gutter-y)}.col{flex:1 0 0%;-webkit-flex:1 0 0%}.row-cols-auto>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.row-cols-1>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.row-cols-2>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.row-cols-3>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.row-cols-4>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.row-cols-5>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:20%}.row-cols-6>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-auto{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.col-1{flex:0 0 auto;-webkit-flex:0 0 auto;width:8.33333%}.col-2{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-3{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.col-4{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.col-5{flex:0 0 auto;-webkit-flex:0 0 auto;width:41.66667%}.col-6{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.col-7{flex:0 0 auto;-webkit-flex:0 0 auto;width:58.33333%}.col-8{flex:0 0 auto;-webkit-flex:0 0 auto;width:66.66667%}.col-9{flex:0 0 auto;-webkit-flex:0 0 auto;width:75%}.col-10{flex:0 0 auto;-webkit-flex:0 0 auto;width:83.33333%}.col-11{flex:0 0 auto;-webkit-flex:0 0 auto;width:91.66667%}.col-12{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.offset-1{margin-left:8.33333%}.offset-2{margin-left:16.66667%}.offset-3{margin-left:25%}.offset-4{margin-left:33.33333%}.offset-5{margin-left:41.66667%}.offset-6{margin-left:50%}.offset-7{margin-left:58.33333%}.offset-8{margin-left:66.66667%}.offset-9{margin-left:75%}.offset-10{margin-left:83.33333%}.offset-11{margin-left:91.66667%}.g-0,.gx-0{--bs-gutter-x: 0}.g-0,.gy-0{--bs-gutter-y: 0}.g-1,.gx-1{--bs-gutter-x: .25rem}.g-1,.gy-1{--bs-gutter-y: .25rem}.g-2,.gx-2{--bs-gutter-x: .5rem}.g-2,.gy-2{--bs-gutter-y: .5rem}.g-3,.gx-3{--bs-gutter-x: 1rem}.g-3,.gy-3{--bs-gutter-y: 1rem}.g-4,.gx-4{--bs-gutter-x: 1.5rem}.g-4,.gy-4{--bs-gutter-y: 1.5rem}.g-5,.gx-5{--bs-gutter-x: 3rem}.g-5,.gy-5{--bs-gutter-y: 3rem}@media (min-width: 576px){.col-sm{flex:1 0 0%;-webkit-flex:1 0 0%}.row-cols-sm-auto>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.row-cols-sm-1>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.row-cols-sm-2>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.row-cols-sm-3>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.row-cols-sm-4>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.row-cols-sm-5>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:20%}.row-cols-sm-6>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-sm-auto{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.col-sm-1{flex:0 0 auto;-webkit-flex:0 0 auto;width:8.33333%}.col-sm-2{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-sm-3{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.col-sm-4{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.col-sm-5{flex:0 0 auto;-webkit-flex:0 0 auto;width:41.66667%}.col-sm-6{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.col-sm-7{flex:0 0 auto;-webkit-flex:0 0 auto;width:58.33333%}.col-sm-8{flex:0 0 auto;-webkit-flex:0 0 auto;width:66.66667%}.col-sm-9{flex:0 0 auto;-webkit-flex:0 0 auto;width:75%}.col-sm-10{flex:0 0 auto;-webkit-flex:0 0 auto;width:83.33333%}.col-sm-11{flex:0 0 auto;-webkit-flex:0 0 auto;width:91.66667%}.col-sm-12{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.offset-sm-0{margin-left:0}.offset-sm-1{margin-left:8.33333%}.offset-sm-2{margin-left:16.66667%}.offset-sm-3{margin-left:25%}.offset-sm-4{margin-left:33.33333%}.offset-sm-5{margin-left:41.66667%}.offset-sm-6{margin-left:50%}.offset-sm-7{margin-left:58.33333%}.offset-sm-8{margin-left:66.66667%}.offset-sm-9{margin-left:75%}.offset-sm-10{margin-left:83.33333%}.offset-sm-11{margin-left:91.66667%}.g-sm-0,.gx-sm-0{--bs-gutter-x: 0}.g-sm-0,.gy-sm-0{--bs-gutter-y: 0}.g-sm-1,.gx-sm-1{--bs-gutter-x: .25rem}.g-sm-1,.gy-sm-1{--bs-gutter-y: .25rem}.g-sm-2,.gx-sm-2{--bs-gutter-x: .5rem}.g-sm-2,.gy-sm-2{--bs-gutter-y: .5rem}.g-sm-3,.gx-sm-3{--bs-gutter-x: 1rem}.g-sm-3,.gy-sm-3{--bs-gutter-y: 1rem}.g-sm-4,.gx-sm-4{--bs-gutter-x: 1.5rem}.g-sm-4,.gy-sm-4{--bs-gutter-y: 1.5rem}.g-sm-5,.gx-sm-5{--bs-gutter-x: 3rem}.g-sm-5,.gy-sm-5{--bs-gutter-y: 3rem}}@media (min-width: 768px){.col-md{flex:1 0 0%;-webkit-flex:1 0 0%}.row-cols-md-auto>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.row-cols-md-1>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.row-cols-md-2>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.row-cols-md-3>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.row-cols-md-4>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.row-cols-md-5>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:20%}.row-cols-md-6>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-md-auto{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.col-md-1{flex:0 0 auto;-webkit-flex:0 0 auto;width:8.33333%}.col-md-2{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-md-3{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.col-md-4{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.col-md-5{flex:0 0 auto;-webkit-flex:0 0 auto;width:41.66667%}.col-md-6{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.col-md-7{flex:0 0 auto;-webkit-flex:0 0 auto;width:58.33333%}.col-md-8{flex:0 0 auto;-webkit-flex:0 0 auto;width:66.66667%}.col-md-9{flex:0 0 auto;-webkit-flex:0 0 auto;width:75%}.col-md-10{flex:0 0 auto;-webkit-flex:0 0 auto;width:83.33333%}.col-md-11{flex:0 0 auto;-webkit-flex:0 0 auto;width:91.66667%}.col-md-12{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.offset-md-0{margin-left:0}.offset-md-1{margin-left:8.33333%}.offset-md-2{margin-left:16.66667%}.offset-md-3{margin-left:25%}.offset-md-4{margin-left:33.33333%}.offset-md-5{margin-left:41.66667%}.offset-md-6{margin-left:50%}.offset-md-7{margin-left:58.33333%}.offset-md-8{margin-left:66.66667%}.offset-md-9{margin-left:75%}.offset-md-10{margin-left:83.33333%}.offset-md-11{margin-left:91.66667%}.g-md-0,.gx-md-0{--bs-gutter-x: 0}.g-md-0,.gy-md-0{--bs-gutter-y: 0}.g-md-1,.gx-md-1{--bs-gutter-x: .25rem}.g-md-1,.gy-md-1{--bs-gutter-y: .25rem}.g-md-2,.gx-md-2{--bs-gutter-x: .5rem}.g-md-2,.gy-md-2{--bs-gutter-y: .5rem}.g-md-3,.gx-md-3{--bs-gutter-x: 1rem}.g-md-3,.gy-md-3{--bs-gutter-y: 1rem}.g-md-4,.gx-md-4{--bs-gutter-x: 1.5rem}.g-md-4,.gy-md-4{--bs-gutter-y: 1.5rem}.g-md-5,.gx-md-5{--bs-gutter-x: 3rem}.g-md-5,.gy-md-5{--bs-gutter-y: 3rem}}@media (min-width: 992px){.col-lg{flex:1 0 0%;-webkit-flex:1 0 0%}.row-cols-lg-auto>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.row-cols-lg-1>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.row-cols-lg-2>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.row-cols-lg-3>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.row-cols-lg-4>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.row-cols-lg-5>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:20%}.row-cols-lg-6>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-lg-auto{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.col-lg-1{flex:0 0 auto;-webkit-flex:0 0 auto;width:8.33333%}.col-lg-2{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-lg-3{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.col-lg-4{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.col-lg-5{flex:0 0 auto;-webkit-flex:0 0 auto;width:41.66667%}.col-lg-6{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.col-lg-7{flex:0 0 auto;-webkit-flex:0 0 auto;width:58.33333%}.col-lg-8{flex:0 0 auto;-webkit-flex:0 0 auto;width:66.66667%}.col-lg-9{flex:0 0 auto;-webkit-flex:0 0 auto;width:75%}.col-lg-10{flex:0 0 auto;-webkit-flex:0 0 auto;width:83.33333%}.col-lg-11{flex:0 0 auto;-webkit-flex:0 0 auto;width:91.66667%}.col-lg-12{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.offset-lg-0{margin-left:0}.offset-lg-1{margin-left:8.33333%}.offset-lg-2{margin-left:16.66667%}.offset-lg-3{margin-left:25%}.offset-lg-4{margin-left:33.33333%}.offset-lg-5{margin-left:41.66667%}.offset-lg-6{margin-left:50%}.offset-lg-7{margin-left:58.33333%}.offset-lg-8{margin-left:66.66667%}.offset-lg-9{margin-left:75%}.offset-lg-10{margin-left:83.33333%}.offset-lg-11{margin-left:91.66667%}.g-lg-0,.gx-lg-0{--bs-gutter-x: 0}.g-lg-0,.gy-lg-0{--bs-gutter-y: 0}.g-lg-1,.gx-lg-1{--bs-gutter-x: .25rem}.g-lg-1,.gy-lg-1{--bs-gutter-y: .25rem}.g-lg-2,.gx-lg-2{--bs-gutter-x: .5rem}.g-lg-2,.gy-lg-2{--bs-gutter-y: .5rem}.g-lg-3,.gx-lg-3{--bs-gutter-x: 1rem}.g-lg-3,.gy-lg-3{--bs-gutter-y: 1rem}.g-lg-4,.gx-lg-4{--bs-gutter-x: 1.5rem}.g-lg-4,.gy-lg-4{--bs-gutter-y: 1.5rem}.g-lg-5,.gx-lg-5{--bs-gutter-x: 3rem}.g-lg-5,.gy-lg-5{--bs-gutter-y: 3rem}}@media (min-width: 1200px){.col-xl{flex:1 0 0%;-webkit-flex:1 0 0%}.row-cols-xl-auto>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.row-cols-xl-1>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.row-cols-xl-2>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.row-cols-xl-3>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.row-cols-xl-4>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.row-cols-xl-5>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:20%}.row-cols-xl-6>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-xl-auto{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.col-xl-1{flex:0 0 auto;-webkit-flex:0 0 auto;width:8.33333%}.col-xl-2{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-xl-3{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.col-xl-4{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.col-xl-5{flex:0 0 auto;-webkit-flex:0 0 auto;width:41.66667%}.col-xl-6{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.col-xl-7{flex:0 0 auto;-webkit-flex:0 0 auto;width:58.33333%}.col-xl-8{flex:0 0 auto;-webkit-flex:0 0 auto;width:66.66667%}.col-xl-9{flex:0 0 auto;-webkit-flex:0 0 auto;width:75%}.col-xl-10{flex:0 0 auto;-webkit-flex:0 0 auto;width:83.33333%}.col-xl-11{flex:0 0 auto;-webkit-flex:0 0 auto;width:91.66667%}.col-xl-12{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.offset-xl-0{margin-left:0}.offset-xl-1{margin-left:8.33333%}.offset-xl-2{margin-left:16.66667%}.offset-xl-3{margin-left:25%}.offset-xl-4{margin-left:33.33333%}.offset-xl-5{margin-left:41.66667%}.offset-xl-6{margin-left:50%}.offset-xl-7{margin-left:58.33333%}.offset-xl-8{margin-left:66.66667%}.offset-xl-9{margin-left:75%}.offset-xl-10{margin-left:83.33333%}.offset-xl-11{margin-left:91.66667%}.g-xl-0,.gx-xl-0{--bs-gutter-x: 0}.g-xl-0,.gy-xl-0{--bs-gutter-y: 0}.g-xl-1,.gx-xl-1{--bs-gutter-x: .25rem}.g-xl-1,.gy-xl-1{--bs-gutter-y: .25rem}.g-xl-2,.gx-xl-2{--bs-gutter-x: .5rem}.g-xl-2,.gy-xl-2{--bs-gutter-y: .5rem}.g-xl-3,.gx-xl-3{--bs-gutter-x: 1rem}.g-xl-3,.gy-xl-3{--bs-gutter-y: 1rem}.g-xl-4,.gx-xl-4{--bs-gutter-x: 1.5rem}.g-xl-4,.gy-xl-4{--bs-gutter-y: 1.5rem}.g-xl-5,.gx-xl-5{--bs-gutter-x: 3rem}.g-xl-5,.gy-xl-5{--bs-gutter-y: 3rem}}@media (min-width: 1400px){.col-xxl{flex:1 0 0%;-webkit-flex:1 0 0%}.row-cols-xxl-auto>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.row-cols-xxl-1>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.row-cols-xxl-2>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.row-cols-xxl-3>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.row-cols-xxl-4>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.row-cols-xxl-5>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:20%}.row-cols-xxl-6>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-xxl-auto{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.col-xxl-1{flex:0 0 auto;-webkit-flex:0 0 auto;width:8.33333%}.col-xxl-2{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-xxl-3{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.col-xxl-4{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.col-xxl-5{flex:0 0 auto;-webkit-flex:0 0 auto;width:41.66667%}.col-xxl-6{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.col-xxl-7{flex:0 0 auto;-webkit-flex:0 0 auto;width:58.33333%}.col-xxl-8{flex:0 0 auto;-webkit-flex:0 0 auto;width:66.66667%}.col-xxl-9{flex:0 0 auto;-webkit-flex:0 0 auto;width:75%}.col-xxl-10{flex:0 0 auto;-webkit-flex:0 0 auto;width:83.33333%}.col-xxl-11{flex:0 0 auto;-webkit-flex:0 0 auto;width:91.66667%}.col-xxl-12{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.offset-xxl-0{margin-left:0}.offset-xxl-1{margin-left:8.33333%}.offset-xxl-2{margin-left:16.66667%}.offset-xxl-3{margin-left:25%}.offset-xxl-4{margin-left:33.33333%}.offset-xxl-5{margin-left:41.66667%}.offset-xxl-6{margin-left:50%}.offset-xxl-7{margin-left:58.33333%}.offset-xxl-8{margin-left:66.66667%}.offset-xxl-9{margin-left:75%}.offset-xxl-10{margin-left:83.33333%}.offset-xxl-11{margin-left:91.66667%}.g-xxl-0,.gx-xxl-0{--bs-gutter-x: 0}.g-xxl-0,.gy-xxl-0{--bs-gutter-y: 0}.g-xxl-1,.gx-xxl-1{--bs-gutter-x: .25rem}.g-xxl-1,.gy-xxl-1{--bs-gutter-y: .25rem}.g-xxl-2,.gx-xxl-2{--bs-gutter-x: .5rem}.g-xxl-2,.gy-xxl-2{--bs-gutter-y: .5rem}.g-xxl-3,.gx-xxl-3{--bs-gutter-x: 1rem}.g-xxl-3,.gy-xxl-3{--bs-gutter-y: 1rem}.g-xxl-4,.gx-xxl-4{--bs-gutter-x: 1.5rem}.g-xxl-4,.gy-xxl-4{--bs-gutter-y: 1.5rem}.g-xxl-5,.gx-xxl-5{--bs-gutter-x: 3rem}.g-xxl-5,.gy-xxl-5{--bs-gutter-y: 3rem}}.table{--bs-table-color: var(--bs-body-color);--bs-table-bg: rgba(0,0,0,0);--bs-table-border-color: var(--bs-border-color);--bs-table-accent-bg: rgba(0,0,0,0);--bs-table-striped-color: var(--bs-body-color);--bs-table-striped-bg: rgba(0,0,0,0.05);--bs-table-active-color: var(--bs-body-color);--bs-table-active-bg: rgba(0,0,0,0.1);--bs-table-hover-color: var(--bs-body-color);--bs-table-hover-bg: rgba(0,0,0,0.075);width:100%;margin-bottom:1rem;color:var(--bs-table-color);vertical-align:top;border-color:var(--bs-table-border-color)}.table>:not(caption)>*>*{padding:.5rem .5rem;background-color:var(--bs-table-bg);border-bottom-width:1px;box-shadow:inset 0 0 0 9999px var(--bs-table-accent-bg)}.table>tbody{vertical-align:inherit}.table>thead{vertical-align:bottom}.table-group-divider{border-top:2px solid currentcolor}.caption-top{caption-side:top}.table-sm>:not(caption)>*>*{padding:.25rem .25rem}.table-bordered>:not(caption)>*{border-width:1px 0}.table-bordered>:not(caption)>*>*{border-width:0 1px}.table-borderless>:not(caption)>*>*{border-bottom-width:0}.table-borderless>:not(:first-child){border-top-width:0}.table-striped>tbody>tr:nth-of-type(odd)>*{--bs-table-accent-bg: var(--bs-table-striped-bg);color:var(--bs-table-striped-color)}.table-striped-columns>:not(caption)>tr>:nth-child(even){--bs-table-accent-bg: var(--bs-table-striped-bg);color:var(--bs-table-striped-color)}.table-active{--bs-table-accent-bg: var(--bs-table-active-bg);color:var(--bs-table-active-color)}.table-hover>tbody>tr:hover>*{--bs-table-accent-bg: var(--bs-table-hover-bg);color:var(--bs-table-hover-color)}.table-primary{--bs-table-color: #000;--bs-table-bg: #cfe2ff;--bs-table-border-color: #bacbe6;--bs-table-striped-bg: #c5d7f2;--bs-table-striped-color: #000;--bs-table-active-bg: #bacbe6;--bs-table-active-color: #000;--bs-table-hover-bg: #bfd1ec;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-secondary{--bs-table-color: #000;--bs-table-bg: #e2e3e5;--bs-table-border-color: #cbccce;--bs-table-striped-bg: #d7d8da;--bs-table-striped-color: #000;--bs-table-active-bg: #cbccce;--bs-table-active-color: #000;--bs-table-hover-bg: #d1d2d4;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-success{--bs-table-color: #000;--bs-table-bg: #d1e7dd;--bs-table-border-color: #bcd0c7;--bs-table-striped-bg: #c7dbd2;--bs-table-striped-color: #000;--bs-table-active-bg: #bcd0c7;--bs-table-active-color: #000;--bs-table-hover-bg: #c1d6cc;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-info{--bs-table-color: #000;--bs-table-bg: #cff4fc;--bs-table-border-color: #badce3;--bs-table-striped-bg: #c5e8ef;--bs-table-striped-color: #000;--bs-table-active-bg: #badce3;--bs-table-active-color: #000;--bs-table-hover-bg: #bfe2e9;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-warning{--bs-table-color: #000;--bs-table-bg: #fff3cd;--bs-table-border-color: #e6dbb9;--bs-table-striped-bg: #f2e7c3;--bs-table-striped-color: #000;--bs-table-active-bg: #e6dbb9;--bs-table-active-color: #000;--bs-table-hover-bg: #ece1be;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-danger{--bs-table-color: #000;--bs-table-bg: #f8d7da;--bs-table-border-color: #dfc2c4;--bs-table-striped-bg: #eccccf;--bs-table-striped-color: #000;--bs-table-active-bg: #dfc2c4;--bs-table-active-color: #000;--bs-table-hover-bg: #e5c7ca;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-light{--bs-table-color: #000;--bs-table-bg: #f8f9fa;--bs-table-border-color: #dfe0e1;--bs-table-striped-bg: #ecedee;--bs-table-striped-color: #000;--bs-table-active-bg: #dfe0e1;--bs-table-active-color: #000;--bs-table-hover-bg: #e5e6e7;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-dark{--bs-table-color: #fff;--bs-table-bg: #212529;--bs-table-border-color: #373b3e;--bs-table-striped-bg: #2c3034;--bs-table-striped-color: #fff;--bs-table-active-bg: #373b3e;--bs-table-active-color: #fff;--bs-table-hover-bg: #323539;--bs-table-hover-color: #fff;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-responsive{overflow-x:auto;-webkit-overflow-scrolling:touch}@media (max-width: 575.98px){.table-responsive-sm{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 767.98px){.table-responsive-md{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 991.98px){.table-responsive-lg{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 1199.98px){.table-responsive-xl{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 1399.98px){.table-responsive-xxl{overflow-x:auto;-webkit-overflow-scrolling:touch}}.form-label,.shiny-input-container .control-label{margin-bottom:.5rem}.col-form-label{padding-top:calc(.375rem + 1px);padding-bottom:calc(.375rem + 1px);margin-bottom:0;font-size:inherit;line-height:1.5}.col-form-label-lg{padding-top:calc(.5rem + 1px);padding-bottom:calc(.5rem + 1px);font-size:1.25rem}.col-form-label-sm{padding-top:calc(.25rem + 1px);padding-bottom:calc(.25rem + 1px);font-size:.875rem}.form-text,.help-text,.help-block{margin-top:.25rem;font-size:.875em;color:#6c757d}.form-control{display:block;width:100%;padding:.375rem .75rem;font-size:1rem;font-weight:400;line-height:1.5;color:#212529;background-color:#fff;background-clip:padding-box;border:1px solid #ced4da;appearance:none;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;-o-appearance:none;border-radius:.375rem;transition:border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-control{transition:none}}.form-control[type="file"]{overflow:hidden}.form-control[type="file"]:not(:disabled):not([readonly]){cursor:pointer}.form-control:focus{color:#212529;background-color:#fff;border-color:#86b7fe;outline:0;box-shadow:0 0 0 .25rem rgba(13,110,253,0.25)}.form-control::-webkit-date-and-time-value{height:1.5em}.form-control::placeholder{color:#6c757d;opacity:1}.form-control:disabled{background-color:#e9ecef;opacity:1}.form-control::file-selector-button{padding:.375rem .75rem;margin:-.375rem -.75rem;margin-inline-end:.75rem;color:#212529;background-color:#e9ecef;pointer-events:none;border-color:inherit;border-style:solid;border-width:0;border-inline-end-width:1px;border-radius:0;transition:color 0.15s ease-in-out,background-color 0.15s ease-in-out,border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-control::file-selector-button{transition:none}}.form-control:hover:not(:disabled):not([readonly])::file-selector-button{background-color:#dde0e3}.form-control-plaintext{display:block;width:100%;padding:.375rem 0;margin-bottom:0;line-height:1.5;color:#212529;background-color:transparent;border:solid transparent;border-width:1px 0}.form-control-plaintext:focus{outline:0}.form-control-plaintext.form-control-sm,.form-control-plaintext.form-control-lg{padding-right:0;padding-left:0}.form-control-sm{min-height:calc(1.5em + .5rem + 2px);padding:.25rem .5rem;font-size:.875rem;border-radius:.25rem}.form-control-sm::file-selector-button{padding:.25rem .5rem;margin:-.25rem -.5rem;margin-inline-end:.5rem}.form-control-lg{min-height:calc(1.5em + 1rem + 2px);padding:.5rem 1rem;font-size:1.25rem;border-radius:.5rem}.form-control-lg::file-selector-button{padding:.5rem 1rem;margin:-.5rem -1rem;margin-inline-end:1rem}textarea.form-control{min-height:calc(1.5em + .75rem + 2px)}textarea.form-control-sm{min-height:calc(1.5em + .5rem + 2px)}textarea.form-control-lg{min-height:calc(1.5em + 1rem + 2px)}.form-control-color{width:3rem;height:calc(1.5em + .75rem + 2px);padding:.375rem}.form-control-color:not(:disabled):not([readonly]){cursor:pointer}.form-control-color::-moz-color-swatch{border:0 !important;border-radius:.375rem}.form-control-color::-webkit-color-swatch{border-radius:.375rem}.form-control-color.form-control-sm{height:calc(1.5em + .5rem + 2px)}.form-control-color.form-control-lg{height:calc(1.5em + 1rem + 2px)}.form-select{display:block;width:100%;padding:.375rem 2.25rem .375rem .75rem;-moz-padding-start:calc(.75rem - 3px);font-size:1rem;font-weight:400;line-height:1.5;color:#212529;background-color:#fff;background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e");background-repeat:no-repeat;background-position:right .75rem center;background-size:16px 12px;border:1px solid #ced4da;border-radius:.375rem;transition:border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out;appearance:none;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;-o-appearance:none}@media (prefers-reduced-motion: reduce){.form-select{transition:none}}.form-select:focus{border-color:#86b7fe;outline:0;box-shadow:0 0 0 .25rem rgba(13,110,253,0.25)}.form-select[multiple],.form-select[size]:not([size="1"]){padding-right:.75rem;background-image:none}.form-select:disabled{background-color:#e9ecef}.form-select:-moz-focusring{color:transparent;text-shadow:0 0 0 #212529}.form-select-sm{padding-top:.25rem;padding-bottom:.25rem;padding-left:.5rem;font-size:.875rem;border-radius:.25rem}.form-select-lg{padding-top:.5rem;padding-bottom:.5rem;padding-left:1rem;font-size:1.25rem;border-radius:.5rem}.form-check,.shiny-input-container .checkbox,.shiny-input-container .radio{display:block;min-height:1.5rem;padding-left:0;margin-bottom:.125rem}.form-check .form-check-input,.form-check .shiny-input-container .checkbox input,.form-check .shiny-input-container .radio input,.shiny-input-container .checkbox .form-check-input,.shiny-input-container .checkbox .shiny-input-container .checkbox input,.shiny-input-container .checkbox .shiny-input-container .radio input,.shiny-input-container .radio .form-check-input,.shiny-input-container .radio .shiny-input-container .checkbox input,.shiny-input-container .radio .shiny-input-container .radio input{float:left;margin-left:0}.form-check-reverse{padding-right:0;padding-left:0;text-align:right}.form-check-reverse .form-check-input{float:right;margin-right:0;margin-left:0}.form-check-input,.shiny-input-container .checkbox input,.shiny-input-container .checkbox-inline input,.shiny-input-container .radio input,.shiny-input-container .radio-inline input{width:1em;height:1em;margin-top:.25em;vertical-align:top;background-color:#fff;background-repeat:no-repeat;background-position:center;background-size:contain;border:1px solid rgba(0,0,0,0.25);appearance:none;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;-o-appearance:none;print-color-adjust:exact}.form-check-input[type="checkbox"],.shiny-input-container .checkbox input[type="checkbox"],.shiny-input-container .checkbox-inline input[type="checkbox"],.shiny-input-container .radio input[type="checkbox"],.shiny-input-container .radio-inline input[type="checkbox"]{border-radius:.25em}.form-check-input[type="radio"],.shiny-input-container .checkbox input[type="radio"],.shiny-input-container .checkbox-inline input[type="radio"],.shiny-input-container .radio input[type="radio"],.shiny-input-container .radio-inline input[type="radio"]{border-radius:50%}.form-check-input:active,.shiny-input-container .checkbox input:active,.shiny-input-container .checkbox-inline input:active,.shiny-input-container .radio input:active,.shiny-input-container .radio-inline input:active{filter:brightness(90%)}.form-check-input:focus,.shiny-input-container .checkbox input:focus,.shiny-input-container .checkbox-inline input:focus,.shiny-input-container .radio input:focus,.shiny-input-container .radio-inline input:focus{border-color:#86b7fe;outline:0;box-shadow:0 0 0 .25rem rgba(13,110,253,0.25)}.form-check-input:checked,.shiny-input-container .checkbox input:checked,.shiny-input-container .checkbox-inline input:checked,.shiny-input-container .radio input:checked,.shiny-input-container .radio-inline input:checked{background-color:#0d6efd;border-color:#0d6efd}.form-check-input:checked[type="checkbox"],.shiny-input-container .checkbox input:checked[type="checkbox"],.shiny-input-container .checkbox-inline input:checked[type="checkbox"],.shiny-input-container .radio input:checked[type="checkbox"],.shiny-input-container .radio-inline input:checked[type="checkbox"]{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='m6 10 3 3 6-6'/%3e%3c/svg%3e")}.form-check-input:checked[type="radio"],.shiny-input-container .checkbox input:checked[type="radio"],.shiny-input-container .checkbox-inline input:checked[type="radio"],.shiny-input-container .radio input:checked[type="radio"],.shiny-input-container .radio-inline input:checked[type="radio"]{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='2' fill='%23fff'/%3e%3c/svg%3e")}.form-check-input[type="checkbox"]:indeterminate,.shiny-input-container .checkbox input[type="checkbox"]:indeterminate,.shiny-input-container .checkbox-inline input[type="checkbox"]:indeterminate,.shiny-input-container .radio input[type="checkbox"]:indeterminate,.shiny-input-container .radio-inline input[type="checkbox"]:indeterminate{background-color:#0d6efd;border-color:#0d6efd;background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='M6 10h8'/%3e%3c/svg%3e")}.form-check-input:disabled,.shiny-input-container .checkbox input:disabled,.shiny-input-container .checkbox-inline input:disabled,.shiny-input-container .radio input:disabled,.shiny-input-container .radio-inline input:disabled{pointer-events:none;filter:none;opacity:.5}.form-check-input[disabled]~.form-check-label,.form-check-input[disabled]~span,.form-check-input:disabled~.form-check-label,.form-check-input:disabled~span,.shiny-input-container .checkbox input[disabled]~.form-check-label,.shiny-input-container .checkbox input[disabled]~span,.shiny-input-container .checkbox input:disabled~.form-check-label,.shiny-input-container .checkbox input:disabled~span,.shiny-input-container .checkbox-inline input[disabled]~.form-check-label,.shiny-input-container .checkbox-inline input[disabled]~span,.shiny-input-container .checkbox-inline input:disabled~.form-check-label,.shiny-input-container .checkbox-inline input:disabled~span,.shiny-input-container .radio input[disabled]~.form-check-label,.shiny-input-container .radio input[disabled]~span,.shiny-input-container .radio input:disabled~.form-check-label,.shiny-input-container .radio input:disabled~span,.shiny-input-container .radio-inline input[disabled]~.form-check-label,.shiny-input-container .radio-inline input[disabled]~span,.shiny-input-container .radio-inline input:disabled~.form-check-label,.shiny-input-container .radio-inline input:disabled~span{cursor:default;opacity:.5}.form-check-label,.shiny-input-container .checkbox label,.shiny-input-container .checkbox-inline label,.shiny-input-container .radio label,.shiny-input-container .radio-inline label{cursor:pointer}.form-switch{padding-left:2.5em}.form-switch .form-check-input{width:2em;margin-left:-2.5em;background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='rgba%280,0,0,0.25%29'/%3e%3c/svg%3e");background-position:left center;border-radius:2em;transition:background-position 0.15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-switch .form-check-input{transition:none}}.form-switch .form-check-input:focus{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%2386b7fe'/%3e%3c/svg%3e")}.form-switch .form-check-input:checked{background-position:right center;background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%23fff'/%3e%3c/svg%3e")}.form-switch.form-check-reverse{padding-right:2.5em;padding-left:0}.form-switch.form-check-reverse .form-check-input{margin-right:-2.5em;margin-left:0}.form-check-inline{display:inline-block;margin-right:1rem}.btn-check{position:absolute;clip:rect(0, 0, 0, 0);pointer-events:none}.btn-check[disabled]+.btn,.btn-check:disabled+.btn{pointer-events:none;filter:none;opacity:.65}.form-range{width:100%;height:1.5rem;padding:0;background-color:transparent;appearance:none;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;-o-appearance:none}.form-range:focus{outline:0}.form-range:focus::-webkit-slider-thumb{box-shadow:0 0 0 1px #fff,0 0 0 .25rem rgba(13,110,253,0.25)}.form-range:focus::-moz-range-thumb{box-shadow:0 0 0 1px #fff,0 0 0 .25rem rgba(13,110,253,0.25)}.form-range::-moz-focus-outer{border:0}.form-range::-webkit-slider-thumb{width:1rem;height:1rem;margin-top:-.25rem;background-color:#0d6efd;border:0;border-radius:1rem;transition:background-color 0.15s ease-in-out,border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out;appearance:none;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;-o-appearance:none}@media (prefers-reduced-motion: reduce){.form-range::-webkit-slider-thumb{transition:none}}.form-range::-webkit-slider-thumb:active{background-color:#b6d4fe}.form-range::-webkit-slider-runnable-track{width:100%;height:.5rem;color:transparent;cursor:pointer;background-color:#dee2e6;border-color:transparent;border-radius:1rem}.form-range::-moz-range-thumb{width:1rem;height:1rem;background-color:#0d6efd;border:0;border-radius:1rem;transition:background-color 0.15s ease-in-out,border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out;appearance:none;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;-o-appearance:none}@media (prefers-reduced-motion: reduce){.form-range::-moz-range-thumb{transition:none}}.form-range::-moz-range-thumb:active{background-color:#b6d4fe}.form-range::-moz-range-track{width:100%;height:.5rem;color:transparent;cursor:pointer;background-color:#dee2e6;border-color:transparent;border-radius:1rem}.form-range:disabled{pointer-events:none}.form-range:disabled::-webkit-slider-thumb{background-color:#adb5bd}.form-range:disabled::-moz-range-thumb{background-color:#adb5bd}.form-floating{position:relative}.form-floating>.form-control,.form-floating>.form-control-plaintext,.form-floating>.form-select{height:calc(3.5rem + 2px);line-height:1.25}.form-floating>label{position:absolute;top:0;left:0;width:100%;height:100%;padding:1rem .75rem;overflow:hidden;text-align:start;text-overflow:ellipsis;white-space:nowrap;pointer-events:none;border:1px solid transparent;transform-origin:0 0;transition:opacity 0.1s ease-in-out,transform 0.1s ease-in-out}@media (prefers-reduced-motion: reduce){.form-floating>label{transition:none}}.form-floating>.form-control,.form-floating>.form-control-plaintext{padding:1rem .75rem}.form-floating>.form-control::placeholder,.form-floating>.form-control-plaintext::placeholder{color:transparent}.form-floating>.form-control:focus,.form-floating>.form-control:not(:placeholder-shown),.form-floating>.form-control-plaintext:focus,.form-floating>.form-control-plaintext:not(:placeholder-shown){padding-top:1.625rem;padding-bottom:.625rem}.form-floating>.form-control:-webkit-autofill,.form-floating>.form-control-plaintext:-webkit-autofill{padding-top:1.625rem;padding-bottom:.625rem}.form-floating>.form-select{padding-top:1.625rem;padding-bottom:.625rem}.form-floating>.form-control:focus~label,.form-floating>.form-control:not(:placeholder-shown)~label,.form-floating>.form-control-plaintext~label,.form-floating>.form-select~label{opacity:.65;transform:scale(0.85) translateY(-0.5rem) translateX(0.15rem)}.form-floating>.form-control:-webkit-autofill~label{opacity:.65;transform:scale(0.85) translateY(-0.5rem) translateX(0.15rem)}.form-floating>.form-control-plaintext~label{border-width:1px 0}.input-group{position:relative;display:flex;display:-webkit-flex;flex-wrap:wrap;-webkit-flex-wrap:wrap;align-items:stretch;-webkit-align-items:stretch;width:100%}.input-group>.form-control,.input-group>.form-select,.input-group>.form-floating{position:relative;flex:1 1 auto;-webkit-flex:1 1 auto;width:1%;min-width:0}.input-group>.form-control:focus,.input-group>.form-select:focus,.input-group>.form-floating:focus-within{z-index:5}.input-group .btn{position:relative;z-index:2}.input-group .btn:focus{z-index:5}.input-group-text{display:flex;display:-webkit-flex;align-items:center;-webkit-align-items:center;padding:.375rem .75rem;font-size:1rem;font-weight:400;line-height:1.5;color:#212529;text-align:center;white-space:nowrap;background-color:#e9ecef;border:1px solid #ced4da;border-radius:.375rem}.input-group-lg>.form-control,.input-group-lg>.form-select,.input-group-lg>.input-group-text,.input-group-lg>.btn{padding:.5rem 1rem;font-size:1.25rem;border-radius:.5rem}.input-group-sm>.form-control,.input-group-sm>.form-select,.input-group-sm>.input-group-text,.input-group-sm>.btn{padding:.25rem .5rem;font-size:.875rem;border-radius:.25rem}.input-group-lg>.form-select,.input-group-sm>.form-select{padding-right:3rem}.input-group:not(.has-validation)>:not(:last-child):not(.dropdown-toggle):not(.dropdown-menu):not(.form-floating),.input-group:not(.has-validation)>.dropdown-toggle:nth-last-child(n + 3),.input-group:not(.has-validation)>.form-floating:not(:last-child)>.form-control,.input-group:not(.has-validation)>.form-floating:not(:last-child)>.form-select{border-top-right-radius:0;border-bottom-right-radius:0}.input-group.has-validation>:nth-last-child(n + 3):not(.dropdown-toggle):not(.dropdown-menu):not(.form-floating),.input-group.has-validation>.dropdown-toggle:nth-last-child(n + 4),.input-group.has-validation>.form-floating:nth-last-child(n + 3)>.form-control,.input-group.has-validation>.form-floating:nth-last-child(n + 3)>.form-select{border-top-right-radius:0;border-bottom-right-radius:0}.input-group>:not(:first-child):not(.dropdown-menu):not(.valid-tooltip):not(.valid-feedback):not(.invalid-tooltip):not(.invalid-feedback){margin-left:-1px;border-top-left-radius:0;border-bottom-left-radius:0}.input-group>.form-floating:not(:first-child)>.form-control,.input-group>.form-floating:not(:first-child)>.form-select{border-top-left-radius:0;border-bottom-left-radius:0}.valid-feedback{display:none;width:100%;margin-top:.25rem;font-size:.875em;color:#198754}.valid-tooltip{position:absolute;top:100%;z-index:5;display:none;max-width:100%;padding:.25rem .5rem;margin-top:.1rem;font-size:.875rem;color:#fff;background-color:rgba(25,135,84,0.9);border-radius:.375rem}.was-validated :valid~.valid-feedback,.was-validated :valid~.valid-tooltip,.is-valid~.valid-feedback,.is-valid~.valid-tooltip{display:block}.was-validated .form-control:valid,.form-control.is-valid{border-color:#198754;padding-right:calc(1.5em + .75rem);background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");background-repeat:no-repeat;background-position:right calc(.375em + .1875rem) center;background-size:calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-control:valid:focus,.form-control.is-valid:focus{border-color:#198754;box-shadow:0 0 0 .25rem rgba(25,135,84,0.25)}.was-validated textarea.form-control:valid,textarea.form-control.is-valid{padding-right:calc(1.5em + .75rem);background-position:top calc(.375em + .1875rem) right calc(.375em + .1875rem)}.was-validated .form-select:valid,.form-select.is-valid{border-color:#198754}.was-validated .form-select:valid:not([multiple]):not([size]),.was-validated .form-select:valid:not([multiple])[size="1"],.form-select.is-valid:not([multiple]):not([size]),.form-select.is-valid:not([multiple])[size="1"]{padding-right:4.125rem;background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e"),url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");background-position:right .75rem center,center right 2.25rem;background-size:16px 12px,calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-select:valid:focus,.form-select.is-valid:focus{border-color:#198754;box-shadow:0 0 0 .25rem rgba(25,135,84,0.25)}.was-validated .form-control-color:valid,.form-control-color.is-valid{width:calc(3rem + calc(1.5em + .75rem))}.was-validated .form-check-input:valid,.form-check-input.is-valid{border-color:#198754}.was-validated .form-check-input:valid:checked,.form-check-input.is-valid:checked{background-color:#198754}.was-validated .form-check-input:valid:focus,.form-check-input.is-valid:focus{box-shadow:0 0 0 .25rem rgba(25,135,84,0.25)}.was-validated .form-check-input:valid~.form-check-label,.form-check-input.is-valid~.form-check-label{color:#198754}.form-check-inline .form-check-input~.valid-feedback{margin-left:.5em}.was-validated .input-group>.form-control:not(:focus):valid,.input-group>.form-control:not(:focus).is-valid,.was-validated .input-group>.form-select:not(:focus):valid,.input-group>.form-select:not(:focus).is-valid,.was-validated .input-group>.form-floating:not(:focus-within):valid,.input-group>.form-floating:not(:focus-within).is-valid{z-index:3}.invalid-feedback{display:none;width:100%;margin-top:.25rem;font-size:.875em;color:#dc3545}.invalid-tooltip{position:absolute;top:100%;z-index:5;display:none;max-width:100%;padding:.25rem .5rem;margin-top:.1rem;font-size:.875rem;color:#fff;background-color:rgba(220,53,69,0.9);border-radius:.375rem}.was-validated :invalid~.invalid-feedback,.was-validated :invalid~.invalid-tooltip,.is-invalid~.invalid-feedback,.is-invalid~.invalid-tooltip{display:block}.was-validated .form-control:invalid,.form-control.is-invalid{border-color:#dc3545;padding-right:calc(1.5em + .75rem);background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");background-repeat:no-repeat;background-position:right calc(.375em + .1875rem) center;background-size:calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-control:invalid:focus,.form-control.is-invalid:focus{border-color:#dc3545;box-shadow:0 0 0 .25rem rgba(220,53,69,0.25)}.was-validated textarea.form-control:invalid,textarea.form-control.is-invalid{padding-right:calc(1.5em + .75rem);background-position:top calc(.375em + .1875rem) right calc(.375em + .1875rem)}.was-validated .form-select:invalid,.form-select.is-invalid{border-color:#dc3545}.was-validated .form-select:invalid:not([multiple]):not([size]),.was-validated .form-select:invalid:not([multiple])[size="1"],.form-select.is-invalid:not([multiple]):not([size]),.form-select.is-invalid:not([multiple])[size="1"]{padding-right:4.125rem;background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e"),url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");background-position:right .75rem center,center right 2.25rem;background-size:16px 12px,calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-select:invalid:focus,.form-select.is-invalid:focus{border-color:#dc3545;box-shadow:0 0 0 .25rem rgba(220,53,69,0.25)}.was-validated .form-control-color:invalid,.form-control-color.is-invalid{width:calc(3rem + calc(1.5em + .75rem))}.was-validated .form-check-input:invalid,.form-check-input.is-invalid{border-color:#dc3545}.was-validated .form-check-input:invalid:checked,.form-check-input.is-invalid:checked{background-color:#dc3545}.was-validated .form-check-input:invalid:focus,.form-check-input.is-invalid:focus{box-shadow:0 0 0 .25rem rgba(220,53,69,0.25)}.was-validated .form-check-input:invalid~.form-check-label,.form-check-input.is-invalid~.form-check-label{color:#dc3545}.form-check-inline .form-check-input~.invalid-feedback{margin-left:.5em}.was-validated .input-group>.form-control:not(:focus):invalid,.input-group>.form-control:not(:focus).is-invalid,.was-validated .input-group>.form-select:not(:focus):invalid,.input-group>.form-select:not(:focus).is-invalid,.was-validated .input-group>.form-floating:not(:focus-within):invalid,.input-group>.form-floating:not(:focus-within).is-invalid{z-index:4}.btn{--bs-btn-padding-x: .75rem;--bs-btn-padding-y: .375rem;--bs-btn-font-family: ;--bs-btn-font-size:1rem;--bs-btn-font-weight: 400;--bs-btn-line-height: 1.5;--bs-btn-color: #212529;--bs-btn-bg: transparent;--bs-btn-border-width: 1px;--bs-btn-border-color: transparent;--bs-btn-border-radius: .375rem;--bs-btn-hover-border-color: transparent;--bs-btn-box-shadow: inset 0 1px 0 rgba(255,255,255,0.15),0 1px 1px rgba(0,0,0,0.075);--bs-btn-disabled-opacity: .65;--bs-btn-focus-box-shadow: 0 0 0 .25rem rgba(var(--bs-btn-focus-shadow-rgb), .5);display:inline-block;padding:var(--bs-btn-padding-y) var(--bs-btn-padding-x);font-family:var(--bs-btn-font-family);font-size:var(--bs-btn-font-size);font-weight:var(--bs-btn-font-weight);line-height:var(--bs-btn-line-height);color:var(--bs-btn-color);text-align:center;text-decoration:none;-webkit-text-decoration:none;-moz-text-decoration:none;-ms-text-decoration:none;-o-text-decoration:none;vertical-align:middle;cursor:pointer;user-select:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;-o-user-select:none;border:var(--bs-btn-border-width) solid var(--bs-btn-border-color);border-radius:var(--bs-btn-border-radius);background-color:var(--bs-btn-bg);transition:color 0.15s ease-in-out,background-color 0.15s ease-in-out,border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out}@media (prefers-reduced-motion: reduce){.btn{transition:none}}.btn:hover{color:var(--bs-btn-hover-color);background-color:var(--bs-btn-hover-bg);border-color:var(--bs-btn-hover-border-color)}.btn-check+.btn:hover{color:var(--bs-btn-color);background-color:var(--bs-btn-bg);border-color:var(--bs-btn-border-color)}.btn:focus-visible{color:var(--bs-btn-hover-color);background-color:var(--bs-btn-hover-bg);border-color:var(--bs-btn-hover-border-color);outline:0;box-shadow:var(--bs-btn-focus-box-shadow)}.btn-check:focus-visible+.btn{border-color:var(--bs-btn-hover-border-color);outline:0;box-shadow:var(--bs-btn-focus-box-shadow)}.btn-check:checked+.btn,:not(.btn-check)+.btn:active,.btn:first-child:active,.btn.active,.btn.show,.btn.in{color:var(--bs-btn-active-color);background-color:var(--bs-btn-active-bg);border-color:var(--bs-btn-active-border-color)}.btn-check:checked+.btn:focus-visible,:not(.btn-check)+.btn:active:focus-visible,.btn:first-child:active:focus-visible,.btn.active:focus-visible,.btn.show:focus-visible,.btn.in:focus-visible{box-shadow:var(--bs-btn-focus-box-shadow)}.btn:disabled,.btn.disabled,fieldset:disabled .btn{color:var(--bs-btn-disabled-color);pointer-events:none;background-color:var(--bs-btn-disabled-bg);border-color:var(--bs-btn-disabled-border-color);opacity:var(--bs-btn-disabled-opacity)}.btn-default{--bs-btn-color: #000;--bs-btn-bg: #dee2e6;--bs-btn-border-color: #dee2e6;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #e3e6ea;--bs-btn-hover-border-color: #e1e5e9;--bs-btn-focus-shadow-rgb: 189,192,196;--bs-btn-active-color: #000;--bs-btn-active-bg: #e5e8eb;--bs-btn-active-border-color: #e1e5e9;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #dee2e6;--bs-btn-disabled-border-color: #dee2e6}.btn-primary{--bs-btn-color: #fff;--bs-btn-bg: #0d6efd;--bs-btn-border-color: #0d6efd;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #0b5ed7;--bs-btn-hover-border-color: #0a58ca;--bs-btn-focus-shadow-rgb: 49,132,253;--bs-btn-active-color: #fff;--bs-btn-active-bg: #0a58ca;--bs-btn-active-border-color: #0a53be;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #0d6efd;--bs-btn-disabled-border-color: #0d6efd}.btn-secondary{--bs-btn-color: #fff;--bs-btn-bg: #6c757d;--bs-btn-border-color: #6c757d;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #5c636a;--bs-btn-hover-border-color: #565e64;--bs-btn-focus-shadow-rgb: 130,138,145;--bs-btn-active-color: #fff;--bs-btn-active-bg: #565e64;--bs-btn-active-border-color: #51585e;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #6c757d;--bs-btn-disabled-border-color: #6c757d}.btn-success{--bs-btn-color: #fff;--bs-btn-bg: #198754;--bs-btn-border-color: #198754;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #157347;--bs-btn-hover-border-color: #146c43;--bs-btn-focus-shadow-rgb: 60,153,110;--bs-btn-active-color: #fff;--bs-btn-active-bg: #146c43;--bs-btn-active-border-color: #13653f;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #198754;--bs-btn-disabled-border-color: #198754}.btn-info{--bs-btn-color: #000;--bs-btn-bg: #0dcaf0;--bs-btn-border-color: #0dcaf0;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #31d2f2;--bs-btn-hover-border-color: #25cff2;--bs-btn-focus-shadow-rgb: 11,172,204;--bs-btn-active-color: #000;--bs-btn-active-bg: #3dd5f3;--bs-btn-active-border-color: #25cff2;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #0dcaf0;--bs-btn-disabled-border-color: #0dcaf0}.btn-warning{--bs-btn-color: #000;--bs-btn-bg: #ffc107;--bs-btn-border-color: #ffc107;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #ffca2c;--bs-btn-hover-border-color: #ffc720;--bs-btn-focus-shadow-rgb: 217,164,6;--bs-btn-active-color: #000;--bs-btn-active-bg: #ffcd39;--bs-btn-active-border-color: #ffc720;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #ffc107;--bs-btn-disabled-border-color: #ffc107}.btn-danger{--bs-btn-color: #fff;--bs-btn-bg: #dc3545;--bs-btn-border-color: #dc3545;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #bb2d3b;--bs-btn-hover-border-color: #b02a37;--bs-btn-focus-shadow-rgb: 225,83,97;--bs-btn-active-color: #fff;--bs-btn-active-bg: #b02a37;--bs-btn-active-border-color: #a52834;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #dc3545;--bs-btn-disabled-border-color: #dc3545}.btn-light{--bs-btn-color: #000;--bs-btn-bg: #f8f9fa;--bs-btn-border-color: #f8f9fa;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #d3d4d5;--bs-btn-hover-border-color: #c6c7c8;--bs-btn-focus-shadow-rgb: 211,212,213;--bs-btn-active-color: #000;--bs-btn-active-bg: #c6c7c8;--bs-btn-active-border-color: #babbbc;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #f8f9fa;--bs-btn-disabled-border-color: #f8f9fa}.btn-dark{--bs-btn-color: #fff;--bs-btn-bg: #212529;--bs-btn-border-color: #212529;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #424649;--bs-btn-hover-border-color: #373b3e;--bs-btn-focus-shadow-rgb: 66,70,73;--bs-btn-active-color: #fff;--bs-btn-active-bg: #4d5154;--bs-btn-active-border-color: #373b3e;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #212529;--bs-btn-disabled-border-color: #212529}.btn-outline-default{--bs-btn-color: #dee2e6;--bs-btn-border-color: #dee2e6;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #dee2e6;--bs-btn-hover-border-color: #dee2e6;--bs-btn-focus-shadow-rgb: 222,226,230;--bs-btn-active-color: #000;--bs-btn-active-bg: #dee2e6;--bs-btn-active-border-color: #dee2e6;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #dee2e6;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #dee2e6;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-primary{--bs-btn-color: #0d6efd;--bs-btn-border-color: #0d6efd;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #0d6efd;--bs-btn-hover-border-color: #0d6efd;--bs-btn-focus-shadow-rgb: 13,110,253;--bs-btn-active-color: #fff;--bs-btn-active-bg: #0d6efd;--bs-btn-active-border-color: #0d6efd;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #0d6efd;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #0d6efd;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-secondary{--bs-btn-color: #6c757d;--bs-btn-border-color: #6c757d;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #6c757d;--bs-btn-hover-border-color: #6c757d;--bs-btn-focus-shadow-rgb: 108,117,125;--bs-btn-active-color: #fff;--bs-btn-active-bg: #6c757d;--bs-btn-active-border-color: #6c757d;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #6c757d;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #6c757d;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-success{--bs-btn-color: #198754;--bs-btn-border-color: #198754;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #198754;--bs-btn-hover-border-color: #198754;--bs-btn-focus-shadow-rgb: 25,135,84;--bs-btn-active-color: #fff;--bs-btn-active-bg: #198754;--bs-btn-active-border-color: #198754;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #198754;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #198754;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-info{--bs-btn-color: #0dcaf0;--bs-btn-border-color: #0dcaf0;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #0dcaf0;--bs-btn-hover-border-color: #0dcaf0;--bs-btn-focus-shadow-rgb: 13,202,240;--bs-btn-active-color: #000;--bs-btn-active-bg: #0dcaf0;--bs-btn-active-border-color: #0dcaf0;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #0dcaf0;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #0dcaf0;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-warning{--bs-btn-color: #ffc107;--bs-btn-border-color: #ffc107;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #ffc107;--bs-btn-hover-border-color: #ffc107;--bs-btn-focus-shadow-rgb: 255,193,7;--bs-btn-active-color: #000;--bs-btn-active-bg: #ffc107;--bs-btn-active-border-color: #ffc107;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #ffc107;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #ffc107;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-danger{--bs-btn-color: #dc3545;--bs-btn-border-color: #dc3545;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #dc3545;--bs-btn-hover-border-color: #dc3545;--bs-btn-focus-shadow-rgb: 220,53,69;--bs-btn-active-color: #fff;--bs-btn-active-bg: #dc3545;--bs-btn-active-border-color: #dc3545;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #dc3545;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #dc3545;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-light{--bs-btn-color: #f8f9fa;--bs-btn-border-color: #f8f9fa;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #f8f9fa;--bs-btn-hover-border-color: #f8f9fa;--bs-btn-focus-shadow-rgb: 248,249,250;--bs-btn-active-color: #000;--bs-btn-active-bg: #f8f9fa;--bs-btn-active-border-color: #f8f9fa;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #f8f9fa;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #f8f9fa;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-dark{--bs-btn-color: #212529;--bs-btn-border-color: #212529;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #212529;--bs-btn-hover-border-color: #212529;--bs-btn-focus-shadow-rgb: 33,37,41;--bs-btn-active-color: #fff;--bs-btn-active-bg: #212529;--bs-btn-active-border-color: #212529;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #212529;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #212529;--bs-btn-bg: transparent;--bs-gradient: none}.btn-link{--bs-btn-font-weight: 400;--bs-btn-color: var(--bs-link-color);--bs-btn-bg: transparent;--bs-btn-border-color: transparent;--bs-btn-hover-color: var(--bs-link-hover-color);--bs-btn-hover-border-color: transparent;--bs-btn-active-color: var(--bs-link-hover-color);--bs-btn-active-border-color: transparent;--bs-btn-disabled-color: #6c757d;--bs-btn-disabled-border-color: transparent;--bs-btn-box-shadow: none;--bs-btn-focus-shadow-rgb: 49,132,253;text-decoration:underline;-webkit-text-decoration:underline;-moz-text-decoration:underline;-ms-text-decoration:underline;-o-text-decoration:underline}.btn-link:focus-visible{color:var(--bs-btn-color)}.btn-link:hover{color:var(--bs-btn-hover-color)}.btn-lg,.btn-group-lg>.btn{--bs-btn-padding-y: .5rem;--bs-btn-padding-x: 1rem;--bs-btn-font-size:1.25rem;--bs-btn-border-radius: .5rem}.btn-sm,.btn-group-sm>.btn{--bs-btn-padding-y: .25rem;--bs-btn-padding-x: .5rem;--bs-btn-font-size:.875rem;--bs-btn-border-radius: .25rem}.fade{transition:opacity 0.15s linear}@media (prefers-reduced-motion: reduce){.fade{transition:none}}.fade:not(.show):not(.in){opacity:0}.collapse:not(.show):not(.in){display:none}.collapsing{height:0;overflow:hidden;transition:height 0.35s ease}@media (prefers-reduced-motion: reduce){.collapsing{transition:none}}.collapsing.collapse-horizontal{width:0;height:auto;transition:width 0.35s ease}@media (prefers-reduced-motion: reduce){.collapsing.collapse-horizontal{transition:none}}.dropup,.dropend,.dropdown,.dropstart,.dropup-center,.dropdown-center{position:relative}.dropdown-toggle{white-space:nowrap}.dropdown-toggle::after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:"";border-top:.3em solid;border-right:.3em solid transparent;border-bottom:0;border-left:.3em solid transparent}.dropdown-toggle:empty::after{margin-left:0}.dropdown-menu{--bs-dropdown-zindex: 1000;--bs-dropdown-min-width: 10rem;--bs-dropdown-padding-x: 0;--bs-dropdown-padding-y: .5rem;--bs-dropdown-spacer: .125rem;--bs-dropdown-font-size:1rem;--bs-dropdown-color: #212529;--bs-dropdown-bg: #fff;--bs-dropdown-border-color: var(--bs-border-color-translucent);--bs-dropdown-border-radius: .375rem;--bs-dropdown-border-width: 1px;--bs-dropdown-inner-border-radius: calc(.375rem - 1px);--bs-dropdown-divider-bg: var(--bs-border-color-translucent);--bs-dropdown-divider-margin-y: .5rem;--bs-dropdown-box-shadow: 0 0.5rem 1rem rgba(0,0,0,0.15);--bs-dropdown-link-color: #212529;--bs-dropdown-link-hover-color: #1e2125;--bs-dropdown-link-hover-bg: #e9ecef;--bs-dropdown-link-active-color: #fff;--bs-dropdown-link-active-bg: #0d6efd;--bs-dropdown-link-disabled-color: #adb5bd;--bs-dropdown-item-padding-x: 1rem;--bs-dropdown-item-padding-y: .25rem;--bs-dropdown-header-color: #6c757d;--bs-dropdown-header-padding-x: 1rem;--bs-dropdown-header-padding-y: .5rem;position:absolute;z-index:var(--bs-dropdown-zindex);display:none;min-width:var(--bs-dropdown-min-width);padding:var(--bs-dropdown-padding-y) var(--bs-dropdown-padding-x);margin:0;font-size:var(--bs-dropdown-font-size);color:var(--bs-dropdown-color);text-align:left;list-style:none;background-color:var(--bs-dropdown-bg);background-clip:padding-box;border:var(--bs-dropdown-border-width) solid var(--bs-dropdown-border-color);border-radius:var(--bs-dropdown-border-radius)}.dropdown-menu[data-bs-popper]{top:100%;left:0;margin-top:var(--bs-dropdown-spacer)}.dropdown-menu-start{--bs-position: start}.dropdown-menu-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-end{--bs-position: end}.dropdown-menu-end[data-bs-popper]{right:0;left:auto}@media (min-width: 576px){.dropdown-menu-sm-start{--bs-position: start}.dropdown-menu-sm-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-sm-end{--bs-position: end}.dropdown-menu-sm-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 768px){.dropdown-menu-md-start{--bs-position: start}.dropdown-menu-md-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-md-end{--bs-position: end}.dropdown-menu-md-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 992px){.dropdown-menu-lg-start{--bs-position: start}.dropdown-menu-lg-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-lg-end{--bs-position: end}.dropdown-menu-lg-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 1200px){.dropdown-menu-xl-start{--bs-position: start}.dropdown-menu-xl-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-xl-end{--bs-position: end}.dropdown-menu-xl-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 1400px){.dropdown-menu-xxl-start{--bs-position: start}.dropdown-menu-xxl-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-xxl-end{--bs-position: end}.dropdown-menu-xxl-end[data-bs-popper]{right:0;left:auto}}.dropup .dropdown-menu[data-bs-popper]{top:auto;bottom:100%;margin-top:0;margin-bottom:var(--bs-dropdown-spacer)}.dropup .dropdown-toggle::after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:"";border-top:0;border-right:.3em solid transparent;border-bottom:.3em solid;border-left:.3em solid transparent}.dropup .dropdown-toggle:empty::after{margin-left:0}.dropend .dropdown-menu[data-bs-popper]{top:0;right:auto;left:100%;margin-top:0;margin-left:var(--bs-dropdown-spacer)}.dropend .dropdown-toggle::after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:"";border-top:.3em solid transparent;border-right:0;border-bottom:.3em solid transparent;border-left:.3em solid}.dropend .dropdown-toggle:empty::after{margin-left:0}.dropend .dropdown-toggle::after{vertical-align:0}.dropstart .dropdown-menu[data-bs-popper]{top:0;right:100%;left:auto;margin-top:0;margin-right:var(--bs-dropdown-spacer)}.dropstart .dropdown-toggle::after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:""}.dropstart .dropdown-toggle::after{display:none}.dropstart .dropdown-toggle::before{display:inline-block;margin-right:.255em;vertical-align:.255em;content:"";border-top:.3em solid transparent;border-right:.3em solid;border-bottom:.3em solid transparent}.dropstart .dropdown-toggle:empty::after{margin-left:0}.dropstart .dropdown-toggle::before{vertical-align:0}.dropdown-divider,.dropdown-menu>li.divider{height:0;margin:var(--bs-dropdown-divider-margin-y) 0;overflow:hidden;border-top:1px solid var(--bs-dropdown-divider-bg);opacity:1}.dropdown-item,.dropdown-menu>li>a{display:block;width:100%;padding:var(--bs-dropdown-item-padding-y) var(--bs-dropdown-item-padding-x);clear:both;font-weight:400;color:var(--bs-dropdown-link-color);text-align:inherit;text-decoration:none;-webkit-text-decoration:none;-moz-text-decoration:none;-ms-text-decoration:none;-o-text-decoration:none;white-space:nowrap;background-color:transparent;border:0}.dropdown-item:hover,.dropdown-menu>li>a:hover,.dropdown-item:focus,.dropdown-menu>li>a:focus{color:var(--bs-dropdown-link-hover-color);background-color:var(--bs-dropdown-link-hover-bg)}.dropdown-item.active,.dropdown-menu>li>a.active,.dropdown-item:active,.dropdown-menu>li>a:active{color:var(--bs-dropdown-link-active-color);text-decoration:none;background-color:var(--bs-dropdown-link-active-bg)}.dropdown-item.disabled,.dropdown-menu>li>a.disabled,.dropdown-item:disabled,.dropdown-menu>li>a:disabled{color:var(--bs-dropdown-link-disabled-color);pointer-events:none;background-color:transparent}.dropdown-menu.show,.dropdown-menu.in{display:block}.dropdown-header{display:block;padding:var(--bs-dropdown-header-padding-y) var(--bs-dropdown-header-padding-x);margin-bottom:0;font-size:.875rem;color:var(--bs-dropdown-header-color);white-space:nowrap}.dropdown-item-text{display:block;padding:var(--bs-dropdown-item-padding-y) var(--bs-dropdown-item-padding-x);color:var(--bs-dropdown-link-color)}.dropdown-menu-dark{--bs-dropdown-color: #dee2e6;--bs-dropdown-bg: #343a40;--bs-dropdown-border-color: var(--bs-border-color-translucent);--bs-dropdown-box-shadow: ;--bs-dropdown-link-color: #dee2e6;--bs-dropdown-link-hover-color: #fff;--bs-dropdown-divider-bg: var(--bs-border-color-translucent);--bs-dropdown-link-hover-bg: rgba(255,255,255,0.15);--bs-dropdown-link-active-color: #fff;--bs-dropdown-link-active-bg: #0d6efd;--bs-dropdown-link-disabled-color: #adb5bd;--bs-dropdown-header-color: #adb5bd}.btn-group,.btn-group-vertical{position:relative;display:inline-flex;vertical-align:middle}.btn-group>.btn,.btn-group-vertical>.btn{position:relative;flex:1 1 auto;-webkit-flex:1 1 auto}.btn-group>.btn-check:checked+.btn,.btn-group>.btn-check:focus+.btn,.btn-group>.btn:hover,.btn-group>.btn:focus,.btn-group>.btn:active,.btn-group>.btn.active,.btn-group-vertical>.btn-check:checked+.btn,.btn-group-vertical>.btn-check:focus+.btn,.btn-group-vertical>.btn:hover,.btn-group-vertical>.btn:focus,.btn-group-vertical>.btn:active,.btn-group-vertical>.btn.active{z-index:1}.btn-toolbar{display:flex;display:-webkit-flex;flex-wrap:wrap;-webkit-flex-wrap:wrap;justify-content:flex-start;-webkit-justify-content:flex-start}.btn-toolbar .input-group{width:auto}.btn-group{border-radius:.375rem}.btn-group>:not(.btn-check:first-child)+.btn,.btn-group>.btn-group:not(:first-child){margin-left:-1px}.btn-group>.btn:not(:last-child):not(.dropdown-toggle),.btn-group>.btn.dropdown-toggle-split:first-child,.btn-group>.btn-group:not(:last-child)>.btn{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:nth-child(n + 3),.btn-group>:not(.btn-check)+.btn,.btn-group>.btn-group:not(:first-child)>.btn{border-top-left-radius:0;border-bottom-left-radius:0}.dropdown-toggle-split{padding-right:.5625rem;padding-left:.5625rem}.dropdown-toggle-split::after,.dropup .dropdown-toggle-split::after,.dropend .dropdown-toggle-split::after{margin-left:0}.dropstart .dropdown-toggle-split::before{margin-right:0}.btn-sm+.dropdown-toggle-split,.btn-group-sm>.btn+.dropdown-toggle-split{padding-right:.375rem;padding-left:.375rem}.btn-lg+.dropdown-toggle-split,.btn-group-lg>.btn+.dropdown-toggle-split{padding-right:.75rem;padding-left:.75rem}.btn-group-vertical{flex-direction:column;-webkit-flex-direction:column;align-items:flex-start;-webkit-align-items:flex-start;justify-content:center;-webkit-justify-content:center}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group{width:100%}.btn-group-vertical>.btn:not(:first-child),.btn-group-vertical>.btn-group:not(:first-child){margin-top:-1px}.btn-group-vertical>.btn:not(:last-child):not(.dropdown-toggle),.btn-group-vertical>.btn-group:not(:last-child)>.btn{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn~.btn,.btn-group-vertical>.btn-group:not(:first-child)>.btn{border-top-left-radius:0;border-top-right-radius:0}.nav{--bs-nav-link-padding-x: 1rem;--bs-nav-link-padding-y: .5rem;--bs-nav-link-font-weight: ;--bs-nav-link-color: var(--bs-link-color);--bs-nav-link-hover-color: var(--bs-link-hover-color);--bs-nav-link-disabled-color: #6c757d;display:flex;display:-webkit-flex;flex-wrap:wrap;-webkit-flex-wrap:wrap;padding-left:0;margin-bottom:0;list-style:none}.nav-link,.nav-tabs>li>a,.nav-pills>li>a,ul.nav.navbar-nav>li>a{display:block;padding:var(--bs-nav-link-padding-y) var(--bs-nav-link-padding-x);font-size:var(--bs-nav-link-font-size);font-weight:var(--bs-nav-link-font-weight);color:var(--bs-nav-link-color);text-decoration:none;-webkit-text-decoration:none;-moz-text-decoration:none;-ms-text-decoration:none;-o-text-decoration:none;transition:color 0.15s ease-in-out,background-color 0.15s ease-in-out,border-color 0.15s ease-in-out}@media (prefers-reduced-motion: reduce){.nav-link,.nav-tabs>li>a,.nav-pills>li>a,ul.nav.navbar-nav>li>a{transition:none}}.nav-link:hover,.nav-tabs>li>a:hover,.nav-pills>li>a:hover,ul.nav.navbar-nav>li>a:hover,.nav-link:focus,.nav-tabs>li>a:focus,.nav-pills>li>a:focus,ul.nav.navbar-nav>li>a:focus{color:var(--bs-nav-link-hover-color)}.nav-link.disabled,.nav-tabs>li>a.disabled,.nav-pills>li>a.disabled,ul.nav.navbar-nav>li>a.disabled{color:var(--bs-nav-link-disabled-color);pointer-events:none;cursor:default}.nav-tabs{--bs-nav-tabs-border-width: 1px;--bs-nav-tabs-border-color: #dee2e6;--bs-nav-tabs-border-radius: .375rem;--bs-nav-tabs-link-hover-border-color: #e9ecef #e9ecef #dee2e6;--bs-nav-tabs-link-active-color: #495057;--bs-nav-tabs-link-active-bg: #fff;--bs-nav-tabs-link-active-border-color: #dee2e6 #dee2e6 #fff;border-bottom:var(--bs-nav-tabs-border-width) solid var(--bs-nav-tabs-border-color)}.nav-tabs .nav-link,.nav-tabs>li>a,.nav-tabs .nav-pills>li>a,.nav-tabs ul.nav.navbar-nav>li>a{margin-bottom:calc(-1 * var(--bs-nav-tabs-border-width));background:none;border:var(--bs-nav-tabs-border-width) solid transparent;border-top-left-radius:var(--bs-nav-tabs-border-radius);border-top-right-radius:var(--bs-nav-tabs-border-radius)}.nav-tabs .nav-link:hover,.nav-tabs>li>a:hover,.nav-tabs .nav-pills>li>a:hover,.nav-tabs ul.nav.navbar-nav>li>a:hover,.nav-tabs .nav-link:focus,.nav-tabs>li>a:focus,.nav-tabs .nav-pills>li>a:focus,.nav-tabs ul.nav.navbar-nav>li>a:focus{isolation:isolate;border-color:var(--bs-nav-tabs-link-hover-border-color)}.nav-tabs .nav-link.disabled,.nav-tabs>li>a.disabled,.nav-tabs .nav-pills>li>a.disabled,.nav-tabs ul.nav.navbar-nav>li>a.disabled,.nav-tabs .nav-link:disabled,.nav-tabs>li>a:disabled,.nav-tabs .nav-pills>li>a:disabled,.nav-tabs ul.nav.navbar-nav>li>a:disabled{color:var(--bs-nav-link-disabled-color);background-color:transparent;border-color:transparent}.nav-tabs .nav-link.active,.nav-tabs>li>a.active,.nav-tabs .nav-pills>li>a.active,.nav-tabs ul.nav.navbar-nav>li>a.active,.nav-tabs .nav-item.show .nav-link,.nav-tabs .nav-item.in .nav-link,.nav-tabs .nav-item.show .nav-tabs>li>a,.nav-tabs .nav-item.in .nav-tabs>li>a,.nav-tabs .nav-item.show .nav-pills>li>a,.nav-tabs .nav-item.in .nav-pills>li>a,.nav-tabs>li.show .nav-link,.nav-tabs>li.in .nav-link,.nav-tabs>li.show .nav-tabs>li>a,.nav-tabs>li.in .nav-tabs>li>a,.nav-tabs>li.show .nav-pills>li>a,.nav-tabs>li.in .nav-pills>li>a,.nav-tabs .nav-pills>li.show .nav-link,.nav-tabs .nav-pills>li.in .nav-link,.nav-tabs .nav-pills>li.show .nav-tabs>li>a,.nav-tabs .nav-pills>li.in .nav-tabs>li>a,.nav-tabs .nav-pills>li.show .nav-pills>li>a,.nav-tabs .nav-pills>li.in .nav-pills>li>a,.nav-tabs .nav-item.show ul.nav.navbar-nav>li>a,.nav-tabs .nav-item.in ul.nav.navbar-nav>li>a,.nav-tabs>li.show ul.nav.navbar-nav>li>a,.nav-tabs>li.in ul.nav.navbar-nav>li>a,.nav-tabs .nav-pills>li.show ul.nav.navbar-nav>li>a,.nav-tabs .nav-pills>li.in ul.nav.navbar-nav>li>a,.nav-tabs ul.nav.navbar-nav>li.show:not(.dropdown) .nav-link,.nav-tabs ul.nav.navbar-nav>li.in:not(.dropdown) .nav-link,.nav-tabs ul.nav.navbar-nav>li.show:not(.dropdown) .nav-tabs>li>a,.nav-tabs ul.nav.navbar-nav>li.in:not(.dropdown) .nav-tabs>li>a,.nav-tabs ul.nav.navbar-nav>li.show:not(.dropdown) .nav-pills>li>a,.nav-tabs ul.nav.navbar-nav>li.in:not(.dropdown) .nav-pills>li>a,.nav-tabs ul.nav.navbar-nav>li.show:not(.dropdown) ul.nav.navbar-nav>li>a,.nav-tabs ul.nav.navbar-nav>li.in:not(.dropdown) ul.nav.navbar-nav>li>a{color:var(--bs-nav-tabs-link-active-color);background-color:var(--bs-nav-tabs-link-active-bg);border-color:var(--bs-nav-tabs-link-active-border-color)}.nav-tabs .dropdown-menu{margin-top:calc(-1 * var(--bs-nav-tabs-border-width));border-top-left-radius:0;border-top-right-radius:0}.nav-pills{--bs-nav-pills-border-radius: .375rem;--bs-nav-pills-link-active-color: #fff;--bs-nav-pills-link-active-bg: #0d6efd}.nav-pills .nav-link,.nav-pills .nav-tabs>li>a,.nav-pills>li>a,.nav-pills ul.nav.navbar-nav>li>a{background:none;border:0;border-radius:var(--bs-nav-pills-border-radius)}.nav-pills .nav-link:disabled,.nav-pills .nav-tabs>li>a:disabled,.nav-pills>li>a:disabled,.nav-pills ul.nav.navbar-nav>li>a:disabled{color:var(--bs-nav-link-disabled-color);background-color:transparent;border-color:transparent}.nav-pills .nav-link.active,.nav-pills .nav-tabs>li>a.active,.nav-pills>li>a.active,.nav-pills ul.nav.navbar-nav>li>a.active,.nav-pills .show>.nav-link,.nav-pills .in>.nav-link,.nav-pills .nav-tabs>li.show>a,.nav-pills .nav-tabs>li.in>a,.nav-pills>li.show>a,.nav-pills>li.in>a,.nav-pills ul.nav.navbar-nav>li.show>a,.nav-pills ul.nav.navbar-nav>li.in>a{color:var(--bs-nav-pills-link-active-color);background-color:var(--bs-nav-pills-link-active-bg)}.nav-fill>.nav-link,.nav-tabs>li.nav-fill>a,.nav-pills>li.nav-fill>a,ul.nav.navbar-nav>li.nav-fill>a,.nav-fill .nav-item,.nav-fill .nav-tabs>li,.nav-fill .nav-pills>li,.nav-fill ul.nav.navbar-nav>li:not(.dropdown){flex:1 1 auto;-webkit-flex:1 1 auto;text-align:center}.nav-justified>.nav-link,.nav-tabs>li.nav-justified>a,.nav-pills>li.nav-justified>a,ul.nav.navbar-nav>li.nav-justified>a,.nav-justified .nav-item,.nav-justified .nav-tabs>li,.nav-justified .nav-pills>li,.nav-justified ul.nav.navbar-nav>li:not(.dropdown){flex-basis:0;-webkit-flex-basis:0;flex-grow:1;-webkit-flex-grow:1;text-align:center}.nav-fill .nav-item .nav-link,.nav-fill .nav-tabs>li .nav-link,.nav-fill .nav-tabs>li>a,.nav-fill .nav-pills>li .nav-link,.nav-fill .nav-pills>li>a,.nav-fill .nav-item ul.nav.navbar-nav>li>a,.nav-fill .nav-tabs>li ul.nav.navbar-nav>li>a,.nav-fill .nav-pills>li ul.nav.navbar-nav>li>a,.nav-fill ul.nav.navbar-nav>li:not(.dropdown) .nav-link,.nav-fill ul.nav.navbar-nav>li:not(.dropdown) .nav-tabs>li>a,.nav-fill ul.nav.navbar-nav>li:not(.dropdown) .nav-pills>li>a,.nav-fill ul.nav.navbar-nav>li:not(.dropdown) ul.nav.navbar-nav>li>a,.nav-justified .nav-item .nav-link,.nav-justified .nav-tabs>li .nav-link,.nav-justified .nav-tabs>li>a,.nav-justified .nav-pills>li .nav-link,.nav-justified .nav-pills>li>a,.nav-justified .nav-item ul.nav.navbar-nav>li>a,.nav-justified .nav-tabs>li ul.nav.navbar-nav>li>a,.nav-justified .nav-pills>li ul.nav.navbar-nav>li>a,.nav-justified ul.nav.navbar-nav>li:not(.dropdown) .nav-link,.nav-justified ul.nav.navbar-nav>li:not(.dropdown) .nav-tabs>li>a,.nav-justified ul.nav.navbar-nav>li:not(.dropdown) .nav-pills>li>a,.nav-justified ul.nav.navbar-nav>li:not(.dropdown) ul.nav.navbar-nav>li>a{width:100%}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.navbar{--bs-navbar-padding-x: 0;--bs-navbar-padding-y: .5rem;--bs-navbar-color: rgba(0,0,0,0.55);--bs-navbar-hover-color: rgba(0,0,0,0.7);--bs-navbar-disabled-color: rgba(0,0,0,0.3);--bs-navbar-active-color: rgba(0,0,0,0.9);--bs-navbar-brand-padding-y: .3125rem;--bs-navbar-brand-margin-end: 1rem;--bs-navbar-brand-font-size: 1.25rem;--bs-navbar-brand-color: rgba(0,0,0,0.9);--bs-navbar-brand-hover-color: rgba(0,0,0,0.9);--bs-navbar-nav-link-padding-x: .5rem;--bs-navbar-toggler-padding-y: .25rem;--bs-navbar-toggler-padding-x: .75rem;--bs-navbar-toggler-font-size: 1.25rem;--bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%280,0,0,0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");--bs-navbar-toggler-border-color: rgba(0,0,0,0.1);--bs-navbar-toggler-border-radius: .375rem;--bs-navbar-toggler-focus-width: .25rem;--bs-navbar-toggler-transition: box-shadow 0.15s ease-in-out;position:relative;display:flex;display:-webkit-flex;flex-wrap:wrap;-webkit-flex-wrap:wrap;align-items:center;-webkit-align-items:center;justify-content:space-between;-webkit-justify-content:space-between;padding:var(--bs-navbar-padding-y) var(--bs-navbar-padding-x)}.navbar>.container,.navbar>.container-fluid,.navbar>.container-sm,.navbar>.container-md,.navbar>.container-lg,.navbar>.container-xl,.navbar>.container-xxl{display:flex;display:-webkit-flex;flex-wrap:inherit;-webkit-flex-wrap:inherit;align-items:center;-webkit-align-items:center;justify-content:space-between;-webkit-justify-content:space-between}.navbar-brand{padding-top:var(--bs-navbar-brand-padding-y);padding-bottom:var(--bs-navbar-brand-padding-y);margin-right:var(--bs-navbar-brand-margin-end);font-size:var(--bs-navbar-brand-font-size);color:var(--bs-navbar-brand-color);text-decoration:none;-webkit-text-decoration:none;-moz-text-decoration:none;-ms-text-decoration:none;-o-text-decoration:none;white-space:nowrap}.navbar-brand:hover,.navbar-brand:focus{color:var(--bs-navbar-brand-hover-color)}.navbar-nav{--bs-nav-link-padding-x: 0;--bs-nav-link-padding-y: .5rem;--bs-nav-link-font-weight: ;--bs-nav-link-color: var(--bs-navbar-color);--bs-nav-link-hover-color: var(--bs-navbar-hover-color);--bs-nav-link-disabled-color: var(--bs-navbar-disabled-color);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;padding-left:0;margin-bottom:0;list-style:none}.navbar-nav .show>.nav-link,.navbar-nav .in>.nav-link,.navbar-nav .nav-tabs>li.show>a,.navbar-nav .nav-tabs>li.in>a,.navbar-nav .nav-pills>li.show>a,.navbar-nav .nav-pills>li.in>a,ul.nav.navbar-nav>li.show>a,ul.nav.navbar-nav>li.in>a,.navbar-nav .active>.nav-link,.navbar-nav .nav-tabs>li.active>a,.navbar-nav .nav-pills>li.active>a,ul.nav.navbar-nav>li.active>a,.navbar-nav .nav-link.active,.navbar-nav .nav-tabs>li>a.active,.navbar-nav .nav-pills>li>a.active,ul.nav.navbar-nav>li>a.active{color:var(--bs-navbar-active-color)}.navbar-nav .dropdown-menu{position:static}.navbar-text{padding-top:.5rem;padding-bottom:.5rem;color:var(--bs-navbar-color)}.navbar-text a,.navbar-text a:hover,.navbar-text a:focus{color:var(--bs-navbar-active-color)}.navbar-collapse{flex-basis:100%;-webkit-flex-basis:100%;flex-grow:1;-webkit-flex-grow:1;align-items:center;-webkit-align-items:center}.navbar-toggler,.navbar-toggle{padding:var(--bs-navbar-toggler-padding-y) var(--bs-navbar-toggler-padding-x);font-size:var(--bs-navbar-toggler-font-size);line-height:1;color:var(--bs-navbar-color);background-color:transparent;border:var(--bs-border-width) solid var(--bs-navbar-toggler-border-color);border-radius:var(--bs-navbar-toggler-border-radius);transition:var(--bs-navbar-toggler-transition)}@media (prefers-reduced-motion: reduce){.navbar-toggler,.navbar-toggle{transition:none}}.navbar-toggler:hover,.navbar-toggle:hover{text-decoration:none}.navbar-toggler:focus,.navbar-toggle:focus{text-decoration:none;outline:0;box-shadow:0 0 0 var(--bs-navbar-toggler-focus-width)}.navbar-toggler-icon,.navbar-toggle>.icon-bar:last-child{display:inline-block;width:1.5em;height:1.5em;vertical-align:middle;background-image:var(--bs-navbar-toggler-icon-bg);background-repeat:no-repeat;background-position:center;background-size:100%}.navbar-nav-scroll{max-height:var(--bs-scroll-height, 75vh);overflow-y:auto}@media (min-width: 576px){.navbar-expand-sm,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl){flex-wrap:nowrap;-webkit-flex-wrap:nowrap;justify-content:flex-start;-webkit-justify-content:flex-start}.navbar-expand-sm .navbar-nav,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-nav{flex-direction:row;-webkit-flex-direction:row}.navbar-expand-sm .navbar-nav .dropdown-menu,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-sm .navbar-nav .nav-link,.navbar-expand-sm .navbar-nav .nav-tabs>li>a,.navbar-expand-sm .navbar-nav .nav-pills>li>a,.navbar-expand-sm ul.nav.navbar-nav>li>a,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-nav .nav-link,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-nav .nav-tabs>li>a,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-nav .nav-pills>li>a,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) ul.nav.navbar-nav>li>a{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-sm .navbar-nav-scroll,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-nav-scroll{overflow:visible}.navbar-expand-sm .navbar-collapse,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-collapse{display:flex !important;display:-webkit-flex !important;flex-basis:auto;-webkit-flex-basis:auto}.navbar-expand-sm .navbar-toggler,.navbar-expand-sm .navbar-toggle,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-toggler,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-toggle{display:none}.navbar-expand-sm .offcanvas,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .offcanvas{position:static;z-index:auto;flex-grow:1;-webkit-flex-grow:1;width:auto !important;height:auto !important;visibility:visible !important;background-color:transparent !important;border:0 !important;transform:none !important;transition:none}.navbar-expand-sm .offcanvas .offcanvas-header,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .offcanvas .offcanvas-header{display:none}.navbar-expand-sm .offcanvas .offcanvas-body,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .offcanvas .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 768px){.navbar-expand-md{flex-wrap:nowrap;-webkit-flex-wrap:nowrap;justify-content:flex-start;-webkit-justify-content:flex-start}.navbar-expand-md .navbar-nav{flex-direction:row;-webkit-flex-direction:row}.navbar-expand-md .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-md .navbar-nav .nav-link,.navbar-expand-md .navbar-nav .nav-tabs>li>a,.navbar-expand-md .navbar-nav .nav-pills>li>a,.navbar-expand-md ul.nav.navbar-nav>li>a{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-md .navbar-nav-scroll{overflow:visible}.navbar-expand-md .navbar-collapse{display:flex !important;display:-webkit-flex !important;flex-basis:auto;-webkit-flex-basis:auto}.navbar-expand-md .navbar-toggler,.navbar-expand-md .navbar-toggle{display:none}.navbar-expand-md .offcanvas{position:static;z-index:auto;flex-grow:1;-webkit-flex-grow:1;width:auto !important;height:auto !important;visibility:visible !important;background-color:transparent !important;border:0 !important;transform:none !important;transition:none}.navbar-expand-md .offcanvas .offcanvas-header{display:none}.navbar-expand-md .offcanvas .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 992px){.navbar-expand-lg{flex-wrap:nowrap;-webkit-flex-wrap:nowrap;justify-content:flex-start;-webkit-justify-content:flex-start}.navbar-expand-lg .navbar-nav{flex-direction:row;-webkit-flex-direction:row}.navbar-expand-lg .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-lg .navbar-nav .nav-link,.navbar-expand-lg .navbar-nav .nav-tabs>li>a,.navbar-expand-lg .navbar-nav .nav-pills>li>a,.navbar-expand-lg ul.nav.navbar-nav>li>a{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-lg .navbar-nav-scroll{overflow:visible}.navbar-expand-lg .navbar-collapse{display:flex !important;display:-webkit-flex !important;flex-basis:auto;-webkit-flex-basis:auto}.navbar-expand-lg .navbar-toggler,.navbar-expand-lg .navbar-toggle{display:none}.navbar-expand-lg .offcanvas{position:static;z-index:auto;flex-grow:1;-webkit-flex-grow:1;width:auto !important;height:auto !important;visibility:visible !important;background-color:transparent !important;border:0 !important;transform:none !important;transition:none}.navbar-expand-lg .offcanvas .offcanvas-header{display:none}.navbar-expand-lg .offcanvas .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 1200px){.navbar-expand-xl{flex-wrap:nowrap;-webkit-flex-wrap:nowrap;justify-content:flex-start;-webkit-justify-content:flex-start}.navbar-expand-xl .navbar-nav{flex-direction:row;-webkit-flex-direction:row}.navbar-expand-xl .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-xl .navbar-nav .nav-link,.navbar-expand-xl .navbar-nav .nav-tabs>li>a,.navbar-expand-xl .navbar-nav .nav-pills>li>a,.navbar-expand-xl ul.nav.navbar-nav>li>a{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-xl .navbar-nav-scroll{overflow:visible}.navbar-expand-xl .navbar-collapse{display:flex !important;display:-webkit-flex !important;flex-basis:auto;-webkit-flex-basis:auto}.navbar-expand-xl .navbar-toggler,.navbar-expand-xl .navbar-toggle{display:none}.navbar-expand-xl .offcanvas{position:static;z-index:auto;flex-grow:1;-webkit-flex-grow:1;width:auto !important;height:auto !important;visibility:visible !important;background-color:transparent !important;border:0 !important;transform:none !important;transition:none}.navbar-expand-xl .offcanvas .offcanvas-header{display:none}.navbar-expand-xl .offcanvas .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 1400px){.navbar-expand-xxl{flex-wrap:nowrap;-webkit-flex-wrap:nowrap;justify-content:flex-start;-webkit-justify-content:flex-start}.navbar-expand-xxl .navbar-nav{flex-direction:row;-webkit-flex-direction:row}.navbar-expand-xxl .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-xxl .navbar-nav .nav-link,.navbar-expand-xxl .navbar-nav .nav-tabs>li>a,.navbar-expand-xxl .navbar-nav .nav-pills>li>a,.navbar-expand-xxl ul.nav.navbar-nav>li>a{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-xxl .navbar-nav-scroll{overflow:visible}.navbar-expand-xxl .navbar-collapse{display:flex !important;display:-webkit-flex !important;flex-basis:auto;-webkit-flex-basis:auto}.navbar-expand-xxl .navbar-toggler,.navbar-expand-xxl .navbar-toggle{display:none}.navbar-expand-xxl .offcanvas{position:static;z-index:auto;flex-grow:1;-webkit-flex-grow:1;width:auto !important;height:auto !important;visibility:visible !important;background-color:transparent !important;border:0 !important;transform:none !important;transition:none}.navbar-expand-xxl .offcanvas .offcanvas-header{display:none}.navbar-expand-xxl .offcanvas .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible}}.navbar-expand{flex-wrap:nowrap;-webkit-flex-wrap:nowrap;justify-content:flex-start;-webkit-justify-content:flex-start}.navbar-expand .navbar-nav{flex-direction:row;-webkit-flex-direction:row}.navbar-expand .navbar-nav .dropdown-menu{position:absolute}.navbar-expand .navbar-nav .nav-link,.navbar-expand .navbar-nav .nav-tabs>li>a,.navbar-expand .navbar-nav .nav-pills>li>a,.navbar-expand ul.nav.navbar-nav>li>a{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand .navbar-nav-scroll{overflow:visible}.navbar-expand .navbar-collapse{display:flex !important;display:-webkit-flex !important;flex-basis:auto;-webkit-flex-basis:auto}.navbar-expand .navbar-toggler,.navbar-expand .navbar-toggle{display:none}.navbar-expand .offcanvas{position:static;z-index:auto;flex-grow:1;-webkit-flex-grow:1;width:auto !important;height:auto !important;visibility:visible !important;background-color:transparent !important;border:0 !important;transform:none !important;transition:none}.navbar-expand .offcanvas .offcanvas-header{display:none}.navbar-expand .offcanvas .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible}.navbar-light,.navbar.navbar-default{background-color:#f8f9fa}.navbar-dark,.navbar.navbar-inverse{background-color:#212529;--bs-navbar-color: rgba(255,255,255,0.55);--bs-navbar-hover-color: rgba(255,255,255,0.75);--bs-navbar-disabled-color: rgba(255,255,255,0.25);--bs-navbar-active-color: #fff;--bs-navbar-brand-color: #fff;--bs-navbar-brand-hover-color: #fff;--bs-navbar-toggler-border-color: rgba(255,255,255,0.1);--bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%28255,255,255,0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e")}.card,.well{--bs-card-spacer-y: 1rem;--bs-card-spacer-x: 1rem;--bs-card-title-spacer-y: .5rem;--bs-card-border-width: 1px;--bs-card-border-color: var(--bs-border-color-translucent);--bs-card-border-radius: .375rem;--bs-card-box-shadow: ;--bs-card-inner-border-radius: calc(.375rem - 1px);--bs-card-cap-padding-y: .5rem;--bs-card-cap-padding-x: 1rem;--bs-card-cap-bg: rgba(0,0,0,0.03);--bs-card-cap-color: ;--bs-card-height: ;--bs-card-color: ;--bs-card-bg: #fff;--bs-card-img-overlay-padding: 1rem;--bs-card-group-margin: .75rem;position:relative;display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;min-width:0;height:var(--bs-card-height);word-wrap:break-word;background-color:var(--bs-card-bg);background-clip:border-box;border:var(--bs-card-border-width) solid var(--bs-card-border-color);border-radius:var(--bs-card-border-radius)}.card>hr,.well>hr{margin-right:0;margin-left:0}.card>.list-group,.well>.list-group{border-top:inherit;border-bottom:inherit}.card>.list-group:first-child,.well>.list-group:first-child{border-top-width:0;border-top-left-radius:var(--bs-card-inner-border-radius);border-top-right-radius:var(--bs-card-inner-border-radius)}.card>.list-group:last-child,.well>.list-group:last-child{border-bottom-width:0;border-bottom-right-radius:var(--bs-card-inner-border-radius);border-bottom-left-radius:var(--bs-card-inner-border-radius)}.card>.card-header+.list-group,.well>.card-header+.list-group,.card>.list-group+.card-footer,.well>.list-group+.card-footer{border-top:0}.card-body{flex:1 1 auto;-webkit-flex:1 1 auto;padding:var(--bs-card-spacer-y) var(--bs-card-spacer-x);color:var(--bs-card-color)}.card-title{margin-bottom:var(--bs-card-title-spacer-y)}.card-subtitle{margin-top:calc(-.5 * var(--bs-card-title-spacer-y));margin-bottom:0}.card-text:last-child{margin-bottom:0}.card-link+.card-link{margin-left:var(--bs-card-spacer-x)}.card-header{padding:var(--bs-card-cap-padding-y) var(--bs-card-cap-padding-x);margin-bottom:0;color:var(--bs-card-cap-color);background-color:var(--bs-card-cap-bg);border-bottom:var(--bs-card-border-width) solid var(--bs-card-border-color)}.card-header:first-child{border-radius:var(--bs-card-inner-border-radius) var(--bs-card-inner-border-radius) 0 0}.card-footer{padding:var(--bs-card-cap-padding-y) var(--bs-card-cap-padding-x);color:var(--bs-card-cap-color);background-color:var(--bs-card-cap-bg);border-top:var(--bs-card-border-width) solid var(--bs-card-border-color)}.card-footer:last-child{border-radius:0 0 var(--bs-card-inner-border-radius) var(--bs-card-inner-border-radius)}.card-header-tabs{margin-right:calc(-.5 * var(--bs-card-cap-padding-x));margin-bottom:calc(-1 * var(--bs-card-cap-padding-y));margin-left:calc(-.5 * var(--bs-card-cap-padding-x));border-bottom:0}.card-header-tabs .nav-link.active,.card-header-tabs .nav-tabs>li>a.active,.card-header-tabs .nav-pills>li>a.active,.card-header-tabs ul.nav.navbar-nav>li>a.active{background-color:var(--bs-card-bg);border-bottom-color:var(--bs-card-bg)}.card-header-pills{margin-right:calc(-.5 * var(--bs-card-cap-padding-x));margin-left:calc(-.5 * var(--bs-card-cap-padding-x))}.card-img-overlay{position:absolute;top:0;right:0;bottom:0;left:0;padding:var(--bs-card-img-overlay-padding);border-radius:var(--bs-card-inner-border-radius)}.card-img,.card-img-top,.card-img-bottom{width:100%}.card-img,.card-img-top{border-top-left-radius:var(--bs-card-inner-border-radius);border-top-right-radius:var(--bs-card-inner-border-radius)}.card-img,.card-img-bottom{border-bottom-right-radius:var(--bs-card-inner-border-radius);border-bottom-left-radius:var(--bs-card-inner-border-radius)}.card-group>.card,.card-group>.well{margin-bottom:var(--bs-card-group-margin)}@media (min-width: 576px){.card-group{display:flex;display:-webkit-flex;flex-flow:row wrap;-webkit-flex-flow:row wrap}.card-group>.card,.card-group>.well{flex:1 0 0%;-webkit-flex:1 0 0%;margin-bottom:0}.card-group>.card+.card,.card-group>.well+.card,.card-group>.card+.well,.card-group>.well+.well{margin-left:0;border-left:0}.card-group>.card:not(:last-child),.card-group>.well:not(:last-child){border-top-right-radius:0;border-bottom-right-radius:0}.card-group>.card:not(:last-child) .card-img-top,.card-group>.well:not(:last-child) .card-img-top,.card-group>.card:not(:last-child) .card-header,.card-group>.well:not(:last-child) .card-header{border-top-right-radius:0}.card-group>.card:not(:last-child) .card-img-bottom,.card-group>.well:not(:last-child) .card-img-bottom,.card-group>.card:not(:last-child) .card-footer,.card-group>.well:not(:last-child) .card-footer{border-bottom-right-radius:0}.card-group>.card:not(:first-child),.card-group>.well:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.card-group>.card:not(:first-child) .card-img-top,.card-group>.well:not(:first-child) .card-img-top,.card-group>.card:not(:first-child) .card-header,.card-group>.well:not(:first-child) .card-header{border-top-left-radius:0}.card-group>.card:not(:first-child) .card-img-bottom,.card-group>.well:not(:first-child) .card-img-bottom,.card-group>.card:not(:first-child) .card-footer,.card-group>.well:not(:first-child) .card-footer{border-bottom-left-radius:0}}.accordion{--bs-accordion-color: #212529;--bs-accordion-bg: #fff;--bs-accordion-transition: color 0.15s ease-in-out,background-color 0.15s ease-in-out,border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out,border-radius 0.15s ease;--bs-accordion-border-color: var(--bs-border-color);--bs-accordion-border-width: 1px;--bs-accordion-border-radius: .375rem;--bs-accordion-inner-border-radius: calc(.375rem - 1px);--bs-accordion-btn-padding-x: 1.25rem;--bs-accordion-btn-padding-y: 1rem;--bs-accordion-btn-color: #212529;--bs-accordion-btn-bg: var(--bs-accordion-bg);--bs-accordion-btn-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23212529'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");--bs-accordion-btn-icon-width: 1.25rem;--bs-accordion-btn-icon-transform: rotate(-180deg);--bs-accordion-btn-icon-transition: transform 0.2s ease-in-out;--bs-accordion-btn-active-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill=''%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");--bs-accordion-btn-focus-border-color: #86b7fe;--bs-accordion-btn-focus-box-shadow: 0 0 0 .25rem rgba(13,110,253,0.25);--bs-accordion-body-padding-x: 1.25rem;--bs-accordion-body-padding-y: 1rem;--bs-accordion-active-color: ;--bs-accordion-active-bg: }.accordion-button{position:relative;display:flex;display:-webkit-flex;align-items:center;-webkit-align-items:center;width:100%;padding:var(--bs-accordion-btn-padding-y) var(--bs-accordion-btn-padding-x);font-size:1rem;color:var(--bs-accordion-btn-color);text-align:left;background-color:var(--bs-accordion-btn-bg);border:0;border-radius:0;overflow-anchor:none;transition:var(--bs-accordion-transition)}@media (prefers-reduced-motion: reduce){.accordion-button{transition:none}}.accordion-button:not(.collapsed){color:var(--bs-accordion-active-color);background-color:var(--bs-accordion-active-bg);box-shadow:inset 0 calc(-1 * var(--bs-accordion-border-width)) 0 var(--bs-accordion-border-color)}.accordion-button:not(.collapsed)::after{background-image:var(--bs-accordion-btn-active-icon);transform:var(--bs-accordion-btn-icon-transform)}.accordion-button::after{flex-shrink:0;-webkit-flex-shrink:0;width:var(--bs-accordion-btn-icon-width);height:var(--bs-accordion-btn-icon-width);margin-left:auto;content:"";background-image:var(--bs-accordion-btn-icon);background-repeat:no-repeat;background-size:var(--bs-accordion-btn-icon-width);transition:var(--bs-accordion-btn-icon-transition)}@media (prefers-reduced-motion: reduce){.accordion-button::after{transition:none}}.accordion-button:hover{z-index:2}.accordion-button:focus{z-index:3;border-color:var(--bs-accordion-btn-focus-border-color);outline:0;box-shadow:var(--bs-accordion-btn-focus-box-shadow)}.accordion-header{margin-bottom:0}.accordion-item{color:var(--bs-accordion-color);background-color:var(--bs-accordion-bg);border:var(--bs-accordion-border-width) solid var(--bs-accordion-border-color)}.accordion-item:first-of-type{border-top-left-radius:var(--bs-accordion-border-radius);border-top-right-radius:var(--bs-accordion-border-radius)}.accordion-item:first-of-type .accordion-button{border-top-left-radius:var(--bs-accordion-inner-border-radius);border-top-right-radius:var(--bs-accordion-inner-border-radius)}.accordion-item:not(:first-of-type){border-top:0}.accordion-item:last-of-type{border-bottom-right-radius:var(--bs-accordion-border-radius);border-bottom-left-radius:var(--bs-accordion-border-radius)}.accordion-item:last-of-type .accordion-button.collapsed{border-bottom-right-radius:var(--bs-accordion-inner-border-radius);border-bottom-left-radius:var(--bs-accordion-inner-border-radius)}.accordion-item:last-of-type .accordion-collapse{border-bottom-right-radius:var(--bs-accordion-border-radius);border-bottom-left-radius:var(--bs-accordion-border-radius)}.accordion-body{padding:var(--bs-accordion-body-padding-y) var(--bs-accordion-body-padding-x)}.accordion-flush .accordion-collapse,.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion .accordion-collapse{border-width:0}.accordion-flush .accordion-item,.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion .accordion-item{border-right:0;border-left:0;border-radius:0}.accordion-flush .accordion-item:first-child,.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion .accordion-item:first-child{border-top:0}.accordion-flush .accordion-item:last-child,.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion .accordion-item:last-child{border-bottom:0}.accordion-flush .accordion-item .accordion-button,.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion .accordion-item .accordion-button,.accordion-flush .accordion-item .accordion-button.collapsed{border-radius:0}.breadcrumb{--bs-breadcrumb-padding-x: 0;--bs-breadcrumb-padding-y: 0;--bs-breadcrumb-margin-bottom: 1rem;--bs-breadcrumb-bg: ;--bs-breadcrumb-border-radius: ;--bs-breadcrumb-divider-color: #6c757d;--bs-breadcrumb-item-padding-x: .5rem;--bs-breadcrumb-item-active-color: #6c757d;display:flex;display:-webkit-flex;flex-wrap:wrap;-webkit-flex-wrap:wrap;padding:var(--bs-breadcrumb-padding-y) var(--bs-breadcrumb-padding-x);margin-bottom:var(--bs-breadcrumb-margin-bottom);font-size:var(--bs-breadcrumb-font-size);list-style:none;background-color:var(--bs-breadcrumb-bg);border-radius:var(--bs-breadcrumb-border-radius)}.breadcrumb-item+.breadcrumb-item{padding-left:var(--bs-breadcrumb-item-padding-x)}.breadcrumb-item+.breadcrumb-item::before{float:left;padding-right:var(--bs-breadcrumb-item-padding-x);color:var(--bs-breadcrumb-divider-color);content:var(--bs-breadcrumb-divider, "/") /* rtl: var(--bs-breadcrumb-divider, "/") */}.breadcrumb-item.active{color:var(--bs-breadcrumb-item-active-color)}.pagination{--bs-pagination-padding-x: .75rem;--bs-pagination-padding-y: .375rem;--bs-pagination-font-size:1rem;--bs-pagination-color: var(--bs-link-color);--bs-pagination-bg: #fff;--bs-pagination-border-width: 1px;--bs-pagination-border-color: #dee2e6;--bs-pagination-border-radius: .375rem;--bs-pagination-hover-color: var(--bs-link-hover-color);--bs-pagination-hover-bg: #e9ecef;--bs-pagination-hover-border-color: #dee2e6;--bs-pagination-focus-color: var(--bs-link-hover-color);--bs-pagination-focus-bg: #e9ecef;--bs-pagination-focus-box-shadow: 0 0 0 .25rem rgba(13,110,253,0.25);--bs-pagination-active-color: #fff;--bs-pagination-active-bg: #0d6efd;--bs-pagination-active-border-color: #0d6efd;--bs-pagination-disabled-color: #6c757d;--bs-pagination-disabled-bg: #fff;--bs-pagination-disabled-border-color: #dee2e6;display:flex;display:-webkit-flex;padding-left:0;list-style:none}.page-link{position:relative;display:block;padding:var(--bs-pagination-padding-y) var(--bs-pagination-padding-x);font-size:var(--bs-pagination-font-size);color:var(--bs-pagination-color);text-decoration:none;-webkit-text-decoration:none;-moz-text-decoration:none;-ms-text-decoration:none;-o-text-decoration:none;background-color:var(--bs-pagination-bg);border:var(--bs-pagination-border-width) solid var(--bs-pagination-border-color);transition:color 0.15s ease-in-out,background-color 0.15s ease-in-out,border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out}@media (prefers-reduced-motion: reduce){.page-link{transition:none}}.page-link:hover{z-index:2;color:var(--bs-pagination-hover-color);background-color:var(--bs-pagination-hover-bg);border-color:var(--bs-pagination-hover-border-color)}.page-link:focus{z-index:3;color:var(--bs-pagination-focus-color);background-color:var(--bs-pagination-focus-bg);outline:0;box-shadow:var(--bs-pagination-focus-box-shadow)}.page-link.active,.active>.page-link{z-index:3;color:var(--bs-pagination-active-color);background-color:var(--bs-pagination-active-bg);border-color:var(--bs-pagination-active-border-color)}.page-link.disabled,.disabled>.page-link{color:var(--bs-pagination-disabled-color);pointer-events:none;background-color:var(--bs-pagination-disabled-bg);border-color:var(--bs-pagination-disabled-border-color)}.page-item:not(:first-child) .page-link{margin-left:-1px}.page-item:first-child .page-link{border-top-left-radius:var(--bs-pagination-border-radius);border-bottom-left-radius:var(--bs-pagination-border-radius)}.page-item:last-child .page-link{border-top-right-radius:var(--bs-pagination-border-radius);border-bottom-right-radius:var(--bs-pagination-border-radius)}.pagination-lg{--bs-pagination-padding-x: 1.5rem;--bs-pagination-padding-y: .75rem;--bs-pagination-font-size:1.25rem;--bs-pagination-border-radius: .5rem}.pagination-sm{--bs-pagination-padding-x: .5rem;--bs-pagination-padding-y: .25rem;--bs-pagination-font-size:.875rem;--bs-pagination-border-radius: .25rem}.badge{--bs-badge-padding-x: .65em;--bs-badge-padding-y: .35em;--bs-badge-font-size:.75em;--bs-badge-font-weight: 700;--bs-badge-color: #fff;--bs-badge-border-radius: .375rem;display:inline-block;padding:var(--bs-badge-padding-y) var(--bs-badge-padding-x);font-size:var(--bs-badge-font-size);font-weight:var(--bs-badge-font-weight);line-height:1;color:var(--bs-badge-color);text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:var(--bs-badge-border-radius)}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.alert{--bs-alert-bg: transparent;--bs-alert-padding-x: 1rem;--bs-alert-padding-y: 1rem;--bs-alert-margin-bottom: 1rem;--bs-alert-color: inherit;--bs-alert-border-color: transparent;--bs-alert-border: 1px solid var(--bs-alert-border-color);--bs-alert-border-radius: .375rem;position:relative;padding:var(--bs-alert-padding-y) var(--bs-alert-padding-x);margin-bottom:var(--bs-alert-margin-bottom);color:var(--bs-alert-color);background-color:var(--bs-alert-bg);border:var(--bs-alert-border);border-radius:var(--bs-alert-border-radius)}.alert-heading{color:inherit}.alert-link{font-weight:700}.alert-dismissible{padding-right:3rem}.alert-dismissible .btn-close{position:absolute;top:0;right:0;z-index:2;padding:1.25rem 1rem}.alert-default{--bs-alert-color: #595a5c;--bs-alert-bg: #f8f9fa;--bs-alert-border-color: #f5f6f8}.alert-default .alert-link{color:#47484a}.alert-primary{--bs-alert-color: #084298;--bs-alert-bg: #cfe2ff;--bs-alert-border-color: #b6d4fe}.alert-primary .alert-link{color:#06357a}.alert-secondary{--bs-alert-color: #41464b;--bs-alert-bg: #e2e3e5;--bs-alert-border-color: #d3d6d8}.alert-secondary .alert-link{color:#34383c}.alert-success{--bs-alert-color: #0f5132;--bs-alert-bg: #d1e7dd;--bs-alert-border-color: #badbcc}.alert-success .alert-link{color:#0c4128}.alert-info{--bs-alert-color: #055160;--bs-alert-bg: #cff4fc;--bs-alert-border-color: #b6effb}.alert-info .alert-link{color:#04414d}.alert-warning{--bs-alert-color: #664d03;--bs-alert-bg: #fff3cd;--bs-alert-border-color: #ffecb5}.alert-warning .alert-link{color:#523e02}.alert-danger{--bs-alert-color: #842029;--bs-alert-bg: #f8d7da;--bs-alert-border-color: #f5c2c7}.alert-danger .alert-link{color:#6a1a21}.alert-light{--bs-alert-color: #636464;--bs-alert-bg: #fefefe;--bs-alert-border-color: #fdfdfe}.alert-light .alert-link{color:#4f5050}.alert-dark{--bs-alert-color: #141619;--bs-alert-bg: #d3d3d4;--bs-alert-border-color: #bcbebf}.alert-dark .alert-link{color:#101214}@keyframes progress-bar-stripes{0%{background-position-x:1rem}}.progress{--bs-progress-height: 1rem;--bs-progress-font-size:.75rem;--bs-progress-bg: #e9ecef;--bs-progress-border-radius: .375rem;--bs-progress-box-shadow: inset 0 1px 2px rgba(0,0,0,0.075);--bs-progress-bar-color: #fff;--bs-progress-bar-bg: #0d6efd;--bs-progress-bar-transition: width 0.6s ease;display:flex;display:-webkit-flex;height:var(--bs-progress-height);overflow:hidden;font-size:var(--bs-progress-font-size);background-color:var(--bs-progress-bg);border-radius:var(--bs-progress-border-radius)}.progress-bar{display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;justify-content:center;-webkit-justify-content:center;overflow:hidden;color:var(--bs-progress-bar-color);text-align:center;white-space:nowrap;background-color:var(--bs-progress-bar-bg);transition:var(--bs-progress-bar-transition)}@media (prefers-reduced-motion: reduce){.progress-bar{transition:none}}.progress-bar-striped{background-image:linear-gradient(45deg, rgba(255,255,255,0.15) 25%, transparent 25%, transparent 50%, rgba(255,255,255,0.15) 50%, rgba(255,255,255,0.15) 75%, transparent 75%, transparent);background-size:var(--bs-progress-height) var(--bs-progress-height)}.progress-bar-animated{animation:1s linear infinite progress-bar-stripes}@media (prefers-reduced-motion: reduce){.progress-bar-animated{animation:none}}.list-group{--bs-list-group-color: #212529;--bs-list-group-bg: #fff;--bs-list-group-border-color: rgba(0,0,0,0.125);--bs-list-group-border-width: 1px;--bs-list-group-border-radius: .375rem;--bs-list-group-item-padding-x: 1rem;--bs-list-group-item-padding-y: .5rem;--bs-list-group-action-color: #495057;--bs-list-group-action-hover-color: #495057;--bs-list-group-action-hover-bg: #f8f9fa;--bs-list-group-action-active-color: #212529;--bs-list-group-action-active-bg: #e9ecef;--bs-list-group-disabled-color: #6c757d;--bs-list-group-disabled-bg: #fff;--bs-list-group-active-color: #fff;--bs-list-group-active-bg: #0d6efd;--bs-list-group-active-border-color: #0d6efd;display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;padding-left:0;margin-bottom:0;border-radius:var(--bs-list-group-border-radius)}.list-group-numbered{list-style-type:none;counter-reset:section}.list-group-numbered>.list-group-item::before{content:counters(section, ".") ". ";counter-increment:section}.list-group-item-action{width:100%;color:var(--bs-list-group-action-color);text-align:inherit}.list-group-item-action:hover,.list-group-item-action:focus{z-index:1;color:var(--bs-list-group-action-hover-color);text-decoration:none;background-color:var(--bs-list-group-action-hover-bg)}.list-group-item-action:active{color:var(--bs-list-group-action-active-color);background-color:var(--bs-list-group-action-active-bg)}.list-group-item{position:relative;display:block;padding:var(--bs-list-group-item-padding-y) var(--bs-list-group-item-padding-x);color:var(--bs-list-group-color);text-decoration:none;-webkit-text-decoration:none;-moz-text-decoration:none;-ms-text-decoration:none;-o-text-decoration:none;background-color:var(--bs-list-group-bg);border:var(--bs-list-group-border-width) solid var(--bs-list-group-border-color)}.list-group-item:first-child{border-top-left-radius:inherit;border-top-right-radius:inherit}.list-group-item:last-child{border-bottom-right-radius:inherit;border-bottom-left-radius:inherit}.list-group-item.disabled,.list-group-item:disabled{color:var(--bs-list-group-disabled-color);pointer-events:none;background-color:var(--bs-list-group-disabled-bg)}.list-group-item.active{z-index:2;color:var(--bs-list-group-active-color);background-color:var(--bs-list-group-active-bg);border-color:var(--bs-list-group-active-border-color)}.list-group-item+.list-group-item{border-top-width:0}.list-group-item+.list-group-item.active{margin-top:calc(-1 * var(--bs-list-group-border-width));border-top-width:var(--bs-list-group-border-width)}.list-group-horizontal{flex-direction:row;-webkit-flex-direction:row}.list-group-horizontal>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal>.list-group-item.active{margin-top:0}.list-group-horizontal>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}@media (min-width: 576px){.list-group-horizontal-sm{flex-direction:row;-webkit-flex-direction:row}.list-group-horizontal-sm>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-sm>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-sm>.list-group-item.active{margin-top:0}.list-group-horizontal-sm>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-sm>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 768px){.list-group-horizontal-md{flex-direction:row;-webkit-flex-direction:row}.list-group-horizontal-md>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-md>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-md>.list-group-item.active{margin-top:0}.list-group-horizontal-md>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-md>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 992px){.list-group-horizontal-lg{flex-direction:row;-webkit-flex-direction:row}.list-group-horizontal-lg>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-lg>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-lg>.list-group-item.active{margin-top:0}.list-group-horizontal-lg>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-lg>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 1200px){.list-group-horizontal-xl{flex-direction:row;-webkit-flex-direction:row}.list-group-horizontal-xl>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-xl>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-xl>.list-group-item.active{margin-top:0}.list-group-horizontal-xl>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-xl>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 1400px){.list-group-horizontal-xxl{flex-direction:row;-webkit-flex-direction:row}.list-group-horizontal-xxl>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-xxl>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-xxl>.list-group-item.active{margin-top:0}.list-group-horizontal-xxl>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-xxl>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}.list-group-flush{border-radius:0}.list-group-flush>.list-group-item{border-width:0 0 var(--bs-list-group-border-width)}.list-group-flush>.list-group-item:last-child{border-bottom-width:0}.list-group-item-default{color:#595a5c;background-color:#f8f9fa}.list-group-item-default.list-group-item-action:hover,.list-group-item-default.list-group-item-action:focus{color:#595a5c;background-color:#dfe0e1}.list-group-item-default.list-group-item-action.active{color:#fff;background-color:#595a5c;border-color:#595a5c}.list-group-item-primary{color:#084298;background-color:#cfe2ff}.list-group-item-primary.list-group-item-action:hover,.list-group-item-primary.list-group-item-action:focus{color:#084298;background-color:#bacbe6}.list-group-item-primary.list-group-item-action.active{color:#fff;background-color:#084298;border-color:#084298}.list-group-item-secondary{color:#41464b;background-color:#e2e3e5}.list-group-item-secondary.list-group-item-action:hover,.list-group-item-secondary.list-group-item-action:focus{color:#41464b;background-color:#cbccce}.list-group-item-secondary.list-group-item-action.active{color:#fff;background-color:#41464b;border-color:#41464b}.list-group-item-success{color:#0f5132;background-color:#d1e7dd}.list-group-item-success.list-group-item-action:hover,.list-group-item-success.list-group-item-action:focus{color:#0f5132;background-color:#bcd0c7}.list-group-item-success.list-group-item-action.active{color:#fff;background-color:#0f5132;border-color:#0f5132}.list-group-item-info{color:#055160;background-color:#cff4fc}.list-group-item-info.list-group-item-action:hover,.list-group-item-info.list-group-item-action:focus{color:#055160;background-color:#badce3}.list-group-item-info.list-group-item-action.active{color:#fff;background-color:#055160;border-color:#055160}.list-group-item-warning{color:#664d03;background-color:#fff3cd}.list-group-item-warning.list-group-item-action:hover,.list-group-item-warning.list-group-item-action:focus{color:#664d03;background-color:#e6dbb9}.list-group-item-warning.list-group-item-action.active{color:#fff;background-color:#664d03;border-color:#664d03}.list-group-item-danger{color:#842029;background-color:#f8d7da}.list-group-item-danger.list-group-item-action:hover,.list-group-item-danger.list-group-item-action:focus{color:#842029;background-color:#dfc2c4}.list-group-item-danger.list-group-item-action.active{color:#fff;background-color:#842029;border-color:#842029}.list-group-item-light{color:#636464;background-color:#fefefe}.list-group-item-light.list-group-item-action:hover,.list-group-item-light.list-group-item-action:focus{color:#636464;background-color:#e5e5e5}.list-group-item-light.list-group-item-action.active{color:#fff;background-color:#636464;border-color:#636464}.list-group-item-dark{color:#141619;background-color:#d3d3d4}.list-group-item-dark.list-group-item-action:hover,.list-group-item-dark.list-group-item-action:focus{color:#141619;background-color:#bebebf}.list-group-item-dark.list-group-item-action.active{color:#fff;background-color:#141619;border-color:#141619}.btn-close{box-sizing:content-box;width:1em;height:1em;padding:.25em .25em;color:#000;background:transparent url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23000'%3e%3cpath d='M.293.293a1 1 0 0 1 1.414 0L8 6.586 14.293.293a1 1 0 1 1 1.414 1.414L9.414 8l6.293 6.293a1 1 0 0 1-1.414 1.414L8 9.414l-6.293 6.293a1 1 0 0 1-1.414-1.414L6.586 8 .293 1.707a1 1 0 0 1 0-1.414z'/%3e%3c/svg%3e") center/1em auto no-repeat;border:0;border-radius:.375rem;opacity:.5}.btn-close:hover{color:#000;text-decoration:none;opacity:.75}.btn-close:focus{outline:0;box-shadow:0 0 0 .25rem rgba(13,110,253,0.25);opacity:1}.btn-close:disabled,.btn-close.disabled{pointer-events:none;user-select:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;-o-user-select:none;opacity:.25}.btn-close-white{filter:invert(1) grayscale(100%) brightness(200%)}.toast{--bs-toast-zindex: 1090;--bs-toast-padding-x: .75rem;--bs-toast-padding-y: .5rem;--bs-toast-spacing: 1.5rem;--bs-toast-max-width: 350px;--bs-toast-font-size:.875rem;--bs-toast-color: ;--bs-toast-bg: rgba(255,255,255,0.85);--bs-toast-border-width: 1px;--bs-toast-border-color: var(--bs-border-color-translucent);--bs-toast-border-radius: .375rem;--bs-toast-box-shadow: 0 0.5rem 1rem rgba(0,0,0,0.15);--bs-toast-header-color: #6c757d;--bs-toast-header-bg: rgba(255,255,255,0.85);--bs-toast-header-border-color: rgba(0,0,0,0.05);width:var(--bs-toast-max-width);max-width:100%;font-size:var(--bs-toast-font-size);color:var(--bs-toast-color);pointer-events:auto;background-color:var(--bs-toast-bg);background-clip:padding-box;border:var(--bs-toast-border-width) solid var(--bs-toast-border-color);box-shadow:var(--bs-toast-box-shadow);border-radius:var(--bs-toast-border-radius)}.toast.showing{opacity:0}.toast:not(.show):not(.in){display:none}.toast-container{--bs-toast-zindex: 1090;position:absolute;z-index:var(--bs-toast-zindex);width:max-content;width:-webkit-max-content;width:-moz-max-content;width:-ms-max-content;width:-o-max-content;max-width:100%;pointer-events:none}.toast-container>:not(:last-child){margin-bottom:var(--bs-toast-spacing)}.toast-header{display:flex;display:-webkit-flex;align-items:center;-webkit-align-items:center;padding:var(--bs-toast-padding-y) var(--bs-toast-padding-x);color:var(--bs-toast-header-color);background-color:var(--bs-toast-header-bg);background-clip:padding-box;border-bottom:var(--bs-toast-border-width) solid var(--bs-toast-header-border-color);border-top-left-radius:calc(var(--bs-toast-border-radius) - var(--bs-toast-border-width));border-top-right-radius:calc(var(--bs-toast-border-radius) - var(--bs-toast-border-width))}.toast-header .btn-close{margin-right:calc(-.5 * var(--bs-toast-padding-x));margin-left:var(--bs-toast-padding-x)}.toast-body{padding:var(--bs-toast-padding-x);word-wrap:break-word}.modal{--bs-modal-zindex: 1055;--bs-modal-width: 500px;--bs-modal-padding: 1rem;--bs-modal-margin: .5rem;--bs-modal-color: ;--bs-modal-bg: #fff;--bs-modal-border-color: var(--bs-border-color-translucent);--bs-modal-border-width: 1px;--bs-modal-border-radius: .5rem;--bs-modal-box-shadow: 0 0.125rem 0.25rem rgba(0,0,0,0.075);--bs-modal-inner-border-radius: calc(.5rem - 1px);--bs-modal-header-padding-x: 1rem;--bs-modal-header-padding-y: 1rem;--bs-modal-header-padding: 1rem 1rem;--bs-modal-header-border-color: var(--bs-border-color);--bs-modal-header-border-width: 1px;--bs-modal-title-line-height: 1.5;--bs-modal-footer-gap: .5rem;--bs-modal-footer-bg: ;--bs-modal-footer-border-color: var(--bs-border-color);--bs-modal-footer-border-width: 1px;position:fixed;top:0;left:0;z-index:var(--bs-modal-zindex);display:none;width:100%;height:100%;overflow-x:hidden;overflow-y:auto;outline:0}.modal-dialog{position:relative;width:auto;margin:var(--bs-modal-margin);pointer-events:none}.modal.fade .modal-dialog{transition:transform 0.3s ease-out;transform:translate(0, -50px)}@media (prefers-reduced-motion: reduce){.modal.fade .modal-dialog{transition:none}}.modal.show .modal-dialog,.modal.in .modal-dialog{transform:none}.modal.modal-static .modal-dialog{transform:scale(1.02)}.modal-dialog-scrollable{height:calc(100% - var(--bs-modal-margin) * 2)}.modal-dialog-scrollable .modal-content{max-height:100%;overflow:hidden}.modal-dialog-scrollable .modal-body{overflow-y:auto}.modal-dialog-centered{display:flex;display:-webkit-flex;align-items:center;-webkit-align-items:center;min-height:calc(100% - var(--bs-modal-margin) * 2)}.modal-content{position:relative;display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;width:100%;color:var(--bs-modal-color);pointer-events:auto;background-color:var(--bs-modal-bg);background-clip:padding-box;border:var(--bs-modal-border-width) solid var(--bs-modal-border-color);border-radius:var(--bs-modal-border-radius);outline:0}.modal-backdrop{--bs-backdrop-zindex: 1050;--bs-backdrop-bg: #000;--bs-backdrop-opacity: .5;position:fixed;top:0;left:0;z-index:var(--bs-backdrop-zindex);width:100vw;height:100vh;background-color:var(--bs-backdrop-bg)}.modal-backdrop.fade{opacity:0}.modal-backdrop.show,.modal-backdrop.in{opacity:var(--bs-backdrop-opacity)}.modal-header{display:flex;display:-webkit-flex;flex-shrink:0;-webkit-flex-shrink:0;align-items:center;-webkit-align-items:center;justify-content:space-between;-webkit-justify-content:space-between;padding:var(--bs-modal-header-padding);border-bottom:var(--bs-modal-header-border-width) solid var(--bs-modal-header-border-color);border-top-left-radius:var(--bs-modal-inner-border-radius);border-top-right-radius:var(--bs-modal-inner-border-radius)}.modal-header .btn-close{padding:calc(var(--bs-modal-header-padding-y) * .5) calc(var(--bs-modal-header-padding-x) * .5);margin:calc(-.5 * var(--bs-modal-header-padding-y)) calc(-.5 * var(--bs-modal-header-padding-x)) calc(-.5 * var(--bs-modal-header-padding-y)) auto}.modal-title{margin-bottom:0;line-height:var(--bs-modal-title-line-height)}.modal-body{position:relative;flex:1 1 auto;-webkit-flex:1 1 auto;padding:var(--bs-modal-padding)}.modal-footer{display:flex;display:-webkit-flex;flex-shrink:0;-webkit-flex-shrink:0;flex-wrap:wrap;-webkit-flex-wrap:wrap;align-items:center;-webkit-align-items:center;justify-content:flex-end;-webkit-justify-content:flex-end;padding:calc(var(--bs-modal-padding) - var(--bs-modal-footer-gap) * .5);background-color:var(--bs-modal-footer-bg);border-top:var(--bs-modal-footer-border-width) solid var(--bs-modal-footer-border-color);border-bottom-right-radius:var(--bs-modal-inner-border-radius);border-bottom-left-radius:var(--bs-modal-inner-border-radius)}.modal-footer>*{margin:calc(var(--bs-modal-footer-gap) * .5)}@media (min-width: 576px){.modal{--bs-modal-margin: 1.75rem;--bs-modal-box-shadow: 0 0.5rem 1rem rgba(0,0,0,0.15)}.modal-dialog{max-width:var(--bs-modal-width);margin-right:auto;margin-left:auto}.modal-sm{--bs-modal-width: 300px}}@media (min-width: 992px){.modal-lg,.modal-xl{--bs-modal-width: 800px}}@media (min-width: 1200px){.modal-xl{--bs-modal-width: 1140px}}.modal-fullscreen{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen .modal-header,.modal-fullscreen .modal-footer{border-radius:0}.modal-fullscreen .modal-body{overflow-y:auto}@media (max-width: 575.98px){.modal-fullscreen-sm-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-sm-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-sm-down .modal-header,.modal-fullscreen-sm-down .modal-footer{border-radius:0}.modal-fullscreen-sm-down .modal-body{overflow-y:auto}}@media (max-width: 767.98px){.modal-fullscreen-md-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-md-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-md-down .modal-header,.modal-fullscreen-md-down .modal-footer{border-radius:0}.modal-fullscreen-md-down .modal-body{overflow-y:auto}}@media (max-width: 991.98px){.modal-fullscreen-lg-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-lg-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-lg-down .modal-header,.modal-fullscreen-lg-down .modal-footer{border-radius:0}.modal-fullscreen-lg-down .modal-body{overflow-y:auto}}@media (max-width: 1199.98px){.modal-fullscreen-xl-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-xl-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-xl-down .modal-header,.modal-fullscreen-xl-down .modal-footer{border-radius:0}.modal-fullscreen-xl-down .modal-body{overflow-y:auto}}@media (max-width: 1399.98px){.modal-fullscreen-xxl-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-xxl-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-xxl-down .modal-header,.modal-fullscreen-xxl-down .modal-footer{border-radius:0}.modal-fullscreen-xxl-down .modal-body{overflow-y:auto}}.tooltip{--bs-tooltip-zindex: 1080;--bs-tooltip-max-width: 200px;--bs-tooltip-padding-x: .5rem;--bs-tooltip-padding-y: .25rem;--bs-tooltip-margin: ;--bs-tooltip-font-size:.875rem;--bs-tooltip-color: #fff;--bs-tooltip-bg: #000;--bs-tooltip-border-radius: .375rem;--bs-tooltip-opacity: .9;--bs-tooltip-arrow-width: .8rem;--bs-tooltip-arrow-height: .4rem;z-index:var(--bs-tooltip-zindex);display:block;padding:var(--bs-tooltip-arrow-height);margin:var(--bs-tooltip-margin);font-family:var(--bs-font-sans-serif);font-style:normal;font-weight:400;line-height:1.5;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;white-space:normal;word-spacing:normal;line-break:auto;font-size:var(--bs-tooltip-font-size);word-wrap:break-word;opacity:0}.tooltip.show,.tooltip.in{opacity:var(--bs-tooltip-opacity)}.tooltip .tooltip-arrow{display:block;width:var(--bs-tooltip-arrow-width);height:var(--bs-tooltip-arrow-height)}.tooltip .tooltip-arrow::before{position:absolute;content:"";border-color:transparent;border-style:solid}.bs-tooltip-top .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^="top"] .tooltip-arrow{bottom:0}.bs-tooltip-top .tooltip-arrow::before,.bs-tooltip-auto[data-popper-placement^="top"] .tooltip-arrow::before{top:-1px;border-width:var(--bs-tooltip-arrow-height) calc(var(--bs-tooltip-arrow-width) * .5) 0;border-top-color:var(--bs-tooltip-bg)}.bs-tooltip-end .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^="right"] .tooltip-arrow{left:0;width:var(--bs-tooltip-arrow-height);height:var(--bs-tooltip-arrow-width)}.bs-tooltip-end .tooltip-arrow::before,.bs-tooltip-auto[data-popper-placement^="right"] .tooltip-arrow::before{right:-1px;border-width:calc(var(--bs-tooltip-arrow-width) * .5) var(--bs-tooltip-arrow-height) calc(var(--bs-tooltip-arrow-width) * .5) 0;border-right-color:var(--bs-tooltip-bg)}.bs-tooltip-bottom .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^="bottom"] .tooltip-arrow{top:0}.bs-tooltip-bottom .tooltip-arrow::before,.bs-tooltip-auto[data-popper-placement^="bottom"] .tooltip-arrow::before{bottom:-1px;border-width:0 calc(var(--bs-tooltip-arrow-width) * .5) var(--bs-tooltip-arrow-height);border-bottom-color:var(--bs-tooltip-bg)}.bs-tooltip-start .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^="left"] .tooltip-arrow{right:0;width:var(--bs-tooltip-arrow-height);height:var(--bs-tooltip-arrow-width)}.bs-tooltip-start .tooltip-arrow::before,.bs-tooltip-auto[data-popper-placement^="left"] .tooltip-arrow::before{left:-1px;border-width:calc(var(--bs-tooltip-arrow-width) * .5) 0 calc(var(--bs-tooltip-arrow-width) * .5) var(--bs-tooltip-arrow-height);border-left-color:var(--bs-tooltip-bg)}.tooltip-inner{max-width:var(--bs-tooltip-max-width);padding:var(--bs-tooltip-padding-y) var(--bs-tooltip-padding-x);color:var(--bs-tooltip-color);text-align:center;background-color:var(--bs-tooltip-bg);border-radius:var(--bs-tooltip-border-radius)}.popover{--bs-popover-zindex: 1070;--bs-popover-max-width: 276px;--bs-popover-font-size:.875rem;--bs-popover-bg: #fff;--bs-popover-border-width: 1px;--bs-popover-border-color: var(--bs-border-color-translucent);--bs-popover-border-radius: .5rem;--bs-popover-inner-border-radius: calc(.5rem - 1px);--bs-popover-box-shadow: 0 0.5rem 1rem rgba(0,0,0,0.15);--bs-popover-header-padding-x: 1rem;--bs-popover-header-padding-y: .5rem;--bs-popover-header-font-size:1rem;--bs-popover-header-color: ;--bs-popover-header-bg: #f0f0f0;--bs-popover-body-padding-x: 1rem;--bs-popover-body-padding-y: 1rem;--bs-popover-body-color: #212529;--bs-popover-arrow-width: 1rem;--bs-popover-arrow-height: .5rem;--bs-popover-arrow-border: var(--bs-popover-border-color);z-index:var(--bs-popover-zindex);display:block;max-width:var(--bs-popover-max-width);font-family:var(--bs-font-sans-serif);font-style:normal;font-weight:400;line-height:1.5;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;white-space:normal;word-spacing:normal;line-break:auto;font-size:var(--bs-popover-font-size);word-wrap:break-word;background-color:var(--bs-popover-bg);background-clip:padding-box;border:var(--bs-popover-border-width) solid var(--bs-popover-border-color);border-radius:var(--bs-popover-border-radius)}.popover .popover-arrow{display:block;width:var(--bs-popover-arrow-width);height:var(--bs-popover-arrow-height)}.popover .popover-arrow::before,.popover .popover-arrow::after{position:absolute;display:block;content:"";border-color:transparent;border-style:solid;border-width:0}.bs-popover-top>.popover-arrow,.bs-popover-auto[data-popper-placement^="top"]>.popover-arrow{bottom:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width))}.bs-popover-top>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="top"]>.popover-arrow::before,.bs-popover-top>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="top"]>.popover-arrow::after{border-width:var(--bs-popover-arrow-height) calc(var(--bs-popover-arrow-width) * .5) 0}.bs-popover-top>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="top"]>.popover-arrow::before{bottom:0;border-top-color:var(--bs-popover-arrow-border)}.bs-popover-top>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="top"]>.popover-arrow::after{bottom:var(--bs-popover-border-width);border-top-color:var(--bs-popover-bg)}.bs-popover-end>.popover-arrow,.bs-popover-auto[data-popper-placement^="right"]>.popover-arrow{left:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width));width:var(--bs-popover-arrow-height);height:var(--bs-popover-arrow-width)}.bs-popover-end>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="right"]>.popover-arrow::before,.bs-popover-end>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="right"]>.popover-arrow::after{border-width:calc(var(--bs-popover-arrow-width) * .5) var(--bs-popover-arrow-height) calc(var(--bs-popover-arrow-width) * .5) 0}.bs-popover-end>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="right"]>.popover-arrow::before{left:0;border-right-color:var(--bs-popover-arrow-border)}.bs-popover-end>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="right"]>.popover-arrow::after{left:var(--bs-popover-border-width);border-right-color:var(--bs-popover-bg)}.bs-popover-bottom>.popover-arrow,.bs-popover-auto[data-popper-placement^="bottom"]>.popover-arrow{top:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width))}.bs-popover-bottom>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="bottom"]>.popover-arrow::before,.bs-popover-bottom>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="bottom"]>.popover-arrow::after{border-width:0 calc(var(--bs-popover-arrow-width) * .5) var(--bs-popover-arrow-height)}.bs-popover-bottom>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="bottom"]>.popover-arrow::before{top:0;border-bottom-color:var(--bs-popover-arrow-border)}.bs-popover-bottom>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="bottom"]>.popover-arrow::after{top:var(--bs-popover-border-width);border-bottom-color:var(--bs-popover-bg)}.bs-popover-bottom .popover-header::before,.bs-popover-auto[data-popper-placement^="bottom"] .popover-header::before{position:absolute;top:0;left:50%;display:block;width:var(--bs-popover-arrow-width);margin-left:calc(-.5 * var(--bs-popover-arrow-width));content:"";border-bottom:var(--bs-popover-border-width) solid var(--bs-popover-header-bg)}.bs-popover-start>.popover-arrow,.bs-popover-auto[data-popper-placement^="left"]>.popover-arrow{right:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width));width:var(--bs-popover-arrow-height);height:var(--bs-popover-arrow-width)}.bs-popover-start>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="left"]>.popover-arrow::before,.bs-popover-start>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="left"]>.popover-arrow::after{border-width:calc(var(--bs-popover-arrow-width) * .5) 0 calc(var(--bs-popover-arrow-width) * .5) var(--bs-popover-arrow-height)}.bs-popover-start>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="left"]>.popover-arrow::before{right:0;border-left-color:var(--bs-popover-arrow-border)}.bs-popover-start>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="left"]>.popover-arrow::after{right:var(--bs-popover-border-width);border-left-color:var(--bs-popover-bg)}.popover-header{padding:var(--bs-popover-header-padding-y) var(--bs-popover-header-padding-x);margin-bottom:0;font-size:var(--bs-popover-header-font-size);color:var(--bs-popover-header-color);background-color:var(--bs-popover-header-bg);border-bottom:var(--bs-popover-border-width) solid var(--bs-popover-border-color);border-top-left-radius:var(--bs-popover-inner-border-radius);border-top-right-radius:var(--bs-popover-inner-border-radius)}.popover-header:empty{display:none}.popover-body{padding:var(--bs-popover-body-padding-y) var(--bs-popover-body-padding-x);color:var(--bs-popover-body-color)}.carousel{position:relative}.carousel.pointer-event{touch-action:pan-y;-webkit-touch-action:pan-y;-moz-touch-action:pan-y;-ms-touch-action:pan-y;-o-touch-action:pan-y}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner::after{display:block;clear:both;content:""}.carousel-item{position:relative;display:none;float:left;width:100%;margin-right:-100%;backface-visibility:hidden;-webkit-backface-visibility:hidden;-moz-backface-visibility:hidden;-ms-backface-visibility:hidden;-o-backface-visibility:hidden;transition:transform .6s ease-in-out}@media (prefers-reduced-motion: reduce){.carousel-item{transition:none}}.carousel-item.active,.carousel-item-next,.carousel-item-prev{display:block}.carousel-item-next:not(.carousel-item-start),.active.carousel-item-end{transform:translateX(100%)}.carousel-item-prev:not(.carousel-item-end),.active.carousel-item-start{transform:translateX(-100%)}.carousel-fade .carousel-item{opacity:0;transition-property:opacity;transform:none}.carousel-fade .carousel-item.active,.carousel-fade .carousel-item-next.carousel-item-start,.carousel-fade .carousel-item-prev.carousel-item-end{z-index:1;opacity:1}.carousel-fade .active.carousel-item-start,.carousel-fade .active.carousel-item-end{z-index:0;opacity:0;transition:opacity 0s .6s}@media (prefers-reduced-motion: reduce){.carousel-fade .active.carousel-item-start,.carousel-fade .active.carousel-item-end{transition:none}}.carousel-control-prev,.carousel-control-next{position:absolute;top:0;bottom:0;z-index:1;display:flex;display:-webkit-flex;align-items:center;-webkit-align-items:center;justify-content:center;-webkit-justify-content:center;width:15%;padding:0;color:#fff;text-align:center;background:none;border:0;opacity:.5;transition:opacity 0.15s ease}@media (prefers-reduced-motion: reduce){.carousel-control-prev,.carousel-control-next{transition:none}}.carousel-control-prev:hover,.carousel-control-prev:focus,.carousel-control-next:hover,.carousel-control-next:focus{color:#fff;text-decoration:none;outline:0;opacity:.9}.carousel-control-prev{left:0}.carousel-control-next{right:0}.carousel-control-prev-icon,.carousel-control-next-icon{display:inline-block;width:2rem;height:2rem;background-repeat:no-repeat;background-position:50%;background-size:100% 100%}.carousel-control-prev-icon{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23fff'%3e%3cpath d='M11.354 1.646a.5.5 0 0 1 0 .708L5.707 8l5.647 5.646a.5.5 0 0 1-.708.708l-6-6a.5.5 0 0 1 0-.708l6-6a.5.5 0 0 1 .708 0z'/%3e%3c/svg%3e")}.carousel-control-next-icon{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23fff'%3e%3cpath d='M4.646 1.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1 0 .708l-6 6a.5.5 0 0 1-.708-.708L10.293 8 4.646 2.354a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e")}.carousel-indicators{position:absolute;right:0;bottom:0;left:0;z-index:2;display:flex;display:-webkit-flex;justify-content:center;-webkit-justify-content:center;padding:0;margin-right:15%;margin-bottom:1rem;margin-left:15%;list-style:none}.carousel-indicators [data-bs-target]{box-sizing:content-box;flex:0 1 auto;-webkit-flex:0 1 auto;width:30px;height:3px;padding:0;margin-right:3px;margin-left:3px;text-indent:-999px;cursor:pointer;background-color:#fff;background-clip:padding-box;border:0;border-top:10px solid transparent;border-bottom:10px solid transparent;opacity:.5;transition:opacity 0.6s ease}@media (prefers-reduced-motion: reduce){.carousel-indicators [data-bs-target]{transition:none}}.carousel-indicators .active{opacity:1}.carousel-caption{position:absolute;right:15%;bottom:1.25rem;left:15%;padding-top:1.25rem;padding-bottom:1.25rem;color:#fff;text-align:center}.carousel-dark .carousel-control-prev-icon,.carousel-dark .carousel-control-next-icon{filter:invert(1) grayscale(100)}.carousel-dark .carousel-indicators [data-bs-target]{background-color:#000}.carousel-dark .carousel-caption{color:#000}.spinner-grow,.spinner-border{display:inline-block;width:var(--bs-spinner-width);height:var(--bs-spinner-height);vertical-align:var(--bs-spinner-vertical-align);border-radius:50%;animation:var(--bs-spinner-animation-speed) linear infinite var(--bs-spinner-animation-name)}@keyframes spinner-border{to{transform:rotate(360deg) /* rtl:ignore */}}.spinner-border{--bs-spinner-width: 2rem;--bs-spinner-height: 2rem;--bs-spinner-vertical-align: -.125em;--bs-spinner-border-width: .25em;--bs-spinner-animation-speed: .75s;--bs-spinner-animation-name: spinner-border;border:var(--bs-spinner-border-width) solid currentcolor;border-right-color:transparent}.spinner-border-sm{--bs-spinner-width: 1rem;--bs-spinner-height: 1rem;--bs-spinner-border-width: .2em}@keyframes spinner-grow{0%{transform:scale(0)}50%{opacity:1;transform:none}}.spinner-grow{--bs-spinner-width: 2rem;--bs-spinner-height: 2rem;--bs-spinner-vertical-align: -.125em;--bs-spinner-animation-speed: .75s;--bs-spinner-animation-name: spinner-grow;background-color:currentcolor;opacity:0}.spinner-grow-sm{--bs-spinner-width: 1rem;--bs-spinner-height: 1rem}@media (prefers-reduced-motion: reduce){.spinner-border,.spinner-grow{--bs-spinner-animation-speed: 1.5s}}.offcanvas,.offcanvas-xxl,.offcanvas-xl,.offcanvas-lg,.offcanvas-md,.offcanvas-sm{--bs-offcanvas-zindex: 1045;--bs-offcanvas-width: 400px;--bs-offcanvas-height: 30vh;--bs-offcanvas-padding-x: 1rem;--bs-offcanvas-padding-y: 1rem;--bs-offcanvas-color: ;--bs-offcanvas-bg: #fff;--bs-offcanvas-border-width: 1px;--bs-offcanvas-border-color: var(--bs-border-color-translucent);--bs-offcanvas-box-shadow: 0 0.125rem 0.25rem rgba(0,0,0,0.075)}@media (max-width: 575.98px){.offcanvas-sm{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:transform .3s ease-in-out}}@media (max-width: 575.98px) and (prefers-reduced-motion: reduce){.offcanvas-sm{transition:none}}@media (max-width: 575.98px){.offcanvas-sm.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(-100%)}.offcanvas-sm.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(100%)}.offcanvas-sm.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-sm.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-sm.showing,.offcanvas-sm.show:not(.hiding),.offcanvas-sm.in:not(.hiding){transform:none}.offcanvas-sm.showing,.offcanvas-sm.hiding,.offcanvas-sm.show,.offcanvas-sm.in{visibility:visible}}@media (min-width: 576px){.offcanvas-sm{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent !important}.offcanvas-sm .offcanvas-header{display:none}.offcanvas-sm .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible;background-color:transparent !important}}@media (max-width: 767.98px){.offcanvas-md{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:transform .3s ease-in-out}}@media (max-width: 767.98px) and (prefers-reduced-motion: reduce){.offcanvas-md{transition:none}}@media (max-width: 767.98px){.offcanvas-md.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(-100%)}.offcanvas-md.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(100%)}.offcanvas-md.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-md.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-md.showing,.offcanvas-md.show:not(.hiding),.offcanvas-md.in:not(.hiding){transform:none}.offcanvas-md.showing,.offcanvas-md.hiding,.offcanvas-md.show,.offcanvas-md.in{visibility:visible}}@media (min-width: 768px){.offcanvas-md{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent !important}.offcanvas-md .offcanvas-header{display:none}.offcanvas-md .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible;background-color:transparent !important}}@media (max-width: 991.98px){.offcanvas-lg{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:transform .3s ease-in-out}}@media (max-width: 991.98px) and (prefers-reduced-motion: reduce){.offcanvas-lg{transition:none}}@media (max-width: 991.98px){.offcanvas-lg.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(-100%)}.offcanvas-lg.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(100%)}.offcanvas-lg.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-lg.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-lg.showing,.offcanvas-lg.show:not(.hiding),.offcanvas-lg.in:not(.hiding){transform:none}.offcanvas-lg.showing,.offcanvas-lg.hiding,.offcanvas-lg.show,.offcanvas-lg.in{visibility:visible}}@media (min-width: 992px){.offcanvas-lg{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent !important}.offcanvas-lg .offcanvas-header{display:none}.offcanvas-lg .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible;background-color:transparent !important}}@media (max-width: 1199.98px){.offcanvas-xl{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:transform .3s ease-in-out}}@media (max-width: 1199.98px) and (prefers-reduced-motion: reduce){.offcanvas-xl{transition:none}}@media (max-width: 1199.98px){.offcanvas-xl.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(-100%)}.offcanvas-xl.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(100%)}.offcanvas-xl.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-xl.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-xl.showing,.offcanvas-xl.show:not(.hiding),.offcanvas-xl.in:not(.hiding){transform:none}.offcanvas-xl.showing,.offcanvas-xl.hiding,.offcanvas-xl.show,.offcanvas-xl.in{visibility:visible}}@media (min-width: 1200px){.offcanvas-xl{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent !important}.offcanvas-xl .offcanvas-header{display:none}.offcanvas-xl .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible;background-color:transparent !important}}@media (max-width: 1399.98px){.offcanvas-xxl{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:transform .3s ease-in-out}}@media (max-width: 1399.98px) and (prefers-reduced-motion: reduce){.offcanvas-xxl{transition:none}}@media (max-width: 1399.98px){.offcanvas-xxl.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(-100%)}.offcanvas-xxl.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(100%)}.offcanvas-xxl.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-xxl.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-xxl.showing,.offcanvas-xxl.show:not(.hiding),.offcanvas-xxl.in:not(.hiding){transform:none}.offcanvas-xxl.showing,.offcanvas-xxl.hiding,.offcanvas-xxl.show,.offcanvas-xxl.in{visibility:visible}}@media (min-width: 1400px){.offcanvas-xxl{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent !important}.offcanvas-xxl .offcanvas-header{display:none}.offcanvas-xxl .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible;background-color:transparent !important}}.offcanvas{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:transform .3s ease-in-out}@media (prefers-reduced-motion: reduce){.offcanvas{transition:none}}.offcanvas.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(-100%)}.offcanvas.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(100%)}.offcanvas.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas.showing,.offcanvas.show:not(.hiding),.offcanvas.in:not(.hiding){transform:none}.offcanvas.showing,.offcanvas.hiding,.offcanvas.show,.offcanvas.in{visibility:visible}.offcanvas-backdrop{position:fixed;top:0;left:0;z-index:1040;width:100vw;height:100vh;background-color:#000}.offcanvas-backdrop.fade{opacity:0}.offcanvas-backdrop.show,.offcanvas-backdrop.in{opacity:.5}.offcanvas-header{display:flex;display:-webkit-flex;align-items:center;-webkit-align-items:center;justify-content:space-between;-webkit-justify-content:space-between;padding:var(--bs-offcanvas-padding-y) var(--bs-offcanvas-padding-x)}.offcanvas-header .btn-close{padding:calc(var(--bs-offcanvas-padding-y) * .5) calc(var(--bs-offcanvas-padding-x) * .5);margin-top:calc(-.5 * var(--bs-offcanvas-padding-y));margin-right:calc(-.5 * var(--bs-offcanvas-padding-x));margin-bottom:calc(-.5 * var(--bs-offcanvas-padding-y))}.offcanvas-title{margin-bottom:0;line-height:1.5}.offcanvas-body{flex-grow:1;-webkit-flex-grow:1;padding:var(--bs-offcanvas-padding-y) var(--bs-offcanvas-padding-x);overflow-y:auto}.placeholder{display:inline-block;min-height:1em;vertical-align:middle;cursor:wait;background-color:currentcolor;opacity:.5}.placeholder.btn::before{display:inline-block;content:""}.placeholder-xs{min-height:.6em}.placeholder-sm{min-height:.8em}.placeholder-lg{min-height:1.2em}.placeholder-glow .placeholder{animation:placeholder-glow 2s ease-in-out infinite}@keyframes placeholder-glow{50%{opacity:.2}}.placeholder-wave{mask-image:linear-gradient(130deg, #000 55%, rgba(0,0,0,0.8) 75%, #000 95%);-webkit-mask-image:linear-gradient(130deg, #000 55%, rgba(0,0,0,0.8) 75%, #000 95%);mask-size:200% 100%;-webkit-mask-size:200% 100%;animation:placeholder-wave 2s linear infinite}@keyframes placeholder-wave{100%{mask-position:-200% 0%;-webkit-mask-position:-200% 0%}}.clearfix::after{display:block;clear:both;content:""}.text-bg-default{color:#000 !important;background-color:RGBA(222,226,230, var(--bs-bg-opacity, 1)) !important}.text-bg-primary{color:#fff !important;background-color:RGBA(13,110,253, var(--bs-bg-opacity, 1)) !important}.text-bg-secondary{color:#fff !important;background-color:RGBA(108,117,125, var(--bs-bg-opacity, 1)) !important}.text-bg-success{color:#fff !important;background-color:RGBA(25,135,84, var(--bs-bg-opacity, 1)) !important}.text-bg-info{color:#000 !important;background-color:RGBA(13,202,240, var(--bs-bg-opacity, 1)) !important}.text-bg-warning{color:#000 !important;background-color:RGBA(255,193,7, var(--bs-bg-opacity, 1)) !important}.text-bg-danger{color:#fff !important;background-color:RGBA(220,53,69, var(--bs-bg-opacity, 1)) !important}.text-bg-light{color:#000 !important;background-color:RGBA(248,249,250, var(--bs-bg-opacity, 1)) !important}.text-bg-dark{color:#fff !important;background-color:RGBA(33,37,41, var(--bs-bg-opacity, 1)) !important}.link-default{color:#dee2e6 !important}.link-default:hover,.link-default:focus{color:#e5e8eb !important}.link-primary{color:#0d6efd !important}.link-primary:hover,.link-primary:focus{color:#0a58ca !important}.link-secondary{color:#6c757d !important}.link-secondary:hover,.link-secondary:focus{color:#565e64 !important}.link-success{color:#198754 !important}.link-success:hover,.link-success:focus{color:#146c43 !important}.link-info{color:#0dcaf0 !important}.link-info:hover,.link-info:focus{color:#3dd5f3 !important}.link-warning{color:#ffc107 !important}.link-warning:hover,.link-warning:focus{color:#ffcd39 !important}.link-danger{color:#dc3545 !important}.link-danger:hover,.link-danger:focus{color:#b02a37 !important}.link-light{color:#f8f9fa !important}.link-light:hover,.link-light:focus{color:#f9fafb !important}.link-dark{color:#212529 !important}.link-dark:hover,.link-dark:focus{color:#1a1e21 !important}.ratio{position:relative;width:100%}.ratio::before{display:block;padding-top:var(--bs-aspect-ratio);content:""}.ratio>*{position:absolute;top:0;left:0;width:100%;height:100%}.ratio-1x1{--bs-aspect-ratio: 100%}.ratio-4x3{--bs-aspect-ratio: calc(3 / 4 * 100%)}.ratio-16x9{--bs-aspect-ratio: calc(9 / 16 * 100%)}.ratio-21x9{--bs-aspect-ratio: calc(9 / 21 * 100%)}.fixed-top,.navbar-fixed-top{position:fixed;top:0;right:0;left:0;z-index:1030}.fixed-bottom,.navbar-fixed-bottom{position:fixed;right:0;bottom:0;left:0;z-index:1030}.sticky-top,.navbar-sticky-top{position:sticky;top:0;z-index:1020}.sticky-bottom{position:sticky;bottom:0;z-index:1020}@media (min-width: 576px){.sticky-sm-top{position:sticky;top:0;z-index:1020}.sticky-sm-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 768px){.sticky-md-top{position:sticky;top:0;z-index:1020}.sticky-md-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 992px){.sticky-lg-top{position:sticky;top:0;z-index:1020}.sticky-lg-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 1200px){.sticky-xl-top{position:sticky;top:0;z-index:1020}.sticky-xl-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 1400px){.sticky-xxl-top{position:sticky;top:0;z-index:1020}.sticky-xxl-bottom{position:sticky;bottom:0;z-index:1020}}.hstack{display:flex;display:-webkit-flex;flex-direction:row;-webkit-flex-direction:row;align-items:center;-webkit-align-items:center;align-self:stretch;-webkit-align-self:stretch}.vstack{display:flex;display:-webkit-flex;flex:1 1 auto;-webkit-flex:1 1 auto;flex-direction:column;-webkit-flex-direction:column;align-self:stretch;-webkit-align-self:stretch}.visually-hidden,.visually-hidden-focusable:not(:focus):not(:focus-within){position:absolute !important;width:1px !important;height:1px !important;padding:0 !important;margin:-1px !important;overflow:hidden !important;clip:rect(0, 0, 0, 0) !important;white-space:nowrap !important;border:0 !important}.stretched-link::after{position:absolute;top:0;right:0;bottom:0;left:0;z-index:1;content:""}.text-truncate{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.vr{display:inline-block;align-self:stretch;-webkit-align-self:stretch;width:1px;min-height:1em;background-color:currentcolor;opacity:.25}.align-baseline{vertical-align:baseline !important}.align-top{vertical-align:top !important}.align-middle{vertical-align:middle !important}.align-bottom{vertical-align:bottom !important}.align-text-bottom{vertical-align:text-bottom !important}.align-text-top{vertical-align:text-top !important}.float-start,.float-left{float:left !important}.float-end,.float-right{float:right !important}.float-none{float:none !important}.opacity-0{opacity:0 !important}.opacity-25{opacity:.25 !important}.opacity-50{opacity:.5 !important}.opacity-75{opacity:.75 !important}.opacity-100{opacity:1 !important}.overflow-auto{overflow:auto !important}.overflow-hidden{overflow:hidden !important}.overflow-visible{overflow:visible !important}.overflow-scroll{overflow:scroll !important}.d-inline{display:inline !important}.d-inline-block{display:inline-block !important}.d-block{display:block !important}.d-grid{display:grid !important}.d-table{display:table !important}.d-table-row{display:table-row !important}.d-table-cell{display:table-cell !important}.d-flex{display:flex !important}.d-inline-flex{display:inline-flex !important}.d-none{display:none !important}.shadow{box-shadow:0 0.5rem 1rem rgba(0,0,0,0.15) !important}.shadow-sm{box-shadow:0 0.125rem 0.25rem rgba(0,0,0,0.075) !important}.shadow-lg{box-shadow:0 1rem 3rem rgba(0,0,0,0.175) !important}.shadow-none{box-shadow:none !important}.position-static{position:static !important}.position-relative{position:relative !important}.position-absolute{position:absolute !important}.position-fixed{position:fixed !important}.position-sticky{position:sticky !important}.top-0{top:0 !important}.top-50{top:50% !important}.top-100{top:100% !important}.bottom-0{bottom:0 !important}.bottom-50{bottom:50% !important}.bottom-100{bottom:100% !important}.start-0{left:0 !important}.start-50{left:50% !important}.start-100{left:100% !important}.end-0{right:0 !important}.end-50{right:50% !important}.end-100{right:100% !important}.translate-middle{transform:translate(-50%, -50%) !important}.translate-middle-x{transform:translateX(-50%) !important}.translate-middle-y{transform:translateY(-50%) !important}.border{border:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color) !important}.border-0{border:0 !important}.border-top{border-top:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color) !important}.border-top-0{border-top:0 !important}.border-end{border-right:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color) !important}.border-end-0{border-right:0 !important}.border-bottom{border-bottom:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color) !important}.border-bottom-0{border-bottom:0 !important}.border-start{border-left:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color) !important}.border-start-0{border-left:0 !important}.border-default{--bs-border-opacity: 1;border-color:rgba(var(--bs-default-rgb), var(--bs-border-opacity)) !important}.border-primary{--bs-border-opacity: 1;border-color:rgba(var(--bs-primary-rgb), var(--bs-border-opacity)) !important}.border-secondary{--bs-border-opacity: 1;border-color:rgba(var(--bs-secondary-rgb), var(--bs-border-opacity)) !important}.border-success{--bs-border-opacity: 1;border-color:rgba(var(--bs-success-rgb), var(--bs-border-opacity)) !important}.border-info{--bs-border-opacity: 1;border-color:rgba(var(--bs-info-rgb), var(--bs-border-opacity)) !important}.border-warning{--bs-border-opacity: 1;border-color:rgba(var(--bs-warning-rgb), var(--bs-border-opacity)) !important}.border-danger{--bs-border-opacity: 1;border-color:rgba(var(--bs-danger-rgb), var(--bs-border-opacity)) !important}.border-light{--bs-border-opacity: 1;border-color:rgba(var(--bs-light-rgb), var(--bs-border-opacity)) !important}.border-dark{--bs-border-opacity: 1;border-color:rgba(var(--bs-dark-rgb), var(--bs-border-opacity)) !important}.border-white{--bs-border-opacity: 1;border-color:rgba(var(--bs-white-rgb), var(--bs-border-opacity)) !important}.border-1{--bs-border-width: 1px}.border-2{--bs-border-width: 2px}.border-3{--bs-border-width: 3px}.border-4{--bs-border-width: 4px}.border-5{--bs-border-width: 5px}.border-opacity-10{--bs-border-opacity: .1}.border-opacity-25{--bs-border-opacity: .25}.border-opacity-50{--bs-border-opacity: .5}.border-opacity-75{--bs-border-opacity: .75}.border-opacity-100{--bs-border-opacity: 1}.w-25{width:25% !important}.w-50{width:50% !important}.w-75{width:75% !important}.w-100{width:100% !important}.w-auto{width:auto !important}.mw-100{max-width:100% !important}.vw-100{width:100vw !important}.min-vw-100{min-width:100vw !important}.h-25{height:25% !important}.h-50{height:50% !important}.h-75{height:75% !important}.h-100{height:100% !important}.h-auto{height:auto !important}.mh-100{max-height:100% !important}.vh-100{height:100vh !important}.min-vh-100{min-height:100vh !important}.flex-fill{flex:1 1 auto !important}.flex-row{flex-direction:row !important}.flex-column{flex-direction:column !important}.flex-row-reverse{flex-direction:row-reverse !important}.flex-column-reverse{flex-direction:column-reverse !important}.flex-grow-0{flex-grow:0 !important}.flex-grow-1{flex-grow:1 !important}.flex-shrink-0{flex-shrink:0 !important}.flex-shrink-1{flex-shrink:1 !important}.flex-wrap{flex-wrap:wrap !important}.flex-nowrap{flex-wrap:nowrap !important}.flex-wrap-reverse{flex-wrap:wrap-reverse !important}.justify-content-start{justify-content:flex-start !important}.justify-content-end{justify-content:flex-end !important}.justify-content-center{justify-content:center !important}.justify-content-between{justify-content:space-between !important}.justify-content-around{justify-content:space-around !important}.justify-content-evenly{justify-content:space-evenly !important}.align-items-start{align-items:flex-start !important}.align-items-end{align-items:flex-end !important}.align-items-center{align-items:center !important}.align-items-baseline{align-items:baseline !important}.align-items-stretch{align-items:stretch !important}.align-content-start{align-content:flex-start !important}.align-content-end{align-content:flex-end !important}.align-content-center{align-content:center !important}.align-content-between{align-content:space-between !important}.align-content-around{align-content:space-around !important}.align-content-stretch{align-content:stretch !important}.align-self-auto{align-self:auto !important}.align-self-start{align-self:flex-start !important}.align-self-end{align-self:flex-end !important}.align-self-center{align-self:center !important}.align-self-baseline{align-self:baseline !important}.align-self-stretch{align-self:stretch !important}.order-first{order:-1 !important}.order-0{order:0 !important}.order-1{order:1 !important}.order-2{order:2 !important}.order-3{order:3 !important}.order-4{order:4 !important}.order-5{order:5 !important}.order-last{order:6 !important}.m-0{margin:0 !important}.m-1{margin:.25rem !important}.m-2{margin:.5rem !important}.m-3{margin:1rem !important}.m-4{margin:1.5rem !important}.m-5{margin:3rem !important}.m-auto{margin:auto !important}.mx-0{margin-right:0 !important;margin-left:0 !important}.mx-1{margin-right:.25rem !important;margin-left:.25rem !important}.mx-2{margin-right:.5rem !important;margin-left:.5rem !important}.mx-3{margin-right:1rem !important;margin-left:1rem !important}.mx-4{margin-right:1.5rem !important;margin-left:1.5rem !important}.mx-5{margin-right:3rem !important;margin-left:3rem !important}.mx-auto{margin-right:auto !important;margin-left:auto !important}.my-0{margin-top:0 !important;margin-bottom:0 !important}.my-1{margin-top:.25rem !important;margin-bottom:.25rem !important}.my-2{margin-top:.5rem !important;margin-bottom:.5rem !important}.my-3{margin-top:1rem !important;margin-bottom:1rem !important}.my-4{margin-top:1.5rem !important;margin-bottom:1.5rem !important}.my-5{margin-top:3rem !important;margin-bottom:3rem !important}.my-auto{margin-top:auto !important;margin-bottom:auto !important}.mt-0{margin-top:0 !important}.mt-1{margin-top:.25rem !important}.mt-2{margin-top:.5rem !important}.mt-3{margin-top:1rem !important}.mt-4{margin-top:1.5rem !important}.mt-5{margin-top:3rem !important}.mt-auto{margin-top:auto !important}.me-0{margin-right:0 !important}.me-1{margin-right:.25rem !important}.me-2{margin-right:.5rem !important}.me-3{margin-right:1rem !important}.me-4{margin-right:1.5rem !important}.me-5{margin-right:3rem !important}.me-auto{margin-right:auto !important}.mb-0{margin-bottom:0 !important}.mb-1{margin-bottom:.25rem !important}.mb-2{margin-bottom:.5rem !important}.mb-3{margin-bottom:1rem !important}.mb-4{margin-bottom:1.5rem !important}.mb-5{margin-bottom:3rem !important}.mb-auto{margin-bottom:auto !important}.ms-0{margin-left:0 !important}.ms-1{margin-left:.25rem !important}.ms-2{margin-left:.5rem !important}.ms-3{margin-left:1rem !important}.ms-4{margin-left:1.5rem !important}.ms-5{margin-left:3rem !important}.ms-auto{margin-left:auto !important}.p-0{padding:0 !important}.p-1{padding:.25rem !important}.p-2{padding:.5rem !important}.p-3{padding:1rem !important}.p-4{padding:1.5rem !important}.p-5{padding:3rem !important}.px-0{padding-right:0 !important;padding-left:0 !important}.px-1{padding-right:.25rem !important;padding-left:.25rem !important}.px-2{padding-right:.5rem !important;padding-left:.5rem !important}.px-3{padding-right:1rem !important;padding-left:1rem !important}.px-4{padding-right:1.5rem !important;padding-left:1.5rem !important}.px-5{padding-right:3rem !important;padding-left:3rem !important}.py-0{padding-top:0 !important;padding-bottom:0 !important}.py-1{padding-top:.25rem !important;padding-bottom:.25rem !important}.py-2{padding-top:.5rem !important;padding-bottom:.5rem !important}.py-3{padding-top:1rem !important;padding-bottom:1rem !important}.py-4{padding-top:1.5rem !important;padding-bottom:1.5rem !important}.py-5{padding-top:3rem !important;padding-bottom:3rem !important}.pt-0{padding-top:0 !important}.pt-1{padding-top:.25rem !important}.pt-2{padding-top:.5rem !important}.pt-3{padding-top:1rem !important}.pt-4{padding-top:1.5rem !important}.pt-5{padding-top:3rem !important}.pe-0{padding-right:0 !important}.pe-1{padding-right:.25rem !important}.pe-2{padding-right:.5rem !important}.pe-3{padding-right:1rem !important}.pe-4{padding-right:1.5rem !important}.pe-5{padding-right:3rem !important}.pb-0{padding-bottom:0 !important}.pb-1{padding-bottom:.25rem !important}.pb-2{padding-bottom:.5rem !important}.pb-3{padding-bottom:1rem !important}.pb-4{padding-bottom:1.5rem !important}.pb-5{padding-bottom:3rem !important}.ps-0{padding-left:0 !important}.ps-1{padding-left:.25rem !important}.ps-2{padding-left:.5rem !important}.ps-3{padding-left:1rem !important}.ps-4{padding-left:1.5rem !important}.ps-5{padding-left:3rem !important}.gap-0{gap:0 !important}.gap-1{gap:.25rem !important}.gap-2{gap:.5rem !important}.gap-3{gap:1rem !important}.gap-4{gap:1.5rem !important}.gap-5{gap:3rem !important}.font-monospace{font-family:var(--bs-font-monospace) !important}.fs-1{font-size:calc(1.375rem + 1.5vw) !important}.fs-2{font-size:calc(1.325rem + .9vw) !important}.fs-3{font-size:calc(1.3rem + .6vw) !important}.fs-4{font-size:calc(1.275rem + .3vw) !important}.fs-5{font-size:1.25rem !important}.fs-6{font-size:1rem !important}.fst-italic{font-style:italic !important}.fst-normal{font-style:normal !important}.fw-light{font-weight:300 !important}.fw-lighter{font-weight:lighter !important}.fw-normal{font-weight:400 !important}.fw-bold{font-weight:700 !important}.fw-semibold{font-weight:600 !important}.fw-bolder{font-weight:bolder !important}.lh-1{line-height:1 !important}.lh-sm{line-height:1.25 !important}.lh-base{line-height:1.5 !important}.lh-lg{line-height:2 !important}.text-start{text-align:left !important}.text-end{text-align:right !important}.text-center{text-align:center !important}.text-decoration-none{text-decoration:none !important}.text-decoration-underline{text-decoration:underline !important}.text-decoration-line-through{text-decoration:line-through !important}.text-lowercase{text-transform:lowercase !important}.text-uppercase{text-transform:uppercase !important}.text-capitalize{text-transform:capitalize !important}.text-wrap{white-space:normal !important}.text-nowrap{white-space:nowrap !important}.text-break{word-wrap:break-word !important;word-break:break-word !important}.text-default{--bs-text-opacity: 1;color:rgba(var(--bs-default-rgb), var(--bs-text-opacity)) !important}.text-primary{--bs-text-opacity: 1;color:rgba(var(--bs-primary-rgb), var(--bs-text-opacity)) !important}.text-secondary{--bs-text-opacity: 1;color:rgba(var(--bs-secondary-rgb), var(--bs-text-opacity)) !important}.text-success{--bs-text-opacity: 1;color:rgba(var(--bs-success-rgb), var(--bs-text-opacity)) !important}.text-info{--bs-text-opacity: 1;color:rgba(var(--bs-info-rgb), var(--bs-text-opacity)) !important}.text-warning{--bs-text-opacity: 1;color:rgba(var(--bs-warning-rgb), var(--bs-text-opacity)) !important}.text-danger{--bs-text-opacity: 1;color:rgba(var(--bs-danger-rgb), var(--bs-text-opacity)) !important}.text-light{--bs-text-opacity: 1;color:rgba(var(--bs-light-rgb), var(--bs-text-opacity)) !important}.text-dark{--bs-text-opacity: 1;color:rgba(var(--bs-dark-rgb), var(--bs-text-opacity)) !important}.text-black{--bs-text-opacity: 1;color:rgba(var(--bs-black-rgb), var(--bs-text-opacity)) !important}.text-white{--bs-text-opacity: 1;color:rgba(var(--bs-white-rgb), var(--bs-text-opacity)) !important}.text-body{--bs-text-opacity: 1;color:rgba(var(--bs-body-color-rgb), var(--bs-text-opacity)) !important}.text-muted,.help-text,.help-block{--bs-text-opacity: 1;color:#6c757d !important}.text-black-50{--bs-text-opacity: 1;color:rgba(0,0,0,0.5) !important}.text-white-50{--bs-text-opacity: 1;color:rgba(255,255,255,0.5) !important}.text-reset{--bs-text-opacity: 1;color:inherit !important}.text-opacity-25{--bs-text-opacity: .25}.text-opacity-50{--bs-text-opacity: .5}.text-opacity-75{--bs-text-opacity: .75}.text-opacity-100{--bs-text-opacity: 1}.bg-default{--bs-bg-opacity: 1;background-color:rgba(var(--bs-default-rgb), var(--bs-bg-opacity)) !important}.bg-primary{--bs-bg-opacity: 1;background-color:rgba(var(--bs-primary-rgb), var(--bs-bg-opacity)) !important}.bg-secondary{--bs-bg-opacity: 1;background-color:rgba(var(--bs-secondary-rgb), var(--bs-bg-opacity)) !important}.bg-success{--bs-bg-opacity: 1;background-color:rgba(var(--bs-success-rgb), var(--bs-bg-opacity)) !important}.bg-info{--bs-bg-opacity: 1;background-color:rgba(var(--bs-info-rgb), var(--bs-bg-opacity)) !important}.bg-warning{--bs-bg-opacity: 1;background-color:rgba(var(--bs-warning-rgb), var(--bs-bg-opacity)) !important}.bg-danger{--bs-bg-opacity: 1;background-color:rgba(var(--bs-danger-rgb), var(--bs-bg-opacity)) !important}.bg-light{--bs-bg-opacity: 1;background-color:rgba(var(--bs-light-rgb), var(--bs-bg-opacity)) !important}.bg-dark{--bs-bg-opacity: 1;background-color:rgba(var(--bs-dark-rgb), var(--bs-bg-opacity)) !important}.bg-black{--bs-bg-opacity: 1;background-color:rgba(var(--bs-black-rgb), var(--bs-bg-opacity)) !important}.bg-white{--bs-bg-opacity: 1;background-color:rgba(var(--bs-white-rgb), var(--bs-bg-opacity)) !important}.bg-body{--bs-bg-opacity: 1;background-color:rgba(var(--bs-body-bg-rgb), var(--bs-bg-opacity)) !important}.bg-transparent{--bs-bg-opacity: 1;background-color:rgba(0,0,0,0) !important}.bg-opacity-10{--bs-bg-opacity: .1}.bg-opacity-25{--bs-bg-opacity: .25}.bg-opacity-50{--bs-bg-opacity: .5}.bg-opacity-75{--bs-bg-opacity: .75}.bg-opacity-100{--bs-bg-opacity: 1}.bg-gradient{background-image:var(--bs-gradient) !important}.user-select-all{user-select:all !important}.user-select-auto{user-select:auto !important}.user-select-none{user-select:none !important}.pe-none{pointer-events:none !important}.pe-auto{pointer-events:auto !important}.rounded{border-radius:var(--bs-border-radius) !important}.rounded-0{border-radius:0 !important}.rounded-1{border-radius:var(--bs-border-radius-sm) !important}.rounded-2{border-radius:var(--bs-border-radius) !important}.rounded-3{border-radius:var(--bs-border-radius-lg) !important}.rounded-4{border-radius:var(--bs-border-radius-xl) !important}.rounded-5{border-radius:var(--bs-border-radius-2xl) !important}.rounded-circle{border-radius:50% !important}.rounded-pill{border-radius:var(--bs-border-radius-pill) !important}.rounded-top{border-top-left-radius:var(--bs-border-radius) !important;border-top-right-radius:var(--bs-border-radius) !important}.rounded-end{border-top-right-radius:var(--bs-border-radius) !important;border-bottom-right-radius:var(--bs-border-radius) !important}.rounded-bottom{border-bottom-right-radius:var(--bs-border-radius) !important;border-bottom-left-radius:var(--bs-border-radius) !important}.rounded-start{border-bottom-left-radius:var(--bs-border-radius) !important;border-top-left-radius:var(--bs-border-radius) !important}.visible{visibility:visible !important}.invisible{visibility:hidden !important}@media (min-width: 576px){.float-sm-start{float:left !important}.float-sm-end{float:right !important}.float-sm-none{float:none !important}.d-sm-inline{display:inline !important}.d-sm-inline-block{display:inline-block !important}.d-sm-block{display:block !important}.d-sm-grid{display:grid !important}.d-sm-table{display:table !important}.d-sm-table-row{display:table-row !important}.d-sm-table-cell{display:table-cell !important}.d-sm-flex{display:flex !important}.d-sm-inline-flex{display:inline-flex !important}.d-sm-none{display:none !important}.flex-sm-fill{flex:1 1 auto !important}.flex-sm-row{flex-direction:row !important}.flex-sm-column{flex-direction:column !important}.flex-sm-row-reverse{flex-direction:row-reverse !important}.flex-sm-column-reverse{flex-direction:column-reverse !important}.flex-sm-grow-0{flex-grow:0 !important}.flex-sm-grow-1{flex-grow:1 !important}.flex-sm-shrink-0{flex-shrink:0 !important}.flex-sm-shrink-1{flex-shrink:1 !important}.flex-sm-wrap{flex-wrap:wrap !important}.flex-sm-nowrap{flex-wrap:nowrap !important}.flex-sm-wrap-reverse{flex-wrap:wrap-reverse !important}.justify-content-sm-start{justify-content:flex-start !important}.justify-content-sm-end{justify-content:flex-end !important}.justify-content-sm-center{justify-content:center !important}.justify-content-sm-between{justify-content:space-between !important}.justify-content-sm-around{justify-content:space-around !important}.justify-content-sm-evenly{justify-content:space-evenly !important}.align-items-sm-start{align-items:flex-start !important}.align-items-sm-end{align-items:flex-end !important}.align-items-sm-center{align-items:center !important}.align-items-sm-baseline{align-items:baseline !important}.align-items-sm-stretch{align-items:stretch !important}.align-content-sm-start{align-content:flex-start !important}.align-content-sm-end{align-content:flex-end !important}.align-content-sm-center{align-content:center !important}.align-content-sm-between{align-content:space-between !important}.align-content-sm-around{align-content:space-around !important}.align-content-sm-stretch{align-content:stretch !important}.align-self-sm-auto{align-self:auto !important}.align-self-sm-start{align-self:flex-start !important}.align-self-sm-end{align-self:flex-end !important}.align-self-sm-center{align-self:center !important}.align-self-sm-baseline{align-self:baseline !important}.align-self-sm-stretch{align-self:stretch !important}.order-sm-first{order:-1 !important}.order-sm-0{order:0 !important}.order-sm-1{order:1 !important}.order-sm-2{order:2 !important}.order-sm-3{order:3 !important}.order-sm-4{order:4 !important}.order-sm-5{order:5 !important}.order-sm-last{order:6 !important}.m-sm-0{margin:0 !important}.m-sm-1{margin:.25rem !important}.m-sm-2{margin:.5rem !important}.m-sm-3{margin:1rem !important}.m-sm-4{margin:1.5rem !important}.m-sm-5{margin:3rem !important}.m-sm-auto{margin:auto !important}.mx-sm-0{margin-right:0 !important;margin-left:0 !important}.mx-sm-1{margin-right:.25rem !important;margin-left:.25rem !important}.mx-sm-2{margin-right:.5rem !important;margin-left:.5rem !important}.mx-sm-3{margin-right:1rem !important;margin-left:1rem !important}.mx-sm-4{margin-right:1.5rem !important;margin-left:1.5rem !important}.mx-sm-5{margin-right:3rem !important;margin-left:3rem !important}.mx-sm-auto{margin-right:auto !important;margin-left:auto !important}.my-sm-0{margin-top:0 !important;margin-bottom:0 !important}.my-sm-1{margin-top:.25rem !important;margin-bottom:.25rem !important}.my-sm-2{margin-top:.5rem !important;margin-bottom:.5rem !important}.my-sm-3{margin-top:1rem !important;margin-bottom:1rem !important}.my-sm-4{margin-top:1.5rem !important;margin-bottom:1.5rem !important}.my-sm-5{margin-top:3rem !important;margin-bottom:3rem !important}.my-sm-auto{margin-top:auto !important;margin-bottom:auto !important}.mt-sm-0{margin-top:0 !important}.mt-sm-1{margin-top:.25rem !important}.mt-sm-2{margin-top:.5rem !important}.mt-sm-3{margin-top:1rem !important}.mt-sm-4{margin-top:1.5rem !important}.mt-sm-5{margin-top:3rem !important}.mt-sm-auto{margin-top:auto !important}.me-sm-0{margin-right:0 !important}.me-sm-1{margin-right:.25rem !important}.me-sm-2{margin-right:.5rem !important}.me-sm-3{margin-right:1rem !important}.me-sm-4{margin-right:1.5rem !important}.me-sm-5{margin-right:3rem !important}.me-sm-auto{margin-right:auto !important}.mb-sm-0{margin-bottom:0 !important}.mb-sm-1{margin-bottom:.25rem !important}.mb-sm-2{margin-bottom:.5rem !important}.mb-sm-3{margin-bottom:1rem !important}.mb-sm-4{margin-bottom:1.5rem !important}.mb-sm-5{margin-bottom:3rem !important}.mb-sm-auto{margin-bottom:auto !important}.ms-sm-0{margin-left:0 !important}.ms-sm-1{margin-left:.25rem !important}.ms-sm-2{margin-left:.5rem !important}.ms-sm-3{margin-left:1rem !important}.ms-sm-4{margin-left:1.5rem !important}.ms-sm-5{margin-left:3rem !important}.ms-sm-auto{margin-left:auto !important}.p-sm-0{padding:0 !important}.p-sm-1{padding:.25rem !important}.p-sm-2{padding:.5rem !important}.p-sm-3{padding:1rem !important}.p-sm-4{padding:1.5rem !important}.p-sm-5{padding:3rem !important}.px-sm-0{padding-right:0 !important;padding-left:0 !important}.px-sm-1{padding-right:.25rem !important;padding-left:.25rem !important}.px-sm-2{padding-right:.5rem !important;padding-left:.5rem !important}.px-sm-3{padding-right:1rem !important;padding-left:1rem !important}.px-sm-4{padding-right:1.5rem !important;padding-left:1.5rem !important}.px-sm-5{padding-right:3rem !important;padding-left:3rem !important}.py-sm-0{padding-top:0 !important;padding-bottom:0 !important}.py-sm-1{padding-top:.25rem !important;padding-bottom:.25rem !important}.py-sm-2{padding-top:.5rem !important;padding-bottom:.5rem !important}.py-sm-3{padding-top:1rem !important;padding-bottom:1rem !important}.py-sm-4{padding-top:1.5rem !important;padding-bottom:1.5rem !important}.py-sm-5{padding-top:3rem !important;padding-bottom:3rem !important}.pt-sm-0{padding-top:0 !important}.pt-sm-1{padding-top:.25rem !important}.pt-sm-2{padding-top:.5rem !important}.pt-sm-3{padding-top:1rem !important}.pt-sm-4{padding-top:1.5rem !important}.pt-sm-5{padding-top:3rem !important}.pe-sm-0{padding-right:0 !important}.pe-sm-1{padding-right:.25rem !important}.pe-sm-2{padding-right:.5rem !important}.pe-sm-3{padding-right:1rem !important}.pe-sm-4{padding-right:1.5rem !important}.pe-sm-5{padding-right:3rem !important}.pb-sm-0{padding-bottom:0 !important}.pb-sm-1{padding-bottom:.25rem !important}.pb-sm-2{padding-bottom:.5rem !important}.pb-sm-3{padding-bottom:1rem !important}.pb-sm-4{padding-bottom:1.5rem !important}.pb-sm-5{padding-bottom:3rem !important}.ps-sm-0{padding-left:0 !important}.ps-sm-1{padding-left:.25rem !important}.ps-sm-2{padding-left:.5rem !important}.ps-sm-3{padding-left:1rem !important}.ps-sm-4{padding-left:1.5rem !important}.ps-sm-5{padding-left:3rem !important}.gap-sm-0{gap:0 !important}.gap-sm-1{gap:.25rem !important}.gap-sm-2{gap:.5rem !important}.gap-sm-3{gap:1rem !important}.gap-sm-4{gap:1.5rem !important}.gap-sm-5{gap:3rem !important}.text-sm-start{text-align:left !important}.text-sm-end{text-align:right !important}.text-sm-center{text-align:center !important}}@media (min-width: 768px){.float-md-start{float:left !important}.float-md-end{float:right !important}.float-md-none{float:none !important}.d-md-inline{display:inline !important}.d-md-inline-block{display:inline-block !important}.d-md-block{display:block !important}.d-md-grid{display:grid !important}.d-md-table{display:table !important}.d-md-table-row{display:table-row !important}.d-md-table-cell{display:table-cell !important}.d-md-flex{display:flex !important}.d-md-inline-flex{display:inline-flex !important}.d-md-none{display:none !important}.flex-md-fill{flex:1 1 auto !important}.flex-md-row{flex-direction:row !important}.flex-md-column{flex-direction:column !important}.flex-md-row-reverse{flex-direction:row-reverse !important}.flex-md-column-reverse{flex-direction:column-reverse !important}.flex-md-grow-0{flex-grow:0 !important}.flex-md-grow-1{flex-grow:1 !important}.flex-md-shrink-0{flex-shrink:0 !important}.flex-md-shrink-1{flex-shrink:1 !important}.flex-md-wrap{flex-wrap:wrap !important}.flex-md-nowrap{flex-wrap:nowrap !important}.flex-md-wrap-reverse{flex-wrap:wrap-reverse !important}.justify-content-md-start{justify-content:flex-start !important}.justify-content-md-end{justify-content:flex-end !important}.justify-content-md-center{justify-content:center !important}.justify-content-md-between{justify-content:space-between !important}.justify-content-md-around{justify-content:space-around !important}.justify-content-md-evenly{justify-content:space-evenly !important}.align-items-md-start{align-items:flex-start !important}.align-items-md-end{align-items:flex-end !important}.align-items-md-center{align-items:center !important}.align-items-md-baseline{align-items:baseline !important}.align-items-md-stretch{align-items:stretch !important}.align-content-md-start{align-content:flex-start !important}.align-content-md-end{align-content:flex-end !important}.align-content-md-center{align-content:center !important}.align-content-md-between{align-content:space-between !important}.align-content-md-around{align-content:space-around !important}.align-content-md-stretch{align-content:stretch !important}.align-self-md-auto{align-self:auto !important}.align-self-md-start{align-self:flex-start !important}.align-self-md-end{align-self:flex-end !important}.align-self-md-center{align-self:center !important}.align-self-md-baseline{align-self:baseline !important}.align-self-md-stretch{align-self:stretch !important}.order-md-first{order:-1 !important}.order-md-0{order:0 !important}.order-md-1{order:1 !important}.order-md-2{order:2 !important}.order-md-3{order:3 !important}.order-md-4{order:4 !important}.order-md-5{order:5 !important}.order-md-last{order:6 !important}.m-md-0{margin:0 !important}.m-md-1{margin:.25rem !important}.m-md-2{margin:.5rem !important}.m-md-3{margin:1rem !important}.m-md-4{margin:1.5rem !important}.m-md-5{margin:3rem !important}.m-md-auto{margin:auto !important}.mx-md-0{margin-right:0 !important;margin-left:0 !important}.mx-md-1{margin-right:.25rem !important;margin-left:.25rem !important}.mx-md-2{margin-right:.5rem !important;margin-left:.5rem !important}.mx-md-3{margin-right:1rem !important;margin-left:1rem !important}.mx-md-4{margin-right:1.5rem !important;margin-left:1.5rem !important}.mx-md-5{margin-right:3rem !important;margin-left:3rem !important}.mx-md-auto{margin-right:auto !important;margin-left:auto !important}.my-md-0{margin-top:0 !important;margin-bottom:0 !important}.my-md-1{margin-top:.25rem !important;margin-bottom:.25rem !important}.my-md-2{margin-top:.5rem !important;margin-bottom:.5rem !important}.my-md-3{margin-top:1rem !important;margin-bottom:1rem !important}.my-md-4{margin-top:1.5rem !important;margin-bottom:1.5rem !important}.my-md-5{margin-top:3rem !important;margin-bottom:3rem !important}.my-md-auto{margin-top:auto !important;margin-bottom:auto !important}.mt-md-0{margin-top:0 !important}.mt-md-1{margin-top:.25rem !important}.mt-md-2{margin-top:.5rem !important}.mt-md-3{margin-top:1rem !important}.mt-md-4{margin-top:1.5rem !important}.mt-md-5{margin-top:3rem !important}.mt-md-auto{margin-top:auto !important}.me-md-0{margin-right:0 !important}.me-md-1{margin-right:.25rem !important}.me-md-2{margin-right:.5rem !important}.me-md-3{margin-right:1rem !important}.me-md-4{margin-right:1.5rem !important}.me-md-5{margin-right:3rem !important}.me-md-auto{margin-right:auto !important}.mb-md-0{margin-bottom:0 !important}.mb-md-1{margin-bottom:.25rem !important}.mb-md-2{margin-bottom:.5rem !important}.mb-md-3{margin-bottom:1rem !important}.mb-md-4{margin-bottom:1.5rem !important}.mb-md-5{margin-bottom:3rem !important}.mb-md-auto{margin-bottom:auto !important}.ms-md-0{margin-left:0 !important}.ms-md-1{margin-left:.25rem !important}.ms-md-2{margin-left:.5rem !important}.ms-md-3{margin-left:1rem !important}.ms-md-4{margin-left:1.5rem !important}.ms-md-5{margin-left:3rem !important}.ms-md-auto{margin-left:auto !important}.p-md-0{padding:0 !important}.p-md-1{padding:.25rem !important}.p-md-2{padding:.5rem !important}.p-md-3{padding:1rem !important}.p-md-4{padding:1.5rem !important}.p-md-5{padding:3rem !important}.px-md-0{padding-right:0 !important;padding-left:0 !important}.px-md-1{padding-right:.25rem !important;padding-left:.25rem !important}.px-md-2{padding-right:.5rem !important;padding-left:.5rem !important}.px-md-3{padding-right:1rem !important;padding-left:1rem !important}.px-md-4{padding-right:1.5rem !important;padding-left:1.5rem !important}.px-md-5{padding-right:3rem !important;padding-left:3rem !important}.py-md-0{padding-top:0 !important;padding-bottom:0 !important}.py-md-1{padding-top:.25rem !important;padding-bottom:.25rem !important}.py-md-2{padding-top:.5rem !important;padding-bottom:.5rem !important}.py-md-3{padding-top:1rem !important;padding-bottom:1rem !important}.py-md-4{padding-top:1.5rem !important;padding-bottom:1.5rem !important}.py-md-5{padding-top:3rem !important;padding-bottom:3rem !important}.pt-md-0{padding-top:0 !important}.pt-md-1{padding-top:.25rem !important}.pt-md-2{padding-top:.5rem !important}.pt-md-3{padding-top:1rem !important}.pt-md-4{padding-top:1.5rem !important}.pt-md-5{padding-top:3rem !important}.pe-md-0{padding-right:0 !important}.pe-md-1{padding-right:.25rem !important}.pe-md-2{padding-right:.5rem !important}.pe-md-3{padding-right:1rem !important}.pe-md-4{padding-right:1.5rem !important}.pe-md-5{padding-right:3rem !important}.pb-md-0{padding-bottom:0 !important}.pb-md-1{padding-bottom:.25rem !important}.pb-md-2{padding-bottom:.5rem !important}.pb-md-3{padding-bottom:1rem !important}.pb-md-4{padding-bottom:1.5rem !important}.pb-md-5{padding-bottom:3rem !important}.ps-md-0{padding-left:0 !important}.ps-md-1{padding-left:.25rem !important}.ps-md-2{padding-left:.5rem !important}.ps-md-3{padding-left:1rem !important}.ps-md-4{padding-left:1.5rem !important}.ps-md-5{padding-left:3rem !important}.gap-md-0{gap:0 !important}.gap-md-1{gap:.25rem !important}.gap-md-2{gap:.5rem !important}.gap-md-3{gap:1rem !important}.gap-md-4{gap:1.5rem !important}.gap-md-5{gap:3rem !important}.text-md-start{text-align:left !important}.text-md-end{text-align:right !important}.text-md-center{text-align:center !important}}@media (min-width: 992px){.float-lg-start{float:left !important}.float-lg-end{float:right !important}.float-lg-none{float:none !important}.d-lg-inline{display:inline !important}.d-lg-inline-block{display:inline-block !important}.d-lg-block{display:block !important}.d-lg-grid{display:grid !important}.d-lg-table{display:table !important}.d-lg-table-row{display:table-row !important}.d-lg-table-cell{display:table-cell !important}.d-lg-flex{display:flex !important}.d-lg-inline-flex{display:inline-flex !important}.d-lg-none{display:none !important}.flex-lg-fill{flex:1 1 auto !important}.flex-lg-row{flex-direction:row !important}.flex-lg-column{flex-direction:column !important}.flex-lg-row-reverse{flex-direction:row-reverse !important}.flex-lg-column-reverse{flex-direction:column-reverse !important}.flex-lg-grow-0{flex-grow:0 !important}.flex-lg-grow-1{flex-grow:1 !important}.flex-lg-shrink-0{flex-shrink:0 !important}.flex-lg-shrink-1{flex-shrink:1 !important}.flex-lg-wrap{flex-wrap:wrap !important}.flex-lg-nowrap{flex-wrap:nowrap !important}.flex-lg-wrap-reverse{flex-wrap:wrap-reverse !important}.justify-content-lg-start{justify-content:flex-start !important}.justify-content-lg-end{justify-content:flex-end !important}.justify-content-lg-center{justify-content:center !important}.justify-content-lg-between{justify-content:space-between !important}.justify-content-lg-around{justify-content:space-around !important}.justify-content-lg-evenly{justify-content:space-evenly !important}.align-items-lg-start{align-items:flex-start !important}.align-items-lg-end{align-items:flex-end !important}.align-items-lg-center{align-items:center !important}.align-items-lg-baseline{align-items:baseline !important}.align-items-lg-stretch{align-items:stretch !important}.align-content-lg-start{align-content:flex-start !important}.align-content-lg-end{align-content:flex-end !important}.align-content-lg-center{align-content:center !important}.align-content-lg-between{align-content:space-between !important}.align-content-lg-around{align-content:space-around !important}.align-content-lg-stretch{align-content:stretch !important}.align-self-lg-auto{align-self:auto !important}.align-self-lg-start{align-self:flex-start !important}.align-self-lg-end{align-self:flex-end !important}.align-self-lg-center{align-self:center !important}.align-self-lg-baseline{align-self:baseline !important}.align-self-lg-stretch{align-self:stretch !important}.order-lg-first{order:-1 !important}.order-lg-0{order:0 !important}.order-lg-1{order:1 !important}.order-lg-2{order:2 !important}.order-lg-3{order:3 !important}.order-lg-4{order:4 !important}.order-lg-5{order:5 !important}.order-lg-last{order:6 !important}.m-lg-0{margin:0 !important}.m-lg-1{margin:.25rem !important}.m-lg-2{margin:.5rem !important}.m-lg-3{margin:1rem !important}.m-lg-4{margin:1.5rem !important}.m-lg-5{margin:3rem !important}.m-lg-auto{margin:auto !important}.mx-lg-0{margin-right:0 !important;margin-left:0 !important}.mx-lg-1{margin-right:.25rem !important;margin-left:.25rem !important}.mx-lg-2{margin-right:.5rem !important;margin-left:.5rem !important}.mx-lg-3{margin-right:1rem !important;margin-left:1rem !important}.mx-lg-4{margin-right:1.5rem !important;margin-left:1.5rem !important}.mx-lg-5{margin-right:3rem !important;margin-left:3rem !important}.mx-lg-auto{margin-right:auto !important;margin-left:auto !important}.my-lg-0{margin-top:0 !important;margin-bottom:0 !important}.my-lg-1{margin-top:.25rem !important;margin-bottom:.25rem !important}.my-lg-2{margin-top:.5rem !important;margin-bottom:.5rem !important}.my-lg-3{margin-top:1rem !important;margin-bottom:1rem !important}.my-lg-4{margin-top:1.5rem !important;margin-bottom:1.5rem !important}.my-lg-5{margin-top:3rem !important;margin-bottom:3rem !important}.my-lg-auto{margin-top:auto !important;margin-bottom:auto !important}.mt-lg-0{margin-top:0 !important}.mt-lg-1{margin-top:.25rem !important}.mt-lg-2{margin-top:.5rem !important}.mt-lg-3{margin-top:1rem !important}.mt-lg-4{margin-top:1.5rem !important}.mt-lg-5{margin-top:3rem !important}.mt-lg-auto{margin-top:auto !important}.me-lg-0{margin-right:0 !important}.me-lg-1{margin-right:.25rem !important}.me-lg-2{margin-right:.5rem !important}.me-lg-3{margin-right:1rem !important}.me-lg-4{margin-right:1.5rem !important}.me-lg-5{margin-right:3rem !important}.me-lg-auto{margin-right:auto !important}.mb-lg-0{margin-bottom:0 !important}.mb-lg-1{margin-bottom:.25rem !important}.mb-lg-2{margin-bottom:.5rem !important}.mb-lg-3{margin-bottom:1rem !important}.mb-lg-4{margin-bottom:1.5rem !important}.mb-lg-5{margin-bottom:3rem !important}.mb-lg-auto{margin-bottom:auto !important}.ms-lg-0{margin-left:0 !important}.ms-lg-1{margin-left:.25rem !important}.ms-lg-2{margin-left:.5rem !important}.ms-lg-3{margin-left:1rem !important}.ms-lg-4{margin-left:1.5rem !important}.ms-lg-5{margin-left:3rem !important}.ms-lg-auto{margin-left:auto !important}.p-lg-0{padding:0 !important}.p-lg-1{padding:.25rem !important}.p-lg-2{padding:.5rem !important}.p-lg-3{padding:1rem !important}.p-lg-4{padding:1.5rem !important}.p-lg-5{padding:3rem !important}.px-lg-0{padding-right:0 !important;padding-left:0 !important}.px-lg-1{padding-right:.25rem !important;padding-left:.25rem !important}.px-lg-2{padding-right:.5rem !important;padding-left:.5rem !important}.px-lg-3{padding-right:1rem !important;padding-left:1rem !important}.px-lg-4{padding-right:1.5rem !important;padding-left:1.5rem !important}.px-lg-5{padding-right:3rem !important;padding-left:3rem !important}.py-lg-0{padding-top:0 !important;padding-bottom:0 !important}.py-lg-1{padding-top:.25rem !important;padding-bottom:.25rem !important}.py-lg-2{padding-top:.5rem !important;padding-bottom:.5rem !important}.py-lg-3{padding-top:1rem !important;padding-bottom:1rem !important}.py-lg-4{padding-top:1.5rem !important;padding-bottom:1.5rem !important}.py-lg-5{padding-top:3rem !important;padding-bottom:3rem !important}.pt-lg-0{padding-top:0 !important}.pt-lg-1{padding-top:.25rem !important}.pt-lg-2{padding-top:.5rem !important}.pt-lg-3{padding-top:1rem !important}.pt-lg-4{padding-top:1.5rem !important}.pt-lg-5{padding-top:3rem !important}.pe-lg-0{padding-right:0 !important}.pe-lg-1{padding-right:.25rem !important}.pe-lg-2{padding-right:.5rem !important}.pe-lg-3{padding-right:1rem !important}.pe-lg-4{padding-right:1.5rem !important}.pe-lg-5{padding-right:3rem !important}.pb-lg-0{padding-bottom:0 !important}.pb-lg-1{padding-bottom:.25rem !important}.pb-lg-2{padding-bottom:.5rem !important}.pb-lg-3{padding-bottom:1rem !important}.pb-lg-4{padding-bottom:1.5rem !important}.pb-lg-5{padding-bottom:3rem !important}.ps-lg-0{padding-left:0 !important}.ps-lg-1{padding-left:.25rem !important}.ps-lg-2{padding-left:.5rem !important}.ps-lg-3{padding-left:1rem !important}.ps-lg-4{padding-left:1.5rem !important}.ps-lg-5{padding-left:3rem !important}.gap-lg-0{gap:0 !important}.gap-lg-1{gap:.25rem !important}.gap-lg-2{gap:.5rem !important}.gap-lg-3{gap:1rem !important}.gap-lg-4{gap:1.5rem !important}.gap-lg-5{gap:3rem !important}.text-lg-start{text-align:left !important}.text-lg-end{text-align:right !important}.text-lg-center{text-align:center !important}}@media (min-width: 1200px){.float-xl-start{float:left !important}.float-xl-end{float:right !important}.float-xl-none{float:none !important}.d-xl-inline{display:inline !important}.d-xl-inline-block{display:inline-block !important}.d-xl-block{display:block !important}.d-xl-grid{display:grid !important}.d-xl-table{display:table !important}.d-xl-table-row{display:table-row !important}.d-xl-table-cell{display:table-cell !important}.d-xl-flex{display:flex !important}.d-xl-inline-flex{display:inline-flex !important}.d-xl-none{display:none !important}.flex-xl-fill{flex:1 1 auto !important}.flex-xl-row{flex-direction:row !important}.flex-xl-column{flex-direction:column !important}.flex-xl-row-reverse{flex-direction:row-reverse !important}.flex-xl-column-reverse{flex-direction:column-reverse !important}.flex-xl-grow-0{flex-grow:0 !important}.flex-xl-grow-1{flex-grow:1 !important}.flex-xl-shrink-0{flex-shrink:0 !important}.flex-xl-shrink-1{flex-shrink:1 !important}.flex-xl-wrap{flex-wrap:wrap !important}.flex-xl-nowrap{flex-wrap:nowrap !important}.flex-xl-wrap-reverse{flex-wrap:wrap-reverse !important}.justify-content-xl-start{justify-content:flex-start !important}.justify-content-xl-end{justify-content:flex-end !important}.justify-content-xl-center{justify-content:center !important}.justify-content-xl-between{justify-content:space-between !important}.justify-content-xl-around{justify-content:space-around !important}.justify-content-xl-evenly{justify-content:space-evenly !important}.align-items-xl-start{align-items:flex-start !important}.align-items-xl-end{align-items:flex-end !important}.align-items-xl-center{align-items:center !important}.align-items-xl-baseline{align-items:baseline !important}.align-items-xl-stretch{align-items:stretch !important}.align-content-xl-start{align-content:flex-start !important}.align-content-xl-end{align-content:flex-end !important}.align-content-xl-center{align-content:center !important}.align-content-xl-between{align-content:space-between !important}.align-content-xl-around{align-content:space-around !important}.align-content-xl-stretch{align-content:stretch !important}.align-self-xl-auto{align-self:auto !important}.align-self-xl-start{align-self:flex-start !important}.align-self-xl-end{align-self:flex-end !important}.align-self-xl-center{align-self:center !important}.align-self-xl-baseline{align-self:baseline !important}.align-self-xl-stretch{align-self:stretch !important}.order-xl-first{order:-1 !important}.order-xl-0{order:0 !important}.order-xl-1{order:1 !important}.order-xl-2{order:2 !important}.order-xl-3{order:3 !important}.order-xl-4{order:4 !important}.order-xl-5{order:5 !important}.order-xl-last{order:6 !important}.m-xl-0{margin:0 !important}.m-xl-1{margin:.25rem !important}.m-xl-2{margin:.5rem !important}.m-xl-3{margin:1rem !important}.m-xl-4{margin:1.5rem !important}.m-xl-5{margin:3rem !important}.m-xl-auto{margin:auto !important}.mx-xl-0{margin-right:0 !important;margin-left:0 !important}.mx-xl-1{margin-right:.25rem !important;margin-left:.25rem !important}.mx-xl-2{margin-right:.5rem !important;margin-left:.5rem !important}.mx-xl-3{margin-right:1rem !important;margin-left:1rem !important}.mx-xl-4{margin-right:1.5rem !important;margin-left:1.5rem !important}.mx-xl-5{margin-right:3rem !important;margin-left:3rem !important}.mx-xl-auto{margin-right:auto !important;margin-left:auto !important}.my-xl-0{margin-top:0 !important;margin-bottom:0 !important}.my-xl-1{margin-top:.25rem !important;margin-bottom:.25rem !important}.my-xl-2{margin-top:.5rem !important;margin-bottom:.5rem !important}.my-xl-3{margin-top:1rem !important;margin-bottom:1rem !important}.my-xl-4{margin-top:1.5rem !important;margin-bottom:1.5rem !important}.my-xl-5{margin-top:3rem !important;margin-bottom:3rem !important}.my-xl-auto{margin-top:auto !important;margin-bottom:auto !important}.mt-xl-0{margin-top:0 !important}.mt-xl-1{margin-top:.25rem !important}.mt-xl-2{margin-top:.5rem !important}.mt-xl-3{margin-top:1rem !important}.mt-xl-4{margin-top:1.5rem !important}.mt-xl-5{margin-top:3rem !important}.mt-xl-auto{margin-top:auto !important}.me-xl-0{margin-right:0 !important}.me-xl-1{margin-right:.25rem !important}.me-xl-2{margin-right:.5rem !important}.me-xl-3{margin-right:1rem !important}.me-xl-4{margin-right:1.5rem !important}.me-xl-5{margin-right:3rem !important}.me-xl-auto{margin-right:auto !important}.mb-xl-0{margin-bottom:0 !important}.mb-xl-1{margin-bottom:.25rem !important}.mb-xl-2{margin-bottom:.5rem !important}.mb-xl-3{margin-bottom:1rem !important}.mb-xl-4{margin-bottom:1.5rem !important}.mb-xl-5{margin-bottom:3rem !important}.mb-xl-auto{margin-bottom:auto !important}.ms-xl-0{margin-left:0 !important}.ms-xl-1{margin-left:.25rem !important}.ms-xl-2{margin-left:.5rem !important}.ms-xl-3{margin-left:1rem !important}.ms-xl-4{margin-left:1.5rem !important}.ms-xl-5{margin-left:3rem !important}.ms-xl-auto{margin-left:auto !important}.p-xl-0{padding:0 !important}.p-xl-1{padding:.25rem !important}.p-xl-2{padding:.5rem !important}.p-xl-3{padding:1rem !important}.p-xl-4{padding:1.5rem !important}.p-xl-5{padding:3rem !important}.px-xl-0{padding-right:0 !important;padding-left:0 !important}.px-xl-1{padding-right:.25rem !important;padding-left:.25rem !important}.px-xl-2{padding-right:.5rem !important;padding-left:.5rem !important}.px-xl-3{padding-right:1rem !important;padding-left:1rem !important}.px-xl-4{padding-right:1.5rem !important;padding-left:1.5rem !important}.px-xl-5{padding-right:3rem !important;padding-left:3rem !important}.py-xl-0{padding-top:0 !important;padding-bottom:0 !important}.py-xl-1{padding-top:.25rem !important;padding-bottom:.25rem !important}.py-xl-2{padding-top:.5rem !important;padding-bottom:.5rem !important}.py-xl-3{padding-top:1rem !important;padding-bottom:1rem !important}.py-xl-4{padding-top:1.5rem !important;padding-bottom:1.5rem !important}.py-xl-5{padding-top:3rem !important;padding-bottom:3rem !important}.pt-xl-0{padding-top:0 !important}.pt-xl-1{padding-top:.25rem !important}.pt-xl-2{padding-top:.5rem !important}.pt-xl-3{padding-top:1rem !important}.pt-xl-4{padding-top:1.5rem !important}.pt-xl-5{padding-top:3rem !important}.pe-xl-0{padding-right:0 !important}.pe-xl-1{padding-right:.25rem !important}.pe-xl-2{padding-right:.5rem !important}.pe-xl-3{padding-right:1rem !important}.pe-xl-4{padding-right:1.5rem !important}.pe-xl-5{padding-right:3rem !important}.pb-xl-0{padding-bottom:0 !important}.pb-xl-1{padding-bottom:.25rem !important}.pb-xl-2{padding-bottom:.5rem !important}.pb-xl-3{padding-bottom:1rem !important}.pb-xl-4{padding-bottom:1.5rem !important}.pb-xl-5{padding-bottom:3rem !important}.ps-xl-0{padding-left:0 !important}.ps-xl-1{padding-left:.25rem !important}.ps-xl-2{padding-left:.5rem !important}.ps-xl-3{padding-left:1rem !important}.ps-xl-4{padding-left:1.5rem !important}.ps-xl-5{padding-left:3rem !important}.gap-xl-0{gap:0 !important}.gap-xl-1{gap:.25rem !important}.gap-xl-2{gap:.5rem !important}.gap-xl-3{gap:1rem !important}.gap-xl-4{gap:1.5rem !important}.gap-xl-5{gap:3rem !important}.text-xl-start{text-align:left !important}.text-xl-end{text-align:right !important}.text-xl-center{text-align:center !important}}@media (min-width: 1400px){.float-xxl-start{float:left !important}.float-xxl-end{float:right !important}.float-xxl-none{float:none !important}.d-xxl-inline{display:inline !important}.d-xxl-inline-block{display:inline-block !important}.d-xxl-block{display:block !important}.d-xxl-grid{display:grid !important}.d-xxl-table{display:table !important}.d-xxl-table-row{display:table-row !important}.d-xxl-table-cell{display:table-cell !important}.d-xxl-flex{display:flex !important}.d-xxl-inline-flex{display:inline-flex !important}.d-xxl-none{display:none !important}.flex-xxl-fill{flex:1 1 auto !important}.flex-xxl-row{flex-direction:row !important}.flex-xxl-column{flex-direction:column !important}.flex-xxl-row-reverse{flex-direction:row-reverse !important}.flex-xxl-column-reverse{flex-direction:column-reverse !important}.flex-xxl-grow-0{flex-grow:0 !important}.flex-xxl-grow-1{flex-grow:1 !important}.flex-xxl-shrink-0{flex-shrink:0 !important}.flex-xxl-shrink-1{flex-shrink:1 !important}.flex-xxl-wrap{flex-wrap:wrap !important}.flex-xxl-nowrap{flex-wrap:nowrap !important}.flex-xxl-wrap-reverse{flex-wrap:wrap-reverse !important}.justify-content-xxl-start{justify-content:flex-start !important}.justify-content-xxl-end{justify-content:flex-end !important}.justify-content-xxl-center{justify-content:center !important}.justify-content-xxl-between{justify-content:space-between !important}.justify-content-xxl-around{justify-content:space-around !important}.justify-content-xxl-evenly{justify-content:space-evenly !important}.align-items-xxl-start{align-items:flex-start !important}.align-items-xxl-end{align-items:flex-end !important}.align-items-xxl-center{align-items:center !important}.align-items-xxl-baseline{align-items:baseline !important}.align-items-xxl-stretch{align-items:stretch !important}.align-content-xxl-start{align-content:flex-start !important}.align-content-xxl-end{align-content:flex-end !important}.align-content-xxl-center{align-content:center !important}.align-content-xxl-between{align-content:space-between !important}.align-content-xxl-around{align-content:space-around !important}.align-content-xxl-stretch{align-content:stretch !important}.align-self-xxl-auto{align-self:auto !important}.align-self-xxl-start{align-self:flex-start !important}.align-self-xxl-end{align-self:flex-end !important}.align-self-xxl-center{align-self:center !important}.align-self-xxl-baseline{align-self:baseline !important}.align-self-xxl-stretch{align-self:stretch !important}.order-xxl-first{order:-1 !important}.order-xxl-0{order:0 !important}.order-xxl-1{order:1 !important}.order-xxl-2{order:2 !important}.order-xxl-3{order:3 !important}.order-xxl-4{order:4 !important}.order-xxl-5{order:5 !important}.order-xxl-last{order:6 !important}.m-xxl-0{margin:0 !important}.m-xxl-1{margin:.25rem !important}.m-xxl-2{margin:.5rem !important}.m-xxl-3{margin:1rem !important}.m-xxl-4{margin:1.5rem !important}.m-xxl-5{margin:3rem !important}.m-xxl-auto{margin:auto !important}.mx-xxl-0{margin-right:0 !important;margin-left:0 !important}.mx-xxl-1{margin-right:.25rem !important;margin-left:.25rem !important}.mx-xxl-2{margin-right:.5rem !important;margin-left:.5rem !important}.mx-xxl-3{margin-right:1rem !important;margin-left:1rem !important}.mx-xxl-4{margin-right:1.5rem !important;margin-left:1.5rem !important}.mx-xxl-5{margin-right:3rem !important;margin-left:3rem !important}.mx-xxl-auto{margin-right:auto !important;margin-left:auto !important}.my-xxl-0{margin-top:0 !important;margin-bottom:0 !important}.my-xxl-1{margin-top:.25rem !important;margin-bottom:.25rem !important}.my-xxl-2{margin-top:.5rem !important;margin-bottom:.5rem !important}.my-xxl-3{margin-top:1rem !important;margin-bottom:1rem !important}.my-xxl-4{margin-top:1.5rem !important;margin-bottom:1.5rem !important}.my-xxl-5{margin-top:3rem !important;margin-bottom:3rem !important}.my-xxl-auto{margin-top:auto !important;margin-bottom:auto !important}.mt-xxl-0{margin-top:0 !important}.mt-xxl-1{margin-top:.25rem !important}.mt-xxl-2{margin-top:.5rem !important}.mt-xxl-3{margin-top:1rem !important}.mt-xxl-4{margin-top:1.5rem !important}.mt-xxl-5{margin-top:3rem !important}.mt-xxl-auto{margin-top:auto !important}.me-xxl-0{margin-right:0 !important}.me-xxl-1{margin-right:.25rem !important}.me-xxl-2{margin-right:.5rem !important}.me-xxl-3{margin-right:1rem !important}.me-xxl-4{margin-right:1.5rem !important}.me-xxl-5{margin-right:3rem !important}.me-xxl-auto{margin-right:auto !important}.mb-xxl-0{margin-bottom:0 !important}.mb-xxl-1{margin-bottom:.25rem !important}.mb-xxl-2{margin-bottom:.5rem !important}.mb-xxl-3{margin-bottom:1rem !important}.mb-xxl-4{margin-bottom:1.5rem !important}.mb-xxl-5{margin-bottom:3rem !important}.mb-xxl-auto{margin-bottom:auto !important}.ms-xxl-0{margin-left:0 !important}.ms-xxl-1{margin-left:.25rem !important}.ms-xxl-2{margin-left:.5rem !important}.ms-xxl-3{margin-left:1rem !important}.ms-xxl-4{margin-left:1.5rem !important}.ms-xxl-5{margin-left:3rem !important}.ms-xxl-auto{margin-left:auto !important}.p-xxl-0{padding:0 !important}.p-xxl-1{padding:.25rem !important}.p-xxl-2{padding:.5rem !important}.p-xxl-3{padding:1rem !important}.p-xxl-4{padding:1.5rem !important}.p-xxl-5{padding:3rem !important}.px-xxl-0{padding-right:0 !important;padding-left:0 !important}.px-xxl-1{padding-right:.25rem !important;padding-left:.25rem !important}.px-xxl-2{padding-right:.5rem !important;padding-left:.5rem !important}.px-xxl-3{padding-right:1rem !important;padding-left:1rem !important}.px-xxl-4{padding-right:1.5rem !important;padding-left:1.5rem !important}.px-xxl-5{padding-right:3rem !important;padding-left:3rem !important}.py-xxl-0{padding-top:0 !important;padding-bottom:0 !important}.py-xxl-1{padding-top:.25rem !important;padding-bottom:.25rem !important}.py-xxl-2{padding-top:.5rem !important;padding-bottom:.5rem !important}.py-xxl-3{padding-top:1rem !important;padding-bottom:1rem !important}.py-xxl-4{padding-top:1.5rem !important;padding-bottom:1.5rem !important}.py-xxl-5{padding-top:3rem !important;padding-bottom:3rem !important}.pt-xxl-0{padding-top:0 !important}.pt-xxl-1{padding-top:.25rem !important}.pt-xxl-2{padding-top:.5rem !important}.pt-xxl-3{padding-top:1rem !important}.pt-xxl-4{padding-top:1.5rem !important}.pt-xxl-5{padding-top:3rem !important}.pe-xxl-0{padding-right:0 !important}.pe-xxl-1{padding-right:.25rem !important}.pe-xxl-2{padding-right:.5rem !important}.pe-xxl-3{padding-right:1rem !important}.pe-xxl-4{padding-right:1.5rem !important}.pe-xxl-5{padding-right:3rem !important}.pb-xxl-0{padding-bottom:0 !important}.pb-xxl-1{padding-bottom:.25rem !important}.pb-xxl-2{padding-bottom:.5rem !important}.pb-xxl-3{padding-bottom:1rem !important}.pb-xxl-4{padding-bottom:1.5rem !important}.pb-xxl-5{padding-bottom:3rem !important}.ps-xxl-0{padding-left:0 !important}.ps-xxl-1{padding-left:.25rem !important}.ps-xxl-2{padding-left:.5rem !important}.ps-xxl-3{padding-left:1rem !important}.ps-xxl-4{padding-left:1.5rem !important}.ps-xxl-5{padding-left:3rem !important}.gap-xxl-0{gap:0 !important}.gap-xxl-1{gap:.25rem !important}.gap-xxl-2{gap:.5rem !important}.gap-xxl-3{gap:1rem !important}.gap-xxl-4{gap:1.5rem !important}.gap-xxl-5{gap:3rem !important}.text-xxl-start{text-align:left !important}.text-xxl-end{text-align:right !important}.text-xxl-center{text-align:center !important}}.bg-default{color:#000}.bg-primary{color:#fff}.bg-secondary{color:#fff}.bg-success{color:#fff}.bg-info{color:#000}.bg-warning{color:#000}.bg-danger{color:#fff}.bg-light{color:#000}.bg-dark{color:#fff}@media (min-width: 1200px){.fs-1{font-size:2.5rem !important}.fs-2{font-size:2rem !important}.fs-3{font-size:1.75rem !important}.fs-4{font-size:1.5rem !important}}@media print{.d-print-inline{display:inline !important}.d-print-inline-block{display:inline-block !important}.d-print-block{display:block !important}.d-print-grid{display:grid !important}.d-print-table{display:table !important}.d-print-table-row{display:table-row !important}.d-print-table-cell{display:table-cell !important}.d-print-flex{display:flex !important}.d-print-inline-flex{display:inline-flex !important}.d-print-none{display:none !important}}.table th[align=left]{text-align:left}.table th[align=right]{text-align:right}.table th[align=center]{text-align:center}.well{display:block;background-color:rgba(0,0,0,0.03);color:#212529;padding:1rem;border-radius:.375rem}.well-lg{padding:1.5rem;border-radius:.5rem}.well-sm{padding:0.5rem;border-radius:.25rem}.draggable .well{background-color:#f7f7f7}.dropdown-menu>li.active>a{color:#fff;text-decoration:none;background-color:#0d6efd}.navbar:not(.fixed-bottom):not(.navbar-fixed-bottom):not(.navbar-fixed-bottom)+div>.tab-content>.tab-pane{--bslib-navbar-margin: 20px;margin-top:var(--bslib-navbar-margin)}ul.nav.navbar-nav{flex:1;-webkit-flex:1}ul.nav.navbar-nav.navbar-right{flex:unset;-webkit-flex:unset;display:flex;display:-webkit-flex;justify-content:flex-end;-webkit-justify-content:flex-end}.navbar.navbar-default{background-color:#f8f9fa !important}.navbar.navbar-inverse{background-color:#212529 !important}.navbar-toggle>.icon-bar{display:none}@media (max-width: 575.98px){.navbar-header{width:100%}.navbar-header .navbar-toggle{float:right}}.nav-tabs>li.active>a{color:#495057;background-color:#fff;border-color:#dee2e6 #dee2e6 #fff}.nav-pills>li.active>a{color:#fff;background-color:#0d6efd}.nav-stacked{flex-direction:column;-webkit-flex-direction:column}.progress-bar-default{background-color:#dee2e6;color:#000}.progress-bar-primary{background-color:#0d6efd;color:#fff}.progress-bar-secondary{background-color:#6c757d;color:#fff}.progress-bar-success{background-color:#198754;color:#fff}.progress-bar-info{background-color:#0dcaf0;color:#000}.progress-bar-warning{background-color:#ffc107;color:#000}.progress-bar-danger{background-color:#dc3545;color:#fff}.progress-bar-light{background-color:#f8f9fa;color:#000}.progress-bar-dark{background-color:#212529;color:#fff}@font-face{font-family:'Glyphicons Halflings';src:url("fonts/bootstrap/glyphicons-halflings-regular.eot");src:url("fonts/bootstrap/glyphicons-halflings-regular.eot?#iefix") format("embedded-opentype"),url("fonts/bootstrap/glyphicons-halflings-regular.woff2") format("woff2"),url("fonts/bootstrap/glyphicons-halflings-regular.woff") format("woff"),url("fonts/bootstrap/glyphicons-halflings-regular.ttf") format("truetype"),url("fonts/bootstrap/glyphicons-halflings-regular.svg#glyphicons_halflingsregular") format("svg")}.glyphicon{position:relative;top:1px;display:inline-block;font-family:'Glyphicons Halflings';font-style:normal;font-weight:normal;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.glyphicon-asterisk:before{content:"\2a"}.glyphicon-plus:before{content:"\2b"}.glyphicon-euro:before,.glyphicon-eur:before{content:"\20ac"}.glyphicon-minus:before{content:"\2212"}.glyphicon-cloud:before{content:"\2601"}.glyphicon-envelope:before{content:"\2709"}.glyphicon-pencil:before{content:"\270f"}.glyphicon-glass:before{content:"\e001"}.glyphicon-music:before{content:"\e002"}.glyphicon-search:before{content:"\e003"}.glyphicon-heart:before{content:"\e005"}.glyphicon-star:before{content:"\e006"}.glyphicon-star-empty:before{content:"\e007"}.glyphicon-user:before{content:"\e008"}.glyphicon-film:before{content:"\e009"}.glyphicon-th-large:before{content:"\e010"}.glyphicon-th:before{content:"\e011"}.glyphicon-th-list:before{content:"\e012"}.glyphicon-ok:before{content:"\e013"}.glyphicon-remove:before{content:"\e014"}.glyphicon-zoom-in:before{content:"\e015"}.glyphicon-zoom-out:before{content:"\e016"}.glyphicon-off:before{content:"\e017"}.glyphicon-signal:before{content:"\e018"}.glyphicon-cog:before{content:"\e019"}.glyphicon-trash:before{content:"\e020"}.glyphicon-home:before{content:"\e021"}.glyphicon-file:before{content:"\e022"}.glyphicon-time:before{content:"\e023"}.glyphicon-road:before{content:"\e024"}.glyphicon-download-alt:before{content:"\e025"}.glyphicon-download:before{content:"\e026"}.glyphicon-upload:before{content:"\e027"}.glyphicon-inbox:before{content:"\e028"}.glyphicon-play-circle:before{content:"\e029"}.glyphicon-repeat:before{content:"\e030"}.glyphicon-refresh:before{content:"\e031"}.glyphicon-list-alt:before{content:"\e032"}.glyphicon-lock:before{content:"\e033"}.glyphicon-flag:before{content:"\e034"}.glyphicon-headphones:before{content:"\e035"}.glyphicon-volume-off:before{content:"\e036"}.glyphicon-volume-down:before{content:"\e037"}.glyphicon-volume-up:before{content:"\e038"}.glyphicon-qrcode:before{content:"\e039"}.glyphicon-barcode:before{content:"\e040"}.glyphicon-tag:before{content:"\e041"}.glyphicon-tags:before{content:"\e042"}.glyphicon-book:before{content:"\e043"}.glyphicon-bookmark:before{content:"\e044"}.glyphicon-print:before{content:"\e045"}.glyphicon-camera:before{content:"\e046"}.glyphicon-font:before{content:"\e047"}.glyphicon-bold:before{content:"\e048"}.glyphicon-italic:before{content:"\e049"}.glyphicon-text-height:before{content:"\e050"}.glyphicon-text-width:before{content:"\e051"}.glyphicon-align-left:before{content:"\e052"}.glyphicon-align-center:before{content:"\e053"}.glyphicon-align-right:before{content:"\e054"}.glyphicon-align-justify:before{content:"\e055"}.glyphicon-list:before{content:"\e056"}.glyphicon-indent-left:before{content:"\e057"}.glyphicon-indent-right:before{content:"\e058"}.glyphicon-facetime-video:before{content:"\e059"}.glyphicon-picture:before{content:"\e060"}.glyphicon-map-marker:before{content:"\e062"}.glyphicon-adjust:before{content:"\e063"}.glyphicon-tint:before{content:"\e064"}.glyphicon-edit:before{content:"\e065"}.glyphicon-share:before{content:"\e066"}.glyphicon-check:before{content:"\e067"}.glyphicon-move:before{content:"\e068"}.glyphicon-step-backward:before{content:"\e069"}.glyphicon-fast-backward:before{content:"\e070"}.glyphicon-backward:before{content:"\e071"}.glyphicon-play:before{content:"\e072"}.glyphicon-pause:before{content:"\e073"}.glyphicon-stop:before{content:"\e074"}.glyphicon-forward:before{content:"\e075"}.glyphicon-fast-forward:before{content:"\e076"}.glyphicon-step-forward:before{content:"\e077"}.glyphicon-eject:before{content:"\e078"}.glyphicon-chevron-left:before{content:"\e079"}.glyphicon-chevron-right:before{content:"\e080"}.glyphicon-plus-sign:before{content:"\e081"}.glyphicon-minus-sign:before{content:"\e082"}.glyphicon-remove-sign:before{content:"\e083"}.glyphicon-ok-sign:before{content:"\e084"}.glyphicon-question-sign:before{content:"\e085"}.glyphicon-info-sign:before{content:"\e086"}.glyphicon-screenshot:before{content:"\e087"}.glyphicon-remove-circle:before{content:"\e088"}.glyphicon-ok-circle:before{content:"\e089"}.glyphicon-ban-circle:before{content:"\e090"}.glyphicon-arrow-left:before{content:"\e091"}.glyphicon-arrow-right:before{content:"\e092"}.glyphicon-arrow-up:before{content:"\e093"}.glyphicon-arrow-down:before{content:"\e094"}.glyphicon-share-alt:before{content:"\e095"}.glyphicon-resize-full:before{content:"\e096"}.glyphicon-resize-small:before{content:"\e097"}.glyphicon-exclamation-sign:before{content:"\e101"}.glyphicon-gift:before{content:"\e102"}.glyphicon-leaf:before{content:"\e103"}.glyphicon-fire:before{content:"\e104"}.glyphicon-eye-open:before{content:"\e105"}.glyphicon-eye-close:before{content:"\e106"}.glyphicon-warning-sign:before{content:"\e107"}.glyphicon-plane:before{content:"\e108"}.glyphicon-calendar:before{content:"\e109"}.glyphicon-random:before{content:"\e110"}.glyphicon-comment:before{content:"\e111"}.glyphicon-magnet:before{content:"\e112"}.glyphicon-chevron-up:before{content:"\e113"}.glyphicon-chevron-down:before{content:"\e114"}.glyphicon-retweet:before{content:"\e115"}.glyphicon-shopping-cart:before{content:"\e116"}.glyphicon-folder-close:before{content:"\e117"}.glyphicon-folder-open:before{content:"\e118"}.glyphicon-resize-vertical:before{content:"\e119"}.glyphicon-resize-horizontal:before{content:"\e120"}.glyphicon-hdd:before{content:"\e121"}.glyphicon-bullhorn:before{content:"\e122"}.glyphicon-bell:before{content:"\e123"}.glyphicon-certificate:before{content:"\e124"}.glyphicon-thumbs-up:before{content:"\e125"}.glyphicon-thumbs-down:before{content:"\e126"}.glyphicon-hand-right:before{content:"\e127"}.glyphicon-hand-left:before{content:"\e128"}.glyphicon-hand-up:before{content:"\e129"}.glyphicon-hand-down:before{content:"\e130"}.glyphicon-circle-arrow-right:before{content:"\e131"}.glyphicon-circle-arrow-left:before{content:"\e132"}.glyphicon-circle-arrow-up:before{content:"\e133"}.glyphicon-circle-arrow-down:before{content:"\e134"}.glyphicon-globe:before{content:"\e135"}.glyphicon-wrench:before{content:"\e136"}.glyphicon-tasks:before{content:"\e137"}.glyphicon-filter:before{content:"\e138"}.glyphicon-briefcase:before{content:"\e139"}.glyphicon-fullscreen:before{content:"\e140"}.glyphicon-dashboard:before{content:"\e141"}.glyphicon-paperclip:before{content:"\e142"}.glyphicon-heart-empty:before{content:"\e143"}.glyphicon-link:before{content:"\e144"}.glyphicon-phone:before{content:"\e145"}.glyphicon-pushpin:before{content:"\e146"}.glyphicon-usd:before{content:"\e148"}.glyphicon-gbp:before{content:"\e149"}.glyphicon-sort:before{content:"\e150"}.glyphicon-sort-by-alphabet:before{content:"\e151"}.glyphicon-sort-by-alphabet-alt:before{content:"\e152"}.glyphicon-sort-by-order:before{content:"\e153"}.glyphicon-sort-by-order-alt:before{content:"\e154"}.glyphicon-sort-by-attributes:before{content:"\e155"}.glyphicon-sort-by-attributes-alt:before{content:"\e156"}.glyphicon-unchecked:before{content:"\e157"}.glyphicon-expand:before{content:"\e158"}.glyphicon-collapse-down:before{content:"\e159"}.glyphicon-collapse-up:before{content:"\e160"}.glyphicon-log-in:before{content:"\e161"}.glyphicon-flash:before{content:"\e162"}.glyphicon-log-out:before{content:"\e163"}.glyphicon-new-window:before{content:"\e164"}.glyphicon-record:before{content:"\e165"}.glyphicon-save:before{content:"\e166"}.glyphicon-open:before{content:"\e167"}.glyphicon-saved:before{content:"\e168"}.glyphicon-import:before{content:"\e169"}.glyphicon-export:before{content:"\e170"}.glyphicon-send:before{content:"\e171"}.glyphicon-floppy-disk:before{content:"\e172"}.glyphicon-floppy-saved:before{content:"\e173"}.glyphicon-floppy-remove:before{content:"\e174"}.glyphicon-floppy-save:before{content:"\e175"}.glyphicon-floppy-open:before{content:"\e176"}.glyphicon-credit-card:before{content:"\e177"}.glyphicon-transfer:before{content:"\e178"}.glyphicon-cutlery:before{content:"\e179"}.glyphicon-header:before{content:"\e180"}.glyphicon-compressed:before{content:"\e181"}.glyphicon-earphone:before{content:"\e182"}.glyphicon-phone-alt:before{content:"\e183"}.glyphicon-tower:before{content:"\e184"}.glyphicon-stats:before{content:"\e185"}.glyphicon-sd-video:before{content:"\e186"}.glyphicon-hd-video:before{content:"\e187"}.glyphicon-subtitles:before{content:"\e188"}.glyphicon-sound-stereo:before{content:"\e189"}.glyphicon-sound-dolby:before{content:"\e190"}.glyphicon-sound-5-1:before{content:"\e191"}.glyphicon-sound-6-1:before{content:"\e192"}.glyphicon-sound-7-1:before{content:"\e193"}.glyphicon-copyright-mark:before{content:"\e194"}.glyphicon-registration-mark:before{content:"\e195"}.glyphicon-cloud-download:before{content:"\e197"}.glyphicon-cloud-upload:before{content:"\e198"}.glyphicon-tree-conifer:before{content:"\e199"}.glyphicon-tree-deciduous:before{content:"\e200"}.glyphicon-cd:before{content:"\e201"}.glyphicon-save-file:before{content:"\e202"}.glyphicon-open-file:before{content:"\e203"}.glyphicon-level-up:before{content:"\e204"}.glyphicon-copy:before{content:"\e205"}.glyphicon-paste:before{content:"\e206"}.glyphicon-alert:before{content:"\e209"}.glyphicon-equalizer:before{content:"\e210"}.glyphicon-king:before{content:"\e211"}.glyphicon-queen:before{content:"\e212"}.glyphicon-pawn:before{content:"\e213"}.glyphicon-bishop:before{content:"\e214"}.glyphicon-knight:before{content:"\e215"}.glyphicon-baby-formula:before{content:"\e216"}.glyphicon-tent:before{content:"\26fa"}.glyphicon-blackboard:before{content:"\e218"}.glyphicon-bed:before{content:"\e219"}.glyphicon-apple:before{content:"\f8ff"}.glyphicon-erase:before{content:"\e221"}.glyphicon-hourglass:before{content:"\231b"}.glyphicon-lamp:before{content:"\e223"}.glyphicon-duplicate:before{content:"\e224"}.glyphicon-piggy-bank:before{content:"\e225"}.glyphicon-scissors:before{content:"\e226"}.glyphicon-bitcoin:before{content:"\e227"}.glyphicon-btc:before{content:"\e227"}.glyphicon-xbt:before{content:"\e227"}.glyphicon-yen:before{content:"\00a5"}.glyphicon-jpy:before{content:"\00a5"}.glyphicon-ruble:before{content:"\20bd"}.glyphicon-rub:before{content:"\20bd"}.glyphicon-scale:before{content:"\e230"}.glyphicon-ice-lolly:before{content:"\e231"}.glyphicon-ice-lolly-tasted:before{content:"\e232"}.glyphicon-education:before{content:"\e233"}.glyphicon-option-horizontal:before{content:"\e234"}.glyphicon-option-vertical:before{content:"\e235"}.glyphicon-menu-hamburger:before{content:"\e236"}.glyphicon-modal-window:before{content:"\e237"}.glyphicon-oil:before{content:"\e238"}.glyphicon-grain:before{content:"\e239"}.glyphicon-sunglasses:before{content:"\e240"}.glyphicon-text-size:before{content:"\e241"}.glyphicon-text-color:before{content:"\e242"}.glyphicon-text-background:before{content:"\e243"}.glyphicon-object-align-top:before{content:"\e244"}.glyphicon-object-align-bottom:before{content:"\e245"}.glyphicon-object-align-horizontal:before{content:"\e246"}.glyphicon-object-align-left:before{content:"\e247"}.glyphicon-object-align-vertical:before{content:"\e248"}.glyphicon-object-align-right:before{content:"\e249"}.glyphicon-triangle-right:before{content:"\e250"}.glyphicon-triangle-left:before{content:"\e251"}.glyphicon-triangle-bottom:before{content:"\e252"}.glyphicon-triangle-top:before{content:"\e253"}.glyphicon-console:before{content:"\e254"}.glyphicon-superscript:before{content:"\e255"}.glyphicon-subscript:before{content:"\e256"}.glyphicon-menu-left:before{content:"\e257"}.glyphicon-menu-right:before{content:"\e258"}.glyphicon-menu-down:before{content:"\e259"}.glyphicon-menu-up:before{content:"\e260"}.form-group{margin-bottom:1rem}.input-daterange .input-group-addon.input-group-prepend.input-group-append{padding:inherit;line-height:inherit;text-shadow:inherit;border-width:0}.input-daterange .input-group-addon.input-group-prepend.input-group-append .input-group-text{border-radius:0}pre.shiny-code{padding:0.5rem}.section.level1,.section.level2,.section.level3,section.level1,section.level2,section.level3{margin-top:1.5rem}.section.level4,.section.level5,.section.level6,section.level4,section.level5,section.level6{margin-top:1rem}.accordion .accordion-icon:not(:empty){margin-right:0.25rem;display:flex}.accordion .accordion-button:not(.collapsed){box-shadow:none}.accordion .accordion-button:not(.collapsed):focus{box-shadow:var(--bs-accordion-btn-focus-box-shadow)}.bslib-card .card-body+.card-body{padding-top:0}.bslib-card .card-body{overflow:auto}.bslib-card .card-body p{margin-top:0}.bslib-card .card-body p:last-child{margin-bottom:0}.bslib-card .card-body{max-height:var(--bslib-card-body-max-height, none)}.bslib-card.bslib-full-screen>.card-body{max-height:var(--bslib-card-body-max-height-full-screen, none)}.bslib-card .card-header .form-group{margin-bottom:0}.bslib-card .card-header .selectize-control{margin-bottom:0}.bslib-card .card-header .selectize-control .item{margin-right:1.15rem}.bslib-card .card-footer{margin-top:auto}.bslib-card .bslib-navs-card-title{display:flex;flex-wrap:wrap;justify-content:space-between;align-items:center}.bslib-card .bslib-navs-card-title .nav{margin-left:auto}.bslib-card .bslib-sidebar-layout:not([data-bslib-sidebar-border="true"]){border:none}.bslib-card .bslib-sidebar-layout:not([data-bslib-sidebar-border-radius="true"]){border-top-left-radius:0;border-top-right-radius:0}.bslib-full-screen{position:fixed;inset:3.5rem 1rem 1rem;height:auto !important;max-height:none !important;width:auto !important;z-index:1070}.bslib-full-screen-enter{display:none;position:absolute;bottom:1px;right:3px;margin:0.5rem;padding:0.55rem !important;font-size:.8rem;cursor:pointer;opacity:.6;color:rgba(var(--bs-body-bg-rgb), 1);z-index:1070}.bslib-full-screen-enter:hover{opacity:1}.card:hover:not(.bslib-full-screen) .bslib-full-screen-enter,.well:hover:not(.bslib-full-screen) .bslib-full-screen-enter{display:block}@media (max-width: 575.98px){.bslib-full-screen-enter{display:none !important}}.bslib-full-screen-exit{position:relative;top:1.35rem;font-size:0.9rem;cursor:pointer;text-decoration:none;display:flex;float:right;margin-right:2.15rem;align-items:center;color:rgba(var(--bs-body-bg-rgb), 0.8)}.bslib-full-screen-exit:hover{color:rgba(var(--bs-body-bg-rgb), 1)}.bslib-full-screen-exit svg{margin-left:0.5rem;font-size:1.5rem}#bslib-full-screen-overlay{position:fixed;inset:0;background-color:rgba(var(--bs-body-color-rgb), 0.6);z-index:1069}.tab-content>.tab-pane.html-fill-container{display:none}.tab-content>.active.html-fill-container{display:flex}.tab-content.html-fill-container{padding:0}.bslib-page-fill{width:100%;height:100%;margin:0;padding:1rem;gap:1rem}@media (max-width: 575.98px){.bslib-page-fill{height:var(--bslib-page-fill-mobile-height, auto)}}.bslib-column-wrap{display:grid !important;gap:1rem;height:var(--bslib-column-wrap-height)}.bslib-column-wrap .card,.bslib-column-wrap .well{margin-bottom:0}@media (max-width: 575.98px){.bslib-column-wrap{grid-template-columns:1fr !important;height:var(--bslib-column-wrap-height-mobile)}}.bslib-sidebar-layout{--bslib-sidebar-transition: grid-template-columns ease-in-out 0.5s;--bslib-sidebar-border: var(--bs-card-border-width, 1px) solid var(--bs-card-border-color, var(--bs-border-color-translucent));--bslib-sidebar-border-radius: var(--bs-border-radius);--bslib-sidebar-vert-border: var(--bs-card-border-width, 1px) solid var(--bs-card-border-color, var(--bs-border-color-translucent));--bslib-collapse-toggle-border: var(--bs-card-border-width, 1px) solid var(--bs-card-border-color, var(--bs-border-color-translucent));--bslib-collapse-toggle-transform: 90deg;--bslib-collapse-toggle-right-transform: -90deg;display:grid !important;grid-template-columns:Min(calc(100% - 1rem), var(--bslib-sidebar-width, 250px)) minmax(0, 1fr);position:relative;transition:var(--bslib-sidebar-transition);border:var(--bslib-sidebar-border);border-radius:var(--bslib-sidebar-border-radius)}@media (prefers-reduced-motion: reduce){.bslib-sidebar-layout{transition:none}}.bslib-sidebar-layout[data-bslib-sidebar-border="false"]{border:none}.bslib-sidebar-layout[data-bslib-sidebar-border-radius="false"]{border-radius:initial}.bslib-sidebar-layout>.main,.bslib-sidebar-layout>.sidebar{grid-row:1 / 2;border-radius:inherit;overflow:auto}.bslib-sidebar-layout>.main{grid-column:2 / 3;border-top-left-radius:0;border-bottom-left-radius:0;padding:1.5rem}.bslib-sidebar-layout>.sidebar{grid-column:1 / 2;width:100%;height:100%;border-right:var(--bslib-sidebar-vert-border);border-top-right-radius:0;border-bottom-right-radius:0;background-color:#f8f9fa;color:#000}.bslib-sidebar-layout>.sidebar>.sidebar-content{display:flex;flex-direction:column;padding:1.5rem}.bslib-sidebar-layout>.sidebar>.sidebar-content>:last-child:not(.sidebar-title){margin-bottom:0}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion{margin-left:-1.5rem;margin-right:-1.5rem}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion:first-child{margin-top:-1.5rem}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion:last-child{margin-bottom:-1.5rem}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion:not(:last-child){margin-bottom:1rem}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion .accordion-body{display:flex;flex-direction:column}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion:not(:first-child) .accordion-item:first-child{border-top:var(--bs-accordion-border-width) solid var(--bs-accordion-border-color)}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion:not(:last-child) .accordion-item:last-child{border-bottom:var(--bs-accordion-border-width) solid var(--bs-accordion-border-color)}.bslib-sidebar-layout>.sidebar>.sidebar-content>.sidebar-title+.accordion{margin-top:calc(-1rem - var(--bs-card-border-width, 1px))}.bslib-sidebar-layout>.sidebar>.sidebar-content>.sidebar-title:has(+.accordion){border-bottom:none}.bslib-sidebar-layout>.sidebar .shiny-input-container{width:100%}.bslib-sidebar-layout>.collapse-toggle{grid-row:1 / 2;grid-column:1 / 2;display:inline-flex;align-items:center;position:absolute;right:-1rem;bottom:calc(1.5rem + var(--bslib-sidebar-overlap-counter, 0) * calc(1rem + 1.5rem));border:var(--bslib-collapse-toggle-border);border-left:none;border-radius:0 var(--bs-border-radius) var(--bs-border-radius) 0;padding:7px 0;background-color:#f8f9fa;color:#000}.bslib-sidebar-layout>.collapse-toggle>.collapse-icon{opacity:0.8;width:1rem;height:1rem;transform:rotate(var(--bslib-collapse-toggle-transform));transition:transform ease-in-out 0.35s}.bslib-sidebar-layout>.collapse-toggle:hover>.collapse-icon{opacity:1}.bslib-sidebar-layout .sidebar-title{font-size:1.25rem;line-height:1.25;margin-top:0;margin-bottom:1rem;padding-bottom:1rem;border-bottom:var(--bslib-sidebar-border)}.bslib-sidebar-layout.sidebar-right{grid-template-columns:minmax(0, 1fr) Min(calc(100% - 1rem), var(--bslib-sidebar-width, 250px))}.bslib-sidebar-layout.sidebar-right>.main{grid-column:1 / 2;border-top-right-radius:0;border-bottom-right-radius:0;border-top-left-radius:inherit;border-bottom-left-radius:inherit}.bslib-sidebar-layout.sidebar-right>.sidebar{grid-column:2 / 3;border-right:none;border-left:var(--bslib-sidebar-vert-border);border-top-left-radius:0;border-bottom-left-radius:0}.bslib-sidebar-layout.sidebar-right>.collapse-toggle{grid-column:2 / 3;left:-1rem;right:unset;border-radius:var(--bs-border-radius) 0 0 var(--bs-border-radius);border-right:none;border-left:var(--bslib-collapse-toggle-border)}.bslib-sidebar-layout.sidebar-right>.collapse-toggle>.collapse-icon{transform:rotate(var(--bslib-collapse-toggle-right-transform))}.bslib-sidebar-layout.sidebar-collapsed{--bslib-collapse-toggle-transform: -90deg;--bslib-collapse-toggle-right-transform: 90deg;--bslib-sidebar-vert-border: none;grid-template-columns:0 minmax(0, 1fr)}.bslib-sidebar-layout.sidebar-collapsed.sidebar-right{grid-template-columns:minmax(0, 1fr) 0}.bslib-sidebar-layout.sidebar-collapsed:not(.transitioning)>.sidebar>*{display:none}.bslib-sidebar-layout.sidebar-collapsed>.main{border-radius:inherit}.bslib-sidebar-layout.sidebar-collapsed>.collapse-toggle{right:calc(-1rem - var(--bs-card-border-width, 1px))}.bslib-sidebar-layout.sidebar-collapsed.sidebar-right>.collapse-toggle{left:calc(-1rem - var(--bs-card-border-width, 1px));right:unset}@media (min-width: 576px){.bslib-sidebar-layout.transitioning>.sidebar>.sidebar-content{display:none}}@media (max-width: 575.98px){.bslib-sidebar-layout,.bslib-sidebar-layout.sidebar-right{--bslib-sidebar-vert-border: none;--bslib-sidebar-horiz-border: var(--bs-card-border-width, 1px) solid var(--bs-card-border-color, var(--bs-border-color-translucent));--bslib-collapse-toggle-transform: -180deg;--bslib-collapse-toggle-right-transform: -180deg;grid-template-columns:1fr !important;grid-template-rows:fit-content(var(--bslib-sidebar-max-height-mobile, auto)) minmax(0, 1fr)}.bslib-sidebar-layout[data-bslib-sidebar-open="desktop"],.bslib-sidebar-layout.sidebar-right[data-bslib-sidebar-open="desktop"]{--bslib-sidebar-js-init-collapsed: true}.bslib-sidebar-layout>.sidebar,.bslib-sidebar-layout.sidebar-right>.sidebar{grid-row:1 / 2;grid-column:1 / 2;width:100%;border:none;border-bottom:var(--bslib-sidebar-horiz-border);border-radius:0}.bslib-sidebar-layout>.main,.bslib-sidebar-layout.sidebar-right>.main{grid-row:2 / 3;grid-column:1 / 2;border-top-left-radius:0;border-top-right-radius:0;border-bottom-right-radius:inherit;border-bottom-left-radius:inherit}.bslib-sidebar-layout>.collapse-toggle,.bslib-sidebar-layout.sidebar-right>.collapse-toggle{grid-row:2 / 3;grid-column:1 / 2;border-top:none !important;border:var(--bslib-collapse-toggle-border);border-radius:0 0 var(--bs-border-radius) var(--bs-border-radius);padding:0 4px}.bslib-sidebar-layout>.collapse-toggle,.bslib-sidebar-layout.sidebar-right>.collapse-toggle,.bslib-sidebar-layout.sidebar-right>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-right>.collapse-toggle{top:calc(-1 * var(--bs-card-border-width, 1px))}.bslib-sidebar-layout.sidebar-collapsed>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-right.sidebar-collapsed>.collapse-toggle{top:0}.bslib-sidebar-layout>.collapse-toggle,.bslib-sidebar-layout.sidebar-collapsed>.collapse-toggle,.bslib-sidebar-layout.sidebar-right>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed>.collapse-toggle,.bslib-sidebar-layout.sidebar-right>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-right>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-right.sidebar-collapsed>.collapse-toggle{right:calc(1.5rem + var(--bslib-sidebar-counter, 0) * calc(1rem + 1.5rem));bottom:initial;left:initial}.bslib-sidebar-layout.sidebar-collapsed,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed{--bslib-collapse-toggle-transform: 0deg;--bslib-collapse-toggle-right-transform: 0deg;grid-template-rows:0 minmax(0, 1fr)}.bslib-sidebar-layout.sidebar-collapsed>.main,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed>.main{border-top-left-radius:inherit;border-top-right-radius:inherit}.bslib-sidebar-layout.sidebar-collapsed>.sidebar,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed>.sidebar{border-bottom:none}}.navbar+.container-fluid:has(>.tab-content>.tab-pane.active>.bslib-sidebar-layout),.navbar+.container-sm:has(>.tab-content>.tab-pane.active>.bslib-sidebar-layout),.navbar+.container-md:has(>.tab-content>.tab-pane.active>.bslib-sidebar-layout),.navbar+.container-lg:has(>.tab-content>.tab-pane.active>.bslib-sidebar-layout),.navbar+.container-xl:has(>.tab-content>.tab-pane.active>.bslib-sidebar-layout),.navbar+.container-xxl:has(>.tab-content>.tab-pane.active>.bslib-sidebar-layout){padding-left:0;padding-right:0}.navbar+.container-fluid>.tab-content>.tab-pane.active>.bslib-sidebar-layout:not([data-bslib-sidebar-border="true"]),.navbar+.container-sm>.tab-content>.tab-pane.active>.bslib-sidebar-layout:not([data-bslib-sidebar-border="true"]),.navbar+.container-md>.tab-content>.tab-pane.active>.bslib-sidebar-layout:not([data-bslib-sidebar-border="true"]),.navbar+.container-lg>.tab-content>.tab-pane.active>.bslib-sidebar-layout:not([data-bslib-sidebar-border="true"]),.navbar+.container-xl>.tab-content>.tab-pane.active>.bslib-sidebar-layout:not([data-bslib-sidebar-border="true"]),.navbar+.container-xxl>.tab-content>.tab-pane.active>.bslib-sidebar-layout:not([data-bslib-sidebar-border="true"]){border:none}.navbar+.container-fluid>.tab-content>.tab-pane.active>.bslib-sidebar-layout:not([data-bslib-sidebar-border-radius="true"]),.navbar+.container-sm>.tab-content>.tab-pane.active>.bslib-sidebar-layout:not([data-bslib-sidebar-border-radius="true"]),.navbar+.container-md>.tab-content>.tab-pane.active>.bslib-sidebar-layout:not([data-bslib-sidebar-border-radius="true"]),.navbar+.container-lg>.tab-content>.tab-pane.active>.bslib-sidebar-layout:not([data-bslib-sidebar-border-radius="true"]),.navbar+.container-xl>.tab-content>.tab-pane.active>.bslib-sidebar-layout:not([data-bslib-sidebar-border-radius="true"]),.navbar+.container-xxl>.tab-content>.tab-pane.active>.bslib-sidebar-layout:not([data-bslib-sidebar-border-radius="true"]){border-radius:0}.bslib-value-box .value-box-grid{grid-template-columns:var(--bslib-value-box-widths)}.bslib-value-box .value-box-showcase{align-items:center;justify-content:center;margin-top:auto;margin-bottom:auto;padding:1rem;max-height:var(--bslib-value-box-max-height)}.bslib-value-box .value-box-showcase .bi,.bslib-value-box .value-box-showcase .fa{opacity:.85}.bslib-value-box .value-box-showcase .bi{font-size:5rem}.bslib-value-box .value-box-showcase .fa{font-size:4rem}.bslib-value-box .value-box-showcase.showcase-top-right{align-items:end;padding-left:0;padding-bottom:0}.bslib-value-box .value-box-area{justify-content:center;padding:1.5rem 1rem;font-size:.9rem;font-weight:500}.bslib-value-box .value-box-area *{color:inherit;margin-bottom:0;margin-top:0}.bslib-value-box .value-box-area.border-start{border-color:rgba(222,226,230,0.3) !important}.bslib-value-box.bslib-full-screen .value-box-grid{grid-template-columns:var(--bslib-value-box-widths-full-screen)}.bslib-value-box.bslib-full-screen .value-box-showcase{max-height:var(--bslib-value-box-max-height-full-screen)}.bslib-value-box:not(.bslib-full-screen) .value-box-showcase.showcase-top-right{margin-top:0}@media (max-width: 575.98px){.bslib-value-box .value-box-grid{grid-template-columns:var(--bslib-value-box-widths) !important}}@media (min-width: 576px){.nav:not(.nav-hidden){display:flex !important;display:-webkit-flex !important}.nav:not(.nav-hidden):not(.nav-stacked):not(.flex-column){float:none !important}.nav:not(.nav-hidden):not(.nav-stacked):not(.flex-column)>.bslib-nav-spacer{margin-left:auto !important}.nav:not(.nav-hidden):not(.nav-stacked):not(.flex-column)>.form-inline{margin-top:auto;margin-bottom:auto}.nav:not(.nav-hidden).nav-stacked{flex-direction:column;-webkit-flex-direction:column;height:100%}.nav:not(.nav-hidden).nav-stacked>.bslib-nav-spacer{margin-top:auto !important}}
+   */:root{--bs-blue: #0d6efd;--bs-indigo: #6610f2;--bs-purple: #6f42c1;--bs-pink: #d63384;--bs-red: #dc3545;--bs-orange: #fd7e14;--bs-yellow: #ffc107;--bs-green: #198754;--bs-teal: #20c997;--bs-cyan: #0dcaf0;--bs-black: #000;--bs-white: #fff;--bs-gray: #6c757d;--bs-gray-dark: #343a40;--bs-gray-100: #f8f9fa;--bs-gray-200: #e9ecef;--bs-gray-300: #dee2e6;--bs-gray-400: #ced4da;--bs-gray-500: #adb5bd;--bs-gray-600: #6c757d;--bs-gray-700: #495057;--bs-gray-800: #343a40;--bs-gray-900: #212529;--bs-default: #dee2e6;--bs-primary: #0d6efd;--bs-secondary: #6c757d;--bs-success: #198754;--bs-info: #0dcaf0;--bs-warning: #ffc107;--bs-danger: #dc3545;--bs-light: #f8f9fa;--bs-dark: #212529;--bs-default-rgb: 222,226,230;--bs-primary-rgb: 13,110,253;--bs-secondary-rgb: 108,117,125;--bs-success-rgb: 25,135,84;--bs-info-rgb: 13,202,240;--bs-warning-rgb: 255,193,7;--bs-danger-rgb: 220,53,69;--bs-light-rgb: 248,249,250;--bs-dark-rgb: 33,37,41;--bs-white-rgb: 255,255,255;--bs-black-rgb: 0,0,0;--bs-body-color-rgb: 33,37,41;--bs-body-bg-rgb: 255,255,255;--bs-font-sans-serif: system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", "Noto Sans", "Liberation Sans", Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";--bs-font-monospace: SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;--bs-gradient: linear-gradient(180deg, rgba(255,255,255,0.15), rgba(255,255,255,0));--bs-body-font-family: var(--bs-font-sans-serif);--bs-body-font-size:1rem;--bs-body-font-weight: 400;--bs-body-line-height: 1.5;--bs-body-color: #212529;--bs-body-bg: #fff;--bs-border-width: 1px;--bs-border-style: solid;--bs-border-color: #dee2e6;--bs-border-color-translucent: rgba(0,0,0,0.175);--bs-border-radius: .375rem;--bs-border-radius-sm: .25rem;--bs-border-radius-lg: .5rem;--bs-border-radius-xl: 1rem;--bs-border-radius-2xl: 2rem;--bs-border-radius-pill: 50rem;--bs-link-color: #0d6efd;--bs-link-hover-color: #0a58ca;--bs-code-color: #000;--bs-highlight-bg: #fff3cd}*,*::before,*::after{box-sizing:border-box}@media (prefers-reduced-motion: no-preference){:root{scroll-behavior:smooth}}body{margin:0;font-family:var(--bs-body-font-family);font-size:var(--bs-body-font-size);font-weight:var(--bs-body-font-weight);line-height:var(--bs-body-line-height);color:var(--bs-body-color);text-align:var(--bs-body-text-align);background-color:var(--bs-body-bg);-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:rgba(0,0,0,0)}hr{margin:1rem 0;color:inherit;border:0;border-top:1px solid;opacity:.25}h6,.h6,.bslib-value-box .value-box-area>:first-child,h5,.h5,h4,.h4,h3,.h3,h2,.h2,.bslib-value-box .value-box-area>:nth-child(2),h1,.h1{margin-top:0;margin-bottom:.5rem;font-weight:500;line-height:1.2}h1,.h1{font-size:calc(1.375rem + 1.5vw)}@media (min-width: 1200px){h1,.h1{font-size:2.5rem}}h2,.h2,.bslib-value-box .value-box-area>:nth-child(2){font-size:calc(1.325rem + .9vw)}@media (min-width: 1200px){h2,.h2,.bslib-value-box .value-box-area>:nth-child(2){font-size:2rem}}h3,.h3{font-size:calc(1.3rem + .6vw)}@media (min-width: 1200px){h3,.h3{font-size:1.75rem}}h4,.h4{font-size:calc(1.275rem + .3vw)}@media (min-width: 1200px){h4,.h4{font-size:1.5rem}}h5,.h5{font-size:1.25rem}h6,.h6,.bslib-value-box .value-box-area>:first-child{font-size:1rem}p{margin-top:0;margin-bottom:1rem}abbr[title]{text-decoration:underline dotted;-webkit-text-decoration:underline dotted;-moz-text-decoration:underline dotted;-ms-text-decoration:underline dotted;-o-text-decoration:underline dotted;cursor:help;text-decoration-skip-ink:none}address{margin-bottom:1rem;font-style:normal;line-height:inherit}ol,ul{padding-left:2rem}ol,ul,dl{margin-top:0;margin-bottom:1rem}ol ol,ul ul,ol ul,ul ol{margin-bottom:0}dt{font-weight:700}dd{margin-bottom:.5rem;margin-left:0}blockquote{margin:0 0 1rem;padding:.625rem 1.25rem;border-left:.25rem solid #e9ecef}blockquote p:last-child,blockquote ul:last-child,blockquote ol:last-child{margin-bottom:0}b,strong{font-weight:bolder}small,.small{font-size:.875em}mark,.mark{padding:.1875em;background-color:var(--bs-highlight-bg)}sub,sup{position:relative;font-size:.75em;line-height:0;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}a{color:var(--bs-link-color);text-decoration:underline;-webkit-text-decoration:underline;-moz-text-decoration:underline;-ms-text-decoration:underline;-o-text-decoration:underline}a:hover{color:var(--bs-link-hover-color)}a:not([href]):not([class]),a:not([href]):not([class]):hover{color:inherit;text-decoration:none}pre,code,kbd,samp{font-family:var(--bs-font-monospace);font-size:1em}pre{display:block;margin-top:0;margin-bottom:1rem;overflow:auto;font-size:.875em;color:#000;background-color:#f6f6f6;padding:.5rem;border:1px solid #dee2e6;border-radius:.375rem}pre code{background-color:transparent;font-size:inherit;color:inherit;word-break:normal}code{font-size:.875em;color:var(--bs-code-color);background-color:#f6f6f6;border-radius:.375rem;padding:.125rem .25rem;word-wrap:break-word}a>code{color:inherit}kbd{padding:.1875rem .375rem;font-size:.875em;color:var(--bs-body-bg);background-color:var(--bs-body-color);border-radius:.25rem}kbd kbd{padding:0;font-size:1em}figure{margin:0 0 1rem}img,svg{vertical-align:middle}table{caption-side:bottom;border-collapse:collapse}caption{padding-top:.5rem;padding-bottom:.5rem;color:#6c757d;text-align:left}th{text-align:inherit;text-align:-webkit-match-parent}thead,tbody,tfoot,tr,td,th{border-color:inherit;border-style:solid;border-width:0}label{display:inline-block}button{border-radius:0}button:focus:not(:focus-visible){outline:0}input,button,select,optgroup,textarea{margin:0;font-family:inherit;font-size:inherit;line-height:inherit}button,select{text-transform:none}[role="button"]{cursor:pointer}select{word-wrap:normal}select:disabled{opacity:1}[list]:not([type="date"]):not([type="datetime-local"]):not([type="month"]):not([type="week"]):not([type="time"])::-webkit-calendar-picker-indicator{display:none !important}button,[type="button"],[type="reset"],[type="submit"]{-webkit-appearance:button}button:not(:disabled),[type="button"]:not(:disabled),[type="reset"]:not(:disabled),[type="submit"]:not(:disabled){cursor:pointer}::-moz-focus-inner{padding:0;border-style:none}textarea{resize:vertical}fieldset{min-width:0;padding:0;margin:0;border:0}legend{float:left;width:100%;padding:0;margin-bottom:.5rem;font-size:calc(1.275rem + .3vw);line-height:inherit}@media (min-width: 1200px){legend{font-size:1.5rem}}legend+*{clear:left}::-webkit-datetime-edit-fields-wrapper,::-webkit-datetime-edit-text,::-webkit-datetime-edit-minute,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-year-field{padding:0}::-webkit-inner-spin-button{height:auto}[type="search"]{outline-offset:-2px;-webkit-appearance:textfield}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-color-swatch-wrapper{padding:0}::file-selector-button{font:inherit;-webkit-appearance:button}output{display:inline-block}iframe{border:0}summary{display:list-item;cursor:pointer}progress{vertical-align:baseline}[hidden]{display:none !important}.lead{font-size:1.25rem;font-weight:300}.display-1{font-size:calc(1.625rem + 4.5vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-1{font-size:5rem}}.display-2{font-size:calc(1.575rem + 3.9vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-2{font-size:4.5rem}}.display-3{font-size:calc(1.525rem + 3.3vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-3{font-size:4rem}}.display-4{font-size:calc(1.475rem + 2.7vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-4{font-size:3.5rem}}.display-5{font-size:calc(1.425rem + 2.1vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-5{font-size:3rem}}.display-6{font-size:calc(1.375rem + 1.5vw);font-weight:300;line-height:1.2}@media (min-width: 1200px){.display-6{font-size:2.5rem}}.list-unstyled{padding-left:0;list-style:none}.list-inline{padding-left:0;list-style:none}.list-inline-item{display:inline-block}.list-inline-item:not(:last-child){margin-right:.5rem}.initialism{font-size:.875em;text-transform:uppercase}.blockquote{margin-bottom:1rem;font-size:1.25rem}.blockquote>:last-child{margin-bottom:0}.blockquote-footer{margin-top:-1rem;margin-bottom:1rem;font-size:.875em;color:#6c757d}.blockquote-footer::before{content:"\2014\00A0"}.img-fluid{max-width:100%;height:auto}.img-thumbnail{padding:.25rem;background-color:#fff;border:1px solid var(--bs-border-color);border-radius:.375rem;max-width:100%;height:auto}.figure{display:inline-block}.figure-img{margin-bottom:.5rem;line-height:1}.figure-caption{font-size:.875em;color:#6c757d}.container,.container-fluid,.container-xxl,.container-xl,.container-lg,.container-md,.container-sm{--bs-gutter-x: 1.5rem;--bs-gutter-y: 0;width:100%;padding-right:calc(var(--bs-gutter-x) * .5);padding-left:calc(var(--bs-gutter-x) * .5);margin-right:auto;margin-left:auto}@media (min-width: 576px){.container-sm,.container{max-width:540px}}@media (min-width: 768px){.container-md,.container-sm,.container{max-width:720px}}@media (min-width: 992px){.container-lg,.container-md,.container-sm,.container{max-width:960px}}@media (min-width: 1200px){.container-xl,.container-lg,.container-md,.container-sm,.container{max-width:1140px}}@media (min-width: 1400px){.container-xxl,.container-xl,.container-lg,.container-md,.container-sm,.container{max-width:1320px}}.row{--bs-gutter-x: 1.5rem;--bs-gutter-y: 0;display:flex;display:-webkit-flex;flex-wrap:wrap;-webkit-flex-wrap:wrap;margin-top:calc(-1 * var(--bs-gutter-y));margin-right:calc(-.5 * var(--bs-gutter-x));margin-left:calc(-.5 * var(--bs-gutter-x))}.row>*{flex-shrink:0;-webkit-flex-shrink:0;width:100%;max-width:100%;padding-right:calc(var(--bs-gutter-x) * .5);padding-left:calc(var(--bs-gutter-x) * .5);margin-top:var(--bs-gutter-y)}.grid{display:grid;grid-template-rows:repeat(var(--bs-rows, 1), 1fr);grid-template-columns:repeat(var(--bs-columns, 12), 1fr);gap:var(--bs-gap, 1.5rem)}.grid .g-col-1{grid-column:auto/span 1}.grid .g-col-2{grid-column:auto/span 2}.grid .g-col-3{grid-column:auto/span 3}.grid .g-col-4{grid-column:auto/span 4}.grid .g-col-5{grid-column:auto/span 5}.grid .g-col-6{grid-column:auto/span 6}.grid .g-col-7{grid-column:auto/span 7}.grid .g-col-8{grid-column:auto/span 8}.grid .g-col-9{grid-column:auto/span 9}.grid .g-col-10{grid-column:auto/span 10}.grid .g-col-11{grid-column:auto/span 11}.grid .g-col-12{grid-column:auto/span 12}.grid .g-start-1{grid-column-start:1}.grid .g-start-2{grid-column-start:2}.grid .g-start-3{grid-column-start:3}.grid .g-start-4{grid-column-start:4}.grid .g-start-5{grid-column-start:5}.grid .g-start-6{grid-column-start:6}.grid .g-start-7{grid-column-start:7}.grid .g-start-8{grid-column-start:8}.grid .g-start-9{grid-column-start:9}.grid .g-start-10{grid-column-start:10}.grid .g-start-11{grid-column-start:11}@media (min-width: 576px){.grid .g-col-sm-1{grid-column:auto/span 1}.grid .g-col-sm-2{grid-column:auto/span 2}.grid .g-col-sm-3{grid-column:auto/span 3}.grid .g-col-sm-4{grid-column:auto/span 4}.grid .g-col-sm-5{grid-column:auto/span 5}.grid .g-col-sm-6{grid-column:auto/span 6}.grid .g-col-sm-7{grid-column:auto/span 7}.grid .g-col-sm-8{grid-column:auto/span 8}.grid .g-col-sm-9{grid-column:auto/span 9}.grid .g-col-sm-10{grid-column:auto/span 10}.grid .g-col-sm-11{grid-column:auto/span 11}.grid .g-col-sm-12{grid-column:auto/span 12}.grid .g-start-sm-1{grid-column-start:1}.grid .g-start-sm-2{grid-column-start:2}.grid .g-start-sm-3{grid-column-start:3}.grid .g-start-sm-4{grid-column-start:4}.grid .g-start-sm-5{grid-column-start:5}.grid .g-start-sm-6{grid-column-start:6}.grid .g-start-sm-7{grid-column-start:7}.grid .g-start-sm-8{grid-column-start:8}.grid .g-start-sm-9{grid-column-start:9}.grid .g-start-sm-10{grid-column-start:10}.grid .g-start-sm-11{grid-column-start:11}}@media (min-width: 768px){.grid .g-col-md-1{grid-column:auto/span 1}.grid .g-col-md-2{grid-column:auto/span 2}.grid .g-col-md-3{grid-column:auto/span 3}.grid .g-col-md-4{grid-column:auto/span 4}.grid .g-col-md-5{grid-column:auto/span 5}.grid .g-col-md-6{grid-column:auto/span 6}.grid .g-col-md-7{grid-column:auto/span 7}.grid .g-col-md-8{grid-column:auto/span 8}.grid .g-col-md-9{grid-column:auto/span 9}.grid .g-col-md-10{grid-column:auto/span 10}.grid .g-col-md-11{grid-column:auto/span 11}.grid .g-col-md-12{grid-column:auto/span 12}.grid .g-start-md-1{grid-column-start:1}.grid .g-start-md-2{grid-column-start:2}.grid .g-start-md-3{grid-column-start:3}.grid .g-start-md-4{grid-column-start:4}.grid .g-start-md-5{grid-column-start:5}.grid .g-start-md-6{grid-column-start:6}.grid .g-start-md-7{grid-column-start:7}.grid .g-start-md-8{grid-column-start:8}.grid .g-start-md-9{grid-column-start:9}.grid .g-start-md-10{grid-column-start:10}.grid .g-start-md-11{grid-column-start:11}}@media (min-width: 992px){.grid .g-col-lg-1{grid-column:auto/span 1}.grid .g-col-lg-2{grid-column:auto/span 2}.grid .g-col-lg-3{grid-column:auto/span 3}.grid .g-col-lg-4{grid-column:auto/span 4}.grid .g-col-lg-5{grid-column:auto/span 5}.grid .g-col-lg-6{grid-column:auto/span 6}.grid .g-col-lg-7{grid-column:auto/span 7}.grid .g-col-lg-8{grid-column:auto/span 8}.grid .g-col-lg-9{grid-column:auto/span 9}.grid .g-col-lg-10{grid-column:auto/span 10}.grid .g-col-lg-11{grid-column:auto/span 11}.grid .g-col-lg-12{grid-column:auto/span 12}.grid .g-start-lg-1{grid-column-start:1}.grid .g-start-lg-2{grid-column-start:2}.grid .g-start-lg-3{grid-column-start:3}.grid .g-start-lg-4{grid-column-start:4}.grid .g-start-lg-5{grid-column-start:5}.grid .g-start-lg-6{grid-column-start:6}.grid .g-start-lg-7{grid-column-start:7}.grid .g-start-lg-8{grid-column-start:8}.grid .g-start-lg-9{grid-column-start:9}.grid .g-start-lg-10{grid-column-start:10}.grid .g-start-lg-11{grid-column-start:11}}@media (min-width: 1200px){.grid .g-col-xl-1{grid-column:auto/span 1}.grid .g-col-xl-2{grid-column:auto/span 2}.grid .g-col-xl-3{grid-column:auto/span 3}.grid .g-col-xl-4{grid-column:auto/span 4}.grid .g-col-xl-5{grid-column:auto/span 5}.grid .g-col-xl-6{grid-column:auto/span 6}.grid .g-col-xl-7{grid-column:auto/span 7}.grid .g-col-xl-8{grid-column:auto/span 8}.grid .g-col-xl-9{grid-column:auto/span 9}.grid .g-col-xl-10{grid-column:auto/span 10}.grid .g-col-xl-11{grid-column:auto/span 11}.grid .g-col-xl-12{grid-column:auto/span 12}.grid .g-start-xl-1{grid-column-start:1}.grid .g-start-xl-2{grid-column-start:2}.grid .g-start-xl-3{grid-column-start:3}.grid .g-start-xl-4{grid-column-start:4}.grid .g-start-xl-5{grid-column-start:5}.grid .g-start-xl-6{grid-column-start:6}.grid .g-start-xl-7{grid-column-start:7}.grid .g-start-xl-8{grid-column-start:8}.grid .g-start-xl-9{grid-column-start:9}.grid .g-start-xl-10{grid-column-start:10}.grid .g-start-xl-11{grid-column-start:11}}@media (min-width: 1400px){.grid .g-col-xxl-1{grid-column:auto/span 1}.grid .g-col-xxl-2{grid-column:auto/span 2}.grid .g-col-xxl-3{grid-column:auto/span 3}.grid .g-col-xxl-4{grid-column:auto/span 4}.grid .g-col-xxl-5{grid-column:auto/span 5}.grid .g-col-xxl-6{grid-column:auto/span 6}.grid .g-col-xxl-7{grid-column:auto/span 7}.grid .g-col-xxl-8{grid-column:auto/span 8}.grid .g-col-xxl-9{grid-column:auto/span 9}.grid .g-col-xxl-10{grid-column:auto/span 10}.grid .g-col-xxl-11{grid-column:auto/span 11}.grid .g-col-xxl-12{grid-column:auto/span 12}.grid .g-start-xxl-1{grid-column-start:1}.grid .g-start-xxl-2{grid-column-start:2}.grid .g-start-xxl-3{grid-column-start:3}.grid .g-start-xxl-4{grid-column-start:4}.grid .g-start-xxl-5{grid-column-start:5}.grid .g-start-xxl-6{grid-column-start:6}.grid .g-start-xxl-7{grid-column-start:7}.grid .g-start-xxl-8{grid-column-start:8}.grid .g-start-xxl-9{grid-column-start:9}.grid .g-start-xxl-10{grid-column-start:10}.grid .g-start-xxl-11{grid-column-start:11}}.col{flex:1 0 0%;-webkit-flex:1 0 0%}.row-cols-auto>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.row-cols-1>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.row-cols-2>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.row-cols-3>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.row-cols-4>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.row-cols-5>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:20%}.row-cols-6>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-auto{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.col-1{flex:0 0 auto;-webkit-flex:0 0 auto;width:8.33333%}.col-2{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-3{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.col-4{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.col-5{flex:0 0 auto;-webkit-flex:0 0 auto;width:41.66667%}.col-6{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.col-7{flex:0 0 auto;-webkit-flex:0 0 auto;width:58.33333%}.col-8{flex:0 0 auto;-webkit-flex:0 0 auto;width:66.66667%}.col-9{flex:0 0 auto;-webkit-flex:0 0 auto;width:75%}.col-10{flex:0 0 auto;-webkit-flex:0 0 auto;width:83.33333%}.col-11{flex:0 0 auto;-webkit-flex:0 0 auto;width:91.66667%}.col-12{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.offset-1{margin-left:8.33333%}.offset-2{margin-left:16.66667%}.offset-3{margin-left:25%}.offset-4{margin-left:33.33333%}.offset-5{margin-left:41.66667%}.offset-6{margin-left:50%}.offset-7{margin-left:58.33333%}.offset-8{margin-left:66.66667%}.offset-9{margin-left:75%}.offset-10{margin-left:83.33333%}.offset-11{margin-left:91.66667%}.g-0,.gx-0{--bs-gutter-x: 0}.g-0,.gy-0{--bs-gutter-y: 0}.g-1,.gx-1{--bs-gutter-x: .25rem}.g-1,.gy-1{--bs-gutter-y: .25rem}.g-2,.gx-2{--bs-gutter-x: .5rem}.g-2,.gy-2{--bs-gutter-y: .5rem}.g-3,.gx-3{--bs-gutter-x: 1rem}.g-3,.gy-3{--bs-gutter-y: 1rem}.g-4,.gx-4{--bs-gutter-x: 1.5rem}.g-4,.gy-4{--bs-gutter-y: 1.5rem}.g-5,.gx-5{--bs-gutter-x: 3rem}.g-5,.gy-5{--bs-gutter-y: 3rem}@media (min-width: 576px){.col-sm{flex:1 0 0%;-webkit-flex:1 0 0%}.row-cols-sm-auto>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.row-cols-sm-1>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.row-cols-sm-2>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.row-cols-sm-3>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.row-cols-sm-4>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.row-cols-sm-5>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:20%}.row-cols-sm-6>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-sm-auto{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.col-sm-1{flex:0 0 auto;-webkit-flex:0 0 auto;width:8.33333%}.col-sm-2{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-sm-3{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.col-sm-4{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.col-sm-5{flex:0 0 auto;-webkit-flex:0 0 auto;width:41.66667%}.col-sm-6{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.col-sm-7{flex:0 0 auto;-webkit-flex:0 0 auto;width:58.33333%}.col-sm-8{flex:0 0 auto;-webkit-flex:0 0 auto;width:66.66667%}.col-sm-9{flex:0 0 auto;-webkit-flex:0 0 auto;width:75%}.col-sm-10{flex:0 0 auto;-webkit-flex:0 0 auto;width:83.33333%}.col-sm-11{flex:0 0 auto;-webkit-flex:0 0 auto;width:91.66667%}.col-sm-12{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.offset-sm-0{margin-left:0}.offset-sm-1{margin-left:8.33333%}.offset-sm-2{margin-left:16.66667%}.offset-sm-3{margin-left:25%}.offset-sm-4{margin-left:33.33333%}.offset-sm-5{margin-left:41.66667%}.offset-sm-6{margin-left:50%}.offset-sm-7{margin-left:58.33333%}.offset-sm-8{margin-left:66.66667%}.offset-sm-9{margin-left:75%}.offset-sm-10{margin-left:83.33333%}.offset-sm-11{margin-left:91.66667%}.g-sm-0,.gx-sm-0{--bs-gutter-x: 0}.g-sm-0,.gy-sm-0{--bs-gutter-y: 0}.g-sm-1,.gx-sm-1{--bs-gutter-x: .25rem}.g-sm-1,.gy-sm-1{--bs-gutter-y: .25rem}.g-sm-2,.gx-sm-2{--bs-gutter-x: .5rem}.g-sm-2,.gy-sm-2{--bs-gutter-y: .5rem}.g-sm-3,.gx-sm-3{--bs-gutter-x: 1rem}.g-sm-3,.gy-sm-3{--bs-gutter-y: 1rem}.g-sm-4,.gx-sm-4{--bs-gutter-x: 1.5rem}.g-sm-4,.gy-sm-4{--bs-gutter-y: 1.5rem}.g-sm-5,.gx-sm-5{--bs-gutter-x: 3rem}.g-sm-5,.gy-sm-5{--bs-gutter-y: 3rem}}@media (min-width: 768px){.col-md{flex:1 0 0%;-webkit-flex:1 0 0%}.row-cols-md-auto>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.row-cols-md-1>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.row-cols-md-2>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.row-cols-md-3>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.row-cols-md-4>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.row-cols-md-5>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:20%}.row-cols-md-6>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-md-auto{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.col-md-1{flex:0 0 auto;-webkit-flex:0 0 auto;width:8.33333%}.col-md-2{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-md-3{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.col-md-4{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.col-md-5{flex:0 0 auto;-webkit-flex:0 0 auto;width:41.66667%}.col-md-6{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.col-md-7{flex:0 0 auto;-webkit-flex:0 0 auto;width:58.33333%}.col-md-8{flex:0 0 auto;-webkit-flex:0 0 auto;width:66.66667%}.col-md-9{flex:0 0 auto;-webkit-flex:0 0 auto;width:75%}.col-md-10{flex:0 0 auto;-webkit-flex:0 0 auto;width:83.33333%}.col-md-11{flex:0 0 auto;-webkit-flex:0 0 auto;width:91.66667%}.col-md-12{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.offset-md-0{margin-left:0}.offset-md-1{margin-left:8.33333%}.offset-md-2{margin-left:16.66667%}.offset-md-3{margin-left:25%}.offset-md-4{margin-left:33.33333%}.offset-md-5{margin-left:41.66667%}.offset-md-6{margin-left:50%}.offset-md-7{margin-left:58.33333%}.offset-md-8{margin-left:66.66667%}.offset-md-9{margin-left:75%}.offset-md-10{margin-left:83.33333%}.offset-md-11{margin-left:91.66667%}.g-md-0,.gx-md-0{--bs-gutter-x: 0}.g-md-0,.gy-md-0{--bs-gutter-y: 0}.g-md-1,.gx-md-1{--bs-gutter-x: .25rem}.g-md-1,.gy-md-1{--bs-gutter-y: .25rem}.g-md-2,.gx-md-2{--bs-gutter-x: .5rem}.g-md-2,.gy-md-2{--bs-gutter-y: .5rem}.g-md-3,.gx-md-3{--bs-gutter-x: 1rem}.g-md-3,.gy-md-3{--bs-gutter-y: 1rem}.g-md-4,.gx-md-4{--bs-gutter-x: 1.5rem}.g-md-4,.gy-md-4{--bs-gutter-y: 1.5rem}.g-md-5,.gx-md-5{--bs-gutter-x: 3rem}.g-md-5,.gy-md-5{--bs-gutter-y: 3rem}}@media (min-width: 992px){.col-lg{flex:1 0 0%;-webkit-flex:1 0 0%}.row-cols-lg-auto>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.row-cols-lg-1>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.row-cols-lg-2>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.row-cols-lg-3>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.row-cols-lg-4>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.row-cols-lg-5>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:20%}.row-cols-lg-6>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-lg-auto{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.col-lg-1{flex:0 0 auto;-webkit-flex:0 0 auto;width:8.33333%}.col-lg-2{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-lg-3{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.col-lg-4{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.col-lg-5{flex:0 0 auto;-webkit-flex:0 0 auto;width:41.66667%}.col-lg-6{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.col-lg-7{flex:0 0 auto;-webkit-flex:0 0 auto;width:58.33333%}.col-lg-8{flex:0 0 auto;-webkit-flex:0 0 auto;width:66.66667%}.col-lg-9{flex:0 0 auto;-webkit-flex:0 0 auto;width:75%}.col-lg-10{flex:0 0 auto;-webkit-flex:0 0 auto;width:83.33333%}.col-lg-11{flex:0 0 auto;-webkit-flex:0 0 auto;width:91.66667%}.col-lg-12{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.offset-lg-0{margin-left:0}.offset-lg-1{margin-left:8.33333%}.offset-lg-2{margin-left:16.66667%}.offset-lg-3{margin-left:25%}.offset-lg-4{margin-left:33.33333%}.offset-lg-5{margin-left:41.66667%}.offset-lg-6{margin-left:50%}.offset-lg-7{margin-left:58.33333%}.offset-lg-8{margin-left:66.66667%}.offset-lg-9{margin-left:75%}.offset-lg-10{margin-left:83.33333%}.offset-lg-11{margin-left:91.66667%}.g-lg-0,.gx-lg-0{--bs-gutter-x: 0}.g-lg-0,.gy-lg-0{--bs-gutter-y: 0}.g-lg-1,.gx-lg-1{--bs-gutter-x: .25rem}.g-lg-1,.gy-lg-1{--bs-gutter-y: .25rem}.g-lg-2,.gx-lg-2{--bs-gutter-x: .5rem}.g-lg-2,.gy-lg-2{--bs-gutter-y: .5rem}.g-lg-3,.gx-lg-3{--bs-gutter-x: 1rem}.g-lg-3,.gy-lg-3{--bs-gutter-y: 1rem}.g-lg-4,.gx-lg-4{--bs-gutter-x: 1.5rem}.g-lg-4,.gy-lg-4{--bs-gutter-y: 1.5rem}.g-lg-5,.gx-lg-5{--bs-gutter-x: 3rem}.g-lg-5,.gy-lg-5{--bs-gutter-y: 3rem}}@media (min-width: 1200px){.col-xl{flex:1 0 0%;-webkit-flex:1 0 0%}.row-cols-xl-auto>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.row-cols-xl-1>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.row-cols-xl-2>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.row-cols-xl-3>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.row-cols-xl-4>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.row-cols-xl-5>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:20%}.row-cols-xl-6>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-xl-auto{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.col-xl-1{flex:0 0 auto;-webkit-flex:0 0 auto;width:8.33333%}.col-xl-2{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-xl-3{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.col-xl-4{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.col-xl-5{flex:0 0 auto;-webkit-flex:0 0 auto;width:41.66667%}.col-xl-6{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.col-xl-7{flex:0 0 auto;-webkit-flex:0 0 auto;width:58.33333%}.col-xl-8{flex:0 0 auto;-webkit-flex:0 0 auto;width:66.66667%}.col-xl-9{flex:0 0 auto;-webkit-flex:0 0 auto;width:75%}.col-xl-10{flex:0 0 auto;-webkit-flex:0 0 auto;width:83.33333%}.col-xl-11{flex:0 0 auto;-webkit-flex:0 0 auto;width:91.66667%}.col-xl-12{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.offset-xl-0{margin-left:0}.offset-xl-1{margin-left:8.33333%}.offset-xl-2{margin-left:16.66667%}.offset-xl-3{margin-left:25%}.offset-xl-4{margin-left:33.33333%}.offset-xl-5{margin-left:41.66667%}.offset-xl-6{margin-left:50%}.offset-xl-7{margin-left:58.33333%}.offset-xl-8{margin-left:66.66667%}.offset-xl-9{margin-left:75%}.offset-xl-10{margin-left:83.33333%}.offset-xl-11{margin-left:91.66667%}.g-xl-0,.gx-xl-0{--bs-gutter-x: 0}.g-xl-0,.gy-xl-0{--bs-gutter-y: 0}.g-xl-1,.gx-xl-1{--bs-gutter-x: .25rem}.g-xl-1,.gy-xl-1{--bs-gutter-y: .25rem}.g-xl-2,.gx-xl-2{--bs-gutter-x: .5rem}.g-xl-2,.gy-xl-2{--bs-gutter-y: .5rem}.g-xl-3,.gx-xl-3{--bs-gutter-x: 1rem}.g-xl-3,.gy-xl-3{--bs-gutter-y: 1rem}.g-xl-4,.gx-xl-4{--bs-gutter-x: 1.5rem}.g-xl-4,.gy-xl-4{--bs-gutter-y: 1.5rem}.g-xl-5,.gx-xl-5{--bs-gutter-x: 3rem}.g-xl-5,.gy-xl-5{--bs-gutter-y: 3rem}}@media (min-width: 1400px){.col-xxl{flex:1 0 0%;-webkit-flex:1 0 0%}.row-cols-xxl-auto>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.row-cols-xxl-1>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.row-cols-xxl-2>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.row-cols-xxl-3>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.row-cols-xxl-4>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.row-cols-xxl-5>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:20%}.row-cols-xxl-6>*{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-xxl-auto{flex:0 0 auto;-webkit-flex:0 0 auto;width:auto}.col-xxl-1{flex:0 0 auto;-webkit-flex:0 0 auto;width:8.33333%}.col-xxl-2{flex:0 0 auto;-webkit-flex:0 0 auto;width:16.66667%}.col-xxl-3{flex:0 0 auto;-webkit-flex:0 0 auto;width:25%}.col-xxl-4{flex:0 0 auto;-webkit-flex:0 0 auto;width:33.33333%}.col-xxl-5{flex:0 0 auto;-webkit-flex:0 0 auto;width:41.66667%}.col-xxl-6{flex:0 0 auto;-webkit-flex:0 0 auto;width:50%}.col-xxl-7{flex:0 0 auto;-webkit-flex:0 0 auto;width:58.33333%}.col-xxl-8{flex:0 0 auto;-webkit-flex:0 0 auto;width:66.66667%}.col-xxl-9{flex:0 0 auto;-webkit-flex:0 0 auto;width:75%}.col-xxl-10{flex:0 0 auto;-webkit-flex:0 0 auto;width:83.33333%}.col-xxl-11{flex:0 0 auto;-webkit-flex:0 0 auto;width:91.66667%}.col-xxl-12{flex:0 0 auto;-webkit-flex:0 0 auto;width:100%}.offset-xxl-0{margin-left:0}.offset-xxl-1{margin-left:8.33333%}.offset-xxl-2{margin-left:16.66667%}.offset-xxl-3{margin-left:25%}.offset-xxl-4{margin-left:33.33333%}.offset-xxl-5{margin-left:41.66667%}.offset-xxl-6{margin-left:50%}.offset-xxl-7{margin-left:58.33333%}.offset-xxl-8{margin-left:66.66667%}.offset-xxl-9{margin-left:75%}.offset-xxl-10{margin-left:83.33333%}.offset-xxl-11{margin-left:91.66667%}.g-xxl-0,.gx-xxl-0{--bs-gutter-x: 0}.g-xxl-0,.gy-xxl-0{--bs-gutter-y: 0}.g-xxl-1,.gx-xxl-1{--bs-gutter-x: .25rem}.g-xxl-1,.gy-xxl-1{--bs-gutter-y: .25rem}.g-xxl-2,.gx-xxl-2{--bs-gutter-x: .5rem}.g-xxl-2,.gy-xxl-2{--bs-gutter-y: .5rem}.g-xxl-3,.gx-xxl-3{--bs-gutter-x: 1rem}.g-xxl-3,.gy-xxl-3{--bs-gutter-y: 1rem}.g-xxl-4,.gx-xxl-4{--bs-gutter-x: 1.5rem}.g-xxl-4,.gy-xxl-4{--bs-gutter-y: 1.5rem}.g-xxl-5,.gx-xxl-5{--bs-gutter-x: 3rem}.g-xxl-5,.gy-xxl-5{--bs-gutter-y: 3rem}}.table{--bs-table-color: var(--bs-body-color);--bs-table-bg: rgba(0,0,0,0);--bs-table-border-color: var(--bs-border-color);--bs-table-accent-bg: rgba(0,0,0,0);--bs-table-striped-color: var(--bs-body-color);--bs-table-striped-bg: rgba(0,0,0,0.05);--bs-table-active-color: var(--bs-body-color);--bs-table-active-bg: rgba(0,0,0,0.1);--bs-table-hover-color: var(--bs-body-color);--bs-table-hover-bg: rgba(0,0,0,0.075);width:100%;margin-bottom:1rem;color:var(--bs-table-color);vertical-align:top;border-color:var(--bs-table-border-color)}.table>:not(caption)>*>*{padding:.5rem .5rem;background-color:var(--bs-table-bg);border-bottom-width:1px;box-shadow:inset 0 0 0 9999px var(--bs-table-accent-bg)}.table>tbody{vertical-align:inherit}.table>thead{vertical-align:bottom}.table-group-divider{border-top:2px solid currentcolor}.caption-top{caption-side:top}.table-sm>:not(caption)>*>*{padding:.25rem .25rem}.table-bordered>:not(caption)>*{border-width:1px 0}.table-bordered>:not(caption)>*>*{border-width:0 1px}.table-borderless>:not(caption)>*>*{border-bottom-width:0}.table-borderless>:not(:first-child){border-top-width:0}.table-striped>tbody>tr:nth-of-type(odd)>*{--bs-table-accent-bg: var(--bs-table-striped-bg);color:var(--bs-table-striped-color)}.table-striped-columns>:not(caption)>tr>:nth-child(even){--bs-table-accent-bg: var(--bs-table-striped-bg);color:var(--bs-table-striped-color)}.table-active{--bs-table-accent-bg: var(--bs-table-active-bg);color:var(--bs-table-active-color)}.table-hover>tbody>tr:hover>*{--bs-table-accent-bg: var(--bs-table-hover-bg);color:var(--bs-table-hover-color)}.table-primary{--bs-table-color: #000;--bs-table-bg: #cfe2ff;--bs-table-border-color: #bacbe6;--bs-table-striped-bg: #c5d7f2;--bs-table-striped-color: #000;--bs-table-active-bg: #bacbe6;--bs-table-active-color: #000;--bs-table-hover-bg: #bfd1ec;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-secondary{--bs-table-color: #000;--bs-table-bg: #e2e3e5;--bs-table-border-color: #cbccce;--bs-table-striped-bg: #d7d8da;--bs-table-striped-color: #000;--bs-table-active-bg: #cbccce;--bs-table-active-color: #000;--bs-table-hover-bg: #d1d2d4;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-success{--bs-table-color: #000;--bs-table-bg: #d1e7dd;--bs-table-border-color: #bcd0c7;--bs-table-striped-bg: #c7dbd2;--bs-table-striped-color: #000;--bs-table-active-bg: #bcd0c7;--bs-table-active-color: #000;--bs-table-hover-bg: #c1d6cc;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-info{--bs-table-color: #000;--bs-table-bg: #cff4fc;--bs-table-border-color: #badce3;--bs-table-striped-bg: #c5e8ef;--bs-table-striped-color: #000;--bs-table-active-bg: #badce3;--bs-table-active-color: #000;--bs-table-hover-bg: #bfe2e9;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-warning{--bs-table-color: #000;--bs-table-bg: #fff3cd;--bs-table-border-color: #e6dbb9;--bs-table-striped-bg: #f2e7c3;--bs-table-striped-color: #000;--bs-table-active-bg: #e6dbb9;--bs-table-active-color: #000;--bs-table-hover-bg: #ece1be;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-danger{--bs-table-color: #000;--bs-table-bg: #f8d7da;--bs-table-border-color: #dfc2c4;--bs-table-striped-bg: #eccccf;--bs-table-striped-color: #000;--bs-table-active-bg: #dfc2c4;--bs-table-active-color: #000;--bs-table-hover-bg: #e5c7ca;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-light{--bs-table-color: #000;--bs-table-bg: #f8f9fa;--bs-table-border-color: #dfe0e1;--bs-table-striped-bg: #ecedee;--bs-table-striped-color: #000;--bs-table-active-bg: #dfe0e1;--bs-table-active-color: #000;--bs-table-hover-bg: #e5e6e7;--bs-table-hover-color: #000;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-dark{--bs-table-color: #fff;--bs-table-bg: #212529;--bs-table-border-color: #373b3e;--bs-table-striped-bg: #2c3034;--bs-table-striped-color: #fff;--bs-table-active-bg: #373b3e;--bs-table-active-color: #fff;--bs-table-hover-bg: #323539;--bs-table-hover-color: #fff;color:var(--bs-table-color);border-color:var(--bs-table-border-color)}.table-responsive{overflow-x:auto;-webkit-overflow-scrolling:touch}@media (max-width: 575.98px){.table-responsive-sm{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 767.98px){.table-responsive-md{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 991.98px){.table-responsive-lg{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 1199.98px){.table-responsive-xl{overflow-x:auto;-webkit-overflow-scrolling:touch}}@media (max-width: 1399.98px){.table-responsive-xxl{overflow-x:auto;-webkit-overflow-scrolling:touch}}.form-label,.shiny-input-container .control-label{margin-bottom:.5rem}.col-form-label{padding-top:calc(.375rem + 1px);padding-bottom:calc(.375rem + 1px);margin-bottom:0;font-size:inherit;line-height:1.5}.col-form-label-lg{padding-top:calc(.5rem + 1px);padding-bottom:calc(.5rem + 1px);font-size:1.25rem}.col-form-label-sm{padding-top:calc(.25rem + 1px);padding-bottom:calc(.25rem + 1px);font-size:.875rem}.form-text,.help-text,.help-block{margin-top:.25rem;font-size:.875em;color:#6c757d}.form-control{display:block;width:100%;padding:.375rem .75rem;font-size:1rem;font-weight:400;line-height:1.5;color:#212529;background-color:#fff;background-clip:padding-box;border:1px solid #ced4da;appearance:none;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;-o-appearance:none;border-radius:.375rem;transition:border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-control{transition:none}}.form-control[type="file"]{overflow:hidden}.form-control[type="file"]:not(:disabled):not([readonly]){cursor:pointer}.form-control:focus{color:#212529;background-color:#fff;border-color:#86b7fe;outline:0;box-shadow:0 0 0 .25rem rgba(13,110,253,0.25)}.form-control::-webkit-date-and-time-value{height:1.5em}.form-control::placeholder{color:#6c757d;opacity:1}.form-control:disabled{background-color:#e9ecef;opacity:1}.form-control::file-selector-button{padding:.375rem .75rem;margin:-.375rem -.75rem;margin-inline-end:.75rem;color:#212529;background-color:#e9ecef;pointer-events:none;border-color:inherit;border-style:solid;border-width:0;border-inline-end-width:1px;border-radius:0;transition:color 0.15s ease-in-out,background-color 0.15s ease-in-out,border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-control::file-selector-button{transition:none}}.form-control:hover:not(:disabled):not([readonly])::file-selector-button{background-color:#dde0e3}.form-control-plaintext{display:block;width:100%;padding:.375rem 0;margin-bottom:0;line-height:1.5;color:#212529;background-color:transparent;border:solid transparent;border-width:1px 0}.form-control-plaintext:focus{outline:0}.form-control-plaintext.form-control-sm,.form-control-plaintext.form-control-lg{padding-right:0;padding-left:0}.form-control-sm{min-height:calc(1.5em + .5rem + 2px);padding:.25rem .5rem;font-size:.875rem;border-radius:.25rem}.form-control-sm::file-selector-button{padding:.25rem .5rem;margin:-.25rem -.5rem;margin-inline-end:.5rem}.form-control-lg{min-height:calc(1.5em + 1rem + 2px);padding:.5rem 1rem;font-size:1.25rem;border-radius:.5rem}.form-control-lg::file-selector-button{padding:.5rem 1rem;margin:-.5rem -1rem;margin-inline-end:1rem}textarea.form-control{min-height:calc(1.5em + .75rem + 2px)}textarea.form-control-sm{min-height:calc(1.5em + .5rem + 2px)}textarea.form-control-lg{min-height:calc(1.5em + 1rem + 2px)}.form-control-color{width:3rem;height:calc(1.5em + .75rem + 2px);padding:.375rem}.form-control-color:not(:disabled):not([readonly]){cursor:pointer}.form-control-color::-moz-color-swatch{border:0 !important;border-radius:.375rem}.form-control-color::-webkit-color-swatch{border-radius:.375rem}.form-control-color.form-control-sm{height:calc(1.5em + .5rem + 2px)}.form-control-color.form-control-lg{height:calc(1.5em + 1rem + 2px)}.form-select{display:block;width:100%;padding:.375rem 2.25rem .375rem .75rem;-moz-padding-start:calc(.75rem - 3px);font-size:1rem;font-weight:400;line-height:1.5;color:#212529;background-color:#fff;background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e");background-repeat:no-repeat;background-position:right .75rem center;background-size:16px 12px;border:1px solid #ced4da;border-radius:.375rem;transition:border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out;appearance:none;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;-o-appearance:none}@media (prefers-reduced-motion: reduce){.form-select{transition:none}}.form-select:focus{border-color:#86b7fe;outline:0;box-shadow:0 0 0 .25rem rgba(13,110,253,0.25)}.form-select[multiple],.form-select[size]:not([size="1"]){padding-right:.75rem;background-image:none}.form-select:disabled{background-color:#e9ecef}.form-select:-moz-focusring{color:transparent;text-shadow:0 0 0 #212529}.form-select-sm{padding-top:.25rem;padding-bottom:.25rem;padding-left:.5rem;font-size:.875rem;border-radius:.25rem}.form-select-lg{padding-top:.5rem;padding-bottom:.5rem;padding-left:1rem;font-size:1.25rem;border-radius:.5rem}.form-check,.shiny-input-container .checkbox,.shiny-input-container .radio{display:block;min-height:1.5rem;padding-left:0;margin-bottom:.125rem}.form-check .form-check-input,.form-check .shiny-input-container .checkbox input,.form-check .shiny-input-container .radio input,.shiny-input-container .checkbox .form-check-input,.shiny-input-container .checkbox .shiny-input-container .checkbox input,.shiny-input-container .checkbox .shiny-input-container .radio input,.shiny-input-container .radio .form-check-input,.shiny-input-container .radio .shiny-input-container .checkbox input,.shiny-input-container .radio .shiny-input-container .radio input{float:left;margin-left:0}.form-check-reverse{padding-right:0;padding-left:0;text-align:right}.form-check-reverse .form-check-input{float:right;margin-right:0;margin-left:0}.form-check-input,.shiny-input-container .checkbox input,.shiny-input-container .checkbox-inline input,.shiny-input-container .radio input,.shiny-input-container .radio-inline input{width:1em;height:1em;margin-top:.25em;vertical-align:top;background-color:#fff;background-repeat:no-repeat;background-position:center;background-size:contain;border:1px solid rgba(0,0,0,0.25);appearance:none;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;-o-appearance:none;print-color-adjust:exact}.form-check-input[type="checkbox"],.shiny-input-container .checkbox input[type="checkbox"],.shiny-input-container .checkbox-inline input[type="checkbox"],.shiny-input-container .radio input[type="checkbox"],.shiny-input-container .radio-inline input[type="checkbox"]{border-radius:.25em}.form-check-input[type="radio"],.shiny-input-container .checkbox input[type="radio"],.shiny-input-container .checkbox-inline input[type="radio"],.shiny-input-container .radio input[type="radio"],.shiny-input-container .radio-inline input[type="radio"]{border-radius:50%}.form-check-input:active,.shiny-input-container .checkbox input:active,.shiny-input-container .checkbox-inline input:active,.shiny-input-container .radio input:active,.shiny-input-container .radio-inline input:active{filter:brightness(90%)}.form-check-input:focus,.shiny-input-container .checkbox input:focus,.shiny-input-container .checkbox-inline input:focus,.shiny-input-container .radio input:focus,.shiny-input-container .radio-inline input:focus{border-color:#86b7fe;outline:0;box-shadow:0 0 0 .25rem rgba(13,110,253,0.25)}.form-check-input:checked,.shiny-input-container .checkbox input:checked,.shiny-input-container .checkbox-inline input:checked,.shiny-input-container .radio input:checked,.shiny-input-container .radio-inline input:checked{background-color:#0d6efd;border-color:#0d6efd}.form-check-input:checked[type="checkbox"],.shiny-input-container .checkbox input:checked[type="checkbox"],.shiny-input-container .checkbox-inline input:checked[type="checkbox"],.shiny-input-container .radio input:checked[type="checkbox"],.shiny-input-container .radio-inline input:checked[type="checkbox"]{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='m6 10 3 3 6-6'/%3e%3c/svg%3e")}.form-check-input:checked[type="radio"],.shiny-input-container .checkbox input:checked[type="radio"],.shiny-input-container .checkbox-inline input:checked[type="radio"],.shiny-input-container .radio input:checked[type="radio"],.shiny-input-container .radio-inline input:checked[type="radio"]{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='2' fill='%23fff'/%3e%3c/svg%3e")}.form-check-input[type="checkbox"]:indeterminate,.shiny-input-container .checkbox input[type="checkbox"]:indeterminate,.shiny-input-container .checkbox-inline input[type="checkbox"]:indeterminate,.shiny-input-container .radio input[type="checkbox"]:indeterminate,.shiny-input-container .radio-inline input[type="checkbox"]:indeterminate{background-color:#0d6efd;border-color:#0d6efd;background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='M6 10h8'/%3e%3c/svg%3e")}.form-check-input:disabled,.shiny-input-container .checkbox input:disabled,.shiny-input-container .checkbox-inline input:disabled,.shiny-input-container .radio input:disabled,.shiny-input-container .radio-inline input:disabled{pointer-events:none;filter:none;opacity:.5}.form-check-input[disabled]~.form-check-label,.form-check-input[disabled]~span,.form-check-input:disabled~.form-check-label,.form-check-input:disabled~span,.shiny-input-container .checkbox input[disabled]~.form-check-label,.shiny-input-container .checkbox input[disabled]~span,.shiny-input-container .checkbox input:disabled~.form-check-label,.shiny-input-container .checkbox input:disabled~span,.shiny-input-container .checkbox-inline input[disabled]~.form-check-label,.shiny-input-container .checkbox-inline input[disabled]~span,.shiny-input-container .checkbox-inline input:disabled~.form-check-label,.shiny-input-container .checkbox-inline input:disabled~span,.shiny-input-container .radio input[disabled]~.form-check-label,.shiny-input-container .radio input[disabled]~span,.shiny-input-container .radio input:disabled~.form-check-label,.shiny-input-container .radio input:disabled~span,.shiny-input-container .radio-inline input[disabled]~.form-check-label,.shiny-input-container .radio-inline input[disabled]~span,.shiny-input-container .radio-inline input:disabled~.form-check-label,.shiny-input-container .radio-inline input:disabled~span{cursor:default;opacity:.5}.form-check-label,.shiny-input-container .checkbox label,.shiny-input-container .checkbox-inline label,.shiny-input-container .radio label,.shiny-input-container .radio-inline label{cursor:pointer}.form-switch{padding-left:2.5em}.form-switch .form-check-input{width:2em;margin-left:-2.5em;background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='rgba%280,0,0,0.25%29'/%3e%3c/svg%3e");background-position:left center;border-radius:2em;transition:background-position 0.15s ease-in-out}@media (prefers-reduced-motion: reduce){.form-switch .form-check-input{transition:none}}.form-switch .form-check-input:focus{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%2386b7fe'/%3e%3c/svg%3e")}.form-switch .form-check-input:checked{background-position:right center;background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%23fff'/%3e%3c/svg%3e")}.form-switch.form-check-reverse{padding-right:2.5em;padding-left:0}.form-switch.form-check-reverse .form-check-input{margin-right:-2.5em;margin-left:0}.form-check-inline{display:inline-block;margin-right:1rem}.btn-check{position:absolute;clip:rect(0, 0, 0, 0);pointer-events:none}.btn-check[disabled]+.btn,.btn-check:disabled+.btn{pointer-events:none;filter:none;opacity:.65}.form-range{width:100%;height:1.5rem;padding:0;background-color:transparent;appearance:none;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;-o-appearance:none}.form-range:focus{outline:0}.form-range:focus::-webkit-slider-thumb{box-shadow:0 0 0 1px #fff,0 0 0 .25rem rgba(13,110,253,0.25)}.form-range:focus::-moz-range-thumb{box-shadow:0 0 0 1px #fff,0 0 0 .25rem rgba(13,110,253,0.25)}.form-range::-moz-focus-outer{border:0}.form-range::-webkit-slider-thumb{width:1rem;height:1rem;margin-top:-.25rem;background-color:#0d6efd;border:0;border-radius:1rem;transition:background-color 0.15s ease-in-out,border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out;appearance:none;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;-o-appearance:none}@media (prefers-reduced-motion: reduce){.form-range::-webkit-slider-thumb{transition:none}}.form-range::-webkit-slider-thumb:active{background-color:#b6d4fe}.form-range::-webkit-slider-runnable-track{width:100%;height:.5rem;color:transparent;cursor:pointer;background-color:#dee2e6;border-color:transparent;border-radius:1rem}.form-range::-moz-range-thumb{width:1rem;height:1rem;background-color:#0d6efd;border:0;border-radius:1rem;transition:background-color 0.15s ease-in-out,border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out;appearance:none;-webkit-appearance:none;-moz-appearance:none;-ms-appearance:none;-o-appearance:none}@media (prefers-reduced-motion: reduce){.form-range::-moz-range-thumb{transition:none}}.form-range::-moz-range-thumb:active{background-color:#b6d4fe}.form-range::-moz-range-track{width:100%;height:.5rem;color:transparent;cursor:pointer;background-color:#dee2e6;border-color:transparent;border-radius:1rem}.form-range:disabled{pointer-events:none}.form-range:disabled::-webkit-slider-thumb{background-color:#adb5bd}.form-range:disabled::-moz-range-thumb{background-color:#adb5bd}.form-floating{position:relative}.form-floating>.form-control,.form-floating>.form-control-plaintext,.form-floating>.form-select{height:calc(3.5rem + 2px);line-height:1.25}.form-floating>label{position:absolute;top:0;left:0;width:100%;height:100%;padding:1rem .75rem;overflow:hidden;text-align:start;text-overflow:ellipsis;white-space:nowrap;pointer-events:none;border:1px solid transparent;transform-origin:0 0;transition:opacity 0.1s ease-in-out,transform 0.1s ease-in-out}@media (prefers-reduced-motion: reduce){.form-floating>label{transition:none}}.form-floating>.form-control,.form-floating>.form-control-plaintext{padding:1rem .75rem}.form-floating>.form-control::placeholder,.form-floating>.form-control-plaintext::placeholder{color:transparent}.form-floating>.form-control:focus,.form-floating>.form-control:not(:placeholder-shown),.form-floating>.form-control-plaintext:focus,.form-floating>.form-control-plaintext:not(:placeholder-shown){padding-top:1.625rem;padding-bottom:.625rem}.form-floating>.form-control:-webkit-autofill,.form-floating>.form-control-plaintext:-webkit-autofill{padding-top:1.625rem;padding-bottom:.625rem}.form-floating>.form-select{padding-top:1.625rem;padding-bottom:.625rem}.form-floating>.form-control:focus~label,.form-floating>.form-control:not(:placeholder-shown)~label,.form-floating>.form-control-plaintext~label,.form-floating>.form-select~label{opacity:.65;transform:scale(0.85) translateY(-0.5rem) translateX(0.15rem)}.form-floating>.form-control:-webkit-autofill~label{opacity:.65;transform:scale(0.85) translateY(-0.5rem) translateX(0.15rem)}.form-floating>.form-control-plaintext~label{border-width:1px 0}.input-group{position:relative;display:flex;display:-webkit-flex;flex-wrap:wrap;-webkit-flex-wrap:wrap;align-items:stretch;-webkit-align-items:stretch;width:100%}.input-group>.form-control,.input-group>.form-select,.input-group>.form-floating{position:relative;flex:1 1 auto;-webkit-flex:1 1 auto;width:1%;min-width:0}.input-group>.form-control:focus,.input-group>.form-select:focus,.input-group>.form-floating:focus-within{z-index:5}.input-group .btn{position:relative;z-index:2}.input-group .btn:focus{z-index:5}.input-group-text{display:flex;display:-webkit-flex;align-items:center;-webkit-align-items:center;padding:.375rem .75rem;font-size:1rem;font-weight:400;line-height:1.5;color:#212529;text-align:center;white-space:nowrap;background-color:#e9ecef;border:1px solid #ced4da;border-radius:.375rem}.input-group-lg>.form-control,.input-group-lg>.form-select,.input-group-lg>.input-group-text,.input-group-lg>.btn{padding:.5rem 1rem;font-size:1.25rem;border-radius:.5rem}.input-group-sm>.form-control,.input-group-sm>.form-select,.input-group-sm>.input-group-text,.input-group-sm>.btn{padding:.25rem .5rem;font-size:.875rem;border-radius:.25rem}.input-group-lg>.form-select,.input-group-sm>.form-select{padding-right:3rem}.input-group:not(.has-validation)>:not(:last-child):not(.dropdown-toggle):not(.dropdown-menu):not(.form-floating),.input-group:not(.has-validation)>.dropdown-toggle:nth-last-child(n + 3),.input-group:not(.has-validation)>.form-floating:not(:last-child)>.form-control,.input-group:not(.has-validation)>.form-floating:not(:last-child)>.form-select{border-top-right-radius:0;border-bottom-right-radius:0}.input-group.has-validation>:nth-last-child(n + 3):not(.dropdown-toggle):not(.dropdown-menu):not(.form-floating),.input-group.has-validation>.dropdown-toggle:nth-last-child(n + 4),.input-group.has-validation>.form-floating:nth-last-child(n + 3)>.form-control,.input-group.has-validation>.form-floating:nth-last-child(n + 3)>.form-select{border-top-right-radius:0;border-bottom-right-radius:0}.input-group>:not(:first-child):not(.dropdown-menu):not(.valid-tooltip):not(.valid-feedback):not(.invalid-tooltip):not(.invalid-feedback){margin-left:-1px;border-top-left-radius:0;border-bottom-left-radius:0}.input-group>.form-floating:not(:first-child)>.form-control,.input-group>.form-floating:not(:first-child)>.form-select{border-top-left-radius:0;border-bottom-left-radius:0}.valid-feedback{display:none;width:100%;margin-top:.25rem;font-size:.875em;color:#198754}.valid-tooltip{position:absolute;top:100%;z-index:5;display:none;max-width:100%;padding:.25rem .5rem;margin-top:.1rem;font-size:.875rem;color:#fff;background-color:rgba(25,135,84,0.9);border-radius:.375rem}.was-validated :valid~.valid-feedback,.was-validated :valid~.valid-tooltip,.is-valid~.valid-feedback,.is-valid~.valid-tooltip{display:block}.was-validated .form-control:valid,.form-control.is-valid{border-color:#198754;padding-right:calc(1.5em + .75rem);background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");background-repeat:no-repeat;background-position:right calc(.375em + .1875rem) center;background-size:calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-control:valid:focus,.form-control.is-valid:focus{border-color:#198754;box-shadow:0 0 0 .25rem rgba(25,135,84,0.25)}.was-validated textarea.form-control:valid,textarea.form-control.is-valid{padding-right:calc(1.5em + .75rem);background-position:top calc(.375em + .1875rem) right calc(.375em + .1875rem)}.was-validated .form-select:valid,.form-select.is-valid{border-color:#198754}.was-validated .form-select:valid:not([multiple]):not([size]),.was-validated .form-select:valid:not([multiple])[size="1"],.form-select.is-valid:not([multiple]):not([size]),.form-select.is-valid:not([multiple])[size="1"]{padding-right:4.125rem;background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e"),url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");background-position:right .75rem center,center right 2.25rem;background-size:16px 12px,calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-select:valid:focus,.form-select.is-valid:focus{border-color:#198754;box-shadow:0 0 0 .25rem rgba(25,135,84,0.25)}.was-validated .form-control-color:valid,.form-control-color.is-valid{width:calc(3rem + calc(1.5em + .75rem))}.was-validated .form-check-input:valid,.form-check-input.is-valid{border-color:#198754}.was-validated .form-check-input:valid:checked,.form-check-input.is-valid:checked{background-color:#198754}.was-validated .form-check-input:valid:focus,.form-check-input.is-valid:focus{box-shadow:0 0 0 .25rem rgba(25,135,84,0.25)}.was-validated .form-check-input:valid~.form-check-label,.form-check-input.is-valid~.form-check-label{color:#198754}.form-check-inline .form-check-input~.valid-feedback{margin-left:.5em}.was-validated .input-group>.form-control:not(:focus):valid,.input-group>.form-control:not(:focus).is-valid,.was-validated .input-group>.form-select:not(:focus):valid,.input-group>.form-select:not(:focus).is-valid,.was-validated .input-group>.form-floating:not(:focus-within):valid,.input-group>.form-floating:not(:focus-within).is-valid{z-index:3}.invalid-feedback{display:none;width:100%;margin-top:.25rem;font-size:.875em;color:#dc3545}.invalid-tooltip{position:absolute;top:100%;z-index:5;display:none;max-width:100%;padding:.25rem .5rem;margin-top:.1rem;font-size:.875rem;color:#fff;background-color:rgba(220,53,69,0.9);border-radius:.375rem}.was-validated :invalid~.invalid-feedback,.was-validated :invalid~.invalid-tooltip,.is-invalid~.invalid-feedback,.is-invalid~.invalid-tooltip{display:block}.was-validated .form-control:invalid,.form-control.is-invalid{border-color:#dc3545;padding-right:calc(1.5em + .75rem);background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");background-repeat:no-repeat;background-position:right calc(.375em + .1875rem) center;background-size:calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-control:invalid:focus,.form-control.is-invalid:focus{border-color:#dc3545;box-shadow:0 0 0 .25rem rgba(220,53,69,0.25)}.was-validated textarea.form-control:invalid,textarea.form-control.is-invalid{padding-right:calc(1.5em + .75rem);background-position:top calc(.375em + .1875rem) right calc(.375em + .1875rem)}.was-validated .form-select:invalid,.form-select.is-invalid{border-color:#dc3545}.was-validated .form-select:invalid:not([multiple]):not([size]),.was-validated .form-select:invalid:not([multiple])[size="1"],.form-select.is-invalid:not([multiple]):not([size]),.form-select.is-invalid:not([multiple])[size="1"]{padding-right:4.125rem;background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e"),url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");background-position:right .75rem center,center right 2.25rem;background-size:16px 12px,calc(.75em + .375rem) calc(.75em + .375rem)}.was-validated .form-select:invalid:focus,.form-select.is-invalid:focus{border-color:#dc3545;box-shadow:0 0 0 .25rem rgba(220,53,69,0.25)}.was-validated .form-control-color:invalid,.form-control-color.is-invalid{width:calc(3rem + calc(1.5em + .75rem))}.was-validated .form-check-input:invalid,.form-check-input.is-invalid{border-color:#dc3545}.was-validated .form-check-input:invalid:checked,.form-check-input.is-invalid:checked{background-color:#dc3545}.was-validated .form-check-input:invalid:focus,.form-check-input.is-invalid:focus{box-shadow:0 0 0 .25rem rgba(220,53,69,0.25)}.was-validated .form-check-input:invalid~.form-check-label,.form-check-input.is-invalid~.form-check-label{color:#dc3545}.form-check-inline .form-check-input~.invalid-feedback{margin-left:.5em}.was-validated .input-group>.form-control:not(:focus):invalid,.input-group>.form-control:not(:focus).is-invalid,.was-validated .input-group>.form-select:not(:focus):invalid,.input-group>.form-select:not(:focus).is-invalid,.was-validated .input-group>.form-floating:not(:focus-within):invalid,.input-group>.form-floating:not(:focus-within).is-invalid{z-index:4}.btn{--bs-btn-padding-x: .75rem;--bs-btn-padding-y: .375rem;--bs-btn-font-family: ;--bs-btn-font-size:1rem;--bs-btn-font-weight: 400;--bs-btn-line-height: 1.5;--bs-btn-color: #212529;--bs-btn-bg: transparent;--bs-btn-border-width: 1px;--bs-btn-border-color: transparent;--bs-btn-border-radius: .375rem;--bs-btn-hover-border-color: transparent;--bs-btn-box-shadow: inset 0 1px 0 rgba(255,255,255,0.15),0 1px 1px rgba(0,0,0,0.075);--bs-btn-disabled-opacity: .65;--bs-btn-focus-box-shadow: 0 0 0 .25rem rgba(var(--bs-btn-focus-shadow-rgb), .5);display:inline-block;padding:var(--bs-btn-padding-y) var(--bs-btn-padding-x);font-family:var(--bs-btn-font-family);font-size:var(--bs-btn-font-size);font-weight:var(--bs-btn-font-weight);line-height:var(--bs-btn-line-height);color:var(--bs-btn-color);text-align:center;text-decoration:none;-webkit-text-decoration:none;-moz-text-decoration:none;-ms-text-decoration:none;-o-text-decoration:none;vertical-align:middle;cursor:pointer;user-select:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;-o-user-select:none;border:var(--bs-btn-border-width) solid var(--bs-btn-border-color);border-radius:var(--bs-btn-border-radius);background-color:var(--bs-btn-bg);transition:color 0.15s ease-in-out,background-color 0.15s ease-in-out,border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out}@media (prefers-reduced-motion: reduce){.btn{transition:none}}.btn:hover{color:var(--bs-btn-hover-color);background-color:var(--bs-btn-hover-bg);border-color:var(--bs-btn-hover-border-color)}.btn-check+.btn:hover{color:var(--bs-btn-color);background-color:var(--bs-btn-bg);border-color:var(--bs-btn-border-color)}.btn:focus-visible{color:var(--bs-btn-hover-color);background-color:var(--bs-btn-hover-bg);border-color:var(--bs-btn-hover-border-color);outline:0;box-shadow:var(--bs-btn-focus-box-shadow)}.btn-check:focus-visible+.btn{border-color:var(--bs-btn-hover-border-color);outline:0;box-shadow:var(--bs-btn-focus-box-shadow)}.btn-check:checked+.btn,:not(.btn-check)+.btn:active,.btn:first-child:active,.btn.active,.btn.show,.btn.in{color:var(--bs-btn-active-color);background-color:var(--bs-btn-active-bg);border-color:var(--bs-btn-active-border-color)}.btn-check:checked+.btn:focus-visible,:not(.btn-check)+.btn:active:focus-visible,.btn:first-child:active:focus-visible,.btn.active:focus-visible,.btn.show:focus-visible,.btn.in:focus-visible{box-shadow:var(--bs-btn-focus-box-shadow)}.btn:disabled,.btn.disabled,fieldset:disabled .btn{color:var(--bs-btn-disabled-color);pointer-events:none;background-color:var(--bs-btn-disabled-bg);border-color:var(--bs-btn-disabled-border-color);opacity:var(--bs-btn-disabled-opacity)}.btn-default{--bs-btn-color: #000;--bs-btn-bg: #dee2e6;--bs-btn-border-color: #dee2e6;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #e3e6ea;--bs-btn-hover-border-color: #e1e5e9;--bs-btn-focus-shadow-rgb: 189,192,196;--bs-btn-active-color: #000;--bs-btn-active-bg: #e5e8eb;--bs-btn-active-border-color: #e1e5e9;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #dee2e6;--bs-btn-disabled-border-color: #dee2e6}.btn-primary{--bs-btn-color: #fff;--bs-btn-bg: #0d6efd;--bs-btn-border-color: #0d6efd;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #0b5ed7;--bs-btn-hover-border-color: #0a58ca;--bs-btn-focus-shadow-rgb: 49,132,253;--bs-btn-active-color: #fff;--bs-btn-active-bg: #0a58ca;--bs-btn-active-border-color: #0a53be;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #0d6efd;--bs-btn-disabled-border-color: #0d6efd}.btn-secondary{--bs-btn-color: #fff;--bs-btn-bg: #6c757d;--bs-btn-border-color: #6c757d;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #5c636a;--bs-btn-hover-border-color: #565e64;--bs-btn-focus-shadow-rgb: 130,138,145;--bs-btn-active-color: #fff;--bs-btn-active-bg: #565e64;--bs-btn-active-border-color: #51585e;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #6c757d;--bs-btn-disabled-border-color: #6c757d}.btn-success{--bs-btn-color: #fff;--bs-btn-bg: #198754;--bs-btn-border-color: #198754;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #157347;--bs-btn-hover-border-color: #146c43;--bs-btn-focus-shadow-rgb: 60,153,110;--bs-btn-active-color: #fff;--bs-btn-active-bg: #146c43;--bs-btn-active-border-color: #13653f;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #198754;--bs-btn-disabled-border-color: #198754}.btn-info{--bs-btn-color: #000;--bs-btn-bg: #0dcaf0;--bs-btn-border-color: #0dcaf0;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #31d2f2;--bs-btn-hover-border-color: #25cff2;--bs-btn-focus-shadow-rgb: 11,172,204;--bs-btn-active-color: #000;--bs-btn-active-bg: #3dd5f3;--bs-btn-active-border-color: #25cff2;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #0dcaf0;--bs-btn-disabled-border-color: #0dcaf0}.btn-warning{--bs-btn-color: #000;--bs-btn-bg: #ffc107;--bs-btn-border-color: #ffc107;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #ffca2c;--bs-btn-hover-border-color: #ffc720;--bs-btn-focus-shadow-rgb: 217,164,6;--bs-btn-active-color: #000;--bs-btn-active-bg: #ffcd39;--bs-btn-active-border-color: #ffc720;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #ffc107;--bs-btn-disabled-border-color: #ffc107}.btn-danger{--bs-btn-color: #fff;--bs-btn-bg: #dc3545;--bs-btn-border-color: #dc3545;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #bb2d3b;--bs-btn-hover-border-color: #b02a37;--bs-btn-focus-shadow-rgb: 225,83,97;--bs-btn-active-color: #fff;--bs-btn-active-bg: #b02a37;--bs-btn-active-border-color: #a52834;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #dc3545;--bs-btn-disabled-border-color: #dc3545}.btn-light{--bs-btn-color: #000;--bs-btn-bg: #f8f9fa;--bs-btn-border-color: #f8f9fa;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #d3d4d5;--bs-btn-hover-border-color: #c6c7c8;--bs-btn-focus-shadow-rgb: 211,212,213;--bs-btn-active-color: #000;--bs-btn-active-bg: #c6c7c8;--bs-btn-active-border-color: #babbbc;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #000;--bs-btn-disabled-bg: #f8f9fa;--bs-btn-disabled-border-color: #f8f9fa}.btn-dark{--bs-btn-color: #fff;--bs-btn-bg: #212529;--bs-btn-border-color: #212529;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #424649;--bs-btn-hover-border-color: #373b3e;--bs-btn-focus-shadow-rgb: 66,70,73;--bs-btn-active-color: #fff;--bs-btn-active-bg: #4d5154;--bs-btn-active-border-color: #373b3e;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #fff;--bs-btn-disabled-bg: #212529;--bs-btn-disabled-border-color: #212529}.btn-outline-default{--bs-btn-color: #dee2e6;--bs-btn-border-color: #dee2e6;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #dee2e6;--bs-btn-hover-border-color: #dee2e6;--bs-btn-focus-shadow-rgb: 222,226,230;--bs-btn-active-color: #000;--bs-btn-active-bg: #dee2e6;--bs-btn-active-border-color: #dee2e6;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #dee2e6;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #dee2e6;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-primary{--bs-btn-color: #0d6efd;--bs-btn-border-color: #0d6efd;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #0d6efd;--bs-btn-hover-border-color: #0d6efd;--bs-btn-focus-shadow-rgb: 13,110,253;--bs-btn-active-color: #fff;--bs-btn-active-bg: #0d6efd;--bs-btn-active-border-color: #0d6efd;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #0d6efd;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #0d6efd;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-secondary{--bs-btn-color: #6c757d;--bs-btn-border-color: #6c757d;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #6c757d;--bs-btn-hover-border-color: #6c757d;--bs-btn-focus-shadow-rgb: 108,117,125;--bs-btn-active-color: #fff;--bs-btn-active-bg: #6c757d;--bs-btn-active-border-color: #6c757d;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #6c757d;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #6c757d;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-success{--bs-btn-color: #198754;--bs-btn-border-color: #198754;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #198754;--bs-btn-hover-border-color: #198754;--bs-btn-focus-shadow-rgb: 25,135,84;--bs-btn-active-color: #fff;--bs-btn-active-bg: #198754;--bs-btn-active-border-color: #198754;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #198754;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #198754;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-info{--bs-btn-color: #0dcaf0;--bs-btn-border-color: #0dcaf0;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #0dcaf0;--bs-btn-hover-border-color: #0dcaf0;--bs-btn-focus-shadow-rgb: 13,202,240;--bs-btn-active-color: #000;--bs-btn-active-bg: #0dcaf0;--bs-btn-active-border-color: #0dcaf0;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #0dcaf0;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #0dcaf0;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-warning{--bs-btn-color: #ffc107;--bs-btn-border-color: #ffc107;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #ffc107;--bs-btn-hover-border-color: #ffc107;--bs-btn-focus-shadow-rgb: 255,193,7;--bs-btn-active-color: #000;--bs-btn-active-bg: #ffc107;--bs-btn-active-border-color: #ffc107;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #ffc107;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #ffc107;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-danger{--bs-btn-color: #dc3545;--bs-btn-border-color: #dc3545;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #dc3545;--bs-btn-hover-border-color: #dc3545;--bs-btn-focus-shadow-rgb: 220,53,69;--bs-btn-active-color: #fff;--bs-btn-active-bg: #dc3545;--bs-btn-active-border-color: #dc3545;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #dc3545;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #dc3545;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-light{--bs-btn-color: #f8f9fa;--bs-btn-border-color: #f8f9fa;--bs-btn-hover-color: #000;--bs-btn-hover-bg: #f8f9fa;--bs-btn-hover-border-color: #f8f9fa;--bs-btn-focus-shadow-rgb: 248,249,250;--bs-btn-active-color: #000;--bs-btn-active-bg: #f8f9fa;--bs-btn-active-border-color: #f8f9fa;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #f8f9fa;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #f8f9fa;--bs-btn-bg: transparent;--bs-gradient: none}.btn-outline-dark{--bs-btn-color: #212529;--bs-btn-border-color: #212529;--bs-btn-hover-color: #fff;--bs-btn-hover-bg: #212529;--bs-btn-hover-border-color: #212529;--bs-btn-focus-shadow-rgb: 33,37,41;--bs-btn-active-color: #fff;--bs-btn-active-bg: #212529;--bs-btn-active-border-color: #212529;--bs-btn-active-shadow: inset 0 3px 5px rgba(0,0,0,0.125);--bs-btn-disabled-color: #212529;--bs-btn-disabled-bg: transparent;--bs-btn-disabled-border-color: #212529;--bs-btn-bg: transparent;--bs-gradient: none}.btn-link{--bs-btn-font-weight: 400;--bs-btn-color: var(--bs-link-color);--bs-btn-bg: transparent;--bs-btn-border-color: transparent;--bs-btn-hover-color: var(--bs-link-hover-color);--bs-btn-hover-border-color: transparent;--bs-btn-active-color: var(--bs-link-hover-color);--bs-btn-active-border-color: transparent;--bs-btn-disabled-color: #6c757d;--bs-btn-disabled-border-color: transparent;--bs-btn-box-shadow: none;--bs-btn-focus-shadow-rgb: 49,132,253;text-decoration:underline;-webkit-text-decoration:underline;-moz-text-decoration:underline;-ms-text-decoration:underline;-o-text-decoration:underline}.btn-link:focus-visible{color:var(--bs-btn-color)}.btn-link:hover{color:var(--bs-btn-hover-color)}.btn-lg,.btn-group-lg>.btn{--bs-btn-padding-y: .5rem;--bs-btn-padding-x: 1rem;--bs-btn-font-size:1.25rem;--bs-btn-border-radius: .5rem}.btn-sm,.btn-group-sm>.btn{--bs-btn-padding-y: .25rem;--bs-btn-padding-x: .5rem;--bs-btn-font-size:.875rem;--bs-btn-border-radius: .25rem}.fade{transition:opacity 0.15s linear}@media (prefers-reduced-motion: reduce){.fade{transition:none}}.fade:not(.show):not(.in){opacity:0}.collapse:not(.show):not(.in){display:none}.collapsing{height:0;overflow:hidden;transition:height 0.35s ease}@media (prefers-reduced-motion: reduce){.collapsing{transition:none}}.collapsing.collapse-horizontal{width:0;height:auto;transition:width 0.35s ease}@media (prefers-reduced-motion: reduce){.collapsing.collapse-horizontal{transition:none}}.dropup,.dropend,.dropdown,.dropstart,.dropup-center,.dropdown-center{position:relative}.dropdown-toggle{white-space:nowrap}.dropdown-toggle::after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:"";border-top:.3em solid;border-right:.3em solid transparent;border-bottom:0;border-left:.3em solid transparent}.dropdown-toggle:empty::after{margin-left:0}.dropdown-menu{--bs-dropdown-zindex: 1000;--bs-dropdown-min-width: 10rem;--bs-dropdown-padding-x: 0;--bs-dropdown-padding-y: .5rem;--bs-dropdown-spacer: .125rem;--bs-dropdown-font-size:1rem;--bs-dropdown-color: #212529;--bs-dropdown-bg: #fff;--bs-dropdown-border-color: var(--bs-border-color-translucent);--bs-dropdown-border-radius: .375rem;--bs-dropdown-border-width: 1px;--bs-dropdown-inner-border-radius: calc(.375rem - 1px);--bs-dropdown-divider-bg: var(--bs-border-color-translucent);--bs-dropdown-divider-margin-y: .5rem;--bs-dropdown-box-shadow: 0 0.5rem 1rem rgba(0,0,0,0.15);--bs-dropdown-link-color: #212529;--bs-dropdown-link-hover-color: #1e2125;--bs-dropdown-link-hover-bg: #e9ecef;--bs-dropdown-link-active-color: #fff;--bs-dropdown-link-active-bg: #0d6efd;--bs-dropdown-link-disabled-color: #adb5bd;--bs-dropdown-item-padding-x: 1rem;--bs-dropdown-item-padding-y: .25rem;--bs-dropdown-header-color: #6c757d;--bs-dropdown-header-padding-x: 1rem;--bs-dropdown-header-padding-y: .5rem;position:absolute;z-index:var(--bs-dropdown-zindex);display:none;min-width:var(--bs-dropdown-min-width);padding:var(--bs-dropdown-padding-y) var(--bs-dropdown-padding-x);margin:0;font-size:var(--bs-dropdown-font-size);color:var(--bs-dropdown-color);text-align:left;list-style:none;background-color:var(--bs-dropdown-bg);background-clip:padding-box;border:var(--bs-dropdown-border-width) solid var(--bs-dropdown-border-color);border-radius:var(--bs-dropdown-border-radius)}.dropdown-menu[data-bs-popper]{top:100%;left:0;margin-top:var(--bs-dropdown-spacer)}.dropdown-menu-start{--bs-position: start}.dropdown-menu-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-end{--bs-position: end}.dropdown-menu-end[data-bs-popper]{right:0;left:auto}@media (min-width: 576px){.dropdown-menu-sm-start{--bs-position: start}.dropdown-menu-sm-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-sm-end{--bs-position: end}.dropdown-menu-sm-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 768px){.dropdown-menu-md-start{--bs-position: start}.dropdown-menu-md-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-md-end{--bs-position: end}.dropdown-menu-md-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 992px){.dropdown-menu-lg-start{--bs-position: start}.dropdown-menu-lg-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-lg-end{--bs-position: end}.dropdown-menu-lg-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 1200px){.dropdown-menu-xl-start{--bs-position: start}.dropdown-menu-xl-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-xl-end{--bs-position: end}.dropdown-menu-xl-end[data-bs-popper]{right:0;left:auto}}@media (min-width: 1400px){.dropdown-menu-xxl-start{--bs-position: start}.dropdown-menu-xxl-start[data-bs-popper]{right:auto;left:0}.dropdown-menu-xxl-end{--bs-position: end}.dropdown-menu-xxl-end[data-bs-popper]{right:0;left:auto}}.dropup .dropdown-menu[data-bs-popper]{top:auto;bottom:100%;margin-top:0;margin-bottom:var(--bs-dropdown-spacer)}.dropup .dropdown-toggle::after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:"";border-top:0;border-right:.3em solid transparent;border-bottom:.3em solid;border-left:.3em solid transparent}.dropup .dropdown-toggle:empty::after{margin-left:0}.dropend .dropdown-menu[data-bs-popper]{top:0;right:auto;left:100%;margin-top:0;margin-left:var(--bs-dropdown-spacer)}.dropend .dropdown-toggle::after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:"";border-top:.3em solid transparent;border-right:0;border-bottom:.3em solid transparent;border-left:.3em solid}.dropend .dropdown-toggle:empty::after{margin-left:0}.dropend .dropdown-toggle::after{vertical-align:0}.dropstart .dropdown-menu[data-bs-popper]{top:0;right:100%;left:auto;margin-top:0;margin-right:var(--bs-dropdown-spacer)}.dropstart .dropdown-toggle::after{display:inline-block;margin-left:.255em;vertical-align:.255em;content:""}.dropstart .dropdown-toggle::after{display:none}.dropstart .dropdown-toggle::before{display:inline-block;margin-right:.255em;vertical-align:.255em;content:"";border-top:.3em solid transparent;border-right:.3em solid;border-bottom:.3em solid transparent}.dropstart .dropdown-toggle:empty::after{margin-left:0}.dropstart .dropdown-toggle::before{vertical-align:0}.dropdown-divider,.dropdown-menu>li.divider{height:0;margin:var(--bs-dropdown-divider-margin-y) 0;overflow:hidden;border-top:1px solid var(--bs-dropdown-divider-bg);opacity:1}.dropdown-item,.dropdown-menu>li>a{display:block;width:100%;padding:var(--bs-dropdown-item-padding-y) var(--bs-dropdown-item-padding-x);clear:both;font-weight:400;color:var(--bs-dropdown-link-color);text-align:inherit;text-decoration:none;-webkit-text-decoration:none;-moz-text-decoration:none;-ms-text-decoration:none;-o-text-decoration:none;white-space:nowrap;background-color:transparent;border:0}.dropdown-item:hover,.dropdown-menu>li>a:hover,.dropdown-item:focus,.dropdown-menu>li>a:focus{color:var(--bs-dropdown-link-hover-color);background-color:var(--bs-dropdown-link-hover-bg)}.dropdown-item.active,.dropdown-menu>li>a.active,.dropdown-item:active,.dropdown-menu>li>a:active{color:var(--bs-dropdown-link-active-color);text-decoration:none;background-color:var(--bs-dropdown-link-active-bg)}.dropdown-item.disabled,.dropdown-menu>li>a.disabled,.dropdown-item:disabled,.dropdown-menu>li>a:disabled{color:var(--bs-dropdown-link-disabled-color);pointer-events:none;background-color:transparent}.dropdown-menu.show,.dropdown-menu.in{display:block}.dropdown-header{display:block;padding:var(--bs-dropdown-header-padding-y) var(--bs-dropdown-header-padding-x);margin-bottom:0;font-size:.875rem;color:var(--bs-dropdown-header-color);white-space:nowrap}.dropdown-item-text{display:block;padding:var(--bs-dropdown-item-padding-y) var(--bs-dropdown-item-padding-x);color:var(--bs-dropdown-link-color)}.dropdown-menu-dark{--bs-dropdown-color: #dee2e6;--bs-dropdown-bg: #343a40;--bs-dropdown-border-color: var(--bs-border-color-translucent);--bs-dropdown-box-shadow: ;--bs-dropdown-link-color: #dee2e6;--bs-dropdown-link-hover-color: #fff;--bs-dropdown-divider-bg: var(--bs-border-color-translucent);--bs-dropdown-link-hover-bg: rgba(255,255,255,0.15);--bs-dropdown-link-active-color: #fff;--bs-dropdown-link-active-bg: #0d6efd;--bs-dropdown-link-disabled-color: #adb5bd;--bs-dropdown-header-color: #adb5bd}.btn-group,.btn-group-vertical{position:relative;display:inline-flex;vertical-align:middle}.btn-group>.btn,.btn-group-vertical>.btn{position:relative;flex:1 1 auto;-webkit-flex:1 1 auto}.btn-group>.btn-check:checked+.btn,.btn-group>.btn-check:focus+.btn,.btn-group>.btn:hover,.btn-group>.btn:focus,.btn-group>.btn:active,.btn-group>.btn.active,.btn-group-vertical>.btn-check:checked+.btn,.btn-group-vertical>.btn-check:focus+.btn,.btn-group-vertical>.btn:hover,.btn-group-vertical>.btn:focus,.btn-group-vertical>.btn:active,.btn-group-vertical>.btn.active{z-index:1}.btn-toolbar{display:flex;display:-webkit-flex;flex-wrap:wrap;-webkit-flex-wrap:wrap;justify-content:flex-start;-webkit-justify-content:flex-start}.btn-toolbar .input-group{width:auto}.btn-group{border-radius:.375rem}.btn-group>:not(.btn-check:first-child)+.btn,.btn-group>.btn-group:not(:first-child){margin-left:-1px}.btn-group>.btn:not(:last-child):not(.dropdown-toggle),.btn-group>.btn.dropdown-toggle-split:first-child,.btn-group>.btn-group:not(:last-child)>.btn{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:nth-child(n + 3),.btn-group>:not(.btn-check)+.btn,.btn-group>.btn-group:not(:first-child)>.btn{border-top-left-radius:0;border-bottom-left-radius:0}.dropdown-toggle-split{padding-right:.5625rem;padding-left:.5625rem}.dropdown-toggle-split::after,.dropup .dropdown-toggle-split::after,.dropend .dropdown-toggle-split::after{margin-left:0}.dropstart .dropdown-toggle-split::before{margin-right:0}.btn-sm+.dropdown-toggle-split,.btn-group-sm>.btn+.dropdown-toggle-split{padding-right:.375rem;padding-left:.375rem}.btn-lg+.dropdown-toggle-split,.btn-group-lg>.btn+.dropdown-toggle-split{padding-right:.75rem;padding-left:.75rem}.btn-group-vertical{flex-direction:column;-webkit-flex-direction:column;align-items:flex-start;-webkit-align-items:flex-start;justify-content:center;-webkit-justify-content:center}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group{width:100%}.btn-group-vertical>.btn:not(:first-child),.btn-group-vertical>.btn-group:not(:first-child){margin-top:-1px}.btn-group-vertical>.btn:not(:last-child):not(.dropdown-toggle),.btn-group-vertical>.btn-group:not(:last-child)>.btn{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn~.btn,.btn-group-vertical>.btn-group:not(:first-child)>.btn{border-top-left-radius:0;border-top-right-radius:0}.nav{--bs-nav-link-padding-x: 1rem;--bs-nav-link-padding-y: .5rem;--bs-nav-link-font-weight: ;--bs-nav-link-color: var(--bs-link-color);--bs-nav-link-hover-color: var(--bs-link-hover-color);--bs-nav-link-disabled-color: #6c757d;display:flex;display:-webkit-flex;flex-wrap:wrap;-webkit-flex-wrap:wrap;padding-left:0;margin-bottom:0;list-style:none}.nav-link,.nav-tabs>li>a,.nav-pills>li>a,ul.nav.navbar-nav>li>a{display:block;padding:var(--bs-nav-link-padding-y) var(--bs-nav-link-padding-x);font-size:var(--bs-nav-link-font-size);font-weight:var(--bs-nav-link-font-weight);color:var(--bs-nav-link-color);text-decoration:none;-webkit-text-decoration:none;-moz-text-decoration:none;-ms-text-decoration:none;-o-text-decoration:none;transition:color 0.15s ease-in-out,background-color 0.15s ease-in-out,border-color 0.15s ease-in-out}@media (prefers-reduced-motion: reduce){.nav-link,.nav-tabs>li>a,.nav-pills>li>a,ul.nav.navbar-nav>li>a{transition:none}}.nav-link:hover,.nav-tabs>li>a:hover,.nav-pills>li>a:hover,ul.nav.navbar-nav>li>a:hover,.nav-link:focus,.nav-tabs>li>a:focus,.nav-pills>li>a:focus,ul.nav.navbar-nav>li>a:focus{color:var(--bs-nav-link-hover-color)}.nav-link.disabled,.nav-tabs>li>a.disabled,.nav-pills>li>a.disabled,ul.nav.navbar-nav>li>a.disabled{color:var(--bs-nav-link-disabled-color);pointer-events:none;cursor:default}.nav-tabs{--bs-nav-tabs-border-width: 1px;--bs-nav-tabs-border-color: #dee2e6;--bs-nav-tabs-border-radius: .375rem;--bs-nav-tabs-link-hover-border-color: #e9ecef #e9ecef #dee2e6;--bs-nav-tabs-link-active-color: #495057;--bs-nav-tabs-link-active-bg: #fff;--bs-nav-tabs-link-active-border-color: #dee2e6 #dee2e6 #fff;border-bottom:var(--bs-nav-tabs-border-width) solid var(--bs-nav-tabs-border-color)}.nav-tabs .nav-link,.nav-tabs>li>a,.nav-tabs .nav-pills>li>a,.nav-tabs ul.nav.navbar-nav>li>a{margin-bottom:calc(-1 * var(--bs-nav-tabs-border-width));background:none;border:var(--bs-nav-tabs-border-width) solid transparent;border-top-left-radius:var(--bs-nav-tabs-border-radius);border-top-right-radius:var(--bs-nav-tabs-border-radius)}.nav-tabs .nav-link:hover,.nav-tabs>li>a:hover,.nav-tabs .nav-pills>li>a:hover,.nav-tabs ul.nav.navbar-nav>li>a:hover,.nav-tabs .nav-link:focus,.nav-tabs>li>a:focus,.nav-tabs .nav-pills>li>a:focus,.nav-tabs ul.nav.navbar-nav>li>a:focus{isolation:isolate;border-color:var(--bs-nav-tabs-link-hover-border-color)}.nav-tabs .nav-link.disabled,.nav-tabs>li>a.disabled,.nav-tabs .nav-pills>li>a.disabled,.nav-tabs ul.nav.navbar-nav>li>a.disabled,.nav-tabs .nav-link:disabled,.nav-tabs>li>a:disabled,.nav-tabs .nav-pills>li>a:disabled,.nav-tabs ul.nav.navbar-nav>li>a:disabled{color:var(--bs-nav-link-disabled-color);background-color:transparent;border-color:transparent}.nav-tabs .nav-link.active,.nav-tabs>li>a.active,.nav-tabs .nav-pills>li>a.active,.nav-tabs ul.nav.navbar-nav>li>a.active,.nav-tabs .nav-item.show .nav-link,.nav-tabs .nav-item.in .nav-link,.nav-tabs .nav-item.show .nav-tabs>li>a,.nav-tabs .nav-item.in .nav-tabs>li>a,.nav-tabs .nav-item.show .nav-pills>li>a,.nav-tabs .nav-item.in .nav-pills>li>a,.nav-tabs>li.show .nav-link,.nav-tabs>li.in .nav-link,.nav-tabs>li.show .nav-tabs>li>a,.nav-tabs>li.in .nav-tabs>li>a,.nav-tabs>li.show .nav-pills>li>a,.nav-tabs>li.in .nav-pills>li>a,.nav-tabs .nav-pills>li.show .nav-link,.nav-tabs .nav-pills>li.in .nav-link,.nav-tabs .nav-pills>li.show .nav-tabs>li>a,.nav-tabs .nav-pills>li.in .nav-tabs>li>a,.nav-tabs .nav-pills>li.show .nav-pills>li>a,.nav-tabs .nav-pills>li.in .nav-pills>li>a,.nav-tabs .nav-item.show ul.nav.navbar-nav>li>a,.nav-tabs .nav-item.in ul.nav.navbar-nav>li>a,.nav-tabs>li.show ul.nav.navbar-nav>li>a,.nav-tabs>li.in ul.nav.navbar-nav>li>a,.nav-tabs .nav-pills>li.show ul.nav.navbar-nav>li>a,.nav-tabs .nav-pills>li.in ul.nav.navbar-nav>li>a,.nav-tabs ul.nav.navbar-nav>li.show:not(.dropdown) .nav-link,.nav-tabs ul.nav.navbar-nav>li.in:not(.dropdown) .nav-link,.nav-tabs ul.nav.navbar-nav>li.show:not(.dropdown) .nav-tabs>li>a,.nav-tabs ul.nav.navbar-nav>li.in:not(.dropdown) .nav-tabs>li>a,.nav-tabs ul.nav.navbar-nav>li.show:not(.dropdown) .nav-pills>li>a,.nav-tabs ul.nav.navbar-nav>li.in:not(.dropdown) .nav-pills>li>a,.nav-tabs ul.nav.navbar-nav>li.show:not(.dropdown) ul.nav.navbar-nav>li>a,.nav-tabs ul.nav.navbar-nav>li.in:not(.dropdown) ul.nav.navbar-nav>li>a{color:var(--bs-nav-tabs-link-active-color);background-color:var(--bs-nav-tabs-link-active-bg);border-color:var(--bs-nav-tabs-link-active-border-color)}.nav-tabs .dropdown-menu{margin-top:calc(-1 * var(--bs-nav-tabs-border-width));border-top-left-radius:0;border-top-right-radius:0}.nav-pills{--bs-nav-pills-border-radius: .375rem;--bs-nav-pills-link-active-color: #fff;--bs-nav-pills-link-active-bg: #0d6efd}.nav-pills .nav-link,.nav-pills .nav-tabs>li>a,.nav-pills>li>a,.nav-pills ul.nav.navbar-nav>li>a{background:none;border:0;border-radius:var(--bs-nav-pills-border-radius)}.nav-pills .nav-link:disabled,.nav-pills .nav-tabs>li>a:disabled,.nav-pills>li>a:disabled,.nav-pills ul.nav.navbar-nav>li>a:disabled{color:var(--bs-nav-link-disabled-color);background-color:transparent;border-color:transparent}.nav-pills .nav-link.active,.nav-pills .nav-tabs>li>a.active,.nav-pills>li>a.active,.nav-pills ul.nav.navbar-nav>li>a.active,.nav-pills .show>.nav-link,.nav-pills .in>.nav-link,.nav-pills .nav-tabs>li.show>a,.nav-pills .nav-tabs>li.in>a,.nav-pills>li.show>a,.nav-pills>li.in>a,.nav-pills ul.nav.navbar-nav>li.show>a,.nav-pills ul.nav.navbar-nav>li.in>a{color:var(--bs-nav-pills-link-active-color);background-color:var(--bs-nav-pills-link-active-bg)}.nav-fill>.nav-link,.nav-tabs>li.nav-fill>a,.nav-pills>li.nav-fill>a,ul.nav.navbar-nav>li.nav-fill>a,.nav-fill .nav-item,.nav-fill .nav-tabs>li,.nav-fill .nav-pills>li,.nav-fill ul.nav.navbar-nav>li:not(.dropdown){flex:1 1 auto;-webkit-flex:1 1 auto;text-align:center}.nav-justified>.nav-link,.nav-tabs>li.nav-justified>a,.nav-pills>li.nav-justified>a,ul.nav.navbar-nav>li.nav-justified>a,.nav-justified .nav-item,.nav-justified .nav-tabs>li,.nav-justified .nav-pills>li,.nav-justified ul.nav.navbar-nav>li:not(.dropdown){flex-basis:0;-webkit-flex-basis:0;flex-grow:1;-webkit-flex-grow:1;text-align:center}.nav-fill .nav-item .nav-link,.nav-fill .nav-tabs>li .nav-link,.nav-fill .nav-tabs>li>a,.nav-fill .nav-pills>li .nav-link,.nav-fill .nav-pills>li>a,.nav-fill .nav-item ul.nav.navbar-nav>li>a,.nav-fill .nav-tabs>li ul.nav.navbar-nav>li>a,.nav-fill .nav-pills>li ul.nav.navbar-nav>li>a,.nav-fill ul.nav.navbar-nav>li:not(.dropdown) .nav-link,.nav-fill ul.nav.navbar-nav>li:not(.dropdown) .nav-tabs>li>a,.nav-fill ul.nav.navbar-nav>li:not(.dropdown) .nav-pills>li>a,.nav-fill ul.nav.navbar-nav>li:not(.dropdown) ul.nav.navbar-nav>li>a,.nav-justified .nav-item .nav-link,.nav-justified .nav-tabs>li .nav-link,.nav-justified .nav-tabs>li>a,.nav-justified .nav-pills>li .nav-link,.nav-justified .nav-pills>li>a,.nav-justified .nav-item ul.nav.navbar-nav>li>a,.nav-justified .nav-tabs>li ul.nav.navbar-nav>li>a,.nav-justified .nav-pills>li ul.nav.navbar-nav>li>a,.nav-justified ul.nav.navbar-nav>li:not(.dropdown) .nav-link,.nav-justified ul.nav.navbar-nav>li:not(.dropdown) .nav-tabs>li>a,.nav-justified ul.nav.navbar-nav>li:not(.dropdown) .nav-pills>li>a,.nav-justified ul.nav.navbar-nav>li:not(.dropdown) ul.nav.navbar-nav>li>a{width:100%}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.navbar{--bs-navbar-padding-x: 0;--bs-navbar-padding-y: .5rem;--bs-navbar-color: rgba(0,0,0,0.55);--bs-navbar-hover-color: rgba(0,0,0,0.7);--bs-navbar-disabled-color: rgba(0,0,0,0.3);--bs-navbar-active-color: rgba(0,0,0,0.9);--bs-navbar-brand-padding-y: .3125rem;--bs-navbar-brand-margin-end: 1rem;--bs-navbar-brand-font-size: 1.25rem;--bs-navbar-brand-color: rgba(0,0,0,0.9);--bs-navbar-brand-hover-color: rgba(0,0,0,0.9);--bs-navbar-nav-link-padding-x: .5rem;--bs-navbar-toggler-padding-y: .25rem;--bs-navbar-toggler-padding-x: .75rem;--bs-navbar-toggler-font-size: 1.25rem;--bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%280,0,0,0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");--bs-navbar-toggler-border-color: rgba(0,0,0,0.1);--bs-navbar-toggler-border-radius: .375rem;--bs-navbar-toggler-focus-width: .25rem;--bs-navbar-toggler-transition: box-shadow 0.15s ease-in-out;position:relative;display:flex;display:-webkit-flex;flex-wrap:wrap;-webkit-flex-wrap:wrap;align-items:center;-webkit-align-items:center;justify-content:space-between;-webkit-justify-content:space-between;padding:var(--bs-navbar-padding-y) var(--bs-navbar-padding-x)}.navbar>.container,.navbar>.container-fluid,.navbar>.container-sm,.navbar>.container-md,.navbar>.container-lg,.navbar>.container-xl,.navbar>.container-xxl{display:flex;display:-webkit-flex;flex-wrap:inherit;-webkit-flex-wrap:inherit;align-items:center;-webkit-align-items:center;justify-content:space-between;-webkit-justify-content:space-between}.navbar-brand{padding-top:var(--bs-navbar-brand-padding-y);padding-bottom:var(--bs-navbar-brand-padding-y);margin-right:var(--bs-navbar-brand-margin-end);font-size:var(--bs-navbar-brand-font-size);color:var(--bs-navbar-brand-color);text-decoration:none;-webkit-text-decoration:none;-moz-text-decoration:none;-ms-text-decoration:none;-o-text-decoration:none;white-space:nowrap}.navbar-brand:hover,.navbar-brand:focus{color:var(--bs-navbar-brand-hover-color)}.navbar-nav{--bs-nav-link-padding-x: 0;--bs-nav-link-padding-y: .5rem;--bs-nav-link-font-weight: ;--bs-nav-link-color: var(--bs-navbar-color);--bs-nav-link-hover-color: var(--bs-navbar-hover-color);--bs-nav-link-disabled-color: var(--bs-navbar-disabled-color);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;padding-left:0;margin-bottom:0;list-style:none}.navbar-nav .show>.nav-link,.navbar-nav .in>.nav-link,.navbar-nav .nav-tabs>li.show>a,.navbar-nav .nav-tabs>li.in>a,.navbar-nav .nav-pills>li.show>a,.navbar-nav .nav-pills>li.in>a,ul.nav.navbar-nav>li.show>a,ul.nav.navbar-nav>li.in>a,.navbar-nav .active>.nav-link,.navbar-nav .nav-tabs>li.active>a,.navbar-nav .nav-pills>li.active>a,ul.nav.navbar-nav>li.active>a,.navbar-nav .nav-link.active,.navbar-nav .nav-tabs>li>a.active,.navbar-nav .nav-pills>li>a.active,ul.nav.navbar-nav>li>a.active{color:var(--bs-navbar-active-color)}.navbar-nav .dropdown-menu{position:static}.navbar-text{padding-top:.5rem;padding-bottom:.5rem;color:var(--bs-navbar-color)}.navbar-text a,.navbar-text a:hover,.navbar-text a:focus{color:var(--bs-navbar-active-color)}.navbar-collapse{flex-basis:100%;-webkit-flex-basis:100%;flex-grow:1;-webkit-flex-grow:1;align-items:center;-webkit-align-items:center}.navbar-toggler,.navbar-toggle{padding:var(--bs-navbar-toggler-padding-y) var(--bs-navbar-toggler-padding-x);font-size:var(--bs-navbar-toggler-font-size);line-height:1;color:var(--bs-navbar-color);background-color:transparent;border:var(--bs-border-width) solid var(--bs-navbar-toggler-border-color);border-radius:var(--bs-navbar-toggler-border-radius);transition:var(--bs-navbar-toggler-transition)}@media (prefers-reduced-motion: reduce){.navbar-toggler,.navbar-toggle{transition:none}}.navbar-toggler:hover,.navbar-toggle:hover{text-decoration:none}.navbar-toggler:focus,.navbar-toggle:focus{text-decoration:none;outline:0;box-shadow:0 0 0 var(--bs-navbar-toggler-focus-width)}.navbar-toggler-icon,.navbar-toggle>.icon-bar:last-child{display:inline-block;width:1.5em;height:1.5em;vertical-align:middle;background-image:var(--bs-navbar-toggler-icon-bg);background-repeat:no-repeat;background-position:center;background-size:100%}.navbar-nav-scroll{max-height:var(--bs-scroll-height, 75vh);overflow-y:auto}@media (min-width: 576px){.navbar-expand-sm,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl){flex-wrap:nowrap;-webkit-flex-wrap:nowrap;justify-content:flex-start;-webkit-justify-content:flex-start}.navbar-expand-sm .navbar-nav,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-nav{flex-direction:row;-webkit-flex-direction:row}.navbar-expand-sm .navbar-nav .dropdown-menu,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-sm .navbar-nav .nav-link,.navbar-expand-sm .navbar-nav .nav-tabs>li>a,.navbar-expand-sm .navbar-nav .nav-pills>li>a,.navbar-expand-sm ul.nav.navbar-nav>li>a,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-nav .nav-link,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-nav .nav-tabs>li>a,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-nav .nav-pills>li>a,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) ul.nav.navbar-nav>li>a{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-sm .navbar-nav-scroll,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-nav-scroll{overflow:visible}.navbar-expand-sm .navbar-collapse,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-collapse{display:flex !important;display:-webkit-flex !important;flex-basis:auto;-webkit-flex-basis:auto}.navbar-expand-sm .navbar-toggler,.navbar-expand-sm .navbar-toggle,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-toggler,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .navbar-toggle{display:none}.navbar-expand-sm .offcanvas,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .offcanvas{position:static;z-index:auto;flex-grow:1;-webkit-flex-grow:1;width:auto !important;height:auto !important;visibility:visible !important;background-color:transparent !important;border:0 !important;transform:none !important;transition:none}.navbar-expand-sm .offcanvas .offcanvas-header,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .offcanvas .offcanvas-header{display:none}.navbar-expand-sm .offcanvas .offcanvas-body,.navbar:not(.navbar-expand):not(.navbar-expand-sm):not(.navbar-expand-md):not(.navbar-expand-lg):not(.navbar-expand-xl) .offcanvas .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 768px){.navbar-expand-md{flex-wrap:nowrap;-webkit-flex-wrap:nowrap;justify-content:flex-start;-webkit-justify-content:flex-start}.navbar-expand-md .navbar-nav{flex-direction:row;-webkit-flex-direction:row}.navbar-expand-md .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-md .navbar-nav .nav-link,.navbar-expand-md .navbar-nav .nav-tabs>li>a,.navbar-expand-md .navbar-nav .nav-pills>li>a,.navbar-expand-md ul.nav.navbar-nav>li>a{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-md .navbar-nav-scroll{overflow:visible}.navbar-expand-md .navbar-collapse{display:flex !important;display:-webkit-flex !important;flex-basis:auto;-webkit-flex-basis:auto}.navbar-expand-md .navbar-toggler,.navbar-expand-md .navbar-toggle{display:none}.navbar-expand-md .offcanvas{position:static;z-index:auto;flex-grow:1;-webkit-flex-grow:1;width:auto !important;height:auto !important;visibility:visible !important;background-color:transparent !important;border:0 !important;transform:none !important;transition:none}.navbar-expand-md .offcanvas .offcanvas-header{display:none}.navbar-expand-md .offcanvas .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 992px){.navbar-expand-lg{flex-wrap:nowrap;-webkit-flex-wrap:nowrap;justify-content:flex-start;-webkit-justify-content:flex-start}.navbar-expand-lg .navbar-nav{flex-direction:row;-webkit-flex-direction:row}.navbar-expand-lg .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-lg .navbar-nav .nav-link,.navbar-expand-lg .navbar-nav .nav-tabs>li>a,.navbar-expand-lg .navbar-nav .nav-pills>li>a,.navbar-expand-lg ul.nav.navbar-nav>li>a{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-lg .navbar-nav-scroll{overflow:visible}.navbar-expand-lg .navbar-collapse{display:flex !important;display:-webkit-flex !important;flex-basis:auto;-webkit-flex-basis:auto}.navbar-expand-lg .navbar-toggler,.navbar-expand-lg .navbar-toggle{display:none}.navbar-expand-lg .offcanvas{position:static;z-index:auto;flex-grow:1;-webkit-flex-grow:1;width:auto !important;height:auto !important;visibility:visible !important;background-color:transparent !important;border:0 !important;transform:none !important;transition:none}.navbar-expand-lg .offcanvas .offcanvas-header{display:none}.navbar-expand-lg .offcanvas .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 1200px){.navbar-expand-xl{flex-wrap:nowrap;-webkit-flex-wrap:nowrap;justify-content:flex-start;-webkit-justify-content:flex-start}.navbar-expand-xl .navbar-nav{flex-direction:row;-webkit-flex-direction:row}.navbar-expand-xl .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-xl .navbar-nav .nav-link,.navbar-expand-xl .navbar-nav .nav-tabs>li>a,.navbar-expand-xl .navbar-nav .nav-pills>li>a,.navbar-expand-xl ul.nav.navbar-nav>li>a{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-xl .navbar-nav-scroll{overflow:visible}.navbar-expand-xl .navbar-collapse{display:flex !important;display:-webkit-flex !important;flex-basis:auto;-webkit-flex-basis:auto}.navbar-expand-xl .navbar-toggler,.navbar-expand-xl .navbar-toggle{display:none}.navbar-expand-xl .offcanvas{position:static;z-index:auto;flex-grow:1;-webkit-flex-grow:1;width:auto !important;height:auto !important;visibility:visible !important;background-color:transparent !important;border:0 !important;transform:none !important;transition:none}.navbar-expand-xl .offcanvas .offcanvas-header{display:none}.navbar-expand-xl .offcanvas .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible}}@media (min-width: 1400px){.navbar-expand-xxl{flex-wrap:nowrap;-webkit-flex-wrap:nowrap;justify-content:flex-start;-webkit-justify-content:flex-start}.navbar-expand-xxl .navbar-nav{flex-direction:row;-webkit-flex-direction:row}.navbar-expand-xxl .navbar-nav .dropdown-menu{position:absolute}.navbar-expand-xxl .navbar-nav .nav-link,.navbar-expand-xxl .navbar-nav .nav-tabs>li>a,.navbar-expand-xxl .navbar-nav .nav-pills>li>a,.navbar-expand-xxl ul.nav.navbar-nav>li>a{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand-xxl .navbar-nav-scroll{overflow:visible}.navbar-expand-xxl .navbar-collapse{display:flex !important;display:-webkit-flex !important;flex-basis:auto;-webkit-flex-basis:auto}.navbar-expand-xxl .navbar-toggler,.navbar-expand-xxl .navbar-toggle{display:none}.navbar-expand-xxl .offcanvas{position:static;z-index:auto;flex-grow:1;-webkit-flex-grow:1;width:auto !important;height:auto !important;visibility:visible !important;background-color:transparent !important;border:0 !important;transform:none !important;transition:none}.navbar-expand-xxl .offcanvas .offcanvas-header{display:none}.navbar-expand-xxl .offcanvas .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible}}.navbar-expand{flex-wrap:nowrap;-webkit-flex-wrap:nowrap;justify-content:flex-start;-webkit-justify-content:flex-start}.navbar-expand .navbar-nav{flex-direction:row;-webkit-flex-direction:row}.navbar-expand .navbar-nav .dropdown-menu{position:absolute}.navbar-expand .navbar-nav .nav-link,.navbar-expand .navbar-nav .nav-tabs>li>a,.navbar-expand .navbar-nav .nav-pills>li>a,.navbar-expand ul.nav.navbar-nav>li>a{padding-right:var(--bs-navbar-nav-link-padding-x);padding-left:var(--bs-navbar-nav-link-padding-x)}.navbar-expand .navbar-nav-scroll{overflow:visible}.navbar-expand .navbar-collapse{display:flex !important;display:-webkit-flex !important;flex-basis:auto;-webkit-flex-basis:auto}.navbar-expand .navbar-toggler,.navbar-expand .navbar-toggle{display:none}.navbar-expand .offcanvas{position:static;z-index:auto;flex-grow:1;-webkit-flex-grow:1;width:auto !important;height:auto !important;visibility:visible !important;background-color:transparent !important;border:0 !important;transform:none !important;transition:none}.navbar-expand .offcanvas .offcanvas-header{display:none}.navbar-expand .offcanvas .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible}.navbar-light,.navbar.navbar-default{background-color:#f8f9fa}.navbar-dark,.navbar.navbar-inverse{background-color:#212529;--bs-navbar-color: rgba(255,255,255,0.55);--bs-navbar-hover-color: rgba(255,255,255,0.75);--bs-navbar-disabled-color: rgba(255,255,255,0.25);--bs-navbar-active-color: #fff;--bs-navbar-brand-color: #fff;--bs-navbar-brand-hover-color: #fff;--bs-navbar-toggler-border-color: rgba(255,255,255,0.1);--bs-navbar-toggler-icon-bg: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%28255,255,255,0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e")}.card,.well{--bs-card-spacer-y: 1rem;--bs-card-spacer-x: 1rem;--bs-card-title-spacer-y: .5rem;--bs-card-border-width: 1px;--bs-card-border-color: var(--bs-border-color-translucent);--bs-card-border-radius: .375rem;--bs-card-box-shadow: ;--bs-card-inner-border-radius: calc(.375rem - 1px);--bs-card-cap-padding-y: .5rem;--bs-card-cap-padding-x: 1rem;--bs-card-cap-bg: rgba(0,0,0,0.03);--bs-card-cap-color: ;--bs-card-height: ;--bs-card-color: ;--bs-card-bg: #fff;--bs-card-img-overlay-padding: 1rem;--bs-card-group-margin: .75rem;position:relative;display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;min-width:0;height:var(--bs-card-height);word-wrap:break-word;background-color:var(--bs-card-bg);background-clip:border-box;border:var(--bs-card-border-width) solid var(--bs-card-border-color);border-radius:var(--bs-card-border-radius)}.card>hr,.well>hr{margin-right:0;margin-left:0}.card>.list-group,.well>.list-group{border-top:inherit;border-bottom:inherit}.card>.list-group:first-child,.well>.list-group:first-child{border-top-width:0;border-top-left-radius:var(--bs-card-inner-border-radius);border-top-right-radius:var(--bs-card-inner-border-radius)}.card>.list-group:last-child,.well>.list-group:last-child{border-bottom-width:0;border-bottom-right-radius:var(--bs-card-inner-border-radius);border-bottom-left-radius:var(--bs-card-inner-border-radius)}.card>.card-header+.list-group,.well>.card-header+.list-group,.card>.list-group+.card-footer,.well>.list-group+.card-footer{border-top:0}.card-body{flex:1 1 auto;-webkit-flex:1 1 auto;padding:var(--bs-card-spacer-y) var(--bs-card-spacer-x);color:var(--bs-card-color)}.card-title{margin-bottom:var(--bs-card-title-spacer-y)}.card-subtitle{margin-top:calc(-.5 * var(--bs-card-title-spacer-y));margin-bottom:0}.card-text:last-child{margin-bottom:0}.card-link+.card-link{margin-left:var(--bs-card-spacer-x)}.card-header{padding:var(--bs-card-cap-padding-y) var(--bs-card-cap-padding-x);margin-bottom:0;color:var(--bs-card-cap-color);background-color:var(--bs-card-cap-bg);border-bottom:var(--bs-card-border-width) solid var(--bs-card-border-color)}.card-header:first-child{border-radius:var(--bs-card-inner-border-radius) var(--bs-card-inner-border-radius) 0 0}.card-footer{padding:var(--bs-card-cap-padding-y) var(--bs-card-cap-padding-x);color:var(--bs-card-cap-color);background-color:var(--bs-card-cap-bg);border-top:var(--bs-card-border-width) solid var(--bs-card-border-color)}.card-footer:last-child{border-radius:0 0 var(--bs-card-inner-border-radius) var(--bs-card-inner-border-radius)}.card-header-tabs{margin-right:calc(-.5 * var(--bs-card-cap-padding-x));margin-bottom:calc(-1 * var(--bs-card-cap-padding-y));margin-left:calc(-.5 * var(--bs-card-cap-padding-x));border-bottom:0}.card-header-tabs .nav-link.active,.card-header-tabs .nav-tabs>li>a.active,.card-header-tabs .nav-pills>li>a.active,.card-header-tabs ul.nav.navbar-nav>li>a.active{background-color:var(--bs-card-bg);border-bottom-color:var(--bs-card-bg)}.card-header-pills{margin-right:calc(-.5 * var(--bs-card-cap-padding-x));margin-left:calc(-.5 * var(--bs-card-cap-padding-x))}.card-img-overlay{position:absolute;top:0;right:0;bottom:0;left:0;padding:var(--bs-card-img-overlay-padding);border-radius:var(--bs-card-inner-border-radius)}.card-img,.card-img-top,.card-img-bottom{width:100%}.card-img,.card-img-top{border-top-left-radius:var(--bs-card-inner-border-radius);border-top-right-radius:var(--bs-card-inner-border-radius)}.card-img,.card-img-bottom{border-bottom-right-radius:var(--bs-card-inner-border-radius);border-bottom-left-radius:var(--bs-card-inner-border-radius)}.card-group>.card,.card-group>.well{margin-bottom:var(--bs-card-group-margin)}@media (min-width: 576px){.card-group{display:flex;display:-webkit-flex;flex-flow:row wrap;-webkit-flex-flow:row wrap}.card-group>.card,.card-group>.well{flex:1 0 0%;-webkit-flex:1 0 0%;margin-bottom:0}.card-group>.card+.card,.card-group>.well+.card,.card-group>.card+.well,.card-group>.well+.well{margin-left:0;border-left:0}.card-group>.card:not(:last-child),.card-group>.well:not(:last-child){border-top-right-radius:0;border-bottom-right-radius:0}.card-group>.card:not(:last-child) .card-img-top,.card-group>.well:not(:last-child) .card-img-top,.card-group>.card:not(:last-child) .card-header,.card-group>.well:not(:last-child) .card-header{border-top-right-radius:0}.card-group>.card:not(:last-child) .card-img-bottom,.card-group>.well:not(:last-child) .card-img-bottom,.card-group>.card:not(:last-child) .card-footer,.card-group>.well:not(:last-child) .card-footer{border-bottom-right-radius:0}.card-group>.card:not(:first-child),.card-group>.well:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.card-group>.card:not(:first-child) .card-img-top,.card-group>.well:not(:first-child) .card-img-top,.card-group>.card:not(:first-child) .card-header,.card-group>.well:not(:first-child) .card-header{border-top-left-radius:0}.card-group>.card:not(:first-child) .card-img-bottom,.card-group>.well:not(:first-child) .card-img-bottom,.card-group>.card:not(:first-child) .card-footer,.card-group>.well:not(:first-child) .card-footer{border-bottom-left-radius:0}}.accordion{--bs-accordion-color: #212529;--bs-accordion-bg: #fff;--bs-accordion-transition: color 0.15s ease-in-out,background-color 0.15s ease-in-out,border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out,border-radius 0.15s ease;--bs-accordion-border-color: var(--bs-border-color);--bs-accordion-border-width: 1px;--bs-accordion-border-radius: .375rem;--bs-accordion-inner-border-radius: calc(.375rem - 1px);--bs-accordion-btn-padding-x: 1.25rem;--bs-accordion-btn-padding-y: 1rem;--bs-accordion-btn-color: #212529;--bs-accordion-btn-bg: var(--bs-accordion-bg);--bs-accordion-btn-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23212529'%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");--bs-accordion-btn-icon-width: 1.25rem;--bs-accordion-btn-icon-transform: rotate(-180deg);--bs-accordion-btn-icon-transition: transform 0.2s ease-in-out;--bs-accordion-btn-active-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill=''%3e%3cpath fill-rule='evenodd' d='M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e");--bs-accordion-btn-focus-border-color: #86b7fe;--bs-accordion-btn-focus-box-shadow: 0 0 0 .25rem rgba(13,110,253,0.25);--bs-accordion-body-padding-x: 1.25rem;--bs-accordion-body-padding-y: 1rem;--bs-accordion-active-color: ;--bs-accordion-active-bg: }.accordion-button{position:relative;display:flex;display:-webkit-flex;align-items:center;-webkit-align-items:center;width:100%;padding:var(--bs-accordion-btn-padding-y) var(--bs-accordion-btn-padding-x);font-size:1rem;color:var(--bs-accordion-btn-color);text-align:left;background-color:var(--bs-accordion-btn-bg);border:0;border-radius:0;overflow-anchor:none;transition:var(--bs-accordion-transition)}@media (prefers-reduced-motion: reduce){.accordion-button{transition:none}}.accordion-button:not(.collapsed){color:var(--bs-accordion-active-color);background-color:var(--bs-accordion-active-bg);box-shadow:inset 0 calc(-1 * var(--bs-accordion-border-width)) 0 var(--bs-accordion-border-color)}.accordion-button:not(.collapsed)::after{background-image:var(--bs-accordion-btn-active-icon);transform:var(--bs-accordion-btn-icon-transform)}.accordion-button::after{flex-shrink:0;-webkit-flex-shrink:0;width:var(--bs-accordion-btn-icon-width);height:var(--bs-accordion-btn-icon-width);margin-left:auto;content:"";background-image:var(--bs-accordion-btn-icon);background-repeat:no-repeat;background-size:var(--bs-accordion-btn-icon-width);transition:var(--bs-accordion-btn-icon-transition)}@media (prefers-reduced-motion: reduce){.accordion-button::after{transition:none}}.accordion-button:hover{z-index:2}.accordion-button:focus{z-index:3;border-color:var(--bs-accordion-btn-focus-border-color);outline:0;box-shadow:var(--bs-accordion-btn-focus-box-shadow)}.accordion-header{margin-bottom:0}.accordion-item{color:var(--bs-accordion-color);background-color:var(--bs-accordion-bg);border:var(--bs-accordion-border-width) solid var(--bs-accordion-border-color)}.accordion-item:first-of-type{border-top-left-radius:var(--bs-accordion-border-radius);border-top-right-radius:var(--bs-accordion-border-radius)}.accordion-item:first-of-type .accordion-button{border-top-left-radius:var(--bs-accordion-inner-border-radius);border-top-right-radius:var(--bs-accordion-inner-border-radius)}.accordion-item:not(:first-of-type){border-top:0}.accordion-item:last-of-type{border-bottom-right-radius:var(--bs-accordion-border-radius);border-bottom-left-radius:var(--bs-accordion-border-radius)}.accordion-item:last-of-type .accordion-button.collapsed{border-bottom-right-radius:var(--bs-accordion-inner-border-radius);border-bottom-left-radius:var(--bs-accordion-inner-border-radius)}.accordion-item:last-of-type .accordion-collapse{border-bottom-right-radius:var(--bs-accordion-border-radius);border-bottom-left-radius:var(--bs-accordion-border-radius)}.accordion-body{padding:var(--bs-accordion-body-padding-y) var(--bs-accordion-body-padding-x)}.accordion-flush .accordion-collapse,.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion .accordion-collapse{border-width:0}.accordion-flush .accordion-item,.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion .accordion-item{border-right:0;border-left:0;border-radius:0}.accordion-flush .accordion-item:first-child,.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion .accordion-item:first-child{border-top:0}.accordion-flush .accordion-item:last-child,.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion .accordion-item:last-child{border-bottom:0}.accordion-flush .accordion-item .accordion-button,.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion .accordion-item .accordion-button,.accordion-flush .accordion-item .accordion-button.collapsed{border-radius:0}.breadcrumb{--bs-breadcrumb-padding-x: 0;--bs-breadcrumb-padding-y: 0;--bs-breadcrumb-margin-bottom: 1rem;--bs-breadcrumb-bg: ;--bs-breadcrumb-border-radius: ;--bs-breadcrumb-divider-color: #6c757d;--bs-breadcrumb-item-padding-x: .5rem;--bs-breadcrumb-item-active-color: #6c757d;display:flex;display:-webkit-flex;flex-wrap:wrap;-webkit-flex-wrap:wrap;padding:var(--bs-breadcrumb-padding-y) var(--bs-breadcrumb-padding-x);margin-bottom:var(--bs-breadcrumb-margin-bottom);font-size:var(--bs-breadcrumb-font-size);list-style:none;background-color:var(--bs-breadcrumb-bg);border-radius:var(--bs-breadcrumb-border-radius)}.breadcrumb-item+.breadcrumb-item{padding-left:var(--bs-breadcrumb-item-padding-x)}.breadcrumb-item+.breadcrumb-item::before{float:left;padding-right:var(--bs-breadcrumb-item-padding-x);color:var(--bs-breadcrumb-divider-color);content:var(--bs-breadcrumb-divider, "/") /* rtl: var(--bs-breadcrumb-divider, "/") */}.breadcrumb-item.active{color:var(--bs-breadcrumb-item-active-color)}.pagination{--bs-pagination-padding-x: .75rem;--bs-pagination-padding-y: .375rem;--bs-pagination-font-size:1rem;--bs-pagination-color: var(--bs-link-color);--bs-pagination-bg: #fff;--bs-pagination-border-width: 1px;--bs-pagination-border-color: #dee2e6;--bs-pagination-border-radius: .375rem;--bs-pagination-hover-color: var(--bs-link-hover-color);--bs-pagination-hover-bg: #e9ecef;--bs-pagination-hover-border-color: #dee2e6;--bs-pagination-focus-color: var(--bs-link-hover-color);--bs-pagination-focus-bg: #e9ecef;--bs-pagination-focus-box-shadow: 0 0 0 .25rem rgba(13,110,253,0.25);--bs-pagination-active-color: #fff;--bs-pagination-active-bg: #0d6efd;--bs-pagination-active-border-color: #0d6efd;--bs-pagination-disabled-color: #6c757d;--bs-pagination-disabled-bg: #fff;--bs-pagination-disabled-border-color: #dee2e6;display:flex;display:-webkit-flex;padding-left:0;list-style:none}.page-link{position:relative;display:block;padding:var(--bs-pagination-padding-y) var(--bs-pagination-padding-x);font-size:var(--bs-pagination-font-size);color:var(--bs-pagination-color);text-decoration:none;-webkit-text-decoration:none;-moz-text-decoration:none;-ms-text-decoration:none;-o-text-decoration:none;background-color:var(--bs-pagination-bg);border:var(--bs-pagination-border-width) solid var(--bs-pagination-border-color);transition:color 0.15s ease-in-out,background-color 0.15s ease-in-out,border-color 0.15s ease-in-out,box-shadow 0.15s ease-in-out}@media (prefers-reduced-motion: reduce){.page-link{transition:none}}.page-link:hover{z-index:2;color:var(--bs-pagination-hover-color);background-color:var(--bs-pagination-hover-bg);border-color:var(--bs-pagination-hover-border-color)}.page-link:focus{z-index:3;color:var(--bs-pagination-focus-color);background-color:var(--bs-pagination-focus-bg);outline:0;box-shadow:var(--bs-pagination-focus-box-shadow)}.page-link.active,.active>.page-link{z-index:3;color:var(--bs-pagination-active-color);background-color:var(--bs-pagination-active-bg);border-color:var(--bs-pagination-active-border-color)}.page-link.disabled,.disabled>.page-link{color:var(--bs-pagination-disabled-color);pointer-events:none;background-color:var(--bs-pagination-disabled-bg);border-color:var(--bs-pagination-disabled-border-color)}.page-item:not(:first-child) .page-link{margin-left:-1px}.page-item:first-child .page-link{border-top-left-radius:var(--bs-pagination-border-radius);border-bottom-left-radius:var(--bs-pagination-border-radius)}.page-item:last-child .page-link{border-top-right-radius:var(--bs-pagination-border-radius);border-bottom-right-radius:var(--bs-pagination-border-radius)}.pagination-lg{--bs-pagination-padding-x: 1.5rem;--bs-pagination-padding-y: .75rem;--bs-pagination-font-size:1.25rem;--bs-pagination-border-radius: .5rem}.pagination-sm{--bs-pagination-padding-x: .5rem;--bs-pagination-padding-y: .25rem;--bs-pagination-font-size:.875rem;--bs-pagination-border-radius: .25rem}.badge{--bs-badge-padding-x: .65em;--bs-badge-padding-y: .35em;--bs-badge-font-size:.75em;--bs-badge-font-weight: 700;--bs-badge-color: #fff;--bs-badge-border-radius: .375rem;display:inline-block;padding:var(--bs-badge-padding-y) var(--bs-badge-padding-x);font-size:var(--bs-badge-font-size);font-weight:var(--bs-badge-font-weight);line-height:1;color:var(--bs-badge-color);text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:var(--bs-badge-border-radius)}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.alert{--bs-alert-bg: transparent;--bs-alert-padding-x: 1rem;--bs-alert-padding-y: 1rem;--bs-alert-margin-bottom: 1rem;--bs-alert-color: inherit;--bs-alert-border-color: transparent;--bs-alert-border: 1px solid var(--bs-alert-border-color);--bs-alert-border-radius: .375rem;position:relative;padding:var(--bs-alert-padding-y) var(--bs-alert-padding-x);margin-bottom:var(--bs-alert-margin-bottom);color:var(--bs-alert-color);background-color:var(--bs-alert-bg);border:var(--bs-alert-border);border-radius:var(--bs-alert-border-radius)}.alert-heading{color:inherit}.alert-link{font-weight:700}.alert-dismissible{padding-right:3rem}.alert-dismissible .btn-close{position:absolute;top:0;right:0;z-index:2;padding:1.25rem 1rem}.alert-default{--bs-alert-color: #595a5c;--bs-alert-bg: #f8f9fa;--bs-alert-border-color: #f5f6f8}.alert-default .alert-link{color:#47484a}.alert-primary{--bs-alert-color: #084298;--bs-alert-bg: #cfe2ff;--bs-alert-border-color: #b6d4fe}.alert-primary .alert-link{color:#06357a}.alert-secondary{--bs-alert-color: #41464b;--bs-alert-bg: #e2e3e5;--bs-alert-border-color: #d3d6d8}.alert-secondary .alert-link{color:#34383c}.alert-success{--bs-alert-color: #0f5132;--bs-alert-bg: #d1e7dd;--bs-alert-border-color: #badbcc}.alert-success .alert-link{color:#0c4128}.alert-info{--bs-alert-color: #055160;--bs-alert-bg: #cff4fc;--bs-alert-border-color: #b6effb}.alert-info .alert-link{color:#04414d}.alert-warning{--bs-alert-color: #664d03;--bs-alert-bg: #fff3cd;--bs-alert-border-color: #ffecb5}.alert-warning .alert-link{color:#523e02}.alert-danger{--bs-alert-color: #842029;--bs-alert-bg: #f8d7da;--bs-alert-border-color: #f5c2c7}.alert-danger .alert-link{color:#6a1a21}.alert-light{--bs-alert-color: #636464;--bs-alert-bg: #fefefe;--bs-alert-border-color: #fdfdfe}.alert-light .alert-link{color:#4f5050}.alert-dark{--bs-alert-color: #141619;--bs-alert-bg: #d3d3d4;--bs-alert-border-color: #bcbebf}.alert-dark .alert-link{color:#101214}@keyframes progress-bar-stripes{0%{background-position-x:1rem}}.progress{--bs-progress-height: 1rem;--bs-progress-font-size:.75rem;--bs-progress-bg: #e9ecef;--bs-progress-border-radius: .375rem;--bs-progress-box-shadow: inset 0 1px 2px rgba(0,0,0,0.075);--bs-progress-bar-color: #fff;--bs-progress-bar-bg: #0d6efd;--bs-progress-bar-transition: width 0.6s ease;display:flex;display:-webkit-flex;height:var(--bs-progress-height);overflow:hidden;font-size:var(--bs-progress-font-size);background-color:var(--bs-progress-bg);border-radius:var(--bs-progress-border-radius)}.progress-bar{display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;justify-content:center;-webkit-justify-content:center;overflow:hidden;color:var(--bs-progress-bar-color);text-align:center;white-space:nowrap;background-color:var(--bs-progress-bar-bg);transition:var(--bs-progress-bar-transition)}@media (prefers-reduced-motion: reduce){.progress-bar{transition:none}}.progress-bar-striped{background-image:linear-gradient(45deg, rgba(255,255,255,0.15) 25%, transparent 25%, transparent 50%, rgba(255,255,255,0.15) 50%, rgba(255,255,255,0.15) 75%, transparent 75%, transparent);background-size:var(--bs-progress-height) var(--bs-progress-height)}.progress-bar-animated{animation:1s linear infinite progress-bar-stripes}@media (prefers-reduced-motion: reduce){.progress-bar-animated{animation:none}}.list-group{--bs-list-group-color: #212529;--bs-list-group-bg: #fff;--bs-list-group-border-color: rgba(0,0,0,0.125);--bs-list-group-border-width: 1px;--bs-list-group-border-radius: .375rem;--bs-list-group-item-padding-x: 1rem;--bs-list-group-item-padding-y: .5rem;--bs-list-group-action-color: #495057;--bs-list-group-action-hover-color: #495057;--bs-list-group-action-hover-bg: #f8f9fa;--bs-list-group-action-active-color: #212529;--bs-list-group-action-active-bg: #e9ecef;--bs-list-group-disabled-color: #6c757d;--bs-list-group-disabled-bg: #fff;--bs-list-group-active-color: #fff;--bs-list-group-active-bg: #0d6efd;--bs-list-group-active-border-color: #0d6efd;display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;padding-left:0;margin-bottom:0;border-radius:var(--bs-list-group-border-radius)}.list-group-numbered{list-style-type:none;counter-reset:section}.list-group-numbered>.list-group-item::before{content:counters(section, ".") ". ";counter-increment:section}.list-group-item-action{width:100%;color:var(--bs-list-group-action-color);text-align:inherit}.list-group-item-action:hover,.list-group-item-action:focus{z-index:1;color:var(--bs-list-group-action-hover-color);text-decoration:none;background-color:var(--bs-list-group-action-hover-bg)}.list-group-item-action:active{color:var(--bs-list-group-action-active-color);background-color:var(--bs-list-group-action-active-bg)}.list-group-item{position:relative;display:block;padding:var(--bs-list-group-item-padding-y) var(--bs-list-group-item-padding-x);color:var(--bs-list-group-color);text-decoration:none;-webkit-text-decoration:none;-moz-text-decoration:none;-ms-text-decoration:none;-o-text-decoration:none;background-color:var(--bs-list-group-bg);border:var(--bs-list-group-border-width) solid var(--bs-list-group-border-color)}.list-group-item:first-child{border-top-left-radius:inherit;border-top-right-radius:inherit}.list-group-item:last-child{border-bottom-right-radius:inherit;border-bottom-left-radius:inherit}.list-group-item.disabled,.list-group-item:disabled{color:var(--bs-list-group-disabled-color);pointer-events:none;background-color:var(--bs-list-group-disabled-bg)}.list-group-item.active{z-index:2;color:var(--bs-list-group-active-color);background-color:var(--bs-list-group-active-bg);border-color:var(--bs-list-group-active-border-color)}.list-group-item+.list-group-item{border-top-width:0}.list-group-item+.list-group-item.active{margin-top:calc(-1 * var(--bs-list-group-border-width));border-top-width:var(--bs-list-group-border-width)}.list-group-horizontal{flex-direction:row;-webkit-flex-direction:row}.list-group-horizontal>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal>.list-group-item.active{margin-top:0}.list-group-horizontal>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}@media (min-width: 576px){.list-group-horizontal-sm{flex-direction:row;-webkit-flex-direction:row}.list-group-horizontal-sm>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-sm>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-sm>.list-group-item.active{margin-top:0}.list-group-horizontal-sm>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-sm>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 768px){.list-group-horizontal-md{flex-direction:row;-webkit-flex-direction:row}.list-group-horizontal-md>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-md>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-md>.list-group-item.active{margin-top:0}.list-group-horizontal-md>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-md>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 992px){.list-group-horizontal-lg{flex-direction:row;-webkit-flex-direction:row}.list-group-horizontal-lg>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-lg>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-lg>.list-group-item.active{margin-top:0}.list-group-horizontal-lg>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-lg>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 1200px){.list-group-horizontal-xl{flex-direction:row;-webkit-flex-direction:row}.list-group-horizontal-xl>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-xl>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-xl>.list-group-item.active{margin-top:0}.list-group-horizontal-xl>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-xl>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}@media (min-width: 1400px){.list-group-horizontal-xxl{flex-direction:row;-webkit-flex-direction:row}.list-group-horizontal-xxl>.list-group-item:first-child:not(:last-child){border-bottom-left-radius:var(--bs-list-group-border-radius);border-top-right-radius:0}.list-group-horizontal-xxl>.list-group-item:last-child:not(:first-child){border-top-right-radius:var(--bs-list-group-border-radius);border-bottom-left-radius:0}.list-group-horizontal-xxl>.list-group-item.active{margin-top:0}.list-group-horizontal-xxl>.list-group-item+.list-group-item{border-top-width:var(--bs-list-group-border-width);border-left-width:0}.list-group-horizontal-xxl>.list-group-item+.list-group-item.active{margin-left:calc(-1 * var(--bs-list-group-border-width));border-left-width:var(--bs-list-group-border-width)}}.list-group-flush{border-radius:0}.list-group-flush>.list-group-item{border-width:0 0 var(--bs-list-group-border-width)}.list-group-flush>.list-group-item:last-child{border-bottom-width:0}.list-group-item-default{color:#595a5c;background-color:#f8f9fa}.list-group-item-default.list-group-item-action:hover,.list-group-item-default.list-group-item-action:focus{color:#595a5c;background-color:#dfe0e1}.list-group-item-default.list-group-item-action.active{color:#fff;background-color:#595a5c;border-color:#595a5c}.list-group-item-primary{color:#084298;background-color:#cfe2ff}.list-group-item-primary.list-group-item-action:hover,.list-group-item-primary.list-group-item-action:focus{color:#084298;background-color:#bacbe6}.list-group-item-primary.list-group-item-action.active{color:#fff;background-color:#084298;border-color:#084298}.list-group-item-secondary{color:#41464b;background-color:#e2e3e5}.list-group-item-secondary.list-group-item-action:hover,.list-group-item-secondary.list-group-item-action:focus{color:#41464b;background-color:#cbccce}.list-group-item-secondary.list-group-item-action.active{color:#fff;background-color:#41464b;border-color:#41464b}.list-group-item-success{color:#0f5132;background-color:#d1e7dd}.list-group-item-success.list-group-item-action:hover,.list-group-item-success.list-group-item-action:focus{color:#0f5132;background-color:#bcd0c7}.list-group-item-success.list-group-item-action.active{color:#fff;background-color:#0f5132;border-color:#0f5132}.list-group-item-info{color:#055160;background-color:#cff4fc}.list-group-item-info.list-group-item-action:hover,.list-group-item-info.list-group-item-action:focus{color:#055160;background-color:#badce3}.list-group-item-info.list-group-item-action.active{color:#fff;background-color:#055160;border-color:#055160}.list-group-item-warning{color:#664d03;background-color:#fff3cd}.list-group-item-warning.list-group-item-action:hover,.list-group-item-warning.list-group-item-action:focus{color:#664d03;background-color:#e6dbb9}.list-group-item-warning.list-group-item-action.active{color:#fff;background-color:#664d03;border-color:#664d03}.list-group-item-danger{color:#842029;background-color:#f8d7da}.list-group-item-danger.list-group-item-action:hover,.list-group-item-danger.list-group-item-action:focus{color:#842029;background-color:#dfc2c4}.list-group-item-danger.list-group-item-action.active{color:#fff;background-color:#842029;border-color:#842029}.list-group-item-light{color:#636464;background-color:#fefefe}.list-group-item-light.list-group-item-action:hover,.list-group-item-light.list-group-item-action:focus{color:#636464;background-color:#e5e5e5}.list-group-item-light.list-group-item-action.active{color:#fff;background-color:#636464;border-color:#636464}.list-group-item-dark{color:#141619;background-color:#d3d3d4}.list-group-item-dark.list-group-item-action:hover,.list-group-item-dark.list-group-item-action:focus{color:#141619;background-color:#bebebf}.list-group-item-dark.list-group-item-action.active{color:#fff;background-color:#141619;border-color:#141619}.btn-close{box-sizing:content-box;width:1em;height:1em;padding:.25em .25em;color:#000;background:transparent url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23000'%3e%3cpath d='M.293.293a1 1 0 0 1 1.414 0L8 6.586 14.293.293a1 1 0 1 1 1.414 1.414L9.414 8l6.293 6.293a1 1 0 0 1-1.414 1.414L8 9.414l-6.293 6.293a1 1 0 0 1-1.414-1.414L6.586 8 .293 1.707a1 1 0 0 1 0-1.414z'/%3e%3c/svg%3e") center/1em auto no-repeat;border:0;border-radius:.375rem;opacity:.5}.btn-close:hover{color:#000;text-decoration:none;opacity:.75}.btn-close:focus{outline:0;box-shadow:0 0 0 .25rem rgba(13,110,253,0.25);opacity:1}.btn-close:disabled,.btn-close.disabled{pointer-events:none;user-select:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;-o-user-select:none;opacity:.25}.btn-close-white{filter:invert(1) grayscale(100%) brightness(200%)}.toast{--bs-toast-zindex: 1090;--bs-toast-padding-x: .75rem;--bs-toast-padding-y: .5rem;--bs-toast-spacing: 1.5rem;--bs-toast-max-width: 350px;--bs-toast-font-size:.875rem;--bs-toast-color: ;--bs-toast-bg: rgba(255,255,255,0.85);--bs-toast-border-width: 1px;--bs-toast-border-color: var(--bs-border-color-translucent);--bs-toast-border-radius: .375rem;--bs-toast-box-shadow: 0 0.5rem 1rem rgba(0,0,0,0.15);--bs-toast-header-color: #6c757d;--bs-toast-header-bg: rgba(255,255,255,0.85);--bs-toast-header-border-color: rgba(0,0,0,0.05);width:var(--bs-toast-max-width);max-width:100%;font-size:var(--bs-toast-font-size);color:var(--bs-toast-color);pointer-events:auto;background-color:var(--bs-toast-bg);background-clip:padding-box;border:var(--bs-toast-border-width) solid var(--bs-toast-border-color);box-shadow:var(--bs-toast-box-shadow);border-radius:var(--bs-toast-border-radius)}.toast.showing{opacity:0}.toast:not(.show):not(.in){display:none}.toast-container{--bs-toast-zindex: 1090;position:absolute;z-index:var(--bs-toast-zindex);width:max-content;width:-webkit-max-content;width:-moz-max-content;width:-ms-max-content;width:-o-max-content;max-width:100%;pointer-events:none}.toast-container>:not(:last-child){margin-bottom:var(--bs-toast-spacing)}.toast-header{display:flex;display:-webkit-flex;align-items:center;-webkit-align-items:center;padding:var(--bs-toast-padding-y) var(--bs-toast-padding-x);color:var(--bs-toast-header-color);background-color:var(--bs-toast-header-bg);background-clip:padding-box;border-bottom:var(--bs-toast-border-width) solid var(--bs-toast-header-border-color);border-top-left-radius:calc(var(--bs-toast-border-radius) - var(--bs-toast-border-width));border-top-right-radius:calc(var(--bs-toast-border-radius) - var(--bs-toast-border-width))}.toast-header .btn-close{margin-right:calc(-.5 * var(--bs-toast-padding-x));margin-left:var(--bs-toast-padding-x)}.toast-body{padding:var(--bs-toast-padding-x);word-wrap:break-word}.modal{--bs-modal-zindex: 1055;--bs-modal-width: 500px;--bs-modal-padding: 1rem;--bs-modal-margin: .5rem;--bs-modal-color: ;--bs-modal-bg: #fff;--bs-modal-border-color: var(--bs-border-color-translucent);--bs-modal-border-width: 1px;--bs-modal-border-radius: .5rem;--bs-modal-box-shadow: 0 0.125rem 0.25rem rgba(0,0,0,0.075);--bs-modal-inner-border-radius: calc(.5rem - 1px);--bs-modal-header-padding-x: 1rem;--bs-modal-header-padding-y: 1rem;--bs-modal-header-padding: 1rem 1rem;--bs-modal-header-border-color: var(--bs-border-color);--bs-modal-header-border-width: 1px;--bs-modal-title-line-height: 1.5;--bs-modal-footer-gap: .5rem;--bs-modal-footer-bg: ;--bs-modal-footer-border-color: var(--bs-border-color);--bs-modal-footer-border-width: 1px;position:fixed;top:0;left:0;z-index:var(--bs-modal-zindex);display:none;width:100%;height:100%;overflow-x:hidden;overflow-y:auto;outline:0}.modal-dialog{position:relative;width:auto;margin:var(--bs-modal-margin);pointer-events:none}.modal.fade .modal-dialog{transition:transform 0.3s ease-out;transform:translate(0, -50px)}@media (prefers-reduced-motion: reduce){.modal.fade .modal-dialog{transition:none}}.modal.show .modal-dialog,.modal.in .modal-dialog{transform:none}.modal.modal-static .modal-dialog{transform:scale(1.02)}.modal-dialog-scrollable{height:calc(100% - var(--bs-modal-margin) * 2)}.modal-dialog-scrollable .modal-content{max-height:100%;overflow:hidden}.modal-dialog-scrollable .modal-body{overflow-y:auto}.modal-dialog-centered{display:flex;display:-webkit-flex;align-items:center;-webkit-align-items:center;min-height:calc(100% - var(--bs-modal-margin) * 2)}.modal-content{position:relative;display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;width:100%;color:var(--bs-modal-color);pointer-events:auto;background-color:var(--bs-modal-bg);background-clip:padding-box;border:var(--bs-modal-border-width) solid var(--bs-modal-border-color);border-radius:var(--bs-modal-border-radius);outline:0}.modal-backdrop{--bs-backdrop-zindex: 1050;--bs-backdrop-bg: #000;--bs-backdrop-opacity: .5;position:fixed;top:0;left:0;z-index:var(--bs-backdrop-zindex);width:100vw;height:100vh;background-color:var(--bs-backdrop-bg)}.modal-backdrop.fade{opacity:0}.modal-backdrop.show,.modal-backdrop.in{opacity:var(--bs-backdrop-opacity)}.modal-header{display:flex;display:-webkit-flex;flex-shrink:0;-webkit-flex-shrink:0;align-items:center;-webkit-align-items:center;justify-content:space-between;-webkit-justify-content:space-between;padding:var(--bs-modal-header-padding);border-bottom:var(--bs-modal-header-border-width) solid var(--bs-modal-header-border-color);border-top-left-radius:var(--bs-modal-inner-border-radius);border-top-right-radius:var(--bs-modal-inner-border-radius)}.modal-header .btn-close{padding:calc(var(--bs-modal-header-padding-y) * .5) calc(var(--bs-modal-header-padding-x) * .5);margin:calc(-.5 * var(--bs-modal-header-padding-y)) calc(-.5 * var(--bs-modal-header-padding-x)) calc(-.5 * var(--bs-modal-header-padding-y)) auto}.modal-title{margin-bottom:0;line-height:var(--bs-modal-title-line-height)}.modal-body{position:relative;flex:1 1 auto;-webkit-flex:1 1 auto;padding:var(--bs-modal-padding)}.modal-footer{display:flex;display:-webkit-flex;flex-shrink:0;-webkit-flex-shrink:0;flex-wrap:wrap;-webkit-flex-wrap:wrap;align-items:center;-webkit-align-items:center;justify-content:flex-end;-webkit-justify-content:flex-end;padding:calc(var(--bs-modal-padding) - var(--bs-modal-footer-gap) * .5);background-color:var(--bs-modal-footer-bg);border-top:var(--bs-modal-footer-border-width) solid var(--bs-modal-footer-border-color);border-bottom-right-radius:var(--bs-modal-inner-border-radius);border-bottom-left-radius:var(--bs-modal-inner-border-radius)}.modal-footer>*{margin:calc(var(--bs-modal-footer-gap) * .5)}@media (min-width: 576px){.modal{--bs-modal-margin: 1.75rem;--bs-modal-box-shadow: 0 0.5rem 1rem rgba(0,0,0,0.15)}.modal-dialog{max-width:var(--bs-modal-width);margin-right:auto;margin-left:auto}.modal-sm{--bs-modal-width: 300px}}@media (min-width: 992px){.modal-lg,.modal-xl{--bs-modal-width: 800px}}@media (min-width: 1200px){.modal-xl{--bs-modal-width: 1140px}}.modal-fullscreen{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen .modal-header,.modal-fullscreen .modal-footer{border-radius:0}.modal-fullscreen .modal-body{overflow-y:auto}@media (max-width: 575.98px){.modal-fullscreen-sm-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-sm-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-sm-down .modal-header,.modal-fullscreen-sm-down .modal-footer{border-radius:0}.modal-fullscreen-sm-down .modal-body{overflow-y:auto}}@media (max-width: 767.98px){.modal-fullscreen-md-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-md-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-md-down .modal-header,.modal-fullscreen-md-down .modal-footer{border-radius:0}.modal-fullscreen-md-down .modal-body{overflow-y:auto}}@media (max-width: 991.98px){.modal-fullscreen-lg-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-lg-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-lg-down .modal-header,.modal-fullscreen-lg-down .modal-footer{border-radius:0}.modal-fullscreen-lg-down .modal-body{overflow-y:auto}}@media (max-width: 1199.98px){.modal-fullscreen-xl-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-xl-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-xl-down .modal-header,.modal-fullscreen-xl-down .modal-footer{border-radius:0}.modal-fullscreen-xl-down .modal-body{overflow-y:auto}}@media (max-width: 1399.98px){.modal-fullscreen-xxl-down{width:100vw;max-width:none;height:100%;margin:0}.modal-fullscreen-xxl-down .modal-content{height:100%;border:0;border-radius:0}.modal-fullscreen-xxl-down .modal-header,.modal-fullscreen-xxl-down .modal-footer{border-radius:0}.modal-fullscreen-xxl-down .modal-body{overflow-y:auto}}.tooltip{--bs-tooltip-zindex: 1080;--bs-tooltip-max-width: 200px;--bs-tooltip-padding-x: .5rem;--bs-tooltip-padding-y: .25rem;--bs-tooltip-margin: ;--bs-tooltip-font-size:.875rem;--bs-tooltip-color: #fff;--bs-tooltip-bg: #000;--bs-tooltip-border-radius: .375rem;--bs-tooltip-opacity: .9;--bs-tooltip-arrow-width: .8rem;--bs-tooltip-arrow-height: .4rem;z-index:var(--bs-tooltip-zindex);display:block;padding:var(--bs-tooltip-arrow-height);margin:var(--bs-tooltip-margin);font-family:var(--bs-font-sans-serif);font-style:normal;font-weight:400;line-height:1.5;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;white-space:normal;word-spacing:normal;line-break:auto;font-size:var(--bs-tooltip-font-size);word-wrap:break-word;opacity:0}.tooltip.show,.tooltip.in{opacity:var(--bs-tooltip-opacity)}.tooltip .tooltip-arrow{display:block;width:var(--bs-tooltip-arrow-width);height:var(--bs-tooltip-arrow-height)}.tooltip .tooltip-arrow::before{position:absolute;content:"";border-color:transparent;border-style:solid}.bs-tooltip-top .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^="top"] .tooltip-arrow{bottom:0}.bs-tooltip-top .tooltip-arrow::before,.bs-tooltip-auto[data-popper-placement^="top"] .tooltip-arrow::before{top:-1px;border-width:var(--bs-tooltip-arrow-height) calc(var(--bs-tooltip-arrow-width) * .5) 0;border-top-color:var(--bs-tooltip-bg)}.bs-tooltip-end .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^="right"] .tooltip-arrow{left:0;width:var(--bs-tooltip-arrow-height);height:var(--bs-tooltip-arrow-width)}.bs-tooltip-end .tooltip-arrow::before,.bs-tooltip-auto[data-popper-placement^="right"] .tooltip-arrow::before{right:-1px;border-width:calc(var(--bs-tooltip-arrow-width) * .5) var(--bs-tooltip-arrow-height) calc(var(--bs-tooltip-arrow-width) * .5) 0;border-right-color:var(--bs-tooltip-bg)}.bs-tooltip-bottom .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^="bottom"] .tooltip-arrow{top:0}.bs-tooltip-bottom .tooltip-arrow::before,.bs-tooltip-auto[data-popper-placement^="bottom"] .tooltip-arrow::before{bottom:-1px;border-width:0 calc(var(--bs-tooltip-arrow-width) * .5) var(--bs-tooltip-arrow-height);border-bottom-color:var(--bs-tooltip-bg)}.bs-tooltip-start .tooltip-arrow,.bs-tooltip-auto[data-popper-placement^="left"] .tooltip-arrow{right:0;width:var(--bs-tooltip-arrow-height);height:var(--bs-tooltip-arrow-width)}.bs-tooltip-start .tooltip-arrow::before,.bs-tooltip-auto[data-popper-placement^="left"] .tooltip-arrow::before{left:-1px;border-width:calc(var(--bs-tooltip-arrow-width) * .5) 0 calc(var(--bs-tooltip-arrow-width) * .5) var(--bs-tooltip-arrow-height);border-left-color:var(--bs-tooltip-bg)}.tooltip-inner{max-width:var(--bs-tooltip-max-width);padding:var(--bs-tooltip-padding-y) var(--bs-tooltip-padding-x);color:var(--bs-tooltip-color);text-align:center;background-color:var(--bs-tooltip-bg);border-radius:var(--bs-tooltip-border-radius)}.popover{--bs-popover-zindex: 1070;--bs-popover-max-width: 276px;--bs-popover-font-size:.875rem;--bs-popover-bg: #fff;--bs-popover-border-width: 1px;--bs-popover-border-color: var(--bs-border-color-translucent);--bs-popover-border-radius: .5rem;--bs-popover-inner-border-radius: calc(.5rem - 1px);--bs-popover-box-shadow: 0 0.5rem 1rem rgba(0,0,0,0.15);--bs-popover-header-padding-x: 1rem;--bs-popover-header-padding-y: .5rem;--bs-popover-header-font-size:1rem;--bs-popover-header-color: ;--bs-popover-header-bg: #f0f0f0;--bs-popover-body-padding-x: 1rem;--bs-popover-body-padding-y: 1rem;--bs-popover-body-color: #212529;--bs-popover-arrow-width: 1rem;--bs-popover-arrow-height: .5rem;--bs-popover-arrow-border: var(--bs-popover-border-color);z-index:var(--bs-popover-zindex);display:block;max-width:var(--bs-popover-max-width);font-family:var(--bs-font-sans-serif);font-style:normal;font-weight:400;line-height:1.5;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;white-space:normal;word-spacing:normal;line-break:auto;font-size:var(--bs-popover-font-size);word-wrap:break-word;background-color:var(--bs-popover-bg);background-clip:padding-box;border:var(--bs-popover-border-width) solid var(--bs-popover-border-color);border-radius:var(--bs-popover-border-radius)}.popover .popover-arrow{display:block;width:var(--bs-popover-arrow-width);height:var(--bs-popover-arrow-height)}.popover .popover-arrow::before,.popover .popover-arrow::after{position:absolute;display:block;content:"";border-color:transparent;border-style:solid;border-width:0}.bs-popover-top>.popover-arrow,.bs-popover-auto[data-popper-placement^="top"]>.popover-arrow{bottom:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width))}.bs-popover-top>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="top"]>.popover-arrow::before,.bs-popover-top>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="top"]>.popover-arrow::after{border-width:var(--bs-popover-arrow-height) calc(var(--bs-popover-arrow-width) * .5) 0}.bs-popover-top>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="top"]>.popover-arrow::before{bottom:0;border-top-color:var(--bs-popover-arrow-border)}.bs-popover-top>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="top"]>.popover-arrow::after{bottom:var(--bs-popover-border-width);border-top-color:var(--bs-popover-bg)}.bs-popover-end>.popover-arrow,.bs-popover-auto[data-popper-placement^="right"]>.popover-arrow{left:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width));width:var(--bs-popover-arrow-height);height:var(--bs-popover-arrow-width)}.bs-popover-end>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="right"]>.popover-arrow::before,.bs-popover-end>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="right"]>.popover-arrow::after{border-width:calc(var(--bs-popover-arrow-width) * .5) var(--bs-popover-arrow-height) calc(var(--bs-popover-arrow-width) * .5) 0}.bs-popover-end>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="right"]>.popover-arrow::before{left:0;border-right-color:var(--bs-popover-arrow-border)}.bs-popover-end>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="right"]>.popover-arrow::after{left:var(--bs-popover-border-width);border-right-color:var(--bs-popover-bg)}.bs-popover-bottom>.popover-arrow,.bs-popover-auto[data-popper-placement^="bottom"]>.popover-arrow{top:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width))}.bs-popover-bottom>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="bottom"]>.popover-arrow::before,.bs-popover-bottom>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="bottom"]>.popover-arrow::after{border-width:0 calc(var(--bs-popover-arrow-width) * .5) var(--bs-popover-arrow-height)}.bs-popover-bottom>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="bottom"]>.popover-arrow::before{top:0;border-bottom-color:var(--bs-popover-arrow-border)}.bs-popover-bottom>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="bottom"]>.popover-arrow::after{top:var(--bs-popover-border-width);border-bottom-color:var(--bs-popover-bg)}.bs-popover-bottom .popover-header::before,.bs-popover-auto[data-popper-placement^="bottom"] .popover-header::before{position:absolute;top:0;left:50%;display:block;width:var(--bs-popover-arrow-width);margin-left:calc(-.5 * var(--bs-popover-arrow-width));content:"";border-bottom:var(--bs-popover-border-width) solid var(--bs-popover-header-bg)}.bs-popover-start>.popover-arrow,.bs-popover-auto[data-popper-placement^="left"]>.popover-arrow{right:calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width));width:var(--bs-popover-arrow-height);height:var(--bs-popover-arrow-width)}.bs-popover-start>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="left"]>.popover-arrow::before,.bs-popover-start>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="left"]>.popover-arrow::after{border-width:calc(var(--bs-popover-arrow-width) * .5) 0 calc(var(--bs-popover-arrow-width) * .5) var(--bs-popover-arrow-height)}.bs-popover-start>.popover-arrow::before,.bs-popover-auto[data-popper-placement^="left"]>.popover-arrow::before{right:0;border-left-color:var(--bs-popover-arrow-border)}.bs-popover-start>.popover-arrow::after,.bs-popover-auto[data-popper-placement^="left"]>.popover-arrow::after{right:var(--bs-popover-border-width);border-left-color:var(--bs-popover-bg)}.popover-header{padding:var(--bs-popover-header-padding-y) var(--bs-popover-header-padding-x);margin-bottom:0;font-size:var(--bs-popover-header-font-size);color:var(--bs-popover-header-color);background-color:var(--bs-popover-header-bg);border-bottom:var(--bs-popover-border-width) solid var(--bs-popover-border-color);border-top-left-radius:var(--bs-popover-inner-border-radius);border-top-right-radius:var(--bs-popover-inner-border-radius)}.popover-header:empty{display:none}.popover-body{padding:var(--bs-popover-body-padding-y) var(--bs-popover-body-padding-x);color:var(--bs-popover-body-color)}.carousel{position:relative}.carousel.pointer-event{touch-action:pan-y;-webkit-touch-action:pan-y;-moz-touch-action:pan-y;-ms-touch-action:pan-y;-o-touch-action:pan-y}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner::after{display:block;clear:both;content:""}.carousel-item{position:relative;display:none;float:left;width:100%;margin-right:-100%;backface-visibility:hidden;-webkit-backface-visibility:hidden;-moz-backface-visibility:hidden;-ms-backface-visibility:hidden;-o-backface-visibility:hidden;transition:transform .6s ease-in-out}@media (prefers-reduced-motion: reduce){.carousel-item{transition:none}}.carousel-item.active,.carousel-item-next,.carousel-item-prev{display:block}.carousel-item-next:not(.carousel-item-start),.active.carousel-item-end{transform:translateX(100%)}.carousel-item-prev:not(.carousel-item-end),.active.carousel-item-start{transform:translateX(-100%)}.carousel-fade .carousel-item{opacity:0;transition-property:opacity;transform:none}.carousel-fade .carousel-item.active,.carousel-fade .carousel-item-next.carousel-item-start,.carousel-fade .carousel-item-prev.carousel-item-end{z-index:1;opacity:1}.carousel-fade .active.carousel-item-start,.carousel-fade .active.carousel-item-end{z-index:0;opacity:0;transition:opacity 0s .6s}@media (prefers-reduced-motion: reduce){.carousel-fade .active.carousel-item-start,.carousel-fade .active.carousel-item-end{transition:none}}.carousel-control-prev,.carousel-control-next{position:absolute;top:0;bottom:0;z-index:1;display:flex;display:-webkit-flex;align-items:center;-webkit-align-items:center;justify-content:center;-webkit-justify-content:center;width:15%;padding:0;color:#fff;text-align:center;background:none;border:0;opacity:.5;transition:opacity 0.15s ease}@media (prefers-reduced-motion: reduce){.carousel-control-prev,.carousel-control-next{transition:none}}.carousel-control-prev:hover,.carousel-control-prev:focus,.carousel-control-next:hover,.carousel-control-next:focus{color:#fff;text-decoration:none;outline:0;opacity:.9}.carousel-control-prev{left:0}.carousel-control-next{right:0}.carousel-control-prev-icon,.carousel-control-next-icon{display:inline-block;width:2rem;height:2rem;background-repeat:no-repeat;background-position:50%;background-size:100% 100%}.carousel-control-prev-icon{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23fff'%3e%3cpath d='M11.354 1.646a.5.5 0 0 1 0 .708L5.707 8l5.647 5.646a.5.5 0 0 1-.708.708l-6-6a.5.5 0 0 1 0-.708l6-6a.5.5 0 0 1 .708 0z'/%3e%3c/svg%3e")}.carousel-control-next-icon{background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23fff'%3e%3cpath d='M4.646 1.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1 0 .708l-6 6a.5.5 0 0 1-.708-.708L10.293 8 4.646 2.354a.5.5 0 0 1 0-.708z'/%3e%3c/svg%3e")}.carousel-indicators{position:absolute;right:0;bottom:0;left:0;z-index:2;display:flex;display:-webkit-flex;justify-content:center;-webkit-justify-content:center;padding:0;margin-right:15%;margin-bottom:1rem;margin-left:15%;list-style:none}.carousel-indicators [data-bs-target]{box-sizing:content-box;flex:0 1 auto;-webkit-flex:0 1 auto;width:30px;height:3px;padding:0;margin-right:3px;margin-left:3px;text-indent:-999px;cursor:pointer;background-color:#fff;background-clip:padding-box;border:0;border-top:10px solid transparent;border-bottom:10px solid transparent;opacity:.5;transition:opacity 0.6s ease}@media (prefers-reduced-motion: reduce){.carousel-indicators [data-bs-target]{transition:none}}.carousel-indicators .active{opacity:1}.carousel-caption{position:absolute;right:15%;bottom:1.25rem;left:15%;padding-top:1.25rem;padding-bottom:1.25rem;color:#fff;text-align:center}.carousel-dark .carousel-control-prev-icon,.carousel-dark .carousel-control-next-icon{filter:invert(1) grayscale(100)}.carousel-dark .carousel-indicators [data-bs-target]{background-color:#000}.carousel-dark .carousel-caption{color:#000}.spinner-grow,.spinner-border{display:inline-block;width:var(--bs-spinner-width);height:var(--bs-spinner-height);vertical-align:var(--bs-spinner-vertical-align);border-radius:50%;animation:var(--bs-spinner-animation-speed) linear infinite var(--bs-spinner-animation-name)}@keyframes spinner-border{to{transform:rotate(360deg) /* rtl:ignore */}}.spinner-border{--bs-spinner-width: 2rem;--bs-spinner-height: 2rem;--bs-spinner-vertical-align: -.125em;--bs-spinner-border-width: .25em;--bs-spinner-animation-speed: .75s;--bs-spinner-animation-name: spinner-border;border:var(--bs-spinner-border-width) solid currentcolor;border-right-color:transparent}.spinner-border-sm{--bs-spinner-width: 1rem;--bs-spinner-height: 1rem;--bs-spinner-border-width: .2em}@keyframes spinner-grow{0%{transform:scale(0)}50%{opacity:1;transform:none}}.spinner-grow{--bs-spinner-width: 2rem;--bs-spinner-height: 2rem;--bs-spinner-vertical-align: -.125em;--bs-spinner-animation-speed: .75s;--bs-spinner-animation-name: spinner-grow;background-color:currentcolor;opacity:0}.spinner-grow-sm{--bs-spinner-width: 1rem;--bs-spinner-height: 1rem}@media (prefers-reduced-motion: reduce){.spinner-border,.spinner-grow{--bs-spinner-animation-speed: 1.5s}}.offcanvas,.offcanvas-xxl,.offcanvas-xl,.offcanvas-lg,.offcanvas-md,.offcanvas-sm{--bs-offcanvas-zindex: 1045;--bs-offcanvas-width: 400px;--bs-offcanvas-height: 30vh;--bs-offcanvas-padding-x: 1rem;--bs-offcanvas-padding-y: 1rem;--bs-offcanvas-color: ;--bs-offcanvas-bg: #fff;--bs-offcanvas-border-width: 1px;--bs-offcanvas-border-color: var(--bs-border-color-translucent);--bs-offcanvas-box-shadow: 0 0.125rem 0.25rem rgba(0,0,0,0.075)}@media (max-width: 575.98px){.offcanvas-sm{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:transform .3s ease-in-out}}@media (max-width: 575.98px) and (prefers-reduced-motion: reduce){.offcanvas-sm{transition:none}}@media (max-width: 575.98px){.offcanvas-sm.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(-100%)}.offcanvas-sm.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(100%)}.offcanvas-sm.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-sm.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-sm.showing,.offcanvas-sm.show:not(.hiding),.offcanvas-sm.in:not(.hiding){transform:none}.offcanvas-sm.showing,.offcanvas-sm.hiding,.offcanvas-sm.show,.offcanvas-sm.in{visibility:visible}}@media (min-width: 576px){.offcanvas-sm{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent !important}.offcanvas-sm .offcanvas-header{display:none}.offcanvas-sm .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible;background-color:transparent !important}}@media (max-width: 767.98px){.offcanvas-md{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:transform .3s ease-in-out}}@media (max-width: 767.98px) and (prefers-reduced-motion: reduce){.offcanvas-md{transition:none}}@media (max-width: 767.98px){.offcanvas-md.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(-100%)}.offcanvas-md.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(100%)}.offcanvas-md.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-md.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-md.showing,.offcanvas-md.show:not(.hiding),.offcanvas-md.in:not(.hiding){transform:none}.offcanvas-md.showing,.offcanvas-md.hiding,.offcanvas-md.show,.offcanvas-md.in{visibility:visible}}@media (min-width: 768px){.offcanvas-md{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent !important}.offcanvas-md .offcanvas-header{display:none}.offcanvas-md .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible;background-color:transparent !important}}@media (max-width: 991.98px){.offcanvas-lg{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:transform .3s ease-in-out}}@media (max-width: 991.98px) and (prefers-reduced-motion: reduce){.offcanvas-lg{transition:none}}@media (max-width: 991.98px){.offcanvas-lg.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(-100%)}.offcanvas-lg.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(100%)}.offcanvas-lg.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-lg.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-lg.showing,.offcanvas-lg.show:not(.hiding),.offcanvas-lg.in:not(.hiding){transform:none}.offcanvas-lg.showing,.offcanvas-lg.hiding,.offcanvas-lg.show,.offcanvas-lg.in{visibility:visible}}@media (min-width: 992px){.offcanvas-lg{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent !important}.offcanvas-lg .offcanvas-header{display:none}.offcanvas-lg .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible;background-color:transparent !important}}@media (max-width: 1199.98px){.offcanvas-xl{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:transform .3s ease-in-out}}@media (max-width: 1199.98px) and (prefers-reduced-motion: reduce){.offcanvas-xl{transition:none}}@media (max-width: 1199.98px){.offcanvas-xl.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(-100%)}.offcanvas-xl.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(100%)}.offcanvas-xl.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-xl.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-xl.showing,.offcanvas-xl.show:not(.hiding),.offcanvas-xl.in:not(.hiding){transform:none}.offcanvas-xl.showing,.offcanvas-xl.hiding,.offcanvas-xl.show,.offcanvas-xl.in{visibility:visible}}@media (min-width: 1200px){.offcanvas-xl{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent !important}.offcanvas-xl .offcanvas-header{display:none}.offcanvas-xl .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible;background-color:transparent !important}}@media (max-width: 1399.98px){.offcanvas-xxl{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:transform .3s ease-in-out}}@media (max-width: 1399.98px) and (prefers-reduced-motion: reduce){.offcanvas-xxl{transition:none}}@media (max-width: 1399.98px){.offcanvas-xxl.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(-100%)}.offcanvas-xxl.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(100%)}.offcanvas-xxl.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas-xxl.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas-xxl.showing,.offcanvas-xxl.show:not(.hiding),.offcanvas-xxl.in:not(.hiding){transform:none}.offcanvas-xxl.showing,.offcanvas-xxl.hiding,.offcanvas-xxl.show,.offcanvas-xxl.in{visibility:visible}}@media (min-width: 1400px){.offcanvas-xxl{--bs-offcanvas-height: auto;--bs-offcanvas-border-width: 0;background-color:transparent !important}.offcanvas-xxl .offcanvas-header{display:none}.offcanvas-xxl .offcanvas-body{display:flex;display:-webkit-flex;flex-grow:0;-webkit-flex-grow:0;padding:0;overflow-y:visible;background-color:transparent !important}}.offcanvas{position:fixed;bottom:0;z-index:var(--bs-offcanvas-zindex);display:flex;display:-webkit-flex;flex-direction:column;-webkit-flex-direction:column;max-width:100%;color:var(--bs-offcanvas-color);visibility:hidden;background-color:var(--bs-offcanvas-bg);background-clip:padding-box;outline:0;transition:transform .3s ease-in-out}@media (prefers-reduced-motion: reduce){.offcanvas{transition:none}}.offcanvas.offcanvas-start{top:0;left:0;width:var(--bs-offcanvas-width);border-right:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(-100%)}.offcanvas.offcanvas-end{top:0;right:0;width:var(--bs-offcanvas-width);border-left:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateX(100%)}.offcanvas.offcanvas-top{top:0;right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-bottom:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(-100%)}.offcanvas.offcanvas-bottom{right:0;left:0;height:var(--bs-offcanvas-height);max-height:100%;border-top:var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);transform:translateY(100%)}.offcanvas.showing,.offcanvas.show:not(.hiding),.offcanvas.in:not(.hiding){transform:none}.offcanvas.showing,.offcanvas.hiding,.offcanvas.show,.offcanvas.in{visibility:visible}.offcanvas-backdrop{position:fixed;top:0;left:0;z-index:1040;width:100vw;height:100vh;background-color:#000}.offcanvas-backdrop.fade{opacity:0}.offcanvas-backdrop.show,.offcanvas-backdrop.in{opacity:.5}.offcanvas-header{display:flex;display:-webkit-flex;align-items:center;-webkit-align-items:center;justify-content:space-between;-webkit-justify-content:space-between;padding:var(--bs-offcanvas-padding-y) var(--bs-offcanvas-padding-x)}.offcanvas-header .btn-close{padding:calc(var(--bs-offcanvas-padding-y) * .5) calc(var(--bs-offcanvas-padding-x) * .5);margin-top:calc(-.5 * var(--bs-offcanvas-padding-y));margin-right:calc(-.5 * var(--bs-offcanvas-padding-x));margin-bottom:calc(-.5 * var(--bs-offcanvas-padding-y))}.offcanvas-title{margin-bottom:0;line-height:1.5}.offcanvas-body{flex-grow:1;-webkit-flex-grow:1;padding:var(--bs-offcanvas-padding-y) var(--bs-offcanvas-padding-x);overflow-y:auto}.placeholder{display:inline-block;min-height:1em;vertical-align:middle;cursor:wait;background-color:currentcolor;opacity:.5}.placeholder.btn::before{display:inline-block;content:""}.placeholder-xs{min-height:.6em}.placeholder-sm{min-height:.8em}.placeholder-lg{min-height:1.2em}.placeholder-glow .placeholder{animation:placeholder-glow 2s ease-in-out infinite}@keyframes placeholder-glow{50%{opacity:.2}}.placeholder-wave{mask-image:linear-gradient(130deg, #000 55%, rgba(0,0,0,0.8) 75%, #000 95%);-webkit-mask-image:linear-gradient(130deg, #000 55%, rgba(0,0,0,0.8) 75%, #000 95%);mask-size:200% 100%;-webkit-mask-size:200% 100%;animation:placeholder-wave 2s linear infinite}@keyframes placeholder-wave{100%{mask-position:-200% 0%;-webkit-mask-position:-200% 0%}}.clearfix::after{display:block;clear:both;content:""}.text-bg-default{color:#000 !important;background-color:RGBA(222,226,230, var(--bs-bg-opacity, 1)) !important}.text-bg-primary{color:#fff !important;background-color:RGBA(13,110,253, var(--bs-bg-opacity, 1)) !important}.text-bg-secondary{color:#fff !important;background-color:RGBA(108,117,125, var(--bs-bg-opacity, 1)) !important}.text-bg-success{color:#fff !important;background-color:RGBA(25,135,84, var(--bs-bg-opacity, 1)) !important}.text-bg-info{color:#000 !important;background-color:RGBA(13,202,240, var(--bs-bg-opacity, 1)) !important}.text-bg-warning{color:#000 !important;background-color:RGBA(255,193,7, var(--bs-bg-opacity, 1)) !important}.text-bg-danger{color:#fff !important;background-color:RGBA(220,53,69, var(--bs-bg-opacity, 1)) !important}.text-bg-light{color:#000 !important;background-color:RGBA(248,249,250, var(--bs-bg-opacity, 1)) !important}.text-bg-dark{color:#fff !important;background-color:RGBA(33,37,41, var(--bs-bg-opacity, 1)) !important}.link-default{color:#dee2e6 !important}.link-default:hover,.link-default:focus{color:#e5e8eb !important}.link-primary{color:#0d6efd !important}.link-primary:hover,.link-primary:focus{color:#0a58ca !important}.link-secondary{color:#6c757d !important}.link-secondary:hover,.link-secondary:focus{color:#565e64 !important}.link-success{color:#198754 !important}.link-success:hover,.link-success:focus{color:#146c43 !important}.link-info{color:#0dcaf0 !important}.link-info:hover,.link-info:focus{color:#3dd5f3 !important}.link-warning{color:#ffc107 !important}.link-warning:hover,.link-warning:focus{color:#ffcd39 !important}.link-danger{color:#dc3545 !important}.link-danger:hover,.link-danger:focus{color:#b02a37 !important}.link-light{color:#f8f9fa !important}.link-light:hover,.link-light:focus{color:#f9fafb !important}.link-dark{color:#212529 !important}.link-dark:hover,.link-dark:focus{color:#1a1e21 !important}.ratio{position:relative;width:100%}.ratio::before{display:block;padding-top:var(--bs-aspect-ratio);content:""}.ratio>*{position:absolute;top:0;left:0;width:100%;height:100%}.ratio-1x1{--bs-aspect-ratio: 100%}.ratio-4x3{--bs-aspect-ratio: calc(3 / 4 * 100%)}.ratio-16x9{--bs-aspect-ratio: calc(9 / 16 * 100%)}.ratio-21x9{--bs-aspect-ratio: calc(9 / 21 * 100%)}.fixed-top,.navbar-fixed-top{position:fixed;top:0;right:0;left:0;z-index:1030}.fixed-bottom,.navbar-fixed-bottom{position:fixed;right:0;bottom:0;left:0;z-index:1030}.sticky-top,.navbar-sticky-top{position:sticky;top:0;z-index:1020}.sticky-bottom{position:sticky;bottom:0;z-index:1020}@media (min-width: 576px){.sticky-sm-top{position:sticky;top:0;z-index:1020}.sticky-sm-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 768px){.sticky-md-top{position:sticky;top:0;z-index:1020}.sticky-md-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 992px){.sticky-lg-top{position:sticky;top:0;z-index:1020}.sticky-lg-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 1200px){.sticky-xl-top{position:sticky;top:0;z-index:1020}.sticky-xl-bottom{position:sticky;bottom:0;z-index:1020}}@media (min-width: 1400px){.sticky-xxl-top{position:sticky;top:0;z-index:1020}.sticky-xxl-bottom{position:sticky;bottom:0;z-index:1020}}.hstack{display:flex;display:-webkit-flex;flex-direction:row;-webkit-flex-direction:row;align-items:center;-webkit-align-items:center;align-self:stretch;-webkit-align-self:stretch}.vstack{display:flex;display:-webkit-flex;flex:1 1 auto;-webkit-flex:1 1 auto;flex-direction:column;-webkit-flex-direction:column;align-self:stretch;-webkit-align-self:stretch}.visually-hidden,.visually-hidden-focusable:not(:focus):not(:focus-within){position:absolute !important;width:1px !important;height:1px !important;padding:0 !important;margin:-1px !important;overflow:hidden !important;clip:rect(0, 0, 0, 0) !important;white-space:nowrap !important;border:0 !important}.stretched-link::after{position:absolute;top:0;right:0;bottom:0;left:0;z-index:1;content:""}.text-truncate{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.vr{display:inline-block;align-self:stretch;-webkit-align-self:stretch;width:1px;min-height:1em;background-color:currentcolor;opacity:.25}.align-baseline{vertical-align:baseline !important}.align-top{vertical-align:top !important}.align-middle{vertical-align:middle !important}.align-bottom{vertical-align:bottom !important}.align-text-bottom{vertical-align:text-bottom !important}.align-text-top{vertical-align:text-top !important}.float-start,.float-left{float:left !important}.float-end,.float-right{float:right !important}.float-none{float:none !important}.opacity-0{opacity:0 !important}.opacity-25{opacity:.25 !important}.opacity-50{opacity:.5 !important}.opacity-75{opacity:.75 !important}.opacity-100{opacity:1 !important}.overflow-auto{overflow:auto !important}.overflow-hidden{overflow:hidden !important}.overflow-visible{overflow:visible !important}.overflow-scroll{overflow:scroll !important}.d-inline{display:inline !important}.d-inline-block{display:inline-block !important}.d-block{display:block !important}.d-grid{display:grid !important}.d-table{display:table !important}.d-table-row{display:table-row !important}.d-table-cell{display:table-cell !important}.d-flex{display:flex !important}.d-inline-flex{display:inline-flex !important}.d-none{display:none !important}.shadow{box-shadow:0 0.5rem 1rem rgba(0,0,0,0.15) !important}.shadow-sm{box-shadow:0 0.125rem 0.25rem rgba(0,0,0,0.075) !important}.shadow-lg{box-shadow:0 1rem 3rem rgba(0,0,0,0.175) !important}.shadow-none{box-shadow:none !important}.position-static{position:static !important}.position-relative{position:relative !important}.position-absolute{position:absolute !important}.position-fixed{position:fixed !important}.position-sticky{position:sticky !important}.top-0{top:0 !important}.top-50{top:50% !important}.top-100{top:100% !important}.bottom-0{bottom:0 !important}.bottom-50{bottom:50% !important}.bottom-100{bottom:100% !important}.start-0{left:0 !important}.start-50{left:50% !important}.start-100{left:100% !important}.end-0{right:0 !important}.end-50{right:50% !important}.end-100{right:100% !important}.translate-middle{transform:translate(-50%, -50%) !important}.translate-middle-x{transform:translateX(-50%) !important}.translate-middle-y{transform:translateY(-50%) !important}.border{border:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color) !important}.border-0{border:0 !important}.border-top{border-top:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color) !important}.border-top-0{border-top:0 !important}.border-end{border-right:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color) !important}.border-end-0{border-right:0 !important}.border-bottom{border-bottom:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color) !important}.border-bottom-0{border-bottom:0 !important}.border-start{border-left:var(--bs-border-width) var(--bs-border-style) var(--bs-border-color) !important}.border-start-0{border-left:0 !important}.border-default{--bs-border-opacity: 1;border-color:rgba(var(--bs-default-rgb), var(--bs-border-opacity)) !important}.border-primary{--bs-border-opacity: 1;border-color:rgba(var(--bs-primary-rgb), var(--bs-border-opacity)) !important}.border-secondary{--bs-border-opacity: 1;border-color:rgba(var(--bs-secondary-rgb), var(--bs-border-opacity)) !important}.border-success{--bs-border-opacity: 1;border-color:rgba(var(--bs-success-rgb), var(--bs-border-opacity)) !important}.border-info{--bs-border-opacity: 1;border-color:rgba(var(--bs-info-rgb), var(--bs-border-opacity)) !important}.border-warning{--bs-border-opacity: 1;border-color:rgba(var(--bs-warning-rgb), var(--bs-border-opacity)) !important}.border-danger{--bs-border-opacity: 1;border-color:rgba(var(--bs-danger-rgb), var(--bs-border-opacity)) !important}.border-light{--bs-border-opacity: 1;border-color:rgba(var(--bs-light-rgb), var(--bs-border-opacity)) !important}.border-dark{--bs-border-opacity: 1;border-color:rgba(var(--bs-dark-rgb), var(--bs-border-opacity)) !important}.border-white{--bs-border-opacity: 1;border-color:rgba(var(--bs-white-rgb), var(--bs-border-opacity)) !important}.border-1{--bs-border-width: 1px}.border-2{--bs-border-width: 2px}.border-3{--bs-border-width: 3px}.border-4{--bs-border-width: 4px}.border-5{--bs-border-width: 5px}.border-opacity-10{--bs-border-opacity: .1}.border-opacity-25{--bs-border-opacity: .25}.border-opacity-50{--bs-border-opacity: .5}.border-opacity-75{--bs-border-opacity: .75}.border-opacity-100{--bs-border-opacity: 1}.w-25{width:25% !important}.w-50{width:50% !important}.w-75{width:75% !important}.w-100{width:100% !important}.w-auto{width:auto !important}.mw-100{max-width:100% !important}.vw-100{width:100vw !important}.min-vw-100{min-width:100vw !important}.h-25{height:25% !important}.h-50{height:50% !important}.h-75{height:75% !important}.h-100{height:100% !important}.h-auto{height:auto !important}.mh-100{max-height:100% !important}.vh-100{height:100vh !important}.min-vh-100{min-height:100vh !important}.flex-fill{flex:1 1 auto !important}.flex-row{flex-direction:row !important}.flex-column{flex-direction:column !important}.flex-row-reverse{flex-direction:row-reverse !important}.flex-column-reverse{flex-direction:column-reverse !important}.flex-grow-0{flex-grow:0 !important}.flex-grow-1{flex-grow:1 !important}.flex-shrink-0{flex-shrink:0 !important}.flex-shrink-1{flex-shrink:1 !important}.flex-wrap{flex-wrap:wrap !important}.flex-nowrap{flex-wrap:nowrap !important}.flex-wrap-reverse{flex-wrap:wrap-reverse !important}.justify-content-start{justify-content:flex-start !important}.justify-content-end{justify-content:flex-end !important}.justify-content-center{justify-content:center !important}.justify-content-between{justify-content:space-between !important}.justify-content-around{justify-content:space-around !important}.justify-content-evenly{justify-content:space-evenly !important}.align-items-start{align-items:flex-start !important}.align-items-end{align-items:flex-end !important}.align-items-center{align-items:center !important}.align-items-baseline{align-items:baseline !important}.align-items-stretch{align-items:stretch !important}.align-content-start{align-content:flex-start !important}.align-content-end{align-content:flex-end !important}.align-content-center{align-content:center !important}.align-content-between{align-content:space-between !important}.align-content-around{align-content:space-around !important}.align-content-stretch{align-content:stretch !important}.align-self-auto{align-self:auto !important}.align-self-start{align-self:flex-start !important}.align-self-end{align-self:flex-end !important}.align-self-center{align-self:center !important}.align-self-baseline{align-self:baseline !important}.align-self-stretch{align-self:stretch !important}.order-first{order:-1 !important}.order-0{order:0 !important}.order-1{order:1 !important}.order-2{order:2 !important}.order-3{order:3 !important}.order-4{order:4 !important}.order-5{order:5 !important}.order-last{order:6 !important}.m-0{margin:0 !important}.m-1{margin:.25rem !important}.m-2{margin:.5rem !important}.m-3{margin:1rem !important}.m-4{margin:1.5rem !important}.m-5{margin:3rem !important}.m-auto{margin:auto !important}.mx-0{margin-right:0 !important;margin-left:0 !important}.mx-1{margin-right:.25rem !important;margin-left:.25rem !important}.mx-2{margin-right:.5rem !important;margin-left:.5rem !important}.mx-3{margin-right:1rem !important;margin-left:1rem !important}.mx-4{margin-right:1.5rem !important;margin-left:1.5rem !important}.mx-5{margin-right:3rem !important;margin-left:3rem !important}.mx-auto{margin-right:auto !important;margin-left:auto !important}.my-0{margin-top:0 !important;margin-bottom:0 !important}.my-1{margin-top:.25rem !important;margin-bottom:.25rem !important}.my-2{margin-top:.5rem !important;margin-bottom:.5rem !important}.my-3{margin-top:1rem !important;margin-bottom:1rem !important}.my-4{margin-top:1.5rem !important;margin-bottom:1.5rem !important}.my-5{margin-top:3rem !important;margin-bottom:3rem !important}.my-auto{margin-top:auto !important;margin-bottom:auto !important}.mt-0{margin-top:0 !important}.mt-1{margin-top:.25rem !important}.mt-2{margin-top:.5rem !important}.mt-3{margin-top:1rem !important}.mt-4{margin-top:1.5rem !important}.mt-5{margin-top:3rem !important}.mt-auto{margin-top:auto !important}.me-0{margin-right:0 !important}.me-1{margin-right:.25rem !important}.me-2{margin-right:.5rem !important}.me-3{margin-right:1rem !important}.me-4{margin-right:1.5rem !important}.me-5{margin-right:3rem !important}.me-auto{margin-right:auto !important}.mb-0{margin-bottom:0 !important}.mb-1{margin-bottom:.25rem !important}.mb-2{margin-bottom:.5rem !important}.mb-3{margin-bottom:1rem !important}.mb-4{margin-bottom:1.5rem !important}.mb-5{margin-bottom:3rem !important}.mb-auto{margin-bottom:auto !important}.ms-0{margin-left:0 !important}.ms-1{margin-left:.25rem !important}.ms-2{margin-left:.5rem !important}.ms-3{margin-left:1rem !important}.ms-4{margin-left:1.5rem !important}.ms-5{margin-left:3rem !important}.ms-auto{margin-left:auto !important}.p-0{padding:0 !important}.p-1{padding:.25rem !important}.p-2{padding:.5rem !important}.p-3{padding:1rem !important}.p-4{padding:1.5rem !important}.p-5{padding:3rem !important}.px-0{padding-right:0 !important;padding-left:0 !important}.px-1{padding-right:.25rem !important;padding-left:.25rem !important}.px-2{padding-right:.5rem !important;padding-left:.5rem !important}.px-3{padding-right:1rem !important;padding-left:1rem !important}.px-4{padding-right:1.5rem !important;padding-left:1.5rem !important}.px-5{padding-right:3rem !important;padding-left:3rem !important}.py-0{padding-top:0 !important;padding-bottom:0 !important}.py-1{padding-top:.25rem !important;padding-bottom:.25rem !important}.py-2{padding-top:.5rem !important;padding-bottom:.5rem !important}.py-3{padding-top:1rem !important;padding-bottom:1rem !important}.py-4{padding-top:1.5rem !important;padding-bottom:1.5rem !important}.py-5{padding-top:3rem !important;padding-bottom:3rem !important}.pt-0{padding-top:0 !important}.pt-1{padding-top:.25rem !important}.pt-2{padding-top:.5rem !important}.pt-3{padding-top:1rem !important}.pt-4{padding-top:1.5rem !important}.pt-5{padding-top:3rem !important}.pe-0{padding-right:0 !important}.pe-1{padding-right:.25rem !important}.pe-2{padding-right:.5rem !important}.pe-3{padding-right:1rem !important}.pe-4{padding-right:1.5rem !important}.pe-5{padding-right:3rem !important}.pb-0{padding-bottom:0 !important}.pb-1{padding-bottom:.25rem !important}.pb-2{padding-bottom:.5rem !important}.pb-3{padding-bottom:1rem !important}.pb-4{padding-bottom:1.5rem !important}.pb-5{padding-bottom:3rem !important}.ps-0{padding-left:0 !important}.ps-1{padding-left:.25rem !important}.ps-2{padding-left:.5rem !important}.ps-3{padding-left:1rem !important}.ps-4{padding-left:1.5rem !important}.ps-5{padding-left:3rem !important}.gap-0{gap:0 !important}.gap-1{gap:.25rem !important}.gap-2{gap:.5rem !important}.gap-3{gap:1rem !important}.gap-4{gap:1.5rem !important}.gap-5{gap:3rem !important}.font-monospace{font-family:var(--bs-font-monospace) !important}.fs-1{font-size:calc(1.375rem + 1.5vw) !important}.fs-2{font-size:calc(1.325rem + .9vw) !important}.fs-3{font-size:calc(1.3rem + .6vw) !important}.fs-4{font-size:calc(1.275rem + .3vw) !important}.fs-5{font-size:1.25rem !important}.fs-6{font-size:1rem !important}.fst-italic{font-style:italic !important}.fst-normal{font-style:normal !important}.fw-light{font-weight:300 !important}.fw-lighter{font-weight:lighter !important}.fw-normal{font-weight:400 !important}.fw-bold{font-weight:700 !important}.fw-semibold{font-weight:600 !important}.fw-bolder{font-weight:bolder !important}.lh-1{line-height:1 !important}.lh-sm{line-height:1.25 !important}.lh-base{line-height:1.5 !important}.lh-lg{line-height:2 !important}.text-start{text-align:left !important}.text-end{text-align:right !important}.text-center{text-align:center !important}.text-decoration-none{text-decoration:none !important}.text-decoration-underline{text-decoration:underline !important}.text-decoration-line-through{text-decoration:line-through !important}.text-lowercase{text-transform:lowercase !important}.text-uppercase{text-transform:uppercase !important}.text-capitalize{text-transform:capitalize !important}.text-wrap{white-space:normal !important}.text-nowrap{white-space:nowrap !important}.text-break{word-wrap:break-word !important;word-break:break-word !important}.text-default{--bs-text-opacity: 1;color:rgba(var(--bs-default-rgb), var(--bs-text-opacity)) !important}.text-primary{--bs-text-opacity: 1;color:rgba(var(--bs-primary-rgb), var(--bs-text-opacity)) !important}.text-secondary{--bs-text-opacity: 1;color:rgba(var(--bs-secondary-rgb), var(--bs-text-opacity)) !important}.text-success{--bs-text-opacity: 1;color:rgba(var(--bs-success-rgb), var(--bs-text-opacity)) !important}.text-info{--bs-text-opacity: 1;color:rgba(var(--bs-info-rgb), var(--bs-text-opacity)) !important}.text-warning{--bs-text-opacity: 1;color:rgba(var(--bs-warning-rgb), var(--bs-text-opacity)) !important}.text-danger{--bs-text-opacity: 1;color:rgba(var(--bs-danger-rgb), var(--bs-text-opacity)) !important}.text-light{--bs-text-opacity: 1;color:rgba(var(--bs-light-rgb), var(--bs-text-opacity)) !important}.text-dark{--bs-text-opacity: 1;color:rgba(var(--bs-dark-rgb), var(--bs-text-opacity)) !important}.text-black{--bs-text-opacity: 1;color:rgba(var(--bs-black-rgb), var(--bs-text-opacity)) !important}.text-white{--bs-text-opacity: 1;color:rgba(var(--bs-white-rgb), var(--bs-text-opacity)) !important}.text-body{--bs-text-opacity: 1;color:rgba(var(--bs-body-color-rgb), var(--bs-text-opacity)) !important}.text-muted,.help-text,.help-block{--bs-text-opacity: 1;color:#6c757d !important}.text-black-50{--bs-text-opacity: 1;color:rgba(0,0,0,0.5) !important}.text-white-50{--bs-text-opacity: 1;color:rgba(255,255,255,0.5) !important}.text-reset{--bs-text-opacity: 1;color:inherit !important}.text-opacity-25{--bs-text-opacity: .25}.text-opacity-50{--bs-text-opacity: .5}.text-opacity-75{--bs-text-opacity: .75}.text-opacity-100{--bs-text-opacity: 1}.bg-default{--bs-bg-opacity: 1;background-color:rgba(var(--bs-default-rgb), var(--bs-bg-opacity)) !important}.bg-primary{--bs-bg-opacity: 1;background-color:rgba(var(--bs-primary-rgb), var(--bs-bg-opacity)) !important}.bg-secondary{--bs-bg-opacity: 1;background-color:rgba(var(--bs-secondary-rgb), var(--bs-bg-opacity)) !important}.bg-success{--bs-bg-opacity: 1;background-color:rgba(var(--bs-success-rgb), var(--bs-bg-opacity)) !important}.bg-info{--bs-bg-opacity: 1;background-color:rgba(var(--bs-info-rgb), var(--bs-bg-opacity)) !important}.bg-warning{--bs-bg-opacity: 1;background-color:rgba(var(--bs-warning-rgb), var(--bs-bg-opacity)) !important}.bg-danger{--bs-bg-opacity: 1;background-color:rgba(var(--bs-danger-rgb), var(--bs-bg-opacity)) !important}.bg-light{--bs-bg-opacity: 1;background-color:rgba(var(--bs-light-rgb), var(--bs-bg-opacity)) !important}.bg-dark{--bs-bg-opacity: 1;background-color:rgba(var(--bs-dark-rgb), var(--bs-bg-opacity)) !important}.bg-black{--bs-bg-opacity: 1;background-color:rgba(var(--bs-black-rgb), var(--bs-bg-opacity)) !important}.bg-white{--bs-bg-opacity: 1;background-color:rgba(var(--bs-white-rgb), var(--bs-bg-opacity)) !important}.bg-body{--bs-bg-opacity: 1;background-color:rgba(var(--bs-body-bg-rgb), var(--bs-bg-opacity)) !important}.bg-transparent{--bs-bg-opacity: 1;background-color:rgba(0,0,0,0) !important}.bg-opacity-10{--bs-bg-opacity: .1}.bg-opacity-25{--bs-bg-opacity: .25}.bg-opacity-50{--bs-bg-opacity: .5}.bg-opacity-75{--bs-bg-opacity: .75}.bg-opacity-100{--bs-bg-opacity: 1}.bg-gradient{background-image:var(--bs-gradient) !important}.user-select-all{user-select:all !important}.user-select-auto{user-select:auto !important}.user-select-none{user-select:none !important}.pe-none{pointer-events:none !important}.pe-auto{pointer-events:auto !important}.rounded{border-radius:var(--bs-border-radius) !important}.rounded-0{border-radius:0 !important}.rounded-1{border-radius:var(--bs-border-radius-sm) !important}.rounded-2{border-radius:var(--bs-border-radius) !important}.rounded-3{border-radius:var(--bs-border-radius-lg) !important}.rounded-4{border-radius:var(--bs-border-radius-xl) !important}.rounded-5{border-radius:var(--bs-border-radius-2xl) !important}.rounded-circle{border-radius:50% !important}.rounded-pill{border-radius:var(--bs-border-radius-pill) !important}.rounded-top{border-top-left-radius:var(--bs-border-radius) !important;border-top-right-radius:var(--bs-border-radius) !important}.rounded-end{border-top-right-radius:var(--bs-border-radius) !important;border-bottom-right-radius:var(--bs-border-radius) !important}.rounded-bottom{border-bottom-right-radius:var(--bs-border-radius) !important;border-bottom-left-radius:var(--bs-border-radius) !important}.rounded-start{border-bottom-left-radius:var(--bs-border-radius) !important;border-top-left-radius:var(--bs-border-radius) !important}.visible{visibility:visible !important}.invisible{visibility:hidden !important}@media (min-width: 576px){.float-sm-start{float:left !important}.float-sm-end{float:right !important}.float-sm-none{float:none !important}.d-sm-inline{display:inline !important}.d-sm-inline-block{display:inline-block !important}.d-sm-block{display:block !important}.d-sm-grid{display:grid !important}.d-sm-table{display:table !important}.d-sm-table-row{display:table-row !important}.d-sm-table-cell{display:table-cell !important}.d-sm-flex{display:flex !important}.d-sm-inline-flex{display:inline-flex !important}.d-sm-none{display:none !important}.flex-sm-fill{flex:1 1 auto !important}.flex-sm-row{flex-direction:row !important}.flex-sm-column{flex-direction:column !important}.flex-sm-row-reverse{flex-direction:row-reverse !important}.flex-sm-column-reverse{flex-direction:column-reverse !important}.flex-sm-grow-0{flex-grow:0 !important}.flex-sm-grow-1{flex-grow:1 !important}.flex-sm-shrink-0{flex-shrink:0 !important}.flex-sm-shrink-1{flex-shrink:1 !important}.flex-sm-wrap{flex-wrap:wrap !important}.flex-sm-nowrap{flex-wrap:nowrap !important}.flex-sm-wrap-reverse{flex-wrap:wrap-reverse !important}.justify-content-sm-start{justify-content:flex-start !important}.justify-content-sm-end{justify-content:flex-end !important}.justify-content-sm-center{justify-content:center !important}.justify-content-sm-between{justify-content:space-between !important}.justify-content-sm-around{justify-content:space-around !important}.justify-content-sm-evenly{justify-content:space-evenly !important}.align-items-sm-start{align-items:flex-start !important}.align-items-sm-end{align-items:flex-end !important}.align-items-sm-center{align-items:center !important}.align-items-sm-baseline{align-items:baseline !important}.align-items-sm-stretch{align-items:stretch !important}.align-content-sm-start{align-content:flex-start !important}.align-content-sm-end{align-content:flex-end !important}.align-content-sm-center{align-content:center !important}.align-content-sm-between{align-content:space-between !important}.align-content-sm-around{align-content:space-around !important}.align-content-sm-stretch{align-content:stretch !important}.align-self-sm-auto{align-self:auto !important}.align-self-sm-start{align-self:flex-start !important}.align-self-sm-end{align-self:flex-end !important}.align-self-sm-center{align-self:center !important}.align-self-sm-baseline{align-self:baseline !important}.align-self-sm-stretch{align-self:stretch !important}.order-sm-first{order:-1 !important}.order-sm-0{order:0 !important}.order-sm-1{order:1 !important}.order-sm-2{order:2 !important}.order-sm-3{order:3 !important}.order-sm-4{order:4 !important}.order-sm-5{order:5 !important}.order-sm-last{order:6 !important}.m-sm-0{margin:0 !important}.m-sm-1{margin:.25rem !important}.m-sm-2{margin:.5rem !important}.m-sm-3{margin:1rem !important}.m-sm-4{margin:1.5rem !important}.m-sm-5{margin:3rem !important}.m-sm-auto{margin:auto !important}.mx-sm-0{margin-right:0 !important;margin-left:0 !important}.mx-sm-1{margin-right:.25rem !important;margin-left:.25rem !important}.mx-sm-2{margin-right:.5rem !important;margin-left:.5rem !important}.mx-sm-3{margin-right:1rem !important;margin-left:1rem !important}.mx-sm-4{margin-right:1.5rem !important;margin-left:1.5rem !important}.mx-sm-5{margin-right:3rem !important;margin-left:3rem !important}.mx-sm-auto{margin-right:auto !important;margin-left:auto !important}.my-sm-0{margin-top:0 !important;margin-bottom:0 !important}.my-sm-1{margin-top:.25rem !important;margin-bottom:.25rem !important}.my-sm-2{margin-top:.5rem !important;margin-bottom:.5rem !important}.my-sm-3{margin-top:1rem !important;margin-bottom:1rem !important}.my-sm-4{margin-top:1.5rem !important;margin-bottom:1.5rem !important}.my-sm-5{margin-top:3rem !important;margin-bottom:3rem !important}.my-sm-auto{margin-top:auto !important;margin-bottom:auto !important}.mt-sm-0{margin-top:0 !important}.mt-sm-1{margin-top:.25rem !important}.mt-sm-2{margin-top:.5rem !important}.mt-sm-3{margin-top:1rem !important}.mt-sm-4{margin-top:1.5rem !important}.mt-sm-5{margin-top:3rem !important}.mt-sm-auto{margin-top:auto !important}.me-sm-0{margin-right:0 !important}.me-sm-1{margin-right:.25rem !important}.me-sm-2{margin-right:.5rem !important}.me-sm-3{margin-right:1rem !important}.me-sm-4{margin-right:1.5rem !important}.me-sm-5{margin-right:3rem !important}.me-sm-auto{margin-right:auto !important}.mb-sm-0{margin-bottom:0 !important}.mb-sm-1{margin-bottom:.25rem !important}.mb-sm-2{margin-bottom:.5rem !important}.mb-sm-3{margin-bottom:1rem !important}.mb-sm-4{margin-bottom:1.5rem !important}.mb-sm-5{margin-bottom:3rem !important}.mb-sm-auto{margin-bottom:auto !important}.ms-sm-0{margin-left:0 !important}.ms-sm-1{margin-left:.25rem !important}.ms-sm-2{margin-left:.5rem !important}.ms-sm-3{margin-left:1rem !important}.ms-sm-4{margin-left:1.5rem !important}.ms-sm-5{margin-left:3rem !important}.ms-sm-auto{margin-left:auto !important}.p-sm-0{padding:0 !important}.p-sm-1{padding:.25rem !important}.p-sm-2{padding:.5rem !important}.p-sm-3{padding:1rem !important}.p-sm-4{padding:1.5rem !important}.p-sm-5{padding:3rem !important}.px-sm-0{padding-right:0 !important;padding-left:0 !important}.px-sm-1{padding-right:.25rem !important;padding-left:.25rem !important}.px-sm-2{padding-right:.5rem !important;padding-left:.5rem !important}.px-sm-3{padding-right:1rem !important;padding-left:1rem !important}.px-sm-4{padding-right:1.5rem !important;padding-left:1.5rem !important}.px-sm-5{padding-right:3rem !important;padding-left:3rem !important}.py-sm-0{padding-top:0 !important;padding-bottom:0 !important}.py-sm-1{padding-top:.25rem !important;padding-bottom:.25rem !important}.py-sm-2{padding-top:.5rem !important;padding-bottom:.5rem !important}.py-sm-3{padding-top:1rem !important;padding-bottom:1rem !important}.py-sm-4{padding-top:1.5rem !important;padding-bottom:1.5rem !important}.py-sm-5{padding-top:3rem !important;padding-bottom:3rem !important}.pt-sm-0{padding-top:0 !important}.pt-sm-1{padding-top:.25rem !important}.pt-sm-2{padding-top:.5rem !important}.pt-sm-3{padding-top:1rem !important}.pt-sm-4{padding-top:1.5rem !important}.pt-sm-5{padding-top:3rem !important}.pe-sm-0{padding-right:0 !important}.pe-sm-1{padding-right:.25rem !important}.pe-sm-2{padding-right:.5rem !important}.pe-sm-3{padding-right:1rem !important}.pe-sm-4{padding-right:1.5rem !important}.pe-sm-5{padding-right:3rem !important}.pb-sm-0{padding-bottom:0 !important}.pb-sm-1{padding-bottom:.25rem !important}.pb-sm-2{padding-bottom:.5rem !important}.pb-sm-3{padding-bottom:1rem !important}.pb-sm-4{padding-bottom:1.5rem !important}.pb-sm-5{padding-bottom:3rem !important}.ps-sm-0{padding-left:0 !important}.ps-sm-1{padding-left:.25rem !important}.ps-sm-2{padding-left:.5rem !important}.ps-sm-3{padding-left:1rem !important}.ps-sm-4{padding-left:1.5rem !important}.ps-sm-5{padding-left:3rem !important}.gap-sm-0{gap:0 !important}.gap-sm-1{gap:.25rem !important}.gap-sm-2{gap:.5rem !important}.gap-sm-3{gap:1rem !important}.gap-sm-4{gap:1.5rem !important}.gap-sm-5{gap:3rem !important}.text-sm-start{text-align:left !important}.text-sm-end{text-align:right !important}.text-sm-center{text-align:center !important}}@media (min-width: 768px){.float-md-start{float:left !important}.float-md-end{float:right !important}.float-md-none{float:none !important}.d-md-inline{display:inline !important}.d-md-inline-block{display:inline-block !important}.d-md-block{display:block !important}.d-md-grid{display:grid !important}.d-md-table{display:table !important}.d-md-table-row{display:table-row !important}.d-md-table-cell{display:table-cell !important}.d-md-flex{display:flex !important}.d-md-inline-flex{display:inline-flex !important}.d-md-none{display:none !important}.flex-md-fill{flex:1 1 auto !important}.flex-md-row{flex-direction:row !important}.flex-md-column{flex-direction:column !important}.flex-md-row-reverse{flex-direction:row-reverse !important}.flex-md-column-reverse{flex-direction:column-reverse !important}.flex-md-grow-0{flex-grow:0 !important}.flex-md-grow-1{flex-grow:1 !important}.flex-md-shrink-0{flex-shrink:0 !important}.flex-md-shrink-1{flex-shrink:1 !important}.flex-md-wrap{flex-wrap:wrap !important}.flex-md-nowrap{flex-wrap:nowrap !important}.flex-md-wrap-reverse{flex-wrap:wrap-reverse !important}.justify-content-md-start{justify-content:flex-start !important}.justify-content-md-end{justify-content:flex-end !important}.justify-content-md-center{justify-content:center !important}.justify-content-md-between{justify-content:space-between !important}.justify-content-md-around{justify-content:space-around !important}.justify-content-md-evenly{justify-content:space-evenly !important}.align-items-md-start{align-items:flex-start !important}.align-items-md-end{align-items:flex-end !important}.align-items-md-center{align-items:center !important}.align-items-md-baseline{align-items:baseline !important}.align-items-md-stretch{align-items:stretch !important}.align-content-md-start{align-content:flex-start !important}.align-content-md-end{align-content:flex-end !important}.align-content-md-center{align-content:center !important}.align-content-md-between{align-content:space-between !important}.align-content-md-around{align-content:space-around !important}.align-content-md-stretch{align-content:stretch !important}.align-self-md-auto{align-self:auto !important}.align-self-md-start{align-self:flex-start !important}.align-self-md-end{align-self:flex-end !important}.align-self-md-center{align-self:center !important}.align-self-md-baseline{align-self:baseline !important}.align-self-md-stretch{align-self:stretch !important}.order-md-first{order:-1 !important}.order-md-0{order:0 !important}.order-md-1{order:1 !important}.order-md-2{order:2 !important}.order-md-3{order:3 !important}.order-md-4{order:4 !important}.order-md-5{order:5 !important}.order-md-last{order:6 !important}.m-md-0{margin:0 !important}.m-md-1{margin:.25rem !important}.m-md-2{margin:.5rem !important}.m-md-3{margin:1rem !important}.m-md-4{margin:1.5rem !important}.m-md-5{margin:3rem !important}.m-md-auto{margin:auto !important}.mx-md-0{margin-right:0 !important;margin-left:0 !important}.mx-md-1{margin-right:.25rem !important;margin-left:.25rem !important}.mx-md-2{margin-right:.5rem !important;margin-left:.5rem !important}.mx-md-3{margin-right:1rem !important;margin-left:1rem !important}.mx-md-4{margin-right:1.5rem !important;margin-left:1.5rem !important}.mx-md-5{margin-right:3rem !important;margin-left:3rem !important}.mx-md-auto{margin-right:auto !important;margin-left:auto !important}.my-md-0{margin-top:0 !important;margin-bottom:0 !important}.my-md-1{margin-top:.25rem !important;margin-bottom:.25rem !important}.my-md-2{margin-top:.5rem !important;margin-bottom:.5rem !important}.my-md-3{margin-top:1rem !important;margin-bottom:1rem !important}.my-md-4{margin-top:1.5rem !important;margin-bottom:1.5rem !important}.my-md-5{margin-top:3rem !important;margin-bottom:3rem !important}.my-md-auto{margin-top:auto !important;margin-bottom:auto !important}.mt-md-0{margin-top:0 !important}.mt-md-1{margin-top:.25rem !important}.mt-md-2{margin-top:.5rem !important}.mt-md-3{margin-top:1rem !important}.mt-md-4{margin-top:1.5rem !important}.mt-md-5{margin-top:3rem !important}.mt-md-auto{margin-top:auto !important}.me-md-0{margin-right:0 !important}.me-md-1{margin-right:.25rem !important}.me-md-2{margin-right:.5rem !important}.me-md-3{margin-right:1rem !important}.me-md-4{margin-right:1.5rem !important}.me-md-5{margin-right:3rem !important}.me-md-auto{margin-right:auto !important}.mb-md-0{margin-bottom:0 !important}.mb-md-1{margin-bottom:.25rem !important}.mb-md-2{margin-bottom:.5rem !important}.mb-md-3{margin-bottom:1rem !important}.mb-md-4{margin-bottom:1.5rem !important}.mb-md-5{margin-bottom:3rem !important}.mb-md-auto{margin-bottom:auto !important}.ms-md-0{margin-left:0 !important}.ms-md-1{margin-left:.25rem !important}.ms-md-2{margin-left:.5rem !important}.ms-md-3{margin-left:1rem !important}.ms-md-4{margin-left:1.5rem !important}.ms-md-5{margin-left:3rem !important}.ms-md-auto{margin-left:auto !important}.p-md-0{padding:0 !important}.p-md-1{padding:.25rem !important}.p-md-2{padding:.5rem !important}.p-md-3{padding:1rem !important}.p-md-4{padding:1.5rem !important}.p-md-5{padding:3rem !important}.px-md-0{padding-right:0 !important;padding-left:0 !important}.px-md-1{padding-right:.25rem !important;padding-left:.25rem !important}.px-md-2{padding-right:.5rem !important;padding-left:.5rem !important}.px-md-3{padding-right:1rem !important;padding-left:1rem !important}.px-md-4{padding-right:1.5rem !important;padding-left:1.5rem !important}.px-md-5{padding-right:3rem !important;padding-left:3rem !important}.py-md-0{padding-top:0 !important;padding-bottom:0 !important}.py-md-1{padding-top:.25rem !important;padding-bottom:.25rem !important}.py-md-2{padding-top:.5rem !important;padding-bottom:.5rem !important}.py-md-3{padding-top:1rem !important;padding-bottom:1rem !important}.py-md-4{padding-top:1.5rem !important;padding-bottom:1.5rem !important}.py-md-5{padding-top:3rem !important;padding-bottom:3rem !important}.pt-md-0{padding-top:0 !important}.pt-md-1{padding-top:.25rem !important}.pt-md-2{padding-top:.5rem !important}.pt-md-3{padding-top:1rem !important}.pt-md-4{padding-top:1.5rem !important}.pt-md-5{padding-top:3rem !important}.pe-md-0{padding-right:0 !important}.pe-md-1{padding-right:.25rem !important}.pe-md-2{padding-right:.5rem !important}.pe-md-3{padding-right:1rem !important}.pe-md-4{padding-right:1.5rem !important}.pe-md-5{padding-right:3rem !important}.pb-md-0{padding-bottom:0 !important}.pb-md-1{padding-bottom:.25rem !important}.pb-md-2{padding-bottom:.5rem !important}.pb-md-3{padding-bottom:1rem !important}.pb-md-4{padding-bottom:1.5rem !important}.pb-md-5{padding-bottom:3rem !important}.ps-md-0{padding-left:0 !important}.ps-md-1{padding-left:.25rem !important}.ps-md-2{padding-left:.5rem !important}.ps-md-3{padding-left:1rem !important}.ps-md-4{padding-left:1.5rem !important}.ps-md-5{padding-left:3rem !important}.gap-md-0{gap:0 !important}.gap-md-1{gap:.25rem !important}.gap-md-2{gap:.5rem !important}.gap-md-3{gap:1rem !important}.gap-md-4{gap:1.5rem !important}.gap-md-5{gap:3rem !important}.text-md-start{text-align:left !important}.text-md-end{text-align:right !important}.text-md-center{text-align:center !important}}@media (min-width: 992px){.float-lg-start{float:left !important}.float-lg-end{float:right !important}.float-lg-none{float:none !important}.d-lg-inline{display:inline !important}.d-lg-inline-block{display:inline-block !important}.d-lg-block{display:block !important}.d-lg-grid{display:grid !important}.d-lg-table{display:table !important}.d-lg-table-row{display:table-row !important}.d-lg-table-cell{display:table-cell !important}.d-lg-flex{display:flex !important}.d-lg-inline-flex{display:inline-flex !important}.d-lg-none{display:none !important}.flex-lg-fill{flex:1 1 auto !important}.flex-lg-row{flex-direction:row !important}.flex-lg-column{flex-direction:column !important}.flex-lg-row-reverse{flex-direction:row-reverse !important}.flex-lg-column-reverse{flex-direction:column-reverse !important}.flex-lg-grow-0{flex-grow:0 !important}.flex-lg-grow-1{flex-grow:1 !important}.flex-lg-shrink-0{flex-shrink:0 !important}.flex-lg-shrink-1{flex-shrink:1 !important}.flex-lg-wrap{flex-wrap:wrap !important}.flex-lg-nowrap{flex-wrap:nowrap !important}.flex-lg-wrap-reverse{flex-wrap:wrap-reverse !important}.justify-content-lg-start{justify-content:flex-start !important}.justify-content-lg-end{justify-content:flex-end !important}.justify-content-lg-center{justify-content:center !important}.justify-content-lg-between{justify-content:space-between !important}.justify-content-lg-around{justify-content:space-around !important}.justify-content-lg-evenly{justify-content:space-evenly !important}.align-items-lg-start{align-items:flex-start !important}.align-items-lg-end{align-items:flex-end !important}.align-items-lg-center{align-items:center !important}.align-items-lg-baseline{align-items:baseline !important}.align-items-lg-stretch{align-items:stretch !important}.align-content-lg-start{align-content:flex-start !important}.align-content-lg-end{align-content:flex-end !important}.align-content-lg-center{align-content:center !important}.align-content-lg-between{align-content:space-between !important}.align-content-lg-around{align-content:space-around !important}.align-content-lg-stretch{align-content:stretch !important}.align-self-lg-auto{align-self:auto !important}.align-self-lg-start{align-self:flex-start !important}.align-self-lg-end{align-self:flex-end !important}.align-self-lg-center{align-self:center !important}.align-self-lg-baseline{align-self:baseline !important}.align-self-lg-stretch{align-self:stretch !important}.order-lg-first{order:-1 !important}.order-lg-0{order:0 !important}.order-lg-1{order:1 !important}.order-lg-2{order:2 !important}.order-lg-3{order:3 !important}.order-lg-4{order:4 !important}.order-lg-5{order:5 !important}.order-lg-last{order:6 !important}.m-lg-0{margin:0 !important}.m-lg-1{margin:.25rem !important}.m-lg-2{margin:.5rem !important}.m-lg-3{margin:1rem !important}.m-lg-4{margin:1.5rem !important}.m-lg-5{margin:3rem !important}.m-lg-auto{margin:auto !important}.mx-lg-0{margin-right:0 !important;margin-left:0 !important}.mx-lg-1{margin-right:.25rem !important;margin-left:.25rem !important}.mx-lg-2{margin-right:.5rem !important;margin-left:.5rem !important}.mx-lg-3{margin-right:1rem !important;margin-left:1rem !important}.mx-lg-4{margin-right:1.5rem !important;margin-left:1.5rem !important}.mx-lg-5{margin-right:3rem !important;margin-left:3rem !important}.mx-lg-auto{margin-right:auto !important;margin-left:auto !important}.my-lg-0{margin-top:0 !important;margin-bottom:0 !important}.my-lg-1{margin-top:.25rem !important;margin-bottom:.25rem !important}.my-lg-2{margin-top:.5rem !important;margin-bottom:.5rem !important}.my-lg-3{margin-top:1rem !important;margin-bottom:1rem !important}.my-lg-4{margin-top:1.5rem !important;margin-bottom:1.5rem !important}.my-lg-5{margin-top:3rem !important;margin-bottom:3rem !important}.my-lg-auto{margin-top:auto !important;margin-bottom:auto !important}.mt-lg-0{margin-top:0 !important}.mt-lg-1{margin-top:.25rem !important}.mt-lg-2{margin-top:.5rem !important}.mt-lg-3{margin-top:1rem !important}.mt-lg-4{margin-top:1.5rem !important}.mt-lg-5{margin-top:3rem !important}.mt-lg-auto{margin-top:auto !important}.me-lg-0{margin-right:0 !important}.me-lg-1{margin-right:.25rem !important}.me-lg-2{margin-right:.5rem !important}.me-lg-3{margin-right:1rem !important}.me-lg-4{margin-right:1.5rem !important}.me-lg-5{margin-right:3rem !important}.me-lg-auto{margin-right:auto !important}.mb-lg-0{margin-bottom:0 !important}.mb-lg-1{margin-bottom:.25rem !important}.mb-lg-2{margin-bottom:.5rem !important}.mb-lg-3{margin-bottom:1rem !important}.mb-lg-4{margin-bottom:1.5rem !important}.mb-lg-5{margin-bottom:3rem !important}.mb-lg-auto{margin-bottom:auto !important}.ms-lg-0{margin-left:0 !important}.ms-lg-1{margin-left:.25rem !important}.ms-lg-2{margin-left:.5rem !important}.ms-lg-3{margin-left:1rem !important}.ms-lg-4{margin-left:1.5rem !important}.ms-lg-5{margin-left:3rem !important}.ms-lg-auto{margin-left:auto !important}.p-lg-0{padding:0 !important}.p-lg-1{padding:.25rem !important}.p-lg-2{padding:.5rem !important}.p-lg-3{padding:1rem !important}.p-lg-4{padding:1.5rem !important}.p-lg-5{padding:3rem !important}.px-lg-0{padding-right:0 !important;padding-left:0 !important}.px-lg-1{padding-right:.25rem !important;padding-left:.25rem !important}.px-lg-2{padding-right:.5rem !important;padding-left:.5rem !important}.px-lg-3{padding-right:1rem !important;padding-left:1rem !important}.px-lg-4{padding-right:1.5rem !important;padding-left:1.5rem !important}.px-lg-5{padding-right:3rem !important;padding-left:3rem !important}.py-lg-0{padding-top:0 !important;padding-bottom:0 !important}.py-lg-1{padding-top:.25rem !important;padding-bottom:.25rem !important}.py-lg-2{padding-top:.5rem !important;padding-bottom:.5rem !important}.py-lg-3{padding-top:1rem !important;padding-bottom:1rem !important}.py-lg-4{padding-top:1.5rem !important;padding-bottom:1.5rem !important}.py-lg-5{padding-top:3rem !important;padding-bottom:3rem !important}.pt-lg-0{padding-top:0 !important}.pt-lg-1{padding-top:.25rem !important}.pt-lg-2{padding-top:.5rem !important}.pt-lg-3{padding-top:1rem !important}.pt-lg-4{padding-top:1.5rem !important}.pt-lg-5{padding-top:3rem !important}.pe-lg-0{padding-right:0 !important}.pe-lg-1{padding-right:.25rem !important}.pe-lg-2{padding-right:.5rem !important}.pe-lg-3{padding-right:1rem !important}.pe-lg-4{padding-right:1.5rem !important}.pe-lg-5{padding-right:3rem !important}.pb-lg-0{padding-bottom:0 !important}.pb-lg-1{padding-bottom:.25rem !important}.pb-lg-2{padding-bottom:.5rem !important}.pb-lg-3{padding-bottom:1rem !important}.pb-lg-4{padding-bottom:1.5rem !important}.pb-lg-5{padding-bottom:3rem !important}.ps-lg-0{padding-left:0 !important}.ps-lg-1{padding-left:.25rem !important}.ps-lg-2{padding-left:.5rem !important}.ps-lg-3{padding-left:1rem !important}.ps-lg-4{padding-left:1.5rem !important}.ps-lg-5{padding-left:3rem !important}.gap-lg-0{gap:0 !important}.gap-lg-1{gap:.25rem !important}.gap-lg-2{gap:.5rem !important}.gap-lg-3{gap:1rem !important}.gap-lg-4{gap:1.5rem !important}.gap-lg-5{gap:3rem !important}.text-lg-start{text-align:left !important}.text-lg-end{text-align:right !important}.text-lg-center{text-align:center !important}}@media (min-width: 1200px){.float-xl-start{float:left !important}.float-xl-end{float:right !important}.float-xl-none{float:none !important}.d-xl-inline{display:inline !important}.d-xl-inline-block{display:inline-block !important}.d-xl-block{display:block !important}.d-xl-grid{display:grid !important}.d-xl-table{display:table !important}.d-xl-table-row{display:table-row !important}.d-xl-table-cell{display:table-cell !important}.d-xl-flex{display:flex !important}.d-xl-inline-flex{display:inline-flex !important}.d-xl-none{display:none !important}.flex-xl-fill{flex:1 1 auto !important}.flex-xl-row{flex-direction:row !important}.flex-xl-column{flex-direction:column !important}.flex-xl-row-reverse{flex-direction:row-reverse !important}.flex-xl-column-reverse{flex-direction:column-reverse !important}.flex-xl-grow-0{flex-grow:0 !important}.flex-xl-grow-1{flex-grow:1 !important}.flex-xl-shrink-0{flex-shrink:0 !important}.flex-xl-shrink-1{flex-shrink:1 !important}.flex-xl-wrap{flex-wrap:wrap !important}.flex-xl-nowrap{flex-wrap:nowrap !important}.flex-xl-wrap-reverse{flex-wrap:wrap-reverse !important}.justify-content-xl-start{justify-content:flex-start !important}.justify-content-xl-end{justify-content:flex-end !important}.justify-content-xl-center{justify-content:center !important}.justify-content-xl-between{justify-content:space-between !important}.justify-content-xl-around{justify-content:space-around !important}.justify-content-xl-evenly{justify-content:space-evenly !important}.align-items-xl-start{align-items:flex-start !important}.align-items-xl-end{align-items:flex-end !important}.align-items-xl-center{align-items:center !important}.align-items-xl-baseline{align-items:baseline !important}.align-items-xl-stretch{align-items:stretch !important}.align-content-xl-start{align-content:flex-start !important}.align-content-xl-end{align-content:flex-end !important}.align-content-xl-center{align-content:center !important}.align-content-xl-between{align-content:space-between !important}.align-content-xl-around{align-content:space-around !important}.align-content-xl-stretch{align-content:stretch !important}.align-self-xl-auto{align-self:auto !important}.align-self-xl-start{align-self:flex-start !important}.align-self-xl-end{align-self:flex-end !important}.align-self-xl-center{align-self:center !important}.align-self-xl-baseline{align-self:baseline !important}.align-self-xl-stretch{align-self:stretch !important}.order-xl-first{order:-1 !important}.order-xl-0{order:0 !important}.order-xl-1{order:1 !important}.order-xl-2{order:2 !important}.order-xl-3{order:3 !important}.order-xl-4{order:4 !important}.order-xl-5{order:5 !important}.order-xl-last{order:6 !important}.m-xl-0{margin:0 !important}.m-xl-1{margin:.25rem !important}.m-xl-2{margin:.5rem !important}.m-xl-3{margin:1rem !important}.m-xl-4{margin:1.5rem !important}.m-xl-5{margin:3rem !important}.m-xl-auto{margin:auto !important}.mx-xl-0{margin-right:0 !important;margin-left:0 !important}.mx-xl-1{margin-right:.25rem !important;margin-left:.25rem !important}.mx-xl-2{margin-right:.5rem !important;margin-left:.5rem !important}.mx-xl-3{margin-right:1rem !important;margin-left:1rem !important}.mx-xl-4{margin-right:1.5rem !important;margin-left:1.5rem !important}.mx-xl-5{margin-right:3rem !important;margin-left:3rem !important}.mx-xl-auto{margin-right:auto !important;margin-left:auto !important}.my-xl-0{margin-top:0 !important;margin-bottom:0 !important}.my-xl-1{margin-top:.25rem !important;margin-bottom:.25rem !important}.my-xl-2{margin-top:.5rem !important;margin-bottom:.5rem !important}.my-xl-3{margin-top:1rem !important;margin-bottom:1rem !important}.my-xl-4{margin-top:1.5rem !important;margin-bottom:1.5rem !important}.my-xl-5{margin-top:3rem !important;margin-bottom:3rem !important}.my-xl-auto{margin-top:auto !important;margin-bottom:auto !important}.mt-xl-0{margin-top:0 !important}.mt-xl-1{margin-top:.25rem !important}.mt-xl-2{margin-top:.5rem !important}.mt-xl-3{margin-top:1rem !important}.mt-xl-4{margin-top:1.5rem !important}.mt-xl-5{margin-top:3rem !important}.mt-xl-auto{margin-top:auto !important}.me-xl-0{margin-right:0 !important}.me-xl-1{margin-right:.25rem !important}.me-xl-2{margin-right:.5rem !important}.me-xl-3{margin-right:1rem !important}.me-xl-4{margin-right:1.5rem !important}.me-xl-5{margin-right:3rem !important}.me-xl-auto{margin-right:auto !important}.mb-xl-0{margin-bottom:0 !important}.mb-xl-1{margin-bottom:.25rem !important}.mb-xl-2{margin-bottom:.5rem !important}.mb-xl-3{margin-bottom:1rem !important}.mb-xl-4{margin-bottom:1.5rem !important}.mb-xl-5{margin-bottom:3rem !important}.mb-xl-auto{margin-bottom:auto !important}.ms-xl-0{margin-left:0 !important}.ms-xl-1{margin-left:.25rem !important}.ms-xl-2{margin-left:.5rem !important}.ms-xl-3{margin-left:1rem !important}.ms-xl-4{margin-left:1.5rem !important}.ms-xl-5{margin-left:3rem !important}.ms-xl-auto{margin-left:auto !important}.p-xl-0{padding:0 !important}.p-xl-1{padding:.25rem !important}.p-xl-2{padding:.5rem !important}.p-xl-3{padding:1rem !important}.p-xl-4{padding:1.5rem !important}.p-xl-5{padding:3rem !important}.px-xl-0{padding-right:0 !important;padding-left:0 !important}.px-xl-1{padding-right:.25rem !important;padding-left:.25rem !important}.px-xl-2{padding-right:.5rem !important;padding-left:.5rem !important}.px-xl-3{padding-right:1rem !important;padding-left:1rem !important}.px-xl-4{padding-right:1.5rem !important;padding-left:1.5rem !important}.px-xl-5{padding-right:3rem !important;padding-left:3rem !important}.py-xl-0{padding-top:0 !important;padding-bottom:0 !important}.py-xl-1{padding-top:.25rem !important;padding-bottom:.25rem !important}.py-xl-2{padding-top:.5rem !important;padding-bottom:.5rem !important}.py-xl-3{padding-top:1rem !important;padding-bottom:1rem !important}.py-xl-4{padding-top:1.5rem !important;padding-bottom:1.5rem !important}.py-xl-5{padding-top:3rem !important;padding-bottom:3rem !important}.pt-xl-0{padding-top:0 !important}.pt-xl-1{padding-top:.25rem !important}.pt-xl-2{padding-top:.5rem !important}.pt-xl-3{padding-top:1rem !important}.pt-xl-4{padding-top:1.5rem !important}.pt-xl-5{padding-top:3rem !important}.pe-xl-0{padding-right:0 !important}.pe-xl-1{padding-right:.25rem !important}.pe-xl-2{padding-right:.5rem !important}.pe-xl-3{padding-right:1rem !important}.pe-xl-4{padding-right:1.5rem !important}.pe-xl-5{padding-right:3rem !important}.pb-xl-0{padding-bottom:0 !important}.pb-xl-1{padding-bottom:.25rem !important}.pb-xl-2{padding-bottom:.5rem !important}.pb-xl-3{padding-bottom:1rem !important}.pb-xl-4{padding-bottom:1.5rem !important}.pb-xl-5{padding-bottom:3rem !important}.ps-xl-0{padding-left:0 !important}.ps-xl-1{padding-left:.25rem !important}.ps-xl-2{padding-left:.5rem !important}.ps-xl-3{padding-left:1rem !important}.ps-xl-4{padding-left:1.5rem !important}.ps-xl-5{padding-left:3rem !important}.gap-xl-0{gap:0 !important}.gap-xl-1{gap:.25rem !important}.gap-xl-2{gap:.5rem !important}.gap-xl-3{gap:1rem !important}.gap-xl-4{gap:1.5rem !important}.gap-xl-5{gap:3rem !important}.text-xl-start{text-align:left !important}.text-xl-end{text-align:right !important}.text-xl-center{text-align:center !important}}@media (min-width: 1400px){.float-xxl-start{float:left !important}.float-xxl-end{float:right !important}.float-xxl-none{float:none !important}.d-xxl-inline{display:inline !important}.d-xxl-inline-block{display:inline-block !important}.d-xxl-block{display:block !important}.d-xxl-grid{display:grid !important}.d-xxl-table{display:table !important}.d-xxl-table-row{display:table-row !important}.d-xxl-table-cell{display:table-cell !important}.d-xxl-flex{display:flex !important}.d-xxl-inline-flex{display:inline-flex !important}.d-xxl-none{display:none !important}.flex-xxl-fill{flex:1 1 auto !important}.flex-xxl-row{flex-direction:row !important}.flex-xxl-column{flex-direction:column !important}.flex-xxl-row-reverse{flex-direction:row-reverse !important}.flex-xxl-column-reverse{flex-direction:column-reverse !important}.flex-xxl-grow-0{flex-grow:0 !important}.flex-xxl-grow-1{flex-grow:1 !important}.flex-xxl-shrink-0{flex-shrink:0 !important}.flex-xxl-shrink-1{flex-shrink:1 !important}.flex-xxl-wrap{flex-wrap:wrap !important}.flex-xxl-nowrap{flex-wrap:nowrap !important}.flex-xxl-wrap-reverse{flex-wrap:wrap-reverse !important}.justify-content-xxl-start{justify-content:flex-start !important}.justify-content-xxl-end{justify-content:flex-end !important}.justify-content-xxl-center{justify-content:center !important}.justify-content-xxl-between{justify-content:space-between !important}.justify-content-xxl-around{justify-content:space-around !important}.justify-content-xxl-evenly{justify-content:space-evenly !important}.align-items-xxl-start{align-items:flex-start !important}.align-items-xxl-end{align-items:flex-end !important}.align-items-xxl-center{align-items:center !important}.align-items-xxl-baseline{align-items:baseline !important}.align-items-xxl-stretch{align-items:stretch !important}.align-content-xxl-start{align-content:flex-start !important}.align-content-xxl-end{align-content:flex-end !important}.align-content-xxl-center{align-content:center !important}.align-content-xxl-between{align-content:space-between !important}.align-content-xxl-around{align-content:space-around !important}.align-content-xxl-stretch{align-content:stretch !important}.align-self-xxl-auto{align-self:auto !important}.align-self-xxl-start{align-self:flex-start !important}.align-self-xxl-end{align-self:flex-end !important}.align-self-xxl-center{align-self:center !important}.align-self-xxl-baseline{align-self:baseline !important}.align-self-xxl-stretch{align-self:stretch !important}.order-xxl-first{order:-1 !important}.order-xxl-0{order:0 !important}.order-xxl-1{order:1 !important}.order-xxl-2{order:2 !important}.order-xxl-3{order:3 !important}.order-xxl-4{order:4 !important}.order-xxl-5{order:5 !important}.order-xxl-last{order:6 !important}.m-xxl-0{margin:0 !important}.m-xxl-1{margin:.25rem !important}.m-xxl-2{margin:.5rem !important}.m-xxl-3{margin:1rem !important}.m-xxl-4{margin:1.5rem !important}.m-xxl-5{margin:3rem !important}.m-xxl-auto{margin:auto !important}.mx-xxl-0{margin-right:0 !important;margin-left:0 !important}.mx-xxl-1{margin-right:.25rem !important;margin-left:.25rem !important}.mx-xxl-2{margin-right:.5rem !important;margin-left:.5rem !important}.mx-xxl-3{margin-right:1rem !important;margin-left:1rem !important}.mx-xxl-4{margin-right:1.5rem !important;margin-left:1.5rem !important}.mx-xxl-5{margin-right:3rem !important;margin-left:3rem !important}.mx-xxl-auto{margin-right:auto !important;margin-left:auto !important}.my-xxl-0{margin-top:0 !important;margin-bottom:0 !important}.my-xxl-1{margin-top:.25rem !important;margin-bottom:.25rem !important}.my-xxl-2{margin-top:.5rem !important;margin-bottom:.5rem !important}.my-xxl-3{margin-top:1rem !important;margin-bottom:1rem !important}.my-xxl-4{margin-top:1.5rem !important;margin-bottom:1.5rem !important}.my-xxl-5{margin-top:3rem !important;margin-bottom:3rem !important}.my-xxl-auto{margin-top:auto !important;margin-bottom:auto !important}.mt-xxl-0{margin-top:0 !important}.mt-xxl-1{margin-top:.25rem !important}.mt-xxl-2{margin-top:.5rem !important}.mt-xxl-3{margin-top:1rem !important}.mt-xxl-4{margin-top:1.5rem !important}.mt-xxl-5{margin-top:3rem !important}.mt-xxl-auto{margin-top:auto !important}.me-xxl-0{margin-right:0 !important}.me-xxl-1{margin-right:.25rem !important}.me-xxl-2{margin-right:.5rem !important}.me-xxl-3{margin-right:1rem !important}.me-xxl-4{margin-right:1.5rem !important}.me-xxl-5{margin-right:3rem !important}.me-xxl-auto{margin-right:auto !important}.mb-xxl-0{margin-bottom:0 !important}.mb-xxl-1{margin-bottom:.25rem !important}.mb-xxl-2{margin-bottom:.5rem !important}.mb-xxl-3{margin-bottom:1rem !important}.mb-xxl-4{margin-bottom:1.5rem !important}.mb-xxl-5{margin-bottom:3rem !important}.mb-xxl-auto{margin-bottom:auto !important}.ms-xxl-0{margin-left:0 !important}.ms-xxl-1{margin-left:.25rem !important}.ms-xxl-2{margin-left:.5rem !important}.ms-xxl-3{margin-left:1rem !important}.ms-xxl-4{margin-left:1.5rem !important}.ms-xxl-5{margin-left:3rem !important}.ms-xxl-auto{margin-left:auto !important}.p-xxl-0{padding:0 !important}.p-xxl-1{padding:.25rem !important}.p-xxl-2{padding:.5rem !important}.p-xxl-3{padding:1rem !important}.p-xxl-4{padding:1.5rem !important}.p-xxl-5{padding:3rem !important}.px-xxl-0{padding-right:0 !important;padding-left:0 !important}.px-xxl-1{padding-right:.25rem !important;padding-left:.25rem !important}.px-xxl-2{padding-right:.5rem !important;padding-left:.5rem !important}.px-xxl-3{padding-right:1rem !important;padding-left:1rem !important}.px-xxl-4{padding-right:1.5rem !important;padding-left:1.5rem !important}.px-xxl-5{padding-right:3rem !important;padding-left:3rem !important}.py-xxl-0{padding-top:0 !important;padding-bottom:0 !important}.py-xxl-1{padding-top:.25rem !important;padding-bottom:.25rem !important}.py-xxl-2{padding-top:.5rem !important;padding-bottom:.5rem !important}.py-xxl-3{padding-top:1rem !important;padding-bottom:1rem !important}.py-xxl-4{padding-top:1.5rem !important;padding-bottom:1.5rem !important}.py-xxl-5{padding-top:3rem !important;padding-bottom:3rem !important}.pt-xxl-0{padding-top:0 !important}.pt-xxl-1{padding-top:.25rem !important}.pt-xxl-2{padding-top:.5rem !important}.pt-xxl-3{padding-top:1rem !important}.pt-xxl-4{padding-top:1.5rem !important}.pt-xxl-5{padding-top:3rem !important}.pe-xxl-0{padding-right:0 !important}.pe-xxl-1{padding-right:.25rem !important}.pe-xxl-2{padding-right:.5rem !important}.pe-xxl-3{padding-right:1rem !important}.pe-xxl-4{padding-right:1.5rem !important}.pe-xxl-5{padding-right:3rem !important}.pb-xxl-0{padding-bottom:0 !important}.pb-xxl-1{padding-bottom:.25rem !important}.pb-xxl-2{padding-bottom:.5rem !important}.pb-xxl-3{padding-bottom:1rem !important}.pb-xxl-4{padding-bottom:1.5rem !important}.pb-xxl-5{padding-bottom:3rem !important}.ps-xxl-0{padding-left:0 !important}.ps-xxl-1{padding-left:.25rem !important}.ps-xxl-2{padding-left:.5rem !important}.ps-xxl-3{padding-left:1rem !important}.ps-xxl-4{padding-left:1.5rem !important}.ps-xxl-5{padding-left:3rem !important}.gap-xxl-0{gap:0 !important}.gap-xxl-1{gap:.25rem !important}.gap-xxl-2{gap:.5rem !important}.gap-xxl-3{gap:1rem !important}.gap-xxl-4{gap:1.5rem !important}.gap-xxl-5{gap:3rem !important}.text-xxl-start{text-align:left !important}.text-xxl-end{text-align:right !important}.text-xxl-center{text-align:center !important}}.bg-default{color:#000}.bg-primary{color:#fff}.bg-secondary{color:#fff}.bg-success{color:#fff}.bg-info{color:#000}.bg-warning{color:#000}.bg-danger{color:#fff}.bg-light{color:#000}.bg-dark{color:#fff}@media (min-width: 1200px){.fs-1{font-size:2.5rem !important}.fs-2{font-size:2rem !important}.fs-3{font-size:1.75rem !important}.fs-4{font-size:1.5rem !important}}@media print{.d-print-inline{display:inline !important}.d-print-inline-block{display:inline-block !important}.d-print-block{display:block !important}.d-print-grid{display:grid !important}.d-print-table{display:table !important}.d-print-table-row{display:table-row !important}.d-print-table-cell{display:table-cell !important}.d-print-flex{display:flex !important}.d-print-inline-flex{display:inline-flex !important}.d-print-none{display:none !important}}.table th[align=left]{text-align:left}.table th[align=right]{text-align:right}.table th[align=center]{text-align:center}.well{display:block;background-color:rgba(0,0,0,0.03);color:#212529;padding:1rem;border-radius:.375rem}.well-lg{padding:1.5rem;border-radius:.5rem}.well-sm{padding:0.5rem;border-radius:.25rem}.draggable .well{background-color:#f7f7f7}.dropdown-menu>li.active>a{color:#fff;text-decoration:none;background-color:#0d6efd}.navbar:not(.fixed-bottom):not(.navbar-fixed-bottom):not(.navbar-fixed-bottom)+div>.tab-content>.tab-pane{--bslib-navbar-margin: 20px;margin-top:var(--bslib-navbar-margin)}ul.nav.navbar-nav{flex:1;-webkit-flex:1}ul.nav.navbar-nav.navbar-right{flex:unset;-webkit-flex:unset;display:flex;display:-webkit-flex;justify-content:flex-end;-webkit-justify-content:flex-end}.navbar.navbar-default{background-color:#f8f9fa !important}.navbar.navbar-inverse{background-color:#212529 !important}.navbar-toggle>.icon-bar{display:none}@media (max-width: 575.98px){.navbar-header{width:100%}.navbar-header .navbar-toggle{float:right}}.nav-tabs>li.active>a{color:#495057;background-color:#fff;border-color:#dee2e6 #dee2e6 #fff}.nav-pills>li.active>a{color:#fff;background-color:#0d6efd}.nav-stacked{flex-direction:column;-webkit-flex-direction:column}.progress-bar-default{background-color:#dee2e6;color:#000}.progress-bar-primary{background-color:#0d6efd;color:#fff}.progress-bar-secondary{background-color:#6c757d;color:#fff}.progress-bar-success{background-color:#198754;color:#fff}.progress-bar-info{background-color:#0dcaf0;color:#000}.progress-bar-warning{background-color:#ffc107;color:#000}.progress-bar-danger{background-color:#dc3545;color:#fff}.progress-bar-light{background-color:#f8f9fa;color:#000}.progress-bar-dark{background-color:#212529;color:#fff}@font-face{font-family:'Glyphicons Halflings';src:url("fonts/bootstrap/glyphicons-halflings-regular.eot");src:url("fonts/bootstrap/glyphicons-halflings-regular.eot?#iefix") format("embedded-opentype"),url("fonts/bootstrap/glyphicons-halflings-regular.woff2") format("woff2"),url("fonts/bootstrap/glyphicons-halflings-regular.woff") format("woff"),url("fonts/bootstrap/glyphicons-halflings-regular.ttf") format("truetype"),url("fonts/bootstrap/glyphicons-halflings-regular.svg#glyphicons_halflingsregular") format("svg")}.glyphicon{position:relative;top:1px;display:inline-block;font-family:'Glyphicons Halflings';font-style:normal;font-weight:normal;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.glyphicon-asterisk:before{content:"\2a"}.glyphicon-plus:before{content:"\2b"}.glyphicon-euro:before,.glyphicon-eur:before{content:"\20ac"}.glyphicon-minus:before{content:"\2212"}.glyphicon-cloud:before{content:"\2601"}.glyphicon-envelope:before{content:"\2709"}.glyphicon-pencil:before{content:"\270f"}.glyphicon-glass:before{content:"\e001"}.glyphicon-music:before{content:"\e002"}.glyphicon-search:before{content:"\e003"}.glyphicon-heart:before{content:"\e005"}.glyphicon-star:before{content:"\e006"}.glyphicon-star-empty:before{content:"\e007"}.glyphicon-user:before{content:"\e008"}.glyphicon-film:before{content:"\e009"}.glyphicon-th-large:before{content:"\e010"}.glyphicon-th:before{content:"\e011"}.glyphicon-th-list:before{content:"\e012"}.glyphicon-ok:before{content:"\e013"}.glyphicon-remove:before{content:"\e014"}.glyphicon-zoom-in:before{content:"\e015"}.glyphicon-zoom-out:before{content:"\e016"}.glyphicon-off:before{content:"\e017"}.glyphicon-signal:before{content:"\e018"}.glyphicon-cog:before{content:"\e019"}.glyphicon-trash:before{content:"\e020"}.glyphicon-home:before{content:"\e021"}.glyphicon-file:before{content:"\e022"}.glyphicon-time:before{content:"\e023"}.glyphicon-road:before{content:"\e024"}.glyphicon-download-alt:before{content:"\e025"}.glyphicon-download:before{content:"\e026"}.glyphicon-upload:before{content:"\e027"}.glyphicon-inbox:before{content:"\e028"}.glyphicon-play-circle:before{content:"\e029"}.glyphicon-repeat:before{content:"\e030"}.glyphicon-refresh:before{content:"\e031"}.glyphicon-list-alt:before{content:"\e032"}.glyphicon-lock:before{content:"\e033"}.glyphicon-flag:before{content:"\e034"}.glyphicon-headphones:before{content:"\e035"}.glyphicon-volume-off:before{content:"\e036"}.glyphicon-volume-down:before{content:"\e037"}.glyphicon-volume-up:before{content:"\e038"}.glyphicon-qrcode:before{content:"\e039"}.glyphicon-barcode:before{content:"\e040"}.glyphicon-tag:before{content:"\e041"}.glyphicon-tags:before{content:"\e042"}.glyphicon-book:before{content:"\e043"}.glyphicon-bookmark:before{content:"\e044"}.glyphicon-print:before{content:"\e045"}.glyphicon-camera:before{content:"\e046"}.glyphicon-font:before{content:"\e047"}.glyphicon-bold:before{content:"\e048"}.glyphicon-italic:before{content:"\e049"}.glyphicon-text-height:before{content:"\e050"}.glyphicon-text-width:before{content:"\e051"}.glyphicon-align-left:before{content:"\e052"}.glyphicon-align-center:before{content:"\e053"}.glyphicon-align-right:before{content:"\e054"}.glyphicon-align-justify:before{content:"\e055"}.glyphicon-list:before{content:"\e056"}.glyphicon-indent-left:before{content:"\e057"}.glyphicon-indent-right:before{content:"\e058"}.glyphicon-facetime-video:before{content:"\e059"}.glyphicon-picture:before{content:"\e060"}.glyphicon-map-marker:before{content:"\e062"}.glyphicon-adjust:before{content:"\e063"}.glyphicon-tint:before{content:"\e064"}.glyphicon-edit:before{content:"\e065"}.glyphicon-share:before{content:"\e066"}.glyphicon-check:before{content:"\e067"}.glyphicon-move:before{content:"\e068"}.glyphicon-step-backward:before{content:"\e069"}.glyphicon-fast-backward:before{content:"\e070"}.glyphicon-backward:before{content:"\e071"}.glyphicon-play:before{content:"\e072"}.glyphicon-pause:before{content:"\e073"}.glyphicon-stop:before{content:"\e074"}.glyphicon-forward:before{content:"\e075"}.glyphicon-fast-forward:before{content:"\e076"}.glyphicon-step-forward:before{content:"\e077"}.glyphicon-eject:before{content:"\e078"}.glyphicon-chevron-left:before{content:"\e079"}.glyphicon-chevron-right:before{content:"\e080"}.glyphicon-plus-sign:before{content:"\e081"}.glyphicon-minus-sign:before{content:"\e082"}.glyphicon-remove-sign:before{content:"\e083"}.glyphicon-ok-sign:before{content:"\e084"}.glyphicon-question-sign:before{content:"\e085"}.glyphicon-info-sign:before{content:"\e086"}.glyphicon-screenshot:before{content:"\e087"}.glyphicon-remove-circle:before{content:"\e088"}.glyphicon-ok-circle:before{content:"\e089"}.glyphicon-ban-circle:before{content:"\e090"}.glyphicon-arrow-left:before{content:"\e091"}.glyphicon-arrow-right:before{content:"\e092"}.glyphicon-arrow-up:before{content:"\e093"}.glyphicon-arrow-down:before{content:"\e094"}.glyphicon-share-alt:before{content:"\e095"}.glyphicon-resize-full:before{content:"\e096"}.glyphicon-resize-small:before{content:"\e097"}.glyphicon-exclamation-sign:before{content:"\e101"}.glyphicon-gift:before{content:"\e102"}.glyphicon-leaf:before{content:"\e103"}.glyphicon-fire:before{content:"\e104"}.glyphicon-eye-open:before{content:"\e105"}.glyphicon-eye-close:before{content:"\e106"}.glyphicon-warning-sign:before{content:"\e107"}.glyphicon-plane:before{content:"\e108"}.glyphicon-calendar:before{content:"\e109"}.glyphicon-random:before{content:"\e110"}.glyphicon-comment:before{content:"\e111"}.glyphicon-magnet:before{content:"\e112"}.glyphicon-chevron-up:before{content:"\e113"}.glyphicon-chevron-down:before{content:"\e114"}.glyphicon-retweet:before{content:"\e115"}.glyphicon-shopping-cart:before{content:"\e116"}.glyphicon-folder-close:before{content:"\e117"}.glyphicon-folder-open:before{content:"\e118"}.glyphicon-resize-vertical:before{content:"\e119"}.glyphicon-resize-horizontal:before{content:"\e120"}.glyphicon-hdd:before{content:"\e121"}.glyphicon-bullhorn:before{content:"\e122"}.glyphicon-bell:before{content:"\e123"}.glyphicon-certificate:before{content:"\e124"}.glyphicon-thumbs-up:before{content:"\e125"}.glyphicon-thumbs-down:before{content:"\e126"}.glyphicon-hand-right:before{content:"\e127"}.glyphicon-hand-left:before{content:"\e128"}.glyphicon-hand-up:before{content:"\e129"}.glyphicon-hand-down:before{content:"\e130"}.glyphicon-circle-arrow-right:before{content:"\e131"}.glyphicon-circle-arrow-left:before{content:"\e132"}.glyphicon-circle-arrow-up:before{content:"\e133"}.glyphicon-circle-arrow-down:before{content:"\e134"}.glyphicon-globe:before{content:"\e135"}.glyphicon-wrench:before{content:"\e136"}.glyphicon-tasks:before{content:"\e137"}.glyphicon-filter:before{content:"\e138"}.glyphicon-briefcase:before{content:"\e139"}.glyphicon-fullscreen:before{content:"\e140"}.glyphicon-dashboard:before{content:"\e141"}.glyphicon-paperclip:before{content:"\e142"}.glyphicon-heart-empty:before{content:"\e143"}.glyphicon-link:before{content:"\e144"}.glyphicon-phone:before{content:"\e145"}.glyphicon-pushpin:before{content:"\e146"}.glyphicon-usd:before{content:"\e148"}.glyphicon-gbp:before{content:"\e149"}.glyphicon-sort:before{content:"\e150"}.glyphicon-sort-by-alphabet:before{content:"\e151"}.glyphicon-sort-by-alphabet-alt:before{content:"\e152"}.glyphicon-sort-by-order:before{content:"\e153"}.glyphicon-sort-by-order-alt:before{content:"\e154"}.glyphicon-sort-by-attributes:before{content:"\e155"}.glyphicon-sort-by-attributes-alt:before{content:"\e156"}.glyphicon-unchecked:before{content:"\e157"}.glyphicon-expand:before{content:"\e158"}.glyphicon-collapse-down:before{content:"\e159"}.glyphicon-collapse-up:before{content:"\e160"}.glyphicon-log-in:before{content:"\e161"}.glyphicon-flash:before{content:"\e162"}.glyphicon-log-out:before{content:"\e163"}.glyphicon-new-window:before{content:"\e164"}.glyphicon-record:before{content:"\e165"}.glyphicon-save:before{content:"\e166"}.glyphicon-open:before{content:"\e167"}.glyphicon-saved:before{content:"\e168"}.glyphicon-import:before{content:"\e169"}.glyphicon-export:before{content:"\e170"}.glyphicon-send:before{content:"\e171"}.glyphicon-floppy-disk:before{content:"\e172"}.glyphicon-floppy-saved:before{content:"\e173"}.glyphicon-floppy-remove:before{content:"\e174"}.glyphicon-floppy-save:before{content:"\e175"}.glyphicon-floppy-open:before{content:"\e176"}.glyphicon-credit-card:before{content:"\e177"}.glyphicon-transfer:before{content:"\e178"}.glyphicon-cutlery:before{content:"\e179"}.glyphicon-header:before{content:"\e180"}.glyphicon-compressed:before{content:"\e181"}.glyphicon-earphone:before{content:"\e182"}.glyphicon-phone-alt:before{content:"\e183"}.glyphicon-tower:before{content:"\e184"}.glyphicon-stats:before{content:"\e185"}.glyphicon-sd-video:before{content:"\e186"}.glyphicon-hd-video:before{content:"\e187"}.glyphicon-subtitles:before{content:"\e188"}.glyphicon-sound-stereo:before{content:"\e189"}.glyphicon-sound-dolby:before{content:"\e190"}.glyphicon-sound-5-1:before{content:"\e191"}.glyphicon-sound-6-1:before{content:"\e192"}.glyphicon-sound-7-1:before{content:"\e193"}.glyphicon-copyright-mark:before{content:"\e194"}.glyphicon-registration-mark:before{content:"\e195"}.glyphicon-cloud-download:before{content:"\e197"}.glyphicon-cloud-upload:before{content:"\e198"}.glyphicon-tree-conifer:before{content:"\e199"}.glyphicon-tree-deciduous:before{content:"\e200"}.glyphicon-cd:before{content:"\e201"}.glyphicon-save-file:before{content:"\e202"}.glyphicon-open-file:before{content:"\e203"}.glyphicon-level-up:before{content:"\e204"}.glyphicon-copy:before{content:"\e205"}.glyphicon-paste:before{content:"\e206"}.glyphicon-alert:before{content:"\e209"}.glyphicon-equalizer:before{content:"\e210"}.glyphicon-king:before{content:"\e211"}.glyphicon-queen:before{content:"\e212"}.glyphicon-pawn:before{content:"\e213"}.glyphicon-bishop:before{content:"\e214"}.glyphicon-knight:before{content:"\e215"}.glyphicon-baby-formula:before{content:"\e216"}.glyphicon-tent:before{content:"\26fa"}.glyphicon-blackboard:before{content:"\e218"}.glyphicon-bed:before{content:"\e219"}.glyphicon-apple:before{content:"\f8ff"}.glyphicon-erase:before{content:"\e221"}.glyphicon-hourglass:before{content:"\231b"}.glyphicon-lamp:before{content:"\e223"}.glyphicon-duplicate:before{content:"\e224"}.glyphicon-piggy-bank:before{content:"\e225"}.glyphicon-scissors:before{content:"\e226"}.glyphicon-bitcoin:before{content:"\e227"}.glyphicon-btc:before{content:"\e227"}.glyphicon-xbt:before{content:"\e227"}.glyphicon-yen:before{content:"\00a5"}.glyphicon-jpy:before{content:"\00a5"}.glyphicon-ruble:before{content:"\20bd"}.glyphicon-rub:before{content:"\20bd"}.glyphicon-scale:before{content:"\e230"}.glyphicon-ice-lolly:before{content:"\e231"}.glyphicon-ice-lolly-tasted:before{content:"\e232"}.glyphicon-education:before{content:"\e233"}.glyphicon-option-horizontal:before{content:"\e234"}.glyphicon-option-vertical:before{content:"\e235"}.glyphicon-menu-hamburger:before{content:"\e236"}.glyphicon-modal-window:before{content:"\e237"}.glyphicon-oil:before{content:"\e238"}.glyphicon-grain:before{content:"\e239"}.glyphicon-sunglasses:before{content:"\e240"}.glyphicon-text-size:before{content:"\e241"}.glyphicon-text-color:before{content:"\e242"}.glyphicon-text-background:before{content:"\e243"}.glyphicon-object-align-top:before{content:"\e244"}.glyphicon-object-align-bottom:before{content:"\e245"}.glyphicon-object-align-horizontal:before{content:"\e246"}.glyphicon-object-align-left:before{content:"\e247"}.glyphicon-object-align-vertical:before{content:"\e248"}.glyphicon-object-align-right:before{content:"\e249"}.glyphicon-triangle-right:before{content:"\e250"}.glyphicon-triangle-left:before{content:"\e251"}.glyphicon-triangle-bottom:before{content:"\e252"}.glyphicon-triangle-top:before{content:"\e253"}.glyphicon-console:before{content:"\e254"}.glyphicon-superscript:before{content:"\e255"}.glyphicon-subscript:before{content:"\e256"}.glyphicon-menu-left:before{content:"\e257"}.glyphicon-menu-right:before{content:"\e258"}.glyphicon-menu-down:before{content:"\e259"}.glyphicon-menu-up:before{content:"\e260"}.form-group{margin-bottom:1rem}.input-daterange .input-group-addon.input-group-prepend.input-group-append{padding:inherit;line-height:inherit;text-shadow:inherit;border-width:0}.input-daterange .input-group-addon.input-group-prepend.input-group-append .input-group-text{border-radius:0}pre.shiny-code{padding:0.5rem}.section.level1,.section.level2,.section.level3,section.level1,section.level2,section.level3{margin-top:1.5rem}.section.level4,.section.level5,.section.level6,section.level4,section.level5,section.level6{margin-top:1rem}.accordion .accordion-icon:not(:empty){margin-right:0.25rem;display:flex}.accordion .accordion-button:not(.collapsed){box-shadow:none}.accordion .accordion-button:not(.collapsed):focus{box-shadow:var(--bs-accordion-btn-focus-box-shadow)}.bslib-card .card-body+.card-body{padding-top:0}.bslib-card .card-body{overflow:auto}.bslib-card .card-body p{margin-top:0}.bslib-card .card-body p:last-child{margin-bottom:0}.bslib-card .card-body{max-height:var(--bslib-card-body-max-height, none)}.bslib-card.bslib-full-screen>.card-body{max-height:var(--bslib-card-body-max-height-full-screen, none)}.bslib-card .card-header .form-group{margin-bottom:0}.bslib-card .card-header .selectize-control{margin-bottom:0}.bslib-card .card-header .selectize-control .item{margin-right:1.15rem}.bslib-card .card-footer{margin-top:auto}.bslib-card .bslib-navs-card-title{display:flex;flex-wrap:wrap;justify-content:space-between;align-items:center}.bslib-card .bslib-navs-card-title .nav{margin-left:auto}.bslib-card .bslib-sidebar-layout:not([data-bslib-sidebar-border="true"]){border:none}.bslib-card .bslib-sidebar-layout:not([data-bslib-sidebar-border-radius="true"]){border-top-left-radius:0;border-top-right-radius:0}.bslib-full-screen{position:fixed;inset:3.5rem 1rem 1rem;height:auto !important;max-height:none !important;width:auto !important;z-index:1070}.bslib-full-screen-enter{display:none;position:absolute;bottom:1px;right:3px;margin:0.5rem;padding:0.55rem !important;font-size:.8rem;cursor:pointer;opacity:.6;color:rgba(var(--bs-body-bg-rgb), 1);z-index:1070}.bslib-full-screen-enter:hover{opacity:1}.card:hover:not(.bslib-full-screen)>.bslib-full-screen-enter,.well:hover:not(.bslib-full-screen)>.bslib-full-screen-enter{display:block}.bslib-has-full-screen .card:hover>.bslib-full-screen-enter,.bslib-has-full-screen .well:hover>.bslib-full-screen-enter{display:none}@media (max-width: 575.98px){.bslib-full-screen-enter{display:none !important}}.bslib-full-screen-exit{position:relative;top:1.35rem;font-size:0.9rem;cursor:pointer;text-decoration:none;display:flex;float:right;margin-right:2.15rem;align-items:center;color:rgba(var(--bs-body-bg-rgb), 0.8)}.bslib-full-screen-exit:hover{color:rgba(var(--bs-body-bg-rgb), 1)}.bslib-full-screen-exit svg{margin-left:0.5rem;font-size:1.5rem}#bslib-full-screen-overlay{position:fixed;inset:0;background-color:rgba(var(--bs-body-color-rgb), 0.6);backdrop-filter:blur(2px);-webkit-backdrop-filter:blur(2px);z-index:1069;animation:bslib-full-screen-overlay-enter 400ms cubic-bezier(0.6, 0.02, 0.65, 1) forwards}@keyframes bslib-full-screen-overlay-enter{0%{opacity:0}100%{opacity:1}}.tab-content>.tab-pane.html-fill-container{display:none}.tab-content>.active.html-fill-container{display:flex}.tab-content.html-fill-container{padding:0}.bslib-page-fill{width:100%;height:100%;margin:0;padding:1rem;gap:1rem}.bslib-page-title{background-color:#212529;color:#fff;font-size:1.5rem;font-weight:300;padding:1rem;padding-left:1.5rem;margin-bottom:0}@media (max-width: 575.98px){.bslib-page-fill{height:var(--bslib-page-fill-mobile-height, auto)}}:root{--bslib-mb-spacer: 1rem}.bslib-mb-spacer{margin-bottom:var(--bslib-mb-spacer)}.bslib-gap-spacing{gap:var(--bslib-mb-spacer)}.bslib-gap-spacing>.bslib-mb-spacer,.bslib-gap-spacing>.form-group,.bslib-gap-spacing>p,.bslib-gap-spacing>pre{margin-bottom:0}.bslib-grid{display:grid !important;gap:1rem;height:var(--bslib-grid-height)}@media (max-width: 575.98px){.bslib-grid{grid-template-columns:1fr !important;height:var(--bslib-grid-height-mobile)}}.bslib-grid.grid{grid-template-rows:unset;grid-auto-rows:var(--bslib-grid--row-heights);--bslib-grid--row-heights--xs: unset;--bslib-grid--row-heights--sm: unset;--bslib-grid--row-heights--md: unset;--bslib-grid--row-heights--lg: unset;--bslib-grid--row-heights--xl: unset;--bslib-grid--row-heights--xxl: unset}.bslib-grid.grid.bslib-grid--row-heights--xs{--bslib-grid--row-heights: var(--bslib-grid--row-heights--xs)}@media (min-width: 576px){.bslib-grid.grid.bslib-grid--row-heights--sm{--bslib-grid--row-heights: var(--bslib-grid--row-heights--sm)}}@media (min-width: 768px){.bslib-grid.grid.bslib-grid--row-heights--md{--bslib-grid--row-heights: var(--bslib-grid--row-heights--md)}}@media (min-width: 992px){.bslib-grid.grid.bslib-grid--row-heights--lg{--bslib-grid--row-heights: var(--bslib-grid--row-heights--lg)}}@media (min-width: 1200px){.bslib-grid.grid.bslib-grid--row-heights--xl{--bslib-grid--row-heights: var(--bslib-grid--row-heights--xl)}}@media (min-width: 1400px){.bslib-grid.grid.bslib-grid--row-heights--xxl{--bslib-grid--row-heights: var(--bslib-grid--row-heights--xxl)}}.bslib-grid-item{grid-column:auto/span 1}@media (max-width: 767.98px){.bslib-grid-item{grid-column:1 / -1}}@media (max-width: 575.98px){.bslib-grid.grid{height:unset !important;grid-auto-rows:var(--bslib-grid--row-heights--xs, auto)}}.bslib-sidebar-layout{--bslib-sidebar-transition: grid-template-columns ease-in-out 500ms;--bslib-sidebar-border: var(--bs-card-border-width, 1px) solid var(--bs-card-border-color, var(--bs-border-color-translucent));--bslib-sidebar-border-radius: var(--bs-border-radius);--bslib-sidebar-vert-border: var(--bs-card-border-width, 1px) solid var(--bs-card-border-color, var(--bs-border-color-translucent));--bslib-sidebar-bg: #f7f7f7;--bslib-sidebar-fg: #000;--bslib-collapse-toggle-border: var(--bs-card-border-width, 1px) solid var(--bs-card-border-color, var(--bs-border-color-translucent));--bslib-collapse-toggle-transform: 90deg;--bslib-collapse-toggle-right-transform: -90deg;display:grid !important;grid-template-columns:Min(calc(100% - 1rem), var(--bslib-sidebar-width, 250px)) minmax(0, 1fr);position:relative;transition:var(--bslib-sidebar-transition);border:var(--bslib-sidebar-border);border-radius:var(--bslib-sidebar-border-radius)}@media (prefers-reduced-motion: reduce){.bslib-sidebar-layout{transition:none}}.bslib-sidebar-layout[data-bslib-sidebar-border="false"]{border:none}.bslib-sidebar-layout[data-bslib-sidebar-border-radius="false"]{border-radius:initial}.bslib-sidebar-layout>.main,.bslib-sidebar-layout>.sidebar{grid-row:1 / 2;border-radius:inherit;overflow:auto}.bslib-sidebar-layout>.main{grid-column:2 / 3;border-top-left-radius:0;border-bottom-left-radius:0;padding:1.5rem}.bslib-sidebar-layout>.sidebar{grid-column:1 / 2;width:100%;height:100%;border-right:var(--bslib-sidebar-vert-border);border-top-right-radius:0;border-bottom-right-radius:0;background-color:var(--bslib-sidebar-bg);color:var(--bslib-sidebar-fg)}.bslib-sidebar-layout>.sidebar>.sidebar-content{display:flex;flex-direction:column;padding:1.5rem}.bslib-sidebar-layout>.sidebar>.sidebar-content>:last-child:not(.sidebar-title){margin-bottom:0}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion{margin-left:-1.5rem;margin-right:-1.5rem}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion:first-child{margin-top:-1.5rem}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion:last-child{margin-bottom:-1.5rem}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion:not(:last-child){margin-bottom:1rem}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion .accordion-body{display:flex;flex-direction:column}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion:not(:first-child) .accordion-item:first-child{border-top:var(--bs-accordion-border-width) solid var(--bs-accordion-border-color)}.bslib-sidebar-layout>.sidebar>.sidebar-content>.accordion:not(:last-child) .accordion-item:last-child{border-bottom:var(--bs-accordion-border-width) solid var(--bs-accordion-border-color)}.bslib-sidebar-layout>.sidebar>.sidebar-content>.sidebar-title+.accordion{margin-top:calc(-1rem - var(--bs-card-border-width, 1px))}.bslib-sidebar-layout>.sidebar>.sidebar-content>.sidebar-title:has(+.accordion){border-bottom:none}.bslib-sidebar-layout>.sidebar .shiny-input-container{width:100%}.bslib-sidebar-layout>.collapse-toggle{grid-row:1 / 2;grid-column:1 / 2;display:inline-flex;align-items:center;position:absolute;right:-1rem;bottom:calc(1.5rem + var(--bslib-sidebar-overlap-counter, 0) * calc(1rem + 1.5rem));border:var(--bslib-collapse-toggle-border);border-left:none;border-radius:0 var(--bs-border-radius) var(--bs-border-radius) 0;padding:7px 0;background-color:var(--bslib-sidebar-bg);color:var(--bslib-sidebar-fg)}.bslib-sidebar-layout>.collapse-toggle>.collapse-icon{opacity:0.8;width:1rem;height:1rem;transform:rotate(var(--bslib-collapse-toggle-transform));transition:transform cubic-bezier(0.68, -0.55, 0.27, 1.55) 500ms}.bslib-sidebar-layout>.collapse-toggle:hover>.collapse-icon{opacity:1}.bslib-sidebar-layout .sidebar-title{font-size:1.25rem;line-height:1.25;margin-top:0;margin-bottom:1rem;padding-bottom:1rem;border-bottom:var(--bslib-sidebar-border)}.bslib-sidebar-layout.sidebar-right{grid-template-columns:minmax(0, 1fr) Min(calc(100% - 1rem), var(--bslib-sidebar-width, 250px))}.bslib-sidebar-layout.sidebar-right>.main{grid-column:1 / 2;border-top-right-radius:0;border-bottom-right-radius:0;border-top-left-radius:inherit;border-bottom-left-radius:inherit}.bslib-sidebar-layout.sidebar-right>.sidebar{grid-column:2 / 3;border-right:none;border-left:var(--bslib-sidebar-vert-border);border-top-left-radius:0;border-bottom-left-radius:0}.bslib-sidebar-layout.sidebar-right>.collapse-toggle{grid-column:2 / 3;left:-1rem;right:unset;border-radius:var(--bs-border-radius) 0 0 var(--bs-border-radius);border-right:none;border-left:var(--bslib-collapse-toggle-border)}.bslib-sidebar-layout.sidebar-right>.collapse-toggle>.collapse-icon{transform:rotate(var(--bslib-collapse-toggle-right-transform))}.bslib-sidebar-layout.sidebar-collapsed{--bslib-collapse-toggle-transform: -90deg;--bslib-collapse-toggle-right-transform: 90deg;--bslib-sidebar-vert-border: none;grid-template-columns:0 minmax(0, 1fr)}.bslib-sidebar-layout.sidebar-collapsed.sidebar-right{grid-template-columns:minmax(0, 1fr) 0}.bslib-sidebar-layout.sidebar-collapsed:not(.transitioning)>.sidebar>*{display:none}.bslib-sidebar-layout.sidebar-collapsed>.main{border-radius:inherit}.bslib-sidebar-layout.sidebar-collapsed>.collapse-toggle{right:calc(-1rem - var(--bs-card-border-width, 1px))}.bslib-sidebar-layout.sidebar-collapsed.sidebar-right>.collapse-toggle{left:calc(-1rem - var(--bs-card-border-width, 1px));right:unset}@media (min-width: 576px){.bslib-sidebar-layout.transitioning>.sidebar>.sidebar-content{display:none}}@media (max-width: 575.98px){.bslib-sidebar-layout,.bslib-sidebar-layout.sidebar-right{--bslib-sidebar-vert-border: none;--bslib-sidebar-horiz-border: var(--bs-card-border-width, 1px) solid var(--bs-card-border-color, var(--bs-border-color-translucent));--bslib-collapse-toggle-transform: -180deg;--bslib-collapse-toggle-right-transform: -180deg;grid-template-columns:1fr !important;grid-template-rows:fit-content(var(--bslib-sidebar-max-height-mobile, auto)) minmax(0, 1fr)}.bslib-sidebar-layout[data-bslib-sidebar-open="desktop"],.bslib-sidebar-layout.sidebar-right[data-bslib-sidebar-open="desktop"]{--bslib-sidebar-js-init-collapsed: true}.bslib-sidebar-layout>.sidebar,.bslib-sidebar-layout.sidebar-right>.sidebar{grid-row:1 / 2;grid-column:1 / 2;width:100%;border:none;border-bottom:var(--bslib-sidebar-horiz-border);border-radius:0}.bslib-sidebar-layout>.main,.bslib-sidebar-layout.sidebar-right>.main{grid-row:2 / 3;grid-column:1 / 2;border-top-left-radius:0;border-top-right-radius:0;border-bottom-right-radius:inherit;border-bottom-left-radius:inherit}.bslib-sidebar-layout>.collapse-toggle,.bslib-sidebar-layout.sidebar-right>.collapse-toggle{grid-row:2 / 3;grid-column:1 / 2;border-top:none !important;border:var(--bslib-collapse-toggle-border);border-radius:0 0 var(--bs-border-radius) var(--bs-border-radius);padding:0 4px}.bslib-sidebar-layout>.collapse-toggle>.collapse-icon,.bslib-sidebar-layout.sidebar-right>.collapse-toggle>.collapse-icon{transition-duration:165ms}.bslib-sidebar-layout>.collapse-toggle,.bslib-sidebar-layout.sidebar-right>.collapse-toggle,.bslib-sidebar-layout.sidebar-right>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-right>.collapse-toggle{top:calc(-1 * var(--bs-card-border-width, 1px))}.bslib-sidebar-layout.sidebar-collapsed>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-right.sidebar-collapsed>.collapse-toggle{top:0}.bslib-sidebar-layout>.collapse-toggle,.bslib-sidebar-layout.sidebar-collapsed>.collapse-toggle,.bslib-sidebar-layout.sidebar-right>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed>.collapse-toggle,.bslib-sidebar-layout.sidebar-right>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-right>.collapse-toggle,.bslib-sidebar-layout.sidebar-right.sidebar-right.sidebar-collapsed>.collapse-toggle{right:calc(1.5rem + var(--bslib-sidebar-counter, 0) * calc(1rem + 1.5rem));bottom:initial;left:initial}.bslib-sidebar-layout.sidebar-collapsed,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed{--bslib-collapse-toggle-transform: 0deg;--bslib-collapse-toggle-right-transform: 0deg;grid-template-rows:0 minmax(0, 1fr)}.bslib-sidebar-layout.sidebar-collapsed>.main,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed>.main{border-top-left-radius:inherit;border-top-right-radius:inherit}.bslib-sidebar-layout.sidebar-collapsed>.sidebar,.bslib-sidebar-layout.sidebar-right.sidebar-collapsed>.sidebar{border-bottom:none}}.navbar+.container-fluid:has(>.tab-content>.tab-pane.active.html-fill-container),.navbar+.container-sm:has(>.tab-content>.tab-pane.active.html-fill-container),.navbar+.container-md:has(>.tab-content>.tab-pane.active.html-fill-container),.navbar+.container-lg:has(>.tab-content>.tab-pane.active.html-fill-container),.navbar+.container-xl:has(>.tab-content>.tab-pane.active.html-fill-container),.navbar+.container-xxl:has(>.tab-content>.tab-pane.active.html-fill-container){padding-left:0;padding-right:0}.navbar+.container-fluid>.tab-content>.tab-pane.active.html-fill-container,.navbar+.container-sm>.tab-content>.tab-pane.active.html-fill-container,.navbar+.container-md>.tab-content>.tab-pane.active.html-fill-container,.navbar+.container-lg>.tab-content>.tab-pane.active.html-fill-container,.navbar+.container-xl>.tab-content>.tab-pane.active.html-fill-container,.navbar+.container-xxl>.tab-content>.tab-pane.active.html-fill-container{padding:1rem;gap:1rem}.navbar+.container-fluid>.tab-content>.tab-pane.active.html-fill-container:has(>.bslib-sidebar-layout:only-child),.navbar+.container-sm>.tab-content>.tab-pane.active.html-fill-container:has(>.bslib-sidebar-layout:only-child),.navbar+.container-md>.tab-content>.tab-pane.active.html-fill-container:has(>.bslib-sidebar-layout:only-child),.navbar+.container-lg>.tab-content>.tab-pane.active.html-fill-container:has(>.bslib-sidebar-layout:only-child),.navbar+.container-xl>.tab-content>.tab-pane.active.html-fill-container:has(>.bslib-sidebar-layout:only-child),.navbar+.container-xxl>.tab-content>.tab-pane.active.html-fill-container:has(>.bslib-sidebar-layout:only-child){padding:0}.navbar+.container-fluid>.tab-content>.tab-pane.active.html-fill-container>.bslib-sidebar-layout:only-child:not([data-bslib-sidebar-border="true"]),.navbar+.container-sm>.tab-content>.tab-pane.active.html-fill-container>.bslib-sidebar-layout:only-child:not([data-bslib-sidebar-border="true"]),.navbar+.container-md>.tab-content>.tab-pane.active.html-fill-container>.bslib-sidebar-layout:only-child:not([data-bslib-sidebar-border="true"]),.navbar+.container-lg>.tab-content>.tab-pane.active.html-fill-container>.bslib-sidebar-layout:only-child:not([data-bslib-sidebar-border="true"]),.navbar+.container-xl>.tab-content>.tab-pane.active.html-fill-container>.bslib-sidebar-layout:only-child:not([data-bslib-sidebar-border="true"]),.navbar+.container-xxl>.tab-content>.tab-pane.active.html-fill-container>.bslib-sidebar-layout:only-child:not([data-bslib-sidebar-border="true"]){border-left:none;border-right:none;border-bottom:none}.navbar+.container-fluid>.tab-content>.tab-pane.active.html-fill-container>.bslib-sidebar-layout:only-child:not([data-bslib-sidebar-border-radius="true"]),.navbar+.container-sm>.tab-content>.tab-pane.active.html-fill-container>.bslib-sidebar-layout:only-child:not([data-bslib-sidebar-border-radius="true"]),.navbar+.container-md>.tab-content>.tab-pane.active.html-fill-container>.bslib-sidebar-layout:only-child:not([data-bslib-sidebar-border-radius="true"]),.navbar+.container-lg>.tab-content>.tab-pane.active.html-fill-container>.bslib-sidebar-layout:only-child:not([data-bslib-sidebar-border-radius="true"]),.navbar+.container-xl>.tab-content>.tab-pane.active.html-fill-container>.bslib-sidebar-layout:only-child:not([data-bslib-sidebar-border-radius="true"]),.navbar+.container-xxl>.tab-content>.tab-pane.active.html-fill-container>.bslib-sidebar-layout:only-child:not([data-bslib-sidebar-border-radius="true"]){border-radius:0}.navbar+div>.bslib-sidebar-layout{border-top:var(--bslib-sidebar-border)}.bslib-value-box .value-box-grid{grid-template-columns:var(--bslib-value-box-widths)}.bslib-value-box .value-box-showcase{align-items:center;justify-content:center;margin-top:auto;margin-bottom:auto;padding:1rem;max-height:var(--bslib-value-box-max-height)}.bslib-value-box .value-box-showcase .bi,.bslib-value-box .value-box-showcase .fa{opacity:.85}.bslib-value-box .value-box-showcase .bi{font-size:5rem}.bslib-value-box .value-box-showcase .fa{font-size:4rem}.bslib-value-box .value-box-showcase.showcase-top-right{align-items:end;padding-left:0;padding-bottom:0}.bslib-value-box .value-box-area{justify-content:center;padding:1.5rem 1rem;font-size:.9rem;font-weight:500}.bslib-value-box .value-box-area *{color:inherit;margin-bottom:0;margin-top:0}.bslib-value-box .value-box-area>:first-child{color:inherit}.bslib-value-box .value-box-area>:first-child::after{content:'\00a0 '}.bslib-value-box .value-box-area>:nth-child(2){color:inherit}.bslib-value-box .value-box-area>:nth-child(2)::after{content:'\00a0 '}.bslib-value-box .value-box-area.border-start{border-color:rgba(222,226,230,0.3) !important}.bslib-value-box.bslib-full-screen .value-box-grid{grid-template-columns:var(--bslib-value-box-widths-full-screen)}.bslib-value-box.bslib-full-screen .value-box-showcase{max-height:var(--bslib-value-box-max-height-full-screen)}.bslib-value-box:not(.bslib-full-screen) .value-box-showcase.showcase-top-right{margin-top:0}@media (max-width: 575.98px){.bslib-value-box .value-box-grid{grid-template-columns:var(--bslib-value-box-widths) !important}}@media (min-width: 576px){.nav:not(.nav-hidden){display:flex !important;display:-webkit-flex !important}.nav:not(.nav-hidden):not(.nav-stacked):not(.flex-column){float:none !important}.nav:not(.nav-hidden):not(.nav-stacked):not(.flex-column)>.bslib-nav-spacer{margin-left:auto !important}.nav:not(.nav-hidden):not(.nav-stacked):not(.flex-column)>.form-inline{margin-top:auto;margin-bottom:auto}.nav:not(.nav-hidden).nav-stacked{flex-direction:column;-webkit-flex-direction:column;height:100%}.nav:not(.nav-hidden).nav-stacked>.bslib-nav-spacer{margin-top:auto !important}}
```

### Comparing `shiny-0.3.3/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot` & `shiny-0.4.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg` & `shiny-0.4.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf` & `shiny-0.4.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff` & `shiny-0.4.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2` & `shiny-0.4.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/css/bootstrap-datepicker3.css` & `shiny-0.4.0/shiny/www/shared/datepicker/css/bootstrap-datepicker3.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css` & `shiny-0.4.0/shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/bootstrap-datepicker.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.az.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.az.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bg.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bg.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bm.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bm.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bn.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bn.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ca.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ca.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cs.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cs.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.da.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.da.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.de.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.de.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.el.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.el.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-AU.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-AU.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-CA.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-CA.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-GB.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-GB.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-IE.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-IE.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-NZ.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-NZ.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-ZA.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-ZA.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eo.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eo.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.es.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.es.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.et.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.et.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eu.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eu.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fa.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fa.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fi.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fi.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr-CH.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr-CH.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.he.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.he.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hi.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hi.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hu.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hu.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hy.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hy.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ka.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ka.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kh.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kh.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kk.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kk.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.km.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.km.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ko.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ko.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kr.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kr.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lt.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lt.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lv.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lv.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mk.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mk.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mn.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mn.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl-BE.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl-BE.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.no.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.no.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.oc.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.oc.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pl.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pl.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs-latin.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs-latin.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ru.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ru.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.si.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.si.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sq.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sq.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ta.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ta.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tg.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tg.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.th.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.th.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tk.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tk.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uk.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uk.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-cyrl.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-cyrl.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-latn.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-latn.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.vi.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.vi.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-CN.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-CN.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-TW.min.js` & `shiny-0.4.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-TW.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/scss/build3.scss` & `shiny-0.4.0/shiny/www/shared/datepicker/scss/build3.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/datepicker/scss/datepicker3.scss` & `shiny-0.4.0/shiny/www/shared/datepicker/scss/datepicker3.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/highlight/LICENSE` & `shiny-0.4.0/shiny/www/shared/highlight/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/highlight/classref.txt` & `shiny-0.4.0/shiny/www/shared/highlight/classref.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/highlight/highlight.pack.js` & `shiny-0.4.0/shiny/www/shared/highlight/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/highlight/rstudio.css` & `shiny-0.4.0/shiny/www/shared/highlight/rstudio.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/ionrangeslider/css/ion.rangeSlider.css` & `shiny-0.4.0/shiny/www/shared/ionrangeslider/css/ion.rangeSlider.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.js` & `shiny-0.4.0/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.min.js` & `shiny-0.4.0/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/ionrangeslider/scss/_base.scss` & `shiny-0.4.0/shiny/www/shared/ionrangeslider/scss/_base.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/ionrangeslider/scss/shiny.scss` & `shiny-0.4.0/shiny/www/shared/ionrangeslider/scss/shiny.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jquery/jquery-3.6.0.js` & `shiny-0.4.0/shiny/www/shared/jquery/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jquery/jquery-3.6.0.min.js` & `shiny-0.4.0/shiny/www/shared/jquery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jquery/jquery-3.6.0.min.map` & `shiny-0.4.0/shiny/www/shared/jquery/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/AUTHORS.txt` & `shiny-0.4.0/shiny/www/shared/jqueryui/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/LICENSE.txt` & `shiny-0.4.0/shiny/www/shared/jqueryui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/images/ui-icons_444444_256x240.png` & `shiny-0.4.0/shiny/www/shared/jqueryui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/images/ui-icons_555555_256x240.png` & `shiny-0.4.0/shiny/www/shared/jqueryui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/images/ui-icons_777620_256x240.png` & `shiny-0.4.0/shiny/www/shared/jqueryui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/images/ui-icons_777777_256x240.png` & `shiny-0.4.0/shiny/www/shared/jqueryui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/images/ui-icons_cc0000_256x240.png` & `shiny-0.4.0/shiny/www/shared/jqueryui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/images/ui-icons_ffffff_256x240.png` & `shiny-0.4.0/shiny/www/shared/jqueryui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/index.html` & `shiny-0.4.0/shiny/www/shared/jqueryui/index.html`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.css` & `shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.js` & `shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.min.css` & `shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.min.js` & `shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.structure.css` & `shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.structure.min.css` & `shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.theme.css` & `shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/jqueryui/jquery-ui.theme.min.css` & `shiny-0.4.0/shiny/www/shared/jqueryui/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/requirejs/require.min.js` & `shiny-0.4.0/shiny/www/shared/requirejs/require.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.js` & `shiny-0.4.0/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.min.js` & `shiny-0.4.0/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/selectize/css/selectize.bootstrap3.css` & `shiny-0.4.0/shiny/www/shared/selectize/css/selectize.bootstrap3.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/selectize/js/selectize.min.js` & `shiny-0.4.0/shiny/www/shared/selectize/js/selectize.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/selectize/scss/plugins/dropdown_header.scss` & `shiny-0.4.0/shiny/www/shared/selectize/scss/plugins/dropdown_header.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/selectize/scss/plugins/remove_button.scss` & `shiny-0.4.0/shiny/www/shared/selectize/scss/plugins/remove_button.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/selectize/scss/selectize.bootstrap3.scss` & `shiny-0.4.0/shiny/www/shared/selectize/scss/selectize.bootstrap3.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/selectize/scss/selectize.bootstrap4.scss` & `shiny-0.4.0/shiny/www/shared/selectize/scss/selectize.bootstrap4.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/selectize/scss/selectize.default.scss` & `shiny-0.4.0/shiny/www/shared/selectize/scss/selectize.default.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/selectize/scss/selectize.scss` & `shiny-0.4.0/shiny/www/shared/selectize/scss/selectize.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny-autoreload.js` & `shiny-0.4.0/shiny/www/shared/shiny-autoreload.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny-autoreload.js.map` & `shiny-0.4.0/shiny/www/shared/shiny-autoreload.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny-showcase.css` & `shiny-0.4.0/shiny/www/shared/shiny-showcase.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny-showcase.js` & `shiny-0.4.0/shiny/www/shared/shiny-showcase.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny-showcase.js.map` & `shiny-0.4.0/shiny/www/shared/shiny-showcase.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny-testmode.js.map` & `shiny-0.4.0/shiny/www/shared/shiny-testmode.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny.js` & `shiny-0.4.0/shiny/www/shared/shiny.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny.js.map` & `shiny-0.4.0/shiny/www/shared/shiny.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny.min.css` & `shiny-0.4.0/shiny/www/shared/shiny.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny.min.js` & `shiny-0.4.0/shiny/www/shared/shiny.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny.min.js.map` & `shiny-0.4.0/shiny/www/shared/shiny.min.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny_scss/bootstrap.scss` & `shiny-0.4.0/shiny/www/shared/shiny_scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/shiny_scss/shiny.scss` & `shiny-0.4.0/shiny/www/shared/shiny_scss/shiny.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/showdown/compressed/showdown.js` & `shiny-0.4.0/shiny/www/shared/showdown/compressed/showdown.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/showdown/license.txt` & `shiny-0.4.0/shiny/www/shared/showdown/license.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/showdown/src/showdown.js` & `shiny-0.4.0/shiny/www/shared/showdown/src/showdown.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny/www/shared/strftime/strftime-min.js` & `shiny-0.4.0/shiny/www/shared/strftime/strftime-min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/shiny.egg-info/SOURCES.txt` & `shiny-0.4.0/shiny.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -42,24 +42,29 @@
 shiny/examples/Module/app.py
 shiny/examples/Progress/app.py
 shiny/examples/SafeException/app.py
 shiny/examples/SilentCancelOutputException/app.py
 shiny/examples/SilentException/app.py
 shiny/examples/Value/app.py
 shiny/examples/close/app.py
+shiny/examples/data_frame/app.py
 shiny/examples/download/app.py
 shiny/examples/download/mtcars.csv
 shiny/examples/download_button/app.py
 shiny/examples/download_button/mtcars.csv
 shiny/examples/download_link/app.py
 shiny/examples/download_link/mtcars.csv
 shiny/examples/dynamic_route/app.py
 shiny/examples/event/app.py
 shiny/examples/file_reader/app.py
 shiny/examples/file_reader/mtcars.csv
+shiny/examples/include_css/app.py
+shiny/examples/include_css/css/styles.css
+shiny/examples/include_javascript/app.py
+shiny/examples/include_javascript/js/app.js
 shiny/examples/input_action_button/app.py
 shiny/examples/input_action_link/app.py
 shiny/examples/input_checkbox/app.py
 shiny/examples/input_checkbox_group/app.py
 shiny/examples/input_date/app.py
 shiny/examples/input_date_range/app.py
 shiny/examples/input_file/app.py
@@ -116,49 +121,87 @@
 shiny/examples/update_slider/app.py
 shiny/examples/update_text/app.py
 shiny/examples/www_dir/app.py
 shiny/examples/www_dir/www/css/more-styles.css
 shiny/examples/www_dir/www/css/styles.css
 shiny/examples/www_dir/www/js/changetext.js
 shiny/experimental/__init__.py
+shiny/experimental/e2e/accordion/app.py
+shiny/experimental/e2e/navbar/app.py
+shiny/experimental/e2e/sidebar/app.py
+shiny/experimental/e2e/sidebar/data.py
+shiny/experimental/examples/accordion/app.py
+shiny/experimental/examples/accordion_panel/app.py
+shiny/experimental/examples/accordion_panel_close/app.py
+shiny/experimental/examples/accordion_panel_insert/app.py
+shiny/experimental/examples/accordion_panel_open/app.py
+shiny/experimental/examples/accordion_panel_remove/app.py
+shiny/experimental/examples/accordion_panel_set/app.py
+shiny/experimental/examples/accordion_panel_update/app.py
+shiny/experimental/examples/as_fill_carrier/app.py
+shiny/experimental/examples/as_fill_item/app.py
+shiny/experimental/examples/as_fillable_container/app.py
+shiny/experimental/examples/card/app.py
+shiny/experimental/examples/card_body/app.py
+shiny/experimental/examples/card_footer/app.py
+shiny/experimental/examples/card_header/app.py
+shiny/experimental/examples/card_image/app.py
+shiny/experimental/examples/card_title/app.py
+shiny/experimental/examples/layout_column_wrap/app.py
+shiny/experimental/examples/layout_sidebar/app.py
+shiny/experimental/examples/page_sidebar/app.py
+shiny/experimental/examples/showcase_left_center/app.py
+shiny/experimental/examples/showcase_top_right/app.py
+shiny/experimental/examples/sidebar/app.py
+shiny/experimental/examples/sidebar_toggle/app.py
+shiny/experimental/examples/value_box/app.py
 shiny/experimental/ui/__init__.py
+shiny/experimental/ui/_accordion.py
 shiny/experimental/ui/_card.py
-shiny/experimental/ui/_card_full_screen.py
-shiny/experimental/ui/_card_item.py
 shiny/experimental/ui/_color.py
-shiny/experimental/ui/_css.py
+shiny/experimental/ui/_css_unit.py
 shiny/experimental/ui/_fill.py
 shiny/experimental/ui/_htmldeps.py
 shiny/experimental/ui/_input_text.py
 shiny/experimental/ui/_layout.py
+shiny/experimental/ui/_navs.py
 shiny/experimental/ui/_output.py
 shiny/experimental/ui/_page.py
 shiny/experimental/ui/_sidebar.py
+shiny/experimental/ui/_tag.py
+shiny/experimental/ui/_utils.py
 shiny/experimental/ui/_valuebox.py
-shiny/experimental/www/card-full-screen.js
-shiny/experimental/www/fill.css
 shiny/experimental/www/textarea-autoresize.css
 shiny/experimental/www/textarea-autoresize.js
-shiny/experimental/www/sidebar/sidebar.min.js
-shiny/experimental/www/sidebar/sidebar.min.js.map
+shiny/experimental/www/bslib/_version.json
+shiny/experimental/www/bslib/components/accordion.min.js
+shiny/experimental/www/bslib/components/accordion.min.js.map
+shiny/experimental/www/bslib/components/card.min.js
+shiny/experimental/www/bslib/components/card.min.js.map
+shiny/experimental/www/bslib/components/sidebar.min.js
+shiny/experimental/www/bslib/components/sidebar.min.js.map
+shiny/experimental/www/htmltools/_version.json
+shiny/experimental/www/htmltools/fill/fill.css
 shiny/reactive/__init__.py
 shiny/reactive/_core.py
 shiny/reactive/_poll.py
 shiny/reactive/_reactives.py
 shiny/render/__init__.py
 shiny/render/_coordmap.py
+shiny/render/_dataframe.py
 shiny/render/_render.py
 shiny/render/_try_render_plot.py
 shiny/session/__init__.py
 shiny/session/_session.py
 shiny/session/_utils.py
 shiny/ui/__init__.py
 shiny/ui/_bootstrap.py
 shiny/ui/_download_button.py
 shiny/ui/_html_dependencies.py
+shiny/ui/_include_helpers.py
 shiny/ui/_input_action_button.py
 shiny/ui/_input_check_radio.py
 shiny/ui/_input_date.py
 shiny/ui/_input_file.py
 shiny/ui/_input_numeric.py
 shiny/ui/_input_password.py
 shiny/ui/_input_select.py
@@ -171,45 +214,48 @@
 shiny/ui/_navs.py
 shiny/ui/_notification.py
 shiny/ui/_output.py
 shiny/ui/_page.py
 shiny/ui/_plot_output_opts.py
 shiny/ui/_progress.py
 shiny/ui/_utils.py
+shiny/ui/_x/_css_unit.py
+shiny/ui/_x/_fill.py
+shiny/ui/_x/_htmldeps.py
+shiny/ui/_x/_sidebar.py
+shiny/ui/_x/_tag.py
+shiny/ui/_x/_utils.py
+shiny/ui/dataframe/_dataframe.py
+shiny/ui/dataframe/js/dist/index.js
+shiny/ui/dataframe/js/dist/index.js.map
+shiny/www/shared/_version.json
 shiny/www/shared/shiny-autoreload.js
 shiny/www/shared/shiny-autoreload.js.map
 shiny/www/shared/shiny-showcase.css
 shiny/www/shared/shiny-showcase.js
 shiny/www/shared/shiny-showcase.js.map
 shiny/www/shared/shiny-testmode.js
 shiny/www/shared/shiny-testmode.js.map
 shiny/www/shared/shiny.js
 shiny/www/shared/shiny.js.map
 shiny/www/shared/shiny.min.css
 shiny/www/shared/shiny.min.js
 shiny/www/shared/shiny.min.js.map
+shiny/www/shared/_x/bslib/components/sidebar.min.js
+shiny/www/shared/_x/bslib/components/sidebar.min.js.map
+shiny/www/shared/_x/htmltools/fill/fill.css
+shiny/www/shared/bootstrap/_version.json
 shiny/www/shared/bootstrap/bootstrap.bundle.min.js
 shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map
 shiny/www/shared/bootstrap/bootstrap.min.css
-shiny/www/shared/bootstrap/version.json
 shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot
 shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg
 shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf
 shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff
 shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2
-shiny/www/shared/datatables/upgrade1.10.txt
-shiny/www/shared/datatables/css/dataTables.bootstrap.css
-shiny/www/shared/datatables/css/dataTables.extra.css
-shiny/www/shared/datatables/images/sort_asc.png
-shiny/www/shared/datatables/images/sort_asc_disabled.png
-shiny/www/shared/datatables/images/sort_both.png
-shiny/www/shared/datatables/images/sort_desc.png
-shiny/www/shared/datatables/images/sort_desc_disabled.png
-shiny/www/shared/datatables/js/dataTables.bootstrap.js
-shiny/www/shared/datatables/js/jquery.dataTables.min.js
 shiny/www/shared/datepicker/css/bootstrap-datepicker3.css
 shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css
 shiny/www/shared/datepicker/js/bootstrap-datepicker.js
 shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js
 shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js
 shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js
 shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js
@@ -357,8 +403,9 @@
 tests/test_poll.py
 tests/test_reactives.py
 tests/test_shinysession.py
 tests/test_static.py
 tests/test_ui.py
 tests/test_ui_dependencies.py
 tests/test_utils.py
-tests/test_utils_async.py
+tests/test_utils_async.py
+tests/test_x_sidebar.py
```

### Comparing `shiny-0.3.3/shiny.egg-info/requires.txt` & `shiny-0.4.0/shiny.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -8,42 +8,47 @@
 click>=8.0.3
 markdown-it-py>=1.1.0
 mdit-py-plugins>=0.3.0
 linkify-it-py>=1.0
 appdirs>=1.4.4
 asgiref>=3.5.2
 
+[:platform_system != "Emscripten"]
+watchfiles>=0.18.0
+
 [:python_version < "3.8"]
 importlib-metadata<5,>=1.1.0
 
 [dev]
 black>=23.1.0
 flake8-bugbear>=23.2.13
 isort>=5.10.1
-pyright>=1.1.244
+pyright==1.1.311
 pre-commit>=2.15.0
 wheel
 matplotlib
 pandas
 pandas-stubs
 numpy
-shinyswatch>=0.2.3
+shinyswatch>=0.2.4
 
 [dev:python_version <= "3.7"]
 flake8==3.9.2
 
 [dev:python_version > "3.7"]
 flake8>=6.0.0
 
 [test]
 pytest>=6.2.4
 pytest-asyncio>=0.17.2
 pytest-playwright>=0.3.0
 pytest-xdist
 pytest-timeout
+pytest-rerunfailures
+syrupy
 psutil
 astropy
 suntime
 timezonefinder
 ipyleaflet
 shinywidgets
 seaborn
```

### Comparing `shiny-0.3.3/tests/asyncio_prevent.py` & `shiny-0.4.0/tests/asyncio_prevent.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/tests/mocktime.py` & `shiny-0.4.0/tests/mocktime.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/tests/test_e2e_regex_matching.py` & `shiny-0.4.0/tests/test_e2e_regex_matching.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/tests/test_markdown.py` & `shiny-0.4.0/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/tests/test_modules.py` & `shiny-0.4.0/tests/test_modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import asyncio
 from typing import Dict, Union, cast
 
 import pytest
 from htmltools import Tag, TagList
 
-from shiny import *
+from shiny import App, Inputs, Outputs, Session, module, reactive, ui
 from shiny._connection import MockConnection
 from shiny._namespaces import resolve_id
 from shiny.session import get_current_session
 
 
 @module.ui
 def mod_inner_ui() -> TagList:
```

### Comparing `shiny-0.3.3/tests/test_namespaces.py` & `shiny-0.4.0/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/tests/test_navs.py` & `shiny-0.4.0/tests/test_navs.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/tests/test_poll.py` & `shiny-0.4.0/tests/test_poll.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 from enum import Enum
 from random import random
 from types import TracebackType
 from typing import Any, Callable, Dict, Optional, Type, cast
 
 import pytest
 
-from shiny import *
-from shiny import _utils
+from shiny import Session, _utils, session
 from shiny._namespaces import Root
-from shiny.reactive import *
+from shiny.reactive import Effect, Value, file_reader, flush, isolate, poll
 
 from .mocktime import MockTime
 
 
 class OnEndedSessionCallbacks:
     """
     A far-too-minimal mock of Session that implements nothing but on_ended. This is
```

### Comparing `shiny-0.3.3/tests/test_reactives.py` & `shiny-0.4.0/tests/test_reactives.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Tests for `shiny.reactive`."""
 
 import asyncio
 from typing import List
 
 import pytest
 
-from shiny import App, render, ui
+from shiny import App, render, req, ui
 from shiny._connection import MockConnection
-from shiny._validation import SilentException, req
-from shiny.input_handler import ActionButtonValue
-from shiny.reactive import *
+from shiny.reactive import Calc, Effect, Value, event, flush, invalidate_later, isolate
 from shiny.reactive._core import ReactiveWarning
+from shiny.types import ActionButtonValue, SilentException
 
 from .mocktime import MockTime
 
 
 @pytest.mark.asyncio
 async def test_flush_runs_newly_invalidated():
     """
```

### Comparing `shiny-0.3.3/tests/test_shinysession.py` & `shiny-0.4.0/tests/test_shinysession.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/tests/test_static.py` & `shiny-0.4.0/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/tests/test_ui.py` & `shiny-0.4.0/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/tests/test_ui_dependencies.py` & `shiny-0.4.0/tests/test_ui_dependencies.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/tests/test_utils.py` & `shiny-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `shiny-0.3.3/tests/test_utils_async.py` & `shiny-0.4.0/tests/test_utils_async.py`

 * *Files identical despite different names*


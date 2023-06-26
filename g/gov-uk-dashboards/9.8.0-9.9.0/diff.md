# Comparing `tmp/gov_uk_dashboards-9.8.0.tar.gz` & `tmp/gov_uk_dashboards-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gov_uk_dashboards-9.8.0.tar", last modified: Fri Jun 16 15:17:07 2023, max compression
+gzip compressed data, was "gov_uk_dashboards-9.9.0.tar", last modified: Mon Jun 26 13:23:56 2023, max compression
```

## Comparing `gov_uk_dashboards-9.8.0.tar` & `gov_uk_dashboards-9.9.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.507847 gov_uk_dashboards-9.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-16 15:17:07.507847 gov_uk_dashboards-9.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.483847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.487847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/attach-event-to-dash.js
--rw-r--r--   0 runner    (1001) docker     (123)   160823 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/dashboard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.487847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    40816 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/fonts/bold-affa96571d-v2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    31480 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/fonts/bold-b542beb274-v2.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33382 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/fonts/light-94a07e06a1-v2.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    43425 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/fonts/light-f591b13f7d-v2.woff
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/get_assets_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)    34806 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/govuk-frontend-3.14.0.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.491847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)    19884 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/DLUHC_WHITE_Master_AW_sm.png
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/govuk-crest-2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/govuk-crest.png
--rw-r--r--   0 runner    (1001) docker     (123)    22050 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/hm-government-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   114604 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/selecting_how_to.png
--rw-r--r--   0 runner    (1001) docker     (123)    75724 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/viewing_charts_how_to.png
--rw-r--r--   0 runner    (1001) docker     (123)   104943 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/viewing_tables_how_to.png
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/mobile-nav.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.491847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/topojson/
--rw-r--r--   0 runner    (1001) docker     (123)    49104 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/topojson/usa_110m.json
--rw-r--r--   0 runner    (1001) docker     (123)   136642 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/topojson/world_110m.json
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/colours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.491847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.503847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/apply_and_reset_filters_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/banners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/captioned_figure.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/card.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/card_full_width.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/collapsible_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/comparison_la_filter_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/dashboard_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/details.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/download_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/filter_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/footer.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/heading.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/html_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/key_value_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/main_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/navbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/no_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/notification_banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/paragraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/phase_banner.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/row_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/side_navbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/tooltip_title.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/visualisation_commentary.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/visualisation_title.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/warning_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.503847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/chart_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.503847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/enums/dash_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/line_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.503847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/styles/line_style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.503847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/formatting/human_readable.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/formatting/rounding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.507847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.507847 gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/dap/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/dap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/dap/dap_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/dap/get_dataframe_from_cds.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/enable_basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/http_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/template.html
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:17:07.483847 gov_uk_dashboards-9.8.0/gov_uk_dashboards.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-16 15:17:07.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-16 15:17:07.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:17:07.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 15:17:07.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 15:17:07.000000 gov_uk_dashboards-9.8.0/gov_uk_dashboards.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:17:07.507847 gov_uk_dashboards-9.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-16 15:14:23.000000 gov_uk_dashboards-9.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.554583 gov_uk_dashboards-9.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-26 13:23:56.554583 gov_uk_dashboards-9.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.546583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.546583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/attach-event-to-dash.js
+-rw-r--r--   0 runner    (1001) docker     (123)   160823 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.550583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    40816 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/fonts/bold-affa96571d-v2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    31480 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/fonts/bold-b542beb274-v2.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33382 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/fonts/light-94a07e06a1-v2.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    43425 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/fonts/light-f591b13f7d-v2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/get_assets_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34806 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/govuk-frontend-3.14.0.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.550583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    19884 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/DLUHC_WHITE_Master_AW_sm.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/govuk-crest-2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/govuk-crest.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22050 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/hm-government-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   114604 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/selecting_how_to.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75724 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/viewing_charts_how_to.png
+-rw-r--r--   0 runner    (1001) docker     (123)   104943 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/viewing_tables_how_to.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/mobile-nav.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.550583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/topojson/
+-rw-r--r--   0 runner    (1001) docker     (123)    49104 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/topojson/usa_110m.json
+-rw-r--r--   0 runner    (1001) docker     (123)   136642 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/topojson/world_110m.json
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/colours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.550583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.554583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/apply_and_reset_filters_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/banners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/captioned_figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/card_full_width.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/collapsible_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/comparison_la_filter_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/dashboard_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/download_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/filter_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/heading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/html_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/key_value_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/main_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/navbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/no_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/notification_banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/paragraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/phase_banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/row_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/side_navbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/tooltip_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/visualisation_commentary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/visualisation_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/warning_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.554583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/chart_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.554583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/enums/dash_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/line_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.554583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/styles/line_style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.554583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/formatting/human_readable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/formatting/rounding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.554583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.554583 gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/dap/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/dap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/dap/dap_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/dap/get_dataframe_from_cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/enable_basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/http_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:23:56.546583 gov_uk_dashboards-9.9.0/gov_uk_dashboards.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-26 13:23:56.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-26 13:23:56.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:23:56.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-26 13:23:56.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 13:23:56.000000 gov_uk_dashboards-9.9.0/gov_uk_dashboards.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 13:23:56.554583 gov_uk_dashboards-9.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-26 13:21:05.000000 gov_uk_dashboards-9.9.0/setup.py
```

### Comparing `gov_uk_dashboards-9.8.0/LICENSE` & `gov_uk_dashboards-9.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/PKG-INFO` & `gov_uk_dashboards-9.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gov_uk_dashboards
-Version: 9.8.0
+Version: 9.9.0
 Summary: Provides access to functionality common to creating a data dashboard.
 Author: Department for Levelling Up, Housing and Communities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Gov UK dashboards
```

### Comparing `gov_uk_dashboards-9.8.0/README.md` & `gov_uk_dashboards-9.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/__init__.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/__init__.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/attach-event-to-dash.js` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/attach-event-to-dash.js`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/dashboard.css` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/dashboard.css`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/fonts/bold-affa96571d-v2.woff` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/fonts/bold-affa96571d-v2.woff`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/fonts/bold-b542beb274-v2.woff2` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/fonts/bold-b542beb274-v2.woff2`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/fonts/light-94a07e06a1-v2.woff2` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/fonts/light-94a07e06a1-v2.woff2`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/fonts/light-f591b13f7d-v2.woff` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/fonts/light-f591b13f7d-v2.woff`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/govuk-frontend-3.14.0.min.js` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/govuk-frontend-3.14.0.min.js`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/DLUHC_WHITE_Master_AW_sm.png` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/DLUHC_WHITE_Master_AW_sm.png`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/favicon.ico` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/govuk-crest-2x.png` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/govuk-crest-2x.png`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/govuk-crest.png` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/govuk-crest.png`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/hm-government-logo.png` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/hm-government-logo.png`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/selecting_how_to.png` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/selecting_how_to.png`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/viewing_charts_how_to.png` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/viewing_charts_how_to.png`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/images/viewing_tables_how_to.png` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/images/viewing_tables_how_to.png`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/mobile-nav.js` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/mobile-nav.js`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/topojson/usa_110m.json` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/topojson/usa_110m.json`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/assets/topojson/world_110m.json` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/assets/topojson/world_110m.json`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/axes.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/axes.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/colours.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/colours.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/__init__.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/apply_and_reset_filters_buttons.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/apply_and_reset_filters_buttons.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/banners.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/banners.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/captioned_figure.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/captioned_figure.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/collapsible_panel.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/collapsible_panel.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/comparison_la_filter_button.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/comparison_la_filter_button.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/dashboard_container.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/dashboard_container.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/details.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/details.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/download_button.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/download_button.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/filter_panel.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/filter_panel.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/footer.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/footer.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/graph.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/graph.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/heading.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/heading.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/html_list.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/html_list.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/key_value_pair.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/key_value_pair.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/main_content.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/main_content.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/navbar.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/navbar.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/notification_banner.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/notification_banner.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/paragraph.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/paragraph.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/phase_banner.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/phase_banner.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/row_component.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/row_component.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/side_navbar.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/side_navbar.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/table.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/table.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/tooltip.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/tooltip.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/tooltip_title.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/tooltip_title.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/visualisation_commentary.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/visualisation_commentary.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/components/plotly/visualisation_title.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/components/plotly/visualisation_title.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/__init__.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/__init__.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/chart_data.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/chart_data.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/line_chart.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/line_chart.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/figures/styles/line_style.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/figures/styles/line_style.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/formatting/human_readable.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/formatting/human_readable.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/formatting/rounding.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/formatting/rounding.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/dap/dap_deployment.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/dap/dap_deployment.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/dap/get_dataframe_from_cds.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/dap/get_dataframe_from_cds.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/enable_basic_auth.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/enable_basic_auth.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards/lib/http_headers.py` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards/lib/http_headers.py`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards.egg-info/PKG-INFO` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gov-uk-dashboards
-Version: 9.8.0
+Version: 9.9.0
 Summary: Provides access to functionality common to creating a data dashboard.
 Author: Department for Levelling Up, Housing and Communities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Gov UK dashboards
```

### Comparing `gov_uk_dashboards-9.8.0/gov_uk_dashboards.egg-info/SOURCES.txt` & `gov_uk_dashboards-9.9.0/gov_uk_dashboards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gov_uk_dashboards-9.8.0/setup.py` & `gov_uk_dashboards-9.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (this_directory / "README.md").read_text(encoding="UTF-8")
 
 # Call setup function
 setup(
     author="Department for Levelling Up, Housing and Communities",
     description="Provides access to functionality common to creating a data dashboard.",
     name="gov_uk_dashboards",
-    version="9.8.0",
+    version="9.9.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "setuptools~=59.8",
         "dash~=2.0",
         "numpy>=1.22.0",
```


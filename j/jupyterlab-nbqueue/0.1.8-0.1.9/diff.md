# Comparing `tmp/jupyterlab_nbqueue-0.1.8.tar.gz` & `tmp/jupyterlab_nbqueue-0.1.9.tar.gz`

## Comparing `jupyterlab_nbqueue-0.1.8.tar` & `jupyterlab_nbqueue-0.1.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/.bxplorer.db
--rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/.jupyterlab-nbqueue.db
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/RELEASE.md
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/RunningCode.ipynb
--rw-r--r--   0        0        0    54279 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/RunningCode.nbconvert.ipynb
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/install.json
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/setup.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/test04.ipynb
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/test04.nbconvert.ipynb
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/tsconfig.json
--rw-r--r--   0        0        0   209091 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/yarn.lock
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyter-config/nb-config/jupyterlab_nbqueue.json
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyter-config/server-config/jupyterlab_nbqueue.json
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/_version.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/cmd_launcher.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/db_handler.py
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/handlers.py
--rw-r--r--   0        0        0    22112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/build_log.json
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/package.json
--rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/77df7d949de7b5ae43b0.woff2
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/8be134a2ed7f85fceac5.ttf
--rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf
--rw-r--r--   0        0        0    63566 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js
--rw-r--r--   0        0        0    34653 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js.map
--rw-r--r--   0        0        0    30547 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js.map
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/style.js
--rw-r--r--   0        0        0   439063 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js
--rw-r--r--   0        0        0   529754 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map
--rw-r--r--   0        0        0  1074536 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js
--rw-r--r--   0        0        0  1311425 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map
--rw-r--r--   0        0        0   426094 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js
--rw-r--r--   0        0        0   332375 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/src/handler.ts
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/src/index.ts
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/src/svg.d.ts
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/src/components/CustomProps.tsx
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/src/components/RunComponent.tsx
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/src/components/RunsContext.tsx
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/src/components/RunsPanelComponent.tsx
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/src/components/runs.ts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/src/style/IconsStyle.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/src/widgets/RunsPanelWidget.tsx
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/base.css
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/index.js
--rw-r--r--   0        0        0    16753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/nbqueue_logo_v1.svg
--rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/nbqueue_logo_v2.svg
--rw-r--r--   0        0        0   966058 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/fontawesome/css/all.css
--rw-r--r--   0        0        0   163322 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/fontawesome/css/fontawesome.css
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/fontawesome/css/solid.css
--rw-r--r--   0        0        0   105753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/fontawesome/js/fontawesome.js
--rw-r--r--   0        0        0   125539 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/fontawesome/js/pro.js
--rw-r--r--   0        0        0  1794940 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/fontawesome/js/solid.js
--rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   279576 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/style/fontawesome/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/LICENSE
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/README.md
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/.bxplorer.db
+-rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/.jupyterlab-nbqueue.db
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/RELEASE.md
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/RunningCode.ipynb
+-rw-r--r--   0        0        0    54279 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/RunningCode.nbconvert.ipynb
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/install.json
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/setup.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/test04.ipynb
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/test04.nbconvert.ipynb
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/tsconfig.json
+-rw-r--r--   0        0        0   209091 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/yarn.lock
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyter-config/nb-config/jupyterlab_nbqueue.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyter-config/server-config/jupyterlab_nbqueue.json
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/_version.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/cmd_launcher.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/db_handler.py
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/handlers.py
+-rw-r--r--   0        0        0    22112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/build_log.json
+-rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/package.json
+-rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/77df7d949de7b5ae43b0.woff2
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/8be134a2ed7f85fceac5.ttf
+-rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf
+-rw-r--r--   0        0        0    63566 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js
+-rw-r--r--   0        0        0    34653 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js.map
+-rw-r--r--   0        0        0    30547 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js.map
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/style.js
+-rw-r--r--   0        0        0   439063 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js
+-rw-r--r--   0        0        0   529754 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map
+-rw-r--r--   0        0        0  1074536 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js
+-rw-r--r--   0        0        0  1311425 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map
+-rw-r--r--   0        0        0   426094 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js
+-rw-r--r--   0        0        0   332375 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/src/handler.ts
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/src/index.ts
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/src/svg.d.ts
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/src/components/CustomProps.tsx
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/src/components/RunComponent.tsx
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/src/components/RunsContext.tsx
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/src/components/RunsPanelComponent.tsx
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/src/components/runs.ts
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/src/style/IconsStyle.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/src/widgets/RunsPanelWidget.tsx
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/base.css
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/index.js
+-rw-r--r--   0        0        0    16753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/nbqueue_logo_v1.svg
+-rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/nbqueue_logo_v2.svg
+-rw-r--r--   0        0        0   966058 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/fontawesome/css/all.css
+-rw-r--r--   0        0        0   163322 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/fontawesome/css/fontawesome.css
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/fontawesome/css/solid.css
+-rw-r--r--   0        0        0   105753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/fontawesome/js/fontawesome.js
+-rw-r--r--   0        0        0   125539 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/fontawesome/js/pro.js
+-rw-r--r--   0        0        0  1794940 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/fontawesome/js/solid.js
+-rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   279576 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/style/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/README.md
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.9/PKG-INFO
```

### Comparing `jupyterlab_nbqueue-0.1.8/.bxplorer.db` & `jupyterlab_nbqueue-0.1.9/.bxplorer.db`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/RELEASE.md` & `jupyterlab_nbqueue-0.1.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/RunningCode.ipynb` & `jupyterlab_nbqueue-0.1.9/RunningCode.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/RunningCode.nbconvert.ipynb` & `jupyterlab_nbqueue-0.1.9/RunningCode.nbconvert.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996651785714286%*

 * *Differences: {"'cells'": "{4: {'metadata': {'execution': {'iopub.execute_input': '2023-06-23T13:59:26.536940Z', "*

 * *            "'iopub.status.busy': '2023-06-23T13:59:26.536649Z', 'iopub.status.idle': "*

 * *            "'2023-06-23T13:59:26.551835Z', 'shell.execute_reply': "*

 * *            "'2023-06-23T13:59:26.550640Z'}}}, 5: {'metadata': {'execution': "*

 * *            "{'iopub.execute_input': '2023-06-23T13:59:26.556066Z', 'iopub.status.busy': "*

 * *            "'2023-06-23T13:59:26.555726Z', 'iopub.status.idle': '2023-06-23T13:59:2 […]*

```diff
@@ -30,18 +30,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "collapsed": false,
                 "execution": {
-                    "iopub.execute_input": "2023-06-23T13:29:50.253679Z",
-                    "iopub.status.busy": "2023-06-23T13:29:50.253371Z",
-                    "iopub.status.idle": "2023-06-23T13:29:50.261615Z",
-                    "shell.execute_reply": "2023-06-23T13:29:50.261043Z"
+                    "iopub.execute_input": "2023-06-23T13:59:26.536940Z",
+                    "iopub.status.busy": "2023-06-23T13:59:26.536649Z",
+                    "iopub.status.idle": "2023-06-23T13:59:26.551835Z",
+                    "shell.execute_reply": "2023-06-23T13:59:26.550640Z"
                 },
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
@@ -50,18 +50,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "collapsed": false,
                 "execution": {
-                    "iopub.execute_input": "2023-06-23T13:29:50.264891Z",
-                    "iopub.status.busy": "2023-06-23T13:29:50.264592Z",
-                    "iopub.status.idle": "2023-06-23T13:29:50.268225Z",
-                    "shell.execute_reply": "2023-06-23T13:29:50.267549Z"
+                    "iopub.execute_input": "2023-06-23T13:59:26.556066Z",
+                    "iopub.status.busy": "2023-06-23T13:59:26.555726Z",
+                    "iopub.status.idle": "2023-06-23T13:59:26.559578Z",
+                    "shell.execute_reply": "2023-06-23T13:59:26.558899Z"
                 },
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [
                 {
@@ -102,18 +102,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "collapsed": false,
                 "execution": {
-                    "iopub.execute_input": "2023-06-23T13:29:50.315429Z",
-                    "iopub.status.busy": "2023-06-23T13:29:50.315130Z",
-                    "iopub.status.idle": "2023-06-23T13:29:51.323095Z",
-                    "shell.execute_reply": "2023-06-23T13:29:51.322339Z"
+                    "iopub.execute_input": "2023-06-23T13:59:26.607895Z",
+                    "iopub.status.busy": "2023-06-23T13:59:26.607600Z",
+                    "iopub.status.idle": "2023-06-23T13:59:27.614409Z",
+                    "shell.execute_reply": "2023-06-23T13:59:27.612817Z"
                 },
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
@@ -131,18 +131,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "collapsed": false,
                 "execution": {
-                    "iopub.execute_input": "2023-06-23T13:29:51.328180Z",
-                    "iopub.status.busy": "2023-06-23T13:29:51.327824Z",
-                    "iopub.status.idle": "2023-06-23T13:29:51.331925Z",
-                    "shell.execute_reply": "2023-06-23T13:29:51.331046Z"
+                    "iopub.execute_input": "2023-06-23T13:59:27.618791Z",
+                    "iopub.status.busy": "2023-06-23T13:59:27.618471Z",
+                    "iopub.status.idle": "2023-06-23T13:59:27.622363Z",
+                    "shell.execute_reply": "2023-06-23T13:59:27.621688Z"
                 },
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
@@ -208,18 +208,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
                 "collapsed": false,
                 "execution": {
-                    "iopub.execute_input": "2023-06-23T13:29:51.336536Z",
-                    "iopub.status.busy": "2023-06-23T13:29:51.336106Z",
-                    "iopub.status.idle": "2023-06-23T13:29:51.340742Z",
-                    "shell.execute_reply": "2023-06-23T13:29:51.339922Z"
+                    "iopub.execute_input": "2023-06-23T13:59:27.626240Z",
+                    "iopub.status.busy": "2023-06-23T13:59:27.625964Z",
+                    "iopub.status.idle": "2023-06-23T13:59:27.629436Z",
+                    "shell.execute_reply": "2023-06-23T13:59:27.628745Z"
                 },
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [
                 {
@@ -236,18 +236,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
                 "collapsed": false,
                 "execution": {
-                    "iopub.execute_input": "2023-06-23T13:29:51.345015Z",
-                    "iopub.status.busy": "2023-06-23T13:29:51.344661Z",
-                    "iopub.status.idle": "2023-06-23T13:29:51.349263Z",
-                    "shell.execute_reply": "2023-06-23T13:29:51.348413Z"
+                    "iopub.execute_input": "2023-06-23T13:59:27.632806Z",
+                    "iopub.status.busy": "2023-06-23T13:59:27.632381Z",
+                    "iopub.status.idle": "2023-06-23T13:59:27.635959Z",
+                    "shell.execute_reply": "2023-06-23T13:59:27.635256Z"
                 },
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [
                 {
@@ -279,18 +279,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {
                 "collapsed": false,
                 "execution": {
-                    "iopub.execute_input": "2023-06-23T13:29:51.354055Z",
-                    "iopub.status.busy": "2023-06-23T13:29:51.353662Z",
-                    "iopub.status.idle": "2023-06-23T13:29:52.366852Z",
-                    "shell.execute_reply": "2023-06-23T13:29:52.365510Z"
+                    "iopub.execute_input": "2023-06-23T13:59:27.639657Z",
+                    "iopub.status.busy": "2023-06-23T13:59:27.639299Z",
+                    "iopub.status.idle": "2023-06-23T13:59:28.652939Z",
+                    "shell.execute_reply": "2023-06-23T13:59:28.651643Z"
                 },
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [
                 {
@@ -325,18 +325,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {
                 "collapsed": false,
                 "execution": {
-                    "iopub.execute_input": "2023-06-23T13:29:52.371551Z",
-                    "iopub.status.busy": "2023-06-23T13:29:52.371066Z",
-                    "iopub.status.idle": "2023-06-23T13:29:52.376287Z",
-                    "shell.execute_reply": "2023-06-23T13:29:52.375530Z"
+                    "iopub.execute_input": "2023-06-23T13:59:28.657402Z",
+                    "iopub.status.busy": "2023-06-23T13:59:28.657064Z",
+                    "iopub.status.idle": "2023-06-23T13:59:28.661192Z",
+                    "shell.execute_reply": "2023-06-23T13:59:28.660534Z"
                 },
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [
                 {
@@ -410,18 +410,18 @@
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
                 "collapsed": false,
                 "execution": {
-                    "iopub.execute_input": "2023-06-23T13:29:52.379851Z",
-                    "iopub.status.busy": "2023-06-23T13:29:52.379563Z",
-                    "iopub.status.idle": "2023-06-23T13:29:52.386061Z",
-                    "shell.execute_reply": "2023-06-23T13:29:52.385387Z"
+                    "iopub.execute_input": "2023-06-23T13:59:28.664544Z",
+                    "iopub.status.busy": "2023-06-23T13:59:28.664272Z",
+                    "iopub.status.idle": "2023-06-23T13:59:28.670106Z",
+                    "shell.execute_reply": "2023-06-23T13:59:28.669386Z"
                 },
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [
                 {
```

### Comparing `jupyterlab_nbqueue-0.1.8/package.json` & `jupyterlab_nbqueue-0.1.9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.9'"}*

```diff
@@ -183,9 +183,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

### Comparing `jupyterlab_nbqueue-0.1.8/test04.ipynb` & `jupyterlab_nbqueue-0.1.9/test04.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/test04.nbconvert.ipynb` & `jupyterlab_nbqueue-0.1.9/test04.nbconvert.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/tsconfig.json` & `jupyterlab_nbqueue-0.1.9/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/yarn.lock` & `jupyterlab_nbqueue-0.1.9/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/__init__.py` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/cmd_launcher.py` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/cmd_launcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,46 +17,39 @@
     db = DBHandler()
     parser.add_argument("notebook", type=str)
     args = parser.parse_args()
     process = None
     success = None
     message = ''
     try:        
-        logger.info('************ BEGIN cmd_launcher.py ************')
         notebook = args.notebook
         cmd_split = shlex.split(f'jupyter nbconvert --to notebook --execute ./{notebook}')
-        logger.info(f'******* jupyter nbconvert --to notebook --execute ./{notebook} *******')
         process = subprocess.Popen(cmd_split, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         success = True
     except subprocess.CalledProcessError as exc:
         print(f"Program failed {exc.returncode} - {exc}")
         message = f"Program failed {exc.returncode} - {exc}"
     except subprocess.TimeoutExpired as exc:
         print(f"Program timed out {exc}")
         message = f"Program timed out {exc}"
     except Exception as exc:
         print(f"Exception {exc}")
         message = f"Exception {exc}"
     else:
         success = True
     finally:
-        logger.info('************ FINALLY cmd_launcher.py ************')
         with db.get_session() as session:
             if process:
                 newProcess = Runs(pid=process.pid, name=notebook, status='', message='')
                 newProcess.status = 'Running' if success else 'Error'
                 newProcess.message = '' if success else message
                 session.add(newProcess)
                 session.commit()
                               
                 out, error = process.communicate()
-                logger.info('************ BEGIN process.communicate ************')
-                logger.info(out)
-                logger.info(error)
-                logger.info('************ END process.communicate ************')
                 if error.strip() != '':
                     session.query(Runs).filter_by(pid=process.pid).update({'status': 'Error', 'message': error.strip()})
 
                 if out.strip() != '':
                     session.query(Runs).filter_by(pid=process.pid).update({'status': 'Finished'})
                 # session.query(Runs).filter_by(pid=process.pid).update({'status': 'Finished'})
```

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/db_handler.py` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/db_handler.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/handlers.py` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/build_log.json` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/package.json` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js.map` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js.map` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map` & `jupyterlab_nbqueue-0.1.9/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/src/handler.ts` & `jupyterlab_nbqueue-0.1.9/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/src/index.ts` & `jupyterlab_nbqueue-0.1.9/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/src/components/RunComponent.tsx` & `jupyterlab_nbqueue-0.1.9/src/components/RunComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/src/components/RunsContext.tsx` & `jupyterlab_nbqueue-0.1.9/src/components/RunsContext.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/src/components/RunsPanelComponent.tsx` & `jupyterlab_nbqueue-0.1.9/src/components/RunsPanelComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/src/widgets/RunsPanelWidget.tsx` & `jupyterlab_nbqueue-0.1.9/src/widgets/RunsPanelWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/style/nbqueue_logo_v1.svg` & `jupyterlab_nbqueue-0.1.9/style/nbqueue_logo_v1.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/style/nbqueue_logo_v2.svg` & `jupyterlab_nbqueue-0.1.9/style/nbqueue_logo_v2.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/style/fontawesome/css/all.css` & `jupyterlab_nbqueue-0.1.9/style/fontawesome/css/all.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/style/fontawesome/css/fontawesome.css` & `jupyterlab_nbqueue-0.1.9/style/fontawesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/style/fontawesome/css/solid.css` & `jupyterlab_nbqueue-0.1.9/style/fontawesome/css/solid.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/style/fontawesome/js/fontawesome.js` & `jupyterlab_nbqueue-0.1.9/style/fontawesome/js/fontawesome.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/style/fontawesome/js/pro.js` & `jupyterlab_nbqueue-0.1.9/style/fontawesome/js/pro.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/style/fontawesome/js/solid.js` & `jupyterlab_nbqueue-0.1.9/style/fontawesome/js/solid.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/style/fontawesome/webfonts/fa-solid-900.ttf` & `jupyterlab_nbqueue-0.1.9/style/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/style/fontawesome/webfonts/fa-solid-900.woff` & `jupyterlab_nbqueue-0.1.9/style/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/style/fontawesome/webfonts/fa-solid-900.woff2` & `jupyterlab_nbqueue-0.1.9/style/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/.gitignore` & `jupyterlab_nbqueue-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/LICENSE` & `jupyterlab_nbqueue-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/README.md` & `jupyterlab_nbqueue-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/pyproject.toml` & `jupyterlab_nbqueue-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.8/PKG-INFO` & `jupyterlab_nbqueue-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nbqueue
-Version: 0.1.8
+Version: 0.1.9
 Summary: A JupyterLab extension for queuing notebooks executions.
 Project-URL: Homepage, https://github.com/Navteca/jupyterlab-nbqueue.git
 Project-URL: Bug Tracker, https://github.com/Navteca/jupyterlab-nbqueue.git/issues
 Project-URL: Repository, https://github.com/Navteca/jupyterlab-nbqueue.git.git
 Author-email: Navteca LLC <info@navteca.com>
 License: BSD 3-Clause License
```


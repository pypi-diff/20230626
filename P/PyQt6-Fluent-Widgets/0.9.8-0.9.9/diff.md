# Comparing `tmp/PyQt6-Fluent-Widgets-0.9.8.tar.gz` & `tmp/PyQt6-Fluent-Widgets-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt6-Fluent-Widgets-0.9.8.tar", last modified: Mon Jun 26 01:02:39 2023, max compression
+gzip compressed data, was "dist\PyQt6-Fluent-Widgets-0.9.9.tar", last modified: Mon Jun 26 15:44:49 2023, max compression
```

## Comparing `PyQt6-Fluent-Widgets-0.9.8.tar` & `PyQt6-Fluent-Widgets-0.9.9.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.401082 PyQt6-Fluent-Widgets-0.9.8/
--rw-rw-rw-   0        0        0    35823 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/LICENSE
--rw-rw-rw-   0        0        0     4162 2023-06-26 01:02:39.399475 PyQt6-Fluent-Widgets-0.9.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.134984 PyQt6-Fluent-Widgets-0.9.8/PyQt6_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     4162 2023-06-26 01:02:38.000000 PyQt6-Fluent-Widgets-0.9.8/PyQt6_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3880 2023-06-26 01:02:38.000000 PyQt6-Fluent-Widgets-0.9.8/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 01:02:38.000000 PyQt6-Fluent-Widgets-0.9.8/PyQt6_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-06-26 01:02:38.000000 PyQt6-Fluent-Widgets-0.9.8/PyQt6_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-26 01:02:38.000000 PyQt6-Fluent-Widgets-0.9.8/PyQt6_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3362 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.137991 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/
--rw-rw-rw-   0        0        0      516 2023-06-26 00:37:57.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.146315 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  5217293 2023-06-26 00:40:21.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.195604 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      513 2023-06-05 16:02:17.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     2034 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     3193 2023-06-05 15:58:00.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0    10634 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0    18431 2023-06-05 16:02:17.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/deprecation.py
--rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      817 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    10281 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     4775 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3866 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0     4847 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0     7193 2023-06-26 00:37:57.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      452 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.203783 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-06-05 16:02:17.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.222681 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-06-05 16:02:17.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    21626 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7484 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19514 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     5783 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.237094 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      170 2023-06-05 16:02:17.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14992 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5432 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11791 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3227 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2424 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.253451 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-06-05 15:57:58.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2669 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5438 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1262 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.278065 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      535 2023-06-26 00:37:57.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0    10942 2023-06-26 00:39:05.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8103 2023-06-26 00:39:12.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    20038 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    14790 2023-06-26 00:51:22.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6265 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     1422 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.302037 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-06-05 16:02:18.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5388 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0     8152 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     6102 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2840 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    13338 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1544 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.383201 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     2219 2023-06-26 00:37:57.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     4656 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    19420 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     3084 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     1642 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    13269 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0     8072 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0     2135 2023-06-26 00:37:57.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1383 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    18880 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0     3262 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    10184 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3786 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    31602 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0     7602 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     1940 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2511 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    18221 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     5111 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     4513 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6364 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5923 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     9210 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0     8765 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    24690 2023-06-26 00:47:22.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10495 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     2825 2023-06-26 00:36:36.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:02:39.396448 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/window/
--rw-rw-rw-   0        0        0       74 2023-06-26 00:37:57.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    10321 2023-06-26 00:45:34.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     1611 2023-06-26 00:41:54.000000 PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2023-06-26 01:02:39.403248 PyQt6-Fluent-Widgets-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1245 2023-06-26 00:38:13.000000 PyQt6-Fluent-Widgets-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.902466 PyQt6-Fluent-Widgets-0.9.9/
+-rw-rw-rw-   0        0        0    35823 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0     4162 2023-06-26 15:44:49.900961 PyQt6-Fluent-Widgets-0.9.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.704644 PyQt6-Fluent-Widgets-0.9.9/PyQt6_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     4162 2023-06-26 15:44:49.000000 PyQt6-Fluent-Widgets-0.9.9/PyQt6_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3924 2023-06-26 15:44:49.000000 PyQt6-Fluent-Widgets-0.9.9/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:44:49.000000 PyQt6-Fluent-Widgets-0.9.9/PyQt6_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-06-26 15:44:49.000000 PyQt6-Fluent-Widgets-0.9.9/PyQt6_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-26 15:44:49.000000 PyQt6-Fluent-Widgets-0.9.9/PyQt6_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3362 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.706660 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/
+-rw-rw-rw-   0        0        0      516 2023-06-26 15:38:20.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.711130 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  5217293 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.754873 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      513 2023-06-05 16:02:17.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     2034 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     3657 2023-06-26 15:38:20.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0    10634 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0    18431 2023-06-05 16:02:17.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/deprecation.py
+-rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      817 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    10281 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     4775 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3866 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0     4847 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0     7193 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      452 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.757203 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-06-05 16:02:17.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.770605 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-06-05 16:02:17.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    21626 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7484 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19514 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     5783 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.784611 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      170 2023-06-05 16:02:17.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14992 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5432 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11791 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3227 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2424 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.794942 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-06-05 15:57:58.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2669 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5438 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1262 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.810099 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      535 2023-06-26 00:37:57.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0    10942 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8103 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    20038 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    14790 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6265 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     1422 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.826241 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-06-05 16:02:18.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5388 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0     8152 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     6102 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2840 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    13338 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1544 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.890900 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     2275 2023-06-26 15:38:20.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4656 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    19420 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     3084 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     1642 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    13269 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     8072 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0     9734 2023-06-26 15:41:42.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2135 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1383 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    18880 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0     3262 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    10184 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3786 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    31602 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0     7602 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     1940 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2511 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    18221 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     5111 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     4513 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6364 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5923 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     9210 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0     8765 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    24958 2023-06-26 15:39:25.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10495 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     2825 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:44:49.897953 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0       74 2023-06-26 00:37:57.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    10321 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     1611 2023-06-26 15:37:56.000000 PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 15:44:49.902466 PyQt6-Fluent-Widgets-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1245 2023-06-26 15:38:42.000000 PyQt6-Fluent-Widgets-0.9.9/setup.py
```

### Comparing `PyQt6-Fluent-Widgets-0.9.8/LICENSE` & `PyQt6-Fluent-Widgets-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/PKG-INFO` & `PyQt6-Fluent-Widgets-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Fluent-Widgets
-Version: 0.9.8
+Version: 0.9.9
 Summary: A fluent design widgets library based on PyQt6
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt6-Fluent-Widgets Version: 0.9.8 Summary: A
+Metadata-Version: 2.1 Name: PyQt6-Fluent-Widgets Version: 0.9.9 Summary: A
 fluent design widgets library based on PyQt6 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6 Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6 Project-URL: Bug Tracker,
 https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyqt6 fluent
 widgets Classifier: Programming Language :: Python :: 3 Classifier: License ::
```

### Comparing `PyQt6-Fluent-Widgets-0.9.8/PyQt6_Fluent_Widgets.egg-info/PKG-INFO` & `PyQt6-Fluent-Widgets-0.9.9/PyQt6_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Fluent-Widgets
-Version: 0.9.8
+Version: 0.9.9
 Summary: A fluent design widgets library based on PyQt6
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt6-Fluent-Widgets Version: 0.9.8 Summary: A
+Metadata-Version: 2.1 Name: PyQt6-Fluent-Widgets Version: 0.9.9 Summary: A
 fluent design widgets library based on PyQt6 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6 Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6 Project-URL: Bug Tracker,
 https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyqt6 fluent
 widgets Classifier: Programming Language :: Python :: 3 Classifier: License ::
```

### Comparing `PyQt6-Fluent-Widgets-0.9.8/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt` & `PyQt6-Fluent-Widgets-0.9.9/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 qfluentwidgets/components/widgets/__init__.py
 qfluentwidgets/components/widgets/acrylic_label.py
 qfluentwidgets/components/widgets/button.py
 qfluentwidgets/components/widgets/card_widget.py
 qfluentwidgets/components/widgets/check_box.py
 qfluentwidgets/components/widgets/combo_box.py
 qfluentwidgets/components/widgets/cycle_list_widget.py
+qfluentwidgets/components/widgets/flyout.py
 qfluentwidgets/components/widgets/frameless_window.py
 qfluentwidgets/components/widgets/icon_widget.py
 qfluentwidgets/components/widgets/info_bar.py
 qfluentwidgets/components/widgets/label.py
 qfluentwidgets/components/widgets/line_edit.py
 qfluentwidgets/components/widgets/list_view.py
 qfluentwidgets/components/widgets/menu.py
```

### Comparing `PyQt6-Fluent-Widgets-0.9.8/README.md` & `PyQt6-Fluent-Widgets-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/__init__.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 from .components import *
 from .common import *
 from .window import *
 from ._rc import resource
```

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/_rc/resource.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/__init__.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/animation.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/auto_wrap.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/auto_wrap.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         for num, wid in cls.char_widths:
             if o <= num:
                 return wid
 
         return 1
 
     @classmethod
-    def wrap(cls, text, width, once=True):
+    def wrap(cls, text: str, width: int, once=True):
         """ Wrap according to string length
 
         Parameters
         ----------
         text: str
             the text to be wrapped
 
@@ -47,24 +47,39 @@
         -------
         wrap_text: str
             text after auto word wrap process
 
         is_wrapped: bool
             whether a line break occurs in the text
         """
+        texts = text.strip().split('\n')
+        result = []
+        is_wrapped = False
+
+        for text in texts:
+            text_wrapped, wrapped = cls._wrap_line(text, width, once)
+            is_wrapped |= wrapped
+            result.append(text_wrapped)
+            if once:
+                result.extend(texts[1:])
+                break
+
+        return '\n'.join(result), is_wrapped
+
+    @classmethod
+    def _wrap_line(cls, text: str, width: int, once=True):
         count = 0
         last_count = 0
         chars = []
         is_wrapped = False
         break_pos = 0
         is_break_alpha = True
         n_inside_break = 0
 
         i = 0
-        text = text.strip()
         while i < len(text):
             c = text[i]
             length = cls.get_width(c)
             count += length
 
             # record the position of blank character
             if c == " " or length > 1:
```

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/config.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/deprecation.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/deprecation.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/exception_handler.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/font.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/icon.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/image_utils.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/overload.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/router.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/smooth_scroll.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/common/style_sheet.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/calendar_picker.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/calendar_view.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/date_picker.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/picker_base.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/time_picker.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/color_dialog.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/dialog.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/message_dialog.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/expand_layout.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/flow_layout.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/v_box_layout.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/__init__.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_bar.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_interface.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_panel.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_widget.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/pivot.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/pivot.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/segmented_widget.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/__init__.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/expand_setting_card.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/options_setting_card.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/setting_card.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/setting_card_group.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/__init__.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 from .table_view import TableView, TableWidget, TableItemDelegate
 from .tool_tip import ToolTip, ToolTipFilter, ToolTipPosition
 from .tree_view import TreeWidget, TreeView, TreeItemDelegate
 from .cycle_list_widget import CycleListWidget
 from .progress_bar import IndeterminateProgressBar, ProgressBar
 from .progress_ring import ProgressRing
 from .scroll_bar import ScrollBar, SmoothScrollBar, SmoothScrollDelegate
-from .teaching_tip import TeachingTip, TeachingTipTailPosition
+from .teaching_tip import TeachingTip, TeachingTipTailPosition
+from .flyout import FlyoutView, FlyoutViewBase, Flyout
```

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/acrylic_label.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/button.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/card_widget.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/check_box.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/combo_box.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/frameless_window.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/icon_widget.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/info_bar.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/label.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/line_edit.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/list_view.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/menu.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/progress_bar.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/progress_ring.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/scroll_area.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/scroll_bar.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/slider.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/spin_box.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/stacked_widget.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/state_tool_tip.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/switch_button.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/table_view.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/teaching_tip.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/teaching_tip.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,16 @@
         if isinstance(image, str):
             self.image = QImage(image)
         elif isinstance(image, QPixmap):
             self.image = image.toImage()
         elif not self.image:
             self.image = QImage()
 
+        self.originImage = QImage(self.image)
+
         self.hBoxLayout = QHBoxLayout(self)
         self.viewLayout = QHBoxLayout()
         self.widgetLayout = QVBoxLayout()
         self.manager = TeachingTipManager.make(tailPosition)
 
         self.titleLabel = QLabel(title, self)
         self.contentLabel = QLabel(content, self)
@@ -125,26 +127,28 @@
 
         # adjust content margins
         margins = QMargins(6, 5, 6, 5)
         margins.setLeft(20 if not self.icon else 5)
         margins.setRight(20 if not self.isClosable else 6)
         self.viewLayout.setContentsMargins(margins)
 
-        self._adjustImage()
-        vm = self.manager.viewMargins(self)
-        margins.setTop(vm.top())
-        margins.setBottom(vm.bottom())
-        self.viewLayout.setContentsMargins(margins)
+        self.adjustImage()
 
-    def _adjustImage(self):
+    def adjustImage(self):
         if self.image.isNull():
             return
 
-        w = max(200, self.viewLayout.sizeHint().width() - 2)
-        self.image = self.image.scaledToWidth(w, Qt.TransformationMode.SmoothTransformation)
+        w = self.viewLayout.sizeHint().width() - 2
+        self.image = self.originImage.scaledToWidth(w, Qt.TransformationMode.SmoothTransformation)
+
+        vm = self.manager.viewMargins(self)
+        margins = self.viewLayout.contentsMargins()
+        margins.setTop(vm.top())
+        margins.setBottom(vm.bottom())
+        self.viewLayout.setContentsMargins(margins)
 
     def _adjustText(self):
         w = min(900, QApplication.screenAt(
             QCursor.pos()).geometry().width() - 200)
 
         # adjust title
         chars = max(min(w / 10, 120), 30)
@@ -152,17 +156,22 @@
 
         # adjust content
         chars = max(min(w / 9, 120), 30)
         self.contentLabel.setText(TextWrap.wrap(self.content, chars, False)[0])
 
         self.adjustSize()
 
+    def showEvent(self, e):
+        super().showEvent(e)
+        self.adjustImage()
+        self.adjustSize()
+
     def paintEvent(self, e):
         painter = QPainter(self)
-        painter.setRenderHints(QPainter.RenderHint.Antialiasing)
+        painter.setRenderHints(QPainter.RenderHint.Antialiasing | QPainter.RenderHint.SmoothPixmapTransform)
 
         painter.setBrush(
             QColor(40, 40, 40) if isDarkTheme() else QColor(249, 249, 249))
         painter.setPen(
             QColor(23, 23, 23) if isDarkTheme() else QColor(195, 195, 195))
 
         self.manager.draw(self, painter)
@@ -336,15 +345,15 @@
         """ draw the shape of tip """
         # draw border and background
         rect = tip.rect().adjusted(1, 1, -1, -1)
         painter.drawRoundedRect(rect, 8, 8)
 
     def _drawImage(self, tip: TeachingTipView, painter: QPainter):
         """ draw the header image of tip """
-        if not tip.image:
+        if tip.image.isNull():
             return
 
         path = QPainterPath()
         path.setFillRule(Qt.FillRule.WindingFill)
 
         w, h = tip.image.width(), tip.image.height()
         rect = QRectF(1, 1, w, h)
@@ -403,15 +412,15 @@
         path.addPolygon(
             QPolygonF([QPointF(w/2 - 7, pt), QPointF(w/2, 1), QPointF(w/2 + 7, pt)]))
 
         painter.drawPath(path.simplified())
 
     def _drawImage(self, tip: TeachingTipView, painter: QPainter):
         """ draw the header image of tip """
-        if not tip.image:
+        if tip.image.isNull():
             return
 
         path = QPainterPath()
         path.setFillRule(Qt.FillRule.WindingFill)
 
         w, h = tip.image.width(), tip.image.height()
         rect = QRectF(1, 0, w, h)
```

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/tool_tip.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/tree_view.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/window/fluent_window.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/window/fluent_window.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/qfluentwidgets/window/stacked_widget.py` & `PyQt6-Fluent-Widgets-0.9.9/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.9.8/setup.py` & `PyQt6-Fluent-Widgets-0.9.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt6-Fluent-Widgets",
-    version="0.9.8",
+    version="0.9.9",
     keywords="pyqt6 fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PyQt6",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```


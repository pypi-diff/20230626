# Comparing `tmp/PySide6-Fluent-Widgets-0.9.8.tar.gz` & `tmp/PySide6-Fluent-Widgets-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide6-Fluent-Widgets-0.9.8.tar", last modified: Sun Jun 25 15:53:52 2023, max compression
+gzip compressed data, was "dist\PySide6-Fluent-Widgets-0.9.9.tar", last modified: Mon Jun 26 15:14:54 2023, max compression
```

## Comparing `PySide6-Fluent-Widgets-0.9.8.tar` & `PySide6-Fluent-Widgets-0.9.9.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.887874 PySide6-Fluent-Widgets-0.9.8/
--rw-rw-rw-   0        0        0    35821 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/LICENSE
--rw-rw-rw-   0        0        0     4191 2023-06-25 15:53:52.884667 PySide6-Fluent-Widgets-0.9.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.672610 PySide6-Fluent-Widgets-0.9.8/PySide6_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     4191 2023-06-25 15:53:52.000000 PySide6-Fluent-Widgets-0.9.8/PySide6_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3890 2023-06-25 15:53:52.000000 PySide6-Fluent-Widgets-0.9.8/PySide6_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 15:53:52.000000 PySide6-Fluent-Widgets-0.9.8/PySide6_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-06-25 15:53:52.000000 PySide6-Fluent-Widgets-0.9.8/PySide6_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-25 15:53:52.000000 PySide6-Fluent-Widgets-0.9.8/PySide6_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3381 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.675264 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/
--rw-rw-rw-   0        0        0      524 2023-06-25 15:42:50.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.680583 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  5217295 2023-06-25 15:44:41.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.731115 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      513 2023-06-05 16:02:17.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     1998 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     3193 2023-06-05 15:58:00.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0    10643 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0    18431 2023-06-05 16:02:17.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/deprecation.py
--rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      807 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    10208 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     4785 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3862 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0     4862 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0     7186 2023-06-25 15:42:50.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      454 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.733381 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-06-05 16:02:17.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.749091 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-06-05 16:02:17.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2073 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    21168 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7464 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19071 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     5675 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.764429 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      170 2023-06-05 16:02:17.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14828 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5327 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11413 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3244 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2425 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.772879 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-06-05 15:57:58.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2658 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5437 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1305 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.791346 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      535 2023-06-25 15:42:50.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0    10698 2023-06-25 15:42:50.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8129 2023-06-25 15:42:50.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    19839 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    14515 2023-06-25 15:43:59.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6200 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     1390 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.807782 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-06-05 16:02:18.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5314 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0     8036 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     6028 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2838 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    13114 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1590 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.873492 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     2207 2023-06-25 15:42:50.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     4596 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    19251 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     3062 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     1615 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    13661 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7934 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0     2049 2023-06-25 15:42:50.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1327 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    18492 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0     3221 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0     9979 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3639 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    31459 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0     7494 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     1875 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2481 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17730 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     5266 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     4403 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6335 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5854 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     8985 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0     8950 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    24469 2023-06-25 15:45:57.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10402 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     2738 2023-06-25 15:42:34.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:53:52.881718 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/window/
--rw-rw-rw-   0        0        0       74 2023-06-25 15:42:50.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    10176 2023-06-25 15:45:57.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     1586 2023-06-25 15:46:13.000000 PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2023-06-25 15:53:52.887874 PySide6-Fluent-Widgets-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-06-25 15:43:37.000000 PySide6-Fluent-Widgets-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:54.183416 PySide6-Fluent-Widgets-0.9.9/
+-rw-rw-rw-   0        0        0    35821 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0     4191 2023-06-26 15:14:54.181272 PySide6-Fluent-Widgets-0.9.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:53.969602 PySide6-Fluent-Widgets-0.9.9/PySide6_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     4191 2023-06-26 15:14:53.000000 PySide6-Fluent-Widgets-0.9.9/PySide6_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3934 2023-06-26 15:14:53.000000 PySide6-Fluent-Widgets-0.9.9/PySide6_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:14:53.000000 PySide6-Fluent-Widgets-0.9.9/PySide6_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-26 15:14:53.000000 PySide6-Fluent-Widgets-0.9.9/PySide6_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-26 15:14:53.000000 PySide6-Fluent-Widgets-0.9.9/PySide6_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3381 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:53.971854 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/
+-rw-rw-rw-   0        0        0      524 2023-06-26 15:10:17.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:53.976721 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  5217295 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:54.029888 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      513 2023-06-05 16:02:17.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     1998 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     3657 2023-06-26 15:10:17.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0    10643 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0    18431 2023-06-05 16:02:17.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/deprecation.py
+-rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      807 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    10208 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     4785 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3862 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0     4862 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0     7186 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      454 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:54.031901 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-06-05 16:02:17.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:54.046929 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-06-05 16:02:17.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2073 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    21168 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7464 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19071 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     5675 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:54.061430 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      170 2023-06-05 16:02:17.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14828 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5327 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11413 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3244 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2425 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:54.069887 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-06-05 15:57:58.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2658 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5437 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1305 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:54.086826 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      535 2023-06-26 00:37:57.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0    10698 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8129 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    19839 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    14515 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6200 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     1390 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:54.104648 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-06-05 16:02:18.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5314 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0     8036 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     6028 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2838 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    13114 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1590 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:54.171130 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     2263 2023-06-26 15:10:17.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4596 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    19251 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     3062 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     1615 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    13661 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7934 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0     9525 2023-06-26 15:11:38.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2049 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1327 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    18492 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0     3221 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0     9979 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3639 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    31459 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0     7494 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     1875 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2481 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    17730 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     5266 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     4403 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6335 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5854 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     8985 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0     8950 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    24726 2023-06-26 15:10:17.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10402 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     2738 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:14:54.178064 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0       74 2023-06-26 00:37:57.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    10176 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     1586 2023-06-26 15:08:50.000000 PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 15:14:54.183416 PySide6-Fluent-Widgets-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1260 2023-06-26 15:10:32.000000 PySide6-Fluent-Widgets-0.9.9/setup.py
```

### Comparing `PySide6-Fluent-Widgets-0.9.8/LICENSE` & `PySide6-Fluent-Widgets-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/PKG-INFO` & `PySide6-Fluent-Widgets-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Fluent-Widgets
-Version: 0.9.8
+Version: 0.9.9
 Summary: A fluent design widgets library based on PySide6
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 0.9.8 Summary: A
+Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 0.9.9 Summary: A
 fluent design widgets library based on PySide6 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6 Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6 Project-URL: Bug Tracker,
 https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyside6 fluent
 widgets Classifier: Programming Language :: Python :: 3 Classifier: License ::
```

### Comparing `PySide6-Fluent-Widgets-0.9.8/PySide6_Fluent_Widgets.egg-info/PKG-INFO` & `PySide6-Fluent-Widgets-0.9.9/PySide6_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide6-Fluent-Widgets
-Version: 0.9.8
+Version: 0.9.9
 Summary: A fluent design widgets library based on PySide6
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 0.9.8 Summary: A
+Metadata-Version: 2.1 Name: PySide6-Fluent-Widgets Version: 0.9.9 Summary: A
 fluent design widgets library based on PySide6 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6 Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6 Project-URL: Bug Tracker,
 https://github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyside6 fluent
 widgets Classifier: Programming Language :: Python :: 3 Classifier: License ::
```

### Comparing `PySide6-Fluent-Widgets-0.9.8/PySide6_Fluent_Widgets.egg-info/SOURCES.txt` & `PySide6-Fluent-Widgets-0.9.9/PySide6_Fluent_Widgets.egg-info/SOURCES.txt`

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

### Comparing `PySide6-Fluent-Widgets-0.9.8/README.md` & `PySide6-Fluent-Widgets-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/__init__.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PySide6/examples.
 
 :copyright: (c) 2023 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 from .components import *
 from .common import *
 from .window import *
 from ._rc import resource
```

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/_rc/resource.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/__init__.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/animation.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/auto_wrap.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/auto_wrap.py`

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

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/config.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/deprecation.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/deprecation.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/exception_handler.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/font.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/icon.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/image_utils.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/overload.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/router.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/smooth_scroll.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/common/style_sheet.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/calendar_picker.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/calendar_view.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/date_picker.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/picker_base.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/time_picker.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/color_dialog.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/dialog.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/message_dialog.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/expand_layout.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/flow_layout.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/v_box_layout.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/__init__.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_bar.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_interface.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_panel.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_widget.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/pivot.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/pivot.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/segmented_widget.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/__init__.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/expand_setting_card.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/options_setting_card.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/setting_card.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/setting_card_group.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/__init__.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/__init__.py`

 * *Files 6% similar despite different names*

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

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/acrylic_label.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/button.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/card_widget.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/check_box.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/combo_box.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/frameless_window.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/icon_widget.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/info_bar.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/label.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/line_edit.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/list_view.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/menu.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/progress_bar.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/progress_ring.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/scroll_area.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/scroll_bar.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/slider.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/spin_box.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/stacked_widget.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/state_tool_tip.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/switch_button.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/table_view.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/teaching_tip.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/teaching_tip.py`

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
-        self.image = self.image.scaledToWidth(w, Qt.SmoothTransformation)
+        w = self.viewLayout.sizeHint().width() - 2
+        self.image = self.originImage.scaledToWidth(w, Qt.SmoothTransformation)
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
-        painter.setRenderHints(QPainter.Antialiasing)
+        painter.setRenderHints(QPainter.Antialiasing | QPainter.SmoothPixmapTransform)
 
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
         path.setFillRule(Qt.WindingFill)
 
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
         path.setFillRule(Qt.WindingFill)
 
         w, h = tip.image.width(), tip.image.height()
         rect = QRectF(1, 0, w, h)
```

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/tool_tip.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/tree_view.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/window/fluent_window.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/window/fluent_window.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/qfluentwidgets/window/stacked_widget.py` & `PySide6-Fluent-Widgets-0.9.9/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PySide6-Fluent-Widgets-0.9.8/setup.py` & `PySide6-Fluent-Widgets-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide6-Fluent-Widgets",
-    version="0.9.8",
+    version="0.9.9",
     keywords="pyside6 fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PySide6",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```


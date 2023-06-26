# Comparing `tmp/PyQt-Fluent-Widgets-0.9.8.tar.gz` & `tmp/PyQt-Fluent-Widgets-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt-Fluent-Widgets-0.9.8.tar", last modified: Sun Jun 25 15:23:21 2023, max compression
+gzip compressed data, was "dist\PyQt-Fluent-Widgets-0.9.9.tar", last modified: Mon Jun 26 15:05:57 2023, max compression
```

## Comparing `PyQt-Fluent-Widgets-0.9.8.tar` & `PyQt-Fluent-Widgets-0.9.9.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.426539 PyQt-Fluent-Widgets-0.9.8/
--rw-rw-rw-   0        0        0    35823 2023-06-23 14:43:59.000000 PyQt-Fluent-Widgets-0.9.8/LICENSE
--rw-rw-rw-   0        0        0     4866 2023-06-25 15:23:21.424475 PyQt-Fluent-Widgets-0.9.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.206581 PyQt-Fluent-Widgets-0.9.8/PyQt_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     4866 2023-06-25 15:23:20.000000 PyQt-Fluent-Widgets-0.9.8/PyQt_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3875 2023-06-25 15:23:21.000000 PyQt-Fluent-Widgets-0.9.8/PyQt_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 15:23:20.000000 PyQt-Fluent-Widgets-0.9.8/PyQt_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-06-25 15:23:20.000000 PyQt-Fluent-Widgets-0.9.8/PyQt_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-25 15:23:20.000000 PyQt-Fluent-Widgets-0.9.8/PyQt_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4090 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.208593 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/
--rw-rw-rw-   0        0        0      515 2023-06-25 06:30:01.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.213863 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  5217293 2023-06-25 08:43:51.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.262738 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      513 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/animation.py
--rw-rw-rw-   0        0        0     3193 2023-06-05 15:58:00.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0    10659 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0    18431 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/deprecation.py
--rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0      803 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/font.py
--rw-rw-rw-   0        0        0    10228 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     4783 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/overload.py
--rw-rw-rw-   0        0        0     3866 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/router.py
--rw-rw-rw-   0        0        0     4851 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0     7180 2023-06-25 09:21:02.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/style_sheet.py
--rw-rw-rw-   0        0        0      452 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.266347 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.281239 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      234 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     2084 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/calendar_picker.py
--rw-rw-rw-   0        0        0    21160 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/calendar_view.py
--rw-rw-rw-   0        0        0     7455 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19077 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     5783 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.297504 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      170 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    14724 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5291 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11337 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3238 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2500 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.307740 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-06-05 15:57:58.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2692 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5433 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1301 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.326037 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      535 2023-06-25 01:30:12.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0    10717 2023-06-25 05:47:10.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_bar.py
--rw-rw-rw-   0        0        0     8131 2023-06-25 05:47:27.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    19841 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0    14529 2023-06-25 01:30:12.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_widget.py
--rw-rw-rw-   0        0        0     6202 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/pivot.py
--rw-rw-rw-   0        0        0     1386 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/segmented_widget.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.343646 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-06-05 16:02:18.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5316 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0     8027 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     6034 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2840 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    13119 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1586 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.413368 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0     2219 2023-06-25 08:20:08.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     4598 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0    19281 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0     3064 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/card_widget.py
--rw-rw-rw-   0        0        0     1609 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    13208 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7881 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0     2043 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/frameless_window.py
--rw-rw-rw-   0        0        0     1329 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    18494 2023-06-25 08:02:34.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0     3211 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0    10004 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3860 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/list_view.py
--rw-rw-rw-   0        0        0    31338 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0     7520 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     1866 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/progress_ring.py
--rw-rw-rw-   0        0        0     2479 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0    17756 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/scroll_bar.py
--rw-rw-rw-   0        0        0     5132 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     4397 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6334 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5790 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     9027 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0     8730 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/table_view.py
--rw-rw-rw-   0        0        0    24463 2023-06-25 15:11:39.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/teaching_tip.py
--rw-rw-rw-   0        0        0    10384 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     2693 2023-06-23 15:01:50.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/tree_view.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:23:21.422236 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/window/
--rw-rw-rw-   0        0        0       74 2023-06-25 02:29:42.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/window/__init__.py
--rw-rw-rw-   0        0        0    10170 2023-06-25 06:28:57.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/window/fluent_window.py
--rw-rw-rw-   0        0        0     1590 2023-06-25 05:05:08.000000 PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/window/stacked_widget.py
--rw-rw-rw-   0        0        0       42 2023-06-25 15:23:21.426539 PyQt-Fluent-Widgets-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-06-25 06:29:56.000000 PyQt-Fluent-Widgets-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:57.088299 PyQt-Fluent-Widgets-0.9.9/
+-rw-rw-rw-   0        0        0    35823 2023-06-26 00:36:36.000000 PyQt-Fluent-Widgets-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0     4866 2023-06-26 15:05:57.086877 PyQt-Fluent-Widgets-0.9.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:56.880044 PyQt-Fluent-Widgets-0.9.9/PyQt_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     4866 2023-06-26 15:05:56.000000 PyQt-Fluent-Widgets-0.9.9/PyQt_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3919 2023-06-26 15:05:56.000000 PyQt-Fluent-Widgets-0.9.9/PyQt_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:05:56.000000 PyQt-Fluent-Widgets-0.9.9/PyQt_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-06-26 15:05:56.000000 PyQt-Fluent-Widgets-0.9.9/PyQt_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-26 15:05:56.000000 PyQt-Fluent-Widgets-0.9.9/PyQt_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4090 2023-06-26 01:06:04.000000 PyQt-Fluent-Widgets-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:56.882048 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/
+-rw-rw-rw-   0        0        0      515 2023-06-26 14:34:13.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:56.886655 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-06-05 15:57:58.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  5217293 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:56.930684 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      513 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     2004 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/animation.py
+-rw-rw-rw-   0        0        0     3657 2023-06-26 13:17:51.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0    10659 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0    18431 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/deprecation.py
+-rw-rw-rw-   0        0        0      675 2023-06-05 15:57:58.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0      803 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/font.py
+-rw-rw-rw-   0        0        0    10228 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     4783 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     1635 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/overload.py
+-rw-rw-rw-   0        0        0     3866 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/router.py
+-rw-rw-rw-   0        0        0     4851 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0     7180 2023-06-26 12:32:33.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/style_sheet.py
+-rw-rw-rw-   0        0        0      452 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:56.932191 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:56.947558 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      234 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     2084 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/calendar_picker.py
+-rw-rw-rw-   0        0        0    21160 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/calendar_view.py
+-rw-rw-rw-   0        0        0     7455 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19077 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     5783 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:56.962201 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      170 2023-06-05 16:02:17.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    14724 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5291 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11337 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3238 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2500 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:56.972026 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-06-05 15:57:58.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2692 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5433 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1301 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:56.988695 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      535 2023-06-26 00:37:57.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0    10717 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_bar.py
+-rw-rw-rw-   0        0        0     8131 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    19841 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0    14529 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_widget.py
+-rw-rw-rw-   0        0        0     6202 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/pivot.py
+-rw-rw-rw-   0        0        0     1386 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/segmented_widget.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:57.006665 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-06-05 16:02:18.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5316 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0     8027 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     6034 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2840 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    13119 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1586 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:57.076882 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0     2275 2023-06-26 12:52:58.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4598 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0    19281 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0     3064 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/card_widget.py
+-rw-rw-rw-   0        0        0     1609 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    13208 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7881 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0     9519 2023-06-26 14:33:03.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/flyout.py
+-rw-rw-rw-   0        0        0     2043 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/frameless_window.py
+-rw-rw-rw-   0        0        0     1329 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    18494 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0     3211 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0    10004 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3860 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/list_view.py
+-rw-rw-rw-   0        0        0    31338 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0     7520 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     1866 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/progress_ring.py
+-rw-rw-rw-   0        0        0     2479 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0    17756 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/scroll_bar.py
+-rw-rw-rw-   0        0        0     5132 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     4397 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6334 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5790 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     9027 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0     8730 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/table_view.py
+-rw-rw-rw-   0        0        0    24720 2023-06-26 12:37:58.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/teaching_tip.py
+-rw-rw-rw-   0        0        0    10384 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     2693 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/tree_view.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:05:57.083764 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/window/
+-rw-rw-rw-   0        0        0       74 2023-06-26 00:37:57.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/window/__init__.py
+-rw-rw-rw-   0        0        0    10170 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/window/fluent_window.py
+-rw-rw-rw-   0        0        0     1590 2023-06-26 01:06:05.000000 PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/window/stacked_widget.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 15:05:57.088299 PyQt-Fluent-Widgets-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-06-26 14:34:08.000000 PyQt-Fluent-Widgets-0.9.9/setup.py
```

### Comparing `PyQt-Fluent-Widgets-0.9.8/LICENSE` & `PyQt-Fluent-Widgets-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/PKG-INFO` & `PyQt-Fluent-Widgets-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt-Fluent-Widgets
-Version: 0.9.8
+Version: 0.9.9
 Summary: A fluent design widgets library based on PyQt5
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 0.9.8 Summary: A
+Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 0.9.9 Summary: A
 fluent design widgets library based on PyQt5 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets Project-URL: Bug Tracker, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyqt fluent widgets
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
```

### Comparing `PyQt-Fluent-Widgets-0.9.8/PyQt_Fluent_Widgets.egg-info/PKG-INFO` & `PyQt-Fluent-Widgets-0.9.9/PyQt_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt-Fluent-Widgets
-Version: 0.9.8
+Version: 0.9.9
 Summary: A fluent design widgets library based on PyQt5
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 0.9.8 Summary: A
+Metadata-Version: 2.1 Name: PyQt-Fluent-Widgets Version: 0.9.9 Summary: A
 fluent design widgets library based on PyQt5 Home-page: https://github.com/
 zhiyiYo/PyQt-Fluent-Widgets Author: zhiyiYo Author-email:
 shokokawaii@outlook.com License: GPLv3 Project-URL: Documentation, https://
 pyqt-fluent-widgets.readthedocs.io/ Project-URL: Source Code, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets Project-URL: Bug Tracker, https://
 github.com/zhiyiYo/PyQt-Fluent-Widgets/issues Keywords: pyqt fluent widgets
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
```

### Comparing `PyQt-Fluent-Widgets-0.9.8/PyQt_Fluent_Widgets.egg-info/SOURCES.txt` & `PyQt-Fluent-Widgets-0.9.9/PyQt_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

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

### Comparing `PyQt-Fluent-Widgets-0.9.8/README.md` & `PyQt-Fluent-Widgets-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/__init__.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/master/examples.
 
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

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/_rc/resource.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/__init__.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/animation.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/animation.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/auto_wrap.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/auto_wrap.py`

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

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/config.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/deprecation.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/deprecation.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/exception_handler.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/font.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/font.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/icon.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/image_utils.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/overload.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/overload.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/router.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/router.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/smooth_scroll.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/common/style_sheet.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/calendar_picker.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/calendar_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/calendar_view.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/calendar_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/date_picker.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/picker_base.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/picker_base.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/date_time/time_picker.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/color_dialog.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/dialog.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/dialog_box/message_dialog.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/expand_layout.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/flow_layout.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/layout/v_box_layout.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/__init__.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_bar.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_interface.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_panel.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/navigation_widget.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/pivot.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/pivot.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/navigation/segmented_widget.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/navigation/segmented_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/__init__.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/expand_setting_card.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/options_setting_card.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/setting_card.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/settings/setting_card_group.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/__init__.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/__init__.py`

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

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/acrylic_label.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/button.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/card_widget.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/card_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/check_box.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/check_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/combo_box.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/frameless_window.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/frameless_window.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/icon_widget.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/info_bar.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/info_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/label.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/line_edit.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/list_view.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/menu.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/progress_bar.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/progress_ring.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/progress_ring.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/scroll_area.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/scroll_bar.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/slider.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/spin_box.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/stacked_widget.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/state_tool_tip.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/switch_button.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/table_view.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/table_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/teaching_tip.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/teaching_tip.py`

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

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/tool_tip.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/components/widgets/tree_view.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/window/fluent_window.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/window/fluent_window.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/qfluentwidgets/window/stacked_widget.py` & `PyQt-Fluent-Widgets-0.9.9/qfluentwidgets/window/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.9.8/setup.py` & `PyQt-Fluent-Widgets-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt-Fluent-Widgets",
-    version="0.9.8",
+    version="0.9.9",
     keywords="pyqt fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PyQt5",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```


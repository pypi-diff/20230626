# Comparing `tmp/srsgui-0.4.0.tar.gz` & `tmp/srsgui-0.4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-oktwxdg7\srsgui-0.4.0.tar", last modified: Thu Jun 22 23:50:07 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-8d6hs4yl\srsgui-0.4.0.1.tar", last modified: Mon Jun 26 20:07:06 2023, max compression
```

## Comparing `srsgui-0.4.0.tar` & `srsgui-0.4.0.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.998221 srsgui-0.4.0/
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.877909 srsgui-0.4.0/.github/
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.888958 srsgui-0.4.0/.github/workflows/
--rw-rw-rw-   0        0        0      388 2023-06-19 18:04:40.000000 srsgui-0.4.0/.github/workflows/pages.yml
--rw-rw-rw-   0        0        0     1356 2023-05-16 23:33:10.000000 srsgui-0.4.0/.gitignore
--rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3965 2023-06-22 23:50:06.998221 srsgui-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2985 2023-06-19 17:56:19.000000 srsgui-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.918705 srsgui-0.4.0/docs/
--rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.938704 srsgui-0.4.0/docs/_static/
--rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    88057 2023-06-08 18:01:11.000000 srsgui-0.4.0/docs/_static/dock_widget_floating.png
--rw-rw-rw-   0        0        0    97266 2023-06-08 18:01:11.000000 srsgui-0.4.0/docs/_static/dock_widgets_expanded.png
--rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    52123 2023-06-08 23:01:31.000000 srsgui-0.4.0/docs/_static/lockin-capture.png
--rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    38581 2023-06-08 18:01:11.000000 srsgui-0.4.0/docs/_static/task_selection.png
--rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     8513 2023-06-15 00:44:23.000000 srsgui-0.4.0/docs/application.rst
--rw-rw-rw-   0        0        0      839 2023-06-21 20:11:21.000000 srsgui-0.4.0/docs/changelog.rst
--rw-rw-rw-   0        0        0     1924 2023-06-08 18:01:11.000000 srsgui-0.4.0/docs/conf.py
--rw-rw-rw-   0        0        0     6097 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-06-08 23:01:31.000000 srsgui-0.4.0/docs/create-task.rst
--rw-rw-rw-   0        0        0     6112 2023-06-08 23:01:31.000000 srsgui-0.4.0/docs/define-instrument.rst
--rw-rw-rw-   0        0        0    15640 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/example.rst
--rw-rw-rw-   0        0        0     3803 2023-06-15 00:44:23.000000 srsgui-0.4.0/docs/index.rst
--rw-rw-rw-   0        0        0     4405 2023-06-15 00:44:23.000000 srsgui-0.4.0/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/make.bat
--rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.4.0/docs/requirements..txt
--rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      930 2023-06-08 18:01:11.000000 srsgui-0.4.0/docs/srsgui.inst.rst
--rw-rw-rw-   0        0        0      113 2023-05-24 20:30:53.000000 srsgui-0.4.0/docs/srsgui.rst
--rw-rw-rw-   0        0        0     1077 2023-05-24 20:30:53.000000 srsgui-0.4.0/docs/srsgui.task.rst
--rw-rw-rw-   0        0        0     2065 2023-05-24 20:30:53.000000 srsgui-0.4.0/docs/srsgui.ui.commandtree.rst
--rw-rw-rw-   0        0        0      603 2023-05-24 20:30:53.000000 srsgui-0.4.0/docs/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1646 2023-05-24 20:30:53.000000 srsgui-0.4.0/docs/srsgui.ui.rst
--rw-rw-rw-   0        0        0      620 2023-06-15 00:44:23.000000 srsgui-0.4.0/docs/troubleshooting.rst
--rw-rw-rw-   0        0        0     1489 2023-06-15 00:44:23.000000 srsgui-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.4.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 23:50:06.998221 srsgui-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.938704 srsgui-0.4.0/srsgui/
--rw-rw-rw-   0        0        0     1537 2023-06-21 20:11:21.000000 srsgui-0.4.0/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.4.0/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.888958 srsgui-0.4.0/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.948705 srsgui-0.4.0/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.948705 srsgui-0.4.0/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-06-19 17:56:19.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.958705 srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2250 2023-06-19 17:56:19.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.958705 srsgui-0.4.0/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.4.0/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9907 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.968705 srsgui-0.4.0/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.4.0/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8774 2023-06-22 22:17:34.000000 srsgui-0.4.0/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    19291 2023-06-22 22:15:32.000000 srsgui-0.4.0/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10410 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9990 2023-06-19 18:04:40.000000 srsgui-0.4.0/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.978705 srsgui-0.4.0/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.4.0/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      811 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6989 2023-06-21 20:11:21.000000 srsgui-0.4.0/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5856 2023-06-21 20:11:21.000000 srsgui-0.4.0/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6938 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    23469 2023-06-08 18:01:11.000000 srsgui-0.4.0/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.988215 srsgui-0.4.0/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.4.0/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     6880 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.998221 srsgui-0.4.0/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0        0 2023-05-19 00:30:39.000000 srsgui-0.4.0/srsgui/ui/commandtree/__init__.py
--rw-rw-rw-   0        0        0     3941 2023-05-23 19:11:06.000000 srsgui-0.4.0/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/commandtree/commandhandler.py
--rw-rw-rw-   0        0        0    12605 2023-06-22 21:23:49.000000 srsgui-0.4.0/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     8669 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     5109 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     4852 2023-06-19 18:04:40.000000 srsgui-0.4.0/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.4.0/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9798 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    15880 2023-06-08 18:01:11.000000 srsgui-0.4.0/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    14950 2023-06-21 20:11:21.000000 srsgui-0.4.0/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.998221 srsgui-0.4.0/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1449 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.4.0/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.4.0/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    26525 2023-06-21 20:11:21.000000 srsgui-0.4.0/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.4.0/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.4.0/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.948705 srsgui-0.4.0/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3965 2023-06-22 23:50:06.000000 srsgui-0.4.0/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3170 2023-06-22 23:50:06.000000 srsgui-0.4.0/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 23:50:06.000000 srsgui-0.4.0/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-22 23:50:06.000000 srsgui-0.4.0/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      103 2023-06-22 23:50:06.000000 srsgui-0.4.0/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 23:50:06.000000 srsgui-0.4.0/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.421602 srsgui-0.4.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.313116 srsgui-0.4.0.1/.github/
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.321620 srsgui-0.4.0.1/.github/workflows/
+-rw-rw-rw-   0        0        0      388 2023-06-19 18:04:40.000000 srsgui-0.4.0.1/.github/workflows/pages.yml
+-rw-rw-rw-   0        0        0     1356 2023-05-16 23:33:10.000000 srsgui-0.4.0.1/.gitignore
+-rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.4.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3967 2023-06-26 20:07:06.421602 srsgui-0.4.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2985 2023-06-19 17:56:19.000000 srsgui-0.4.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.351636 srsgui-0.4.0.1/docs/
+-rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.371628 srsgui-0.4.0.1/docs/_static/
+-rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    88057 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/docs/_static/dock_widget_floating.png
+-rw-rw-rw-   0        0        0    97266 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/docs/_static/dock_widgets_expanded.png
+-rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    52123 2023-06-08 23:01:31.000000 srsgui-0.4.0.1/docs/_static/lockin-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    38581 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/docs/_static/task_selection.png
+-rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     8513 2023-06-15 00:44:23.000000 srsgui-0.4.0.1/docs/application.rst
+-rw-rw-rw-   0        0        0      840 2023-06-26 20:05:20.000000 srsgui-0.4.0.1/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1924 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/docs/conf.py
+-rw-rw-rw-   0        0        0     6097 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-06-08 23:01:31.000000 srsgui-0.4.0.1/docs/create-task.rst
+-rw-rw-rw-   0        0        0     6112 2023-06-08 23:01:31.000000 srsgui-0.4.0.1/docs/define-instrument.rst
+-rw-rw-rw-   0        0        0    15640 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/example.rst
+-rw-rw-rw-   0        0        0     3803 2023-06-15 00:44:23.000000 srsgui-0.4.0.1/docs/index.rst
+-rw-rw-rw-   0        0        0     4405 2023-06-15 00:44:23.000000 srsgui-0.4.0.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/make.bat
+-rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.4.0.1/docs/requirements..txt
+-rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/docs/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      930 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/docs/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      113 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/docs/srsgui.rst
+-rw-rw-rw-   0        0        0     1077 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/docs/srsgui.task.rst
+-rw-rw-rw-   0        0        0     2065 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/docs/srsgui.ui.commandtree.rst
+-rw-rw-rw-   0        0        0      603 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/docs/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1646 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/docs/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1101 2023-06-23 17:22:50.000000 srsgui-0.4.0.1/docs/troubleshooting.rst
+-rw-rw-rw-   0        0        0     1489 2023-06-15 00:44:23.000000 srsgui-0.4.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.4.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 20:07:06.421602 srsgui-0.4.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.4.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.371628 srsgui-0.4.0.1/srsgui/
+-rw-rw-rw-   0        0        0     1539 2023-06-26 20:05:20.000000 srsgui-0.4.0.1/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.4.0.1/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.313116 srsgui-0.4.0.1/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.371628 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.381591 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-06-19 17:56:19.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.381591 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2250 2023-06-19 17:56:19.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.391610 srsgui-0.4.0.1/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.4.0.1/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9907 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.391610 srsgui-0.4.0.1/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.4.0.1/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8774 2023-06-23 17:22:50.000000 srsgui-0.4.0.1/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    19291 2023-06-23 17:22:50.000000 srsgui-0.4.0.1/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10410 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9990 2023-06-19 18:04:40.000000 srsgui-0.4.0.1/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.401611 srsgui-0.4.0.1/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.4.0.1/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      811 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6989 2023-06-21 20:11:21.000000 srsgui-0.4.0.1/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5856 2023-06-21 20:11:21.000000 srsgui-0.4.0.1/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6938 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    23469 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.411601 srsgui-0.4.0.1/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.4.0.1/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     6880 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.421602 srsgui-0.4.0.1/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0        0 2023-05-19 00:30:39.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/__init__.py
+-rw-rw-rw-   0        0        0     3941 2023-05-23 19:11:06.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commandhandler.py
+-rw-rw-rw-   0        0        0    12605 2023-06-23 17:22:50.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     8669 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     5109 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     4852 2023-06-19 18:04:40.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.4.0.1/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9798 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    15880 2023-06-08 18:01:11.000000 srsgui-0.4.0.1/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    14950 2023-06-21 20:11:21.000000 srsgui-0.4.0.1/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.421602 srsgui-0.4.0.1/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1449 2023-05-24 20:30:53.000000 srsgui-0.4.0.1/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.4.0.1/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.4.0.1/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.4.0.1/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    26550 2023-06-26 20:05:20.000000 srsgui-0.4.0.1/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.4.0.1/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.4.0.1/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:07:06.371628 srsgui-0.4.0.1/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3967 2023-06-26 20:07:06.000000 srsgui-0.4.0.1/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3170 2023-06-26 20:07:06.000000 srsgui-0.4.0.1/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 20:07:06.000000 srsgui-0.4.0.1/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-26 20:07:06.000000 srsgui-0.4.0.1/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      103 2023-06-26 20:07:06.000000 srsgui-0.4.0.1/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 20:07:06.000000 srsgui-0.4.0.1/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.4.0/.gitignore` & `srsgui-0.4.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/LICENSE.txt` & `srsgui-0.4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/PKG-INFO` & `srsgui-0.4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.4.0
+Version: 0.4.0.1
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
```

### Comparing `srsgui-0.4.0/README.md` & `srsgui-0.4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/Makefile` & `srsgui-0.4.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.4.0.1/docs/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/cg-terminal-screen-capture.png` & `srsgui-0.4.0.1/docs/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/connect-dialog-box-capture.png` & `srsgui-0.4.0.1/docs/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/dock_widget_floating.png` & `srsgui-0.4.0.1/docs/_static/dock_widget_floating.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/dock_widgets_expanded.png` & `srsgui-0.4.0.1/docs/_static/dock_widgets_expanded.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/example-screen-capture-1.png` & `srsgui-0.4.0.1/docs/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/example-screen-capture-2.png` & `srsgui-0.4.0.1/docs/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/initial-screen-capture.png` & `srsgui-0.4.0.1/docs/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/lockin-capture.png` & `srsgui-0.4.0.1/docs/_static/lockin-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.4.0.1/docs/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/second-task-screen-capture.png` & `srsgui-0.4.0.1/docs/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/task_selection.png` & `srsgui-0.4.0.1/docs/_static/task_selection.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/terminal-with-example-2.png` & `srsgui-0.4.0.1/docs/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/_static/terminal-with-example.png` & `srsgui-0.4.0.1/docs/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/application.rst` & `srsgui-0.4.0.1/docs/application.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/changelog.rst` & `srsgui-0.4.0.1/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 V.0.4.0 -- Jun 21, 2023
     * Changed :mod:`IndexCommand <srsgui.inst.indexcommands>`
       to instance variable to handle multiple instances correctly.
       It requires a subclass of IndexCommand to be defined in __init__() of the subclass.
       self.add_parent_to_index_commands() should be called after the definition of index commands.
 
 V.0.3.4 -- Jun 20, 2023
-    * Removed default_value from :class:`CommandInput <srsgui.task.inputs.CommandInput>`.__init__
+    * Removed default_value from :class:`CommandInput <srsgui.task.inputs.CommandInput>`.__init__.
       cmd_instance argument is not necessary, either.
 
 V.0.3.1 -- May 22, 2023
     * Changed task result file name extension to .sgdata.
 
 V.0.3.0 -- May 16, 2023
     * Moved documentation to Github Pages.
```

### Comparing `srsgui-0.4.0/docs/conf.py` & `srsgui-0.4.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/create-project.rst` & `srsgui-0.4.0.1/docs/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/create-task.rst` & `srsgui-0.4.0.1/docs/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/define-instrument.rst` & `srsgui-0.4.0.1/docs/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/example.rst` & `srsgui-0.4.0.1/docs/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/index.rst` & `srsgui-0.4.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/installation.rst` & `srsgui-0.4.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/make.bat` & `srsgui-0.4.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/srsgui.inst.communications.rst` & `srsgui-0.4.0.1/docs/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/srsgui.inst.rst` & `srsgui-0.4.0.1/docs/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/srsgui.task.rst` & `srsgui-0.4.0.1/docs/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/srsgui.ui.commandtree.rst` & `srsgui-0.4.0.1/docs/srsgui.ui.commandtree.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/srsgui.ui.qt.rst` & `srsgui-0.4.0.1/docs/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/docs/srsgui.ui.rst` & `srsgui-0.4.0.1/docs/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/pyproject.toml` & `srsgui-0.4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/__init__.py` & `srsgui-0.4.0.1/srsgui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.4.0"  # Global version number
+__version__ = "0.4.0.1"  # Global version number
```

### Comparing `srsgui-0.4.0/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.4.0.1/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/inst/__init__.py` & `srsgui-0.4.0.1/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/inst/commands.py` & `srsgui-0.4.0.1/srsgui/inst/commands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/inst/communications/interface.py` & `srsgui-0.4.0.1/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/inst/communications/serial_ports.py` & `srsgui-0.4.0.1/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/inst/communications/serialinterface.py` & `srsgui-0.4.0.1/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.4.0.1/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/inst/component.py` & `srsgui-0.4.0.1/srsgui/inst/component.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/inst/exceptions.py` & `srsgui-0.4.0.1/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/inst/indexcommands.py` & `srsgui-0.4.0.1/srsgui/inst/indexcommands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/inst/instrument.py` & `srsgui-0.4.0.1/srsgui/inst/instrument.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/task/callbacks.py` & `srsgui-0.4.0.1/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/task/config.py` & `srsgui-0.4.0.1/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/task/inputs.py` & `srsgui-0.4.0.1/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/task/sessionhandler.py` & `srsgui-0.4.0.1/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/task/task.py` & `srsgui-0.4.0.1/srsgui/task/task.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/task/taskresult.py` & `srsgui-0.4.0.1/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/commandhandler.py` & `srsgui-0.4.0.1/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/commandterminal.py` & `srsgui-0.4.0.1/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.4.0.1/srsgui/ui/commandtree/commanddelegate.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/commandtree/commandhandler.py` & `srsgui-0.4.0.1/srsgui/ui/commandtree/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.4.0.1/srsgui/ui/commandtree/commanditem.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.4.0.1/srsgui/ui/commandtree/commandmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.4.0.1/srsgui/ui/commandtree/commandspinbox.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.4.0.1/srsgui/ui/commandtree/commandtreeview.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.4.0.1/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.4.0.1/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/connectdlg.py` & `srsgui-0.4.0.1/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/deviceinfohandler.py` & `srsgui-0.4.0.1/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/dockhandler.py` & `srsgui-0.4.0.1/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/inputpanel.py` & `srsgui-0.4.0.1/srsgui/ui/inputpanel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/qt/QtCore.py` & `srsgui-0.4.0.1/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/qt/QtGui.py` & `srsgui-0.4.0.1/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.4.0.1/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/qt/__init__.py` & `srsgui-0.4.0.1/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/qtloghandler.py` & `srsgui-0.4.0.1/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/resource_rc.py` & `srsgui-0.4.0.1/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/signalhandler.py` & `srsgui-0.4.0.1/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/srslogo.jpg` & `srsgui-0.4.0.1/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/stdout.py` & `srsgui-0.4.0.1/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/taskmain.py` & `srsgui-0.4.0.1/srsgui/ui/taskmain.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                 logger.error(e)
 
             # Check if argument is given in the command line
             if self.initial_load and len(sys.argv) == 2 and sys.argv[1].split('.')[-1].lower() == 'taskconfig':
                 self.default_config_file = sys.argv[1]
                 self.initial_load = False
             else:
-                popped_path = sys.path.pop()
+                popped_path = sys.path.pop(0)
                 logger.debug('"{}" removed from sys.path'.format(popped_path))
 
             current_dir = str(Path(self.default_config_file).parent)
             sys.path.insert(0, current_dir)
             os.chdir(current_dir)
             logger.debug('Set the current directory to "{}"'.format(current_dir))
             self.config.load(self.default_config_file)
@@ -636,17 +636,17 @@
     def onAbout(self):
         msg = ''
         for name in self.inst_dict:
             inst = self.inst_dict[name]
             if hasattr(inst, "__version__"):
                 version = inst.__version__
             else:
-                version = 'N/A'
-
-            msg += '{} version: {}\n'.format(inst.__class__.__name__, version)
+                version = ''
+            if version:
+                msg += '{} version: {}\n'.format(inst.__class__.__name__, version)
         msg += '\nSrsgui version: {}\n'.format(__version__)
         msg += '\n{} version: {}\n'.format(QT_BINDER, QT_BINDER_VERSION)
         msg += 'Python version: {}\n'.format(sys.version)
         self.display_question(msg, None)
 
     def load_settings(self):
         """
```

### Comparing `srsgui-0.4.0/srsgui/ui/taskmain.ui` & `srsgui-0.4.0.1/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui/ui/ui_taskmain.py` & `srsgui-0.4.0.1/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.0/srsgui.egg-info/PKG-INFO` & `srsgui-0.4.0.1/srsgui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.4.0
+Version: 0.4.0.1
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
```

### Comparing `srsgui-0.4.0/srsgui.egg-info/SOURCES.txt` & `srsgui-0.4.0.1/srsgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*


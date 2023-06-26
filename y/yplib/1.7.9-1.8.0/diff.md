# Comparing `tmp/yplib-1.7.9.tar.gz` & `tmp/yplib-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.7.9.tar", last modified: Mon Jun 26 00:48:42 2023, max compression
+gzip compressed data, was "dist\yplib-1.8.0.tar", last modified: Mon Jun 26 00:53:03 2023, max compression
```

## Comparing `yplib-1.7.9.tar` & `yplib-1.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 00:48:42.506950 yplib-1.7.9/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.9/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-26 00:48:42.506449 yplib-1.7.9/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 00:48:42.507451 yplib-1.7.9/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-26 00:48:36.000000 yplib-1.7.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 00:48:42.503273 yplib-1.7.9/yplib/
--rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.7.9/yplib/__init__.py
--rw-rw-rw-   0        0        0    11739 2023-06-26 00:47:36.000000 yplib-1.7.9/yplib/chart.py
--rw-rw-rw-   0        0        0     8541 2023-06-26 00:22:01.000000 yplib-1.7.9/yplib/chart_html.py
--rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.7.9/yplib/db.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.9/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.9/yplib/http_util.py
--rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.7.9/yplib/index.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.7.9/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-26 00:48:42.505910 yplib-1.7.9/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-26 00:48:42.000000 yplib-1.7.9/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-26 00:48:42.000000 yplib-1.7.9/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 00:48:42.000000 yplib-1.7.9/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-26 00:48:42.000000 yplib-1.7.9/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 00:53:03.347092 yplib-1.8.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.8.0/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-26 00:53:03.346594 yplib-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.8.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 00:53:03.347092 yplib-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-26 00:52:56.000000 yplib-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 00:53:03.343153 yplib-1.8.0/yplib/
+-rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.8.0/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 00:52:47.000000 yplib-1.8.0/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-1.8.0/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.8.0/yplib/db.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.8.0/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.8.0/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.8.0/yplib/index.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.8.0/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-26 00:53:03.346082 yplib-1.8.0/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-26 00:53:03.000000 yplib-1.8.0/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-26 00:53:03.000000 yplib-1.8.0/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 00:53:03.000000 yplib-1.8.0/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-26 00:53:03.000000 yplib-1.8.0/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.7.9/LICENSE` & `yplib-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.7.9/setup.py` & `yplib-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.7.9",
+  version="1.8.0",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.7.9/yplib/chart.py` & `yplib-1.8.0/yplib/chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     legend_data = []
     legend_selected = {}
     for y_one in y_list:
         name_one = y_one['name']
         legend_data.append(name_one)
         if 'hide' in y_one and y_one['hide']:
             legend_selected[name_one] = 0
-    legend = 'data: ' + str(legend_data) + ',\n        selected: ' + str(legend_selected)
+    legend = 'data: ' + str(legend_data) + ',\n            selected: ' + str(legend_selected)
     # {
     #     name: 'Email',
     #     type: 'line',
     #     stack: 'Total',
     #     data: [120, 132, 101, 134, 90, 230, 210],
     # }
     series = []
@@ -309,15 +309,15 @@
 #
 
 # # # 将 list 转化成 图表的例子
 # x_list = []
 # y_list = []
 # # # x 轴有 100 个
 # # # 100 个横坐标
-# for i in range(100):
+# for i in range(1000):
 #     x_list.append(i)
 # #
 # # 有 10 条线
 # for i in range(10):  # 0 1 2 3 4 55
 #     n = {}
 #     n['name'] = str(int(random.uniform(0, 1000)))
 #     data = []
```

### Comparing `yplib-1.7.9/yplib/chart_html.py` & `yplib-1.8.0/yplib/chart_html.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,16 @@
               '        left: "30px",',
               '        right: "40px",',
               '        bottom: "80px",',
               '        containLabel: true,',
               '    },',
               '    toolbox: {',
               '        feature: {',
-              '            saveAsImage: {'
-              '                pixelRatio:5'
+              '            saveAsImage: {',
+              '                pixelRatio: 5',
               '            },',
               '        },',
               '    },',
               '    yAxis: {',
               '        type: "value",',
               '    },',
               '    xAxis: {',
@@ -82,16 +82,16 @@
               '    trigger: "axis",',
               '  },',
               '  title: {',
               '    text: "-chart_name-"',
               '  },',
               '  toolbox: {',
               '    feature: {',
-              '       saveAsImage: {'
-              '           pixelRatio:5'
+              '       saveAsImage: {',
+              '           pixelRatio: 5',
               '       },',
               '    }',
               '  },',
               '    grid: {',
               '        left: "30px",',
               '        right: "40px",',
               '        bottom: "80px",',
@@ -151,16 +151,16 @@
               '    left: 10',
               '  },',
               '  tooltip: {',
               '    trigger: "item"',
               '  },',
               '    toolbox: {',
               '        feature: {',
-              '            saveAsImage: {'
-              '                pixelRatio:5'
+              '            saveAsImage: {',
+              '                pixelRatio: 5',
               '            },',
               '        },',
               '    },',
               '  legend: {',
               '    top: "5%",',
               '    left: "center"',
               '  },',
@@ -200,16 +200,16 @@
               '  },',
               '  toolbox: {',
               '    feature: {',
               '      dataZoom: {',
               '        yAxisIndex: false',
               '      },',
               '      saveAsImage: {',
-              '            saveAsImage: {'
-              '                pixelRatio:5'
+              '            saveAsImage: {',
+              '                pixelRatio: 5',
               '            },',
               '      }',
               '    }',
               '  },',
               '  tooltip: {',
               '    trigger: "axis",',
               '    axisPointer: {',
```

### Comparing `yplib-1.7.9/yplib/db.py` & `yplib-1.8.0/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.9/yplib/file.py` & `yplib-1.8.0/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.9/yplib/http_util.py` & `yplib-1.8.0/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.9/yplib/index.py` & `yplib-1.8.0/yplib/index.py`

 * *Files identical despite different names*


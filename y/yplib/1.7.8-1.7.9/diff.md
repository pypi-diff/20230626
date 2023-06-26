# Comparing `tmp/yplib-1.7.8.tar.gz` & `tmp/yplib-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.7.8.tar", last modified: Sun Jun 25 08:50:42 2023, max compression
+gzip compressed data, was "dist\yplib-1.7.9.tar", last modified: Mon Jun 26 00:48:42 2023, max compression
```

## Comparing `yplib-1.7.8.tar` & `yplib-1.7.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 08:50:42.423374 yplib-1.7.8/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.8/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-25 08:50:42.423268 yplib-1.7.8/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 08:50:42.423958 yplib-1.7.8/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-25 08:48:36.000000 yplib-1.7.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:50:42.420274 yplib-1.7.8/yplib/
--rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.7.8/yplib/__init__.py
--rw-rw-rw-   0        0        0    11634 2023-06-25 08:49:38.000000 yplib-1.7.8/yplib/chart.py
--rw-rw-rw-   0        0        0     8270 2023-06-25 08:40:25.000000 yplib-1.7.8/yplib/chart_html.py
--rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.7.8/yplib/db.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.8/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.8/yplib/http_util.py
--rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.7.8/yplib/index.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.7.8/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:50:42.422643 yplib-1.7.8/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-25 08:50:42.000000 yplib-1.7.8/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-25 08:50:42.000000 yplib-1.7.8/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 08:50:42.000000 yplib-1.7.8/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-25 08:50:42.000000 yplib-1.7.8/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 00:48:42.506950 yplib-1.7.9/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.7.9/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-26 00:48:42.506449 yplib-1.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.7.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 00:48:42.507451 yplib-1.7.9/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-26 00:48:36.000000 yplib-1.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 00:48:42.503273 yplib-1.7.9/yplib/
+-rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.7.9/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11739 2023-06-26 00:47:36.000000 yplib-1.7.9/yplib/chart.py
+-rw-rw-rw-   0        0        0     8541 2023-06-26 00:22:01.000000 yplib-1.7.9/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.7.9/yplib/db.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.7.9/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.7.9/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.7.9/yplib/index.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.7.9/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-26 00:48:42.505910 yplib-1.7.9/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-26 00:48:42.000000 yplib-1.7.9/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-26 00:48:42.000000 yplib-1.7.9/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 00:48:42.000000 yplib-1.7.9/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-26 00:48:42.000000 yplib-1.7.9/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.7.8/LICENSE` & `yplib-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.7.8/setup.py` & `yplib-1.7.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.7.8",
+  version="1.7.9",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.7.8/yplib/chart.py` & `yplib-1.7.9/yplib/chart.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,20 +100,19 @@
             # 第二行开始的数据
             if index > 0:
                 for y in range(1, len(line_one)):
                     y_list[y - 1]['data'].append(line_one[y])
     legend_data = []
     legend_selected = {}
     for y_one in y_list:
-        legend_data.append(y_one['name'])
+        name_one = y_one['name']
+        legend_data.append(name_one)
         if 'hide' in y_one and y_one['hide']:
-            legend_selected[y_one['name']] = 0
-        else:
-            legend_selected[y_one['name']] = 1
-    legend = "data : " + str(legend_data) + ", selected : " + str(legend_selected)
+            legend_selected[name_one] = 0
+    legend = 'data: ' + str(legend_data) + ',\n        selected: ' + str(legend_selected)
     # {
     #     name: 'Email',
     #     type: 'line',
     #     stack: 'Total',
     #     data: [120, 132, 101, 134, 90, 230, 210],
     # }
     series = []
@@ -133,14 +132,19 @@
     insert_data_to_chart(html_data=line_stack_html(),
                          name=name,
                          x_list=x_list,
                          legend=legend,
                          series=series)
 
 
+# print(str([1, 2, 3]))
+# print(str(['a', 'b', 'c']))
+# print(str(map(['a', 'b', 'c'])))
+# print(str(list(map(lambda x: {str(x): 0}, [1, 2, 3, 4]))))
+
 # 将数据整理成折线图
 # 一条折线
 # 数据 : data_list = [
 #             ['2020-01-01', 132],
 #             ['2021-01-01', 181],
 #             ['2022-01-01', 147]
 #         ]
@@ -309,15 +313,15 @@
 # y_list = []
 # # # x 轴有 100 个
 # # # 100 个横坐标
 # for i in range(100):
 #     x_list.append(i)
 # #
 # # 有 10 条线
-# for i in range(1):  # 0 1 2 3 4 55
+# for i in range(10):  # 0 1 2 3 4 55
 #     n = {}
 #     n['name'] = str(int(random.uniform(0, 1000)))
 #     data = []
 #     # 每条线有 100 个纵坐标, 与 x_list 中的对应起来
 #     for i in range(100):
 #         data.append(int(random.uniform(0, 1000)))
 #     n['data'] = data
@@ -325,16 +329,16 @@
 #     y_list.append(n)
 # #
 # to_chart(x_list, y_list)
 #
 #
 # test_list = []
 # for i in range(50):
-#     test_list.append([i, int(random.uniform(0, 1000))])
-#     test_list.append({'name': i, 'value': int(random.uniform(0, 1000))})
+#     test_list.append([i, int(random_int(4))])
+#     test_list.append({'name': i, 'value': int(random_int(4))})
 #
 # to_chart_one(test_list, name='yp')
 # to_chart_one(test_list, name='yp', smooth=True)
 # to_chart_one(test_list, name='yp', is_area=True)
 # to_chart_one(test_list, name='yp', is_area=True, smooth=True)
 #
 # data_list =
```

### Comparing `yplib-1.7.8/yplib/chart_html.py` & `yplib-1.7.9/yplib/chart_html.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
          '        myChart.setOption(option);',
          '    }',
          '    window.addEventListener("resize", myChart.resize);',
          '</script>',
          '</body>',
          '</html>',
          '']
-    return list(map(lambda x: x.replace('-option-', '\n'.join(option)), s))
+    return list(map(lambda x: x.replace('-option-', '\n    '.join(option)), s))
 
 
 # 折线图的 html 模板代码
 def line_stack_html():
     option = ['{',
               '    title: {',
               '        text: "-chart_name-",',
@@ -50,15 +50,17 @@
               '        left: "30px",',
               '        right: "40px",',
               '        bottom: "80px",',
               '        containLabel: true,',
               '    },',
               '    toolbox: {',
               '        feature: {',
-              '            saveAsImage: {pixelRatio:5},',
+              '            saveAsImage: {'
+              '                pixelRatio:5'
+              '            },',
               '        },',
               '    },',
               '    yAxis: {',
               '        type: "value",',
               '    },',
               '    xAxis: {',
               '        type: "category",',
@@ -80,15 +82,17 @@
               '    trigger: "axis",',
               '  },',
               '  title: {',
               '    text: "-chart_name-"',
               '  },',
               '  toolbox: {',
               '    feature: {',
-              '      saveAsImage: {pixelRatio:5}',
+              '       saveAsImage: {'
+              '           pixelRatio:5'
+              '       },',
               '    }',
               '  },',
               '    grid: {',
               '        left: "30px",',
               '        right: "40px",',
               '        bottom: "80px",',
               '        containLabel: true,',
@@ -147,15 +151,17 @@
               '    left: 10',
               '  },',
               '  tooltip: {',
               '    trigger: "item"',
               '  },',
               '    toolbox: {',
               '        feature: {',
-              '            saveAsImage: {pixelRatio:5},',
+              '            saveAsImage: {'
+              '                pixelRatio:5'
+              '            },',
               '        },',
               '    },',
               '  legend: {',
               '    top: "5%",',
               '    left: "center"',
               '  },',
               '  series: [',
@@ -194,15 +200,17 @@
               '  },',
               '  toolbox: {',
               '    feature: {',
               '      dataZoom: {',
               '        yAxisIndex: false',
               '      },',
               '      saveAsImage: {',
-              '        pixelRatio: 5',
+              '            saveAsImage: {'
+              '                pixelRatio:5'
+              '            },',
               '      }',
               '    }',
               '  },',
               '  tooltip: {',
               '    trigger: "axis",',
               '    axisPointer: {',
               '      type: "shadow"',
```

### Comparing `yplib-1.7.8/yplib/db.py` & `yplib-1.7.9/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.8/yplib/file.py` & `yplib-1.7.9/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.8/yplib/http_util.py` & `yplib-1.7.9/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.7.8/yplib/index.py` & `yplib-1.7.9/yplib/index.py`

 * *Files identical despite different names*


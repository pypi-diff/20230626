# Comparing `tmp/projhelper-0.1.7.tar.gz` & `tmp/projhelper-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projhelper-0.1.7.tar", last modified: Mon Jun 19 09:57:39 2023, max compression
+gzip compressed data, was "projhelper-0.1.8.tar", last modified: Mon Jun 26 07:04:36 2023, max compression
```

## Comparing `projhelper-0.1.7.tar` & `projhelper-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:57:39.139509 projhelper-0.1.7/
--rw-rw-rw-   0        0        0      148 2021-08-02 01:33:06.000000 projhelper-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      276 2023-06-19 09:57:39.139509 projhelper-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1650 2023-03-06 09:24:49.000000 projhelper-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 09:57:39.124508 projhelper-0.1.7/projhelper/
--rw-rw-rw-   0        0        0      155 2021-08-02 01:33:06.000000 projhelper-0.1.7/projhelper/__init__.py
--rw-rw-rw-   0        0        0     5281 2023-03-06 09:23:41.000000 projhelper-0.1.7/projhelper/ch_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:57:39.138507 projhelper-0.1.7/projhelper/conf/
--rw-rw-rw-   0        0        0      761 2021-08-02 01:33:06.000000 projhelper-0.1.7/projhelper/conf/conf_dev.cfg
--rw-rw-rw-   0        0        0     3065 2022-07-15 03:08:40.000000 projhelper-0.1.7/projhelper/conf/logging.cfg
--rw-rw-rw-   0        0        0     2718 2022-07-15 03:12:09.000000 projhelper-0.1.7/projhelper/conf/logging_win.cfg
--rw-rw-rw-   0        0        0     5502 2023-06-19 09:55:52.000000 projhelper-0.1.7/projhelper/dbGenerator.py
--rw-rw-rw-   0        0        0     1933 2022-07-15 02:38:28.000000 projhelper-0.1.7/projhelper/loadConf.py
--rw-rw-rw-   0        0        0     1772 2022-07-15 03:43:37.000000 projhelper-0.1.7/projhelper/log.py
--rw-rw-rw-   0        0        0     2023 2022-07-15 03:31:48.000000 projhelper-0.1.7/projhelper/osCmd.py
--rw-rw-rw-   0        0        0     1734 2022-12-19 01:25:51.000000 projhelper-0.1.7/projhelper/pushPrometheus.py
--rw-rw-rw-   0        0        0      332 2021-08-02 01:33:06.000000 projhelper-0.1.7/projhelper/setenv.py
--rw-rw-rw-   0        0        0     1127 2022-07-15 03:33:03.000000 projhelper-0.1.7/projhelper/timeHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:57:39.135512 projhelper-0.1.7/projhelper.egg-info/
--rw-rw-rw-   0        0        0      276 2023-06-19 09:57:39.000000 projhelper-0.1.7/projhelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-06-19 09:57:39.000000 projhelper-0.1.7/projhelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:57:39.000000 projhelper-0.1.7/projhelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 09:57:39.000000 projhelper-0.1.7/projhelper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 09:57:39.139509 projhelper-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      720 2023-06-19 09:57:37.000000 projhelper-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:04:36.792993 projhelper-0.1.8/
+-rw-rw-rw-   0        0        0      148 2021-08-02 01:33:06.000000 projhelper-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      276 2023-06-26 07:04:36.792993 projhelper-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1650 2023-06-26 07:04:32.000000 projhelper-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 07:04:36.756999 projhelper-0.1.8/projhelper/
+-rw-rw-rw-   0        0        0      155 2021-08-02 01:33:06.000000 projhelper-0.1.8/projhelper/__init__.py
+-rw-rw-rw-   0        0        0     5281 2023-03-06 09:23:41.000000 projhelper-0.1.8/projhelper/ch_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:04:36.790996 projhelper-0.1.8/projhelper/conf/
+-rw-rw-rw-   0        0        0      761 2021-08-02 01:33:06.000000 projhelper-0.1.8/projhelper/conf/conf_dev.cfg
+-rw-rw-rw-   0        0        0     3065 2022-07-15 03:08:40.000000 projhelper-0.1.8/projhelper/conf/logging.cfg
+-rw-rw-rw-   0        0        0     2718 2022-07-15 03:12:09.000000 projhelper-0.1.8/projhelper/conf/logging_win.cfg
+-rw-rw-rw-   0        0        0     5502 2023-06-19 10:02:59.000000 projhelper-0.1.8/projhelper/dbGenerator.py
+-rw-rw-rw-   0        0        0     2040 2023-06-26 07:03:39.000000 projhelper-0.1.8/projhelper/loadConf.py
+-rw-rw-rw-   0        0        0     1772 2023-06-26 06:58:26.000000 projhelper-0.1.8/projhelper/log.py
+-rw-rw-rw-   0        0        0     2023 2022-07-15 03:31:48.000000 projhelper-0.1.8/projhelper/osCmd.py
+-rw-rw-rw-   0        0        0     1734 2022-12-19 01:25:51.000000 projhelper-0.1.8/projhelper/pushPrometheus.py
+-rw-rw-rw-   0        0        0      332 2021-08-02 01:33:06.000000 projhelper-0.1.8/projhelper/setenv.py
+-rw-rw-rw-   0        0        0     1127 2022-07-15 03:33:03.000000 projhelper-0.1.8/projhelper/timeHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:04:36.770993 projhelper-0.1.8/projhelper.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-06-26 07:04:36.000000 projhelper-0.1.8/projhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-06-26 07:04:36.000000 projhelper-0.1.8/projhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 07:04:36.000000 projhelper-0.1.8/projhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-26 07:04:36.000000 projhelper-0.1.8/projhelper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 07:04:36.792993 projhelper-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      720 2023-06-26 07:04:32.000000 projhelper-0.1.8/setup.py
```

### Comparing `projhelper-0.1.7/README.md` & `projhelper-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## 说明
     本包名字为*packer*,使用方法包括...
 
 ### 打包方法
     python .\setup.py sdist
 ### 上传
     #pip install twine  #安装后 OS 有twine 命令:  ojh , ojhxxx
-    twine upload dist\projhelper-0.1.6.tar.gz
+    twine upload dist\projhelper-0.1.8.tar.gz
     
 ### 安装方法
     pip install projhelper
 
 ###调用方法
     1:在main.py 里 切换到工作目录, :
         import sys
```

### Comparing `projhelper-0.1.7/projhelper/ch_helper.py` & `projhelper-0.1.8/projhelper/ch_helper.py`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.7/projhelper/conf/conf_dev.cfg` & `projhelper-0.1.8/projhelper/conf/conf_dev.cfg`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.7/projhelper/conf/logging.cfg` & `projhelper-0.1.8/projhelper/conf/logging.cfg`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.7/projhelper/conf/logging_win.cfg` & `projhelper-0.1.8/projhelper/conf/logging_win.cfg`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.7/projhelper/dbGenerator.py` & `projhelper-0.1.8/projhelper/dbGenerator.py`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.7/projhelper/loadConf.py` & `projhelper-0.1.8/projhelper/loadConf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 import configparser as ConfigParser
 import os
 import codecs
 import sys
-from log import logger
+from projhelper.log import logger
 
 #修复key全转为小写问题
 class MyConfigParser(ConfigParser.SafeConfigParser):
     def __init__(self, defaults=None):
         ConfigParser.SafeConfigParser.__init__(self, defaults=defaults)
     def optionxform(self, optionstr):
         return optionstr
@@ -28,15 +28,15 @@
 
 def main(conf_file=''):
     #没传配置文件时, 需要传环境参数 prod|dev|test 等用于对应的配置文件
     if conf_file=='':
         try:
             env=sys.argv[1]
         except BaseException as e:
-            raise Exception("paramsError: usage : python main.py env  [other params ] , env use for conf file , like prod|dev|test")
+            raise Exception("paramsError: usage : \n    1: python main.py env [other params ] , env use for conf file , like prod|dev|test . \n    2: or set param like config=loadConf.main(conf_file='conf/conf_dev.cfg') when  ")
         #默认取项目路径下 conf/conf_xxx 配置文件
         conf_file =os.path.join(os.getcwd(),'conf','conf_%s.cfg'%sys.argv[1])
     config=read_conf(conf_file)
     return(config)
 
 if __name__ == '__main__':
     config=main()
```

### Comparing `projhelper-0.1.7/projhelper/log.py` & `projhelper-0.1.8/projhelper/log.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 #通过调用时指定配置文件 调用时如： main.py dev|prod
 try:
     env = sys.argv[1]
 except BaseException as e:
     env='prod'
 
-log_dir="logs"  #日志目录在运行路径下
 work_dir=os.getcwd()
+log_dir="logs"  #日志目录在运行路径下
 if not log_dir in os.listdir(work_dir):
      os.mkdir(os.path.join(work_dir,"logs"))
 
 #获取配置文件 WINDOWS 跟linux 的只是文件编码不一样，内容一样
 if platform.system() == 'Linux':
     conf_file_full_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'conf','logging.cfg')
 elif platform.system() == 'Windows':
```

### Comparing `projhelper-0.1.7/projhelper/osCmd.py` & `projhelper-0.1.8/projhelper/osCmd.py`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.7/projhelper/pushPrometheus.py` & `projhelper-0.1.8/projhelper/pushPrometheus.py`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.7/projhelper/timeHelper.py` & `projhelper-0.1.8/projhelper/timeHelper.py`

 * *Files identical despite different names*

### Comparing `projhelper-0.1.7/setup.py` & `projhelper-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @mail  : ojhtyy@163.com
 # @File    : setup.py
 from __future__ import print_function
 from setuptools import setup, find_packages
 import sys
 setup(
     name = "projhelper",
-    version = "0.1.7",
+    version = "0.1.8",
     keywords = ("pip", "datacanvas", "helper", "proj"),
     description = "project base helper, include logger ",
     long_description = "eds sdk for python",
     license = "MIT Licence",
 
     url = "",
     author = "oujh",
```


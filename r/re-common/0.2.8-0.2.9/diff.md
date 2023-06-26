# Comparing `tmp/re_common-0.2.8.tar.gz` & `tmp/re_common-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\re_common-0.2.8.tar", last modified: Fri Jul  2 07:42:10 2021, max compression
+gzip compressed data, was "dist\re_common-0.2.9.tar", last modified: Mon Jul  5 08:09:06 2021, max compression
```

## Comparing `re_common-0.2.8.tar` & `re_common-0.2.9.tar`

### file list

```diff
@@ -1,191 +1,191 @@
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:10.963183 re_common-0.2.8/
--rw-rw-rw-   0        0        0      623 2021-07-02 07:42:10.962186 re_common-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      173 2020-08-21 02:44:45.000000 re_common-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.284676 re_common-0.2.8/re_common/
--rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.298639 re_common-0.2.8/re_common/baselibrary/
--rw-rw-rw-   0        0        0      121 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.301630 re_common-0.2.8/re_common/baselibrary/baseabs/
--rw-rw-rw-   0        0        0      242 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/baseabs/__init__.py
--rw-rw-rw-   0        0        0      647 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/baseabs/baseabs.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.399369 re_common-0.2.8/re_common/baselibrary/database/
--rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/database/__init__.py
--rw-rw-rw-   0        0        0     3941 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/database/mbuilder.py
--rw-rw-rw-   0        0        0     2489 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/database/moudle.py
--rw-rw-rw-   0        0        0     4801 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/baselibrary/database/msqlite3.py
--rw-rw-rw-   0        0        0     4109 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/database/mysql.py
--rw-rw-rw-   0        0        0      790 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/database/sql_factory.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.432281 re_common-0.2.8/re_common/baselibrary/mthread/
--rw-rw-rw-   0        0        0    17957 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/mthread/MThreadingRun.py
--rw-rw-rw-   0        0        0    14410 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/mthread/MThreadingRunEvent.py
--rw-rw-rw-   0        0        0       28 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/baselibrary/mthread/__init__.py
--rw-rw-rw-   0        0        0    25658 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/mthread/mythreading.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.539134 re_common-0.2.8/re_common/baselibrary/readconfig/
--rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/readconfig/__init__.py
--rw-rw-rw-   0        0        0      590 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/readconfig/config_factory.py
--rw-rw-rw-   0        0        0     9330 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/readconfig/ini_config.py
--rw-rw-rw-   0        0        0     1311 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/readconfig/toml_config.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.554071 re_common-0.2.8/re_common/baselibrary/temporary/
--rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/temporary/__init__.py
--rw-rw-rw-   0        0        0      737 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/temporary/envdata.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.792570 re_common-0.2.8/re_common/baselibrary/tools/
--rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.834486 re_common-0.2.8/re_common/baselibrary/tools/all_requests/
--rw-rw-rw-   0        0        0        0 2020-10-16 09:08:00.000000 re_common-0.2.8/re_common/baselibrary/tools/all_requests/__init__.py
--rw-rw-rw-   0        0        0     3356 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/all_requests/aiohttp_request.py
--rw-rw-rw-   0        0        0     9658 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/tools/all_requests/mrequest.py
--rw-rw-rw-   0        0        0     2801 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/all_requests/requests_request.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.849418 re_common-0.2.8/re_common/baselibrary/tools/batch_compre/
--rw-rw-rw-   0        0        0        0 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/batch_compre/__init__.py
--rw-rw-rw-   0        0        0      783 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/batch_compre/bijiao_batch.py
--rw-rw-rw-   0        0        0     4269 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/contrast_db3.py
--rw-rw-rw-   0        0        0     1221 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/copy_file.py
--rw-rw-rw-   0        0        0     4166 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/db3_2_sizedb3.py
--rw-rw-rw-   0        0        0     1785 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/foreachgz.py
--rw-rw-rw-   0        0        0      248 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/baselibrary/tools/get_attr.py
--rw-rw-rw-   0        0        0     5157 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/tools/java_code_deal.py
--rw-rw-rw-   0        0        0     2779 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/javacode.py
--rw-rw-rw-   0        0        0     7936 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/merge_file.py
--rw-rw-rw-   0        0        0     6887 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/merge_gz_file.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.880335 re_common-0.2.8/re_common/baselibrary/tools/mhdfstools/
--rw-rw-rw-   0        0        0        0 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/mhdfstools/__init__.py
--rw-rw-rw-   0        0        0     1154 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/tools/mhdfstools/down_hdfs_files.py
--rw-rw-rw-   0        0        0     1281 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/baselibrary/tools/mhdfstools/hdfst.py
--rw-rw-rw-   0        0        0     1147 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/tools/mhdfstools/up_hdfs_files.py
--rw-rw-rw-   0        0        0     1954 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/mongo_tools.py
--rw-rw-rw-   0        0        0     5850 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/move_file.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.930201 re_common-0.2.8/re_common/baselibrary/tools/move_mongo/
--rw-rw-rw-   0        0        0        0 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/move_mongo/__init__.py
--rw-rw-rw-   0        0        0     2038 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/move_mongo/mongo_table_to_file.py
--rw-rw-rw-   0        0        0    13696 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/move_mongo/move_mongo_table.py
--rw-rw-rw-   0        0        0      403 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/move_mongo/use_mttf.py
--rw-rw-rw-   0        0        0     2192 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/move_mongo/use_mv.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.962118 re_common-0.2.8/re_common/baselibrary/tools/mpandas/
--rw-rw-rw-   0        0        0        0 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/mpandas/__init__.py
--rw-rw-rw-   0        0        0     3637 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/tools/mpandas/mpandasreadexcel.py
--rw-rw-rw-   0        0        0      174 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/mpandas/pandas_visualization.py
--rw-rw-rw-   0        0        0     3727 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/tools/myparsel.py
--rw-rw-rw-   0        0        0     1077 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/tools/rename_dir_file.py
--rw-rw-rw-   0        0        0      801 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/tools/split_line_to_many.py
--rw-rw-rw-   0        0        0      994 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/tools/stringtodicts.py
--rw-rw-rw-   0        0        0     2902 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/tools/workwechant_bot.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:10.450234 re_common-0.2.8/re_common/baselibrary/utils/
--rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/utils/__init__.py
--rw-rw-rw-   0        0        0    12903 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/baseaiohttp.py
--rw-rw-rw-   0        0        0     2658 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/utils/baseaiomysql.py
--rw-rw-rw-   0        0        0     6052 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/baseallstep.py
--rw-rw-rw-   0        0        0      532 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/baselibrary/utils/baseavro.py
--rw-rw-rw-   0        0        0      920 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/baselibrary/utils/basecsv.py
--rw-rw-rw-   0        0        0     4339 2021-06-09 05:45:51.000000 re_common-0.2.8/re_common/baselibrary/utils/basedict.py
--rw-rw-rw-   0        0        0     8429 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/basedir.py
--rw-rw-rw-   0        0        0     1436 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/baseencode.py
--rw-rw-rw-   0        0        0      779 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/baseencoding.py
--rw-rw-rw-   0        0        0     8093 2020-09-17 08:19:26.000000 re_common-0.2.8/re_common/baselibrary/utils/baseexcel.py
--rw-rw-rw-   0        0        0     3554 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/utils/baseexcept.py
--rw-rw-rw-   0        0        0    20295 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/basefile.py
--rw-rw-rw-   0        0        0      696 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/baselibrary/utils/baseftp.py
--rw-rw-rw-   0        0        0     1421 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/basegzip.py
--rw-rw-rw-   0        0        0     5055 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/utils/basehdfs.py
--rw-rw-rw-   0        0        0     9503 2020-09-17 08:19:26.000000 re_common-0.2.8/re_common/baselibrary/utils/basehttpx.py
--rw-rw-rw-   0        0        0     2577 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/baseip.py
--rw-rw-rw-   0        0        0        4 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/utils/basejson.py
--rw-rw-rw-   0        0        0      896 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/baselist.py
--rw-rw-rw-   0        0        0     4642 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/basemotor.py
--rw-rw-rw-   0        0        0     3265 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/baselibrary/utils/basemssql.py
--rw-rw-rw-   0        0        0     2364 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/baseodbc.py
--rw-rw-rw-   0        0        0     7729 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/basepandas.py
--rw-rw-rw-   0        0        0      220 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/utils/basepeewee.py
--rw-rw-rw-   0        0        0     7332 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/baselibrary/utils/basepika.py
--rw-rw-rw-   0        0        0     6309 2021-06-10 07:58:27.000000 re_common-0.2.8/re_common/baselibrary/utils/basepymongo.py
--rw-rw-rw-   0        0        0      481 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/utils/basequeue.py
--rw-rw-rw-   0        0        0    10581 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/utils/baserequest.py
--rw-rw-rw-   0        0        0      150 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/utils/baseset.py
--rw-rw-rw-   0        0        0     5376 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/basesmb.py
--rw-rw-rw-   0        0        0    11696 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/utils/basestring.py
--rw-rw-rw-   0        0        0     9975 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/utils/basetime.py
--rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/utils/basetuple.py
--rw-rw-rw-   0        0        0     4898 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/utils/baseurl.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:10.479156 re_common-0.2.8/re_common/baselibrary/utils/core/
--rw-rw-rw-   0        0        0      177 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/utils/core/__init__.py
--rw-rw-rw-   0        0        0      484 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/core/bottomutils.py
--rw-rw-rw-   0        0        0     8442 2021-07-02 07:41:12.000000 re_common-0.2.8/re_common/baselibrary/utils/core/mdeprecated.py
--rw-rw-rw-   0        0        0      687 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/core/mlamada.py
--rw-rw-rw-   0        0        0     4212 2021-06-08 05:10:00.000000 re_common-0.2.8/re_common/baselibrary/utils/core/requests_core.py
--rw-rw-rw-   0        0        0    15737 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/fateadm.py
--rw-rw-rw-   0        0        0     3707 2021-06-08 05:08:59.000000 re_common-0.2.8/re_common/baselibrary/utils/importfun.py
--rw-rw-rw-   0        0        0     1180 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/baselibrary/utils/mfaker.py
--rw-rw-rw-   0        0        0    16412 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/mylogger.py
--rw-rw-rw-   0        0        0    30897 2021-06-08 05:09:00.000000 re_common-0.2.8/re_common/baselibrary/utils/myredisclient.py
--rw-rw-rw-   0        0        0      548 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/pipupgrade.py
--rw-rw-rw-   0        0        0     2077 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/baselibrary/utils/ringlist.py
--rw-rw-rw-   0        0        0     4529 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/baselibrary/utils/ydmhttp.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:10.520047 re_common-0.2.8/re_common/facade/
--rw-rw-rw-   0        0        0       31 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/facade/__init__.py
--rw-rw-rw-   0        0        0      298 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/facade/lazy_import.py
--rw-rw-rw-   0        0        0      500 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/facade/loggerfacade.py
--rw-rw-rw-   0        0        0    18632 2021-06-08 05:09:00.000000 re_common-0.2.8/re_common/facade/mysqlfacade.py
--rw-rw-rw-   0        0        0      746 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/facade/now.py
--rw-rw-rw-   0        0        0     8392 2021-07-02 03:10:35.000000 re_common-0.2.8/re_common/facade/sqlite3facade.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:10.545978 re_common-0.2.8/re_common/facade/use/
--rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/facade/use/__init__.py
--rw-rw-rw-   0        0        0     1747 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/facade/use/mq_use_facade.py
--rw-rw-rw-   0        0        0      692 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/facade/use/proxy_use_facade.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:10.739662 re_common-0.2.8/re_common/libtest/
--rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/libtest/__init__.py
--rw-rw-rw-   0        0        0      605 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/libtest/base_dict_test.py
--rw-rw-rw-   0        0        0      336 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/libtest/baseavro_test.py
--rw-rw-rw-   0        0        0     2306 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/libtest/basemssql_test.py
--rw-rw-rw-   0        0        0      326 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/libtest/baseodbc_test.py
--rw-rw-rw-   0        0        0     1509 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/libtest/basepandas_test.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:10.752629 re_common-0.2.8/re_common/libtest/get_attr_test/
--rw-rw-rw-   0        0        0        0 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/libtest/get_attr_test/__init__.py
--rw-rw-rw-   0        0        0      348 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/libtest/get_attr_test/get_attr_test_settings.py
--rw-rw-rw-   0        0        0      973 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/libtest/get_attr_test/settings.py
--rw-rw-rw-   0        0        0     1481 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/libtest/idencode_test.py
--rw-rw-rw-   0        0        0     1296 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/libtest/iniconfig_test.py
--rw-rw-rw-   0        0        0     1054 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/libtest/ip_test.py
--rw-rw-rw-   0        0        0      687 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/libtest/merge_file_test.py
--rw-rw-rw-   0        0        0      589 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/libtest/mfaker_test.py
--rw-rw-rw-   0        0        0      174 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/libtest/mm3_test.py
--rw-rw-rw-   0        0        0     3023 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/libtest/mylogger_test.py
--rw-rw-rw-   0        0        0      888 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/libtest/myparsel_test.py
--rw-rw-rw-   0        0        0     4830 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/libtest/mysql_test.py
--rw-rw-rw-   0        0        0      519 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/libtest/pymongo_test.py
--rw-rw-rw-   0        0        0      289 2020-09-17 08:19:26.000000 re_common-0.2.8/re_common/libtest/redis_test.py
--rw-rw-rw-   0        0        0      437 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/libtest/split_test.py
--rw-rw-rw-   0        0        0      319 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/libtest/sqlite3_merge_test.py
--rw-rw-rw-   0        0        0      885 2021-04-19 06:54:20.000000 re_common-0.2.8/re_common/libtest/sqlite3_test.py
--rw-rw-rw-   0        0        0      976 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/libtest/tomlconfig_test.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:10.759611 re_common-0.2.8/re_common/libtest/use_tools_test/
--rw-rw-rw-   0        0        0       42 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/libtest/use_tools_test/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:10.763609 re_common-0.2.8/re_common/libtest/user/
--rw-rw-rw-   0        0        0      125 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/libtest/user/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:10.774569 re_common-0.2.8/re_common/studio/
--rw-rw-rw-   0        0        0      305 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/studio/__init__.py
--rw-rw-rw-   0        0        0     1331 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/studio/assignment_expressions.py
--rw-rw-rw-   0        0        0     9104 2020-10-16 09:08:00.000000 re_common-0.2.8/re_common/studio/async.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:10.842388 re_common-0.2.8/re_common/vip/
--rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/vip/__init__.py
--rw-rw-rw-   0        0        0      205 2021-04-19 06:54:21.000000 re_common-0.2.8/re_common/vip/base_step_process.py
--rw-rw-rw-   0        0        0     3272 2021-06-08 05:09:00.000000 re_common-0.2.8/re_common/vip/baseencodeid.py
--rw-rw-rw-   0        0        0     1087 2021-04-19 06:54:21.000000 re_common-0.2.8/re_common/vip/changetaskname.py
--rw-rw-rw-   0        0        0     1991 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/vip/core_var.py
--rw-rw-rw-   0        0        0     3133 2021-04-19 06:54:21.000000 re_common-0.2.8/re_common/vip/mmh3Hash.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:10.944239 re_common-0.2.8/re_common/vip/proxy/
--rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/vip/proxy/__init__.py
--rw-rw-rw-   0        0        0     5002 2021-04-19 06:54:21.000000 re_common-0.2.8/re_common/vip/proxy/allproxys.py
--rw-rw-rw-   0        0        0     5993 2021-04-19 06:54:21.000000 re_common-0.2.8/re_common/vip/proxy/allproxys_thread.py
--rw-rw-rw-   0        0        0     5644 2021-04-19 06:54:21.000000 re_common-0.2.8/re_common/vip/proxy/cnki_proxy.py
--rw-rw-rw-   0        0        0     3380 2021-04-19 06:54:21.000000 re_common-0.2.8/re_common/vip/proxy/kuaidaili.py
--rw-rw-rw-   0        0        0     3954 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/vip/proxy/proxy_all.py
--rw-rw-rw-   0        0        0     1284 2020-08-21 02:44:45.000000 re_common-0.2.8/re_common/vip/proxy/update_kuaidaili_0.py
--rw-rw-rw-   0        0        0     5669 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/vip/proxy/wanfang_proxy.py
--rw-rw-rw-   0        0        0     6924 2021-04-19 06:54:21.000000 re_common-0.2.8/re_common/vip/proxy/wp_proxy_all.py
--rw-rw-rw-   0        0        0     2889 2020-08-12 01:14:20.000000 re_common-0.2.8/re_common/vip/read_rawid_to_txt.py
-drwxrwxrwx   0        0        0        0 2021-07-02 07:42:09.296644 re_common-0.2.8/re_common.egg-info/
--rw-rw-rw-   0        0        0      623 2021-07-02 07:42:07.000000 re_common-0.2.8/re_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6589 2021-07-02 07:42:07.000000 re_common-0.2.8/re_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-02 07:42:07.000000 re_common-0.2.8/re_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2021-07-02 07:42:07.000000 re_common-0.2.8/re_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-07-02 07:42:10.963183 re_common-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1536 2021-07-02 07:41:56.000000 re_common-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.365050 re_common-0.2.9/
+-rw-rw-rw-   0        0        0      623 2021-07-05 08:09:06.365050 re_common-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2020-08-21 02:44:45.000000 re_common-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:05.966309 re_common-0.2.9/re_common/
+-rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/__init__.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:05.977281 re_common-0.2.9/re_common/baselibrary/
+-rw-rw-rw-   0        0        0      121 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:05.981270 re_common-0.2.9/re_common/baselibrary/baseabs/
+-rw-rw-rw-   0        0        0      242 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/baseabs/__init__.py
+-rw-rw-rw-   0        0        0      647 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/baseabs/baseabs.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:05.991243 re_common-0.2.9/re_common/baselibrary/database/
+-rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/database/__init__.py
+-rw-rw-rw-   0        0        0     3941 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/database/mbuilder.py
+-rw-rw-rw-   0        0        0     2489 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/database/moudle.py
+-rw-rw-rw-   0        0        0     4801 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/baselibrary/database/msqlite3.py
+-rw-rw-rw-   0        0        0     4109 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/database/mysql.py
+-rw-rw-rw-   0        0        0      790 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/database/sql_factory.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:05.998224 re_common-0.2.9/re_common/baselibrary/mthread/
+-rw-rw-rw-   0        0        0    17957 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/mthread/MThreadingRun.py
+-rw-rw-rw-   0        0        0    14410 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/mthread/MThreadingRunEvent.py
+-rw-rw-rw-   0        0        0       28 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/baselibrary/mthread/__init__.py
+-rw-rw-rw-   0        0        0    25658 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/mthread/mythreading.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.008197 re_common-0.2.9/re_common/baselibrary/readconfig/
+-rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/readconfig/__init__.py
+-rw-rw-rw-   0        0        0      590 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/readconfig/config_factory.py
+-rw-rw-rw-   0        0        0     9330 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/readconfig/ini_config.py
+-rw-rw-rw-   0        0        0     1311 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/readconfig/toml_config.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.013184 re_common-0.2.9/re_common/baselibrary/temporary/
+-rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/temporary/__init__.py
+-rw-rw-rw-   0        0        0      737 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/temporary/envdata.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.052079 re_common-0.2.9/re_common/baselibrary/tools/
+-rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.063051 re_common-0.2.9/re_common/baselibrary/tools/all_requests/
+-rw-rw-rw-   0        0        0        0 2020-10-16 09:08:00.000000 re_common-0.2.9/re_common/baselibrary/tools/all_requests/__init__.py
+-rw-rw-rw-   0        0        0     3356 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/all_requests/aiohttp_request.py
+-rw-rw-rw-   0        0        0     9658 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/tools/all_requests/mrequest.py
+-rw-rw-rw-   0        0        0     2801 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/all_requests/requests_request.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.066042 re_common-0.2.9/re_common/baselibrary/tools/batch_compre/
+-rw-rw-rw-   0        0        0        0 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/batch_compre/__init__.py
+-rw-rw-rw-   0        0        0      783 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/batch_compre/bijiao_batch.py
+-rw-rw-rw-   0        0        0     4269 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/contrast_db3.py
+-rw-rw-rw-   0        0        0     1221 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/copy_file.py
+-rw-rw-rw-   0        0        0     4166 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/db3_2_sizedb3.py
+-rw-rw-rw-   0        0        0     1785 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/foreachgz.py
+-rw-rw-rw-   0        0        0      248 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/baselibrary/tools/get_attr.py
+-rw-rw-rw-   0        0        0     5157 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/tools/java_code_deal.py
+-rw-rw-rw-   0        0        0     2779 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/javacode.py
+-rw-rw-rw-   0        0        0     7936 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/merge_file.py
+-rw-rw-rw-   0        0        0     6887 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/merge_gz_file.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.074049 re_common-0.2.9/re_common/baselibrary/tools/mhdfstools/
+-rw-rw-rw-   0        0        0        0 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/mhdfstools/__init__.py
+-rw-rw-rw-   0        0        0     1154 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/tools/mhdfstools/down_hdfs_files.py
+-rw-rw-rw-   0        0        0     1281 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/baselibrary/tools/mhdfstools/hdfst.py
+-rw-rw-rw-   0        0        0     1147 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/tools/mhdfstools/up_hdfs_files.py
+-rw-rw-rw-   0        0        0     1954 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/mongo_tools.py
+-rw-rw-rw-   0        0        0     5850 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/move_file.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.085989 re_common-0.2.9/re_common/baselibrary/tools/move_mongo/
+-rw-rw-rw-   0        0        0        0 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/move_mongo/__init__.py
+-rw-rw-rw-   0        0        0     2038 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/move_mongo/mongo_table_to_file.py
+-rw-rw-rw-   0        0        0    13696 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/move_mongo/move_mongo_table.py
+-rw-rw-rw-   0        0        0      403 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/move_mongo/use_mttf.py
+-rw-rw-rw-   0        0        0     2192 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/move_mongo/use_mv.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.095963 re_common-0.2.9/re_common/baselibrary/tools/mpandas/
+-rw-rw-rw-   0        0        0        0 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/mpandas/__init__.py
+-rw-rw-rw-   0        0        0     3637 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/tools/mpandas/mpandasreadexcel.py
+-rw-rw-rw-   0        0        0      174 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/mpandas/pandas_visualization.py
+-rw-rw-rw-   0        0        0     3727 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/tools/myparsel.py
+-rw-rw-rw-   0        0        0     1077 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/tools/rename_dir_file.py
+-rw-rw-rw-   0        0        0      801 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/tools/split_line_to_many.py
+-rw-rw-rw-   0        0        0      994 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/tools/stringtodicts.py
+-rw-rw-rw-   0        0        0     2902 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/tools/workwechant_bot.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.190518 re_common-0.2.9/re_common/baselibrary/utils/
+-rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/utils/__init__.py
+-rw-rw-rw-   0        0        0    12903 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/baseaiohttp.py
+-rw-rw-rw-   0        0        0     2658 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/utils/baseaiomysql.py
+-rw-rw-rw-   0        0        0     6052 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/baseallstep.py
+-rw-rw-rw-   0        0        0      532 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/baselibrary/utils/baseavro.py
+-rw-rw-rw-   0        0        0      920 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/baselibrary/utils/basecsv.py
+-rw-rw-rw-   0        0        0     4339 2021-06-09 05:45:51.000000 re_common-0.2.9/re_common/baselibrary/utils/basedict.py
+-rw-rw-rw-   0        0        0     8429 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/basedir.py
+-rw-rw-rw-   0        0        0     1436 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/baseencode.py
+-rw-rw-rw-   0        0        0      779 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/baseencoding.py
+-rw-rw-rw-   0        0        0     8093 2020-09-17 08:19:26.000000 re_common-0.2.9/re_common/baselibrary/utils/baseexcel.py
+-rw-rw-rw-   0        0        0     3554 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/utils/baseexcept.py
+-rw-rw-rw-   0        0        0    20295 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/basefile.py
+-rw-rw-rw-   0        0        0      696 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/baselibrary/utils/baseftp.py
+-rw-rw-rw-   0        0        0     1421 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/basegzip.py
+-rw-rw-rw-   0        0        0     5055 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/utils/basehdfs.py
+-rw-rw-rw-   0        0        0     9503 2020-09-17 08:19:26.000000 re_common-0.2.9/re_common/baselibrary/utils/basehttpx.py
+-rw-rw-rw-   0        0        0     2577 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/baseip.py
+-rw-rw-rw-   0        0        0        4 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/utils/basejson.py
+-rw-rw-rw-   0        0        0      896 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/baselist.py
+-rw-rw-rw-   0        0        0     4642 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/basemotor.py
+-rw-rw-rw-   0        0        0     3265 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/baselibrary/utils/basemssql.py
+-rw-rw-rw-   0        0        0     2364 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/baseodbc.py
+-rw-rw-rw-   0        0        0     7729 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/basepandas.py
+-rw-rw-rw-   0        0        0      220 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/utils/basepeewee.py
+-rw-rw-rw-   0        0        0     7332 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/baselibrary/utils/basepika.py
+-rw-rw-rw-   0        0        0     6309 2021-06-10 07:58:27.000000 re_common-0.2.9/re_common/baselibrary/utils/basepymongo.py
+-rw-rw-rw-   0        0        0      481 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/utils/basequeue.py
+-rw-rw-rw-   0        0        0    10581 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/utils/baserequest.py
+-rw-rw-rw-   0        0        0      150 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/utils/baseset.py
+-rw-rw-rw-   0        0        0     5376 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/basesmb.py
+-rw-rw-rw-   0        0        0    11696 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/utils/basestring.py
+-rw-rw-rw-   0        0        0     9975 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/utils/basetime.py
+-rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/utils/basetuple.py
+-rw-rw-rw-   0        0        0     4898 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/utils/baseurl.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.204480 re_common-0.2.9/re_common/baselibrary/utils/core/
+-rw-rw-rw-   0        0        0      177 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/utils/core/__init__.py
+-rw-rw-rw-   0        0        0      484 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/core/bottomutils.py
+-rw-rw-rw-   0        0        0     8448 2021-07-05 08:08:08.000000 re_common-0.2.9/re_common/baselibrary/utils/core/mdeprecated.py
+-rw-rw-rw-   0        0        0      687 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/core/mlamada.py
+-rw-rw-rw-   0        0        0     4212 2021-06-08 05:10:00.000000 re_common-0.2.9/re_common/baselibrary/utils/core/requests_core.py
+-rw-rw-rw-   0        0        0    15737 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/fateadm.py
+-rw-rw-rw-   0        0        0     3707 2021-06-08 05:08:59.000000 re_common-0.2.9/re_common/baselibrary/utils/importfun.py
+-rw-rw-rw-   0        0        0     1180 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/baselibrary/utils/mfaker.py
+-rw-rw-rw-   0        0        0    16412 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/mylogger.py
+-rw-rw-rw-   0        0        0    30897 2021-06-08 05:09:00.000000 re_common-0.2.9/re_common/baselibrary/utils/myredisclient.py
+-rw-rw-rw-   0        0        0      548 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/pipupgrade.py
+-rw-rw-rw-   0        0        0     2077 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/baselibrary/utils/ringlist.py
+-rw-rw-rw-   0        0        0     4529 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/baselibrary/utils/ydmhttp.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.216447 re_common-0.2.9/re_common/facade/
+-rw-rw-rw-   0        0        0       31 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/facade/__init__.py
+-rw-rw-rw-   0        0        0      298 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/facade/lazy_import.py
+-rw-rw-rw-   0        0        0      500 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/facade/loggerfacade.py
+-rw-rw-rw-   0        0        0    18632 2021-06-08 05:09:00.000000 re_common-0.2.9/re_common/facade/mysqlfacade.py
+-rw-rw-rw-   0        0        0      746 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/facade/now.py
+-rw-rw-rw-   0        0        0     8392 2021-07-02 03:10:35.000000 re_common-0.2.9/re_common/facade/sqlite3facade.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.222432 re_common-0.2.9/re_common/facade/use/
+-rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/facade/use/__init__.py
+-rw-rw-rw-   0        0        0     1747 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/facade/use/mq_use_facade.py
+-rw-rw-rw-   0        0        0      692 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/facade/use/proxy_use_facade.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.298229 re_common-0.2.9/re_common/libtest/
+-rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/libtest/__init__.py
+-rw-rw-rw-   0        0        0      605 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/libtest/base_dict_test.py
+-rw-rw-rw-   0        0        0      336 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/libtest/baseavro_test.py
+-rw-rw-rw-   0        0        0     2306 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/libtest/basemssql_test.py
+-rw-rw-rw-   0        0        0      326 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/libtest/baseodbc_test.py
+-rw-rw-rw-   0        0        0     1509 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/libtest/basepandas_test.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.303215 re_common-0.2.9/re_common/libtest/get_attr_test/
+-rw-rw-rw-   0        0        0        0 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/libtest/get_attr_test/__init__.py
+-rw-rw-rw-   0        0        0      348 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/libtest/get_attr_test/get_attr_test_settings.py
+-rw-rw-rw-   0        0        0      973 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/libtest/get_attr_test/settings.py
+-rw-rw-rw-   0        0        0     1481 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/libtest/idencode_test.py
+-rw-rw-rw-   0        0        0     1296 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/libtest/iniconfig_test.py
+-rw-rw-rw-   0        0        0     1054 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/libtest/ip_test.py
+-rw-rw-rw-   0        0        0      687 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/libtest/merge_file_test.py
+-rw-rw-rw-   0        0        0      589 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/libtest/mfaker_test.py
+-rw-rw-rw-   0        0        0      174 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/libtest/mm3_test.py
+-rw-rw-rw-   0        0        0     3023 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/libtest/mylogger_test.py
+-rw-rw-rw-   0        0        0      888 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/libtest/myparsel_test.py
+-rw-rw-rw-   0        0        0     4830 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/libtest/mysql_test.py
+-rw-rw-rw-   0        0        0      519 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/libtest/pymongo_test.py
+-rw-rw-rw-   0        0        0      289 2020-09-17 08:19:26.000000 re_common-0.2.9/re_common/libtest/redis_test.py
+-rw-rw-rw-   0        0        0      437 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/libtest/split_test.py
+-rw-rw-rw-   0        0        0      319 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/libtest/sqlite3_merge_test.py
+-rw-rw-rw-   0        0        0      885 2021-04-19 06:54:20.000000 re_common-0.2.9/re_common/libtest/sqlite3_test.py
+-rw-rw-rw-   0        0        0      976 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/libtest/tomlconfig_test.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.304212 re_common-0.2.9/re_common/libtest/use_tools_test/
+-rw-rw-rw-   0        0        0       42 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/libtest/use_tools_test/__init__.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.306207 re_common-0.2.9/re_common/libtest/user/
+-rw-rw-rw-   0        0        0      125 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/libtest/user/__init__.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.313189 re_common-0.2.9/re_common/studio/
+-rw-rw-rw-   0        0        0      305 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/studio/__init__.py
+-rw-rw-rw-   0        0        0     1331 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/studio/assignment_expressions.py
+-rw-rw-rw-   0        0        0     9104 2020-10-16 09:08:00.000000 re_common-0.2.9/re_common/studio/async.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.338122 re_common-0.2.9/re_common/vip/
+-rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/vip/__init__.py
+-rw-rw-rw-   0        0        0      205 2021-04-19 06:54:21.000000 re_common-0.2.9/re_common/vip/base_step_process.py
+-rw-rw-rw-   0        0        0     3272 2021-06-08 05:09:00.000000 re_common-0.2.9/re_common/vip/baseencodeid.py
+-rw-rw-rw-   0        0        0     1087 2021-04-19 06:54:21.000000 re_common-0.2.9/re_common/vip/changetaskname.py
+-rw-rw-rw-   0        0        0     1991 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/vip/core_var.py
+-rw-rw-rw-   0        0        0     3133 2021-04-19 06:54:21.000000 re_common-0.2.9/re_common/vip/mmh3Hash.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:06.362058 re_common-0.2.9/re_common/vip/proxy/
+-rw-rw-rw-   0        0        0        0 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/vip/proxy/__init__.py
+-rw-rw-rw-   0        0        0     5002 2021-04-19 06:54:21.000000 re_common-0.2.9/re_common/vip/proxy/allproxys.py
+-rw-rw-rw-   0        0        0     5993 2021-04-19 06:54:21.000000 re_common-0.2.9/re_common/vip/proxy/allproxys_thread.py
+-rw-rw-rw-   0        0        0     5644 2021-04-19 06:54:21.000000 re_common-0.2.9/re_common/vip/proxy/cnki_proxy.py
+-rw-rw-rw-   0        0        0     3380 2021-04-19 06:54:21.000000 re_common-0.2.9/re_common/vip/proxy/kuaidaili.py
+-rw-rw-rw-   0        0        0     3954 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/vip/proxy/proxy_all.py
+-rw-rw-rw-   0        0        0     1284 2020-08-21 02:44:45.000000 re_common-0.2.9/re_common/vip/proxy/update_kuaidaili_0.py
+-rw-rw-rw-   0        0        0     5669 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/vip/proxy/wanfang_proxy.py
+-rw-rw-rw-   0        0        0     6924 2021-04-19 06:54:21.000000 re_common-0.2.9/re_common/vip/proxy/wp_proxy_all.py
+-rw-rw-rw-   0        0        0     2889 2020-08-12 01:14:20.000000 re_common-0.2.9/re_common/vip/read_rawid_to_txt.py
+drwxrwxrwx   0        0        0        0 2021-07-05 08:09:05.974288 re_common-0.2.9/re_common.egg-info/
+-rw-rw-rw-   0        0        0      623 2021-07-05 08:09:05.000000 re_common-0.2.9/re_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6589 2021-07-05 08:09:05.000000 re_common-0.2.9/re_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-05 08:09:05.000000 re_common-0.2.9/re_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2021-07-05 08:09:05.000000 re_common-0.2.9/re_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-07-05 08:09:06.365050 re_common-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1536 2021-07-05 08:08:08.000000 re_common-0.2.9/setup.py
```

### Comparing `re_common-0.2.8/PKG-INFO` & `re_common-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re_common
-Version: 0.2.8
+Version: 0.2.9
 Summary: a library about all python projects
 Home-page: https://gitee.com/xujiangios/re-common
 Author: vic
 Author-email: xujiang5@163.com
 License: UNKNOWN
 Description: 
             这是一个基础类，依赖很多的第三方包，是一个用得到的第三方库的封装，可以在此基础上迅速构建项目
```

### Comparing `re_common-0.2.8/re_common/baselibrary/baseabs/baseabs.py` & `re_common-0.2.9/re_common/baselibrary/baseabs/baseabs.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/database/mbuilder.py` & `re_common-0.2.9/re_common/baselibrary/database/mbuilder.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/database/moudle.py` & `re_common-0.2.9/re_common/baselibrary/database/moudle.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/database/msqlite3.py` & `re_common-0.2.9/re_common/baselibrary/database/msqlite3.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/database/mysql.py` & `re_common-0.2.9/re_common/baselibrary/database/mysql.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/database/sql_factory.py` & `re_common-0.2.9/re_common/baselibrary/database/sql_factory.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/mthread/MThreadingRun.py` & `re_common-0.2.9/re_common/baselibrary/mthread/MThreadingRun.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/mthread/MThreadingRunEvent.py` & `re_common-0.2.9/re_common/baselibrary/mthread/MThreadingRunEvent.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/mthread/mythreading.py` & `re_common-0.2.9/re_common/baselibrary/mthread/mythreading.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/readconfig/config_factory.py` & `re_common-0.2.9/re_common/baselibrary/readconfig/config_factory.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/readconfig/ini_config.py` & `re_common-0.2.9/re_common/baselibrary/readconfig/ini_config.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/readconfig/toml_config.py` & `re_common-0.2.9/re_common/baselibrary/readconfig/toml_config.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/temporary/envdata.py` & `re_common-0.2.9/re_common/baselibrary/temporary/envdata.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/all_requests/aiohttp_request.py` & `re_common-0.2.9/re_common/baselibrary/tools/all_requests/aiohttp_request.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/all_requests/mrequest.py` & `re_common-0.2.9/re_common/baselibrary/tools/all_requests/mrequest.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/all_requests/requests_request.py` & `re_common-0.2.9/re_common/baselibrary/tools/all_requests/requests_request.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/batch_compre/bijiao_batch.py` & `re_common-0.2.9/re_common/baselibrary/tools/batch_compre/bijiao_batch.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/contrast_db3.py` & `re_common-0.2.9/re_common/baselibrary/tools/contrast_db3.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/copy_file.py` & `re_common-0.2.9/re_common/baselibrary/tools/copy_file.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/db3_2_sizedb3.py` & `re_common-0.2.9/re_common/baselibrary/tools/db3_2_sizedb3.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/foreachgz.py` & `re_common-0.2.9/re_common/baselibrary/tools/foreachgz.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/java_code_deal.py` & `re_common-0.2.9/re_common/baselibrary/tools/java_code_deal.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/javacode.py` & `re_common-0.2.9/re_common/baselibrary/tools/javacode.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/merge_file.py` & `re_common-0.2.9/re_common/baselibrary/tools/merge_file.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/merge_gz_file.py` & `re_common-0.2.9/re_common/baselibrary/tools/merge_gz_file.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/mhdfstools/down_hdfs_files.py` & `re_common-0.2.9/re_common/baselibrary/tools/mhdfstools/down_hdfs_files.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/mhdfstools/hdfst.py` & `re_common-0.2.9/re_common/baselibrary/tools/mhdfstools/hdfst.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/mhdfstools/up_hdfs_files.py` & `re_common-0.2.9/re_common/baselibrary/tools/mhdfstools/up_hdfs_files.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/mongo_tools.py` & `re_common-0.2.9/re_common/baselibrary/tools/mongo_tools.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/move_file.py` & `re_common-0.2.9/re_common/baselibrary/tools/move_file.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/move_mongo/mongo_table_to_file.py` & `re_common-0.2.9/re_common/baselibrary/tools/move_mongo/mongo_table_to_file.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/move_mongo/move_mongo_table.py` & `re_common-0.2.9/re_common/baselibrary/tools/move_mongo/move_mongo_table.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/move_mongo/use_mv.py` & `re_common-0.2.9/re_common/baselibrary/tools/move_mongo/use_mv.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/mpandas/mpandasreadexcel.py` & `re_common-0.2.9/re_common/baselibrary/tools/mpandas/mpandasreadexcel.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/myparsel.py` & `re_common-0.2.9/re_common/baselibrary/tools/myparsel.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/rename_dir_file.py` & `re_common-0.2.9/re_common/baselibrary/tools/rename_dir_file.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/split_line_to_many.py` & `re_common-0.2.9/re_common/baselibrary/tools/split_line_to_many.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/stringtodicts.py` & `re_common-0.2.9/re_common/baselibrary/tools/stringtodicts.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/tools/workwechant_bot.py` & `re_common-0.2.9/re_common/baselibrary/tools/workwechant_bot.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baseaiohttp.py` & `re_common-0.2.9/re_common/baselibrary/utils/baseaiohttp.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baseaiomysql.py` & `re_common-0.2.9/re_common/baselibrary/utils/baseaiomysql.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baseallstep.py` & `re_common-0.2.9/re_common/baselibrary/utils/baseallstep.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baseavro.py` & `re_common-0.2.9/re_common/baselibrary/utils/baseavro.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basecsv.py` & `re_common-0.2.9/re_common/baselibrary/utils/basecsv.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basedict.py` & `re_common-0.2.9/re_common/baselibrary/utils/basedict.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basedir.py` & `re_common-0.2.9/re_common/baselibrary/utils/basedir.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baseencode.py` & `re_common-0.2.9/re_common/baselibrary/utils/baseencode.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baseencoding.py` & `re_common-0.2.9/re_common/baselibrary/utils/baseencoding.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baseexcel.py` & `re_common-0.2.9/re_common/baselibrary/utils/baseexcel.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baseexcept.py` & `re_common-0.2.9/re_common/baselibrary/utils/baseexcept.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basefile.py` & `re_common-0.2.9/re_common/baselibrary/utils/basefile.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baseftp.py` & `re_common-0.2.9/re_common/baselibrary/utils/baseftp.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basegzip.py` & `re_common-0.2.9/re_common/baselibrary/utils/basegzip.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basehdfs.py` & `re_common-0.2.9/re_common/baselibrary/utils/basehdfs.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basehttpx.py` & `re_common-0.2.9/re_common/baselibrary/utils/basehttpx.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baseip.py` & `re_common-0.2.9/re_common/baselibrary/utils/baseip.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baselist.py` & `re_common-0.2.9/re_common/baselibrary/utils/baselist.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basemotor.py` & `re_common-0.2.9/re_common/baselibrary/utils/basemotor.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basemssql.py` & `re_common-0.2.9/re_common/baselibrary/utils/basemssql.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baseodbc.py` & `re_common-0.2.9/re_common/baselibrary/utils/baseodbc.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basepandas.py` & `re_common-0.2.9/re_common/baselibrary/utils/basepandas.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basepika.py` & `re_common-0.2.9/re_common/baselibrary/utils/basepika.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basepymongo.py` & `re_common-0.2.9/re_common/baselibrary/utils/basepymongo.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baserequest.py` & `re_common-0.2.9/re_common/baselibrary/utils/baserequest.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basesmb.py` & `re_common-0.2.9/re_common/baselibrary/utils/basesmb.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basestring.py` & `re_common-0.2.9/re_common/baselibrary/utils/basestring.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/basetime.py` & `re_common-0.2.9/re_common/baselibrary/utils/basetime.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/baseurl.py` & `re_common-0.2.9/re_common/baselibrary/utils/baseurl.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/core/mdeprecated.py` & `re_common-0.2.9/re_common/baselibrary/utils/core/mdeprecated.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         async def wrapper(*args, **kwargs):
             try:
                 return await func(*args, **kwargs)
             except BaseException as e:
                 if callback is not None:
                     if is_print:
                         print("traceback", traceback.format_exc())
-                    bools, one_dic = callback(*sys.exc_info(), *args, **kwargs)
+                    bools, one_dic = await callback(*sys.exc_info(), *args, **kwargs)
                     return bools, one_dic
 
                 return False, {"traceback": traceback.format_exc()}
 
         return wrapper
 
     return dewrapper
```

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/core/mlamada.py` & `re_common-0.2.9/re_common/baselibrary/utils/core/mlamada.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/core/requests_core.py` & `re_common-0.2.9/re_common/baselibrary/utils/core/requests_core.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/fateadm.py` & `re_common-0.2.9/re_common/baselibrary/utils/fateadm.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/importfun.py` & `re_common-0.2.9/re_common/baselibrary/utils/importfun.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/mfaker.py` & `re_common-0.2.9/re_common/baselibrary/utils/mfaker.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/mylogger.py` & `re_common-0.2.9/re_common/baselibrary/utils/mylogger.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/myredisclient.py` & `re_common-0.2.9/re_common/baselibrary/utils/myredisclient.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/pipupgrade.py` & `re_common-0.2.9/re_common/baselibrary/utils/pipupgrade.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/ringlist.py` & `re_common-0.2.9/re_common/baselibrary/utils/ringlist.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/baselibrary/utils/ydmhttp.py` & `re_common-0.2.9/re_common/baselibrary/utils/ydmhttp.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/facade/mysqlfacade.py` & `re_common-0.2.9/re_common/facade/mysqlfacade.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/facade/now.py` & `re_common-0.2.9/re_common/facade/now.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/facade/sqlite3facade.py` & `re_common-0.2.9/re_common/facade/sqlite3facade.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/facade/use/mq_use_facade.py` & `re_common-0.2.9/re_common/facade/use/mq_use_facade.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/facade/use/proxy_use_facade.py` & `re_common-0.2.9/re_common/facade/use/proxy_use_facade.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/base_dict_test.py` & `re_common-0.2.9/re_common/libtest/base_dict_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/basemssql_test.py` & `re_common-0.2.9/re_common/libtest/basemssql_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/basepandas_test.py` & `re_common-0.2.9/re_common/libtest/basepandas_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/get_attr_test/settings.py` & `re_common-0.2.9/re_common/libtest/get_attr_test/settings.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/idencode_test.py` & `re_common-0.2.9/re_common/libtest/idencode_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/iniconfig_test.py` & `re_common-0.2.9/re_common/libtest/iniconfig_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/ip_test.py` & `re_common-0.2.9/re_common/libtest/ip_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/merge_file_test.py` & `re_common-0.2.9/re_common/libtest/merge_file_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/mfaker_test.py` & `re_common-0.2.9/re_common/libtest/mfaker_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/mylogger_test.py` & `re_common-0.2.9/re_common/libtest/mylogger_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/myparsel_test.py` & `re_common-0.2.9/re_common/libtest/myparsel_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/mysql_test.py` & `re_common-0.2.9/re_common/libtest/mysql_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/pymongo_test.py` & `re_common-0.2.9/re_common/libtest/pymongo_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/sqlite3_test.py` & `re_common-0.2.9/re_common/libtest/sqlite3_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/libtest/tomlconfig_test.py` & `re_common-0.2.9/re_common/libtest/tomlconfig_test.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/studio/assignment_expressions.py` & `re_common-0.2.9/re_common/studio/assignment_expressions.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/studio/async.py` & `re_common-0.2.9/re_common/studio/async.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/baseencodeid.py` & `re_common-0.2.9/re_common/vip/baseencodeid.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/changetaskname.py` & `re_common-0.2.9/re_common/vip/changetaskname.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/core_var.py` & `re_common-0.2.9/re_common/vip/core_var.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/mmh3Hash.py` & `re_common-0.2.9/re_common/vip/mmh3Hash.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/proxy/allproxys.py` & `re_common-0.2.9/re_common/vip/proxy/allproxys.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/proxy/allproxys_thread.py` & `re_common-0.2.9/re_common/vip/proxy/allproxys_thread.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/proxy/cnki_proxy.py` & `re_common-0.2.9/re_common/vip/proxy/cnki_proxy.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/proxy/kuaidaili.py` & `re_common-0.2.9/re_common/vip/proxy/kuaidaili.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/proxy/proxy_all.py` & `re_common-0.2.9/re_common/vip/proxy/proxy_all.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/proxy/update_kuaidaili_0.py` & `re_common-0.2.9/re_common/vip/proxy/update_kuaidaili_0.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/proxy/wanfang_proxy.py` & `re_common-0.2.9/re_common/vip/proxy/wanfang_proxy.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/proxy/wp_proxy_all.py` & `re_common-0.2.9/re_common/vip/proxy/wp_proxy_all.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common/vip/read_rawid_to_txt.py` & `re_common-0.2.9/re_common/vip/read_rawid_to_txt.py`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/re_common.egg-info/PKG-INFO` & `re_common-0.2.9/re_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-common
-Version: 0.2.8
+Version: 0.2.9
 Summary: a library about all python projects
 Home-page: https://gitee.com/xujiangios/re-common
 Author: vic
 Author-email: xujiang5@163.com
 License: UNKNOWN
 Description: 
             这是一个基础类，依赖很多的第三方包，是一个用得到的第三方库的封装，可以在此基础上迅速构建项目
```

### Comparing `re_common-0.2.8/re_common.egg-info/SOURCES.txt` & `re_common-0.2.9/re_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `re_common-0.2.8/setup.py` & `re_common-0.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 """
 long_description = """
     这是一个基础类，依赖很多的第三方包，是一个用得到的第三方库的封装，可以在此基础上迅速构建项目
 """
 setuptools.setup(
     name="re_common",
 
-    version="0.2.8",
+    version="0.2.9",
     author="vic",
     author_email="xujiang5@163.com",
     description="a library about all python projects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/xujiangios/re-common",
     packages=setuptools.find_packages(),
```


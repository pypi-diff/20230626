# Comparing `tmp/chatllm-2023.6.2.9.16.47.tar.gz` & `tmp/chatllm-2023.6.26.13.31.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatllm-2023.6.2.9.16.47.tar", last modified: Fri Jun  2 01:16:47 2023, max compression
+gzip compressed data, was "chatllm-2023.6.26.13.31.16.tar", last modified: Mon Jun 26 05:31:17 2023, max compression
```

## Comparing `chatllm-2023.6.2.9.16.47.tar` & `chatllm-2023.6.26.13.31.16.tar`

### file list

```diff
@@ -1,133 +1,137 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.831497 chatllm-2023.6.2.9.16.47/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2023.6.2.9.16.47/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      342 2023-05-31 08:06:48.000000 chatllm-2023.6.2.9.16.47/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     6664 2023-06-02 01:16:47.831335 chatllm-2023.6.2.9.16.47/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     5935 2023-05-31 01:20:56.000000 chatllm-2023.6.2.9.16.47/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2023.6.2.9.16.47/README.md.bak
--rw-r--r--   0 betterme   (501) staff       (20)      898 2023-05-31 01:32:50.000000 chatllm-2023.6.2.9.16.47/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.810805 chatllm-2023.6.2.9.16.47/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.812262 chatllm-2023.6.2.9.16.47/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 chatllm-2023.6.2.9.16.47/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 chatllm-2023.6.2.9.16.47/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 chatllm-2023.6.2.9.16.47/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 chatllm-2023.6.2.9.16.47/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.812562 chatllm-2023.6.2.9.16.47/chatllm/aigc/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2023.6.2.9.16.47/chatllm/aigc/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2023.6.2.9.16.47/chatllm/aigc/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.813828 chatllm-2023.6.2.9.16.47/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2023.6.2.9.16.47/chatllm/api/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2023.6.2.9.16.47/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      586 2023-06-01 01:41:38.000000 chatllm-2023.6.2.9.16.47/chatllm/api/app.py
--rw-r--r--   0 betterme   (501) staff       (20)     1529 2023-05-31 03:52:51.000000 chatllm-2023.6.2.9.16.47/chatllm/api/config.py
--rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-05-31 00:47:03.000000 chatllm-2023.6.2.9.16.47/chatllm/api/datamodels.py
--rw-r--r--   0 betterme   (501) staff       (20)     1749 2023-05-31 00:30:21.000000 chatllm-2023.6.2.9.16.47/chatllm/api/openai_client.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.814683 chatllm-2023.6.2.9.16.47/chatllm/api/routes/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2023.6.2.9.16.47/chatllm/api/routes/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      557 2023-05-29 01:39:47.000000 chatllm-2023.6.2.9.16.47/chatllm/api/routes/api.py
--rw-r--r--   0 betterme   (501) staff       (20)     2200 2023-06-02 01:06:14.000000 chatllm-2023.6.2.9.16.47/chatllm/api/routes/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     4696 2023-06-02 01:03:20.000000 chatllm-2023.6.2.9.16.47/chatllm/api/routes/completions.py
--rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-05-26 07:01:26.000000 chatllm-2023.6.2.9.16.47/chatllm/api/routes/embeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     3471 2023-05-31 08:27:43.000000 chatllm-2023.6.2.9.16.47/chatllm/api/routes/responses.py
--rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2023.6.2.9.16.47/chatllm/api/sse_api.py
--rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2023.6.2.9.16.47/chatllm/api/test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.816616 chatllm-2023.6.2.9.16.47/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/__chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2414 2023-05-31 06:03:52.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chataudio.py
--rw-r--r--   0 betterme   (501) staff       (20)     2395 2023-05-31 09:20:39.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)      316 2023-05-04 03:46:23.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatmind.py
--rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2023.6.2.9.16.47/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 chatllm-2023.6.2.9.16.47/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.816985 chatllm-2023.6.2.9.16.47/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1281 2023-06-01 09:05:12.000000 chatllm-2023.6.2.9.16.47/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      779 2023-05-25 08:42:08.000000 chatllm-2023.6.2.9.16.47/chatllm/closeai.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 chatllm-2023.6.2.9.16.47/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.817513 chatllm-2023.6.2.9.16.47/chatllm/llms/
--rw-r--r--   0 betterme   (501) staff       (20)     1529 2023-06-02 01:07:49.000000 chatllm-2023.6.2.9.16.47/chatllm/llms/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2243 2023-06-02 01:09:41.000000 chatllm-2023.6.2.9.16.47/chatllm/llms/chatglm.py
--rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2023.6.2.9.16.47/chatllm/llms/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2023.6.2.9.16.47/chatllm/llms/llama.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.818319 chatllm-2023.6.2.9.16.47/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2023.6.2.9.16.47/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2023.6.2.9.16.47/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2336 2023-05-29 07:27:53.000000 chatllm-2023.6.2.9.16.47/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2023.6.2.9.16.47/chatllm/utils/gpu_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2023.6.2.9.16.47/chatllm/utils/nbce.py
--rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2023.6.2.9.16.47/chatllm/utils/nbce_test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.819315 chatllm-2023.6.2.9.16.47/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3102 2023-06-01 03:54:54.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-05-15 11:46:17.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2023.6.2.9.16.47/chatllm/webui/visualglm_st.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.811743 chatllm-2023.6.2.9.16.47/chatllm.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     6664 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     2640 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      334 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-06-02 01:16:47.000000 chatllm-2023.6.2.9.16.47/chatllm.egg-info/top_level.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.821978 chatllm-2023.6.2.9.16.47/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.824431 chatllm-2023.6.2.9.16.47/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 chatllm-2023.6.2.9.16.47/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 chatllm-2023.6.2.9.16.47/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)    80933 2023-05-31 01:13:52.000000 chatllm-2023.6.2.9.16.47/data/imgs/chatbox.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 chatllm-2023.6.2.9.16.47/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 chatllm-2023.6.2.9.16.47/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)   477462 2023-05-08 01:03:47.000000 chatllm-2023.6.2.9.16.47/data/imgs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)   333086 2023-05-08 01:03:52.000000 chatllm-2023.6.2.9.16.47/data/imgs/img_1.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 chatllm-2023.6.2.9.16.47/data/imgs/role.png
--rw-r--r--   0 betterme   (501) staff       (20)   443539 2023-05-26 00:55:04.000000 chatllm-2023.6.2.9.16.47/data/imgs/群.png
--rw-r--r--   0 betterme   (501) staff       (20)    31192 2023-05-29 00:57:03.000000 chatllm-2023.6.2.9.16.47/data/openai_keys.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.826919 chatllm-2023.6.2.9.16.47/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 chatllm-2023.6.2.9.16.47/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 chatllm-2023.6.2.9.16.47/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 chatllm-2023.6.2.9.16.47/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 chatllm-2023.6.2.9.16.47/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 chatllm-2023.6.2.9.16.47/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 chatllm-2023.6.2.9.16.47/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 chatllm-2023.6.2.9.16.47/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.830610 chatllm-2023.6.2.9.16.47/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      332 2023-05-31 10:28:33.000000 chatllm-2023.6.2.9.16.47/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       90 2023-05-26 09:35:58.000000 chatllm-2023.6.2.9.16.47/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2023.6.2.9.16.47/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2023.6.2.9.16.47/requirements_api.txt
--rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2023.6.2.9.16.47/requirements_openai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2023.6.2.9.16.47/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2023.6.2.9.16.47/requirements_streamlit.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-06-02 01:16:47.831558 chatllm-2023.6.2.9.16.47/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1700 2023-05-31 05:17:11.000000 chatllm-2023.6.2.9.16.47/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-02 01:16:47.831025 chatllm-2023.6.2.9.16.47/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2023.6.2.9.16.47/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 chatllm-2023.6.2.9.16.47/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.313887 chatllm-2023.6.26.13.31.16/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2023.6.26.13.31.16/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2023-05-31 08:06:48.000000 chatllm-2023.6.26.13.31.16/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     6666 2023-06-26 05:31:17.313709 chatllm-2023.6.26.13.31.16/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     5935 2023-05-31 01:20:56.000000 chatllm-2023.6.26.13.31.16/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2023.6.26.13.31.16/README.md.bak
+-rw-r--r--   0 betterme   (501) staff       (20)     1292 2023-06-12 04:10:57.000000 chatllm-2023.6.26.13.31.16/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.258370 chatllm-2023.6.26.13.31.16/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.260390 chatllm-2023.6.26.13.31.16/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 chatllm-2023.6.26.13.31.16/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 chatllm-2023.6.26.13.31.16/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 chatllm-2023.6.26.13.31.16/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 chatllm-2023.6.26.13.31.16/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.260774 chatllm-2023.6.26.13.31.16/chatllm/aigc/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2023.6.26.13.31.16/chatllm/aigc/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2023.6.26.13.31.16/chatllm/aigc/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.262685 chatllm-2023.6.26.13.31.16/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2023.6.26.13.31.16/chatllm/api/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2023.6.26.13.31.16/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      659 2023-06-02 12:12:32.000000 chatllm-2023.6.26.13.31.16/chatllm/api/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-06-02 12:16:56.000000 chatllm-2023.6.26.13.31.16/chatllm/api/config.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-05-31 00:47:03.000000 chatllm-2023.6.26.13.31.16/chatllm/api/datamodels.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1749 2023-05-31 00:30:21.000000 chatllm-2023.6.26.13.31.16/chatllm/api/openai_client.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.264034 chatllm-2023.6.26.13.31.16/chatllm/api/routes/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2023.6.26.13.31.16/chatllm/api/routes/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      557 2023-05-29 01:39:47.000000 chatllm-2023.6.26.13.31.16/chatllm/api/routes/api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2200 2023-06-02 01:06:14.000000 chatllm-2023.6.26.13.31.16/chatllm/api/routes/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4928 2023-06-04 07:21:05.000000 chatllm-2023.6.26.13.31.16/chatllm/api/routes/completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-06-04 06:52:41.000000 chatllm-2023.6.26.13.31.16/chatllm/api/routes/embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3422 2023-06-26 05:20:07.000000 chatllm-2023.6.26.13.31.16/chatllm/api/routes/responses.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2023.6.26.13.31.16/chatllm/api/sse_api.py
+-rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2023.6.26.13.31.16/chatllm/api/test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.268305 chatllm-2023.6.26.13.31.16/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/__chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2414 2023-05-31 06:03:52.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2417 2023-06-04 08:49:18.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)      316 2023-05-04 03:46:23.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2023.6.26.13.31.16/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 chatllm-2023.6.26.13.31.16/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.268971 chatllm-2023.6.26.13.31.16/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1087 2023-06-15 09:17:56.000000 chatllm-2023.6.26.13.31.16/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      779 2023-05-25 08:42:08.000000 chatllm-2023.6.26.13.31.16/chatllm/closeai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 chatllm-2023.6.26.13.31.16/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.269995 chatllm-2023.6.26.13.31.16/chatllm/llms/
+-rw-r--r--   0 betterme   (501) staff       (20)     1526 2023-06-02 12:11:10.000000 chatllm-2023.6.26.13.31.16/chatllm/llms/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2243 2023-06-02 01:09:41.000000 chatllm-2023.6.26.13.31.16/chatllm/llms/chatglm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2023.6.26.13.31.16/chatllm/llms/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2023.6.26.13.31.16/chatllm/llms/llama.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.270514 chatllm-2023.6.26.13.31.16/chatllm/prompts/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-06-12 03:51:17.000000 chatllm-2023.6.26.13.31.16/chatllm/prompts/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-06-20 08:01:27.000000 chatllm-2023.6.26.13.31.16/chatllm/prompts/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.271983 chatllm-2023.6.26.13.31.16/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2023.6.26.13.31.16/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2023.6.26.13.31.16/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-06-02 10:18:35.000000 chatllm-2023.6.26.13.31.16/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2023.6.26.13.31.16/chatllm/utils/gpu_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2023.6.26.13.31.16/chatllm/utils/nbce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2023.6.26.13.31.16/chatllm/utils/nbce_test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.273987 chatllm-2023.6.26.13.31.16/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2023.6.26.13.31.16/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2023.6.26.13.31.16/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3102 2023-06-01 03:54:54.000000 chatllm-2023.6.26.13.31.16/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      134 2023-06-26 02:13:58.000000 chatllm-2023.6.26.13.31.16/chatllm/webui/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2023.6.26.13.31.16/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2023.6.26.13.31.16/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 chatllm-2023.6.26.13.31.16/chatllm/webui/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2023.6.26.13.31.16/chatllm/webui/visualglm_st.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.259439 chatllm-2023.6.26.13.31.16/chatllm.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     6666 2023-06-26 05:31:17.000000 chatllm-2023.6.26.13.31.16/chatllm.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     2734 2023-06-26 05:31:17.000000 chatllm-2023.6.26.13.31.16/chatllm.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-26 05:31:17.000000 chatllm-2023.6.26.13.31.16/chatllm.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-06-26 05:31:17.000000 chatllm-2023.6.26.13.31.16/chatllm.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-26 05:31:17.000000 chatllm-2023.6.26.13.31.16/chatllm.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      348 2023-06-26 05:31:17.000000 chatllm-2023.6.26.13.31.16/chatllm.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-06-26 05:31:17.000000 chatllm-2023.6.26.13.31.16/chatllm.egg-info/top_level.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.279784 chatllm-2023.6.26.13.31.16/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.292255 chatllm-2023.6.26.13.31.16/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 chatllm-2023.6.26.13.31.16/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 chatllm-2023.6.26.13.31.16/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)    80933 2023-05-31 01:13:52.000000 chatllm-2023.6.26.13.31.16/data/imgs/chatbox.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 chatllm-2023.6.26.13.31.16/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 chatllm-2023.6.26.13.31.16/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)   477462 2023-05-08 01:03:47.000000 chatllm-2023.6.26.13.31.16/data/imgs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)   333086 2023-05-08 01:03:52.000000 chatllm-2023.6.26.13.31.16/data/imgs/img_1.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 chatllm-2023.6.26.13.31.16/data/imgs/role.png
+-rw-r--r--   0 betterme   (501) staff       (20)   484220 2023-06-06 10:32:35.000000 chatllm-2023.6.26.13.31.16/data/imgs/群.png
+-rw-r--r--   0 betterme   (501) staff       (20)    31192 2023-05-29 00:57:03.000000 chatllm-2023.6.26.13.31.16/data/openai_keys.md
+-rw-r--r--   0 betterme   (501) staff       (20)  1242960 2023-06-26 02:02:22.000000 chatllm-2023.6.26.13.31.16/data/中职职教高考政策解读.pdf
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.299724 chatllm-2023.6.26.13.31.16/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 chatllm-2023.6.26.13.31.16/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 chatllm-2023.6.26.13.31.16/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 chatllm-2023.6.26.13.31.16/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 chatllm-2023.6.26.13.31.16/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 chatllm-2023.6.26.13.31.16/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 chatllm-2023.6.26.13.31.16/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 chatllm-2023.6.26.13.31.16/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.311478 chatllm-2023.6.26.13.31.16/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      332 2023-06-06 10:33:00.000000 chatllm-2023.6.26.13.31.16/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       90 2023-05-26 09:35:58.000000 chatllm-2023.6.26.13.31.16/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2023.6.26.13.31.16/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2023.6.26.13.31.16/requirements_api.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2023.6.26.13.31.16/requirements_openai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2023.6.26.13.31.16/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2023.6.26.13.31.16/requirements_streamlit.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-06-26 05:31:17.313944 chatllm-2023.6.26.13.31.16/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1706 2023-06-20 06:25:34.000000 chatllm-2023.6.26.13.31.16/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-26 05:31:17.311987 chatllm-2023.6.26.13.31.16/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2023.6.26.13.31.16/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 chatllm-2023.6.26.13.31.16/tox.ini
```

### Comparing `chatllm-2023.6.2.9.16.47/.gitignore` & `chatllm-2023.6.26.13.31.16/.gitignore`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/.travis.yml` & `chatllm-2023.6.26.13.31.16/.travis.yml`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/LICENSE` & `chatllm-2023.6.26.13.31.16/LICENSE`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/Makefile` & `chatllm-2023.6.26.13.31.16/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/PKG-INFO` & `chatllm-2023.6.26.13.31.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2023.6.2.9.16.47
+Version: 2023.6.26.13.31.16
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatllm-2023.6.2.9.16.47/README.md` & `chatllm-2023.6.26.13.31.16/README.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/README.md.bak` & `chatllm-2023.6.26.13.31.16/README.md.bak`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/TODO.md` & `chatllm-2023.6.26.13.31.16/TODO.md`

 * *Files 22% similar despite different names*

```diff
@@ -12,23 +12,34 @@
 增加bloom
 https://github.com/huggingface/transformers-bloom-inference
 https://huggingface.co/bigscience/bloom-560m
 
 
 提示模板
 https://github.com/f/awesome-chatgpt-prompts
-
-
 https://github.com/TheRamU/Fay
 
 
 # 赚钱
 https://github.com/xiaoming2028/Chatgpt-Makes-Money
 
 #
 https://github.com/yuanzhoulvpi2017/zero_nlp
 
 # chatSQL
 https://huggingface.co/spaces/ls291/ChatSQL
 
 # 网盘
 https://github.com/sc0tfree/updog
+
+# 模型加速
+https://mp.weixin.qq.com/s/uV4Y_q4GnTUAsRVHxJGxGA
+
+# embedding: https://huggingface.co/spaces/mteb/leaderboard
+https://instructor-embedding.github.io/
+https://modelscope.cn/models/damo/nlp_corom_sentence-embedding_chinese-base/summary
+
+打榜
+https://aistudio.baidu.com/aistudio/competition/detail/45/0/leaderboard
+
+# 长篇小说
+https://www.jiqizhixin.com/articles/2023-05-28-3
```

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/_his/FaissANN.py` & `chatllm-2023.6.26.13.31.16/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/_his/_chatllm.py` & `chatllm-2023.6.26.13.31.16/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/_his/_qa.py` & `chatllm-2023.6.26.13.31.16/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/aigc/common.py` & `chatllm-2023.6.26.13.31.16/chatllm/aigc/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/api/app.py` & `chatllm-2023.6.26.13.31.16/chatllm/api/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 # @Software     : PyCharm
 # @Description  :
 
 from meutils.pipe import *
 
 # os.environ['LLM_MODEL'] = '/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm'
 os.environ['DEBUG'] = '1'
+os.environ['DB_URL'] = "mysql+pymysql://root:root123456@localhost/test"
 
 from meutils.serving.fastapi import App
 
 from chatllm.api.routes.api import router
 
 app = App()
 app.include_router(router)
 
 if __name__ == '__main__':
     app = App()
     app.include_router(router)
     app.run()
+
```

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/api/config.py` & `chatllm-2023.6.26.13.31.16/chatllm/api/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,30 +3,38 @@
 # @Project      : AI.  @by PyCharm
 # @File         : config
 # @Time         : 2023/5/26 13:08
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
+import pandas as pd
 
 from meutils.pipe import *
+from meutils.db import MySQL
 from meutils.decorators import clear_cuda_cache
 
 from chatllm.llms import load_llm4chat
 
 torch_gc = clear_cuda_cache(lambda: logger.info('Clear GPU'), bins=os.getenv('TIME_INTERVAL', 15))
 
 ######################配置#####################################
+debug = os.getenv('DEBUG')
+
 tokens = set(os.getenv('TOKENS', 'chatllm').split(','))
 llm_model = os.getenv('LLM_MODEL', '')
 embedding_model = os.getenv('EMBEDDING_MODEL')
 device = os.getenv('DEVICE', 'cpu')
 num_gpus = os.getenv('NUM_GPUS', 2)
 
 llm_role = os.getenv('LLM_ROLE', '')
+
+# 落库
+db_url = os.getenv('DB_URL', '')
+table_name = os.getenv('TABLE_NAME', 'llm')
 ###############################################################
 
 
 if embedding_model:
     from sentence_transformers import SentenceTransformer
 
     embedding_model = SentenceTransformer(embedding_model)
@@ -43,7 +51,23 @@
 _do_chat = load_llm4chat(model_name_or_path=llm_model, device=device, num_gpus=num_gpus)
 
 
 def do_chat(query, **kwargs):
     if llm_role:
         query = """{role}\n请回答以下问题\n{question}""".format(question=query, role=llm_role)  # 增加角色扮演
     return _do_chat(query, **kwargs)
+
+
+# 入库
+def do_db(df: pd.DataFrame, table_name: str):
+    try:
+        import emoji
+        df = df.astype(str)
+        df['choices'] = df['choices'].astype(str).map(emoji.demojize)  # todo: 更优雅的解决方案
+
+        if db_url:
+            db = MySQL(db_url)
+            db.create_table_or_upsert(df, table_name)
+            if debug:
+                logger.debug("Data written successfully 👍")
+    except Exception as e:
+        logger.error(f"Failed to write data ⚠️: {e}")
```

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/api/datamodels.py` & `chatllm-2023.6.26.13.31.16/chatllm/api/datamodels.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/api/openai_client.py` & `chatllm-2023.6.26.13.31.16/chatllm/api/openai_client.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/api/routes/api.py` & `chatllm-2023.6.26.13.31.16/chatllm/api/routes/api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/api/routes/base.py` & `chatllm-2023.6.26.13.31.16/chatllm/api/routes/base.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/api/routes/completions.py` & `chatllm-2023.6.26.13.31.16/chatllm/api/routes/completions.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from sse_starlette import EventSourceResponse
 
 # ME
 from meutils.pipe import *
 from chatllm.api.config import *
 from chatllm.api.datamodels import *
 from chatllm.api.routes.responses import *
+
 import json
 
 router = APIRouter()
 
 
 @router.post("/v1/chat/completions")
 async def chat_completions(body: ChatBody, request: Request, background_tasks: BackgroundTasks):
@@ -47,43 +48,51 @@
             history.append((message.content, "OK"))
         if message.role == 'user':
             user_question = message.content
         elif message.role == 'assistant':
             assistant_answer = message.content
             history.append((user_question, assistant_answer))
 
-    # if os.getenv('DEBUG'): logger.info(f"question: {question}, history: {history}")
-    if os.getenv('DEBUG'):  # 日志
-        logger.debug(await request.body())
-        logger.debug(body)
+    if debug:  # 日志
+        rprint('Request:', json.loads(await request.body()))
+        rprint('ChatBody:', body.dict())
 
     if body.stream:
         async def eval_llm():
             first = True
             response = ''  # 方便入库
             for _response in do_chat(question, history=history, **chat_kwargs):
+                response += _response
                 if first:
                     first = False
                     yield json.dumps(generate_stream_response_start(), ensure_ascii=False)
                 _ = generate_stream_response(_response)
                 yield json.dumps(_, ensure_ascii=False)
 
-                response += _response  # response += _['choices'][0].get('delta').get('content', '')
-
             yield json.dumps(generate_stream_response_stop(), ensure_ascii=False)
             yield "[DONE]"
-            if os.getenv('DEBUG'): logger.success(generate_response(response))  # 日志：todo 写入数据库
+
+            content = generate_response(response)
+            content['user'] = body.user
+            rprint(content)
+            background_tasks.add_task(do_db, pd.DataFrame([content]), 'chatcmpl')
+
+            if debug: logger.success(content)  # 日志
 
         return EventSourceResponse(eval_llm(), ping=10000)
     else:
         response = ''.join(do_chat(question, history=history, **chat_kwargs))
 
-        if os.getenv('DEBUG'): logger.success(generate_response(response))  # 日志
+        content = generate_response(response)
+        content['user'] = body.user
+        background_tasks.add_task(do_db, pd.DataFrame([content]), 'chatcmpl')
+
+        if debug: logger.success(content)  # 日志
 
-        return JSONResponse(content=generate_response(response))
+        return JSONResponse(content)
 
 
 @router.post("/v1/completions")
 async def completions(body: CompletionBody, request: Request, background_tasks: BackgroundTasks):
     background_tasks.add_task(torch_gc)
 
     if request.headers.get("Authorization").split(" ")[1] not in tokens:
@@ -91,32 +100,39 @@
 
     # if not llm_model: # 空模型
     #     raise HTTPException(status.HTTP_404_NOT_FOUND, "LLM model not found!")
 
     question = body.prompt
     chat_kwargs = {"temperature": body.temperature, "top_p": body.top_p, "max_tokens": body.max_tokens}
 
-    # if os.getenv('DEBUG'): logger.info(f"question: {question}")  # 日志
-    if os.getenv('DEBUG'):  # 日志
-        logger.debug(await request.body())
-        logger.debug(body)
+    if debug:  # 日志
+        rprint('Request:', json.loads(await request.body()))
+        rprint('ChatBody:', body.dict())
 
     if body.stream:
         async def eval_llm():
             response = ''  # 方便入库
             for _response in do_chat(question, **chat_kwargs):
+                response += _response
                 _ = generate_stream_response(_response, chat=False)
                 yield json.dumps(_, ensure_ascii=False)
 
-                response += _response  # response += _['choices'][0].get('text', '')
-
             yield json.dumps(generate_stream_response_stop(chat=False), ensure_ascii=False)
             yield "[DONE]"
-            if os.getenv('DEBUG'): logger.success(generate_response(response, chat=False))  # 日志
+
+            content = generate_response(response, chat=False)
+            content['user'] = body.user
+            background_tasks.add_task(do_db, pd.DataFrame([content]), 'cmpl')
+
+            if debug: logger.success(content)  # 日志
 
         return EventSourceResponse(eval_llm(), ping=10000)
     else:
         response = ''.join(do_chat(question, **chat_kwargs))  # 流式合成
 
-        if os.getenv('DEBUG'): logger.success(generate_response(response, chat=False))  # 日志
+        content = generate_response(response, chat=False)
+        content['user'] = body.user
+        background_tasks.add_task(do_db, pd.DataFrame([content]), 'cmpl')
+
+        if debug: logger.success(content)  # 日志
 
-        return JSONResponse(content=generate_response(response, chat=False))
+        return JSONResponse(content)
```

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/api/routes/embeddings.py` & `chatllm-2023.6.26.13.31.16/chatllm/api/routes/embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,26 @@
 from chatllm.api.datamodels import *
 
 router = APIRouter()
 
 
 def do_embeddings(body: EmbeddingsBody, request: Request, background_tasks: BackgroundTasks):
     background_tasks.add_task(torch_gc)
+
     if request.headers.get("Authorization").split(" ")[1] not in tokens:
         raise HTTPException(status.HTTP_401_UNAUTHORIZED, "Token is wrong!")
 
     if not embeddings_model:
         raise HTTPException(status.HTTP_404_NOT_FOUND, "Embeddings model not found!")
 
     texts = body.input
     if isinstance(texts, str):
         texts = [texts]
 
-    embeddings = embeddings_model.encode(texts)
+    embeddings = embedding_model.encode(texts)
 
     data = []
     for i, embed in enumerate(embeddings):
         data.append({
             "object": "embedding",
             "index": i,
             "embedding": embed.tolist(),
```

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/api/sse_api.py` & `chatllm-2023.6.26.13.31.16/chatllm/api/sse_api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/api/test.py` & `chatllm-2023.6.26.13.31.16/chatllm/api/test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/applications/Question2Answer.py` & `chatllm-2023.6.26.13.31.16/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/applications/__chatbase.py` & `chatllm-2023.6.26.13.31.16/chatllm/applications/__chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/applications/chatann.py` & `chatllm-2023.6.26.13.31.16/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/applications/chatbase.py` & `chatllm-2023.6.26.13.31.16/chatllm/applications/chatbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     @clear_cuda_cache(bins=int(os.getenv('GPU_TIME_INTERVAL', 2)))
     def _qa(self, query, knowledge_base='', role='', max_turns=1, return_history=False):
         self.role = role or os.getenv('LLM_ROLE', '')
         self.knowledge_base = str(knowledge_base).strip()
         if self.knowledge_base:
             self.query = self.prompt_template.format(context=self.knowledge_base, question=query, role='')
         else:
-            self.query = """{role}\n请回答以下问题\n{question}""".format(question=query, role=self.role)  # 知识库为空则转通用回答
+            self.query = """{role}\n基于以上角色，请回答以下问题：{question}""".format(question=query, role=self.role)  # 知识库为空则转通用回答
 
         global history
         _history = history[-(max_turns - 1):] if max_turns > 1 else []  # 截取最大轮次
         for _ in self.do_chat(query=self.query.strip(), history=_history, return_history=return_history):
             yield _  # (response, history)
 
     def load_llm(self, model_name_or_path="THUDM/chatglm-6b", device=DEVICE, return_history=False, **kwargs):
```

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/applications/chatcrawler.py` & `chatllm-2023.6.26.13.31.16/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/applications/chatpdf.py` & `chatllm-2023.6.26.13.31.16/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/applications/chatwhoosh.py` & `chatllm-2023.6.26.13.31.16/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/chatyuan.py` & `chatllm-2023.6.26.13.31.16/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/clis/cli.py` & `chatllm-2023.6.26.13.31.16/chatllm/clis/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,22 +9,14 @@
 # @Description  :
 import os
 
 from meutils.pipe import *
 
 cli = typer.Typer(name="ChatLLM CLI")
 
-if LOCAL_HOST.startswith('10.219'):
-    MODEL_PATH = "/CHAT_MODEL/chatglm-6b"
-
-
-@cli.command(help="help")  # help会覆盖docstring
-def clitest(**kwargs):  # 不支持 **kwargs
-    f(**kwargs)
-
 
 @cli.command()  # help会覆盖docstring
 def webui(name: str = 'chatpdf', port=8501):
     """
         chatllm-run webui --name chatpdf --port 8501
     """
     main = get_resolve_path(f'../webui/{name}.py', __file__)
```

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/closeai.py` & `chatllm-2023.6.26.13.31.16/chatllm/closeai.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/embedding.py` & `chatllm-2023.6.26.13.31.16/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/llms/__init__.py` & `chatllm-2023.6.26.13.31.16/chatllm/llms/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     if not model_base:  # 模型基座
         model_base = Path(model_name_or_path).name.lower()
         for p in Path(__file__).parent.glob('*.py'):
             if p.stem in model_base:
                 # logger.warning(p) # 自动推断模型基座
                 model_base = p.stem
 
-    logger.success(f"MODEL_BASE: {model_base}")  # 打印模型基座
+    logger.info(f"MODEL_BASE: {model_base}")  # 打印模型基座
 
     try:
         model_base = importlib.import_module(f"chatllm.llms.{model_base}")
         do_chat = model_base.load_llm4chat(
             model_name_or_path=model_name_or_path,
             device=device,
             num_gpus=num_gpus,
@@ -32,15 +32,15 @@
         return do_chat
 
     except Exception as e:
         logger.error(f"Unsupported model base: 测试环境可测试，生产环境请配置 LLM_MODEL ⚠️\n{e}")
 
         def do_chat(query, **kwargs):  # DEV
             for i in f"🔥🔥🔥\n\n生产环境请配置 LLM_MODEL ⚠️\n\n🔥🔥🔥\n":
-                time.sleep(0.5)
+                time.sleep(0.2)
                 yield i
 
         return do_chat
 
 
 if __name__ == '__main__':
     print(load_llm4chat('/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm-'))
```

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/llms/chatglm.py` & `chatllm-2023.6.26.13.31.16/chatllm/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/llms/demo.py` & `chatllm-2023.6.26.13.31.16/chatllm/llms/demo.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/llms/llama.py` & `chatllm-2023.6.26.13.31.16/chatllm/llms/llama.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/utils/common.py` & `chatllm-2023.6.26.13.31.16/chatllm/utils/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,14 @@
 DEVICE = (
     os.getenv('DEVICE') if 'DEVICE' in os.environ
     else "cuda" if torch.cuda.is_available()
     else "mps" if torch.backends.mps.is_available()
     else "cpu"
 )
 
-if LOCAL_HOST.startswith('10.219'):
-    MODEL_PATH = "/CHAT_MODEL/chatglm-6b"
-else:
-    MODEL_PATH = "THUDM/chatglm-6b"
-
 xgroup = Pipe(lambda ls, step=3, overlap_rate=0: [ls[max(idx - int(step * overlap_rate), 0): idx + step] for idx in
                                                   range(0, len(ls), step)])
 
 
 def textsplitter(text, chunk_size=512, overlap_rate=0.2, sep=''):  # 简单粗暴
     return text.lower().split() | xjoin(sep) | xgroup(chunk_size, overlap_rate)
```

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/utils/gpu_utils.py` & `chatllm-2023.6.26.13.31.16/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/utils/nbce.py` & `chatllm-2023.6.26.13.31.16/chatllm/utils/nbce.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/utils/nbce_test.py` & `chatllm-2023.6.26.13.31.16/chatllm/utils/nbce_test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/webui/chatbase.py` & `chatllm-2023.6.26.13.31.16/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/webui/chatpdf.py` & `chatllm-2023.6.26.13.31.16/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/webui/gradio_ui.py` & `chatllm-2023.6.26.13.31.16/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/webui/nice_ui.py` & `chatllm-2023.6.26.13.31.16/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm/webui/visualglm_st.py` & `chatllm-2023.6.26.13.31.16/chatllm/webui/visualglm_st.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/chatllm.egg-info/PKG-INFO` & `chatllm-2023.6.26.13.31.16/chatllm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2023.6.2.9.16.47
+Version: 2023.6.26.13.31.16
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatllm-2023.6.2.9.16.47/chatllm.egg-info/SOURCES.txt` & `chatllm-2023.6.26.13.31.16/chatllm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 chatllm/clis/README.md
 chatllm/clis/__init__.py
 chatllm/clis/cli.py
 chatllm/llms/__init__.py
 chatllm/llms/chatglm.py
 chatllm/llms/demo.py
 chatllm/llms/llama.py
+chatllm/prompts/__init__.py
+chatllm/prompts/common.py
 chatllm/utils/__init__.py
 chatllm/utils/_textsplitter.py
 chatllm/utils/common.py
 chatllm/utils/gpu_utils.py
 chatllm/utils/nbce.py
 chatllm/utils/nbce_test.py
 chatllm/webui/__init__.py
@@ -80,14 +82,15 @@
 chatllm/webui/chatpdf.py
 chatllm/webui/conf.yaml
 chatllm/webui/gradio_ui.py
 chatllm/webui/nice_ui.py
 chatllm/webui/run.sh
 chatllm/webui/visualglm_st.py
 data/openai_keys.md
+data/中职职教高考政策解读.pdf
 data/姚明.txt
 data/王治郅.txt
 data/科比.txt
 data/财报.pdf
 data/马保国.txt
 data/imgs/LLM.drawio.png
 data/imgs/LLM.png
```

### Comparing `chatllm-2023.6.2.9.16.47/data/imgs/LLM.drawio.png` & `chatllm-2023.6.26.13.31.16/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/imgs/LLM.png` & `chatllm-2023.6.26.13.31.16/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/imgs/chatbox.png` & `chatllm-2023.6.26.13.31.16/data/imgs/chatbox.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/imgs/chatpdf.gif` & `chatllm-2023.6.26.13.31.16/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/imgs/chatpdf_ann_df.png` & `chatllm-2023.6.26.13.31.16/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/imgs/img.png` & `chatllm-2023.6.26.13.31.16/data/imgs/img.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/imgs/img_1.png` & `chatllm-2023.6.26.13.31.16/data/imgs/img_1.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/imgs/role.png` & `chatllm-2023.6.26.13.31.16/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/openai_keys.md` & `chatllm-2023.6.26.13.31.16/data/openai_keys.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/医/500种中药现代研究.txt` & `chatllm-2023.6.26.13.31.16/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/医/古今医统大全.txt` & `chatllm-2023.6.26.13.31.16/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/姚明.txt` & `chatllm-2023.6.26.13.31.16/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/王治郅.txt` & `chatllm-2023.6.26.13.31.16/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/科比.txt` & `chatllm-2023.6.26.13.31.16/data/科比.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/data/财报.pdf` & `chatllm-2023.6.26.13.31.16/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/docs/Makefile` & `chatllm-2023.6.26.13.31.16/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/docs/conf.py` & `chatllm-2023.6.26.13.31.16/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/docs/make.bat` & `chatllm-2023.6.26.13.31.16/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/setup.py` & `chatllm-2023.6.26.13.31.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     extras_require=extras_require,  # pip install -U meutils\[all\]
     license="MIT license",
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords='chatllm',
     name='chatllm',
-    # name='llms', # 抢占包
+    # name='llm-openai', # 抢占包
 
     packages=find_packages(include=['chatllm', 'chatllm.*']),
 
     test_suite='tests',
     url='https://github.com/yuanjie-ai/ChatLLM',
     version=version,  # '0.0.0',
     zip_safe=False,
```

### Comparing `chatllm-2023.6.2.9.16.47/tests/test_llm4gpt.py` & `chatllm-2023.6.26.13.31.16/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.2.9.16.47/tests/内存型.ipynb` & `chatllm-2023.6.26.13.31.16/tests/内存型.ipynb`

 * *Files identical despite different names*


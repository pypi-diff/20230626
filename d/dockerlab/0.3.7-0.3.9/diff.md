# Comparing `tmp/dockerlab-0.3.7.tar.gz` & `tmp/dockerlab-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockerlab-0.3.7.tar", max compression
+gzip compressed data, was "dockerlab-0.3.9.tar", max compression
```

## Comparing `dockerlab-0.3.7.tar` & `dockerlab-0.3.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1073 2023-03-08 09:00:58.887390 dockerlab-0.3.7/LICENSE
--rw-r--r--   0        0        0     4831 2023-04-11 06:49:49.518450 dockerlab-0.3.7/README.md
--rw-r--r--   0        0        0       35 2023-06-23 02:10:29.294390 dockerlab-0.3.7/dockerlab/__init__.py
--rw-r--r--   0        0        0     1226 2023-03-22 12:19:12.078158 dockerlab-0.3.7/dockerlab/asset.py
--rw-r--r--   0        0        0       43 2023-03-15 13:02:22.919974 dockerlab-0.3.7/dockerlab/assets/.gitignore
--rw-r--r--   0        0        0     1534 2023-04-15 12:34:28.706070 dockerlab-0.3.7/dockerlab/assets/docker-compose.yml
--rw-r--r--   0        0        0     6386 2023-06-23 01:50:53.760930 dockerlab-0.3.7/dockerlab/assets/docker.py
--rwxr-xr-x   0        0        0     1608 2023-03-22 08:50:55.864206 dockerlab-0.3.7/dockerlab/assets/misc/init_workspace
--rw-r--r--   0        0        0     1872 2023-03-22 11:41:34.374529 dockerlab-0.3.7/dockerlab/assets/requirements.txt
--rw-r--r--   0        0        0     5619 2023-04-11 06:45:22.077237 dockerlab-0.3.7/dockerlab/cli.py
--rw-r--r--   0        0        0     1198 2023-04-15 12:32:08.444974 dockerlab-0.3.7/dockerlab/post_templates/default.txt
--rw-r--r--   0        0        0      318 2023-03-21 10:22:18.340920 dockerlab-0.3.7/dockerlab/post_templates/node.txt
--rw-r--r--   0        0        0     1500 2023-03-22 07:53:54.516620 dockerlab-0.3.7/dockerlab/post_templates/python.txt
--rw-r--r--   0        0        0     3201 2023-04-15 11:22:30.799781 dockerlab-0.3.7/dockerlab/template.py
--rw-r--r--   0        0        0     3876 2023-06-23 01:55:35.435053 dockerlab-0.3.7/dockerlab/templates/README.md
--rw-r--r--   0        0        0      204 2023-04-15 11:46:28.517882 dockerlab-0.3.7/dockerlab/templates/runtime_node_lts/Dockerfile
--rw-r--r--   0        0        0     1780 2023-06-23 01:54:23.053192 dockerlab-0.3.7/dockerlab/templates/settting.py
--rw-r--r--   0        0        0     4544 2023-03-22 07:50:22.159814 dockerlab-0.3.7/dockerlab/templates/workspace_base/Dockerfile
--rw-r--r--   0        0        0     4577 2023-03-20 12:51:22.275231 dockerlab-0.3.7/dockerlab/templates/workspace_cuda_11_1/Dockerfile
--rw-r--r--   0        0        0     4468 2023-06-23 01:54:00.258144 dockerlab-0.3.7/dockerlab/templates/workspace_cuda_11_3/Dockerfile
--rw-r--r--   0        0        0     4468 2023-03-20 12:51:22.268004 dockerlab-0.3.7/dockerlab/templates/workspace_cuda_11_7/Dockerfile
--rw-r--r--   0        0        0     4571 2023-03-21 12:01:20.782551 dockerlab-0.3.7/dockerlab/templates/workspace_protein/Dockerfile
--rw-r--r--   0        0        0      493 2023-03-20 14:19:33.075541 dockerlab-0.3.7/dockerlab/templates/workspace_pytorch_1_13/Dockerfile
--rw-r--r--   0        0        0      488 2023-03-20 14:19:33.075321 dockerlab-0.3.7/dockerlab/templates/workspace_pytorch_2_0/Dockerfile
--rw-r--r--   0        0        0     2294 2023-03-22 12:19:37.232253 dockerlab-0.3.7/dockerlab/utils.py
--rw-r--r--   0        0        0      593 2023-06-23 02:10:29.293458 dockerlab-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     5510 1970-01-01 00:00:00.000000 dockerlab-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-08 09:00:58.887390 dockerlab-0.3.9/LICENSE
+-rw-r--r--   0        0        0     4831 2023-04-11 06:49:49.518450 dockerlab-0.3.9/README.md
+-rw-r--r--   0        0        0       35 2023-06-26 16:44:28.016371 dockerlab-0.3.9/dockerlab/__init__.py
+-rw-r--r--   0        0        0     1226 2023-03-22 12:19:12.078158 dockerlab-0.3.9/dockerlab/asset.py
+-rw-r--r--   0        0        0       43 2023-03-15 13:02:22.919974 dockerlab-0.3.9/dockerlab/assets/.gitignore
+-rw-r--r--   0        0        0     1534 2023-04-15 12:34:28.706070 dockerlab-0.3.9/dockerlab/assets/docker-compose.yml
+-rw-r--r--   0        0        0     6431 2023-06-24 06:02:35.493860 dockerlab-0.3.9/dockerlab/assets/docker.py
+-rwxr-xr-x   0        0        0     1608 2023-03-22 08:50:55.864206 dockerlab-0.3.9/dockerlab/assets/misc/init_workspace
+-rw-r--r--   0        0        0     1872 2023-03-22 11:41:34.374529 dockerlab-0.3.9/dockerlab/assets/requirements.txt
+-rw-r--r--   0        0        0     5619 2023-04-11 06:45:22.077237 dockerlab-0.3.9/dockerlab/cli.py
+-rw-r--r--   0        0        0     1198 2023-04-15 12:32:08.444974 dockerlab-0.3.9/dockerlab/post_templates/default.txt
+-rw-r--r--   0        0        0      318 2023-03-21 10:22:18.340920 dockerlab-0.3.9/dockerlab/post_templates/node.txt
+-rw-r--r--   0        0        0     1500 2023-03-22 07:53:54.516620 dockerlab-0.3.9/dockerlab/post_templates/python.txt
+-rw-r--r--   0        0        0     3201 2023-04-15 11:22:30.799781 dockerlab-0.3.9/dockerlab/template.py
+-rw-r--r--   0        0        0     3876 2023-06-23 01:55:35.435053 dockerlab-0.3.9/dockerlab/templates/README.md
+-rw-r--r--   0        0        0      204 2023-06-26 16:33:22.218435 dockerlab-0.3.9/dockerlab/templates/runtime_node_lts/Dockerfile
+-rw-r--r--   0        0        0     1780 2023-06-23 01:54:23.053192 dockerlab-0.3.9/dockerlab/templates/settting.py
+-rw-r--r--   0        0        0     4574 2023-06-26 16:33:13.811603 dockerlab-0.3.9/dockerlab/templates/workspace_base/Dockerfile
+-rw-r--r--   0        0        0     4607 2023-06-26 16:32:18.428249 dockerlab-0.3.9/dockerlab/templates/workspace_cuda_11_1/Dockerfile
+-rw-r--r--   0        0        0     4498 2023-06-26 16:32:35.727361 dockerlab-0.3.9/dockerlab/templates/workspace_cuda_11_3/Dockerfile
+-rw-r--r--   0        0        0     4498 2023-06-26 16:32:44.119973 dockerlab-0.3.9/dockerlab/templates/workspace_cuda_11_7/Dockerfile
+-rw-r--r--   0        0        0     4571 2023-06-24 17:08:24.572496 dockerlab-0.3.9/dockerlab/templates/workspace_protein/Dockerfile
+-rw-r--r--   0        0        0      493 2023-03-20 14:19:33.075541 dockerlab-0.3.9/dockerlab/templates/workspace_pytorch_1_13/Dockerfile
+-rw-r--r--   0        0        0      488 2023-03-20 14:19:33.075321 dockerlab-0.3.9/dockerlab/templates/workspace_pytorch_2_0/Dockerfile
+-rw-r--r--   0        0        0     2294 2023-03-22 12:19:37.232253 dockerlab-0.3.9/dockerlab/utils.py
+-rw-r--r--   0        0        0      593 2023-06-26 16:44:28.015231 dockerlab-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     5510 1970-01-01 00:00:00.000000 dockerlab-0.3.9/PKG-INFO
```

### Comparing `dockerlab-0.3.7/LICENSE` & `dockerlab-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/README.md` & `dockerlab-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/dockerlab/asset.py` & `dockerlab-0.3.9/dockerlab/asset.py`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/dockerlab/assets/docker-compose.yml` & `dockerlab-0.3.9/dockerlab/assets/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/dockerlab/assets/docker.py` & `dockerlab-0.3.9/dockerlab/assets/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
     elif args.action == "enter":
         if args.root:
             command = f"docker-compose exec -u root {args.service} {SHELL}"
         else:
             command = f"docker-compose exec {args.service} {SHELL}"
     else:
         command = f"docker-compose {args.action}"
+    command = "DOCKER_BUILDKIT=1 " + command
     print(f"> {command}\n")
     execute(command)
 
 
 def _set_env(env_path=DEFAULT_ENV_PATH, verbose=False):
     e = Env(env_path)
     e["UID"] = os.getuid()
```

### Comparing `dockerlab-0.3.7/dockerlab/assets/misc/init_workspace` & `dockerlab-0.3.9/dockerlab/assets/misc/init_workspace`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/dockerlab/assets/requirements.txt` & `dockerlab-0.3.9/dockerlab/assets/requirements.txt`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/dockerlab/cli.py` & `dockerlab-0.3.9/dockerlab/cli.py`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/dockerlab/post_templates/default.txt` & `dockerlab-0.3.9/dockerlab/post_templates/default.txt`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/dockerlab/post_templates/python.txt` & `dockerlab-0.3.9/dockerlab/post_templates/python.txt`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/dockerlab/template.py` & `dockerlab-0.3.9/dockerlab/template.py`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/dockerlab/templates/README.md` & `dockerlab-0.3.9/dockerlab/templates/README.md`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/dockerlab/templates/settting.py` & `dockerlab-0.3.9/dockerlab/templates/settting.py`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/dockerlab/templates/workspace_base/Dockerfile` & `dockerlab-0.3.9/dockerlab/templates/workspace_base/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     && wget -O tmux-2.8.tar.gz https://github.com/tmux/tmux/archive/2.8.tar.gz \
     && tar zxvf tmux-2.8.tar.gz \
     && cd tmux-2.8 \
     && ./autogen.sh \
     && ./configure --prefix=/usr/local \
     && make \
     && make install \
+    && rm -rf /tmp/tmux-2.8 \
     && rm -rf /var/lib/apt/lists/*
 
 # Tmux configuration
 RUN git clone https://github.com/hughplay/tmux-config.git /tmp/tmux-config \
     && bash /tmp/tmux-config/install.sh \
     && rm -rf /tmp/tmux-config \
     && echo "set -g default-shell `which zsh`" >> ~/.tmux.conf
```

### Comparing `dockerlab-0.3.7/dockerlab/templates/workspace_cuda_11_1/Dockerfile` & `dockerlab-0.3.9/dockerlab/templates/workspace_cuda_11_1/Dockerfile`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     && wget -O tmux-2.8.tar.gz https://github.com/tmux/tmux/archive/2.8.tar.gz \
     && tar zxvf tmux-2.8.tar.gz \
     && cd tmux-2.8 \
     && ./autogen.sh \
     && ./configure --prefix=/usr/local \
     && make \
     && make install \
+    && rm -rf /tmp/tmux-2.8 \
     && rm -rf /var/lib/apt/lists/*
 
 # Tmux configuration
 RUN git clone https://github.com/hughplay/tmux-config.git /tmp/tmux-config \
     && bash /tmp/tmux-config/install.sh \
     && rm -rf /tmp/tmux-config \
     && echo "set -g default-shell `which zsh`" >> ~/.tmux.conf
```

### Comparing `dockerlab-0.3.7/dockerlab/templates/workspace_cuda_11_3/Dockerfile` & `dockerlab-0.3.9/dockerlab/templates/workspace_cuda_11_3/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     && wget -O tmux-2.8.tar.gz https://github.com/tmux/tmux/archive/2.8.tar.gz \
     && tar zxvf tmux-2.8.tar.gz \
     && cd tmux-2.8 \
     && ./autogen.sh \
     && ./configure --prefix=/usr/local \
     && make \
     && make install \
+    && rm -rf /tmp/tmux-2.8 \
     && rm -rf /var/lib/apt/lists/*
 
 # Tmux configuration
 RUN git clone https://github.com/hughplay/tmux-config.git /tmp/tmux-config \
     && bash /tmp/tmux-config/install.sh \
     && rm -rf /tmp/tmux-config \
     && echo "set -g default-shell `which zsh`" >> ~/.tmux.conf
```

### Comparing `dockerlab-0.3.7/dockerlab/templates/workspace_cuda_11_7/Dockerfile` & `dockerlab-0.3.9/dockerlab/templates/workspace_cuda_11_7/Dockerfile`

 * *Files 3% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     && wget -O tmux-2.8.tar.gz https://github.com/tmux/tmux/archive/2.8.tar.gz \
     && tar zxvf tmux-2.8.tar.gz \
     && cd tmux-2.8 \
     && ./autogen.sh \
     && ./configure --prefix=/usr/local \
     && make \
     && make install \
+    && rm -rf /tmp/tmux-2.8 \
     && rm -rf /var/lib/apt/lists/*
 
 # Tmux configuration
 RUN git clone https://github.com/hughplay/tmux-config.git /tmp/tmux-config \
     && bash /tmp/tmux-config/install.sh \
     && rm -rf /tmp/tmux-config \
     && echo "set -g default-shell `which zsh`" >> ~/.tmux.conf
```

### Comparing `dockerlab-0.3.7/dockerlab/templates/workspace_protein/Dockerfile` & `dockerlab-0.3.9/dockerlab/templates/workspace_protein/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     && make \
     && make install \
     && rm -rf /tmp/hmmer
 
 # Install BLAST
 RUN mkdir /tmp/blast \
     && cd /tmp/blast \
-    &&  wget -O ncbi-blast-2.13.0+-x64-linux.tar.gz https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/LATEST/ncbi-blast-2.13.0+-x64-linux.tar.gz \
+    &&  wget -O ncbi-blast-2.13.0+-x64-linux.tar.gz https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/2.13.0/ncbi-blast-2.13.0+-x64-linux.tar.gz \
     && tar zxvf ncbi-blast-2.13.0+-x64-linux.tar.gz \
     && cp ncbi-blast-2.13.0+/bin/* /usr/local/bin/ \
     && rm -rf /tmp/blast
 
 # Install TM-align
 RUN mkdir /tmp/align \
     && cd /tmp/align \
```

### Comparing `dockerlab-0.3.7/dockerlab/utils.py` & `dockerlab-0.3.9/dockerlab/utils.py`

 * *Files identical despite different names*

### Comparing `dockerlab-0.3.7/pyproject.toml` & `dockerlab-0.3.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dockerlab"
-version = "0.3.7"
+version = "0.3.9"
 description = "Build a docker container as your workspace."
 homepage = "https://github.com/hughplay/dockerlab"
 authors = ["Mr.Blue <silverhugh.77@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `dockerlab-0.3.7/PKG-INFO` & `dockerlab-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockerlab
-Version: 0.3.7
+Version: 0.3.9
 Summary: Build a docker container as your workspace.
 Home-page: https://github.com/hughplay/dockerlab
 License: MIT
 Author: Mr.Blue
 Author-email: silverhugh.77@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


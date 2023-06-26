# Comparing `tmp/gitlab-runner-tart-driver-0.1.5.tar.gz` & `tmp/gitlab-runner-tart-driver-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-runner-tart-driver-0.1.5.tar", last modified: Tue Jun 20 14:35:08 2023, max compression
+gzip compressed data, was "gitlab-runner-tart-driver-0.1.6.tar", last modified: Sun Jun 25 18:26:11 2023, max compression
```

## Comparing `gitlab-runner-tart-driver-0.1.5.tar` & `gitlab-runner-tart-driver-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:35:08.922506 gitlab-runner-tart-driver-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)     3303 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    18383 2023-06-20 14:35:08.921506 gitlab-runner-tart-driver-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    17862 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:35:08.918506 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:35:08.920506 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/config.py
--rw-rw-rw-   0 root         (0) root         (0)    10206 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     2145 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:35:08.921506 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1061 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8703 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/tart.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:35:08.921506 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2533 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:35:08.919506 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18383 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1060 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 14:35:08.922506 gitlab-runner-tart-driver-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 18:26:11.548257 gitlab-runner-tart-driver-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    18448 2023-06-25 18:26:11.548257 gitlab-runner-tart-driver-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    17927 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 18:26:11.545257 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 18:26:11.547257 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1617 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/commands/cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/commands/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11270 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/commands/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/commands/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 18:26:11.547257 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8703 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/modules/tart.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/modules/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 18:26:11.547257 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2533 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 18:26:11.546257 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18448 2023-06-25 18:26:11.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-06-25 18:26:11.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 18:26:11.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-25 18:26:11.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 18:26:11.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-25 18:26:11.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-25 18:26:11.000000 gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 18:26:11.548257 gitlab-runner-tart-driver-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-06-25 18:26:04.000000 gitlab-runner-tart-driver-0.1.6/setup.py
```

### Comparing `gitlab-runner-tart-driver-0.1.5/LICENSE.txt` & `gitlab-runner-tart-driver-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.5/PKG-INFO` & `gitlab-runner-tart-driver-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
@@ -432,14 +432,15 @@
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
   Run commands.
 
 Options:
   --default-ssh-username TEXT  username to login to a tart vm
   --default-ssh-password TEXT  password to login to a tart vm
+  --timeout INTEGER            SSH connection timeout in seconds
   -x, --tart-executable TEXT   Path to the tart executable.
   --shell TEXT                 Path to the shell to be used for commands over
                                ssh.
   --help                       Show this message and exit.
 ```
 
 ### Command `cleanup`
```

### Comparing `gitlab-runner-tart-driver-0.1.5/README.md` & `gitlab-runner-tart-driver-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -417,14 +417,15 @@
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
   Run commands.
 
 Options:
   --default-ssh-username TEXT  username to login to a tart vm
   --default-ssh-password TEXT  password to login to a tart vm
+  --timeout INTEGER            SSH connection timeout in seconds
   -x, --tart-executable TEXT   Path to the tart executable.
   --shell TEXT                 Path to the shell to be used for commands over
                                ssh.
   --help                       Show this message and exit.
 ```
 
 ### Command `cleanup`
```

### Comparing `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/cli.py` & `gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/cli.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/config.py` & `gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/commands/config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/prepare.py` & `gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/commands/prepare.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,16 +190,30 @@
     if tart_vm_name in tart_vm_map:
         if tart_vm_map[tart_vm_name].running:
             click.echo(f"[INFO] Found running VM '{tart_vm_name}'. Going to stop it...")
             tart.stop(tart_vm_name)
         click.echo(f"[INFO] Found VM '{tart_vm_name}'. Going to delete it...")
         tart.delete(tart_vm_name)
 
+    # verfiy that the limit of running VMs is not exceeded
+    list_running_vms = []
+    for vm in tart.list():
+        if vm.running:
+            list_running_vms.append(vm)
+
+    if len(list_running_vms) >= p.tart_max_vm_count:
+        click.secho("[ERROR] The limit of running VMs is exceeded.", fg="red")
+        sys.exit(1)
+
     click.echo(f"[INFO] Cloning VM instance '{tart_vm_name}' from '{p.ci_job_image}'")
-    tart.clone(p.ci_job_image, tart_vm_name)
+    try:
+        tart.clone(p.ci_job_image, tart_vm_name)
+    except:
+        click.secho(f"[ERROR] failed to clone image f'{p.ci_job_image}'", fg="red")
+        sys.exit(1)
 
     if cpu or memory or display:
         click.echo(f"[INFO] Configuring instance '{tart_vm_name}' from '{p.ci_job_image}'")
         click.echo(
             f"[INFO] {tart_vm_name} [cpu={cpu if cpu else 'default'}, memory={memory if memory else 'default'}, display={display if display else 'default'}]"
         )
         tart.set(tart_vm_name, cpu=cpu, memory=memory, display=display)
@@ -230,44 +244,62 @@
         os.makedirs(builds_dir, exist_ok=True)
         click.echo(f"[INFO] Builds directory set to '{builds_dir}'")
         volume_mounts.append(TartVolume(source=builds_dir, dest=remote_build_dir, name="builds", ro=False))
 
     for v in volumes:
         volume_mounts.append(TartVolume.from_string(v))
 
-    tart.run(tart_vm_name, volume_mounts)
-    ip = tart.ip(tart_vm_name, timeout=timeout)
-    if not ip:
-        click.echo(f"[ERROR] Error, VM was not reacheable after '{timeout}' seconds")
+    try:
+        tart.run(tart_vm_name, volume_mounts)
+    except:
+        click.secho(f"[ERROR] Failed to start VM '{tart_vm_name}'", fg="red")
         sys.exit(1)
 
-    ssh_session = tart.ssh_session(name=p.vm_name(), username=p.tart_ssh_username, password=p.tart_ssh_password)
-    ssh_session.exec_ssh_command(
-        f"sudo mkdir -p {remote_script_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_script_dir}",
-    )
+    try:
+        ip = tart.ip(tart_vm_name, timeout=timeout)
+    except:
+        click.secho(f"[ERROR] Failed to get IP of VM '{tart_vm_name}'", fg="red")
+        sys.exit(1)
 
-    for volume in volume_mounts:
-        click.echo(f"[INFO] Setting up volume mount '{volume.name}'")
-        ssh_session.exec_ssh_command(
-            f"sudo mkdir -p $(dirname {volume.dest}); sudo ln -sf '/Volumes/My Shared Files/{volume.name}' {volume.dest}",
-        )
+    if not ip:
+        click.echo(f"[ERROR] Error, VM was not reacheable after '{timeout}' seconds")
+        sys.exit(1)
 
-    # if cache and builds volumes are not mounted, make sure to create them locally inside the VM
-    if not cache_dir:
+    try:
+        ssh_session = tart.ssh_session(name=p.vm_name(), username=p.tart_ssh_username, password=p.tart_ssh_password)
         ssh_session.exec_ssh_command(
-            f"sudo mkdir -p {remote_cache_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_cache_dir}",
+            f"sudo mkdir -p {remote_script_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_script_dir}",
         )
 
-    if not builds_dir:
-        ssh_session.exec_ssh_command(
-            f"sudo mkdir -p {remote_build_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_build_dir}",
-        )
+        for volume in volume_mounts:
+            click.echo(f"[INFO] Setting up volume mount '{volume.name}'")
+            ssh_session.exec_ssh_command(
+                f"sudo mkdir -p $(dirname {volume.dest}); sudo ln -sf '/Volumes/My Shared Files/{volume.name}' {volume.dest}",
+            )
+
+        # if cache and builds volumes are not mounted, make sure to create them locally inside the VM
+        if not cache_dir:
+            ssh_session.exec_ssh_command(
+                f"sudo mkdir -p {remote_cache_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_cache_dir}",
+            )
+
+        if not builds_dir:
+            ssh_session.exec_ssh_command(
+                f"sudo mkdir -p {remote_build_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_build_dir}",
+            )
+    except:
+        click.secho(f"[ERROR] Failed so prepare VM '{tart_vm_name}'", fg="red")
+        sys.exit(1)
 
     if install_gitlab_runner:
         click.echo(
             f"[INFO] Installing GitLab Runner '{gitlab_runner_version}' [force: '{force_install_gitlab_runner}']"
         )
-        tart.install_gitlab_runner(name=tart_vm_name, username=p.tart_ssh_username, password=p.tart_ssh_password)
+        try:
+            tart.install_gitlab_runner(name=tart_vm_name, username=p.tart_ssh_username, password=p.tart_ssh_password)
+        except:
+            click.secho(f"[ERROR] Failed to install GitLab Runner '{gitlab_runner_version}'", fg="red")
+            sys.exit(1)
 
     tart.print_spec(tart_vm_name)
 
     sys.exit(0)
```

### Comparing `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/run.py` & `gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/commands/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 @click.option(
     "--default-ssh-username", default="admin", required=False, type=str, help="username to login to a tart vm"
 )
 @click.option(
     "--default-ssh-password", default="admin", required=False, type=str, help="password to login to a tart vm"
 )
 @click.option(
+    "--timeout", "ssh_timeout", default=60, required=False, type=int, help="SSH connection timeout in seconds"
+)
+@click.option(
     "-x",
     "--tart-executable",
     required=False,
     default="tart",
     type=str,
     help="Path to the tart executable.",
 )
@@ -27,32 +30,43 @@
     required=False,
     default="/bin/zsh",
     type=str,
     help="Path to the shell to be used for commands over ssh.",
 )
 @click.argument("script")
 @click.argument("stage")
-def run(default_ssh_username, default_ssh_password, tart_executable, shell, script, stage):
+def run(default_ssh_username, default_ssh_password, ssh_timeout, tart_executable, shell, script, stage):
     """Run commands."""
     p = GitLabCustomCommandConfig()
 
     if not p.tart_ssh_username:
         p.tart_ssh_username = default_ssh_username
     if not p.tart_ssh_password:
         p.tart_ssh_password = default_ssh_password
 
     ######################################################################
     # Connect to VM
     ######################################################################
     tart = Tart(exec_path=tart_executable)
     tart_vm_name = p.vm_name()
-    tart_ip = tart.ip(tart_vm_name, timeout=30)
-    click.echo(f"[INFO] Establishing SSH conntection to '{p.tart_ssh_username}@{tart_ip}'")
 
-    ssh_session = tart.ssh_session(name=p.vm_name(), username=p.tart_ssh_username, password=p.tart_ssh_password)
+    try:
+        tart_ip = tart.ip(tart_vm_name, timeout=ssh_timeout)
+        click.echo(f"[INFO] Establishing SSH conntection to '{p.tart_ssh_username}@{tart_ip}'")
+    except:
+        click.secho(
+            f"[ERROR] Could not establish SSH conntection to '{tart_vm_name}' after '{ssh_timeout}' seconds.", fg="red"
+        )
+        sys.exit(1)
+
+    try:
+        ssh_session = tart.ssh_session(name=p.vm_name(), username=p.tart_ssh_username, password=p.tart_ssh_password)
+    except:
+        click.secho(f"[ERROR] Could not establish SSH session with '{p.tart_ssh_username}@{tart_ip}'", fg="red")
+        sys.exit(1)
 
     click.echo("[INFO] Preparing workspace")
     remote_temp_dir = "/opt/temp"
 
     script_name = os.path.basename(script)
     remote_script_path = os.path.join(remote_temp_dir, stage + "-" + script_name)
```

### Comparing `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py` & `gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from typing import Optional
 
 from pydantic import BaseSettings
+from pydantic import Field
 
 
 class GitLabCustomCommandConfig(BaseSettings):
     """Config parameters needed throughout the process read from the environment"""
 
     ci_job_image: str
     ci_pipeline_id: str
     ci_job_id: str
     ci_concurrent_id: str
     ci_concurrent_project_id: str
     ci_runner_short_token: str
     ci_project_name: str
-    ci_registry: str
-    ci_registry_user: str
-    ci_registry_password: str
+    ci_registry: Optional[str]
+    ci_registry_user: Optional[str]
+    ci_registry_password: Optional[str]
 
     tart_registry_username: Optional[str]
     tart_registry_password: Optional[str]
     tart_registry: Optional[str]
 
     tart_ssh_username: Optional[str]
     tart_ssh_password: Optional[str]
 
+    tart_max_vm_count: Optional[int] = Field(default=2)
+
     class Config:
         """Define the prefix used by GitLab for all environment variables passed to a custom driver.
         see https://docs.gitlab.com/runner/executors/custom.html#stages
         """
 
         env_prefix = "CUSTOM_ENV_"
 
     def vm_name(self):
         """Creates a unique name for a VM"""
-        return f"{self.ci_project_name}-{self.ci_pipeline_id}-{self.ci_job_id}-{self.ci_concurrent_id}"
+        return f"{self.vm_name_prefix}-{self.ci_project_name}-{self.ci_pipeline_id}-{self.ci_job_id}-{self.ci_concurrent_id}"
+
+    @property
+    def vm_name_prefix(self):
+        return "grtd"
```

### Comparing `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/tart.py` & `gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/modules/tart.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/utils.py` & `gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/modules/utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2` & `gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/PKG-INFO` & `gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
@@ -432,14 +432,15 @@
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
   Run commands.
 
 Options:
   --default-ssh-username TEXT  username to login to a tart vm
   --default-ssh-password TEXT  password to login to a tart vm
+  --timeout INTEGER            SSH connection timeout in seconds
   -x, --tart-executable TEXT   Path to the tart executable.
   --shell TEXT                 Path to the shell to be used for commands over
                                ssh.
   --help                       Show this message and exit.
 ```
 
 ### Command `cleanup`
```

### Comparing `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/SOURCES.txt` & `gitlab-runner-tart-driver-0.1.6/gitlab_runner_tart_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.5/setup.py` & `gitlab-runner-tart-driver-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 # read the long description from README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.1.5"
+version = "0.1.6"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
```


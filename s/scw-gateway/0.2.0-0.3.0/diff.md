# Comparing `tmp/scw_gateway-0.2.0.tar.gz` & `tmp/scw_gateway-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_gateway-0.2.0.tar", max compression
+gzip compressed data, was "scw_gateway-0.3.0.tar", max compression
```

## Comparing `scw_gateway-0.2.0.tar` & `scw_gateway-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/__init__.py
--rw-r--r--   0        0        0     6509 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/cli.py
--rw-r--r--   0        0        0      352 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/client.py
--rw-r--r--   0        0        0     2465 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/conf.py
--rw-r--r--   0        0        0     5032 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/gateway.py
--rw-r--r--   0        0        0      281 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/__init__.py
--rw-r--r--   0        0        0     2210 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/cockpit.py
--rw-r--r--   0        0        0     6009 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/container.py
--rw-r--r--   0        0        0      519 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/function.py
--rw-r--r--   0        0        0      319 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/image.py
--rw-r--r--   0        0        0    15754 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/manager.py
--rw-r--r--   0        0        0      999 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/rdb.py
--rw-r--r--   0        0        0     2514 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/infra/secrets.py
--rw-r--r--   0        0        0     1037 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/cli/model.py
--rw-r--r--   0        0        0      921 2023-06-14 15:52:34.389430 scw_gateway-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 scw_gateway-0.2.0/setup.py
--rw-r--r--   0        0        0      622 1970-01-01 00:00:00.000000 scw_gateway-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/cli/__init__.py
+-rw-r--r--   0        0        0     4952 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/cli/cli.py
+-rw-r--r--   0        0        0      352 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/cli/client.py
+-rw-r--r--   0        0        0     2465 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/cli/conf.py
+-rw-r--r--   0        0        0     5032 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/cli/gateway.py
+-rw-r--r--   0        0        0      281 2023-06-26 09:43:44.956290 scw_gateway-0.3.0/cli/infra/__init__.py
+-rw-r--r--   0        0        0     1978 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/cockpit.py
+-rw-r--r--   0        0        0     6009 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/container.py
+-rw-r--r--   0        0        0      519 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/function.py
+-rw-r--r--   0        0        0      317 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/image.py
+-rw-r--r--   0        0        0    15463 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/manager.py
+-rw-r--r--   0        0        0      999 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/rdb.py
+-rw-r--r--   0        0        0     2515 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/infra/secrets.py
+-rw-r--r--   0        0        0     1037 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/cli/model.py
+-rw-r--r--   0        0        0      923 2023-06-26 09:43:44.960290 scw_gateway-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 scw_gateway-0.3.0/setup.py
+-rw-r--r--   0        0        0      622 1970-01-01 00:00:00.000000 scw_gateway-0.3.0/PKG-INFO
```

### Comparing `scw_gateway-0.2.0/cli/cli.py` & `scw_gateway-0.3.0/cli/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,88 @@
 import click
 
-from cli import client
+from cli import client, conf
 from cli.gateway import GatewayManager
 from cli.infra import InfraManager, cockpit
 from cli.model import Route
 
-DB_PASSWORD_OPTION = click.option(
-    "--db-password",
-    required=False,
-    help="The password to use for the database. Will be generated if not provided.",
-    envvar="DB_PASSWORD",
-)
-NO_METRICS_OPTION = click.option(
-    "--no-metrics",
-    is_flag=True,
-    default=False,
-    help="Disable Kong metrics integration with Cockpit.",
-)
-
 
 @click.group()
 def cli():
     """CLI for managing the gateway.
 
     See the README for more information.
     """
 
 
 @cli.command()
-def local_config():
-    """Sets up config for local deployment"""
+def deploy():
+    """Deploys all the gateway components"""
+    scw_client = client.get_scaleway_client()
+    manager = InfraManager(scw_client)
+
+    click.secho("Creating database", fg="blue")
+    manager.create_db()
+    manager.await_db()
+
+    click.secho("Creating container namespace", fg="blue")
+    manager.create_namespace()
+    manager.await_namespace()
+
+    click.secho("Checking cockpit activated", fg="blue")
+    cockpit.ensure_cockpit_activated(scw_client=scw_client)
+
+    click.secho("Creating containers", fg="blue")
+    manager.create_containers()
+    manager.await_containers()
+
+    click.secho("Setting up configuration", fg="blue")
+    manager.set_up_config(False)
+
+    click.secho("Enabling metrics", fg="blue")
+    gateway = GatewayManager()
+    gateway.setup_global_kong_statsd_plugin()
+
+
+@cli.command()
+def check():
+    """Checks the status of all gateway components"""
+    scw_client = client.get_scaleway_client()
+    manager = InfraManager(scw_client)
+
+    manager.check_db()
+    manager.check_namespace()
+    manager.check_containers()
+
+
+@cli.command()
+@click.option(
+    "--yes", "-y", is_flag=True, default=False, help="Skip interactive confirmation"
+)
+def delete(yes=False):
+    """Deletes all the gateway components"""
+
+    do_delete = yes
+    if not do_delete:
+        do_delete = click.confirm(
+            "This will delete all the components of your gateway. Are you sure?"
+        )
+
+    if do_delete:
+        scw_client = client.get_scaleway_client()
+        manager = InfraManager(scw_client)
+
+        manager.delete_containers()
+        manager.delete_db()
+        manager.delete_namespace()
+
+
+@cli.command()
+def dev_config():
+    """Sets up config for local development"""
     scw_client = client.get_scaleway_client()
     manager = InfraManager(scw_client)
     manager.set_up_config(True)
 
 
 @cli.command()
 def remote_config():
@@ -52,175 +101,76 @@
 
 @cli.command()
 @click.argument("relative_url")
 @click.argument("target")
 @click.option(
     "--cors", is_flag=True, default=False, help="Add permissive cors to the route."
 )
-def add_route(relative_url, target, cors):
+@click.option(
+    "--http-methods",
+    "-m",
+    help="HTTP methods that the route should accept. Defaults to all if not specified.",
+    multiple=True,
+)
+def add_route(relative_url: str, target: str, cors: bool, http_methods: list[str]):
     """Adds a route to the gateway"""
     manager = GatewayManager()
 
-    route = Route(relative_url, target, cors=cors)
+    route = Route(
+        relative_url=relative_url,
+        target=target,
+        http_methods=http_methods,
+        cors=cors,
+    )
     manager.add_route(route)
 
 
 @cli.command()
 @click.argument("relative_url")
 @click.argument("target")
 def delete_route(relative_url, target):
     """Deletes a route from the gateway"""
     manager = GatewayManager()
 
     route = Route(relative_url, target)
     manager.delete_route(route)
 
 
-# TODO: integrate with existing CLI commands
-@cli.command()
-def setup_metrics():
-    """Adds metrics plugin to the gateway"""
-    gateway = GatewayManager()
-    gateway.setup_global_kong_statsd_plugin()
-
-
 @cli.command()
 def create_admin_token():
     """Creates a token for the admin container"""
     scw_client = client.get_scaleway_client()
     manager = InfraManager(scw_client)
     token = manager.create_admin_container_token()
     click.secho(token)
 
 
 @cli.command()
-def delete_containers():
-    """Deletes the containers used for the gateway"""
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    manager.delete_containers()
-
-
-@cli.command()
 def get_endpoint():
-    """Returns the endpoint for the gateway"""
+    """Prints the endpoint for the gateway"""
     scw_client = client.get_scaleway_client()
     manager = InfraManager(scw_client)
     endpoint = manager.get_gateway_endpoint()
     click.secho(endpoint)
 
 
 @cli.command()
 def get_admin_endpoint():
-    """Returns the endpoint for the gateway admin"""
+    """Prints the endpoint for the gateway admin"""
     scw_client = client.get_scaleway_client()
     manager = InfraManager(scw_client)
     endpoint = manager.get_gateway_admin_endpoint()
     click.secho(endpoint)
 
 
 @cli.command()
-@DB_PASSWORD_OPTION
-@click.option(
-    "--no-save", is_flag=True, default=False, help="Do not save the password."
-)
-def create_db(db_password: str | None, no_save: bool):
-    """Creates the database for the gateway.
-
-    If --no-save is passed, the password will not be saved to Secret Manager.
-    The password will therefore need to be provided for other commands.
-    """
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    manager.create_db(password=db_password, save_password=not no_save)
-
-
-@cli.command()
-def delete_db():
-    """Deletes the database for the gateway."""
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    manager.delete_db()
-
-
-@cli.command()
-def check_db():
-    """Checks the status of the database"""
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    manager.check_db()
-
-
-@cli.command()
-def await_db():
-    """Waits for the database to be ready"""
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    manager.await_db()
-
-
-@cli.command()
-def create_namespace():
-    """Creates the container container namespace"""
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    manager.create_namespace()
-
-
-@cli.command()
-def check_namespace():
-    """Checks the status of the container namespace"""
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    manager.check_namespace()
-
-
-@cli.command()
-def await_namespace():
-    """Waits for the namespace to be ready"""
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    manager.await_namespace()
-
-
-@cli.command()
-def delete_namespace():
-    """Deletes the container namespace"""
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    manager.delete_namespace()
-
-
-@cli.command()
-@DB_PASSWORD_OPTION
-@NO_METRICS_OPTION
-def create_containers(db_password: str | None, no_metrics: bool):
-    """Creates the containers"""
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    if not no_metrics:
-        # Check that Cockpit is activated
-        no_metrics = not cockpit.ensure_cockpit_activated(scw_client=scw_client)
-    manager.create_containers(db_password=db_password, forward_metrics=not no_metrics)
-
-
-@cli.command()
-def check_containers():
-    """Checks the status of the containers"""
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    manager.check_containers()
-
-
-@cli.command()
-def await_containers():
-    """Waits for the containers to be ready"""
-    scw_client = client.get_scaleway_client()
-    manager = InfraManager(scw_client)
-    manager.await_containers()
+def get_admin_token():
+    """Prints the token for accessing the admin container"""
+    c = conf.InfraConfiguration.load()
+    click.secho(c.gw_admin_token)
 
 
 @cli.command()
 def set_custom_domain():
     """Sets the custom domain for the gateway container"""
     scw_client = client.get_scaleway_client()
     manager = InfraManager(scw_client)
@@ -230,20 +180,18 @@
 @cli.command()
 @click.option(
     "--no-redeploy",
     is_flag=True,
     default=False,
     help="Don't redeploy the container, just update.",
 )
-@DB_PASSWORD_OPTION
 def update_containers(
     no_redeploy: bool,
-    db_password: str | None,
 ):
     """Updates the containers"""
     scw_client = client.get_scaleway_client()
     manager = InfraManager(scw_client)
 
     if no_redeploy:
-        manager.update_container_without_deploy(db_password=db_password)
+        manager.update_container_without_deploy()
     else:
-        manager.update_container(db_password=db_password)
+        manager.update_container()
```

### Comparing `scw_gateway-0.2.0/cli/conf.py` & `scw_gateway-0.3.0/cli/conf.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.2.0/cli/gateway.py` & `scw_gateway-0.3.0/cli/gateway.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.2.0/cli/infra/cockpit.py` & `scw_gateway-0.3.0/cli/infra/cockpit.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,39 +10,32 @@
     query_logs=False,
     write_logs=False,
     setup_logs_rules=False,
     setup_alerts=False,
 )
 
 
-def ensure_cockpit_activated(scw_client: Client) -> bool:
-    """Ensure Cockpit is activated.
-
-    Prompt the user to activate cockpit if it is not activated.
-    """
+def ensure_cockpit_activated(scw_client: Client):
+    """Ensure Cockpit is activated"""
     api = sdk.CockpitV1Beta1API(scw_client)
+
     try:
         api.get_cockpit()
-        return True
+
+        # If successful, cockpit activated
+        return
     except ScalewayException as err:
         if not err.status_code == 404:
             raise
 
-        should_activate_cockpit = click.confirm(
-            "Cockpit not activated for project. Do you want to activate it?",
-        )
-
-        if not should_activate_cockpit:
-            return False
+        # Activate the cockpit
         cockpit = api.activate_cockpit()
         api.wait_for_cockpit(project_id=cockpit.project_id)
         click.secho("Cockpit activated", fg="green")
 
-        return True
-
 
 def get_metrics_push_url(api: sdk.CockpitV1Beta1API) -> str:
     """Get the Cockpit metrics push URL."""
     cockpit = api.get_cockpit()
 
     if not cockpit.endpoints:
         # Should never happen
```

### Comparing `scw_gateway-0.2.0/cli/infra/container.py` & `scw_gateway-0.3.0/cli/infra/container.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.2.0/cli/infra/function.py` & `scw_gateway-0.3.0/cli/infra/function.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.2.0/cli/infra/manager.py` & `scw_gateway-0.3.0/cli/infra/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,61 +139,62 @@
         return container.domain_name
 
     def get_gateway_admin_endpoint(self) -> str:
         """Get the endpoint of the gateway admin."""
         container = self._get_admin_container_or_abort()
         return container.domain_name
 
-    def create_db(self, password: str | None, save_password: bool) -> None:
+    def create_db(self) -> None:
         """Create the database instance."""
 
         instance_name = infra.rdb.DB_INSTANCE_NAME
         instance = infra.rdb.get_database_instance_by_name(self.rdb, instance_name)
         if instance:
             click.secho(f"Database {instance_name} already exists")
             return
 
         click.secho(f"Creating database instance {instance_name}...")
 
-        if not password:
-            logger.info("Generating database password")
-            password = infra.secrets.generate_database_password()
-
-        if save_password:
-            logger.info("Saving database password")
-            infra.secrets.create_db_password_secret(self.secrets, password)
+        logger.debug("Generating database password")
+        password = infra.secrets.generate_database_password()
+
+        logger.debug("Saving database password")
+        infra.secrets.create_db_password_secret(self.secrets, password)
 
         infra.rdb.create_database_instance(self.rdb, password)
         click.secho("Database created", fg="green", bold="true")
 
     def check_db(self):
         """Check the status of the database instance."""
         instance = self._get_database_instance_or_abort()
         click.secho(f"Database status: {instance.status}", bold=True)
 
     def await_db(self) -> None:
         """Wait for the database instance to be ready."""
+
+        click.secho("Waiting for database to be ready...", fg="blue")
+
         instance = self._get_database_instance_or_abort()
         instance = self.rdb.wait_for_instance(instance_id=instance.id)
 
         if instance.status != rdb.InstanceStatus.READY:
             click.secho("Database is not ready", fg="red", bold="true")
             raise click.Abort()
 
-        click.secho("Database ready", fg="green", bold=True)
+        click.secho("Database ready")
 
     def delete_db(self) -> None:
         """Delete the database instance."""
         # Delete the secret
         infra.secrets.delete_db_password_secret(self.secrets)
 
         # Delete the database
         instance = self._get_database_instance_or_abort()
         self.rdb.delete_instance(instance_id=instance.id)
-        click.secho("Database deleted", fg="green", bold=True)
+        click.secho("Database deleted")
 
     def create_namespace(self):
         """Create the namespace for the gateway."""
         namespace_name = infra.cnt.CONTAINER_NAMESPACE
         namespace = infra.cnt.get_namespace_by_name(self.containers, namespace_name)
 
         if namespace:
@@ -214,41 +215,43 @@
             )
             raise click.Abort()
 
         click.secho(f"Namespace status: {namespace.status}", bold=True)
 
     def await_namespace(self):
         """Wait for the namespace to be ready."""
+
+        click.secho("Waiting for namespace to be ready...", fg="blue")
+
         namespace = self._get_namespace_or_abort()
         namespace = self.containers.wait_for_namespace(namespace_id=namespace.id)
         if namespace.status == cnt.NamespaceStatus.ERROR:
             click.secho(
                 f"Namespace in error: {namespace.error_message}",
                 fg="red",
                 bold=True,
             )
             raise click.Abort()
 
         if namespace.status != cnt.NamespaceStatus.READY:
             click.secho("Namespace is not ready", fg="red", bold=True)
             raise click.Abort()
 
-        click.secho("Namespace ready", fg="green", bold=True)
+        click.secho("Namespace ready")
 
     def delete_namespace(self):
         """Delete the namespace."""
         namespace = self._get_namespace_or_abort()
         self.containers.delete_namespace(namespace_id=namespace.id)
-        click.secho("Namespace deleted", fg="green", bold=True)
+        click.secho("Namespace deleted")
 
-    def create_containers(self, db_password: str | None, forward_metrics: bool) -> None:
+    def create_containers(self) -> None:
         """Create containers for Kong and Kong Admin."""
         database_instance = self._get_database_instance_or_abort()
-        if not db_password:
-            db_password = self._get_db_password_or_abort()
+        db_password = self._get_db_password_or_abort()
         db_host, db_port = self._get_database_endpoint_or_abort(database_instance)
 
         # Namespace should be created before creating containers
         namespace = self._get_namespace_or_abort()
 
         admin_container_name = infra.cnt.CONTAINER_ADMIN_NAME
         admin_container = infra.cnt.get_container_by_name(
@@ -272,28 +275,27 @@
         container = infra.cnt.get_container_by_name(
             self.containers, namespace.id, container_name
         )
         if container:
             click.secho(f"Container {container_name} already exists")
             return
 
-        click.secho(f"Creating container {container_name}")
-
-        token, metrics_push_url = None, None
-        if forward_metrics:
-            # Check if token exists
-            token = infra.cpt.get_metrics_token(self.cockpit)
-            if token:
-                click.echo("Cockpit token already exists, recreating")
-                infra.cpt.delete_metrics_token(self.cockpit, token)
-            else:
-                click.echo("Creating Cockpit token")
+        click.secho(
+            f"Creating container {container_name} from tag {infra.image.IMAGE_TAG}"
+        )
 
-            token_key = infra.cpt.create_metrics_token(self.cockpit)
-            metrics_push_url = infra.cpt.get_metrics_push_url(self.cockpit)
+        # Check if token exists
+        token = infra.cpt.get_metrics_token(self.cockpit)
+        if token:
+            click.echo("Cockpit token already exists, deleting")
+            infra.cpt.delete_metrics_token(self.cockpit, token)
+
+        click.echo("Creating Cockpit token")
+        token_key = infra.cpt.create_metrics_token(self.cockpit)
+        metrics_push_url = infra.cpt.get_metrics_push_url(self.cockpit)
 
         created_container = infra.cnt.create_kong_container(
             self.containers,
             namespace.id,
             db_host,
             db_port,
             db_password,
@@ -310,46 +312,49 @@
         container = self._get_container_or_abort()
 
         click.secho(f"Admin container status: {admin_container.status}", bold=True)
         click.secho(f"Container status: {container.status}", bold=True)
 
     def await_containers(self):
         """Wait for the containers to be ready."""
+
+        click.secho("Waiting for containers to be ready...", fg="blue")
+
         admin_container = self._get_admin_container_or_abort()
         container = self._get_container_or_abort()
 
         # Execute in parallel
         results = futures.ThreadPoolExecutor(max_workers=2).map(
             lambda id: self.containers.wait_for_container(container_id=id),
             (admin_container.id, container.id),
         )
         for res in results:
             if res.status == cnt.ContainerStatus.ERROR:
                 click.secho(
                     f"Container {res.name} is in error: {res.error_message}"
-                    "Check the logs for more details.",
+                    ". Check the logs for more details.",
                     fg="red",
                     bold=True,
                 )
                 raise click.Abort()
             if res.status != cnt.ContainerStatus.READY:
                 click.secho(f"Container {res.name} is not ready", fg="red", bold=True)
                 raise click.Abort()
-        click.secho("Containers are ready", fg="green", bold=True)
+        click.secho("Containers are ready")
 
     def delete_containers(self):
         """Delete the containers."""
         admin_container = self._get_admin_container_or_abort()
         container = self._get_container_or_abort()
 
-        click.secho(f"Deleting container {admin_container.name}")
         self.containers.delete_container(container_id=admin_container.id)
+        click.secho("Admin container deleted")
 
-        click.secho(f"Deleting container {container.name}")
         self.containers.delete_container(container_id=container.id)
+        click.secho("Gateway container deleted")
 
     def get_function_endpoint(
         self, namespace_name: str, function_name: str
     ) -> str | None:
         """Get the endpoint of a function."""
         return infra.fnc.get_function_endpoint_by_name(
             self.functions, namespace_name, function_name
@@ -357,36 +362,35 @@
 
     def create_admin_container_token(self) -> str:
         """Create a token to access the private admin container."""
         admin_container = self._get_admin_container_or_abort()
         token = self.containers.create_token(container_id=admin_container.id)
         return token.token
 
-    def update_container(self, db_password: str | None):
+    def update_container(self):
         """Update the container."""
-        self.update_container_without_deploy(db_password=db_password)
+        self.update_container_without_deploy()
 
         admin_container = self._get_admin_container_or_abort()
         container = self._get_container_or_abort()
 
         click.secho("Deploying admin container...")
         self.containers.deploy_container(container_id=admin_container.id)
 
         click.secho("Deploying container...")
         self.containers.deploy_container(container_id=container.id)
 
-    def update_container_without_deploy(self, db_password: str | None):
+    def update_container_without_deploy(self):
         """Update the container without deploying it."""
         admin_container = self._get_admin_container_or_abort()
         container = self._get_container_or_abort()
 
         database_instance = self._get_database_instance_or_abort()
         db_host, db_port = self._get_database_endpoint_or_abort(database_instance)
-        if not db_password:
-            db_password = self._get_db_password_or_abort()
+        db_password = self._get_db_password_or_abort()
 
         click.echo(f"Updating container {admin_container.name}")
         infra.cnt.update_kong_admin_container(
             self.containers, admin_container.id, db_host, db_port, db_password
         )
         click.echo(f"Updating container {container.name}")
```

### Comparing `scw_gateway-0.2.0/cli/infra/rdb.py` & `scw_gateway-0.3.0/cli/infra/rdb.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.2.0/cli/infra/secrets.py` & `scw_gateway-0.3.0/cli/infra/secrets.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 def create_db_password_secret(api: sdk.SecretV1Alpha1API, db_password: str):
     """Store the password to Secret Manager."""
 
     delete_db_password_secret(api)
 
-    logger.info("Creating secret for database password")
+    logger.debug("Creating secret for database password")
     secret = api.create_secret(
         name=PASSWORD_NAME,
         tags=["scw-gw"],
         description="Password for the database for scw-gw",
     )
 
     data = db_password.encode("utf-8")
```

### Comparing `scw_gateway-0.2.0/cli/model.py` & `scw_gateway-0.3.0/cli/model.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.2.0/pyproject.toml` & `scw_gateway-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "scw-gateway"
-version = "0.2.0"
+version = "0.3.0"
 description = "CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem"
 authors = ["Simon Shillaker <sshillaker@scaleway.com>"]
 readme = "README.md"
-packages = [{include = "cli"}]
+packages = [{ include = "cli" }]
 
 [tool.poetry.dependencies]
 loguru = "0.6.0"
 python = "^3.10"
 requests = "^2.28.2"
 click = "^8.1.3"
 pyyaml = "^6.0"
```

### Comparing `scw_gateway-0.2.0/setup.py` & `scw_gateway-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'scaleway>=0.12.0,<0.13.0']
 
 entry_points = \
 {'console_scripts': ['scwgw = cli.cli:cli']}
 
 setup_kwargs = {
     'name': 'scw-gateway',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem',
     'long_description': '',
     'author': 'Simon Shillaker',
     'author_email': 'sshillaker@scaleway.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scw_gateway-0.2.0/PKG-INFO` & `scw_gateway-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scw-gateway
-Version: 0.2.0
+Version: 0.3.0
 Summary: CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem
 Author: Simon Shillaker
 Author-email: sshillaker@scaleway.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


# Comparing `tmp/azureml_contrib_mir-1.8.0-py3-none-any.whl.zip` & `tmp/azureml_contrib_mir-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 25031 bytes, number of entries: 17
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/__init__.py
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/contrib/__init__.py
--rw-rw-rw-  2.0 fat      183 b- defN 20-Jun-22 17:21 azureml/contrib/_mircli/__init__.py
--rw-rw-rw-  2.0 fat    13179 b- defN 20-Jun-22 17:21 azureml/contrib/_mircli/_cli.py
--rw-rw-rw-  2.0 fat    42146 b- defN 20-Jun-22 17:21 azureml/contrib/_mircli/_util.py
--rw-rw-rw-  2.0 fat      347 b- defN 20-Jun-22 17:21 azureml/contrib/mir/__init__.py
--rw-rw-rw-  2.0 fat      441 b- defN 20-Jun-22 17:21 azureml/contrib/mir/webservice/__init__.py
--rw-rw-rw-  2.0 fat      385 b- defN 20-Jun-22 17:21 azureml/contrib/mir/webservice/_util.py
--rw-rw-rw-  2.0 fat    41992 b- defN 20-Jun-22 17:21 azureml/contrib/mir/webservice/mir.py
--rw-rw-rw-  2.0 fat      761 b- defN 20-Jun-22 17:21 azureml/contrib/mir/webservice/data/mir_service_payload_template.json
--rw-rw-rw-  2.0 fat       23 b- defN 20-Jun-22 17:21 azureml_contrib_mir-1.8.0.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat     1021 b- defN 20-Jun-22 17:21 azureml_contrib_mir-1.8.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      643 b- defN 20-Jun-22 17:21 azureml_contrib_mir-1.8.0.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        8 b- defN 20-Jun-22 17:21 azureml_contrib_mir-1.8.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 20-Jun-22 17:21 azureml_contrib_mir-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      406 b- defN 20-Jun-22 17:21 azureml_contrib_mir-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat     1604 b- defN 20-Jun-22 17:21 azureml_contrib_mir-1.8.0.dist-info/RECORD
-17 files, 103738 bytes uncompressed, 22347 bytes compressed:  78.5%
+Zip file size: 25276 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/contrib/__init__.py
+-rw-rw-rw-  2.0 fat      183 b- defN 20-Jul-06 20:24 azureml/contrib/_mircli/__init__.py
+-rw-rw-rw-  2.0 fat    13215 b- defN 20-Jul-06 20:24 azureml/contrib/_mircli/_cli.py
+-rw-rw-rw-  2.0 fat    42623 b- defN 20-Jul-06 20:24 azureml/contrib/_mircli/_util.py
+-rw-rw-rw-  2.0 fat      347 b- defN 20-Jul-06 20:24 azureml/contrib/mir/__init__.py
+-rw-rw-rw-  2.0 fat      441 b- defN 20-Jul-06 20:24 azureml/contrib/mir/webservice/__init__.py
+-rw-rw-rw-  2.0 fat      385 b- defN 20-Jul-06 20:24 azureml/contrib/mir/webservice/_util.py
+-rw-rw-rw-  2.0 fat    43605 b- defN 20-Jul-06 20:24 azureml/contrib/mir/webservice/mir.py
+-rw-rw-rw-  2.0 fat      792 b- defN 20-Jul-06 20:24 azureml/contrib/mir/webservice/data/mir_service_payload_template.json
+-rw-rw-rw-  2.0 fat       23 b- defN 20-Jul-06 20:25 azureml_contrib_mir-1.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat     1021 b- defN 20-Jul-06 20:25 azureml_contrib_mir-1.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      643 b- defN 20-Jul-06 20:25 azureml_contrib_mir-1.9.0.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        8 b- defN 20-Jul-06 20:25 azureml_contrib_mir-1.9.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 20-Jul-06 20:25 azureml_contrib_mir-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      406 b- defN 20-Jul-06 20:25 azureml_contrib_mir-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     1604 b- defN 20-Jul-06 20:25 azureml_contrib_mir-1.9.0.dist-info/RECORD
+17 files, 105895 bytes uncompressed, 22592 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -24,29 +24,29 @@
 
 Filename: azureml/contrib/mir/webservice/mir.py
 Comment: 
 
 Filename: azureml/contrib/mir/webservice/data/mir_service_payload_template.json
 Comment: 
 
-Filename: azureml_contrib_mir-1.8.0.dist-info/DESCRIPTION.rst
+Filename: azureml_contrib_mir-1.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: azureml_contrib_mir-1.8.0.dist-info/LICENSE.txt
+Filename: azureml_contrib_mir-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_contrib_mir-1.8.0.dist-info/metadata.json
+Filename: azureml_contrib_mir-1.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_contrib_mir-1.8.0.dist-info/top_level.txt
+Filename: azureml_contrib_mir-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_contrib_mir-1.8.0.dist-info/WHEEL
+Filename: azureml_contrib_mir-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_contrib_mir-1.8.0.dist-info/METADATA
+Filename: azureml_contrib_mir-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_contrib_mir-1.8.0.dist-info/RECORD
+Filename: azureml_contrib_mir-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/contrib/_mircli/_cli.py

```diff
@@ -23,16 +23,16 @@
                  entry_script, runtime, conda_file, extra_docker_file_steps, source_directory, base_image,
                  base_image_registry, cuda_version, compute_type, cpu_cores, memory_gb, auth_enabled,
                  autoscale_enabled, autoscale_min_replicas, autoscale_max_replicas, autoscale_refresh_seconds,
                  autoscale_target_utilization, collect_model_data, scoring_timeout_ms,
                  replica_max_concurrent_requests, max_request_wait_time, num_replicas,
                  tls_mode, certificate_fingerprints, compute_target, deploy_config_file,
                  profile_metadata_file, path, workspace_name, resource_group, no_wait_flag, verbose_local,
-                 environment_name, environment_version, environment_directory, sku, gpu_cores, osType=None,
-                 context=cli_context):
+                 environment_name, environment_version, environment_directory, sku, gpu_cores,
+                 enable_app_insights, osType=None, context=cli_context):
     # user needs to provide either models, or model_metadata_files
     if (not models) and (not model_metadata_files):
         raise MlCliError('Error, need to specify either --model or --model-metadata-file '
                          'for model(s) to be deployed.')
 
     workspace = context.get_workspace(workspace_name, resource_group, path)
 
@@ -98,22 +98,22 @@
 
                 deploy_compute_type = deploy_config_obj[compute_type_key].lower()
         except Exception as ex:
             raise MlCliError('Error getting deploy compute type from config file.', content=ex)
 
     deploy_config = create_deploy_config(deploy_config_file, deploy_compute_type, cpu_cores, memory_gb, tags_dict,
                                          properties_dict, description, None, auth_enabled, None,
-                                         None, None, None, None,
+                                         enable_app_insights, None, None, None,
                                          None, autoscale_enabled, autoscale_min_replicas,
                                          autoscale_max_replicas, autoscale_refresh_seconds,
                                          autoscale_target_utilization, collect_model_data, scoring_timeout_ms,
                                          replica_max_concurrent_requests, max_request_wait_time, num_replicas,
                                          None, None, tags, properties, gpu_cores, None,
-                                         None, None, None, None,
-                                         None, None, None, tls_mode, certificate_fingerprints, sku, osType)
+                                         None, None, None, None, None, None, None,
+                                         tls_mode, certificate_fingerprints, sku, osType)
 
     # Get profiling results from input file
     profile_results = None
     if profile_metadata_file:
         with open(profile_metadata_file, 'r') as infile:
             profile_metadata = json.load(infile)
             if profile_metadata.get(PROFILE_RECOMMENDED_CPU_KEY) is None or \
```

## azureml/contrib/_mircli/_util.py

```diff
@@ -415,26 +415,26 @@
                 autoscale_target_utilization=autoscale_target_utilization, collect_model_data=collect_model_data,
                 auth_enabled=auth_enabled, cpu_cores=cpu_cores, memory_gb=memory_gb,
                 scoring_timeout_ms=scoring_timeout_ms,
                 replica_max_concurrent_requests=replica_max_concurrent_requests,
                 max_request_wait_time=max_request_wait_time, num_replicas=num_replicas,
                 tags=tags, properties=properties, description=description,
                 tls_mode=tls_mode, certificate_fingerprints=certificate_fingerprints, sku=sku, gpu_cores=gpu_cores,
-                osType=osType)
+                osType=osType, enable_app_insights=enable_app_insights)
     else:
         deploy_config_from_file = file_to_deploy_config(deploy_config_file, tags_dict, properties_dict,
                                                         description, compute_type)
         if compute_type == "mir":
             deploy_config = params_to_mir_config(autoscale_enabled, autoscale_min_replicas, autoscale_max_replicas,
                                                  autoscale_refresh_seconds,
                                                  autoscale_target_utilization, collect_model_data, auth_enabled,
                                                  cpu_cores, memory_gb, scoring_timeout_ms,
                                                  replica_max_concurrent_requests, max_request_wait_time,
                                                  num_replicas, tags, properties, description, tls_mode,
-                                                 certificate_fingerprints, sku, gpu_cores, osType,
+                                                 certificate_fingerprints, sku, gpu_cores, osType, enable_app_insights,
                                                  deploy_config_from_file)
     return deploy_config
 
 
 def file_to_inference_config(workspace, inference_config_file, description, environment_input=None):
     """Takes an inference_config_file and returns the InferenceConfig object
     :param workspace: current AzML workspace
@@ -701,31 +701,32 @@
                     tags=tags_dict,
                     properties=properties_dict,
                     description=description,
                     tls_mode=deploy_config_obj.get('tlsMode'),
                     certificate_fingerprints=deploy_config_obj.get('certificateFingerprints'),
                     sku=deploy_config_obj.get('sku'),
                     gpu_cores=deploy_config_obj.get('containerResourceRequirements', {}).get('gpu'),
-                    osType=deploy_config_obj.get('osType')
+                    osType=deploy_config_obj.get('osType'),
+                    enable_app_insights=deploy_config_obj.get('appInsightsEnabled')
                 )
             else:
                 raise MlCliError("unknown deployment type: {}".format(deploy_compute_type))
             return config
     except WebserviceException as web_service_ex:
         # Deployment config validation failure will raise WebserviceException, so we wrap it with MlCliError
         raise MlCliError('Invalid deployment configuration.', content=web_service_ex)
     except Exception as ex:
         raise MlCliError('Error parsing --deploy-config-file. Must be valid JSON or YAML file.', content=ex)
 
 
 def params_to_mir_config(autoscale_enabled, autoscale_min_replicas, autoscale_max_replicas, autoscale_refresh_seconds,
                          autoscale_target_utilization, collect_model_data, auth_enabled, cpu_cores, memory_gb,
-                         scoring_timeout_ms, replica_max_concurrent_requests,
-                         max_request_wait_time, num_replicas, tags, properties,
-                         description, tls_mode, certificate_fingerprints, sku, gpu_cores, osType, config_from_file):
+                         scoring_timeout_ms, replica_max_concurrent_requests, max_request_wait_time,
+                         num_replicas, tags, properties, description, tls_mode, certificate_fingerprints,
+                         sku, gpu_cores, osType, enable_app_insights, config_from_file):
     """Takes mir config parameters and returns an MirServiceDeploymentConfiguration object.
     The parameters in this method will overwrite attributes from the config
     :param autoscale_enabled: Whether or not to enable autoscaling for this Webservice.
         Defaults to True if num_replicas is None
     :type autoscale_enabled: bool
     :param autoscale_min_replicas: The minimum number of containers to use when autoscaling this Webservice.
         Defaults to 1
@@ -770,14 +771,17 @@
     :type certificate_fingerprints: :class:`list[str]`
     :param sku: Azure SKU type for MIR compute
     :type sku: str
     :param gpu_cores: The number of gpu cores to allocate for this Webservice. Defaults to 1
     :type gpu_cores: int
     :param osType: OS type of the mir service, valid options are "Linux", "Windows"
     :type osType: str
+    :param enable_app_insights: Whether or not to enable Application Insights logging for this Webservice.
+        Defaults to False
+    :type enable_app_insights: bool
     :param config_from_file: Attributes from this object will be used to create the new
         MirServiceDeploymentConfiguration object. Parameters provided to this method take precedence over the
         attributes given by this config object parameter
     :type config_from_file: azureml.contrib.mir.webservice.MirServiceDeploymentConfiguration
     :return: MirServiceDeploymentConfiguration object
     :rtype: azureml.contrib.mir.webservice.MirServiceDeploymentConfiguration
     """
@@ -817,8 +821,10 @@
         properties=properties if properties else config_from_file.properties,
         description=description if description else config_from_file.description,
         tls_mode=tls_mode if tls_mode else config_from_file.tls_mode,
         certificate_fingerprints=certificate_fingerprints
         if certificate_fingerprints else config_from_file.certificate_fingerprints,
         sku=sku if sku else config_from_file.sku,
         gpu_cores=gpu_cores if gpu_cores else config_from_file.gpu_cores,
-        osType=osType if osType else config_from_file.osType)
+        osType=osType if osType else config_from_file.osType,
+        enable_app_insights=enable_app_insights
+        if enable_app_insights is not None else config_from_file.enable_app_insights)
```

## azureml/contrib/mir/webservice/mir.py

```diff
@@ -52,14 +52,15 @@
         if ("validate_payload" not in kwargs or kwargs["validate_payload"]):
             MirWebservice._validate_get_payload(obj_dict)
 
         # Initialize common Webservice attributes
         super(MirWebservice, self)._initialize(workspace, obj_dict)
 
         # Initialize expected MIR specific attributes
+        self.enable_app_insights = obj_dict.get('appInsightsEnabled')
         self.autoscaler = AutoScaler.deserialize(obj_dict['autoScaler'])
         self.compute_name = obj_dict.get('computeName')
         self.container_resource_requirements = \
             ContainerResourceRequirements.deserialize(obj_dict.get('containerResourceRequirements'))
         self.liveness_probe_requirements = \
             LivenessProbeRequirements.deserialize(obj_dict.get('livenessProbeRequirements'))
         self.data_collection = DataCollection.deserialize(obj_dict.get('dataCollection'))
@@ -84,15 +85,16 @@
     @staticmethod
     def deploy_configuration(autoscale_enabled=None, autoscale_min_replicas=None, autoscale_max_replicas=None,
                              autoscale_refresh_seconds=None, autoscale_target_utilization=None,
                              collect_model_data=None, auth_enabled=None, cpu_cores=None, memory_gb=None,
                              scoring_timeout_ms=None, replica_max_concurrent_requests=None,
                              max_request_wait_time=None, num_replicas=None, tags=None, properties=None,
                              description=None, tls_mode=None, certificate_fingerprints=None, sku=None,
-                             gpu_cores=None, osType=None):
+                             gpu_cores=None, osType=None, enable_app_insights=None):
+
         """Create a configuration object for deploying to an MIR compute target.
 
         :param autoscale_enabled: Whether or not to enable autoscaling for this Webservice.
             Defaults to True if num_replicas is None
         :type autoscale_enabled: bool
         :param autoscale_min_replicas: The minimum number of containers to use when autoscaling this Webservice.
             Defaults to 1
@@ -139,26 +141,29 @@
         :param sku: Azure SKU type for MIR compute, valid options are "Standard_A2_v2", "Standard_F16", &
             "Standard_DS2_v2"
         :type sku: str
         :param gpu_cores: The number of gpu cores to allocate for this Webservice. Defaults to 1
         :type gpu_cores: int
         :param osType: OS type of the mir service, valid options are "Linux", "Windows"
         :type osType: str
+        :param enable_app_insights: Whether or not to enable Application Insights logging for this Webservice.
+            Defaults to False.
+        :type enable_app_insights: bool
         :return: A configuration object to use when deploying a Webservice object.
             The first and last characters cannot be hyphens.
         :rtype: MirServiceDeploymentConfiguration
         :raises: azureml.exceptions.WebserviceException
         """
         config = MirServiceDeploymentConfiguration(autoscale_enabled, autoscale_min_replicas, autoscale_max_replicas,
                                                    autoscale_refresh_seconds, autoscale_target_utilization,
                                                    collect_model_data, auth_enabled, cpu_cores, memory_gb,
                                                    scoring_timeout_ms, replica_max_concurrent_requests,
                                                    max_request_wait_time, num_replicas, tags, properties,
                                                    description, tls_mode, certificate_fingerprints, sku, gpu_cores,
-                                                   osType)
+                                                   osType, enable_app_insights)
         return config
 
     def _deploy(self, workspace, name, image, deployment_config, deployment_target, overwrite=False):
         """Deploy the Webservice.
 
         :raises: azureml.exceptions.WebserviceException
         """
@@ -196,28 +201,31 @@
         else:
             raise WebserviceException('Received bad response from service:\n'
                                       'Response Code: {}\n'
                                       'Headers: {}\n'
                                       'Content: {}'.format(resp.status_code, resp.headers, resp.content),
                                       logger=module_logger)
 
-    def update(self, cpu_cores=None, gpu_cores=None, memory_gb=None,
+    def update(self, cpu_cores=None, gpu_cores=None, memory_gb=None, enable_app_insights=None,
                scoring_timeout_ms=None, replica_max_concurrent_requests=None,
                num_replicas=None, models=None, inference_config=None, sku=None,
                tags=None, properties=None, description=None):
         """Update the MirWebservice with provided properties.
 
         Values left as None will remain unchanged in this Webservice.
 
         :param cpu_cores: The number of cpu cores to allocate for this Webservice. Can be a decimal
         :type cpu_cores: float
         :param gpu_cores: The number of gpu cores to allocate for this Webservice. Must be an integer
         :type gpu_cores: int
         :param memory_gb: The amount of memory (in GB) to allocate for this Webservice. Can be a decimal
         :type memory_gb: float
+        :param enable_app_insights: Whether or not to enable Application Insights logging for this Webservice.
+            Defaults to False.
+        :type enable_app_insights: bool
         :param scoring_timeout_ms: A timeout to enforce for scoring calls to this Webservice
         :type scoring_timeout_ms: int
         :param replica_max_concurrent_requests: The number of maximum concurrent requests per replica to allow for this
             Webservice.
         :type replica_max_concurrent_requests: int
         :param max_request_wait_time: The maximum amount of time a request will stay in the queue (in milliseconds)
             before returning a 503 error
@@ -236,25 +244,25 @@
         :param properties: Dictionary of key value properties to add to existing properties dictionary
         :type properties: dict[str, str]
         :param description: A description to give this Webservice
         :type description: str
         :raises: :class:`azureml.exceptions.WebserviceException`
         """
         if not cpu_cores and not memory_gb \
-                and not gpu_cores and not scoring_timeout_ms \
+                and not gpu_cores and enable_app_insights is None and not scoring_timeout_ms \
                 and not replica_max_concurrent_requests and not num_replicas \
                 and models is None and inference_config is None and sku is None \
                 and tags is None and properties is None and not description:
             raise WebserviceException('No parameters provided to update.', logger=module_logger)
 
         headers = {'Content-Type': 'application/json-patch+json'}
         headers.update(self._auth.get_authentication_header())
         params = {}
 
-        self._validate_update(cpu_cores, gpu_cores, memory_gb,
+        self._validate_update(cpu_cores, gpu_cores, memory_gb, enable_app_insights,
                               scoring_timeout_ms, replica_max_concurrent_requests,
                               num_replicas, models, inference_config, sku,
                               tags, properties, description)
 
         patch_list = []
 
         if inference_config:
@@ -284,14 +292,16 @@
             patch_list.append({'op': 'replace', 'path': '/containerResourceRequirements/cpu', 'value': cpu_cores})
         if gpu_cores:
             patch_list.append({'op': 'replace', 'path': '/containerResourceRequirements/gpu', 'value': gpu_cores})
         if memory_gb:
             patch_list.append({'op': 'replace', 'path': '/containerResourceRequirements/memoryInGB',
                                'value': memory_gb})
 
+        if enable_app_insights is not None:
+            patch_list.append({'op': 'replace', 'path': '/appInsightsEnabled', 'value': enable_app_insights})
         if scoring_timeout_ms:
             patch_list.append({'op': 'replace', 'path': '/scoringTimeoutMs', 'value': scoring_timeout_ms})
         if replica_max_concurrent_requests:
             patch_list.append({'op': 'replace', 'path': '/maxConcurrentRequestsPerContainer',
                                'value': replica_max_concurrent_requests})
 
         if num_replicas:
@@ -332,27 +342,30 @@
         else:
             raise WebserviceException('Received bad response from Model Management Service:\n'
                                       'Response Code: {}\n'
                                       'Headers: {}\n'
                                       'Content: {}'.format(resp.status_code, resp.headers, resp.content),
                                       logger=module_logger)
 
-    def _validate_update(self, cpu_cores=None, gpu_cores=None, memory_gb=None,
+    def _validate_update(self, cpu_cores=None, gpu_cores=None, memory_gb=None, enable_app_insights=None,
                          scoring_timeout_ms=None, replica_max_concurrent_requests=None,
                          num_replicas=None, models=None,
                          inference_config=None, sku=None, tags=None,
                          properties=None, description=None):
         """Validate the values provided to update the MIR Webservice.
 
         :param cpu_cores: The number of cpu cores to allocate for this Webservice. Can be a decimal
         :type cpu_cores: float
         :param gpu_cores: The number of gpu cores to allocate for this Webservice. Must be an integer
         :type gpu_cores: int
         :param memory_gb: The amount of memory (in GB) to allocate for this Webservice. Can be a decimal
         :type memory_gb: float
+        :param enable_app_insights: Whether or not to enable Application Insights logging for this Webservice.
+            Defaults to False.
+        :type enable_app_insights: bool
         :param scoring_timeout_ms: A timeout to enforce for scoring calls to this Webservice
         :type scoring_timeout_ms: int
         :param replica_max_concurrent_requests: The number of maximum concurrent requests per replica to allow for this
             Webservice.
         :type replica_max_concurrent_requests: int
         :param num_replicas: The number of containers to allocate for this Webservice
         :type num_replicas: int
@@ -402,16 +415,16 @@
         properties = super(MirWebservice, self).serialize()
         autoscaler = self.autoscaler.serialize() if self.autoscaler else None
         container_resource_requirements = self.container_resource_requirements.serialize() \
             if self.container_resource_requirements else None
         data_collection = self.data_collection.serialize() if self.data_collection else None
         image = self.image.serialize() if self.image else None
         deployment_status = self.deployment_status.serialize() if self.deployment_status else None
-        mir_properties = {'autoScaler': autoscaler, 'computeName': self.compute_name,
-                          'authEnabled': self.auth_enabled,
+        mir_properties = {'appInsightsEnabled': self.enable_app_insights, 'autoScaler': autoscaler,
+                          'computeName': self.compute_name, 'authEnabled': self.auth_enabled,
                           'containerResourceRequirements': container_resource_requirements,
                           'dataCollection': data_collection, 'imageId': self.image_id,
                           'imageDetails': image,
                           'maxConcurrentRequestsPerContainer': self.max_concurrent_requests_per_container,
                           'numReplicas': self.num_replicas, 'deploymentStatus': deployment_status,
                           'scoringTimeoutMs': self.scoring_timeout_ms, 'scoringUri': self.scoring_uri,
                           'tlsMode': self.tls_mode, 'certificateFingerprints': self.certificate_fingerprints,
@@ -484,14 +497,17 @@
     :param cpu_cores: The number of cpu cores to allocate for this Webservice. Can be a decimal. Defaults to 0.1
     :type cpu_cores: float
     :param memory_gb: The amount of memory (in GB) to allocate for this Webservice. Can be a decimal.
         Defaults to 0.5
     :type memory_gb: float
     :param scoring_timeout_ms: A timeout to enforce for scoring calls to this Webservice. Defaults to 60000
     :type scoring_timeout_ms: int
+    :param enable_app_insights: Whether or not to enable Application Insights logging for this Webservice.
+        Defaults to False
+    :type enable_app_insights: bool
     :param replica_max_concurrent_requests: The number of maximum concurrent requests per node to allow for this
         Webservice. Defaults to 1
     :type replica_max_concurrent_requests: int
     :param num_replicas: The number of containers to allocate for this Webservice. No default, if this parameter
         is not set then the autoscaler is enabled by default.
     :type num_replicas: int
     :param tags: Dictionary of key value tags to give this Webservice
@@ -515,15 +531,15 @@
     """
 
     def __init__(self, autoscale_enabled=None, autoscale_min_replicas=None, autoscale_max_replicas=None,
                  autoscale_refresh_seconds=None, autoscale_target_utilization=None, collect_model_data=None,
                  auth_enabled=None, cpu_cores=None, memory_gb=None, scoring_timeout_ms=None,
                  replica_max_concurrent_requests=None, max_request_wait_time=None, num_replicas=None, tags=None,
                  properties=None, description=None, tls_mode=None, certificate_fingerprints=None, sku=None,
-                 gpu_cores=None, osType=None):
+                 gpu_cores=None, osType=None, enable_app_insights=None):
         """Initialize a configuration object for deploying to an MIR compute target.
 
         :param autoscale_enabled: Whether or not to enable autoscaling for this Webservice.
             Defaults to True if num_replicas is None
         :type autoscale_enabled: bool
         :param autoscale_min_replicas: The minimum number of containers to use when autoscaling this Webservice.
             Defaults to 1
@@ -569,14 +585,17 @@
         :type certificate_fingerprints: :class:`list[str]`
         :param sku: Azure SKU type for MIR compute
         :type sku: str
         :param gpu_cores: The number of gpu cores to allocate for this Webservice. Defaults to 1
         :type gpu_cores: int
         :param osType: OS type of the mir service, valid options are "Linux", "Windows"
         :type osType: str
+        :param enable_app_insights: Whether or not to enable Application Insights logging for this Webservice.
+            Defaults to False
+        :type enable_app_insights: bool
         :return: A configuration object to use when deploying a Webservice object.
         :raises: azureml.exceptions.WebserviceException
         """
         super(MirServiceDeploymentConfiguration, self).__init__(MirWebservice)
         self.autoscale_enabled = autoscale_enabled
         self.autoscale_min_replicas = autoscale_min_replicas
         self.autoscale_max_replicas = autoscale_max_replicas
@@ -594,14 +613,15 @@
         self.properties = properties
         self.description = description
         self.tls_mode = tls_mode
         self.certificate_fingerprints = certificate_fingerprints
         self.sku = sku
         self.gpu_cores = gpu_cores
         self.osType = osType
+        self.enable_app_insights = enable_app_insights
         self.validate_configuration()
 
     def validate_configuration(self):
         """Check that the specified configuration values are valid.
 
         Will raise a WebserviceException if validation fails.
 
@@ -656,20 +676,23 @@
         json_payload['maxConcurrentRequestsPerContainer'] = self.replica_max_concurrent_requests
         json_payload['maxQueueWaitMs'] = self.max_request_wait_time
         json_payload['scoringTimeoutMs'] = self.scoring_timeout_ms
         json_payload['tlsMode'] = self.tls_mode
         json_payload['certificateFingerprints'] = self.certificate_fingerprints
         json_payload['sku'] = self.sku
         json_payload['osType'] = self.osType
+        if self.enable_app_insights is not None:
+            json_payload['appInsightsEnabled'] = self.enable_app_insights
+        else:
+            del(json_payload['appInsightsEnabled'])
 
         if self.gpu_cores:
             json_payload['containerResourceRequirements']['gpu'] = self.gpu_cores
         else:
             del (json_payload['containerResourceRequirements']['gpu'])
-
         if overwrite:
             json_payload['overwrite'] = overwrite
         else:
             del (json_payload['overwrite'])
 
         json_payload.update(base_payload)
```

## azureml/contrib/mir/webservice/data/mir_service_payload_template.json

### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'appInsightsEnabled'": 'None'}*

```diff
@@ -1,8 +1,9 @@
 {
+    "appInsightsEnabled": null,
     "authEnabled": false,
     "autoScaler": {
         "autoscaleEnabled": false,
         "maxReplicas": null,
         "minReplicas": null,
         "refreshPeriodInSeconds": null,
         "targetUtilization": null
```

## Comparing `azureml_contrib_mir-1.8.0.dist-info/LICENSE.txt` & `azureml_contrib_mir-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_contrib_mir-1.8.0.dist-info/metadata.json` & `azureml_contrib_mir-1.9.0.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9318181818181818%*

 * *Differences: {"'run_requires'": "{0: {'requires': ['azureml-core (~=1.9.0)']}}", "'version'": "'1.9.0'"}*

```diff
@@ -22,14 +22,14 @@
     "license": "Proprietary https://aka.ms/azureml-preview-sdk-license ",
     "metadata_version": "2.0",
     "name": "azureml-contrib-mir",
     "requires_python": ">=3.5,<4",
     "run_requires": [
         {
             "requires": [
-                "azureml-core (~=1.8.0)"
+                "azureml-core (~=1.9.0)"
             ]
         }
     ],
     "summary": "Azure Machine Learning MIR",
-    "version": "1.8.0"
+    "version": "1.9.0"
 }
```

## Comparing `azureml_contrib_mir-1.8.0.dist-info/RECORD` & `azureml_contrib_mir-1.9.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 azureml/__init__.py,sha256=n0xtZ3iWcoVg5Qognsb7InYAUVAK8s3iaVeHB5GOaNA,251
 azureml/contrib/__init__.py,sha256=n0xtZ3iWcoVg5Qognsb7InYAUVAK8s3iaVeHB5GOaNA,251
 azureml/contrib/_mircli/__init__.py,sha256=JlCCObuOLZyNhIZlsoL51KtFxiY4xKIIzIRDBcdeu6Y,183
-azureml/contrib/_mircli/_cli.py,sha256=KizUwutDRhkhI7SJOG46KmVYyDxUQPMd5n0bvacgsfs,13179
-azureml/contrib/_mircli/_util.py,sha256=Th056UoncbHZ7FmQSNTulSrR2rAZRXtKmIUMJetgag0,42146
+azureml/contrib/_mircli/_cli.py,sha256=LgR60PNwjYS3G4eKAQbBMqJ5KlHtir79otfUEywMgak,13215
+azureml/contrib/_mircli/_util.py,sha256=Oh2SWLRx7vskGlHWC8wWKeB3sKnLQbS4qnucPguX1ns,42623
 azureml/contrib/mir/__init__.py,sha256=OwKQJqaC9EvGbWd281xGLTy8xV9gPinbZe6dEEDVkfo,347
 azureml/contrib/mir/webservice/__init__.py,sha256=BZQjerPNa196b6nPCdfvZ1BFqFE496UBDjvub-w06Ww,441
 azureml/contrib/mir/webservice/_util.py,sha256=IweSfU-mME7pXDEj2Z_usiDfNB641pdTa3aasEtxgaI,385
-azureml/contrib/mir/webservice/mir.py,sha256=ppLK1MZyYf_LB6DQhEyKfSeV62ySHVZN6NQzdypQP7c,41992
-azureml/contrib/mir/webservice/data/mir_service_payload_template.json,sha256=jM3uLYBrbkaYUgM9k3X_MRMMQMLRrP1BktAKGF-Ys_o,761
-azureml_contrib_mir-1.8.0.dist-info/DESCRIPTION.rst,sha256=ONrclgD5z0CzXpW70uAh1cdOs0tUieTWwvba7vUBpdY,23
-azureml_contrib_mir-1.8.0.dist-info/LICENSE.txt,sha256=FOfkEEz4uS7g278F9Rq12rqKF3lLyBUZhVpLetuZrTg,1021
-azureml_contrib_mir-1.8.0.dist-info/METADATA,sha256=CrjIeoBtfEvLuJ81A9GYuq7PvZFLs3peo-yR519ODl0,406
-azureml_contrib_mir-1.8.0.dist-info/RECORD,,
-azureml_contrib_mir-1.8.0.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
-azureml_contrib_mir-1.8.0.dist-info/metadata.json,sha256=NYI8YJrXx4KhaPBcfi6YNenemXsA4iiCTgON3_xAnpY,643
-azureml_contrib_mir-1.8.0.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
+azureml/contrib/mir/webservice/mir.py,sha256=NggbzjpdDOYG8aBgutlbPEBxmcEPF1EiUUTrgxDxAzI,43605
+azureml/contrib/mir/webservice/data/mir_service_payload_template.json,sha256=RSij7s5JdhjTJ331wMHrutVVdfUV6-7E4tJ7ZbIBPoQ,792
+azureml_contrib_mir-1.9.0.dist-info/DESCRIPTION.rst,sha256=ONrclgD5z0CzXpW70uAh1cdOs0tUieTWwvba7vUBpdY,23
+azureml_contrib_mir-1.9.0.dist-info/LICENSE.txt,sha256=FOfkEEz4uS7g278F9Rq12rqKF3lLyBUZhVpLetuZrTg,1021
+azureml_contrib_mir-1.9.0.dist-info/METADATA,sha256=Iyn_A8HQwTzWai3TrM7Z47cXwH3Ge3_SQ7b3Yy4022Q,406
+azureml_contrib_mir-1.9.0.dist-info/RECORD,,
+azureml_contrib_mir-1.9.0.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
+azureml_contrib_mir-1.9.0.dist-info/metadata.json,sha256=xPvG41IZxOr7vQ4cW-Fjen82tjryUk3UPWkMzWyNTDw,643
+azureml_contrib_mir-1.9.0.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
```


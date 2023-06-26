# Comparing `tmp/convocations-0.8.tar.gz` & `tmp/convocations-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convocations-0.8.tar", last modified: Thu Feb 23 23:07:13 2023, max compression
+gzip compressed data, was "convocations-0.9.tar", last modified: Sat Feb 25 00:44:02 2023, max compression
```

## Comparing `convocations-0.8.tar` & `convocations-0.9.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.832342 convocations-0.8/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      418 2023-02-12 23:27:56.000000 convocations-0.8/MANIFEST.in
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5291 2023-02-23 23:07:13.832342 convocations-0.8/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3893 2023-02-12 05:51:10.000000 convocations-0.8/README.md
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       14 2023-02-12 05:51:10.000000 convocations-0.8/airflow.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       50 2023-02-12 05:51:10.000000 convocations-0.8/aws.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       13 2023-02-12 05:51:10.000000 convocations-0.8/certs.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       92 2023-02-12 05:51:10.000000 convocations-0.8/checkpoint.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.812341 convocations-0.8/convocations/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2022-06-26 20:52:06.000000 convocations-0.8/convocations/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.812341 convocations-0.8/convocations/airflow/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5048 2023-02-19 03:44:09.000000 convocations-0.8/convocations/airflow/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.812341 convocations-0.8/convocations/aws/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1722 2023-02-12 23:19:10.000000 convocations-0.8/convocations/aws/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     7715 2023-02-12 22:46:21.000000 convocations-0.8/convocations/aws/ami_helpers.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    20035 2023-02-15 20:43:58.000000 convocations-0.8/convocations/aws/base.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.812341 convocations-0.8/convocations/aws/cfn/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/cfn/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5507 2023-02-23 22:51:11.000000 convocations-0.8/convocations/aws/cfn/import_code_pipeline.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     9133 2023-02-12 23:02:41.000000 convocations-0.8/convocations/aws/cfn/import_ecs_service.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3476 2023-02-12 23:02:52.000000 convocations-0.8/convocations/aws/cfn/import_instance.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4209 2023-02-12 23:01:06.000000 convocations-0.8/convocations/aws/cfn/import_resource_to_cfn.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1666 2023-02-12 23:04:48.000000 convocations-0.8/convocations/aws/cfn/import_route_table.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4213 2023-02-12 23:03:21.000000 convocations-0.8/convocations/aws/cfn/import_security_group.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3008 2023-02-12 23:03:32.000000 convocations-0.8/convocations/aws/cfn/import_subnet.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2210 2023-02-12 23:03:47.000000 convocations-0.8/convocations/aws/cfn/import_vpc.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    23778 2023-02-23 00:06:41.000000 convocations-0.8/convocations/aws/cfn/stack_commands.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.812341 convocations-0.8/convocations/aws/cloudwatch/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      788 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/cloudwatch/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.812341 convocations-0.8/convocations/aws/codebuild/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      615 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/codebuild/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    13433 2023-02-16 08:24:40.000000 convocations-0.8/convocations/aws/codebuild/build.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      168 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/codebuild/detect.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.812341 convocations-0.8/convocations/aws/codedeploy/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3332 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/codedeploy/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.812341 convocations-0.8/convocations/aws/ec2/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    13714 2023-02-16 02:33:12.000000 convocations-0.8/convocations/aws/ec2/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      327 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/ec2/detect.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1301 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/ec2/routing.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3091 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/ec2/ssh.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.812341 convocations-0.8/convocations/aws/ecs/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2091 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/ecs/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.812341 convocations-0.8/convocations/aws/elb/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     8604 2023-02-16 02:21:32.000000 convocations-0.8/convocations/aws/elb/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.812341 convocations-0.8/convocations/aws/iam/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2005 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/iam/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2999 2023-02-14 07:16:22.000000 convocations-0.8/convocations/aws/keypairs.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/aws/mgn/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       40 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/mgn/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2138 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/mgn/launch.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/aws/open_id/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      657 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/open_id/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/aws/organizations/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     8587 2023-02-23 20:21:22.000000 convocations-0.8/convocations/aws/organizations/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/aws/ram/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1311 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/ram/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/aws/rds/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      740 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/rds/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/aws/reservations/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)    13764 2023-02-12 23:11:49.000000 convocations-0.8/convocations/aws/reservations/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/aws/route53/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      949 2023-02-15 18:40:19.000000 convocations-0.8/convocations/aws/route53/__init__.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3704 2023-02-12 23:00:23.000000 convocations-0.8/convocations/aws/route53/zone_parser.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/aws/s3/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1978 2023-02-12 22:44:18.000000 convocations-0.8/convocations/aws/s3/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/aws/ssm/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/ssm/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1777 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/ssm/runners.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/aws/transit_gateway/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5828 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/transit_gateway/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/aws/vpc_peering/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      615 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/vpc_peering/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      560 2023-02-12 05:51:10.000000 convocations-0.8/convocations/aws/wait_helpers.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/base/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2022-07-28 05:52:21.000000 convocations-0.8/convocations/base/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1739 2022-07-28 06:11:51.000000 convocations-0.8/convocations/base/projects.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     6467 2023-02-15 15:29:58.000000 convocations-0.8/convocations/base/utils.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/certs/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      115 2023-02-12 05:51:10.000000 convocations-0.8/convocations/certs/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2678 2023-02-12 05:51:10.000000 convocations-0.8/convocations/certs/validator.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/checkpoint/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      310 2023-02-12 05:51:10.000000 convocations-0.8/convocations/checkpoint/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1082 2023-02-12 05:51:10.000000 convocations-0.8/convocations/checkpoint/base.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      507 2023-02-12 05:51:10.000000 convocations-0.8/convocations/checkpoint/layers.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      648 2023-02-12 05:51:10.000000 convocations-0.8/convocations/checkpoint/objects.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2859 2023-02-12 05:51:10.000000 convocations-0.8/convocations/checkpoint/services.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      433 2023-02-12 05:51:10.000000 convocations-0.8/convocations/checkpoint/versions.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/docker/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      139 2022-12-29 15:16:06.000000 convocations-0.8/convocations/docker/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1021 2023-02-12 05:51:10.000000 convocations-0.8/convocations/docker/template.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.832342 convocations-0.8/convocations/docker/templates/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      188 2022-12-29 15:16:06.000000 convocations-0.8/convocations/docker/templates/.bumpversion.cfg
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2022-12-29 15:16:06.000000 convocations-0.8/convocations/docker/templates/.dockerignore
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       22 2022-12-29 15:16:06.000000 convocations-0.8/convocations/docker/templates/.gitignore
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       52 2022-12-29 15:16:06.000000 convocations-0.8/convocations/docker/templates/Dockerfile
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      364 2022-12-29 15:16:06.000000 convocations-0.8/convocations/docker/templates/Makefile
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      146 2022-12-29 15:16:06.000000 convocations-0.8/convocations/docker/templates/README.md
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      696 2023-02-12 05:51:10.000000 convocations-0.8/convocations/docker/templates/buildspec.yml
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       17 2022-12-29 15:16:06.000000 convocations-0.8/convocations/docker/templates/requirements.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/docker/templates/tasks/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      134 2022-12-29 15:16:06.000000 convocations-0.8/convocations/docker/templates/tasks/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2245 2023-02-12 05:51:10.000000 convocations-0.8/convocations/docker/templates/tasks/build.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        3 2022-12-29 15:16:06.000000 convocations-0.8/convocations/docker/templates/version.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/o365/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-12 05:51:10.000000 convocations-0.8/convocations/o365/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1032 2023-02-12 06:13:27.000000 convocations-0.8/convocations/o365/imap.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/onelogin/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      124 2023-02-12 05:51:10.000000 convocations-0.8/convocations/onelogin/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      718 2023-02-12 05:51:10.000000 convocations-0.8/convocations/onelogin/base.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1094 2023-02-12 05:51:10.000000 convocations-0.8/convocations/onelogin/users.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/palo_alto/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      327 2023-02-12 05:51:10.000000 convocations-0.8/convocations/palo_alto/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4477 2023-02-12 05:51:10.000000 convocations-0.8/convocations/palo_alto/base.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1064 2023-02-12 05:51:10.000000 convocations-0.8/convocations/palo_alto/certificates.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1723 2023-02-12 05:51:10.000000 convocations-0.8/convocations/palo_alto/save_config.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2646 2023-02-12 05:51:10.000000 convocations-0.8/convocations/palo_alto/upgrade.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1542 2023-02-12 05:51:10.000000 convocations-0.8/convocations/palo_alto/weird.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/pypi/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1644 2023-02-19 03:46:53.000000 convocations-0.8/convocations/pypi/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      182 2022-06-27 01:50:00.000000 convocations-0.8/convocations/pypi/program.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.832342 convocations-0.8/convocations/pypi/templates/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      198 2022-07-28 05:30:08.000000 convocations-0.8/convocations/pypi/templates/.bumpversion.cfg
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       22 2022-06-26 14:34:11.000000 convocations-0.8/convocations/pypi/templates/.coveragerc
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1176 2022-06-25 16:57:20.000000 convocations-0.8/convocations/pypi/templates/.gitignore
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       86 2022-07-29 04:27:10.000000 convocations-0.8/convocations/pypi/templates/MANIFEST.in
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      779 2022-07-09 03:40:43.000000 convocations-0.8/convocations/pypi/templates/Makefile
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       13 2022-06-26 21:05:51.000000 convocations-0.8/convocations/pypi/templates/README.md
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       80 2023-02-19 03:45:43.000000 convocations-0.8/convocations/pypi/templates/dev.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       66 2022-06-25 15:04:19.000000 convocations-0.8/convocations/pypi/templates/pytest.ini
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       11 2022-06-26 20:54:41.000000 convocations-0.8/convocations/pypi/templates/requirements.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/pypi/templates/sesame_meow_cat/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2022-07-28 05:37:53.000000 convocations-0.8/convocations/pypi/templates/sesame_meow_cat/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        3 2022-07-28 05:30:20.000000 convocations-0.8/convocations/pypi/templates/sesame_meow_cat/version.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2390 2022-07-28 05:31:23.000000 convocations-0.8/convocations/pypi/templates/setup.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.822341 convocations-0.8/convocations/pypi/templates/test/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2022-07-28 05:37:42.000000 convocations-0.8/convocations/pypi/templates/test/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       16 2022-06-26 21:02:59.000000 convocations-0.8/convocations/pypi/templates/test/conftest.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.832342 convocations-0.8/convocations/python/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      195 2023-02-19 03:39:01.000000 convocations-0.8/convocations/python/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1529 2023-02-19 03:39:47.000000 convocations-0.8/convocations/python/pytest.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     2562 2023-02-19 03:40:21.000000 convocations-0.8/convocations/python/setup.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.832342 convocations-0.8/convocations/sharepoint/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      319 2023-02-12 05:51:10.000000 convocations-0.8/convocations/sharepoint/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1413 2022-07-28 06:18:11.000000 convocations-0.8/convocations/sharepoint/files.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4138 2023-02-12 05:51:10.000000 convocations-0.8/convocations/sharepoint/permissions.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.832342 convocations-0.8/convocations/snobby/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1888 2023-02-13 21:06:04.000000 convocations-0.8/convocations/snobby/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.832342 convocations-0.8/convocations/tundra/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      407 2023-02-12 05:51:10.000000 convocations-0.8/convocations/tundra/__init__.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5400 2023-02-15 17:18:10.000000 convocations-0.8/convocations/tundra/codebuild.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3409 2023-02-15 07:02:16.000000 convocations-0.8/convocations/tundra/deploy.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1952 2023-02-12 05:51:10.000000 convocations-0.8/convocations/tundra/docker.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1792 2023-02-12 05:51:10.000000 convocations-0.8/convocations/tundra/ecs.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      640 2023-02-12 05:51:10.000000 convocations-0.8/convocations/tundra/frontend.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1014 2023-02-12 05:51:10.000000 convocations-0.8/convocations/tundra/template.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.832342 convocations-0.8/convocations/tundra/templates/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      316 2022-12-29 15:16:06.000000 convocations-0.8/convocations/tundra/templates/Makefile
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       79 2022-12-29 15:16:06.000000 convocations-0.8/convocations/tundra/templates/README.md
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4930 2023-02-12 05:51:10.000000 convocations-0.8/convocations/tundra/utils.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1673 2023-02-12 05:51:10.000000 convocations-0.8/convocations/tundra/waiters.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       16 2023-02-23 23:07:03.000000 convocations-0.8/convocations/version.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-23 23:07:13.832342 convocations-0.8/convocations.egg-info/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5291 2023-02-23 23:07:13.000000 convocations-0.8/convocations.egg-info/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     5554 2023-02-23 23:07:13.000000 convocations-0.8/convocations.egg-info/SOURCES.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-02-23 23:07:13.000000 convocations-0.8/convocations.egg-info/dependency_links.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      120 2023-02-23 23:07:13.000000 convocations-0.8/convocations.egg-info/entry_points.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     1004 2023-02-23 23:07:13.000000 convocations-0.8/convocations.egg-info/requires.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       13 2023-02-23 23:07:13.000000 convocations-0.8/convocations.egg-info/top_level.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      239 2023-02-12 05:51:10.000000 convocations-0.8/dev.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        9 2023-02-12 05:51:10.000000 convocations-0.8/onelogin.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       48 2023-02-12 05:51:10.000000 convocations-0.8/palo_alto.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      117 2023-02-18 21:08:34.000000 convocations-0.8/requirements.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2023-02-23 23:07:13.832342 convocations-0.8/setup.cfg
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     3245 2023-02-23 23:07:03.000000 convocations-0.8/setup.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       39 2023-02-12 05:51:10.000000 convocations-0.8/sharepoint.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        6 2023-02-12 05:51:10.000000 convocations-0.8/tundra.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.257481 convocations-0.9/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      418 2023-02-12 23:27:56.000000 convocations-0.9/MANIFEST.in
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5291 2023-02-25 00:44:02.257481 convocations-0.9/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3893 2023-02-12 05:51:10.000000 convocations-0.9/README.md
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       14 2023-02-12 05:51:10.000000 convocations-0.9/airflow.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       50 2023-02-12 05:51:10.000000 convocations-0.9/aws.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       13 2023-02-12 05:51:10.000000 convocations-0.9/certs.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       92 2023-02-12 05:51:10.000000 convocations-0.9/checkpoint.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.237481 convocations-0.9/convocations/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2022-06-26 20:52:06.000000 convocations-0.9/convocations/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.237481 convocations-0.9/convocations/airflow/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5048 2023-02-19 03:44:09.000000 convocations-0.9/convocations/airflow/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.237481 convocations-0.9/convocations/aws/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1722 2023-02-12 23:19:10.000000 convocations-0.9/convocations/aws/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     7715 2023-02-12 22:46:21.000000 convocations-0.9/convocations/aws/ami_helpers.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    20035 2023-02-15 20:43:58.000000 convocations-0.9/convocations/aws/base.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.237481 convocations-0.9/convocations/aws/cfn/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/cfn/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5507 2023-02-23 22:51:11.000000 convocations-0.9/convocations/aws/cfn/import_code_pipeline.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     9133 2023-02-12 23:02:41.000000 convocations-0.9/convocations/aws/cfn/import_ecs_service.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3476 2023-02-12 23:02:52.000000 convocations-0.9/convocations/aws/cfn/import_instance.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4209 2023-02-12 23:01:06.000000 convocations-0.9/convocations/aws/cfn/import_resource_to_cfn.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1666 2023-02-12 23:04:48.000000 convocations-0.9/convocations/aws/cfn/import_route_table.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4213 2023-02-12 23:03:21.000000 convocations-0.9/convocations/aws/cfn/import_security_group.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3008 2023-02-12 23:03:32.000000 convocations-0.9/convocations/aws/cfn/import_subnet.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2210 2023-02-12 23:03:47.000000 convocations-0.9/convocations/aws/cfn/import_vpc.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    23778 2023-02-23 00:06:41.000000 convocations-0.9/convocations/aws/cfn/stack_commands.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/cloudwatch/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      788 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/cloudwatch/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/codebuild/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      615 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/codebuild/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    13433 2023-02-16 08:24:40.000000 convocations-0.9/convocations/aws/codebuild/build.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      168 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/codebuild/detect.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/codedeploy/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3332 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/codedeploy/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/ec2/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    13714 2023-02-16 02:33:12.000000 convocations-0.9/convocations/aws/ec2/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      327 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/ec2/detect.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1301 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/ec2/routing.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3091 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/ec2/ssh.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/ecs/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2091 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/ecs/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/elb/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     8604 2023-02-16 02:21:32.000000 convocations-0.9/convocations/aws/elb/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/iam/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2005 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/iam/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2999 2023-02-14 07:16:22.000000 convocations-0.9/convocations/aws/keypairs.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/mgn/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       40 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/mgn/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2138 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/mgn/launch.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/open_id/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      657 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/open_id/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/organizations/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     8587 2023-02-23 20:21:22.000000 convocations-0.9/convocations/aws/organizations/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/ram/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1311 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/ram/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/rds/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      740 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/rds/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/reservations/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)    13764 2023-02-12 23:11:49.000000 convocations-0.9/convocations/aws/reservations/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/route53/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      949 2023-02-15 18:40:19.000000 convocations-0.9/convocations/aws/route53/__init__.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3704 2023-02-12 23:00:23.000000 convocations-0.9/convocations/aws/route53/zone_parser.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/s3/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1978 2023-02-12 22:44:18.000000 convocations-0.9/convocations/aws/s3/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/ssm/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/ssm/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1777 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/ssm/runners.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/transit_gateway/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5828 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/transit_gateway/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/aws/vpc_peering/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      615 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/vpc_peering/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      560 2023-02-12 05:51:10.000000 convocations-0.9/convocations/aws/wait_helpers.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/base/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2022-07-28 05:52:21.000000 convocations-0.9/convocations/base/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1739 2022-07-28 06:11:51.000000 convocations-0.9/convocations/base/projects.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     6467 2023-02-15 15:29:58.000000 convocations-0.9/convocations/base/utils.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/certs/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      115 2023-02-12 05:51:10.000000 convocations-0.9/convocations/certs/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2678 2023-02-12 05:51:10.000000 convocations-0.9/convocations/certs/validator.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/checkpoint/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      310 2023-02-12 05:51:10.000000 convocations-0.9/convocations/checkpoint/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1082 2023-02-12 05:51:10.000000 convocations-0.9/convocations/checkpoint/base.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      507 2023-02-12 05:51:10.000000 convocations-0.9/convocations/checkpoint/layers.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      648 2023-02-12 05:51:10.000000 convocations-0.9/convocations/checkpoint/objects.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2859 2023-02-12 05:51:10.000000 convocations-0.9/convocations/checkpoint/services.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      433 2023-02-12 05:51:10.000000 convocations-0.9/convocations/checkpoint/versions.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/docker/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      139 2022-12-29 15:16:06.000000 convocations-0.9/convocations/docker/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1021 2023-02-12 05:51:10.000000 convocations-0.9/convocations/docker/template.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.257481 convocations-0.9/convocations/docker/templates/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      188 2022-12-29 15:16:06.000000 convocations-0.9/convocations/docker/templates/.bumpversion.cfg
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2022-12-29 15:16:06.000000 convocations-0.9/convocations/docker/templates/.dockerignore
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       22 2022-12-29 15:16:06.000000 convocations-0.9/convocations/docker/templates/.gitignore
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       52 2022-12-29 15:16:06.000000 convocations-0.9/convocations/docker/templates/Dockerfile
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      364 2022-12-29 15:16:06.000000 convocations-0.9/convocations/docker/templates/Makefile
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      146 2022-12-29 15:16:06.000000 convocations-0.9/convocations/docker/templates/README.md
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      696 2023-02-12 05:51:10.000000 convocations-0.9/convocations/docker/templates/buildspec.yml
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       17 2022-12-29 15:16:06.000000 convocations-0.9/convocations/docker/templates/requirements.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/docker/templates/tasks/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      134 2022-12-29 15:16:06.000000 convocations-0.9/convocations/docker/templates/tasks/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2245 2023-02-12 05:51:10.000000 convocations-0.9/convocations/docker/templates/tasks/build.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        3 2022-12-29 15:16:06.000000 convocations-0.9/convocations/docker/templates/version.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/o365/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2023-02-12 05:51:10.000000 convocations-0.9/convocations/o365/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1032 2023-02-12 06:13:27.000000 convocations-0.9/convocations/o365/imap.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/onelogin/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      124 2023-02-12 05:51:10.000000 convocations-0.9/convocations/onelogin/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      718 2023-02-12 05:51:10.000000 convocations-0.9/convocations/onelogin/base.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1094 2023-02-12 05:51:10.000000 convocations-0.9/convocations/onelogin/users.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/palo_alto/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      327 2023-02-12 05:51:10.000000 convocations-0.9/convocations/palo_alto/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4477 2023-02-12 05:51:10.000000 convocations-0.9/convocations/palo_alto/base.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1064 2023-02-12 05:51:10.000000 convocations-0.9/convocations/palo_alto/certificates.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1723 2023-02-12 05:51:10.000000 convocations-0.9/convocations/palo_alto/save_config.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2646 2023-02-12 05:51:10.000000 convocations-0.9/convocations/palo_alto/upgrade.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1542 2023-02-12 05:51:10.000000 convocations-0.9/convocations/palo_alto/weird.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/pypi/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1644 2023-02-19 03:46:53.000000 convocations-0.9/convocations/pypi/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      182 2022-06-27 01:50:00.000000 convocations-0.9/convocations/pypi/program.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.257481 convocations-0.9/convocations/pypi/templates/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      198 2022-07-28 05:30:08.000000 convocations-0.9/convocations/pypi/templates/.bumpversion.cfg
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       22 2022-06-26 14:34:11.000000 convocations-0.9/convocations/pypi/templates/.coveragerc
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1176 2022-06-25 16:57:20.000000 convocations-0.9/convocations/pypi/templates/.gitignore
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       86 2022-07-29 04:27:10.000000 convocations-0.9/convocations/pypi/templates/MANIFEST.in
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      779 2022-07-09 03:40:43.000000 convocations-0.9/convocations/pypi/templates/Makefile
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       13 2022-06-26 21:05:51.000000 convocations-0.9/convocations/pypi/templates/README.md
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       80 2023-02-19 03:45:43.000000 convocations-0.9/convocations/pypi/templates/dev.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       66 2022-06-25 15:04:19.000000 convocations-0.9/convocations/pypi/templates/pytest.ini
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       11 2022-06-26 20:54:41.000000 convocations-0.9/convocations/pypi/templates/requirements.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/pypi/templates/sesame_meow_cat/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2022-07-28 05:37:53.000000 convocations-0.9/convocations/pypi/templates/sesame_meow_cat/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        3 2022-07-28 05:30:20.000000 convocations-0.9/convocations/pypi/templates/sesame_meow_cat/version.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2390 2022-07-28 05:31:23.000000 convocations-0.9/convocations/pypi/templates/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/pypi/templates/test/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        0 2022-07-28 05:37:42.000000 convocations-0.9/convocations/pypi/templates/test/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       16 2022-06-26 21:02:59.000000 convocations-0.9/convocations/pypi/templates/test/conftest.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.247481 convocations-0.9/convocations/python/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      195 2023-02-19 03:39:01.000000 convocations-0.9/convocations/python/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1529 2023-02-19 03:39:47.000000 convocations-0.9/convocations/python/pytest.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     2562 2023-02-19 03:40:21.000000 convocations-0.9/convocations/python/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.257481 convocations-0.9/convocations/sharepoint/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      319 2023-02-12 05:51:10.000000 convocations-0.9/convocations/sharepoint/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1413 2022-07-28 06:18:11.000000 convocations-0.9/convocations/sharepoint/files.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4138 2023-02-12 05:51:10.000000 convocations-0.9/convocations/sharepoint/permissions.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.257481 convocations-0.9/convocations/snobby/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1888 2023-02-13 21:06:04.000000 convocations-0.9/convocations/snobby/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.257481 convocations-0.9/convocations/tundra/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      407 2023-02-12 05:51:10.000000 convocations-0.9/convocations/tundra/__init__.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5400 2023-02-15 17:18:10.000000 convocations-0.9/convocations/tundra/codebuild.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3439 2023-02-24 20:42:43.000000 convocations-0.9/convocations/tundra/deploy.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1952 2023-02-12 05:51:10.000000 convocations-0.9/convocations/tundra/docker.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1792 2023-02-12 05:51:10.000000 convocations-0.9/convocations/tundra/ecs.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      640 2023-02-12 05:51:10.000000 convocations-0.9/convocations/tundra/frontend.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1014 2023-02-12 05:51:10.000000 convocations-0.9/convocations/tundra/template.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.257481 convocations-0.9/convocations/tundra/templates/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      316 2022-12-29 15:16:06.000000 convocations-0.9/convocations/tundra/templates/Makefile
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       79 2022-12-29 15:16:06.000000 convocations-0.9/convocations/tundra/templates/README.md
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4930 2023-02-12 05:51:10.000000 convocations-0.9/convocations/tundra/utils.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1673 2023-02-12 05:51:10.000000 convocations-0.9/convocations/tundra/waiters.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       16 2023-02-25 00:43:52.000000 convocations-0.9/convocations/version.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-25 00:44:02.257481 convocations-0.9/convocations.egg-info/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5291 2023-02-25 00:44:02.000000 convocations-0.9/convocations.egg-info/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     5554 2023-02-25 00:44:02.000000 convocations-0.9/convocations.egg-info/SOURCES.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-02-25 00:44:02.000000 convocations-0.9/convocations.egg-info/dependency_links.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      120 2023-02-25 00:44:02.000000 convocations-0.9/convocations.egg-info/entry_points.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     1004 2023-02-25 00:44:02.000000 convocations-0.9/convocations.egg-info/requires.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       13 2023-02-25 00:44:02.000000 convocations-0.9/convocations.egg-info/top_level.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      239 2023-02-12 05:51:10.000000 convocations-0.9/dev.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        9 2023-02-12 05:51:10.000000 convocations-0.9/onelogin.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       48 2023-02-12 05:51:10.000000 convocations-0.9/palo_alto.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      117 2023-02-18 21:08:34.000000 convocations-0.9/requirements.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       38 2023-02-25 00:44:02.257481 convocations-0.9/setup.cfg
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     3245 2023-02-25 00:43:52.000000 convocations-0.9/setup.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       39 2023-02-12 05:51:10.000000 convocations-0.9/sharepoint.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        6 2023-02-12 05:51:10.000000 convocations-0.9/tundra.txt
```

### Comparing `convocations-0.8/PKG-INFO` & `convocations-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convocations
-Version: 0.8
+Version: 0.9
 Summary: convocations
 Home-page: https://github.com/crazy-penguins/convocations
 Author: 2ps
 Author-email: pshingavi@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `convocations-0.8/README.md` & `convocations-0.9/README.md`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/airflow/__init__.py` & `convocations-0.9/convocations/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/__init__.py` & `convocations-0.9/convocations/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/ami_helpers.py` & `convocations-0.9/convocations/aws/ami_helpers.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/base.py` & `convocations-0.9/convocations/aws/base.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/cfn/import_code_pipeline.py` & `convocations-0.9/convocations/aws/cfn/import_code_pipeline.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/cfn/import_ecs_service.py` & `convocations-0.9/convocations/aws/cfn/import_ecs_service.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/cfn/import_instance.py` & `convocations-0.9/convocations/aws/cfn/import_instance.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/cfn/import_resource_to_cfn.py` & `convocations-0.9/convocations/aws/cfn/import_resource_to_cfn.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/cfn/import_route_table.py` & `convocations-0.9/convocations/aws/cfn/import_route_table.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/cfn/import_security_group.py` & `convocations-0.9/convocations/aws/cfn/import_security_group.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/cfn/import_subnet.py` & `convocations-0.9/convocations/aws/cfn/import_subnet.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/cfn/import_vpc.py` & `convocations-0.9/convocations/aws/cfn/import_vpc.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/cfn/stack_commands.py` & `convocations-0.9/convocations/aws/cfn/stack_commands.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/cloudwatch/__init__.py` & `convocations-0.9/convocations/aws/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/codebuild/__init__.py` & `convocations-0.9/convocations/aws/codebuild/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/codebuild/build.py` & `convocations-0.9/convocations/aws/codebuild/build.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/codedeploy/__init__.py` & `convocations-0.9/convocations/aws/codedeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/ec2/__init__.py` & `convocations-0.9/convocations/aws/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/ec2/routing.py` & `convocations-0.9/convocations/aws/ec2/routing.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/ec2/ssh.py` & `convocations-0.9/convocations/aws/ec2/ssh.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/ecs/__init__.py` & `convocations-0.9/convocations/aws/ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/elb/__init__.py` & `convocations-0.9/convocations/aws/elb/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/iam/__init__.py` & `convocations-0.9/convocations/aws/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/keypairs.py` & `convocations-0.9/convocations/aws/keypairs.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/mgn/launch.py` & `convocations-0.9/convocations/aws/mgn/launch.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/open_id/__init__.py` & `convocations-0.9/convocations/aws/open_id/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/organizations/__init__.py` & `convocations-0.9/convocations/aws/organizations/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/ram/__init__.py` & `convocations-0.9/convocations/aws/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/rds/__init__.py` & `convocations-0.9/convocations/aws/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/reservations/__init__.py` & `convocations-0.9/convocations/aws/reservations/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/route53/__init__.py` & `convocations-0.9/convocations/aws/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/route53/zone_parser.py` & `convocations-0.9/convocations/aws/route53/zone_parser.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/s3/__init__.py` & `convocations-0.9/convocations/aws/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/ssm/runners.py` & `convocations-0.9/convocations/aws/ssm/runners.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/transit_gateway/__init__.py` & `convocations-0.9/convocations/aws/transit_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/vpc_peering/__init__.py` & `convocations-0.9/convocations/aws/vpc_peering/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/aws/wait_helpers.py` & `convocations-0.9/convocations/aws/wait_helpers.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/base/projects.py` & `convocations-0.9/convocations/base/projects.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/base/utils.py` & `convocations-0.9/convocations/base/utils.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/certs/validator.py` & `convocations-0.9/convocations/certs/validator.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/checkpoint/base.py` & `convocations-0.9/convocations/checkpoint/base.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/checkpoint/objects.py` & `convocations-0.9/convocations/checkpoint/objects.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/checkpoint/services.py` & `convocations-0.9/convocations/checkpoint/services.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/docker/template.py` & `convocations-0.9/convocations/docker/template.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/docker/templates/buildspec.yml` & `convocations-0.9/convocations/docker/templates/buildspec.yml`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/docker/templates/tasks/build.py` & `convocations-0.9/convocations/docker/templates/tasks/build.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/o365/imap.py` & `convocations-0.9/convocations/o365/imap.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/onelogin/base.py` & `convocations-0.9/convocations/onelogin/base.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/onelogin/users.py` & `convocations-0.9/convocations/onelogin/users.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/palo_alto/base.py` & `convocations-0.9/convocations/palo_alto/base.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/palo_alto/certificates.py` & `convocations-0.9/convocations/palo_alto/certificates.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/palo_alto/save_config.py` & `convocations-0.9/convocations/palo_alto/save_config.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/palo_alto/upgrade.py` & `convocations-0.9/convocations/palo_alto/upgrade.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/palo_alto/weird.py` & `convocations-0.9/convocations/palo_alto/weird.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/pypi/__init__.py` & `convocations-0.9/convocations/pypi/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/pypi/templates/.gitignore` & `convocations-0.9/convocations/pypi/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/pypi/templates/Makefile` & `convocations-0.9/convocations/pypi/templates/Makefile`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/pypi/templates/setup.py` & `convocations-0.9/convocations/pypi/templates/setup.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/python/pytest.py` & `convocations-0.9/convocations/python/pytest.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/python/setup.py` & `convocations-0.9/convocations/python/setup.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/sharepoint/files.py` & `convocations-0.9/convocations/sharepoint/files.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/sharepoint/permissions.py` & `convocations-0.9/convocations/sharepoint/permissions.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/snobby/__init__.py` & `convocations-0.9/convocations/snobby/__init__.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/tundra/codebuild.py` & `convocations-0.9/convocations/tundra/codebuild.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/tundra/deploy.py` & `convocations-0.9/convocations/tundra/deploy.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'staging',
     'prod',
     'dags',
 ]
 
 
 @task(klass=AwsTask)
-def staging(ctx, limit=None, branch=None, profile=None, session=None):
+def staging(ctx, limit=None, branch=None, profile=None, session=None, **kwargs):
     """
     deploys to staging environment
     requires the following configuration:
 
     ```yaml
     aws:
       profile: profile_name
@@ -77,15 +77,15 @@
                 f'-e {key}="{value}"' for key, value in kwargs.items()
             ])
             ansible = f'{ansible} {extra}'
         ctx.run(ansible, pty=True)
 
 
 @task(klass=AwsTask)
-def flower(ctx, limit=None, profile=None, session=None):
+def flower(ctx, limit=None, profile=None, session=None, **kwargs):
     """
     deploys flower, requires the following configuration:
 
     ```yaml
     aws:
       profile: profile_name
     tundra:
@@ -101,15 +101,15 @@
     conf = ctx.tundra.deploy.flower
     playbook = conf.get('playbook', 'flower.yml')
     limit = limit or conf.limit
     _deploy(ctx, conf, limit, None, playbook, session=session)
 
 
 @task(klass=AwsTask)
-def dags(ctx, dag, limit=None, profile=None, session=None):
+def dags(ctx, dag, limit=None, profile=None, session=None, **kwargs):
     """
     pushes a specific dag from your local to the peaky / staging environment.
     this will overwrite any dags in these directories.
 
     requires the following context:
 
     ```yaml
```

### Comparing `convocations-0.8/convocations/tundra/docker.py` & `convocations-0.9/convocations/tundra/docker.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/tundra/ecs.py` & `convocations-0.9/convocations/tundra/ecs.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/tundra/frontend.py` & `convocations-0.9/convocations/tundra/frontend.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/tundra/template.py` & `convocations-0.9/convocations/tundra/template.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/tundra/utils.py` & `convocations-0.9/convocations/tundra/utils.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations/tundra/waiters.py` & `convocations-0.9/convocations/tundra/waiters.py`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations.egg-info/PKG-INFO` & `convocations-0.9/convocations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convocations
-Version: 0.8
+Version: 0.9
 Summary: convocations
 Home-page: https://github.com/crazy-penguins/convocations
 Author: 2ps
 Author-email: pshingavi@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `convocations-0.8/convocations.egg-info/SOURCES.txt` & `convocations-0.9/convocations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `convocations-0.8/convocations.egg-info/requires.txt` & `convocations-0.9/convocations.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 jinja2
 pyyaml
 termcolor
 colorama
 raft
 requests
 requests_oauthlib
-murmuration>=0.8
+murmuration>=0.9
 waddle>=1.1
 halo
 python-dateutil
 pytz
 
 [airflow]
 apache-airflow
```

### Comparing `convocations-0.8/setup.py` & `convocations-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Support setuptools only, distutils has a divergent and more annoying API and
 # few folks will lack setuptools.
 from setuptools import setup, find_packages
 from importlib.resources import open_text
 # Version info -- read without importing
 _locals = {}
 
-version = '0.8'
+version = '0.9'
 
 # PyYAML ships a split Python 2/3 codebase. Unfortunately, some pip versions
 # attempt to interpret both halves of PyYAML, yielding SyntaxErrors. Thus, we
 # exclude whichever appears inappropriate for the installing interpreter.
 exclude = ["*.yaml2", 'test']
 
 # Frankenstein long_description: version-specific changelog note + README
@@ -80,15 +80,15 @@
         'jinja2',
         'pyyaml',
         'termcolor',
         'colorama',
         'raft',
         'requests',
         'requests_oauthlib',
-        'murmuration>=0.8',
+        'murmuration>=0.9',
         'waddle>=1.1',
         'halo',
         'python-dateutil',
         'pytz',
     ],
     entry_points={
        'console_scripts': [
```


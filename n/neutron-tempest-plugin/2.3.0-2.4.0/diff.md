# Comparing `tmp/neutron-tempest-plugin-2.3.0.tar.gz` & `tmp/neutron-tempest-plugin-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutron-tempest-plugin-2.3.0.tar", last modified: Thu Apr 27 15:11:42 2023, max compression
+gzip compressed data, was "neutron-tempest-plugin-2.4.0.tar", last modified: Mon Jun 26 09:28:27 2023, max compression
```

## Comparing `neutron-tempest-plugin-2.3.0.tar` & `neutron-tempest-plugin-2.4.0.tar`

### file list

```diff
@@ -1,312 +1,312 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.790973 neutron-tempest-plugin-2.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7008 2023-04-27 15:11:42.000000 neutron-tempest-plugin-2.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43234 2023-04-27 15:11:42.000000 neutron-tempest-plugin-2.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1443 2023-04-27 15:11:42.790973 neutron-tempest-plugin-2.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.746972 neutron-tempest-plugin-2.3.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5198 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/devstack/customize_image.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3019 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/devstack/functions.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.746972 neutron-tempest-plugin-2.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.746972 neutron-tempest-plugin-2.3.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2600 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/doc/source/readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.750972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.758972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.762972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2190 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_agent_availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4585 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_agent_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_extension_driver_port_security_admin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12246 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_external_network_extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3418 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_floating_ips_admin_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3597 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_l3_agent_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4276 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2429 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_logging_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11860 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_network_segment_range.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4192 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11964 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_ports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6283 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7054 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_quotas_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4252 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_routers_dvr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4891 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_routers_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5179 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_routers_ha.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21527 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_shared_network_extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16723 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_tag.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    63450 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/base_routers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/base_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6437 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13901 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_address_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11743 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_address_scopes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_address_scopes_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5296 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_auto_allocated_topology.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1162 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6072 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_conntrack_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4030 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_dhcp_ipv6.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6679 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_extension_driver_port_security.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2235 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_extra_dhcp_options.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6897 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_flavors_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7691 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_floating_ips.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2546 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_floating_ips_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5852 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_local_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7288 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_metering_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_metering_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4923 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_ndp_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6210 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_ndp_proxy_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8764 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_network_ip_availability.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_network_ip_availability_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9208 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_networks_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4848 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_port_forwarding_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10876 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_port_forwardings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12069 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_ports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_ports_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    77821 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_qos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11965 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_qos_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20479 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_revisions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4948 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_router_interface_fip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22869 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_routers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7580 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_routers_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31264 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10498 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_security_groups_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_service_type_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3840 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_subnetpool_prefix_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26618 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_subnetpools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14768 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_subnetpools_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4536 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16121 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_timestamp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15374 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_trunk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2760 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_trunk_details.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13558 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_trunk_negative.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.762972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.762972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17284 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/api/test_bgpvpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3553 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.762972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6119 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/scenario/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62088 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/scenario/test_bgpvpn_basic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.766972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4809 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/services/bgpvpn_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.766972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6862 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16928 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6589 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11865 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/ssh.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/tempest_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8565 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11617 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3170 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.766972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.766972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/api/fwaas_v2_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14670 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/api/test_fwaasv2_extensions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.766972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7110 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/common/fwaas_v2_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.766972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2988 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2734 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13139 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/scenario/test_fwaas_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.766972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4681 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/services/v2_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.766972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.770972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14711 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6503 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions_negative.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.770972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15516 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6982 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base_test_proto.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.770972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4429 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5680 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_4byte_asn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5621 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_basic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.770972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5582 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/test_ipv4.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.770972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5728 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/test_ipv6.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8987 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/test_simple_bgp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1076 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.774973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.774973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/admin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4835 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/admin/test_floatingip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29531 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1176 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2007 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10546 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_connectivity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8028 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_dhcp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10916 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_dns_integration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2640 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_dvr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3688 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_fip64.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26721 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_floatingip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8441 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_internal_dns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10763 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_ipv6.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4109 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_local_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8384 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_mac_learning.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6518 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10387 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12302 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_mtu.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15576 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_multicast.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13020 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_port_forwardings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4891 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_ports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_portsecurity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17605 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_qos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52310 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21291 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_trunk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8153 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_vlan_transparency.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.778973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.778973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/services/bgp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/services/bgp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6738 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/services/bgp/bgp_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.778973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/services/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/services/network/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.778973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/services/network/json/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/services/network/json/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50880 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/services/network/json/network_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.778973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.778973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/services/flowclassifier_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5309 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/services/sfc_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.778973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.778973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8011 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/api/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3355 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/api/test_flowclassifier_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16294 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/api/test_sfc_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/flowclassifier_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.778973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2922 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/scenario/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3805 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/scenario/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50981 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/scenario/test_sfc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3536 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/sfc_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.778973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.782973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5759 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/api/test_taas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3391 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.782973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11849 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/scenario/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10534 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_taas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11086 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_traffic_impact.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.782973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/services/taas_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.782973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.782973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6368 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/api/base_vpnaas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42133 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/api/test_vpnaas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.782973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/scenario/base_vpnaas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11864 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/scenario/test_vpnaas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.782973 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2452 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/services/clients_vpnaas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.750972 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1443 2023-04-27 15:11:42.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11787 2023-04-27 15:11:42.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-27 15:11:42.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-04-27 15:11:42.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-27 15:11:42.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-04-27 15:11:42.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-04-27 15:11:42.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2023-04-27 15:11:42.000000 neutron-tempest-plugin-2.3.0/neutron_tempest_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.782973 neutron-tempest-plugin-2.3.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/playbooks/dvr-multinode-scenario-pre-run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/playbooks/dynamic-routing-pre-run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/playbooks/linuxbridge-scenario-pre-run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.742972 neutron-tempest-plugin-2.3.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.786973 neutron-tempest-plugin-2.3.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/releasenotes/notes/agents-client-delete-method-de1a7fb3f845999c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/releasenotes/notes/drop-py-2-7-74b8379cab4cdc5a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/releasenotes/notes/igmp-snooping-8d6d85608df8880a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/releasenotes/notes/mark-methods-removals-f8b230171c045a3e.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.786973 neutron-tempest-plugin-2.3.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/releasenotes/source/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.786973 neutron-tempest-plugin-2.3.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.786973 neutron-tempest-plugin-2.3.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8695 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.742972 neutron-tempest-plugin-2.3.0/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.742972 neutron-tempest-plugin-2.3.0/roles/docker-setup/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.786973 neutron-tempest-plugin-2.3.0/roles/docker-setup/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/roles/docker-setup/files/52_docker_for_tempest
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/roles/docker-setup/files/docker_apparmor
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.786973 neutron-tempest-plugin-2.3.0/roles/docker-setup/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/roles/docker-setup/tasks/main.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.786973 neutron-tempest-plugin-2.3.0/roles/multi-node-setup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      771 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/roles/multi-node-setup/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.786973 neutron-tempest-plugin-2.3.0/roles/multi-node-setup/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/roles/multi-node-setup/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.786973 neutron-tempest-plugin-2.3.0/roles/multi-node-setup/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/roles/multi-node-setup/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2023-04-27 15:11:42.790973 neutron-tempest-plugin-2.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.786973 neutron-tempest-plugin-2.3.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5745 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/tools/customize_ubuntu_image
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1283 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/tools/misc-sanity-checks.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:11:42.790973 neutron-tempest-plugin-2.3.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10556 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/zuul.d/2023_1_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/zuul.d/base-nested-switch.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49425 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/zuul.d/master_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8664 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9569 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/zuul.d/train_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13375 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/zuul.d/ussuri_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11742 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/zuul.d/victoria_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8585 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/zuul.d/wallaby_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7395 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/zuul.d/xena_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7638 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/zuul.d/yoga_jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9042 2023-04-27 15:11:20.000000 neutron-tempest-plugin-2.3.0/zuul.d/zed_jobs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.766387 neutron-tempest-plugin-2.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7044 2023-06-26 09:28:27.000000 neutron-tempest-plugin-2.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44025 2023-06-26 09:28:27.000000 neutron-tempest-plugin-2.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1443 2023-06-26 09:28:27.766387 neutron-tempest-plugin-2.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.730388 neutron-tempest-plugin-2.4.0/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/devstack/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5198 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/devstack/customize_image.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3019 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/devstack/functions.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.730388 neutron-tempest-plugin-2.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.730388 neutron-tempest-plugin-2.4.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2600 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.730388 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.742387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.746387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2190 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_agent_availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4585 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_agent_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_extension_driver_port_security_admin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12246 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_external_network_extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3418 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_floating_ips_admin_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3597 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_l3_agent_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4276 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2429 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_logging_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11860 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_network_segment_range.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4192 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11964 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_ports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6283 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7054 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_quotas_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4252 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_routers_dvr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4891 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_routers_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5179 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_routers_ha.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21527 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_shared_network_extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16723 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_tag.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    63450 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/base_routers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/base_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6437 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13901 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_address_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11743 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_address_scopes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_address_scopes_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5296 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_auto_allocated_topology.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1162 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6072 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_conntrack_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4030 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_dhcp_ipv6.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6679 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_extension_driver_port_security.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2235 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_extra_dhcp_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6897 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_flavors_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7691 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_floating_ips.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2546 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_floating_ips_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5852 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_local_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7288 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_metering_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_metering_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4923 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_ndp_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6210 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_ndp_proxy_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8764 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_network_ip_availability.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_network_ip_availability_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9208 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_networks_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4848 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_port_forwarding_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10876 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_port_forwardings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12069 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_ports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_ports_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    77868 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_qos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11965 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_qos_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20479 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_revisions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4948 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_router_interface_fip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22869 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_routers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7580 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_routers_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31264 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10498 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_security_groups_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_service_type_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3840 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_subnetpool_prefix_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26618 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_subnetpools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14768 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_subnetpools_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4536 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16121 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_timestamp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15374 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_trunk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2760 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_trunk_details.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13558 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_trunk_negative.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.746387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.746387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17284 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/api/test_bgpvpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3553 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.746387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6125 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/scenario/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    63991 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/scenario/test_bgpvpn_basic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.746387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4809 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/services/bgpvpn_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.746387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6862 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16928 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6589 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11865 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/ssh.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/tempest_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8565 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11617 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3170 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.746387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.750387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/api/fwaas_v2_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14899 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/api/test_fwaasv2_extensions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.750387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7110 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/common/fwaas_v2_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.750387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2988 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2734 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13139 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/scenario/test_fwaas_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.750387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4681 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/services/v2_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.750387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.750387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14711 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6503 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions_negative.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.750387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15516 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6982 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base_test_proto.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.750387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4429 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5680 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_4byte_asn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5621 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_basic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.750387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5582 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/test_ipv4.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.754387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5728 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/test_ipv6.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8987 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/test_simple_bgp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1076 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.754387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.754387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/admin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4835 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/admin/test_floatingip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29563 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1176 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2007 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10546 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_connectivity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8028 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_dhcp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10916 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_dns_integration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2640 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_dvr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3688 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_fip64.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26721 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_floatingip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8441 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_internal_dns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10763 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_ipv6.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4109 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_local_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8384 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_mac_learning.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6518 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10387 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12302 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_mtu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15576 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_multicast.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13020 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_port_forwardings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4891 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_ports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_portsecurity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17605 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_qos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52310 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21291 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_trunk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8153 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_vlan_transparency.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.754387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/services/bgp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/services/bgp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6738 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/services/bgp/bgp_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/services/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/services/network/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/services/network/json/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/services/network/json/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50880 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/services/network/json/network_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/services/flowclassifier_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5309 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/services/sfc_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8011 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/api/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3355 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/api/test_flowclassifier_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16294 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/api/test_sfc_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/flowclassifier_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2922 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/scenario/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3805 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/scenario/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50981 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/scenario/test_sfc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3536 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/sfc_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5759 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/api/test_taas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3391 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11849 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/scenario/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10534 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_taas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11086 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_traffic_impact.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/services/taas_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.758387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6368 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/api/base_vpnaas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42133 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/api/test_vpnaas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/scenario/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/scenario/base_vpnaas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11864 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/scenario/test_vpnaas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2452 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/services/clients_vpnaas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.734387 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1443 2023-06-26 09:28:27.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11787 2023-06-26 09:28:27.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-26 09:28:27.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-06-26 09:28:27.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-26 09:28:27.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-06-26 09:28:27.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-06-26 09:28:27.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2023-06-26 09:28:27.000000 neutron-tempest-plugin-2.4.0/neutron_tempest_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/playbooks/dvr-multinode-scenario-pre-run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/playbooks/dynamic-routing-pre-run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/playbooks/linuxbridge-scenario-pre-run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.726388 neutron-tempest-plugin-2.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/releasenotes/notes/agents-client-delete-method-de1a7fb3f845999c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/releasenotes/notes/drop-py-2-7-74b8379cab4cdc5a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/releasenotes/notes/igmp-snooping-8d6d85608df8880a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/releasenotes/notes/mark-methods-removals-f8b230171c045a3e.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/releasenotes/source/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8695 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.726388 neutron-tempest-plugin-2.4.0/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.726388 neutron-tempest-plugin-2.4.0/roles/docker-setup/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/roles/docker-setup/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/roles/docker-setup/files/52_docker_for_tempest
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/roles/docker-setup/files/docker_apparmor
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/roles/docker-setup/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/roles/docker-setup/tasks/main.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/roles/multi-node-setup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      771 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/roles/multi-node-setup/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/roles/multi-node-setup/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/roles/multi-node-setup/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/roles/multi-node-setup/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/roles/multi-node-setup/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2023-06-26 09:28:27.766387 neutron-tempest-plugin-2.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.762387 neutron-tempest-plugin-2.4.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5745 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/tools/customize_ubuntu_image
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1283 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/tools/misc-sanity-checks.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-26 09:28:27.766387 neutron-tempest-plugin-2.4.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10733 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/zuul.d/2023_1_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1649 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/zuul.d/base-nested-switch.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48934 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/zuul.d/master_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8374 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9569 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/zuul.d/train_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13375 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/zuul.d/ussuri_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11742 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/zuul.d/victoria_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8585 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/zuul.d/wallaby_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8800 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/zuul.d/xena_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8577 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/zuul.d/yoga_jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10140 2023-06-26 09:28:01.000000 neutron-tempest-plugin-2.4.0/zuul.d/zed_jobs.yaml
```

### Comparing `neutron-tempest-plugin-2.3.0/AUTHORS` & `neutron-tempest-plugin-2.4.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 Kailun Qin <kailun.qin@intel.com>
 Ken'ichi Ohmichi <ken-oomichi@wx.jp.nec.com>
 Kevin Benton <blak111@gmail.com>
 Kevin Benton <kevin@benton.pub>
 Kyle Mestery <mestery@mestery.com>
 LIU Yulong <i@liuyulong.me>
 LIU Yulong <liuyulong@letv.com>
+Lajos Katona <katonalala@gmail.com>
 Lajos Katona <lajos.katona@ericsson.com>
 LiZekun <2954674728@qq.com>
 Lucas Alvares Gomes <lucasagomes@gmail.com>
 Luigi Toscano <ltoscano@redhat.com>
 Lujin <luo.lujin@jp.fujitsu.com>
 Luna Das <ld366r@att.com>
 Luong Anh Tuan <tuanla@vn.fujitsu.com>
```

### Comparing `neutron-tempest-plugin-2.3.0/CONTRIBUTING.rst` & `neutron-tempest-plugin-2.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/ChangeLog` & `neutron-tempest-plugin-2.4.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,32 @@
 CHANGES
 =======
 
+2.4.0
+-----
+
+* Revert "Make neutron-tempest-plugin-bgpvpn-bagpipe non-voting"
+* Don't check exit status when nc\_client is spawned
+* Don't use "Zero-I/O mode" in nc client in the TCP mode
+* Define proper common API extensions for 2023.1 and Zed jobs
+* [fwaas]Disassociate all ports before deleting firewall group
+* Adapt bgpvpn scenarios to recent sRBAC changes
+* Make neutron-tempest-plugin-bgpvpn-bagpipe non-voting
+* [S-RBAC] Update DSCP marking rule create API test
+* Revert "Revert "Update nested-virt testing for the 2023.1 cycle""
+* Revert "[S-RBAC] Switch to new policies by default"
+* Don't run stable/xena jobs in check/gate queue anymore
+* Get nc client's command based on the nc on correct host
+
 2.3.0
 -----
 
 * Don't run stadium related jobs when scenario tests are changed
 * Set unlimited SG rules quota in security groups scenario tests
+* [S-RBAC] Switch to new policies by default
 * [Stateless SG] Test fragmented traffic is allowed by stateless SG
 * [Stateless SG] Test if TCP packets with various conn state are allowed
 * [Stateless SG] Ensure replies won't work without ingress rule
 * [Stateless SG] Add test to check connectivity between vms
 * Add plugin.spec to irrelevant-files
 * Skip stateless SG related tests for backends which don't support it
 * Add job definitions for 2023.1 (Antelope) branch
@@ -35,14 +52,15 @@
 * Pin neutron-tempest-plugin for stable/wallaby jobs
 * Stateful SG tests without ingress metadata rule
 * Add the requirements.txt file to the tox deps
 * Make dns\_domain value configurable
 * [taas] Use ubuntu minimal as advanced image
 * Fix nested virt job variant for EM releases
 * [ovn] Use ubuntu minimal as advanced image
+* Test neutron-dynamic-routing on OVN
 * Fix tox.ini with tox4
 * Run security group scenario tests against stateless security groups too
 * Run security group api tests against stateless security groups too
 * Remove note about migration from lib/neutron-legacy to lib/neutron
 
 2.1.0
 -----
```

### Comparing `neutron-tempest-plugin-2.3.0/LICENSE` & `neutron-tempest-plugin-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/PKG-INFO` & `neutron-tempest-plugin-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-tempest-plugin
-Version: 2.3.0
+Version: 2.4.0
 Summary: Tempest plugin for Neutron Project
 Home-page: https://opendev.org/openstack/neutron-tempest-plugin
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ======================
         Neutron Tempest Plugin
```

### Comparing `neutron-tempest-plugin-2.3.0/devstack/README.rst` & `neutron-tempest-plugin-2.4.0/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/devstack/customize_image.sh` & `neutron-tempest-plugin-2.4.0/devstack/customize_image.sh`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/devstack/functions.sh` & `neutron-tempest-plugin-2.4.0/devstack/functions.sh`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/devstack/plugin.sh` & `neutron-tempest-plugin-2.4.0/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/doc/source/conf.py` & `neutron-tempest-plugin-2.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/doc/source/index.rst` & `neutron-tempest-plugin-2.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_agent_availability_zone.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_agent_availability_zone.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_agent_management.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_agent_management.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_extension_driver_port_security_admin.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_extension_driver_port_security_admin.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_external_network_extension.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_external_network_extension.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_floating_ips_admin_actions.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_floating_ips_admin_actions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_l3_agent_scheduler.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_l3_agent_scheduler.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_logging.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_logging.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_logging_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_logging_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_network_segment_range.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_network_segment_range.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_networks.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_networks.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_ports.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_ports.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_quotas.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_quotas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_quotas_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_quotas_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_routers_dvr.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_routers_dvr.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_routers_flavors.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_routers_flavors.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_routers_ha.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_routers_ha.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_security_groups.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_security_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_shared_network_extension.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_shared_network_extension.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/admin/test_tag.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/admin/test_tag.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/base.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/base_routers.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/base_routers.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/base_security_groups.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/base_security_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/clients.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/clients.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_address_groups.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_address_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_address_scopes.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_address_scopes.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_address_scopes_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_address_scopes_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_auto_allocated_topology.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_auto_allocated_topology.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_availability_zones.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_conntrack_helper.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_conntrack_helper.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_dhcp_ipv6.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_dhcp_ipv6.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_extension_driver_port_security.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_extension_driver_port_security.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_extensions.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_extra_dhcp_options.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_extra_dhcp_options.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_flavors_extensions.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_flavors_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_floating_ips.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_floating_ips.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_floating_ips_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_floating_ips_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_local_ip.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_local_ip.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_metering_extensions.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_metering_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_metering_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_metering_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_ndp_proxy.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_ndp_proxy.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_ndp_proxy_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_ndp_proxy_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_network_ip_availability.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_network_ip_availability.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_network_ip_availability_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_network_ip_availability_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_networks.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_networks.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_networks_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_networks_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_port_forwarding_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_port_forwarding_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_port_forwardings.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_port_forwardings.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_ports.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_ports.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_ports_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_ports_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_qos.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_qos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1191,14 +1191,15 @@
         # Setup network
         self.network = self.create_network()
 
         # Create QoS policy
         dscp_policy_id = self.create_qos_policy(
             name=self.policy_name,
             description='test-qos-policy',
+            project_id=self.client.project_id,
             shared=True)['id']
 
         # Associate QoS to the network
         self.admin_client.update_network(
             self.network['id'], qos_policy_id=dscp_policy_id)
 
         # Set a new DSCP rule with the first mark in range
```

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_qos_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_qos_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_revisions.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_revisions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_router_interface_fip.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_router_interface_fip.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_routers.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_routers.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_routers_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_routers_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_security_groups.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_security_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_security_groups_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_security_groups_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_service_type_management.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_service_type_management.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_subnetpool_prefix_ops.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_subnetpool_prefix_ops.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_subnetpools.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_subnetpools.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_subnetpools_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_subnetpools_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_subnets.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_subnets.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_timestamp.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_trunk.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_trunk.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_trunk_details.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_trunk_details.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/api/test_trunk_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/api/test_trunk_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/api/test_bgpvpn.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/api/test_bgpvpn.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/base.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/scenario/manager.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/scenario/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                     rules.append(sg_rule)
 
         return rules
 
     def _create_router(self, client=None, tenant_id=None,
                        namestart='router-smoke'):
         if not client:
-            client = self.routers_client
+            client = self.admin_routers_client
         if not tenant_id:
             tenant_id = client.tenant_id
         name = data_utils.rand_name(namestart)
         result = client.create_router(name=name,
                                       admin_state_up=True,
                                       tenant_id=tenant_id)
         router = result['router']
```

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/scenario/test_bgpvpn_basic.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/scenario/test_bgpvpn_basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,14 +104,28 @@
         self.server_fips = {}
         self._create_security_group_for_test()
         self.RT1 = self.new_rt()
         self.RT2 = self.new_rt()
         self.RT3 = self.new_rt()
         self.RT4 = self.new_rt()
 
+    @classmethod
+    def setup_clients(cls):
+        """This setup the service clients for the tests"""
+        super(TestBGPVPNBasic, cls).setup_clients()
+        cls.admin_security_group_client = cls.os_admin.security_groups_client
+        cls.admin_security_group_rule_client = (
+            cls.os_admin.security_group_rules_client)
+        cls.admin_routers_client = cls.os_admin.routers_client
+        cls.admin_ports_client = cls.os_admin.ports_client
+        cls.admin_networks_client = cls.os_admin.networks_client
+        cls.admin_subnets_client = cls.os_admin.subnets_client
+        cls.admin_fips_client = cls.os_admin.floating_ips_client
+        cls.admin_keys_client = cls.os_admin.keypairs_client
+
     @decorators.idempotent_id('afdd6cad-871a-4343-b97b-6319c76c815d')
     @utils.services('compute', 'network')
     def test_bgpvpn_basic(self):
         """This test checks basic BGPVPN.
 
         1. Create networks A and B with their respective subnets
         2. Start up server 1 in network A
@@ -160,14 +174,15 @@
         6. Create router and connect it to network A
         7. Give a FIP to server 1
         8. Check that server 1 can ping server 2
         """
         self._create_networks_and_subnets()
         self._create_servers()
         self.router_b = self._create_fip_router(
+            client=self.admin_routers_client,
             subnet_id=self.subnets[NET_B][0]['id'])
         self._create_l3_bgpvpn()
         self._associate_all_nets_to_bgpvpn()
         self._associate_fip_and_check_l3_bgpvpn()
 
     @decorators.idempotent_id('7c66aa31-fb3a-4e15-8808-46eb361f153a')
     @utils.services('compute', 'network')
@@ -183,18 +198,21 @@
         7. Create router and connect it to network A
         8. Give a FIP to server 1
         9. Check that server 1 can ping server 2
         """
         self._create_networks_and_subnets()
         self._create_servers()
         self.router_b = self._create_fip_router(
+            client=self.admin_routers_client,
             subnet_id=self.subnets[NET_B][0]['id'])
         self._create_l3_bgpvpn()
         self._associate_all_nets_to_bgpvpn()
-        self.delete_router(self.router_b)
+        self._delete_router(self.router_b,
+                            routers_client=self.admin_routers_client,
+                            ports_client=self.admin_ports_client)
         self._associate_fip_and_check_l3_bgpvpn()
 
     @decorators.idempotent_id('973ab26d-c7d8-4a32-9aa9-2d7e6f406135')
     @utils.services('compute', 'network')
     def test_bgpvpn_variant4(self):
         """This test checks basic BGPVPN.
 
@@ -208,14 +226,15 @@
         8. Check that server 2 can ping server 1
         """
         self._create_networks_and_subnets()
         self._create_servers()
         self._create_l3_bgpvpn()
         self._associate_all_nets_to_bgpvpn()
         self.router_b = self._create_fip_router(
+            client=self.admin_routers_client,
             subnet_id=self.subnets[NET_B][0]['id'])
         self._associate_fip_and_check_l3_bgpvpn()
 
     @decorators.idempotent_id('2ac0696b-e828-4299-9e94-5f9c4988d961')
     @utils.services('compute', 'network')
     def test_bgpvpn_variant5(self):
         """This test checks basic BGPVPN.
@@ -227,14 +246,15 @@
         5. Start up server 2 in network B
         6. Create router and connect it to network A
         7. Give a FIP to server 1
         8. Check that server 2 can ping server 1
         """
         self._create_networks_and_subnets()
         self.router_b = self._create_fip_router(
+            client=self.admin_routers_client,
             subnet_id=self.subnets[NET_B][0]['id'])
         self._create_l3_bgpvpn()
         self._associate_all_nets_to_bgpvpn()
         self._create_servers()
         self._associate_fip_and_check_l3_bgpvpn()
 
     @decorators.idempotent_id('9081338e-a52e-46bb-a40e-bda24ec4b1bd')
@@ -251,14 +271,15 @@
         7. Give a FIP to server 1
         8. Check that server 2 can ping server 1
         """
         self._create_networks_and_subnets()
         self._create_l3_bgpvpn()
         self._associate_all_nets_to_bgpvpn()
         self.router_b = self._create_fip_router(
+            client=self.admin_routers_client,
             subnet_id=self.subnets[NET_B][0]['id'])
         self._create_servers()
         self._associate_fip_and_check_l3_bgpvpn()
 
     @decorators.idempotent_id('133497a1-2788-40f7-be01-b3b64b5ef8cd')
     @utils.services('compute', 'network')
     def test_bgpvpn_update_route_targets_disjoint_targets(self):
@@ -340,18 +361,18 @@
         """
         self._create_networks_and_subnets()
         self._create_servers()
         self.router = self._create_router_and_associate_fip(
             0, self.subnets[NET_A][0])
         self._create_l3_bgpvpn(rts=[], export_rts=[self.RT1],
                                import_rts=[self.RT2])
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_A]['id'])
         self._check_l3_bgpvpn(should_succeed=False)
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_B]['id'])
         self._check_l3_bgpvpn(should_succeed=False)
         self._update_l3_bgpvpn(rts=[self.RT1], import_rts=[], export_rts=[])
         self._check_l3_bgpvpn()
 
     @test.unstable_test("bug 1897408")
     @decorators.idempotent_id('c8bfd695-f731-47a6-86e3-3dfa492e08e0')
@@ -384,21 +405,21 @@
         self._create_networks_and_subnets()
         self._create_l3_bgpvpn(rts=[], import_rts=[self.RT1],
                                export_rts=[self.RT2])
         self._create_servers([[self.networks[NET_A], IP_A_S1_1],
                              [self.networks[NET_B], IP_B_S1_1],
                              [self.networks[NET_A], IP_A_S1_2],
                              [self.networks[NET_B], IP_B_S1_2]])
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_A]['id'])
         self.router_a = self._create_router_and_associate_fip(
             0, self.subnets[NET_A][0])
         self._check_l3_bgpvpn(should_succeed=False)
         self._check_l3_bgpvpn(self.servers[0], self.servers[2])
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_B]['id'])
         self.router_b = self._create_router_and_associate_fip(
             1, self.subnets[NET_B][0])
         self._check_l3_bgpvpn(should_succeed=False)
         self._check_l3_bgpvpn(self.servers[1], self.servers[3])
         self._update_l3_bgpvpn(rts=[self.RT1], import_rts=[], export_rts=[])
         self._check_l3_bgpvpn()
@@ -440,19 +461,19 @@
                              [self.networks[NET_B], IP_B_S1_1],
                              [self.networks[NET_A], IP_A_S1_2],
                              [self.networks[NET_B], IP_B_S1_2]])
         self._create_router_and_associate_fip(
             0, self.subnets[NET_A][0])
         router_b = self._create_router_and_associate_fip(
             3, self.subnets[NET_B][0])
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_A]['id'])
         self._check_l3_bgpvpn(should_succeed=False)
         self._check_l3_bgpvpn(self.servers[0], self.servers[2])
-        self.bgpvpn_client.create_router_association(self.bgpvpn['id'],
+        self.bgpvpn_admin_client.create_router_association(self.bgpvpn['id'],
                                                      router_b['id'])
         self._check_l3_bgpvpn(should_succeed=False)
         self._check_l3_bgpvpn(self.servers[3], self.servers[1])
         self._update_l3_bgpvpn(rts=[self.RT1], import_rts=[], export_rts=[])
         self._check_l3_bgpvpn()
         self._check_l3_bgpvpn(self.servers[0], self.servers[2])
         self._check_l3_bgpvpn(self.servers[3], self.servers[1])
@@ -509,40 +530,40 @@
         primary_port_routes = [{'type': 'prefix',
                                 'local_pref': 200,
                                 'prefix': NET_C_S1}]
         alternate_port_routes = [{'type': 'prefix',
                                   'local_pref': 100,
                                   'prefix': NET_C_S1}]
 
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_A]['id'])
 
         port_id_1 = self.ports[self.servers[1]['id']]['id']
-        body = self.bgpvpn_client.create_port_association(
+        body = self.bgpvpn_admin_client.create_port_association(
             self.bgpvpn['id'], port_id=port_id_1, routes=primary_port_routes)
         port_association_1 = body['port_association']
 
         port_id_2 = self.ports[self.servers[2]['id']]['id']
-        body = self.bgpvpn_client.create_port_association(
+        body = self.bgpvpn_admin_client.create_port_association(
             self.bgpvpn['id'], port_id=port_id_2, routes=alternate_port_routes)
         port_association_2 = body['port_association']
 
         destination_srv_1 = '%s:%s' % (self.servers[1]['name'],
                                        self.servers[1]['id'])
         destination_srv_2 = '%s:%s' % (self.servers[2]['name'],
                                        self.servers[2]['id'])
 
         self._check_l3_bgpvpn_by_specific_ip(
             to_server_ip=IP_C_S1_1,
             validate_server=destination_srv_1)
 
-        self.bgpvpn_client.update_port_association(
+        self.bgpvpn_admin_client.update_port_association(
             self.bgpvpn['id'], port_association_1['id'],
             routes=alternate_port_routes)
-        self.bgpvpn_client.update_port_association(
+        self.bgpvpn_admin_client.update_port_association(
             self.bgpvpn['id'], port_association_2['id'],
             routes=primary_port_routes)
 
         self._check_l3_bgpvpn_by_specific_ip(
             to_server_ip=IP_C_S1_1,
             validate_server=destination_srv_2)
 
@@ -577,17 +598,17 @@
         self._create_networks_and_subnets([NET_A, NET_A_BIS],
                                           [[NET_A_S1, NET_A_S2],
                                            [NET_A_S1, NET_A_S2]])
         bgpvpn_a = self._create_l3_bgpvpn(name='test-l3-bgpvpn-a',
                                           rts=[self.RT1])
         bgpvpn_a_bis = self._create_l3_bgpvpn(name='test-l3-bgpvpn-a-bis',
                                               rts=[self.RT2])
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             bgpvpn_a['id'], self.networks[NET_A]['id'])
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             bgpvpn_a_bis['id'], self.networks[NET_A_BIS]['id'])
         self._create_servers([[self.networks[NET_A], IP_A_S1_1],
                              [self.networks[NET_A_BIS], IP_A_BIS_S1_2],
                              [self.networks[NET_A], IP_A_S1_2],
                              [self.networks[NET_A_BIS], IP_A_BIS_S1_3],
                              [self.networks[NET_A], IP_A_S1_3]])
         self._create_fip_router(subnet_id=self.subnets[NET_A][0]['id'])
@@ -648,26 +669,25 @@
         # preliminary check that no connectivity to 192.168.0.1 initially
         # exists
         self._check_l3_bgpvpn_by_specific_ip(
             should_succeed=False, to_server_ip=IP_C_S1_1)
 
         self._setup_ip_forwarding(1)
         self._setup_ip_address(1, IP_C_S1_1)
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_A]['id'])
         port_id = self.ports[self.servers[1]['id']]['id']
         port_routes = [{'type': 'prefix',
                         'prefix': NET_C_S1}]
-        body = self.bgpvpn_client.create_port_association(self.bgpvpn['id'],
-                                                          port_id=port_id,
-                                                          routes=port_routes)
+        body = self.bgpvpn_admin_client.create_port_association(
+            self.bgpvpn['id'], port_id=port_id, routes=port_routes)
         port_association = body['port_association']
         self._check_l3_bgpvpn_by_specific_ip(
             to_server_ip=IP_C_S1_1)
-        self.bgpvpn_client.update_port_association(
+        self.bgpvpn_admin_client.update_port_association(
             self.bgpvpn['id'], port_association['id'], routes=[])
         self._check_l3_bgpvpn_by_specific_ip(
             should_succeed=False, to_server_ip=IP_C_S1_1)
 
     @decorators.idempotent_id('d92a8a18-c4d0-40d5-8592-713d7dae7d25')
     @utils.services('compute', 'network')
     @utils.requires_ext(extension='bgpvpn-routes-control', service='network')
@@ -713,33 +733,32 @@
             self._check_l3_bgpvpn_by_specific_ip(
                 should_succeed=False, to_server_ip=ip)
 
         self._setup_ip_forwarding(1)
 
         self._setup_range_ip_address(1, LOOPBACKS)
 
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_A]['id'])
         port_id = self.ports[self.servers[1]['id']]['id']
         port_routes = [{'type': 'prefix',
                         'prefix': ip + "/32"}
                        for ip in LOOPBACKS]
 
-        body = self.bgpvpn_client.create_port_association(self.bgpvpn['id'],
-                                                          port_id=port_id,
-                                                          routes=port_routes)
+        body = self.bgpvpn_admin_client.create_port_association(
+            self.bgpvpn['id'], port_id=port_id, routes=port_routes)
         port_association = body['port_association']
 
         for ip in random.sample(LOOPBACKS, SAMPLE_SIZE):
             LOG.debug("Check that server 1 can "
                       "ping server 2 alternative ip %s", ip)
             self._check_l3_bgpvpn_by_specific_ip(
                 to_server_ip=ip)
 
-        self.bgpvpn_client.update_port_association(
+        self.bgpvpn_admin_client.update_port_association(
             self.bgpvpn['id'], port_association['id'], routes=[])
 
         for ip in SUB_LOOPBACKS:
             LOG.debug("Check that server 1 can't "
                       "ping server 2 alternative ip %s", ip)
             self._check_l3_bgpvpn_by_specific_ip(
                 should_succeed=False, to_server_ip=ip)
@@ -778,26 +797,25 @@
         # preliminary check that no connectivity to 192.168.0.1 initially
         # exists
         self._check_l3_bgpvpn_by_specific_ip(
             should_succeed=False, to_server_ip=IP_C_S1_1)
 
         self._setup_ip_forwarding(1)
         self._setup_ip_address(1, IP_C_S1_1)
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_A]['id'])
         port_id = self.ports[self.servers[1]['id']]['id']
         port_routes = [{'type': 'prefix',
                         'prefix': NET_C_S1}]
-        body = self.bgpvpn_client.create_port_association(self.bgpvpn['id'],
-                                                          port_id=port_id,
-                                                          routes=port_routes)
+        body = self.bgpvpn_admin_client.create_port_association(
+            self.bgpvpn['id'], port_id=port_id, routes=port_routes)
         port_association = body['port_association']
         self._check_l3_bgpvpn_by_specific_ip(
             to_server_ip=IP_C_S1_1)
-        self.bgpvpn_client.delete_port_association(
+        self.bgpvpn_admin_client.delete_port_association(
             self.bgpvpn['id'], port_association['id'])
         self._check_l3_bgpvpn_by_specific_ip(
             should_succeed=False, to_server_ip=IP_C_S1_1)
 
     @decorators.idempotent_id('73f629fa-fdae-40fc-8a7e-da3aedcf797a')
     @utils.services('compute', 'network')
     @utils.requires_ext(extension='bgpvpn-routes-control', service='network')
@@ -862,39 +880,39 @@
         self._associate_fip(1)
         self._associate_fip(2)
 
         # disable IP forwarding on VM2
         self._setup_ip_forwarding(0)
 
         # connect network A to its BGPVPN
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             bgpvpn_a['id'], self.networks[NET_A]['id'])
 
         # connect network B to its BGPVPN
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             bgpvpn_b['id'], self.networks[NET_B]['id'])
 
         # connect network C to its BGPVPN
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             bgpvpn_c['id'], self.networks[NET_C]['id'])
 
         # create port associations for A->C traffic
         # (leak routes imported by BGPVPN B -- which happen to include the
         # routes net C -- into net A)
-        self.bgpvpn_client.create_port_association(
+        self.bgpvpn_admin_client.create_port_association(
             bgpvpn_to_a['id'],
             port_id=self.ports[vm2['id']]['id'],
             routes=[{'type': 'bgpvpn',
                      'bgpvpn_id': bgpvpn_b['id']},
                     ])
 
         # create port associations for C->A traffic
         # (leak routes imported by BGPVPN B -- which happen to include the
         # routes from net A -- into net C)
-        body = self.bgpvpn_client.create_port_association(
+        body = self.bgpvpn_admin_client.create_port_association(
             bgpvpn_to_c['id'],
             port_id=self.ports[vm2['id']]['id'],
             routes=[{'type': 'bgpvpn',
                      'bgpvpn_id': bgpvpn_a['id']}])
 
         port_association = body['port_association']
 
@@ -910,15 +928,15 @@
 
         # VM1 should now be able to join VM2
         self._check_l3_bgpvpn_by_specific_ip(from_server=vm1,
                                              to_server_ip=IP_C_S1_1,
                                              should_succeed=True)
 
         # remove port association 1
-        self.bgpvpn_client.delete_port_association(self.bgpvpn['id'],
+        self.bgpvpn_admin_client.delete_port_association(self.bgpvpn['id'],
                                                    port_association['id'])
 
         # check that connectivity is actually interrupted
         self._check_l3_bgpvpn_by_specific_ip(from_server=vm1,
                                              to_server_ip=IP_C_S1_1,
                                              should_succeed=False)
 
@@ -934,15 +952,15 @@
         5. Start up server 2 in network B
         6. Create router and connect it to network A
         7. Give a FIP to server 1
         8. Check that server 1 cannot ping server 2
         """
         self._create_networks_and_subnets()
         self._create_l3_bgpvpn()
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_A]['id'])
         self._create_servers()
         self._associate_fip_and_check_l3_bgpvpn(should_succeed=False)
 
     @decorators.idempotent_id('b6d219b2-90bb-431f-a566-bf6a780d1578')
     @utils.services('compute', 'network')
     def test_bgpvpn_negative_disjoint_import_export(self):
@@ -1003,18 +1021,18 @@
         7. Give a FIP to server 1
         8. Check that server 1 can ping server 2
         9. Delete association of network A
         10. Check that server 1 cannot ping server 2
         """
         self._create_networks_and_subnets()
         self._create_l3_bgpvpn()
-        body = self.bgpvpn_client.create_network_association(
+        body = self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_A]['id'])
         assoc_b = body['network_association']
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_B]['id'])
         self._create_servers()
         self._associate_fip_and_check_l3_bgpvpn()
         self.bgpvpn_admin_client.delete_network_association(self.bgpvpn['id'],
                                                             assoc_b['id'])
         self._check_l3_bgpvpn(should_succeed=False)
 
@@ -1036,18 +1054,18 @@
         11. Delete association of router B
         12. Check that server 1 cannot ping server 2
         """
         self._create_networks_and_subnets()
         router_b = self._create_fip_router(
             subnet_id=self.subnets[NET_B][0]['id'])
         self._create_l3_bgpvpn()
-        self.bgpvpn_client.create_network_association(
+        self.bgpvpn_admin_client.create_network_association(
             self.bgpvpn['id'], self.networks[NET_A]['id'])
-        body = self.bgpvpn_client.create_router_association(self.bgpvpn['id'],
-                                                            router_b['id'])
+        body = self.bgpvpn_admin_client.create_router_association(
+            self.bgpvpn['id'], router_b['id'])
         assoc_b = body['router_association']
         self._create_servers()
         self._associate_fip_and_check_l3_bgpvpn()
         self.bgpvpn_admin_client.delete_router_association(self.bgpvpn['id'],
                                                            assoc_b['id'])
         self._check_l3_bgpvpn(should_succeed=False)
 
@@ -1100,34 +1118,36 @@
         self._associate_all_nets_to_bgpvpn()
         self._associate_fip_and_check_l3_bgpvpn()
         self._update_l3_bgpvpn(rts=[], import_rts=[], export_rts=[])
         self._check_l3_bgpvpn(should_succeed=False)
 
     def _create_security_group_for_test(self):
         self.security_group = self.create_security_group(
-            project_id=self.bgpvpn_client.project_id)
+            project_id=self.bgpvpn_admin_client.project_id,
+            security_groups_client=self.admin_security_group_client,
+            security_group_rules_client=self.admin_security_group_rule_client)
 
     def _create_networks_and_subnets(self, names=None, subnet_cidrs=None,
                                      port_security=True):
         if not names:
             names = [NET_A, NET_B, NET_C]
         if not subnet_cidrs:
             subnet_cidrs = [[NET_A_S1], [NET_B_S1], [NET_C_S1]]
         for (name, subnet_cidrs) in zip(names, subnet_cidrs):
             network = super(manager.NetworkScenarioTest,
                             self).create_network(namestart=name,
-                    port_security_enabled=port_security)
+                    port_security_enabled=port_security,
+                    networks_client=self.admin_networks_client)
             self.networks[name] = network
             self.subnets[name] = []
             for (j, cidr) in enumerate(subnet_cidrs):
                 sub_name = "subnet-%s-%d" % (name, j + 1)
-                subnet = self._create_subnet_with_cidr(network,
-                                                       namestart=sub_name,
-                                                       cidr=cidr,
-                                                       ip_version=4)
+                subnet = self._create_subnet_with_cidr(
+                    network, namestart=sub_name, cidr=cidr, ip_version=4,
+                    subnets_client=self.admin_subnets_client)
                 self.subnets[name].append(subnet)
 
     def _create_subnet_with_cidr(self, network, subnets_client=None,
                                  namestart='subnet-smoke', **kwargs):
         if not subnets_client:
             subnets_client = self.subnets_client
         tenant_cidr = kwargs.get('cidr')
@@ -1142,14 +1162,16 @@
         self.assertEqual(subnet['cidr'], tenant_cidr)
         self.addCleanup(test_utils.call_and_ignore_notfound_exc,
                         subnets_client.delete_subnet, subnet['id'])
         return subnet
 
     def _create_fip_router(self, client=None, public_network_id=None,
                            subnet_id=None):
+        if not client:
+            client = self.admin_routers_client
         router = self._create_router(client, namestart='router-')
         router_id = router['id']
         if public_network_id is None:
             public_network_id = CONF.network.public_network_id
         if client is None:
             client = self.routers_client
         kwargs = {'external_gateway_info': {'network_id': public_network_id}}
@@ -1161,35 +1183,37 @@
                             subnet_id=subnet_id)
         return router
 
     def _associate_fip(self, server_index):
         server = self.servers[server_index]
         fip = self.create_floating_ip(
             server, external_network_id=CONF.network.public_network_id,
-            port_id=self.ports[server['id']]['id'])
+            port_id=self.ports[server['id']]['id'],
+            client=self.admin_fips_client)
         self.server_fips[server['id']] = fip
         return fip
 
     def _create_router_and_associate_fip(self, server_index, subnet):
-        router = self._create_fip_router(subnet_id=subnet['id'])
+        router = self._create_fip_router(client=self.admin_routers_client,
+                                         subnet_id=subnet['id'])
         self._associate_fip(server_index)
         return router
 
     def _create_server(self, name, keypair, network, ip_address,
                        security_group_ids, clients, port_security):
         security_groups = []
         if port_security:
             security_groups = security_group_ids
         create_port_body = {'fixed_ips': [{'ip_address': ip_address}],
                             'namestart': 'port-smoke',
                             'security_groups': security_groups}
 
         port = super(manager.NetworkScenarioTest,
                     self).create_port(network_id=network['id'],
-                                    client=clients.ports_client,
+                                    client=self.admin_ports_client,
                                     **create_port_body)
 
         create_server_kwargs = {
             'key_name': keypair['name'],
             'networks': [{'uuid': network['id'], 'port': port['id']}]
         }
         body, servers = compute.create_test_server(
@@ -1201,38 +1225,39 @@
         server = clients.servers_client.show_server(body['id'])['server']
         LOG.debug('Created server: %s with status: %s', server['id'],
                   server['status'])
         self.ports[server['id']] = port
         return server
 
     def _create_servers(self, ports_config=None, port_security=True):
-        keypair = self.create_keypair()
+        keypair = self.create_keypair(client=self.admin_keys_client)
         security_group_ids = [self.security_group['id']]
         if ports_config is None:
             ports_config = [[self.networks[NET_A], IP_A_S1_1],
                             [self.networks[NET_B], IP_B_S1_1]]
         for (i, port_config) in enumerate(ports_config):
             network = port_config[0]
             server = self._create_server(
                 'server-' + str(i + 1), keypair, network, port_config[1],
-                security_group_ids, self.os_primary, port_security)
+                security_group_ids, self.os_admin, port_security)
             self.servers.append(server)
             self.servers_keypairs[server['id']] = keypair
             self.server_fixed_ips[server['id']] = (
                 server['addresses'][network['name']][0]['addr'])
             self.assertTrue(self.servers_keypairs)
 
     def _create_l3_bgpvpn(self, name='test-l3-bgpvpn', rts=None,
                           import_rts=None, export_rts=None):
         if rts is None and import_rts is None and export_rts is None:
             rts = [self.RT1]
         import_rts = import_rts or []
         export_rts = export_rts or []
         self.bgpvpn = self.create_bgpvpn(
-            self.bgpvpn_admin_client, tenant_id=self.bgpvpn_client.tenant_id,
+            self.bgpvpn_admin_client,
+            tenant_id=self.bgpvpn_admin_client.tenant_id,
             name=name, route_targets=rts, export_targets=export_rts,
             import_targets=import_rts)
         return self.bgpvpn
 
     def _update_l3_bgpvpn(self, rts=None, import_rts=None, export_rts=None,
                           bgpvpn=None):
         bgpvpn = bgpvpn or self.bgpvpn
@@ -1245,15 +1270,15 @@
                                                route_targets=rts,
                                                export_targets=export_rts,
                                                import_targets=import_rts)
 
     def _associate_all_nets_to_bgpvpn(self, bgpvpn=None):
         bgpvpn = bgpvpn or self.bgpvpn
         for network in self.networks.values():
-            self.bgpvpn_client.create_network_association(
+            self.bgpvpn_admin_client.create_network_association(
                 bgpvpn['id'], network['id'])
         LOG.debug('BGPVPN network associations completed')
 
     def _setup_ssh_client(self, server):
         server_fip = self.server_fips[server['id']][
             'floating_ip_address']
         private_key = self.servers_keypairs[server['id']][
@@ -1356,7 +1381,20 @@
                           to_server_ip, from_server_ip, msg)
             raise
 
     def _associate_fip_and_check_l3_bgpvpn(self, should_succeed=True):
         subnet = self.subnets[NET_A][0]
         self.router = self._create_router_and_associate_fip(0, subnet)
         self._check_l3_bgpvpn(should_succeed=should_succeed)
+
+    def _delete_router(self, router, routers_client=None, ports_client=None):
+        if not routers_client:
+            routers_client = self.routers_client
+        if not ports_client:
+            ports_client = self.ports_client
+        ports_rsp = ports_client.list_ports(device_id=router['id'])
+        interfaces = ports_rsp['ports']
+        for i in interfaces:
+            test_utils.call_and_ignore_notfound_exc(
+                routers_client.remove_router_interface, router['id'],
+                subnet_id=i['fixed_ips'][0]['subnet_id'])
+        routers_client.delete_router(router['id'])
```

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/bgpvpn/services/bgpvpn_client.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/bgpvpn/services/bgpvpn_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/constants.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/ip.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/ip.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/shell.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/shell.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/ssh.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/ssh.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/tempest_fixtures.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/tempest_fixtures.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/common/utils.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/common/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/config.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/config.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/exceptions.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/api/fwaas_v2_base.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/api/fwaas_v2_base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/api/test_fwaasv2_extensions.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/api/test_fwaasv2_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,15 +332,18 @@
 
         # Update firewall group
         body = self.firewall_groups_client.update_firewall_group(
             fwg_id,
             ports=[intf_2['port_id']])
         updated_fwg = body["firewall_group"]
         self.assertEqual([intf_2['port_id']], updated_fwg['ports'])
-
+        # Wait for the firewall resource to become ready
+        self._wait_until_ready(fwg_id)
+        # Disassociate all ports with this firewall group
+        self.firewall_groups_client.update_firewall_group(fwg_id, ports=[])
         # Delete firewall_group
         self.firewall_groups_client.delete_firewall_group(fwg_id)
 
     @decorators.idempotent_id('a1f524d8-5336-4769-aa7b-0830bb4df6c8')
     def test_error_on_create_firewall_group_name_default(self):
         try:
             # Create firewall_group with name == reserved default fwg
```

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/common/fwaas_v2_client.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/common/fwaas_v2_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_base.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_manager.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/scenario/fwaas_v2_manager.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/scenario/test_fwaas_v2.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/scenario/test_fwaas_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/fwaas/services/v2_client.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/fwaas/services/v2_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions_negative.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/api/test_bgp_speaker_extensions_negative.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/README` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/README`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base_test_proto.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/base_test_proto.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/base.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_4byte_asn.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_4byte_asn.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_basic.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/basic/test_basic.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/test_ipv4.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv4/test_ipv4.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/test_ipv6.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/ipv6/test_ipv6.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/test_simple_bgp.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/neutron_dynamic_routing/scenario/test_simple_bgp.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/plugin.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/admin/test_floatingip.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/admin/test_floatingip.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/base.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,24 +70,22 @@
             cmd += "-c 'echo %s' " % msg
         else:
             cmd += "-e echo %s " % msg
     cmd += "< /dev/zero &{0}sleep 0.1{0}".format('\n')
     return cmd
 
 
-def get_ncat_client_cmd(ip_address, port, protocol):
-    udp = ''
-    if protocol.lower() == neutron_lib_constants.PROTO_NAME_UDP:
-        udp = '-u'
+def get_ncat_client_cmd(ip_address, port, protocol, ssh_client=None):
     cmd = 'echo "knock knock" | nc '
-    ncat_version = get_ncat_version()
-    if ncat_version > packaging_version.Version('7.60'):
-        cmd += '-z '
-    cmd += '-w 1 %(udp)s %(host)s %(port)s' % {
-        'udp': udp, 'host': ip_address, 'port': port}
+    if protocol.lower() == neutron_lib_constants.PROTO_NAME_UDP:
+        cmd += '-u '
+        ncat_version = get_ncat_version(ssh_client=ssh_client)
+        if ncat_version > packaging_version.Version('7.60'):
+            cmd += '-z '
+    cmd += '-w 1 %(host)s %(port)s' % {'host': ip_address, 'port': port}
     return cmd
 
 
 class BaseTempestTestCase(base_api.BaseNetworkTest):
 
     def create_server(self, flavor_ref, image_ref, key_name, networks,
                       **kwargs):
@@ -632,17 +630,17 @@
 
     def nc_client(self, ip_address, port, protocol, ssh_client=None):
         """Check connectivity to TCP/UDP port at host via nc.
 
         If ssh_client is not given, it is executed locally on host where tests
         are executed. Otherwise ssh_client object is used to execute it.
         """
-        cmd = get_ncat_client_cmd(ip_address, port, protocol)
-        result = shell.execute(cmd, ssh_client=ssh_client)
-        self.assertEqual(0, result.exit_status)
+        cmd = get_ncat_client_cmd(ip_address, port, protocol,
+                                  ssh_client=ssh_client)
+        result = shell.execute(cmd, ssh_client=ssh_client, check=False)
         return result.stdout
 
     def _ensure_public_router(self, client=None, tenant_id=None):
         """Retrieve a router for the given tenant id.
 
         If a public router has been configured, it will be returned.
```

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/constants.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/exceptions.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/exceptions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_basic.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_basic.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_connectivity.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_connectivity.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_dhcp.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_dhcp.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_dns_integration.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_dns_integration.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_dvr.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_dvr.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_fip64.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_fip64.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_floatingip.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_floatingip.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_internal_dns.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_internal_dns.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_ipv6.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_ipv6.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_local_ip.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_local_ip.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_mac_learning.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_mac_learning.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_metadata.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_metadata.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_migration.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_migration.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_mtu.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_mtu.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_multicast.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_multicast.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_port_forwardings.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_port_forwardings.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_ports.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_ports.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_portsecurity.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_portsecurity.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_qos.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_qos.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_security_groups.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_security_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_trunk.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_trunk.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/scenario/test_vlan_transparency.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/scenario/test_vlan_transparency.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/services/bgp/bgp_client.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/services/bgp/bgp_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/services/network/json/network_client.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/services/network/json/network_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/services/flowclassifier_client.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/services/flowclassifier_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/services/sfc_client.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/services/sfc_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/api/base.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/api/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/api/test_flowclassifier_extensions.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/api/test_flowclassifier_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/api/test_sfc_extensions.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/api/test_sfc_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/flowclassifier_client.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/flowclassifier_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/scenario/base.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/scenario/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/scenario/manager.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/scenario/manager.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/scenario/test_sfc.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/scenario/test_sfc.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/sfc/tests/sfc_client.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/sfc/tests/sfc_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/api/test_taas.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/api/test_taas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/base.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/base.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/scenario/manager.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/scenario/manager.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_taas.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_taas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_traffic_impact.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/scenario/test_traffic_impact.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/tap_as_a_service/services/taas_client.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/tap_as_a_service/services/taas_client.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/api/base_vpnaas.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/api/base_vpnaas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/api/test_vpnaas.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/api/test_vpnaas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/scenario/base_vpnaas.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/scenario/base_vpnaas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/scenario/test_vpnaas.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/scenario/test_vpnaas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin/vpnaas/services/clients_vpnaas.py` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin/vpnaas/services/clients_vpnaas.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin.egg-info/PKG-INFO` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-tempest-plugin
-Version: 2.3.0
+Version: 2.4.0
 Summary: Tempest plugin for Neutron Project
 Home-page: https://opendev.org/openstack/neutron-tempest-plugin
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ======================
         Neutron Tempest Plugin
```

### Comparing `neutron-tempest-plugin-2.3.0/neutron_tempest_plugin.egg-info/SOURCES.txt` & `neutron-tempest-plugin-2.4.0/neutron_tempest_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/releasenotes/source/README.rst` & `neutron-tempest-plugin-2.4.0/releasenotes/source/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/releasenotes/source/conf.py` & `neutron-tempest-plugin-2.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/requirements.txt` & `neutron-tempest-plugin-2.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/roles/docker-setup/files/docker_apparmor` & `neutron-tempest-plugin-2.4.0/roles/docker-setup/files/docker_apparmor`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/roles/docker-setup/tasks/main.yml` & `neutron-tempest-plugin-2.4.0/roles/docker-setup/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/roles/multi-node-setup/README.rst` & `neutron-tempest-plugin-2.4.0/roles/multi-node-setup/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/roles/multi-node-setup/tasks/main.yaml` & `neutron-tempest-plugin-2.4.0/roles/multi-node-setup/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/setup.cfg` & `neutron-tempest-plugin-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/setup.py` & `neutron-tempest-plugin-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/tools/customize_ubuntu_image` & `neutron-tempest-plugin-2.4.0/tools/customize_ubuntu_image`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/tools/misc-sanity-checks.sh` & `neutron-tempest-plugin-2.4.0/tools/misc-sanity-checks.sh`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/tox.ini` & `neutron-tempest-plugin-2.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/zuul.d/2023_1_jobs.yaml` & `neutron-tempest-plugin-2.4.0/zuul.d/2023_1_jobs.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
     parent: neutron-tempest-plugin-openvswitch
     override-checkout: stable/2023.1
     vars:
       network_api_extensions_openvswitch:
         - dhcp_agent_scheduler
         - local_ip
         - qos-bw-minimum-ingress
+        - port-resource-request
+        - port-resource-request-groups
       tempest_test_regex: "\
           (^neutron_tempest_plugin.api)|\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
       network_available_features: &available_features
         - ipv6_metadata
@@ -52,16 +54,14 @@
         - net-mtu
         - net-mtu-writable
         - network-ip-availability
         - network_availability_zone
         - network-segment-range
         - pagination
         - port-device-profile
-        - port-resource-request
-        - port-resource-request-groups
         - port-mac-address-regenerate
         - port-security
         - port-security-groups-filtering
         - project-id
         - provider
         - qos
         - qos-fip
@@ -102,18 +102,21 @@
               available_features: "{{ network_available_features | join(',') }}"
 
 - job:
     name: neutron-tempest-plugin-openvswitch-iptables_hybrid-2023-1
     parent: neutron-tempest-plugin-openvswitch-iptables_hybrid
     override-checkout: stable/2023.1
     vars:
+      network_api_extensions_common: *api_extensions
       network_api_extensions_openvswitch:
         - dhcp_agent_scheduler
         - local_ip
         - logging
+        - port-resource-request
+        - port-resource-request-groups
       network_available_features: *available_features
       tempest_test_regex: "\
           (^neutron_tempest_plugin.api)|\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
       # TODO(slaweq): remove trunks subport_connectivity test from blacklist
@@ -153,14 +156,15 @@
         NEUTRON_ENFORCE_SCOPE: true
 
 - job:
     name: neutron-tempest-plugin-linuxbridge-2023-1
     parent: neutron-tempest-plugin-linuxbridge
     override-checkout: stable/2023.1
     vars:
+      network_api_extensions_common: *api_extensions
       network_api_extensions_linuxbridge:
         - dhcp_agent_scheduler
         - vlan-transparent
       network_available_features: *available_features
       tempest_test_regex: "\
           (^neutron_tempest_plugin.api)|\
           (^neutron_tempest_plugin.scenario)|\
```

### Comparing `neutron-tempest-plugin-2.3.0/zuul.d/master_jobs.yaml` & `neutron-tempest-plugin-2.4.0/zuul.d/master_jobs.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1113,32 +1113,15 @@
         neutron-tempest-plugin: https://opendev.org/openstack/neutron-tempest-plugin
       network_api_extensions_bgp:
         - bgp
         - bgp_dragent_scheduler
         - bgp_4byte_asn
       devstack_localrc:
         NETWORK_API_EXTENSIONS: "{{ (network_api_extensions_common + network_api_extensions_bgp) | join(',') }}"
-        Q_AGENT: openvswitch
-        Q_ML2_TENANT_NETWORK_TYPE: vxlan
-        Q_ML2_PLUGIN_MECHANISM_DRIVERS: openvswitch
       devstack_services:
-        # Disable OVN services
-        br-ex-tcpdump: false
-        br-int-flows: false
-        ovn-controller: false
-        ovn-northd: false
-        ovs-vswitchd: false
-        ovsdb-server: false
-        q-ovn-metadata-agent: false
-        # Neutron services
-        q-agt: true
-        q-dhcp: true
-        q-meta: true
-        q-metering: true
-        q-l3: true
         neutron-dr: true
         neutron-dr-agent: true
       tempest_concurrency: 1
       tempest_test_regex: ^neutron_tempest_plugin\.neutron_dynamic_routing
     irrelevant-files:
       - ^\.pylintrc$
       - ^(test-|)requirements.txt$
```

### Comparing `neutron-tempest-plugin-2.3.0/zuul.d/project.yaml` & `neutron-tempest-plugin-2.4.0/zuul.d/project.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -176,48 +176,42 @@
       jobs:
         - neutron-tempest-plugin-dvr-multinode-scenario-2023-1
 
 - project:
     templates:
       - build-openstack-docs-pti
       - neutron-tempest-plugin-jobs
-      - neutron-tempest-plugin-jobs-xena
       - neutron-tempest-plugin-jobs-yoga
       - neutron-tempest-plugin-jobs-zed
       - neutron-tempest-plugin-jobs-2023-1
       - check-requirements
       - tempest-plugin-jobs
       - release-notes-jobs-python3
     check:
       jobs:
         - neutron-tempest-plugin-sfc
-        - neutron-tempest-plugin-sfc-xena
         - neutron-tempest-plugin-sfc-yoga
         - neutron-tempest-plugin-sfc-zed
         - neutron-tempest-plugin-sfc-2023-1
         - neutron-tempest-plugin-bgpvpn-bagpipe
-        - neutron-tempest-plugin-bgpvpn-bagpipe-xena
         - neutron-tempest-plugin-bgpvpn-bagpipe-yoga
         - neutron-tempest-plugin-bgpvpn-bagpipe-zed
         - neutron-tempest-plugin-bgpvpn-bagpipe-2023-1
         - neutron-tempest-plugin-dynamic-routing
-        - neutron-tempest-plugin-dynamic-routing-xena
         - neutron-tempest-plugin-dynamic-routing-yoga
         - neutron-tempest-plugin-dynamic-routing-zed
         - neutron-tempest-plugin-dynamic-routing-2023-1
         - neutron-tempest-plugin-fwaas
         - neutron-tempest-plugin-fwaas-zed
         - neutron-tempest-plugin-fwaas-2023-1
         - neutron-tempest-plugin-vpnaas
-        - neutron-tempest-plugin-vpnaas-xena
         - neutron-tempest-plugin-vpnaas-yoga
         - neutron-tempest-plugin-vpnaas-zed
         - neutron-tempest-plugin-vpnaas-2023-1
         - neutron-tempest-plugin-tap-as-a-service
-        - neutron-tempest-plugin-tap-as-a-service-xena
         - neutron-tempest-plugin-tap-as-a-service-yoga
         - neutron-tempest-plugin-tap-as-a-service-zed
         - neutron-tempest-plugin-tap-as-a-service-2023-1
 
     gate:
       jobs:
         - neutron-tempest-plugin-sfc
```

### Comparing `neutron-tempest-plugin-2.3.0/zuul.d/train_jobs.yaml` & `neutron-tempest-plugin-2.4.0/zuul.d/train_jobs.yaml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/zuul.d/ussuri_jobs.yaml` & `neutron-tempest-plugin-2.4.0/zuul.d/ussuri_jobs.yaml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/zuul.d/victoria_jobs.yaml` & `neutron-tempest-plugin-2.4.0/zuul.d/victoria_jobs.yaml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/zuul.d/wallaby_jobs.yaml` & `neutron-tempest-plugin-2.4.0/zuul.d/wallaby_jobs.yaml`

 * *Files identical despite different names*

### Comparing `neutron-tempest-plugin-2.3.0/zuul.d/xena_jobs.yaml` & `neutron-tempest-plugin-2.4.0/zuul.d/yoga_jobs.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 - job:
-    name: neutron-tempest-plugin-api-xena
+    name: neutron-tempest-plugin-api-yoga
     parent: neutron-tempest-plugin-base
     nodeset: openstack-single-node-focal
-    override-checkout: stable/xena
+    override-checkout: stable/yoga
     vars:
       tempest_concurrency: 4
       tempest_test_regex: ^neutron_tempest_plugin\.api
       # TODO(slaweq): find a way to put this list of extensions in
       # neutron repository and keep it different per branch,
       # then it could be removed from here
       network_api_extensions_common: &api_extensions
@@ -47,14 +47,15 @@
         - net-mtu-writable
         - network-ip-availability
         - network_availability_zone
         - network-segment-range
         - pagination
         - port-device-profile
         - port-resource-request
+        - port-resource-request-groups
         - port-mac-address-regenerate
         - port-security
         - port-security-groups-filtering
         - project-id
         - provider
         - qos
         - qos-bw-minimum-ingress
@@ -75,69 +76,73 @@
         - service-type
         - sorting
         - standard-attr-description
         - standard-attr-revisions
         - standard-attr-segment
         - standard-attr-tag
         - standard-attr-timestamp
+        - stateful-security-group
         - subnet_allocation
         - subnet-dns-publish-fixed-ip
         - subnet-service-types
         - subnetpool-prefix-ops
         - tag-ports-during-bulk-creation
         - trunk
         - trunk-details
         - uplink-status-propagation
       network_api_extensions_tempest:
         - dvr
       network_available_features: &available_features
         - ipv6_metadata
 
 - job:
-    name: neutron-tempest-plugin-scenario-openvswitch-xena
+    name: neutron-tempest-plugin-scenario-openvswitch-yoga
     parent: neutron-tempest-plugin-openvswitch
-    override-checkout: stable/xena
+    override-checkout: stable/yoga
+    nodeset: neutron-nested-virt-ubuntu-focal
     vars:
       tempest_test_regex: "\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
       network_api_extensions: *api_extensions
       network_available_features: *available_features
       devstack_localrc:
-        NETWORK_API_EXTENSIONS: "{{ network_api_extensions | join(',') }}"
+        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions + network_api_extensions_openvswitch) | join(',') }}"
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             network-feature-enabled:
               available_features: "{{ network_available_features | join(',') }}"
 
 - job:
-    name: neutron-tempest-plugin-scenario-openvswitch-iptables_hybrid-xena
+    name: neutron-tempest-plugin-scenario-openvswitch-iptables_hybrid-yoga
     parent: neutron-tempest-plugin-openvswitch-iptables_hybrid
-    override-checkout: stable/xena
+    override-checkout: stable/yoga
+    nodeset: neutron-nested-virt-ubuntu-focal
     vars:
       tempest_test_regex: "\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
       network_api_extensions: *api_extensions
       network_available_features: *available_features
       devstack_localrc:
-        NETWORK_API_EXTENSIONS: "{{ network_api_extensions | join(',') }}"
+        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions + network_api_extensions_openvswitch) | join(',') }}"
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             network-feature-enabled:
               available_features: "{{ network_available_features | join(',') }}"
 
 - job:
-    name: neutron-tempest-plugin-scenario-linuxbridge-xena
+    name: neutron-tempest-plugin-scenario-linuxbridge-yoga
     parent: neutron-tempest-plugin-linuxbridge
-    override-checkout: stable/xena
+    override-checkout: stable/yoga
+    nodeset: neutron-nested-virt-ubuntu-focal
     vars:
       tempest_test_regex: "\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
       network_api_extensions: *api_extensions
       network_available_features: *available_features
@@ -146,78 +151,104 @@
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             network-feature-enabled:
               available_features: "{{ network_available_features | join(',') }}"
 
 - job:
-    name: neutron-tempest-plugin-scenario-ovn-xena
+    name: neutron-tempest-plugin-scenario-ovn-yoga
     parent: neutron-tempest-plugin-ovn
-    override-checkout: stable/xena
+    override-checkout: stable/yoga
+    nodeset: neutron-nested-virt-ubuntu-focal
     vars:
       tempest_test_regex: "\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
       network_api_extensions: *api_extensions
+      network_api_extensions_ovn:
+        - vlan-transparent
       devstack_localrc:
-        NETWORK_API_EXTENSIONS: "{{ network_api_extensions | join(',') }}"
+        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions + network_api_extensions_ovn) | join(',') }}"
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             network-feature-enabled:
               available_features: ""
 
 - job:
-    name: neutron-tempest-plugin-dvr-multinode-scenario-xena
+    name: neutron-tempest-plugin-dvr-multinode-scenario-yoga
     parent: neutron-tempest-plugin-dvr-multinode-scenario
     nodeset: openstack-two-node-focal
-    override-checkout: stable/xena
+    override-checkout: stable/yoga
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-designate-scenario-xena
+    name: neutron-tempest-plugin-designate-scenario-yoga
     parent: neutron-tempest-plugin-designate-scenario
-    override-checkout: stable/xena
+    override-checkout: stable/yoga
+    nodeset: neutron-nested-virt-ubuntu-focal
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-sfc-xena
+    name: neutron-tempest-plugin-sfc-yoga
     parent: neutron-tempest-plugin-sfc
     nodeset: openstack-single-node-focal
-    override-checkout: stable/xena
+    override-checkout: stable/yoga
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-bgpvpn-bagpipe-xena
+    name: neutron-tempest-plugin-bgpvpn-bagpipe-yoga
     parent: neutron-tempest-plugin-bgpvpn-bagpipe
     nodeset: openstack-single-node-focal
-    override-checkout: stable/xena
+    override-checkout: stable/yoga
     vars:
       network_api_extensions: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-dynamic-routing-xena
+    name: neutron-tempest-plugin-dynamic-routing-yoga
     parent: neutron-tempest-plugin-dynamic-routing
     nodeset: openstack-single-node-focal
-    override-checkout: stable/xena
+    override-checkout: stable/yoga
     vars:
       network_api_extensions_common: *api_extensions
+      devstack_localrc:
+        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions_common + network_api_extensions_bgp) | join(',') }}"
+        Q_AGENT: openvswitch
+        Q_ML2_TENANT_NETWORK_TYPE: vxlan
+        Q_ML2_PLUGIN_MECHANISM_DRIVERS: openvswitch
+      devstack_services:
+        # Disable OVN services
+        br-ex-tcpdump: false
+        br-int-flows: false
+        ovn-controller: false
+        ovn-northd: false
+        ovs-vswitchd: false
+        ovsdb-server: false
+        q-ovn-metadata-agent: false
+        # Neutron services
+        q-agt: true
+        q-dhcp: true
+        q-meta: true
+        q-metering: true
+        q-l3: true
+        neutron-dr: true
+        neutron-dr-agent: true
 
 - job:
-    name: neutron-tempest-plugin-vpnaas-xena
+    name: neutron-tempest-plugin-vpnaas-yoga
     parent: neutron-tempest-plugin-vpnaas
     nodeset: openstack-single-node-focal
-    override-checkout: stable/xena
+    override-checkout: stable/yoga
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-tap-as-a-service-xena
+    name: neutron-tempest-plugin-tap-as-a-service-yoga
     parent: neutron-tempest-plugin-tap-as-a-service
     nodeset: openstack-single-node-focal
-    override-checkout: stable/xena
+    override-checkout: stable/yoga
     vars:
       network_api_extensions_common: *api_extensions
```

### Comparing `neutron-tempest-plugin-2.3.0/zuul.d/yoga_jobs.yaml` & `neutron-tempest-plugin-2.4.0/zuul.d/zed_jobs.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 - job:
-    name: neutron-tempest-plugin-api-yoga
-    parent: neutron-tempest-plugin-base
-    nodeset: openstack-single-node-focal
-    override-checkout: stable/yoga
+    name: neutron-tempest-plugin-openvswitch-zed
+    parent: neutron-tempest-plugin-openvswitch
+    override-checkout: stable/zed
+    nodeset: neutron-nested-virt-ubuntu-focal
     vars:
-      tempest_concurrency: 4
-      tempest_test_regex: ^neutron_tempest_plugin\.api
-      # TODO(slaweq): find a way to put this list of extensions in
-      # neutron repository and keep it different per branch,
-      # then it could be removed from here
+      network_api_extensions_openvswitch:
+        - local_ip
+        - port-resource-request
+        - port-resource-request-groups
+        - qos-bw-minimum-ingress
+      tempest_test_regex: "\
+          (^neutron_tempest_plugin.api)|\
+          (^neutron_tempest_plugin.scenario)|\
+          (^tempest.api.compute.servers.test_attach_interfaces)|\
+          (^tempest.api.compute.servers.test_multiple_create)"
       network_api_extensions_common: &api_extensions
         - address-group
         - address-scope
         - agent
         - allowed-address-pairs
         - auto-allocated-topology
         - availability_zone
@@ -30,32 +35,32 @@
         - extra_dhcp_opt
         - extraroute
         - extraroute-atomic
         - filter-validation
         - fip-port-details
         - flavors
         - floating-ip-port-forwarding
+        - floating-ip-port-forwarding-detail
         - floatingip-pools
         - ip-substring-filtering
         - l3-conntrack-helper
+        - l3-ext-ndp-proxy
         - l3-flavors
         - l3-ha
+        - l3-ndp-proxy
         - l3_agent_scheduler
-        - logging
         - metering
         - multi-provider
         - net-mtu
         - net-mtu-writable
         - network-ip-availability
         - network_availability_zone
         - network-segment-range
         - pagination
         - port-device-profile
-        - port-resource-request
-        - port-resource-request-groups
         - port-mac-address-regenerate
         - port-security
         - port-security-groups-filtering
         - project-id
         - provider
         - qos
         - qos-bw-minimum-ingress
@@ -64,15 +69,14 @@
         - quota_details
         - rbac-address-group
         - rbac-address-scope
         - rbac-policies
         - rbac-security-groups
         - rbac-subnetpool
         - router
-        - router-admin-state-down-before-update
         - router_availability_zone
         - security-group
         - security-groups-remote-address-group
         - segment
         - service-type
         - sorting
         - standard-attr-description
@@ -85,143 +89,188 @@
         - subnet-dns-publish-fixed-ip
         - subnet-service-types
         - subnetpool-prefix-ops
         - tag-ports-during-bulk-creation
         - trunk
         - trunk-details
         - uplink-status-propagation
-      network_api_extensions_tempest:
-        - dvr
       network_available_features: &available_features
         - ipv6_metadata
-
-- job:
-    name: neutron-tempest-plugin-scenario-openvswitch-yoga
-    parent: neutron-tempest-plugin-openvswitch
-    override-checkout: stable/yoga
-    vars:
-      tempest_test_regex: "\
-          (^neutron_tempest_plugin.scenario)|\
-          (^tempest.api.compute.servers.test_attach_interfaces)|\
-          (^tempest.api.compute.servers.test_multiple_create)"
-      network_api_extensions: *api_extensions
-      network_available_features: *available_features
       devstack_localrc:
-        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions + network_api_extensions_openvswitch) | join(',') }}"
+        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions_common + network_api_extensions_openvswitch) | join(',') }}"
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             network-feature-enabled:
               available_features: "{{ network_available_features | join(',') }}"
 
 - job:
-    name: neutron-tempest-plugin-scenario-openvswitch-iptables_hybrid-yoga
+    name: neutron-tempest-plugin-openvswitch-iptables_hybrid-zed
     parent: neutron-tempest-plugin-openvswitch-iptables_hybrid
-    override-checkout: stable/yoga
+    override-checkout: stable/zed
+    nodeset: neutron-nested-virt-ubuntu-focal
     vars:
+      network_api_extensions_common: *api_extensions
+      network_api_extensions_openvswitch:
+        - local_ip
+        - logging
+        - port-resource-request
+        - port-resource-request-groups
       tempest_test_regex: "\
+          (^neutron_tempest_plugin.api)|\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
-      network_api_extensions: *api_extensions
+      # TODO(slaweq): remove trunks subport_connectivity test from blacklist
+      # when bug https://bugs.launchpad.net/neutron/+bug/1838760 will be fixed
+      # TODO(akatz): remove established tcp session verification test when the
+      # bug https://bugzilla.redhat.com/show_bug.cgi?id=1965036 will be fixed
+      tempest_exclude_regex: "\
+          (^neutron_tempest_plugin.scenario.test_trunk.TrunkTest.test_subport_connectivity)|\
+          (^neutron_tempest_plugin.scenario.test_security_groups.StatefulNetworkSecGroupTest.test_established_tcp_session_after_re_attachinging_sg)|\
+          (^neutron_tempest_plugin.scenario.test_security_groups.StatelessNetworkSecGroupTest.test_established_tcp_session_after_re_attachinging_sg)"
       network_available_features: *available_features
       devstack_localrc:
-        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions + network_api_extensions_openvswitch) | join(',') }}"
+        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions_common + network_api_extensions_openvswitch) | join(',') }}"
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             network-feature-enabled:
               available_features: "{{ network_available_features | join(',') }}"
 
 - job:
-    name: neutron-tempest-plugin-scenario-linuxbridge-yoga
+    name: neutron-tempest-plugin-linuxbridge-zed
     parent: neutron-tempest-plugin-linuxbridge
-    override-checkout: stable/yoga
+    override-checkout: stable/zed
+    nodeset: neutron-nested-virt-ubuntu-focal
     vars:
+      network_api_extensions_common: *api_extensions
+      network_api_extensions_linuxbridge:
+        - vlan-transparent
       tempest_test_regex: "\
+          (^neutron_tempest_plugin.api)|\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
-      network_api_extensions: *api_extensions
+      tempest_exclude_regex: "\
+          (^neutron_tempest_plugin.scenario.test_vlan_transparency.VlanTransparencyTest)|\
+          (^neutron_tempest_plugin.scenario.test_security_groups.StatefulNetworkSecGroupTest.test_established_tcp_session_after_re_attachinging_sg)|\
+          (^neutron_tempest_plugin.scenario.test_security_groups.StatelessNetworkSecGroupTest.test_established_tcp_session_after_re_attachinging_sg)|\
+          (^neutron_tempest_plugin.scenario.test_floatingip.FloatingIPPortDetailsTest.test_floatingip_port_details)"
       network_available_features: *available_features
       devstack_localrc:
-        NETWORK_API_EXTENSIONS: "{{ network_api_extensions | join(',') }}"
+        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions_common + network_api_extensions_linuxbridge) | join(',') }}"
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             network-feature-enabled:
               available_features: "{{ network_available_features | join(',') }}"
 
 - job:
-    name: neutron-tempest-plugin-scenario-ovn-yoga
+    name: neutron-tempest-plugin-ovn-zed
     parent: neutron-tempest-plugin-ovn
-    override-checkout: stable/yoga
+    override-checkout: stable/zed
+    nodeset: neutron-nested-virt-ubuntu-focal
     vars:
       tempest_test_regex: "\
+          (^neutron_tempest_plugin.api)|\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
+      tempest_exclude_regex: "\
+          (^neutron_tempest_plugin.scenario.test_mtu.NetworkWritableMtuTest)"
       network_api_extensions: *api_extensions
       network_api_extensions_ovn:
         - vlan-transparent
       devstack_localrc:
         NETWORK_API_EXTENSIONS: "{{ (network_api_extensions + network_api_extensions_ovn) | join(',') }}"
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             network-feature-enabled:
               available_features: ""
 
 - job:
-    name: neutron-tempest-plugin-dvr-multinode-scenario-yoga
+    name: neutron-tempest-plugin-dvr-multinode-scenario-zed
     parent: neutron-tempest-plugin-dvr-multinode-scenario
     nodeset: openstack-two-node-focal
-    override-checkout: stable/yoga
+    override-checkout: stable/zed
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-designate-scenario-yoga
+    name: neutron-tempest-plugin-designate-scenario-zed
     parent: neutron-tempest-plugin-designate-scenario
-    override-checkout: stable/yoga
+    override-checkout: stable/zed
+    nodeset: neutron-nested-virt-ubuntu-focal
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-sfc-yoga
+    name: neutron-tempest-plugin-sfc-zed
     parent: neutron-tempest-plugin-sfc
     nodeset: openstack-single-node-focal
-    override-checkout: stable/yoga
+    override-checkout: stable/zed
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-bgpvpn-bagpipe-yoga
+    name: neutron-tempest-plugin-bgpvpn-bagpipe-zed
     parent: neutron-tempest-plugin-bgpvpn-bagpipe
     nodeset: openstack-single-node-focal
-    override-checkout: stable/yoga
+    override-checkout: stable/zed
     vars:
       network_api_extensions: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-dynamic-routing-yoga
+    name: neutron-tempest-plugin-dynamic-routing-zed
     parent: neutron-tempest-plugin-dynamic-routing
     nodeset: openstack-single-node-focal
-    override-checkout: stable/yoga
+    override-checkout: stable/zed
+    vars:
+      network_api_extensions_common: *api_extensions
+      devstack_localrc:
+        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions_common + network_api_extensions_bgp) | join(',') }}"
+        Q_AGENT: openvswitch
+        Q_ML2_TENANT_NETWORK_TYPE: vxlan
+        Q_ML2_PLUGIN_MECHANISM_DRIVERS: openvswitch
+      devstack_services:
+        # Disable OVN services
+        br-ex-tcpdump: false
+        br-int-flows: false
+        ovn-controller: false
+        ovn-northd: false
+        ovs-vswitchd: false
+        ovsdb-server: false
+        q-ovn-metadata-agent: false
+        # Neutron services
+        q-agt: true
+        q-dhcp: true
+        q-meta: true
+        q-metering: true
+        q-l3: true
+        neutron-dr: true
+        neutron-dr-agent: true
+
+- job:
+    name: neutron-tempest-plugin-fwaas-zed
+    parent: neutron-tempest-plugin-fwaas
+    nodeset: openstack-single-node-focal
+    override-checkout: stable/zed
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-vpnaas-yoga
+    name: neutron-tempest-plugin-vpnaas-zed
     parent: neutron-tempest-plugin-vpnaas
     nodeset: openstack-single-node-focal
-    override-checkout: stable/yoga
+    override-checkout: stable/zed
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-tap-as-a-service-yoga
+    name: neutron-tempest-plugin-tap-as-a-service-zed
     parent: neutron-tempest-plugin-tap-as-a-service
     nodeset: openstack-single-node-focal
-    override-checkout: stable/yoga
+    override-checkout: stable/zed
     vars:
       network_api_extensions_common: *api_extensions
```

### Comparing `neutron-tempest-plugin-2.3.0/zuul.d/zed_jobs.yaml` & `neutron-tempest-plugin-2.4.0/zuul.d/xena_jobs.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 - job:
-    name: neutron-tempest-plugin-openvswitch-zed
-    parent: neutron-tempest-plugin-openvswitch
-    override-checkout: stable/zed
-    vars:
-      network_api_extensions_openvswitch:
-        - local_ip
-        - qos-bw-minimum-ingress
-      tempest_test_regex: "\
-          (^neutron_tempest_plugin.api)|\
-          (^neutron_tempest_plugin.scenario)|\
-          (^tempest.api.compute.servers.test_attach_interfaces)|\
-          (^tempest.api.compute.servers.test_multiple_create)"
+    name: neutron-tempest-plugin-api-xena
+    parent: neutron-tempest-plugin-base
+    nodeset: openstack-single-node-focal
+    override-checkout: stable/xena
+    required-projects: &required-projects-xena
+      - openstack/neutron
+      - name: openstack/neutron-tempest-plugin
+        override-checkout: 2.3.0
+      - openstack/tempest
+    vars:
+      tempest_concurrency: 4
+      tempest_test_regex: ^neutron_tempest_plugin\.api
+      # TODO(slaweq): find a way to put this list of extensions in
+      # neutron repository and keep it different per branch,
+      # then it could be removed from here
       network_api_extensions_common: &api_extensions
         - address-group
         - address-scope
         - agent
         - allowed-address-pairs
         - auto-allocated-topology
         - availability_zone
@@ -32,35 +35,31 @@
         - extra_dhcp_opt
         - extraroute
         - extraroute-atomic
         - filter-validation
         - fip-port-details
         - flavors
         - floating-ip-port-forwarding
-        - floating-ip-port-forwarding-detail
         - floatingip-pools
         - ip-substring-filtering
         - l3-conntrack-helper
-        - l3-ext-ndp-proxy
         - l3-flavors
         - l3-ha
-        - l3-ndp-proxy
         - l3_agent_scheduler
         - logging
         - metering
         - multi-provider
         - net-mtu
         - net-mtu-writable
         - network-ip-availability
         - network_availability_zone
         - network-segment-range
         - pagination
         - port-device-profile
         - port-resource-request
-        - port-resource-request-groups
         - port-mac-address-regenerate
         - port-security
         - port-security-groups-filtering
         - project-id
         - provider
         - qos
         - qos-bw-minimum-ingress
@@ -69,178 +68,194 @@
         - quota_details
         - rbac-address-group
         - rbac-address-scope
         - rbac-policies
         - rbac-security-groups
         - rbac-subnetpool
         - router
+        - router-admin-state-down-before-update
         - router_availability_zone
         - security-group
         - security-groups-remote-address-group
         - segment
         - service-type
         - sorting
         - standard-attr-description
         - standard-attr-revisions
         - standard-attr-segment
         - standard-attr-tag
         - standard-attr-timestamp
-        - stateful-security-group
         - subnet_allocation
         - subnet-dns-publish-fixed-ip
         - subnet-service-types
         - subnetpool-prefix-ops
         - tag-ports-during-bulk-creation
         - trunk
         - trunk-details
         - uplink-status-propagation
+      network_api_extensions_tempest:
+        - dvr
       network_available_features: &available_features
         - ipv6_metadata
+
+- job:
+    name: neutron-tempest-plugin-scenario-openvswitch-xena
+    parent: neutron-tempest-plugin-openvswitch
+    override-checkout: stable/xena
+    required-projects: *required-projects-xena
+    vars:
+      tempest_test_regex: "\
+          (^neutron_tempest_plugin.scenario)|\
+          (^tempest.api.compute.servers.test_attach_interfaces)|\
+          (^tempest.api.compute.servers.test_multiple_create)"
+      network_api_extensions: *api_extensions
+      network_available_features: *available_features
       devstack_localrc:
-        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions_common + network_api_extensions_openvswitch) | join(',') }}"
+        NETWORK_API_EXTENSIONS: "{{ network_api_extensions | join(',') }}"
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             network-feature-enabled:
               available_features: "{{ network_available_features | join(',') }}"
 
 - job:
-    name: neutron-tempest-plugin-openvswitch-iptables_hybrid-zed
+    name: neutron-tempest-plugin-scenario-openvswitch-iptables_hybrid-xena
     parent: neutron-tempest-plugin-openvswitch-iptables_hybrid
-    override-checkout: stable/zed
+    override-checkout: stable/xena
+    required-projects: *required-projects-xena
     vars:
-      network_api_extensions_openvswitch:
-        - local_ip
-        - logging
       tempest_test_regex: "\
-          (^neutron_tempest_plugin.api)|\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
-      # TODO(slaweq): remove trunks subport_connectivity test from blacklist
-      # when bug https://bugs.launchpad.net/neutron/+bug/1838760 will be fixed
-      # TODO(akatz): remove established tcp session verification test when the
-      # bug https://bugzilla.redhat.com/show_bug.cgi?id=1965036 will be fixed
-      tempest_exclude_regex: "\
-          (^neutron_tempest_plugin.scenario.test_trunk.TrunkTest.test_subport_connectivity)|\
-          (^neutron_tempest_plugin.scenario.test_security_groups.StatefulNetworkSecGroupTest.test_established_tcp_session_after_re_attachinging_sg)|\
-          (^neutron_tempest_plugin.scenario.test_security_groups.StatelessNetworkSecGroupTest.test_established_tcp_session_after_re_attachinging_sg)"
+      network_api_extensions: *api_extensions
       network_available_features: *available_features
       devstack_localrc:
-        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions_common + network_api_extensions_openvswitch) | join(',') }}"
+        NETWORK_API_EXTENSIONS: "{{ network_api_extensions | join(',') }}"
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             network-feature-enabled:
               available_features: "{{ network_available_features | join(',') }}"
 
 - job:
-    name: neutron-tempest-plugin-linuxbridge-zed
+    name: neutron-tempest-plugin-scenario-linuxbridge-xena
     parent: neutron-tempest-plugin-linuxbridge
-    override-checkout: stable/zed
+    override-checkout: stable/xena
+    required-projects: *required-projects-xena
     vars:
-      network_api_extensions_linuxbridge:
-        - vlan-transparent
       tempest_test_regex: "\
-          (^neutron_tempest_plugin.api)|\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
-      tempest_exclude_regex: "\
-          (^neutron_tempest_plugin.scenario.test_vlan_transparency.VlanTransparencyTest)|\
-          (^neutron_tempest_plugin.scenario.test_security_groups.StatefulNetworkSecGroupTest.test_established_tcp_session_after_re_attachinging_sg)|\
-          (^neutron_tempest_plugin.scenario.test_security_groups.StatelessNetworkSecGroupTest.test_established_tcp_session_after_re_attachinging_sg)|\
-          (^neutron_tempest_plugin.scenario.test_floatingip.FloatingIPPortDetailsTest.test_floatingip_port_details)"
+      network_api_extensions: *api_extensions
       network_available_features: *available_features
       devstack_localrc:
-        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions_common + network_api_extensions_linuxbridge) | join(',') }}"
+        NETWORK_API_EXTENSIONS: "{{ network_api_extensions | join(',') }}"
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             network-feature-enabled:
               available_features: "{{ network_available_features | join(',') }}"
 
 - job:
-    name: neutron-tempest-plugin-ovn-zed
+    name: neutron-tempest-plugin-scenario-ovn-xena
     parent: neutron-tempest-plugin-ovn
-    override-checkout: stable/zed
+    override-checkout: stable/xena
+    required-projects: *required-projects-xena
     vars:
       tempest_test_regex: "\
-          (^neutron_tempest_plugin.api)|\
           (^neutron_tempest_plugin.scenario)|\
           (^tempest.api.compute.servers.test_attach_interfaces)|\
           (^tempest.api.compute.servers.test_multiple_create)"
-      tempest_exclude_regex: "\
-          (^neutron_tempest_plugin.scenario.test_mtu.NetworkWritableMtuTest)"
       network_api_extensions: *api_extensions
-      network_api_extensions_ovn:
-        - vlan-transparent
       devstack_localrc:
-        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions + network_api_extensions_ovn) | join(',') }}"
+        NETWORK_API_EXTENSIONS: "{{ network_api_extensions | join(',') }}"
       devstack_local_conf:
         test-config:
           $TEMPEST_CONFIG:
             network-feature-enabled:
               available_features: ""
 
 - job:
-    name: neutron-tempest-plugin-dvr-multinode-scenario-zed
+    name: neutron-tempest-plugin-dvr-multinode-scenario-xena
     parent: neutron-tempest-plugin-dvr-multinode-scenario
     nodeset: openstack-two-node-focal
-    override-checkout: stable/zed
+    override-checkout: stable/xena
+    required-projects: *required-projects-xena
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-designate-scenario-zed
+    name: neutron-tempest-plugin-designate-scenario-xena
     parent: neutron-tempest-plugin-designate-scenario
-    override-checkout: stable/zed
+    override-checkout: stable/xena
+    required-projects: *required-projects-xena
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-sfc-zed
+    name: neutron-tempest-plugin-sfc-xena
     parent: neutron-tempest-plugin-sfc
     nodeset: openstack-single-node-focal
-    override-checkout: stable/zed
+    override-checkout: stable/xena
+    required-projects: *required-projects-xena
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-bgpvpn-bagpipe-zed
+    name: neutron-tempest-plugin-bgpvpn-bagpipe-xena
     parent: neutron-tempest-plugin-bgpvpn-bagpipe
     nodeset: openstack-single-node-focal
-    override-checkout: stable/zed
+    override-checkout: stable/xena
+    required-projects: *required-projects-xena
     vars:
       network_api_extensions: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-dynamic-routing-zed
+    name: neutron-tempest-plugin-dynamic-routing-xena
     parent: neutron-tempest-plugin-dynamic-routing
     nodeset: openstack-single-node-focal
-    override-checkout: stable/zed
-    vars:
-      network_api_extensions_common: *api_extensions
-
-- job:
-    name: neutron-tempest-plugin-fwaas-zed
-    parent: neutron-tempest-plugin-fwaas
-    nodeset: openstack-single-node-focal
-    override-checkout: stable/zed
+    override-checkout: stable/xena
+    required-projects: *required-projects-xena
     vars:
       network_api_extensions_common: *api_extensions
+      devstack_localrc:
+        NETWORK_API_EXTENSIONS: "{{ (network_api_extensions_common + network_api_extensions_bgp) | join(',') }}"
+        Q_AGENT: openvswitch
+        Q_ML2_TENANT_NETWORK_TYPE: vxlan
+        Q_ML2_PLUGIN_MECHANISM_DRIVERS: openvswitch
+      devstack_services:
+        # Disable OVN services
+        br-ex-tcpdump: false
+        br-int-flows: false
+        ovn-controller: false
+        ovn-northd: false
+        ovs-vswitchd: false
+        ovsdb-server: false
+        q-ovn-metadata-agent: false
+        # Neutron services
+        q-agt: true
+        q-dhcp: true
+        q-meta: true
+        q-metering: true
+        q-l3: true
+        neutron-dr: true
+        neutron-dr-agent: true
 
 - job:
-    name: neutron-tempest-plugin-vpnaas-zed
+    name: neutron-tempest-plugin-vpnaas-xena
     parent: neutron-tempest-plugin-vpnaas
     nodeset: openstack-single-node-focal
-    override-checkout: stable/zed
+    override-checkout: stable/xena
+    required-projects: *required-projects-xena
     vars:
       network_api_extensions_common: *api_extensions
 
 - job:
-    name: neutron-tempest-plugin-tap-as-a-service-zed
+    name: neutron-tempest-plugin-tap-as-a-service-xena
     parent: neutron-tempest-plugin-tap-as-a-service
     nodeset: openstack-single-node-focal
-    override-checkout: stable/zed
+    override-checkout: stable/xena
+    required-projects: *required-projects-xena
     vars:
       network_api_extensions_common: *api_extensions
```


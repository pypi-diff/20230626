# Comparing `tmp/p2pd-2.5.0.tar.gz` & `tmp/p2pd-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2pd-2.5.0.tar", last modified: Sun May 28 08:39:20 2023, max compression
+gzip compressed data, was "p2pd-2.6.0.tar", last modified: Mon Jun 26 06:28:16 2023, max compression
```

## Comparing `p2pd-2.5.0.tar` & `p2pd-2.6.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-28 08:39:20.539903 p2pd-2.5.0/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1570 2023-04-28 06:42:33.000000 p2pd-2.5.0/CREDITS.md
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1072 2023-04-28 06:42:33.000000 p2pd-2.5.0/LICENSE
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      106 2023-05-01 10:43:45.000000 p2pd-2.5.0/MANIFEST.in
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-05-28 08:39:20.539903 p2pd-2.5.0/PKG-INFO
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2707 2023-05-01 10:43:45.000000 p2pd-2.5.0/README.md
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-28 08:39:20.531903 p2pd-2.5.0/p2pd/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1196 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/__init__.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7065 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/ack_udp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6437 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/address.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    30620 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/base_stream.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8028 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/clock_skew.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8004 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/cmd_tools.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7896 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/daemon.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      303 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/echo_server.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      222 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/errors.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5601 2023-05-19 04:37:59.000000 p2pd-2.5.0/p2pd/http_client_lib.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5968 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/http_server_lib.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    22201 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/interface.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11971 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/ip_range.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5784 2023-05-19 04:37:59.000000 p2pd-2.5.0/p2pd/name_store.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    29608 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/nat.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9208 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/nat_test.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    23607 2023-05-19 04:37:59.000000 p2pd-2.5.0/p2pd/net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4438 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/netiface_extra.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13979 2023-05-01 10:43:45.000000 p2pd-2.5.0/p2pd/ntp_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6624 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/p2p_addr.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13522 2023-05-01 10:43:45.000000 p2pd-2.5.0/p2pd/p2p_node.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    26320 2023-04-30 18:46:46.000000 p2pd-2.5.0/p2pd/p2p_pipe.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    15517 2023-04-30 18:46:55.000000 p2pd-2.5.0/p2pd/p2p_protocol.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3072 2023-05-01 10:43:45.000000 p2pd-2.5.0/p2pd/p2p_utils.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13146 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/rest_api.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    32854 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/route.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5992 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/route_table.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11156 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/settings.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/signaling.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    28879 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/stun_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    41037 2023-05-19 04:37:59.000000 p2pd-2.5.0/p2pd/tcp_punch.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4766 2023-05-19 04:37:59.000000 p2pd-2.5.0/p2pd/test_init.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    17104 2023-05-01 10:43:45.000000 p2pd-2.5.0/p2pd/turn_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13940 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/turn_defs.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    10862 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/turn_process.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13894 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/upnp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16417 2023-05-28 08:34:04.000000 p2pd-2.5.0/p2pd/utils.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1027 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/var_names.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4220 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/win_net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16718 2023-04-28 06:42:33.000000 p2pd-2.5.0/p2pd/win_netifaces.py
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-28 08:39:20.535903 p2pd-2.5.0/p2pd.egg-info/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-05-28 08:39:20.000000 p2pd-2.5.0/p2pd.egg-info/PKG-INFO
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1548 2023-05-28 08:39:20.000000 p2pd-2.5.0/p2pd.egg-info/SOURCES.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        1 2023-05-28 08:39:20.000000 p2pd-2.5.0/p2pd.egg-info/dependency_links.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      110 2023-05-28 08:39:20.000000 p2pd-2.5.0/p2pd.egg-info/requires.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        5 2023-05-28 08:39:20.000000 p2pd-2.5.0/p2pd.egg-info/top_level.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      328 2023-05-19 04:37:59.000000 p2pd-2.5.0/requirements.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)       38 2023-05-28 08:39:20.539903 p2pd-2.5.0/setup.cfg
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1161 2023-05-28 08:34:04.000000 p2pd-2.5.0/setup.py
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-28 08:39:20.539903 p2pd-2.5.0/tests/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1090 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_address.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4111 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_bind.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      735 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_clock_skew.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5211 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_cmd.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5111 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_daemon.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_interface.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5161 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_ip_range.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7449 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_nat.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2016 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2793 2023-05-01 10:43:45.000000 p2pd-2.5.0/tests/test_net_afs.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      394 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_p2p_addr.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9769 2023-05-19 04:37:59.000000 p2pd-2.5.0/tests/test_p2p_pipe.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2759 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_p2pd_server.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1258 2023-05-19 04:37:59.000000 p2pd-2.5.0/tests/test_py_examples.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9323 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_route.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1618 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_route_table.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1406 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_rudp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1443 2023-05-01 10:43:45.000000 p2pd-2.5.0/tests/test_signaling.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2342 2023-05-28 08:34:04.000000 p2pd-2.5.0/tests/test_sock.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      992 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_sorted_search.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3385 2023-05-28 08:34:04.000000 p2pd-2.5.0/tests/test_stun_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5614 2023-05-01 10:43:45.000000 p2pd-2.5.0/tests/test_tcp_punch.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6770 2023-05-19 04:37:59.000000 p2pd-2.5.0/tests/test_turn_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2823 2023-04-28 06:42:33.000000 p2pd-2.5.0/tests/test_win_netifaces.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-06-26 06:28:16.876497 p2pd-2.6.0/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1570 2023-04-28 06:42:33.000000 p2pd-2.6.0/CREDITS.md
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1072 2023-04-28 06:42:33.000000 p2pd-2.6.0/LICENSE
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      106 2023-05-01 10:43:45.000000 p2pd-2.6.0/MANIFEST.in
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-06-26 06:28:16.876497 p2pd-2.6.0/PKG-INFO
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2707 2023-05-01 10:43:45.000000 p2pd-2.6.0/README.md
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-06-26 06:28:16.872496 p2pd-2.6.0/p2pd/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1196 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/__init__.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7065 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/ack_udp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6403 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/address.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    30942 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/base_stream.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8006 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/clock_skew.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8004 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/cmd_tools.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7896 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/daemon.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      303 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/echo_server.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      222 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/errors.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5601 2023-05-19 04:37:59.000000 p2pd-2.6.0/p2pd/http_client_lib.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5968 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/http_server_lib.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    23091 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/interface.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11971 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/ip_range.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5758 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/name_store.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    29727 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/nat.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    10521 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/nat_test.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    23607 2023-05-19 04:37:59.000000 p2pd-2.6.0/p2pd/net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4438 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/netiface_extra.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13979 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/ntp_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6624 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/p2p_addr.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13522 2023-05-01 10:43:45.000000 p2pd-2.6.0/p2pd/p2p_node.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    26320 2023-04-30 18:46:46.000000 p2pd-2.6.0/p2pd/p2p_pipe.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    15517 2023-04-30 18:46:55.000000 p2pd-2.6.0/p2pd/p2p_protocol.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3192 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/p2p_utils.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13146 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/rest_api.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    32854 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/route.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5992 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/route_table.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11156 2023-05-28 08:34:04.000000 p2pd-2.6.0/p2pd/settings.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/signaling.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    28962 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/stun_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    41037 2023-05-19 04:37:59.000000 p2pd-2.6.0/p2pd/tcp_punch.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4820 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/test_init.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    17230 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/turn_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13940 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/turn_defs.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    10862 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/turn_process.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13856 2023-06-26 06:25:20.000000 p2pd-2.6.0/p2pd/upnp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16417 2023-05-28 08:34:04.000000 p2pd-2.6.0/p2pd/utils.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1027 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/var_names.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4220 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/win_net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16718 2023-04-28 06:42:33.000000 p2pd-2.6.0/p2pd/win_netifaces.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-06-26 06:28:16.872496 p2pd-2.6.0/p2pd.egg-info/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-06-26 06:28:16.000000 p2pd-2.6.0/p2pd.egg-info/PKG-INFO
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1548 2023-06-26 06:28:16.000000 p2pd-2.6.0/p2pd.egg-info/SOURCES.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        1 2023-06-26 06:28:16.000000 p2pd-2.6.0/p2pd.egg-info/dependency_links.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      110 2023-06-26 06:28:16.000000 p2pd-2.6.0/p2pd.egg-info/requires.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        5 2023-06-26 06:28:16.000000 p2pd-2.6.0/p2pd.egg-info/top_level.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      328 2023-05-19 04:37:59.000000 p2pd-2.6.0/requirements.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)       38 2023-06-26 06:28:16.876497 p2pd-2.6.0/setup.cfg
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1161 2023-06-26 06:25:20.000000 p2pd-2.6.0/setup.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-06-26 06:28:16.876497 p2pd-2.6.0/tests/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1012 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_address.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3929 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_bind.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      683 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_clock_skew.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5211 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_cmd.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5007 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_daemon.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2810 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_interface.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5161 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_ip_range.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7449 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_nat.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2016 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2696 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_net_afs.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      394 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_p2p_addr.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9799 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_p2p_pipe.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2711 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_p2pd_server.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1242 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_py_examples.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9245 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_route.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1618 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_route_table.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1380 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_rudp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1464 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_signaling.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2244 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_sock.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      992 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_sorted_search.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3359 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_stun_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5531 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_tcp_punch.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6713 2023-06-26 06:25:20.000000 p2pd-2.6.0/tests/test_turn_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2823 2023-04-28 06:42:33.000000 p2pd-2.6.0/tests/test_win_netifaces.py
```

### Comparing `p2pd-2.5.0/CREDITS.md` & `p2pd-2.6.0/CREDITS.md`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/LICENSE` & `p2pd-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/PKG-INFO` & `p2pd-2.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2pd
-Version: 2.5.0
+Version: 2.6.0
 Summary: Asynchronous P2P networking library and service
 Home-page: http://github.com/robertsdotpm/p2pd
 Author: Matthew Roberts
 Author-email: matthew@roberts.pm
 License: public domain
 Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,STUN,TURN,SIP,DHCP,add IP to interface,NATPMP,P2P,Peer-to-peer networking library,python
 Classifier: Intended Audience :: Developers
```

### Comparing `p2pd-2.5.0/README.md` & `p2pd-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/__init__.py` & `p2pd-2.6.0/p2pd/__init__.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/ack_udp.py` & `p2pd-2.6.0/p2pd/ack_udp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/address.py` & `p2pd-2.6.0/p2pd/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,14 @@
         return hash(repr(self))
 
     def  __len__(self):
         return 0
 
 async def test_address(): # pragma: no cover
     from p2pd.interface import init_p2pd, Interface
-    netifaces = await init_p2pd()
     i = await Interface()
     print(i)
     a = await Address("www.google.com", 80, i.route()).res()
 
     d = a.to_dict()
     print(d)
```

### Comparing `p2pd-2.5.0/p2pd/base_stream.py` & `p2pd-2.6.0/p2pd/base_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,23 @@
     # Remove a subscription.
     def unsubscribe(self, sub):
         offset = self.hash_sub(sub)
         if offset in self.subs:
             del self.subs[offset]
 
         return self
+    
+    def tup_to_sub(self, dest_tup):
+        return [
+            b"", # Any message.
+            re.escape(b'%s:%d' % ( # Specific IP:port.
+                to_b(dest_tup[0]), 
+                dest_tup[1]
+            ))
+        ]
 
     # Adds a message to the first valid bucket.
     """
     TODO: If the queue is full what should the default
     actions be? Should the program await the queue
     being empty? Should it discard data? Maybe on limit - 1
     call https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.loop.remove_reader and on queue empty add it back.
@@ -744,15 +753,15 @@
 """
 In the spirit of unix a 'pipe' is an protocol and destination
 agnostic way to send data. It supports TCP & UDP: cons & servers.
 It supports using IPv4 and IPv6 destination addresses.
 You can pull data from it based on a regex pattern.
 You can execute code on new messages or connection disconnects.
 """
-async def pipe_open(proto, dest=None, route=None, sock=None, msg_cb=None, conf=NET_CONF):
+async def pipe_open(proto, route, dest=None, sock=None, msg_cb=None, conf=NET_CONF):
     # If no route is set assume default interface route 0.
     if route is None:
         # Load internal addresses.
         i = await Interface().start_local()
 
         # Bind to route 0.
         route = await i.route()
@@ -868,14 +877,17 @@
                 base_proto.set_endpoint_type(TYPE_TCP_CON)
 
         # Set dest if it's present.
         if dest is not None:
             base_proto.stream.dest = dest
             base_proto.stream.set_dest_tup(dest.tup)
 
+            # Queue all messages for convenience.
+            base_proto.subscribe(SUB_ALL)
+
         # Register pipes, msg callbacks, and subscriptions.
         return base_proto
     except Exception as e:
         log_exception()
         if conf["no_close"] == False:
             log("no close is false so trying to clean up.")
             if sock is not None:
```

### Comparing `p2pd-2.5.0/p2pd/clock_skew.py` & `p2pd-2.6.0/p2pd/clock_skew.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,14 @@
     # Unpickle.
     def __setstate__(self, state):
         o = self.from_dict(state)
         self.__dict__ = o.__dict__
 
 async def test_clock_skew(): # pragma: no cover
     from p2pd.interface import init_p2pd, Interface
-    await init_p2pd()
     interface = await Interface().start_local()
     s = await SysClock(interface=interface)
     print(repr(s))
 
 
     return
     f = []
```

### Comparing `p2pd-2.5.0/p2pd/cmd_tools.py` & `p2pd-2.6.0/p2pd/cmd_tools.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/daemon.py` & `p2pd-2.6.0/p2pd/daemon.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/http_client_lib.py` & `p2pd-2.6.0/p2pd/http_client_lib.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/http_server_lib.py` & `p2pd-2.6.0/p2pd/http_server_lib.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/interface.py` & `p2pd-2.6.0/p2pd/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 # Used for specifying the interface for sending out packets on
 # in TCP streams and UDP streams.
 class Interface():
     def __init__(self, name=None, stack=DUEL_STACK, nat=None, netifaces=None):
         super().__init__()
         self.resolved = False
         self.nat = nat or nat_info()
+        self.name = name
         self.rp = {}
         self.v4_lan_ips = []
         self.guid = None
         self.netifaces = netifaces or Interface.get_netifaces()
 
         # Check NAT is valid if set.
         if nat is not None:
@@ -164,43 +165,45 @@
             assert(nat.keys() == nat_info().keys())
 
         # Can provide a stack type to skip processing unsupported AFs.
         # Otherwise all AFs are checked when start() is called.
         self.stack = stack
         assert(self.stack in VALID_STACKS)
 
+    # Load mac, nic_no, and process name.
+    def load_if_info(self):
         # Assume its an AF.
-        if isinstance(name, int):
-            if name not in [IP4, IP6, AF_ANY]:
+        if isinstance(self.name, int):
+            if self.name not in [IP4, IP6, AF_ANY]:
                 raise InterfaceInvalidAF
 
-            name, _ = get_default_iface(self.netifaces, preference=name)
+            self.name, _ = get_default_iface(self.netifaces, preference=self.name)
 
         # No name specified.
         # Get name of default interface.
-        if name is None or name == "":
+        if self.name is None or self.name == "":
             # Windows -- default interface name is a GUID.
             # This is ugly AF.
             iface_name, iface_af = get_default_iface(self.netifaces)
             if iface_name is None:
                 raise InterfaceNotFound
             else:
-                name = iface_name
+                self.name = iface_name
 
             # Allow blank interface names to be used for testing.
             log("> default interface loaded")
 
             # May not be accurate.
             # Start() is the best way to set this.
             self.stack = iface_af
 
         # Windows NIC descriptions are used for the name
         # if the interfaces are detected as all hex.
         # It's more user friendly.
-        self.name = to_s(name)
+        self.name = to_s(self.name)
 
         # Check ID exists.
         if self.netifaces is not None:
             if self.name not in self.netifaces.interfaces():
                 log(f"interface name {self.name} not in {self.netifaces.interfaces()}")
                 raise InterfaceNotFound
             self.type = get_interface_type(self.name)
@@ -294,14 +297,21 @@
 
     # Unpickle.
     def __setstate__(self, state):
         o = self.from_dict(state)
         self.__dict__ = o.__dict__
 
     async def start_local(self, rp=None, skip_resolve=False):
+        # Load internal interface details.
+        if Interface.get_netifaces() is None:
+            self.netifaces = await init_p2pd()
+
+        # Process interface name in right format.
+        self.load_if_info()
+
         # Get routes for AF.
         if rp == None:
             af_list = VALID_AFS
             tasks = []
             for af in af_list:
                 async def helper(af):
                     route = await self.route_test(af)
@@ -321,14 +331,21 @@
         # Update stack type based on routable.
         self.stack = get_interface_stack(self.rp)
         assert(self.stack in VALID_STACKS)
         self.resolved = True
         return self
 
     async def start(self, rp=None, skip_resolve=False):
+        # Load internal interface details.
+        if Interface.get_netifaces() is None:
+            self.netifaces = await init_p2pd()
+
+        # Process interface name in right format.
+        self.load_if_info()
+
         # Get routes for AF.
         if rp == None:
             af_list = VALID_AFS
             tasks = []
             for af in af_list:
                 async def helper(af):
                     try:
@@ -395,15 +412,15 @@
 
             # Run delta test.
             nat_type, delta = await asyncio.wait_for(
                 asyncio.gather(*[
                     fast_nat_test(pipe, STUND_SERVERS[af]),
                     delta_test(stun_client)
                 ]),
-                timeout=2
+                timeout=4
             )
 
             nat = nat_info(nat_type, delta)
             await pipe.close()
 
         # Load NAT type and delta info.
         # On a server should be open.
@@ -423,15 +440,15 @@
     def nic(self, af):
         # Sanity check.
         if self.resolved:
             assert(af in self.what_afs())
         if self.rp != {} and len(self.rp[af].routes):
             return self.route(af).nic()
 
-    def route(self, af=None):
+    def route(self, af=None, bind_port=0):
         # Sanity check.
         if self.resolved:
             af = af or self.supported()[0]
             assert(af in self.what_afs())
 
         # Main route is last.
         if af in self.rp:
@@ -560,16 +577,19 @@
         if len(hay) > len(largest):
             largest = hay
             af_used = af
 
     return [largest, af_used]
 
 async def load_interfaces(netifaces=None, load_nat=True):
-    # Get list of good interfaces with ::/0 or 0.0.0.0 routes.
     netifaces = netifaces or Interface.get_netifaces()
+    if netifaces is None:
+        netifaces = await init_p2pd()
+
+    # Get list of good interfaces with ::/0 or 0.0.0.0 routes.
     ifs = await filter_trash_interfaces(netifaces)
     ifs = to_unique(ifs)
     if ifs == []:
         # Something must have gone wrong so just use regular netifaces.
         ifs = netifaces.interfaces()
 
     # Start all interfaces.
@@ -578,22 +598,30 @@
     for if_name in ifs:
         if_info = str(netifaces.ifaddresses(if_name))
         log(f"Attempt to start if name {if_name}")
         log(f"Net iface results for that if = {if_info}")
         async def worker(if_name):
             try:
                 interface = await Interface(if_name, netifaces=netifaces).start()
-                if load_nat:
-                    await interface.load_nat()
+                try:
+                    if load_nat:
+                        await interface.load_nat()
+                except Exception:
+                    log("Failed to load nat for interface.")
+                    # Just use the default NAT info.
+
                 if_list.append(interface)
             except Exception:
                 log_exception()
                 return
 
-        tasks.append(worker(if_name))
+        tasks.append(
+            # Assume timeout = non-routable.
+            worker(if_name)
+        )
 
     await asyncio.gather(*tasks)
 
     # Filter any interfaces that have no routes.
     # This will filter out loopback and other crap interfaces.
     good_ifs = []
     for interface in if_list:
```

### Comparing `p2pd-2.5.0/p2pd/ip_range.py` & `p2pd-2.6.0/p2pd/ip_range.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/name_store.py` & `p2pd-2.6.0/p2pd/name_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,14 @@
         if "KVS_ERROR" in out:
             raise Exception(out)
         else:
             return out
 
 if __name__ == '__main__':
     async def test_name_store():
-        await init_p2pd()
         i = await Interface().start_local()
         route = i.route()
         url = "http://net-debug.000webhostapp.com/name_store.php"
         db_path = "/home/lounge-linux-vm/Desktop/kvs.db"
         kvs = NameStore(route, url, db_path)
         await kvs.start()
```

### Comparing `p2pd-2.5.0/p2pd/nat.py` & `p2pd-2.6.0/p2pd/nat.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,33 +285,37 @@
                 src_port = random.randrange(4000, MAX_PORT)
 
             # Get the mapping using STUN.
             async def result_wrapper(src_port):
                 # Make sure port isn't in the reserved range.
                 if src_port < 4000 and src_port != 0:
                     raise Exception("src less than 4k in mapping behavior.")
-
+                
+                # Avoid relying on any one server. 
+                server = stun_client.rand_server()
+                
                 # Get mapping using specific source port.
                 _, s, local, mapped, _, _ = await stun_client.get_mapping(
                     proto,
                     do_close=0,
                     source_port=src_port,
                     group=group,
-                    conf=conf
+                    conf=conf,
+                    servers=[server]
                 )
 
                 # Return mapping results.
                 return [local, mapped, s]
 
             # Allow for tests to be done concurrently.
             tasks.append(
                 async_wrap_errors(
                     asyncio.wait_for(
                         result_wrapper(src_port),
-                        0.5
+                        2
                     )
                 )
             )
 
         return tasks
 
     def get_delta_value(delta_no, dist_no, local_dist, preserv_dist, results):
@@ -849,16 +853,15 @@
                 raise Exception(error)
 
 async def nat_predict_main():
     from .stun_client import STUNClient
     from .interface import Interface, init_p2pd
 
     # Load default interface.
-    netifaces = await init_p2pd()
-    i = await Interface(netifaces=netifaces).start_local()
+    i = await Interface().start_local()
     s = STUNClient(i)
     
     # Run delta test and profile it.
     s1 = timestamp(1)
     out = await delta_test(s)
     print(f"delta test time = {timestamp(1) - s1}")
     print(out)
```

### Comparing `p2pd-2.5.0/p2pd/nat_test.py` & `p2pd-2.6.0/p2pd/nat_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,43 @@
+"""
+When using UDP in network programming its common to write
+code so that it has simple loops to retry sending packets if
+no response is received. The problem is: if any packets are lost
+the time spent waiting keeps accumulating to the cost of a round-trip.
+
+The problem is made worse when you consider slow-downs in DNS and
+the often unreliable nature of relying on community servers for
+STUN code. If one is not careful they quickly end up with an
+algorithm that is prohibitively slow in the best case and quite
+unreliable in the worst case.
+
+The original algorithm for doing STUN tests for RFC 3489 used
+incremental tests and was very brittle. However -- due to the
+nature of how these tests work -- it became clear to me that it was
+possible to paralyze the tests into two main phases if a STUN
+server's primary and secondary IP were known beforehand.
+
+Phase 1 tests for [open NAT and full cone] while phase 2 tests for
+[restrict ip and restrict port] behaviors. The algorithm here is designed to run across multiple public servers where it creates races among
+all servers to test a routes NAT. The result is you end up with
+the fastest possible determination of NAT behaviors while also
+building in safe-guards against packet-loss, inconsistent results, misconfigurations, and slow network conditions.
+"""
+
 import time
 from .settings import *
 from .ip_range import *
 from .stun_client import *
 
 # Constants for a NAT test.
 NAT_TEST_NO = 5
 NAT_TEST_TIMEOUT = 0.5
 
 # STUN payload to send, Send IP, send port, reply IP, reply port
-# Shows order of RFC 3869 NAT enumeration sets.
+# Shows order of RFC 3489 NAT enumeration sets.
 NAT_TEST_SCHEMA = [
     # Detects: open NAT.
     ["", "primary", "primary", "primary", "primary"],
 
     # Detects: full cone NAT.
     # Change both reply IP and port.
     [changeRequest, "primary", "primary", "secondary", "secondary"],
```

### Comparing `p2pd-2.5.0/p2pd/net.py` & `p2pd-2.6.0/p2pd/net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/netiface_extra.py` & `p2pd-2.6.0/p2pd/netiface_extra.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/ntp_client.py` & `p2pd-2.6.0/p2pd/ntp_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
         NTPStats object
         """
         # lookup server address
         route = await self.interface.route().bind()
         dest = await Address(host, port, route).res()
 
         # create the socket
-        pipe = await pipe_open(UDP, dest, route)
+        pipe = await pipe_open(UDP, route, dest)
         pipe.subscribe()
         try:
             # create the request packet - mode 3 is client
             query_packet = NTPPacket(mode=3, version=version,
                                 tx_timestamp=system_to_ntp_time(time.time()))
 
             # send the request
```

### Comparing `p2pd-2.5.0/p2pd/p2p_addr.py` & `p2pd-2.6.0/p2pd/p2p_addr.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/p2p_node.py` & `p2pd-2.6.0/p2pd/p2p_node.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/p2p_pipe.py` & `p2pd-2.6.0/p2pd/p2p_pipe.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/p2p_protocol.py` & `p2pd-2.6.0/p2pd/p2p_protocol.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/p2p_utils.py` & `p2pd-2.6.0/p2pd/p2p_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,18 @@
             pp_executor, init_process_pool
         ))
     await asyncio.gather(*tasks)
     return pp_executor
 
 # delay with sys clock and get_pp_executors.
 async def start_p2p_node(port=NODE_PORT, node_id=None, ifs=None, clock_skew=Dec(0), ip=None, pp_executors=False, enable_upnp=False, signal_offsets=None, netifaces=None):
+    netifaces = netifaces or Interface.get_netifaces()
+    if netifaces is None:
+        netifaces = await init_p2pd()
+
     # Load NAT info for interface.
     ifs = ifs or await load_interfaces(netifaces=netifaces)
     assert(len(ifs))
     for interface in ifs:
         # Don't set NAT details if already set.
         if interface.resolved:
             continue
```

### Comparing `p2pd-2.5.0/p2pd/rest_api.py` & `p2pd-2.6.0/p2pd/rest_api.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/route.py` & `p2pd-2.6.0/p2pd/route.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/route_table.py` & `p2pd-2.6.0/p2pd/route_table.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/settings.py` & `p2pd-2.6.0/p2pd/settings.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/signaling.py` & `p2pd-2.6.0/p2pd/signaling.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/stun_client.py` & `p2pd-2.6.0/p2pd/stun_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,14 +518,18 @@
         self.af = af
         self.proto = proto
         self.sock_timeout = sock_timeout
 
         # Threshold / Number = agreement.
         self.t, self.n = consensus
 
+    def rand_server(self):
+        servers = get_stun_servers(self.af, self.proto)
+        return random.choice(servers)
+
     """
     Internal function - don't use directly.
     I liek the cat.
 
     This function has two main modes:
     - regular
     - fast fail
@@ -544,15 +548,14 @@
         # Record start time and define fail result funv.
         random.seed()
         start_time = time.time()
         f_fail = lambda: [None, None, time.time() - start_time]
         use_proto = TCP if fast_fail else proto
         lax = 0 if group == "change" else 1
 
-
         # Limit at 20 to avoid massive delays.
         # If 20 consecutive servers fail
         # something else is wrong.
         servers = servers or get_stun_servers(af, proto)
         stun_addr = None
         for server in servers:
             for i in range(conf["retry_no"]):
@@ -798,15 +801,14 @@
         from .interface import Interface, load_interfaces, init_p2pd
 
 
         # Maybe has a turn server.
         # https://wiki.innovaphone.com/index.php?#title=Howto:Innovaphones_public_services#TURN
         server = ['stun.innovaphone.com', 3478]
 
-        netifaces = await init_p2pd()
 
 
         i = await Interface().start_local()
         s = STUNClient(interface=i, proto=UDP)
         x = await s.get_wan_ip()
         print(x)
         return
```

### Comparing `p2pd-2.5.0/p2pd/tcp_punch.py` & `p2pd-2.6.0/p2pd/tcp_punch.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/test_init.py` & `p2pd-2.6.0/p2pd/test_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,30 +74,33 @@
         log(f"Check pipe: invalid recv buf {buf}")
         return False
 
 # If a random node ID is generated and subbed to over and over.
 # The server may limit new subs from the same IP.
 # But if all test nodes use the same IDs the there will be collisons.
 # Hence generate a unique IQ deterministically.
-def node_name(x):
-    i = Interface()
+def node_name(x, i):
+    assert(i.resolved)
     name_base = to_b(f"{i.mac} {socket.gethostname()}")
     node_name = hashlib.sha256(x + name_base).hexdigest()
     return to_b(node_name)[:10]
 
 class FakeSTUNClient():
     def __init__(self, interface=None, af=IP4):
         self.interface = interface
         self.rip = "1.3.3.7"
         self.sock = None
         self.mappings = [] # [local, mapped] ...
         self.p = 0
         self.wan_ip = None
         self.af = af
 
+    def rand_server(self):
+        return None
+
     def set_mappings(self, mappings):
         self.mappings = mappings
         self.p = 0
 
     def set_wan_ip(self, wan_ip):
         self.wan_ip = wan_ip
```

### Comparing `p2pd-2.5.0/p2pd/turn_client.py` & `p2pd-2.6.0/p2pd/turn_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,14 +327,18 @@
             while self.state != TURN_ERROR_STOPPED:
                 await asyncio.sleep(TURN_REFRESH_EXPIRY - 60)
                 await async_retry(f, count=5, timeout=5)
                 log("Refresh permission.")
 
         # Prevent garbage collection.
         if not already_accepted:
+            # Allow messages to be queued.
+            sub = self.tup_to_sub(peer_relay_tup)
+            self.subscribe(sub)
+
             # White list the peer if needed.
             await async_retry(f, count=5, timeout=5)
 
             # Start the loop to refresh the permission.
             task = asyncio.create_task(
                 async_wrap_errors(
                     refresher()
```

### Comparing `p2pd-2.5.0/p2pd/turn_defs.py` & `p2pd-2.6.0/p2pd/turn_defs.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/turn_process.py` & `p2pd-2.6.0/p2pd/turn_process.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/upnp.py` & `p2pd-2.6.0/p2pd/upnp.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,15 @@
     await route.bind(ips=route.nic())
     sock = await socket_factory(route, sock_type=UDP, conf=sock_conf)
     if af == IP6:
         sock.setsockopt(socket.IPPROTO_IPV6, socket.IP_MULTICAST_TTL, 2)
 
     # Create async pipe wrapper for multicast socket.
     dest = await Address(UPNP_IP[af], UPNP_PORT, route).res()
-    pipe = await pipe_open(UDP, dest, route, sock, conf=sock_conf)
+    pipe = await pipe_open(UDP, route, dest, sock, conf=sock_conf)
     pipe.subscribe()
 
     # Send m-search message.
     buf = m_search_buf(af)
 
     # Multiple sends spaced apart because UDP is garbage.
     for i in range(0, 3):
@@ -423,15 +423,14 @@
 
     # Return port forward tasks.
     return tasks
 
 if __name__ == "__main__":
     async def upnp_main():
         from .interface import Interfaces, init_p2pd
-        netifaces = await init_p2pd()
         i = await Interface().start_local()
         port = 31375
         desc = b"test 10003"
 
 
         print(i.route(IP4).nic())
```

### Comparing `p2pd-2.5.0/p2pd/utils.py` & `p2pd-2.6.0/p2pd/utils.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/var_names.py` & `p2pd-2.6.0/p2pd/var_names.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/win_net.py` & `p2pd-2.6.0/p2pd/win_net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd/win_netifaces.py` & `p2pd-2.6.0/p2pd/win_netifaces.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/p2pd.egg-info/PKG-INFO` & `p2pd-2.6.0/p2pd.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2pd
-Version: 2.5.0
+Version: 2.6.0
 Summary: Asynchronous P2P networking library and service
 Home-page: http://github.com/robertsdotpm/p2pd
 Author: Matthew Roberts
 Author-email: matthew@roberts.pm
 License: public domain
 Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,STUN,TURN,SIP,DHCP,add IP to interface,NATPMP,P2P,Peer-to-peer networking library,python
 Classifier: Intended Audience :: Developers
```

### Comparing `p2pd-2.5.0/p2pd.egg-info/SOURCES.txt` & `p2pd-2.6.0/p2pd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/setup.py` & `p2pd-2.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     install_reqs = f.read().splitlines()
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    version='2.5.0',
+    version='2.6.0',
     name='p2pd',
     description='Asynchronous P2P networking library and service',
     keywords=('NAT traversal, TCP hole punching, simultaneous open, UPnP, STUN, TURN, SIP, DHCP, add IP to interface, NATPMP, P2P, Peer-to-peer networking library, python'),
     long_description_content_type="text/markdown",
     long_description=long_description,
     url='http://github.com/robertsdotpm/p2pd',
     author='Matthew Roberts',
```

### Comparing `p2pd-2.5.0/tests/test_address.py` & `p2pd-2.6.0/tests/test_address.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from p2pd.test_init import *
 from p2pd import Address, HOST_TYPE_IP, HOST_TYPE_DOMAIN
 from p2pd import IP6, IP4
 from p2pd import Interface
 
 class TestIPRange(unittest.IsolatedAsyncioTestCase):
     async def test_domain_resolve(self):
-        await init_p2pd()
         i = await Interface().start_local()
         r = i.route()
         a = await Address("www.google.com", 80, r).res()
         self.assertEqual(a.host_type, HOST_TYPE_DOMAIN)
 
     async def test_v6_resolve(self):
-        await init_p2pd()
         i = await Interface().start_local()
         ip = "2402:1f00:8101:083f:0000:0000:0000:0001"
         r = i.route(IP6)
         a = await Address(ip, 80, r).res()
         self.assertEqual(a.host_type, HOST_TYPE_IP)
         self.assertTrue(a.is_public)
 
     async def test_v4_resolve(self):
-        await init_p2pd()
         i = await Interface().start_local()
         r = i.route(IP4)
         ip = "192.168.0.1"
         a = await Address(ip, 80, r).res()
         self.assertEqual(a.host_type, HOST_TYPE_IP)
         self.assertTrue(a.is_private)
```

### Comparing `p2pd-2.5.0/tests/test_bind.py` & `p2pd-2.6.0/tests/test_bind.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from p2pd.test_init import *
 from p2pd import IPRange, Bind, Route, Interface
 from p2pd.net import BLACK_HOLE_IPS, ip_norm, DUEL_STACK, IP6, IP4
 from p2pd.net import NIC_BIND, EXT_BIND, TCP, socket_factory
 
 class TestBind(unittest.IsolatedAsyncioTestCase):
     async def test_bind(self):
-        await init_p2pd()
         i = await Interface().start_local()
         af = i.stack if i.stack != DUEL_STACK else IP4
         b = Bind(i, af)
 
     async def test_ip_val_v6_bind_types(self):
-        await init_p2pd()
         i = await Interface().start_local()
         try:
             # Test global tuples set.
             ip = ip_norm("2402:1f00:8101:83f::1")
             b = Bind(i, IP6, ips=ip)
             await b.bind()
             self.assertEqual(b.ext_bind, ip)
@@ -32,35 +30,32 @@
             s = await socket_factory(b)
             self.assertTrue(isinstance(s, socket.socket))
             s.close()
         except:
             return
 
     async def test_ip_val_v4_bind_types(self):
-        await init_p2pd()
         i = await Interface().start_local()
 
         # Test nic bind occurs.
         tests = ["192.168.0.1", "8.8.8.8"]
         for ip in tests:
             b = Bind(i, IP4, ips=ip)
             self.assertEqual(b.nic_bind, ip)
             await b.bind()
             self.assertEqual(b.bind_tup(flag=NIC_BIND)[0], ip)
 
     async def test_route_v4_bind_types(self):
-        await init_p2pd()
         i = await Interface().start_local()
         r = i.route(IP4)
         b = await r.bind()
         tup = b.bind_tup(flag=NIC_BIND)
         self.assertTrue(tup[0])
 
     async def test_route_v6_bind_types(self):
-        await init_p2pd()
         i = await Interface().start_local()
 
         try:
             af = IP6
             r = await i.route_test(af)
 
             # Patch EXT to return a pub IP without interface being resolved.
@@ -74,15 +69,14 @@
     # TODO: netifaces is pulling invalid net masks for some IPs?
     async def test_bind_assumptions(self):
         ip = "139.99.209.1"
         #socket.socket(IP4, TCP)
 
 
     async def test_bind_start_v4_all_addr(self):
-        await init_p2pd()
         af = IP4
         try:
             i = await Interface(af).start_local()
         except:
             # If not supported.
             return
 
@@ -95,15 +89,14 @@
         self.assertEqual(route._bind_tups, expected_tups)
         s = await socket_factory(route)
         self.assertTrue(s is not None)
         if s is not None:
             s.close()
 
     async def test_bind_start_v6_all_addr(self):
-        await init_p2pd()
         i = await Interface().start_local()
         try:
             af = IP6
             route = await i.route(af).bind(13453, "*")
             bind_tup = (
                 "::",
                 13453,
```

### Comparing `p2pd-2.5.0/tests/test_clock_skew.py` & `p2pd-2.6.0/tests/test_clock_skew.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from p2pd.test_init import *
 import random
 from p2pd.clock_skew import *
 from p2pd.settings import *
 
 class TestClockSkew(unittest.IsolatedAsyncioTestCase):
     async def test_get_ntp_pool_ntp(self):
-        await init_p2pd()
         i = await Interface().start_local()
         ntp = None
 
         for _ in range(0, 5):
             server = random.choice(NTP_SERVERS)
             ntp = await get_ntp(i, server=server[0])
             if ntp:
                 break
 
         self.assertTrue(ntp)
 
     async def test_get_clock_skew(self):
-        await init_p2pd()
         i = await Interface().start_local()
         sys_clock = await SysClock(i).start()
         self.assertTrue(sys_clock.clock_skew)
 
 if __name__ == '__main__':
     main()
```

### Comparing `p2pd-2.5.0/tests/test_cmd.py` & `p2pd-2.6.0/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/tests/test_daemon.py` & `p2pd-2.6.0/tests/test_daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from p2pd.address import Address
 from p2pd.utils import what_exception
 from p2pd.daemon import Daemon
 
 asyncio.set_event_loop_policy(SelectorEventPolicy())
 class TestDaemon(unittest.IsolatedAsyncioTestCase):
     async def test_listen_all_interface_target(self):
-        await init_p2pd()
         i = await Interface().start_local()
         i.rp[IP6].routes = []
 
         # Daemon instance.
         server_port = 10126
         proto = TCP
         echod = await EchoServer().listen_all(
@@ -23,15 +22,14 @@
             [server_port],
             [proto]
         )
 
         await echod.close()
 
     async def test_bind_target(self):
-        await init_p2pd()
         d = Daemon()
         i = await Interface().start_local()
         i.rp[IP6].routes = []
 
         p = 10233
         b = await Bind(i, i.supported()[0], port=p).bind(p)
         await d._listen(
@@ -39,29 +37,27 @@
             port=p,
             proto=TCP
         )
 
         await d.close()
 
     async def test_listen_specific(self):
-        await init_p2pd()
         d = Daemon()
         i = await Interface().start_local()
         i.rp[IP6].routes = []
 
         p = 10233
         b = await Bind(i, i.supported()[0], port=p).bind(p)
         await d.listen_specific(
             targets=[[b, TCP]],
         )
 
         await d.close()
 
     async def test_daemon(self):
-        await init_p2pd()
         server_port = 10123
         loopbacks = {
             IP4: "127.0.0.1",
             IP6: "::1"
         }
 
         at_least_one = False
@@ -101,16 +97,16 @@
                         [server_port],
                         [proto]
                     )
 
                     # Spawn a pipe to the echo server.
                     pipe = await pipe_open(
                         proto,
-                        dest,
-                        route
+                        route,
+                        dest
                     )
                     self.assertTrue(pipe is not None)
 
                     # Indicate to save all messages to a queue.
                     pipe.subscribe(SUB_ALL)
 
                     # Send message to server.
```

### Comparing `p2pd-2.5.0/tests/test_interface.py` & `p2pd-2.6.0/tests/test_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,43 +7,42 @@
 from p2pd.interface import load_interfaces, filter_trash_interfaces
 from p2pd.interface import if_list_to_dict, dict_to_if_list
 
 asyncio.set_event_loop_policy(SelectorEventPolicy())
 class TestInterface(unittest.IsolatedAsyncioTestCase):
     # Should find at least a valid iface on whatever OS.
     async def test_default_interface(self):
-        await init_p2pd()
-        i = Interface()
+        i = await Interface().start_local()
         self.assertTrue(i.name)
 
-        i = Interface("")
+        i = await Interface("").start_local()
         self.assertTrue(i.name)
 
-        i = Interface(AF_ANY)
+        i = await Interface(AF_ANY).start_local()
         self.assertTrue(i.name)
 
         i = await Interface().start_local()
         d_list = if_list_to_dict([i])
         if_list = dict_to_if_list(d_list)
 
     async def test_invalid_interface_name(self):
-        await init_p2pd()
-        def invalid_interface_name():
-            i = Interface("meow")
+        test_passes = False
+        try:
+            await Interface("meow").start_local()
+        except InterfaceNotFound:
+            test_passes = True
 
-        self.assertRaises(InterfaceNotFound, invalid_interface_name)
+        self.assertTrue(test_passes)
 
     async def test_nat_validation(self):
-        await init_p2pd()
         nat = nat_info()
         i = Interface(nat=nat)
         i.set_nat(nat)
 
     async def test_fake_ext_route(self):
-        await init_p2pd()
         one_valid = False
         for af in VALID_AFS:
             try:
                 # Throws if no default route for AF.
                 i = await Interface(af).start()
 
                 # Throws if no NIC IP for AF.
@@ -54,29 +53,27 @@
 
         self.assertTrue(one_valid)
 
     async def test_win_netifaces_bypass(self):
         pass
 
     async def test_interface_start(self):
-        await init_p2pd()
         start_worked = False
         for af in VALID_AFS:
             try:
                 await Interface(af).start()
                 start_worked = True
                 break
             except Exception:
                 pass
 
         self.assertTrue(start_worked)
 
     async def test_load_interfaces(self):
-        netifaces = await init_p2pd()
-        ifs = await load_interfaces(netifaces=netifaces)
+        ifs = await load_interfaces()
         self.assertTrue(len(ifs))
 
         # Check nic IP fetch. 
         i = ifs[0]
         af = i.supported()[0]
         n = i.nic(af)
         self.assertTrue(n is not None)
```

### Comparing `p2pd-2.5.0/tests/test_ip_range.py` & `p2pd-2.6.0/tests/test_ip_range.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/tests/test_nat.py` & `p2pd-2.6.0/tests/test_nat.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/tests/test_net.py` & `p2pd-2.6.0/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/tests/test_net_afs.py` & `p2pd-2.6.0/tests/test_net_afs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 from p2pd.net import NIC_BIND, EXT_BIND, VALID_AFS, TCP, UDP
 from p2pd.base_stream import SUB_ALL
 
 asyncio.set_event_loop_policy(SelectorEventPolicy())
 
 class TestAFsWork(unittest.IsolatedAsyncioTestCase):
     async def test_afs(self):
-        # The BSD inetd seems broken for echo / udp / localhost bind.
-        await init_p2pd()
-
         # List of public echo servers.
         addr = {
             UDP: {
                 IP4: {
                     "host": "52.43.121.77",
                     "port": 10001
                 },
@@ -70,15 +67,15 @@
                 echo_dest = await Address(
                     addr[proto][af]["host"],
                     addr[proto][af]["port"],
                     route
                 ).res()
 
                 # Open pipe to echo server.
-                pipe = await pipe_open(proto, echo_dest, route)
+                pipe = await pipe_open(proto, route, echo_dest)
                 
                 # Interested in any message.
                 pipe.subscribe(SUB_ALL)
 
                 # Send data down the pipe.
                 for i in range(0, 4):
                     await pipe.send(msg + b"\r\n", echo_dest.tup)
```

### Comparing `p2pd-2.5.0/tests/test_p2p_pipe.py` & `p2pd-2.6.0/tests/test_p2p_pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,29 +35,29 @@
 
     # Load process pool executors.
     pp_executors = await get_pp_executors(workers=2)
 
     # Main node used for testing p2p functionality.
     node_a_ifs = [ifs[0]] if ifs is not None else test_setup.ifs
     node_a = await start_p2p_node(
-        node_id=node_name(b"node_a"),
+        node_id=node_name(b"node_a", node_a_ifs[0]),
 
         # Get brand new unassigned listen port.
         # Avoid TIME_WAIT buggy sockets from port reuse.
         port=0,
         ifs=node_a_ifs,
         clock_skew=test_setup.clock_skew,
         pp_executors=pp_executors,
         enable_upnp=False
     )
 
     # Test local punching algorithm.
     node_b_ifs = [ifs[1  % len(ifs)]] if ifs is not None else test_setup.ifs
     node_b = await start_p2p_node(
-        node_id=node_name(b"node_b"),
+        node_id=node_name(b"node_b", node_b_ifs[0]),
 
         # Get brand new unassigned listen port.
         # Avoid TIME_WAIT buggy sockets from port reuse.
         port=0,
         ifs=node_b_ifs,
         clock_skew=test_setup.clock_skew,
         pp_executors=pp_executors,
```

### Comparing `p2pd-2.5.0/tests/test_p2pd_server.py` & `p2pd-2.6.0/tests/test_p2pd_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 from p2pd.interface import *
 from p2pd.base_stream import *
 from p2pd.rest_api import *
 from p2pd.http_client_lib import *
 
 class TestP2PDServer(unittest.IsolatedAsyncioTestCase):
     async def test_p2pd_server(self):
-        # Init p2pd.
-        await init_p2pd()
-
         # Start the P2PD server.
         i = await Interface().start()
         r = await i.route().bind()
         server = await start_p2pd_server([i], r, port=P2PD_PORT, do_loop=False, do_init=False, enable_upnp=False)
 
         # Make server implement a custom ping protocol extension.
         async def proto_extension(msg, client_tup, pipe):
```

### Comparing `p2pd-2.5.0/tests/test_py_examples.py` & `p2pd-2.6.0/tests/test_py_examples.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 using this module. Easy to know if examples still work.
 """
 
 EXAMPLES_DIR = "../docs/source/python/examples"
 
 class TestPyExamples(unittest.IsolatedAsyncioTestCase):
     async def test_py_examples(self):
-        netifaces = await init_p2pd()
         for no in range(1, 13 + 1):
+            print(no)
             with open(f"{EXAMPLES_DIR}/example_{no}.py") as fp:
                 py_code = fp.read()
 
                 # Event loop is already running so replace
                 # async_test with an await call.
                 py_code = py_code.replace(
                     'async_test(example)',
```

### Comparing `p2pd-2.5.0/tests/test_route.py` & `p2pd-2.6.0/tests/test_route.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,26 +28,23 @@
         def invalid_wan():
             ipr_wan = IPRange(0, "255.255.255.255")
             route = Route(IP4, [ipr_nic], [ipr_wan])
 
         self.assertRaises(Exception, invalid_wan)
 
     async def test_bind_to_route(self):
-        await init_p2pd()
         i = await Interface().start_local()
         b = await Bind(i, i.supported()[0]).bind()
         r = await bind_to_route(b)
 
     async def test_if_to_rp(self):
-        await init_p2pd()
         i = await Interface().start_local()
         rp = interfaces_to_rp([i])
 
     async def test_netiface_addr_to_ipr(self):
-        await init_p2pd()
         loop = asyncio.get_event_loop()
         i = await Interface().start_local()
         af = i.supported()[0]
         r = i.route(af)
         info = {
             "addr": str(r.nic_ips[0]),
             "netmask": cidr_to_netmask(r.nic_ips[0].cidr, af)
```

### Comparing `p2pd-2.5.0/tests/test_route_table.py` & `p2pd-2.6.0/tests/test_route_table.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/tests/test_rudp.py` & `p2pd-2.6.0/tests/test_rudp.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from p2pd import IP6, IP4, Route, Interface
 from p2pd.net import ip_norm, RUDP, UDP, NET_CONF
 from p2pd.base_stream import pipe_open, SUB_ALL, BaseProto
 from p2pd.ack_udp import ACKUDP, BaseACKProto
 
 class TestRUDP(unittest.IsolatedAsyncioTestCase):
     async def test_rudp(self):
-        await init_p2pd()
         i = await Interface().start_local()
         af = i.supported()[0]
         port = 40000
         r = await i.route(af).bind(port)
         dest_tup = (r.nic(), port)
         dest = await Address(*dest_tup, r).res()
         pipe = (await pipe_open(
```

### Comparing `p2pd-2.5.0/tests/test_signaling.py` & `p2pd-2.6.0/tests/test_signaling.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 class TestSignaling(unittest.IsolatedAsyncioTestCase):
     async def test_node_signaling(self):
         if not P2PD_TEST_INFRASTRUCTURE:
             return
 
         # Channel that the test node subs to.
-        await init_p2pd()
+        i = await Interface().start_local()
         dest_id = "p2pd_test_node"
         msg = "msggg"
         f = asyncio.Future()
 
         # Receive a message from our MQTT channel (node ID.)
         async def proc_msg(msg, signal_pipe):
             f.set_result(to_s(msg))
 
         # Start the MQTT client.
-        node_id = node_name(b"node_c")
+        node_id = node_name(b"node_c", i)
         client = None
         for i in range(0, 3):
             client = SignalMock(node_id, proc_msg, mqtt_server=MQTT_SERVERS[i])
             await client.start()
 
             # Use basic echo protocol to test signaling works.
             await client.echo(msg, dest_id)
```

### Comparing `p2pd-2.5.0/tests/test_sock.py` & `p2pd-2.6.0/tests/test_sock.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,15 @@
         #s2.connect(("www.google.com", 80))
 
         s1.close()
         s2.close()
 
     async def test_socket_factory_connect(self):
         loop = asyncio.get_running_loop()
-        netifaces = await init_p2pd()
-        i = await Interface(netifaces=netifaces).start_local()
+        i = await Interface().start_local()
         af = i.supported()[0]
         r = await i.route(af).bind(0)
         d = await Address("8.8.8.8", 53, r)
         s = await socket_factory(route=r, dest_addr=d, sock_type=TCP, conf=NET_CONF)
         con_task = asyncio.create_task(
             loop.sock_connect(
                 s, 
@@ -49,16 +48,15 @@
 
     async def test_high_port_reuse(self):
         # Config for reuse.
         conf = copy.deepcopy(NET_CONF)
         conf["reuse_addr"] = True
 
         # Load default interface.
-        n = await init_p2pd()
-        i = await Interface(netifaces=n).start_local()
+        i = await Interface().start_local()
         r = i.route()
 
         # Make a new socket bound to a high order port.
         high_sock, high_port = await get_high_port_socket(r)
 
         # Make a new socket that shares the same port.
         r = await i.route().bind(high_port)
```

### Comparing `p2pd-2.5.0/tests/test_sorted_search.py` & `p2pd-2.6.0/tests/test_sorted_search.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.5.0/tests/test_stun_client.py` & `p2pd-2.6.0/tests/test_stun_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from p2pd.stun_client import tran_info_patterns, do_stun_request
 from p2pd.stun_client import changeRequest, changePortRequest
 from p2pd.ip_range import IPRange
 
 env = os.environ.copy()
 class TestStunClient(unittest.IsolatedAsyncioTestCase):
     async def test_stun_client(self):
-        await init_p2pd()
         one_valid = False
         for af in VALID_AFS:
             try:
                 # Get default Interface for AF type.
                 i = Interface(af)
                 #rp = use_fixed_rp(i)
                 await i.start()
@@ -67,16 +66,16 @@
                 if nat_type not in [OPEN_INTERNET, SYMMETRIC_UDP_FIREWALL]:
                     continue
 
                 for req in [changeRequest, changePortRequest]:
                     # Test change port request.
                     pipe = (await pipe_open(
                         UDP,
-                        dest,
-                        route
+                        route,
+                        dest
                     )).subscribe(SUB_ALL)
 
                     # Used for matching the TXID for the stun reply.
                     tran_info = tran_info_patterns(dest.tup)
                     tran_info[1] = 0 # Match any host tuple.
                     extra_data = req
                     pipe.subscribe(tran_info[:2])
```

### Comparing `p2pd-2.5.0/tests/test_tcp_punch.py` & `p2pd-2.6.0/tests/test_tcp_punch.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import multiprocessing
 from concurrent.futures import ProcessPoolExecutor
 from decimal import Decimal as Dec
 
 asyncio.set_event_loop_policy(SelectorEventPolicy())
 class TestTCPPunch(unittest.IsolatedAsyncioTestCase):
     async def test_map_info_to_their_maps(self):
-        await init_p2pd()
         map_info = {
             "remote": [5000],
             "reply": [0],
             "local": [10000]
         }
 
         expected = [
@@ -25,29 +24,28 @@
             expected
         )
 
     async def test_self_punch_no_networking(self):
         # Used to schedule and synchronize the punching.
         # Manager is used to push sockets between processes.
         log(">>> test_self_punch_no_networking")
-        netifaces = await init_p2pd()
         sys_clock = SysClock(Dec("0.01"))
         pe = await get_pp_executors()
         #pe2 = await get_pp_executors(workers=2)
         
         if pe is not None:
             qm = multiprocessing.Manager()
         else:
             qm = None
             
         pipe_id = b"pipe_id"
 
         # Load interfaces is slow AF on Windows.
         # Due to it using powershell + regex, lolz.
-        ifs = await load_interfaces(netifaces=netifaces)
+        ifs = await load_interfaces()
         interface = ifs[0]
         if IP4 in interface.supported():
             af = IP4
         else:
             af = IP6
 
         # Pretend we're using an open internet.
```

### Comparing `p2pd-2.5.0/tests/test_turn_client.py` & `p2pd-2.6.0/tests/test_turn_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,16 +99,15 @@
             await turn_client.close()
 
     async def test_turn(self):
         #print(sys.modules.keys())
         # Network interface details.
         log(">>> test_turn")
         n = 0
-        netifaces = await init_p2pd()
-        i = await Interface(netifaces=netifaces).start_local()
+        i = await Interface().start_local()
         af = i.supported()[0]
         r = await i.route(af).bind()
 
         # Address of a TURN server.
         dest = await Address(
             TURN_SERVERS[n]["host"],
             TURN_SERVERS[n]["port"],
```

### Comparing `p2pd-2.5.0/tests/test_win_netifaces.py` & `p2pd-2.6.0/tests/test_win_netifaces.py`

 * *Files identical despite different names*


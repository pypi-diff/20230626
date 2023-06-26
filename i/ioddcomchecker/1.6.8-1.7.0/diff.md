# Comparing `tmp/ioddcomchecker-1.6.8-cp39-cp39-win_amd64.whl.zip` & `tmp/ioddcomchecker-1.7.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 57656 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      732 b- defN 23-May-16 04:32 siogeen/LICENSE.txt
--rw-rw-rw-  2.0 fat   118784 b- defN 23-May-16 04:32 siogeen/tools/IoddComChecker.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      462 b- defN 23-May-16 04:32 siogeen/tools/__init__.py
--rw-rw-rw-  2.0 fat     1401 b- defN 23-May-16 04:32 siogeen/tools/cli/IoddComChecker.py
--rw-rw-rw-  2.0 fat      732 b- defN 23-May-16 04:32 ioddcomchecker-1.6.8.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     5499 b- defN 23-May-16 04:32 ioddcomchecker-1.6.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-16 04:32 ioddcomchecker-1.6.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-16 04:32 ioddcomchecker-1.6.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      778 b- defN 23-May-16 04:32 ioddcomchecker-1.6.8.dist-info/RECORD
-9 files, 128496 bytes uncompressed, 56302 bytes compressed:  56.2%
+Zip file size: 57972 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      732 b- defN 23-Jun-26 03:14 siogeen/LICENSE.txt
+-rw-rw-rw-  2.0 fat   119808 b- defN 23-Jun-26 03:14 siogeen/tools/IoddComChecker.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      462 b- defN 23-Jun-26 03:14 siogeen/tools/__init__.py
+-rw-rw-rw-  2.0 fat     1494 b- defN 23-Jun-26 03:14 siogeen/tools/cli/IoddComChecker.py
+-rw-rw-rw-  2.0 fat      732 b- defN 23-Jun-26 03:14 ioddcomchecker-1.7.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     5941 b- defN 23-Jun-26 03:14 ioddcomchecker-1.7.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-26 03:14 ioddcomchecker-1.7.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-26 03:14 ioddcomchecker-1.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      778 b- defN 23-Jun-26 03:14 ioddcomchecker-1.7.0.dist-info/RECORD
+9 files, 130055 bytes uncompressed, 56618 bytes compressed:  56.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: siogeen/tools/__init__.py
 Comment: 
 
 Filename: siogeen/tools/cli/IoddComChecker.py
 Comment: 
 
-Filename: ioddcomchecker-1.6.8.dist-info/LICENSE.txt
+Filename: ioddcomchecker-1.7.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: ioddcomchecker-1.6.8.dist-info/METADATA
+Filename: ioddcomchecker-1.7.0.dist-info/METADATA
 Comment: 
 
-Filename: ioddcomchecker-1.6.8.dist-info/WHEEL
+Filename: ioddcomchecker-1.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: ioddcomchecker-1.6.8.dist-info/top_level.txt
+Filename: ioddcomchecker-1.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ioddcomchecker-1.6.8.dist-info/RECORD
+Filename: ioddcomchecker-1.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siogeen/tools/cli/IoddComChecker.py

```diff
@@ -16,14 +16,15 @@
         epilog='''Examples:
   python -m siogeen.tools.cli.IoddComChecker
   python -m siogeen.tools.cli.IoddComChecker -a 10.0.0.17 -a 10.0.0.19 --auto''')
     parser.add_argument("-a", "--address",action='append',
                         help="specify one or more master addresses (default all)")
     parser.add_argument("--auto", action='store_true',
                         help="activate master ports if all are disabled")
+    parser.add_argument("--verbose", default=2, help="verbosity 0..3")
     parser.add_argument("--version", action='store_true',
         help="print version")
 
     return parser
 
 if __name__ == '__main__':
     parser = getParser()
@@ -35,8 +36,8 @@
     #args = parser.parse_args(['-a', '192.168.178.77', '--auto'])
 
     from siogeen.tools import IoddComChecker
 
     if args.version:
         print(f"IoddComChecker {IoddComChecker.__version__}")
     else:
-        IoddComChecker.check(args.address, args.auto)
+        IoddComChecker.check(args.address, args.auto, verbose=args.verbose)
```

## Comparing `ioddcomchecker-1.6.8.dist-info/LICENSE.txt` & `ioddcomchecker-1.7.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `ioddcomchecker-1.6.8.dist-info/METADATA` & `ioddcomchecker-1.7.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioddcomchecker
-Version: 1.6.8
+Version: 1.7.0
 Summary: IoddCom IO-Link master checker
 Home-page: https://siogeen.com
 Author: Reimund Renner
 Author-email: reimund@siogeen.com
 License: proprietary and confidential
 Project-URL: Documentation, https://siogeen.com/doc/
 Project-URL: Help Desk, https://siogeen.com/helpdesk/
@@ -76,43 +76,45 @@
 
 .. _request: https://siogeen.com/#contact
 
 Supported Platforms
 ~~~~~~~~~~~~~~~~~~~
 
 ========================= ===================== ===================
-**OS**                    Python 2.7, 3.4-3.5   Python 3.6 - 3.11
+**OS**                    Python 2.7, 3.4-3.6   Python 3.7 - 3.11
 ========================= ===================== ===================
 **Windows**                 [1]_                   x
 **Linux x86/x64**           [1]_                   x
-**Linux Arm (Raspberry)**   [1]_                  3.7-3.11
+**Linux Arm (Raspberry)**   [1]_                   x
 **macOS**                   [1]_                  3.8-3.11
 ========================= ===================== ===================
 
-.. [1] IoddCom for Python 2.7, 3.4 - 3.5 on request_.
+.. [1] IoddCom for Python 2.7, 3.4 - 3.6 on request_.
 
 Support for other platforms on request_.
 
 Supported operating systems and IO-Link masters
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Table of supported IO-Link masters for specific operating systems (OS):
 
-+---------------------------------+---------------------------------------------------+
-| Master                          | supported OS                                      |
-|                                 +---------+----------+--------------+---------------+
-|                                 | Windows |  Linux   | Raspberry Pi | macOS 64 [2]_ |
-+=================================+=========+==========+==============+===============+
-| TMG-USB based masters [3]_      |   x     |    x     |    x         |    x          |
-+---------------------------------+---------+----------+--------------+---------------+
-| TMG ethernet based masters [4]_ |   x     |    x     |    x         |    x          |
-+---------------------------------+---------+----------+--------------+---------------+
-| ifm ethernet based masters [5]_ |   x     |    x     |    x         |    x          |
-+---------------------------------+---------+----------+--------------+---------------+
-| ifm USB based masters [6]_      |   x     |    x     |    x         |    x          |
-+---------------------------------+---------+----------+--------------+---------------+
++--------------------------------------+---------------------------------------------------+
+| Master                               | supported OS                                      |
+|                                      +---------+----------+--------------+---------------+
+|                                      | Windows |  Linux   | Raspberry Pi | macOS 64 [2]_ |
++======================================+=========+==========+==============+===============+
+| TMG-USB based masters [3]_           |   x     |    x     |    x         |    x          |
++--------------------------------------+---------+----------+--------------+---------------+
+| TMG ethernet based masters [4]_      |   x     |    x     |    x         |    x          |
++--------------------------------------+---------+----------+--------------+---------------+
+| ifm ethernet based masters [5]_      |   x     |    x     |    x         |    x          |
++--------------------------------------+---------+----------+--------------+---------------+
+| ifm USB based masters [6]_           |   x     |    x     |    x         |    x          |
++--------------------------------------+---------+----------+--------------+---------------+
+| REST API ethernet based masters [7]_ |   x     |    x     |    x         |    x          |
++--------------------------------------+---------+----------+--------------+---------------+
 
 For Windows, Linux and Raspberry Pi both, 32-bit and 64-bit versions are available.
 
 .. [2] For macOS 13+
 
 .. [3] For example: Baumer, Leuze, Pepperl+Fuchs, SICK AG, Turck
 
@@ -122,14 +124,18 @@
        master type.
        The following functions are missing yet: PD streaming, master data storage read/write,
        master commands, PD valid status
 
 .. [6] Experimental ifm USB IO-Link master AL1060 support. Special functions missing
        like for [5]_
 
+.. [7] Testing REST API IO-Link masters: Sick SIG200/SIG350, Belden Lion-X,
+       MurrElectronik Impact67 Pro/MVK Pro, Balluff.
+       Special functions missing, Balluff not supported yet.
+
 Not supported masters:
 
 * RevolutionPi RevPi masters
 * Pepperl & Fuchs comtrol masters
 * Baumer USB-C and senscontrol masters
 * Germbedded masters
 * TEConcept masters
```

## Comparing `ioddcomchecker-1.6.8.dist-info/RECORD` & `ioddcomchecker-1.7.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 siogeen/LICENSE.txt,sha256=mjUk_O3YPxAZeoS61zCys2pyShGDxR4ghwb55ItZ0lg,732
-siogeen/tools/IoddComChecker.cp39-win_amd64.pyd,sha256=1hZQ3q-RFbAWq9231ZHtXlG0Tex6T3CBZk5dPl4dI4w,118784
+siogeen/tools/IoddComChecker.cp39-win_amd64.pyd,sha256=3teYj5U0ZzzXUu8ht_Z1FOx6rZaBt4gZSBc2x2k_kfw,119808
 siogeen/tools/__init__.py,sha256=CCpWoKGerJjGcTDaC48F6skWG4rDZuBzIKxBIZqL74w,462
-siogeen/tools/cli/IoddComChecker.py,sha256=pgYvQH3Von5tOmaC7nSq7yfyiYjuZuYtdxjI6bCG7_c,1401
-ioddcomchecker-1.6.8.dist-info/LICENSE.txt,sha256=mjUk_O3YPxAZeoS61zCys2pyShGDxR4ghwb55ItZ0lg,732
-ioddcomchecker-1.6.8.dist-info/METADATA,sha256=rkGOjhLpuJKkRBUSbnbL75blvFXTM3S5agYkIU7yJ08,5499
-ioddcomchecker-1.6.8.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-ioddcomchecker-1.6.8.dist-info/top_level.txt,sha256=vIFg0bLkihbkHyuCZUdHmA-50LP8LvTwDknGWir0T5o,8
-ioddcomchecker-1.6.8.dist-info/RECORD,,
+siogeen/tools/cli/IoddComChecker.py,sha256=q42zyT8sVC7LvyJWUrlKZ0Y00VYQiA4iSDcLhWKz_UQ,1494
+ioddcomchecker-1.7.0.dist-info/LICENSE.txt,sha256=mjUk_O3YPxAZeoS61zCys2pyShGDxR4ghwb55ItZ0lg,732
+ioddcomchecker-1.7.0.dist-info/METADATA,sha256=tpwA68_5-irxu0JT4lu6gbyrRUqBCS_n4qgBhz9GYPg,5941
+ioddcomchecker-1.7.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+ioddcomchecker-1.7.0.dist-info/top_level.txt,sha256=vIFg0bLkihbkHyuCZUdHmA-50LP8LvTwDknGWir0T5o,8
+ioddcomchecker-1.7.0.dist-info/RECORD,,
```


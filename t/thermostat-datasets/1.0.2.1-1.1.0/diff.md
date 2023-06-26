# Comparing `tmp/thermostat-datasets-1.0.2.1.tar.gz` & `tmp/thermostat-datasets-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thermostat-datasets-1.0.2.1.tar", last modified: Tue Mar 29 15:49:34 2022, max compression
+gzip compressed data, was "thermostat-datasets-1.1.0.tar", last modified: Mon Jun 26 10:13:22 2023, max compression
```

## Comparing `thermostat-datasets-1.0.2.1.tar` & `thermostat-datasets-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-03-29 15:49:34.212136 thermostat-datasets-1.0.2.1/
--rw-rw-rw-   0        0        0    11560 2022-02-10 08:18:45.000000 thermostat-datasets-1.0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1421 2022-03-29 15:49:34.212136 thermostat-datasets-1.0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    14250 2022-02-10 08:18:45.000000 thermostat-datasets-1.0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2022-03-29 15:49:34.212136 thermostat-datasets-1.0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2320 2022-03-29 15:36:50.000000 thermostat-datasets-1.0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-29 15:49:34.152100 thermostat-datasets-1.0.2.1/src/
-drwxrwxrwx   0        0        0        0 2022-03-29 15:49:34.167113 thermostat-datasets-1.0.2.1/src/thermostat/
--rw-rw-rw-   0        0        0      280 2022-02-10 08:18:45.000000 thermostat-datasets-1.0.2.1/src/thermostat/__init__.py
-drwxrwxrwx   0        0        0        0 2022-03-29 15:49:34.182114 thermostat-datasets-1.0.2.1/src/thermostat/data/
--rw-rw-rw-   0        0        0       24 2022-02-10 08:18:45.000000 thermostat-datasets-1.0.2.1/src/thermostat/data/__init__.py
--rw-rw-rw-   0        0        0      754 2022-02-10 08:18:45.000000 thermostat-datasets-1.0.2.1/src/thermostat/data/additional_configs.py
--rw-rw-rw-   0        0        0    17659 2022-03-15 14:20:36.000000 thermostat-datasets-1.0.2.1/src/thermostat/data/dataset_utils.py
--rw-rw-rw-   0        0        0     4521 2022-03-03 22:38:22.000000 thermostat-datasets-1.0.2.1/src/thermostat/data/readers.py
--rw-rw-rw-   0        0        0    48368 2022-03-29 15:46:21.000000 thermostat-datasets-1.0.2.1/src/thermostat/data/thermostat_configs.py
--rw-rw-rw-   0        0        0     3730 2022-02-10 08:18:45.000000 thermostat-datasets-1.0.2.1/src/thermostat/data/tokenization.py
--rw-rw-rw-   0        0        0     4336 2022-02-10 08:18:45.000000 thermostat-datasets-1.0.2.1/src/thermostat/dataset.py
--rw-rw-rw-   0        0        0     7109 2022-02-10 10:14:29.000000 thermostat-datasets-1.0.2.1/src/thermostat/explain.py
-drwxrwxrwx   0        0        0        0 2022-03-29 15:49:34.197112 thermostat-datasets-1.0.2.1/src/thermostat/explainers/
--rw-rw-rw-   0        0        0      447 2022-03-16 13:21:53.000000 thermostat-datasets-1.0.2.1/src/thermostat/explainers/__init__.py
--rw-rw-rw-   0        0        0     5866 2022-02-10 08:18:45.000000 thermostat-datasets-1.0.2.1/src/thermostat/explainers/grad.py
--rw-rw-rw-   0        0        0    11244 2022-02-10 08:18:45.000000 thermostat-datasets-1.0.2.1/src/thermostat/explainers/iba.py
--rw-rw-rw-   0        0        0     9081 2022-03-01 17:31:38.000000 thermostat-datasets-1.0.2.1/src/thermostat/explainers/lime.py
--rw-rw-rw-   0        0        0     1855 2022-02-10 08:18:45.000000 thermostat-datasets-1.0.2.1/src/thermostat/explainers/occlusion.py
--rw-rw-rw-   0        0        0     4428 2022-03-15 19:24:18.000000 thermostat-datasets-1.0.2.1/src/thermostat/explainers/shap.py
--rw-rw-rw-   0        0        0     1816 2022-03-01 17:28:55.000000 thermostat-datasets-1.0.2.1/src/thermostat/explainers/svs.py
--rw-rw-rw-   0        0        0     4276 2022-02-10 08:18:45.000000 thermostat-datasets-1.0.2.1/src/thermostat/utils.py
--rw-rw-rw-   0        0        0     9816 2022-03-29 13:26:40.000000 thermostat-datasets-1.0.2.1/src/thermostat/visualize.py
-drwxrwxrwx   0        0        0        0 2022-03-29 15:49:34.212136 thermostat-datasets-1.0.2.1/src/thermostat_datasets.egg-info/
--rw-rw-rw-   0        0        0     1421 2022-03-29 15:49:33.000000 thermostat-datasets-1.0.2.1/src/thermostat_datasets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      902 2022-03-29 15:49:34.000000 thermostat-datasets-1.0.2.1/src/thermostat_datasets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-29 15:49:33.000000 thermostat-datasets-1.0.2.1/src/thermostat_datasets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-03-29 12:47:11.000000 thermostat-datasets-1.0.2.1/src/thermostat_datasets.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      168 2022-03-29 15:49:34.000000 thermostat-datasets-1.0.2.1/src/thermostat_datasets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-03-29 15:49:34.000000 thermostat-datasets-1.0.2.1/src/thermostat_datasets.egg-info/top_level.txt
+drwxrwxr-x   0 nfel      (1000) nfel      (1000)        0 2023-06-26 10:13:22.958258 thermostat-datasets-1.1.0/
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)    11358 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/LICENSE
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     1375 2023-06-26 10:13:22.958258 thermostat-datasets-1.1.0/PKG-INFO
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)    14557 2022-07-04 20:42:48.000000 thermostat-datasets-1.1.0/README.md
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)       38 2023-06-26 10:13:22.958258 thermostat-datasets-1.1.0/setup.cfg
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     2263 2023-06-26 10:12:12.000000 thermostat-datasets-1.1.0/setup.py
+drwxrwxr-x   0 nfel      (1000) nfel      (1000)        0 2023-06-26 10:13:22.954258 thermostat-datasets-1.1.0/src/
+drwxrwxr-x   0 nfel      (1000) nfel      (1000)        0 2023-06-26 10:13:22.954258 thermostat-datasets-1.1.0/src/thermostat/
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)      270 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/src/thermostat/__init__.py
+drwxrwxr-x   0 nfel      (1000) nfel      (1000)        0 2023-06-26 10:13:22.958258 thermostat-datasets-1.1.0/src/thermostat/data/
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)       23 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/src/thermostat/data/__init__.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)      731 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/src/thermostat/data/additional_configs.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)    17287 2022-07-04 20:42:48.000000 thermostat-datasets-1.1.0/src/thermostat/data/dataset_utils.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     4404 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/src/thermostat/data/readers.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     2996 2021-06-24 08:19:18.000000 thermostat-datasets-1.1.0/src/thermostat/data/stats.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)    47177 2022-07-04 20:42:48.000000 thermostat-datasets-1.1.0/src/thermostat/data/thermostat_configs.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     3644 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/src/thermostat/data/tokenization.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     4230 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/src/thermostat/dataset.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)    10480 2023-06-26 09:51:07.000000 thermostat-datasets-1.1.0/src/thermostat/explain.py
+drwxrwxr-x   0 nfel      (1000) nfel      (1000)        0 2023-06-26 10:13:22.958258 thermostat-datasets-1.1.0/src/thermostat/explainers/
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)      421 2022-07-04 20:42:48.000000 thermostat-datasets-1.1.0/src/thermostat/explainers/__init__.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     5743 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/src/thermostat/explainers/grad.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)    10960 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/src/thermostat/explainers/iba.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     8892 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/src/thermostat/explainers/lime.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     1816 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/src/thermostat/explainers/occlusion.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     4322 2022-07-04 20:42:48.000000 thermostat-datasets-1.1.0/src/thermostat/explainers/shap.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     1777 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/src/thermostat/explainers/svs.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     4147 2021-10-26 00:36:46.000000 thermostat-datasets-1.1.0/src/thermostat/utils.py
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     9555 2022-07-04 20:42:48.000000 thermostat-datasets-1.1.0/src/thermostat/visualize.py
+drwxrwxr-x   0 nfel      (1000) nfel      (1000)        0 2023-06-26 10:13:22.958258 thermostat-datasets-1.1.0/src/thermostat_datasets.egg-info/
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)     1375 2023-06-26 10:13:22.000000 thermostat-datasets-1.1.0/src/thermostat_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)      931 2023-06-26 10:13:22.000000 thermostat-datasets-1.1.0/src/thermostat_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)        1 2023-06-26 10:13:22.000000 thermostat-datasets-1.1.0/src/thermostat_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)        1 2021-07-01 12:37:41.000000 thermostat-datasets-1.1.0/src/thermostat_datasets.egg-info/not-zip-safe
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)      166 2023-06-26 10:13:22.000000 thermostat-datasets-1.1.0/src/thermostat_datasets.egg-info/requires.txt
+-rw-rw-r--   0 nfel      (1000) nfel      (1000)       11 2023-06-26 10:13:22.000000 thermostat-datasets-1.1.0/src/thermostat_datasets.egg-info/top_level.txt
```

### Comparing `thermostat-datasets-1.0.2.1/LICENSE` & `thermostat-datasets-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `thermostat-datasets-1.0.2.1/PKG-INFO` & `thermostat-datasets-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-Metadata-Version: 2.1
-Name: thermostat-datasets
-Version: 1.0.2.1
-Summary: Collection of NLP model explanations and accompanying analysis tools
-Home-page: https://github.com/DFKI-NLP/thermostat
-Download-URL: https://github.com/DFKI-NLP/thermostat/tags
-Author: DFKI-NLP
-Author-email: nils.feldhus@dfki.de
-License: Apache 2.0
-Keywords: explainability heatmaps feature-attribution natural-language-processing
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-License-File: LICENSE
-
-Thermostat is a large collection of NLP model explanations and accompanying analysis tools. Combines explainability methods from the captum library with Hugging Face's datasets and transformers. Mitigates repetitive execution of common experiments in Explainable NLP and thus reduces the environmental impact and financial roadblocks. Increases comparability and replicability of research. Reduces the implementational burden.
-
+Metadata-Version: 2.1
+Name: thermostat-datasets
+Version: 1.1.0
+Summary: Collection of NLP model explanations and accompanying analysis tools
+Home-page: https://github.com/DFKI-NLP/thermostat
+Download-URL: https://github.com/DFKI-NLP/thermostat/tags
+Author: DFKI-NLP
+Author-email: nils.feldhus@dfki.de
+License: Apache 2.0
+Keywords: explainability heatmaps feature-attribution natural-language-processing
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+License-File: LICENSE
+
+Thermostat is a large collection of NLP model explanations and accompanying analysis tools. Combines explainability methods from the captum library with Hugging Face's datasets and transformers. Mitigates repetitive execution of common experiments in Explainable NLP and thus reduces the environmental impact and financial roadblocks. Increases comparability and replicability of research. Reduces the implementational burden.
```

### Comparing `thermostat-datasets-1.0.2.1/README.md` & `thermostat-datasets-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,277 +1,280 @@
-![logo](figures/logo.png)
-
-### **Thermostat** is a large collection of NLP model explanations and accompanying analysis tools.
-
-* Combines explainability methods from the `captum` library with Hugging Face's `datasets` and `transformers`.
-* Mitigates repetitive execution of common experiments in Explainable NLP and thus reduces the environmental impact and financial roadblocks.
-* Increases comparability and replicability of research.
-* Reduces the implementational burden.
-
-This work is described in our paper accepted to **EMNLP 2021 System Demonstrations** :  
-**Nils Feldhus, Robert Schwarzenberg, and Sebastian Möller.**  
-__Thermostat: A Large Collection of NLP Model Explanations and Analysis Tools.__  *2021.*
-
-arXiv pre-print available here: https://arxiv.org/abs/2108.13961  
-
-
-
-## Installation
-
-### With pip
-
-[![PyPI](https://img.shields.io/pypi/v/thermostat-datasets?style=flat-square)](https://pypi.org/project/thermostat-datasets/)
-
-```bash
-pip install thermostat-datasets
-```
-### Explore on Hugging Face Spaces
-
-The **Spaces** edition of Thermostat launched on October 26, 2021. Check it out here:
-[![](figures/spaces.png)](https://huggingface.co/spaces/nfel/Thermostat)
-
-
-## Usage
-
-Downloading a dataset requires just two lines of code:
-
-```python
-import thermostat
-data = thermostat.load("imdb-bert-lig")
-```
-
-Thermostat datasets can be addressed and loaded with an identifier string that contains three basic coordinates: Dataset, Model, and Explainer. In this example, the dataset is IMDb (sentiment analysis of movie reviews), the model is a BERT model fine-tuned on the IMDb data, the explanations are generated using a (Layer) Integrated Gradients explainer.
-
-`data` then contains the following columns/features:
-* `attributions` (the attributions for each token for each data point; type: List of floats)
-* `idx` (the index of the instance in the dataset)
-* `input_ids` (the token IDs of the original dataset; type: List of ints)
-* `label` (the label of the original dataset; type: int)
-* `predictions` (the class logits of the classifier/downstream model; type: List of floats)  
-
-This is the raw content stored in each of the instances of `data`:
-
-![instance-contents](figures/instance-contents.png)
-
-
-If we print `data`, we get more info such as the actual names of the dataset, the explainer and the model:
-```python
-print(data)
-> IMDb dataset, BERT model, Layer Integrated Gradients explanations
-> Explainer: LayerIntegratedGradients
-> Model: textattack/bert-base-uncased-imdb
-> Dataset: imdb
-```
-
-### Indexing an instance
-We can simply index the loaded dataset like a list:
-
-```python
-import thermostat
-instance = thermostat.load("imdb-bert-lig")[429]
-```
-
-
-
-
-### Visualizing attributions as a heatmap
-
-We can apply `.render()` to every instance to display a heatmap visualization generated by the [displaCy](https://spacy.io/usage/visualizers) library.
-
-```python
-instance.render()  # instance refers to the variable assigned in the last codebox
-```
-
-![heatmap-html](figures/imdb-429.png)
-
-
-### Get simple tuple-based heatmap
-
-The `explanation` attribute stores a tuple-based heatmap with the token, the attribution, and the token index as elements.
-
-```python
-print(instance.explanation)  # instance refers to the variable assigned in the second to last codebox
-
-> [('[CLS]', 0.0, 0),
- ('amazing', 2.3141794204711914, 1),
- ('movie', 0.06655970215797424, 2),
- ('.', -0.47832658886909485, 3),
- ('some', 0.15708176791667938, 4),
- ('of', -0.02931656688451767, 5),
- ('the', -0.08834744244813919, 6),
- ('script', -0.2660972774028778, 7),
- ('writing', -0.4021594822406769, 8),
- ('could', -0.19280624389648438, 9),
- ('have', -0.015477157197892666, 10),
- ('been', -0.21898044645786285, 11),
- ('better', -0.4095713794231415, 12),
- ...]  # abbreviated
-```
-
-The `heatmap` attribute displays it as a `pandas` table:
-
-```python
-print(instance.heatmap)
-
-> token_index    0         1          2         3          4         5    \
-token        [CLS]         i       went       and        saw      this   
-attribution      0 -0.117371  0.0849944  0.165192  0.0362542 -0.029687   
-text_field    text      text       text      text       text      text   
-
-token_index       6         7         8          9          10         11   \
-token           movie      last     night      after      being     coaxed   
-attribution  0.533126  0.240222  0.171116 -0.0450005 -0.0103401  0.0166524   
-text_field       text      text      text       text       text       text   
-
-token_index        13         14          15         16         17   \
-token               to         by           a        few    friends   
-attribution  0.0269605 -0.0213463  0.00761083  0.0216749  0.0579834   
-text_field        text       text        text       text       text   
-
-# abbreviated
-```
-
-
-### Modifying the load function
-`thermostat.load()` is a wrapper around [`datasets.load_dataset()`](https://huggingface.co/docs/datasets/package_reference/loading_methods.html#datasets.load_dataset) and you can use any keyword arguments from `load_dataset()` in `load()`, too (except `path`, `name` and `split` which are reserved), e.g. if you want to use another cache directory, you can use the `cache_dir` argument in `thermostat.load()`.
-
----
-
-## Explainers
-Name | captum implementation | Parameters
---- | --- | ---
-Layer Gradient x Activation (`lgxa`) | [`.attr.LayerGradientXActivation`](https://captum.ai/api/layer.html#layer-gradient-x-activation) |
-Layer Integrated Gradients (`lig`) | [`.attr.LayerIntegratedGradients`](https://captum.ai/api/layer.html#layer-integrated-gradients) | # samples = 25
-LIME (`lime`) | [`.attr.LimeBase`](https://captum.ai/api/lime.html) | # samples = 25, <br>mask prob = 0.3
-Occlusion (`occ`) | [`.attr.Occlusion`](https://captum.ai/api/occlusion.html) | sliding window = 3
-Shapley Value Sampling (`svs`) | [`.attr.ShapleyValueSampling`](https://captum.ai/api/shapley_value_sampling.html) | # samples = 25
-
-
-
-## Datasets + Models
-
-![Overview](figures/overview_v1.png)
-
-✅ = Dataset is downloadable  
-⏏️ = Dataset is finished, but not uploaded yet  
-🔄 = Currently running on cluster (x n = number of jobs/screens)  
-⚠️ = Issue  
-
-### IMDb
-
-[`imdb`](https://huggingface.co/datasets/viewer/?dataset=imdb) is a sentiment analysis dataset with 2 classes (`pos` and `neg`). The available split is the `test` subset containing 25k examples.  
-Example configuration: `imdb-xlnet-lig`
-
-Name | 🤗 | `lgxa` | `lig` | `lime` | `occ` | `svs`  
---- | --- | --- | --- | --- | --- | ---
-ALBERT (`albert`) | [`textattack/albert-base-v2-imdb`](https://huggingface.co/textattack/albert-base-v2-imdb) | ✅ | ✅ | ✅ | ✅ | ✅
-BERT (`bert`) | [`textattack/bert-base-uncased-imdb`](https://huggingface.co/textattack/bert-base-uncased-imdb) | ✅ | ✅ | ✅ | ✅ | ✅
-ELECTRA (`electra`) | [`monologg/electra-small-finetuned-imdb`](https://huggingface.co/monologg/electra-small-finetuned-imdb) | ✅ | ✅ | ✅ | ✅ | ✅
-RoBERTa (`roberta`) | [`textattack/roberta-base-imdb`](https://huggingface.co/textattack/roberta-base-imdb) | ✅ | ✅ | ✅ | ✅ | ✅
-XLNet (`xlnet`) | [`textattack/xlnet-base-cased-imdb`](https://huggingface.co/textattack/xlnet-base-cased-imdb) | ✅ | ✅ | ✅ | ✅ | ✅
-
-
-### MultiNLI
-
-[`multi_nli`](https://huggingface.co/datasets/viewer/?dataset=multi_nli) is a textual entailment dataset. The available split is the `validation_matched` subset containing 9815 examples.  
-Example configuration: `multi_nli-roberta-lime`
-
-Name | 🤗 | `lgxa` | `lig` | `lime` | `occ` | `svs`
---- | --- | --- | --- | --- | --- | ---
-ALBERT (`albert`) | [`prajjwal1/albert-base-v2-mnli`](https://huggingface.co/prajjwal1/albert-base-v2-mnli) | ✅ | ✅ | ✅ | ✅ | ✅
-BERT (`bert`) | [`textattack/bert-base-uncased-MNLI`](https://huggingface.co/textattack/bert-base-uncased-MNLI) | ✅ | ✅ | ✅ | ✅ | ✅
-ELECTRA (`electra`) | [`howey/electra-base-mnli`](https://huggingface.co/howey/electra-base-mnli) | ✅ | ✅ | ✅ | ✅ | ✅
-RoBERTa (`roberta`) | [`textattack/roberta-base-MNLI`](https://huggingface.co/textattack/roberta-base-MNLI) | ✅ | ✅ | ✅ | ✅ | ✅
-XLNet (`xlnet`) | [`textattack/xlnet-base-cased-MNLI`](https://huggingface.co/textattack/xlnet-base-cased-MNLI) | ✅ | ✅ | ✅ | ✅ | ✅
-
-
-### XNLI
-
-[`xnli`](https://huggingface.co/datasets/viewer/?dataset=xnli) is a textual entailment dataset. It provides the test set of MultiNLI through the "en" configuration. The fine-tuned models used here are the same as the MultiNLI ones. The available split is the `test` subset containing 5010 examples.  
-Example configuration: `xnli-roberta-lime`
-
-Name | 🤗 | `lgxa` | `lig` | `lime` | `occ` | `svs`
---- | --- | --- | --- | --- | --- | ---
-ALBERT (`albert`) | [`prajjwal1/albert-base-v2-mnli`](https://huggingface.co/prajjwal1/albert-base-v2-mnli) | ✅ | ✅ | ✅ | ✅ | ✅
-BERT (`bert`) | [`textattack/bert-base-uncased-MNLI`](https://huggingface.co/textattack/bert-base-uncased-MNLI) | ✅ | ✅ | ✅ | ✅ | ✅
-ELECTRA (`electra`) | [`howey/electra-base-mnli`](https://huggingface.co/howey/electra-base-mnli) | ✅ | ✅ | ✅ | ✅ | ✅
-RoBERTa (`roberta`) | [`textattack/roberta-base-MNLI`](https://huggingface.co/textattack/roberta-base-MNLI) | ✅ | ✅ | ✅ | ✅ | ✅
-XLNet (`xlnet`) | [`textattack/xlnet-base-cased-MNLI`](https://huggingface.co/textattack/xlnet-base-cased-MNLI) | ✅ | ✅ | ✅ | ✅ | ✅
-
-
-### AG News
-
-[`ag_news`](https://huggingface.co/datasets/viewer/?dataset=ag_news) is a news topic classification dataset. The available split is the `test` subset containing 7600 examples.  
-Example configuration: `ag_news-albert-svs`
-
-Name | 🤗 | `lgxa` | `lig` | `lime` | `occ` | `svs`
---- | --- | --- | --- | --- | --- | ---
-ALBERT (`albert`) | [`textattack/albert-base-v2-ag-news`](https://huggingface.co/textattack/albert-base-v2-ag-news) | ✅ | ✅ | ✅ | ✅ | ✅
-BERT (`bert`) | [`textattack/bert-base-uncased-ag-news`](https://huggingface.co/textattack/bert-base-uncased-ag-news) | ✅ | ✅ | ✅ | ✅ | ✅
-RoBERTa (`roberta`) | [`textattack/roberta-base-ag-news`](https://huggingface.co/textattack/roberta-base-ag-news) | ✅ | ✅ | ✅ | ✅ | ✅
-
----
-
-### Contribute a dataset
-
-New explanation datasets must follow the JSONL format and include the five fields `attributions`, `idx`, `input_ids`, `label` and `predictions` as described above in "Usage".
-
-Please follow the instructions for writing a dataset loading script in the official docs of [datasets](https://huggingface.co/docs/datasets/add_dataset.html).
-
-Provide the additional Thermostat metadata via the list of builder configs ([click here to see the Thermostat implementation of builder configs](https://github.com/nfelnlp/thermostat/blob/c877ccf9155d42ec8a820ba9789cc84b8eb5f076/src/thermostat/data/thermostat_configs.py#L158)).
-
-Necessary fields include...
-* `name` : The unique identifier string, e.g. including the three coordinates `<DATASET>-<MODEL>-<EXPLAINER>`
-* `dataset` : The full name of the dataset, usually follows the naming convention in `datasets`, e.g. `"imdb"`
-* `explainer` : The full name of the explainer, usually follows the naming convention in `captum`, e.g. `"LayerIntegratedGradients"`
-* `model` : The full name of the model, usually follows the naming convention in `transformers`, e.g. `"textattack/bert-base-uncased-imdb"`
-* `label_column` : The name of the column in the JSONL file that contains the label, usually `"label"`
-* `label_classes` : The list of label names or classes, e.g. `["entailment", "neutral", "contradiction"]` for NLI datasets
-* `text_column` : Either a string (if there is only one text column) or a list of strings that identify the column in the JSONL file that contains the text(s), e.g. `"text"` (IMDb) or `["premise", "hypothesis"]` (NLI)
-* `description` : Should at least state the full names of the three coordinates, can optionally include more info such as hyperparameter choices
-* `data_url` : The URL to the data storage, e.g. a Google Drive link
-
-plus `features` which you can copy from the codebox below:
-```python
-features={"attributions": "attributions",
-          "predictions": "predictions",
-          "input_ids": "input_ids"}
-```
-
-
-While debugging, you can wrap your data with the `Thermopack` class and see if it correctly parses your data:
-
-```python
-import thermostat
-from datasets import load_dataset
-data = load_dataset('your_dataset')
-thermostat.Thermopack(data)
-```
-
-If you're successful, follow the official instructions for [sharing a community provided dataset at the HuggingFace hub](https://huggingface.co/docs/datasets/share_dataset.html).
-
-At first, all Thermostat contributions will have to be loaded via the code example above. Please notify us of existing explanation datasets by creating an [Issue](https://github.com/DFKI-NLP/thermostat/issues) with the tag [Contribution](https://github.com/DFKI-NLP/thermostat/labels/contribution) and a maintainer of this repository will add your dataset to the Thermostat configs s.t. it can be accessed by everyone via `thermostat.load()`.
-
----
-
-## Cite Thermostat
-
-```
-@inproceedings{feldhus2021thermostat,
-    title={Thermostat: A Large Collection of NLP Model Explanations and Analysis Tools},
-    author={Nils Feldhus and Robert Schwarzenberg and Sebastian Möller},
-    year={2021},
-    editor = {Heike Adel and Shuming Shi},
-    booktitle = {Proceedings of the 2021 Conference on Empirical Methods in Natural Language Processing: System Demonstrations},
-}
-```
-
-
-## Disclaimer
-We give no warranties for the correctness of the heatmaps or any other part of the data. This is evolving work and will be hot-patched continuously.
-
-The Thermostat project follows the [ACL and ACM Code of Ethics](https://www.acm.org/code-of-ethics).
-
-
-## Acknowledgements
-
-The majority of the codebase, especially regarding the combination of transformers and captum, stems from our other recent project [Empirical Explainers](https://github.com/DFKI-NLP/emp-exp).
+![logo](figures/logo.png)
+
+### **Thermostat** is a large collection of NLP model explanations and accompanying analysis tools.
+
+* Combines explainability methods from the `captum` library with Hugging Face's `datasets` and `transformers`.
+* Mitigates repetitive execution of common experiments in Explainable NLP and thus reduces the environmental impact and financial roadblocks.
+* Increases comparability and replicability of research.
+* Reduces the implementational burden.
+
+This work is described in our paper accepted to **EMNLP 2021 System Demonstrations** :  
+**Nils Feldhus, Robert Schwarzenberg, and Sebastian Möller.**  
+__Thermostat: A Large Collection of NLP Model Explanations and Analysis Tools.__  *2021.*
+
+arXiv pre-print available here: https://arxiv.org/abs/2108.13961  
+
+
+
+## Installation
+
+### With pip
+
+[![PyPI](https://img.shields.io/pypi/v/thermostat-datasets?style=flat-square)](https://pypi.org/project/thermostat-datasets/)
+
+```bash
+pip install thermostat-datasets
+```
+### Explore on Hugging Face Spaces
+
+The **Spaces** edition of Thermostat launched on October 26, 2021. Check it out here:
+[![](figures/spaces.png)](https://huggingface.co/spaces/nfel/Thermostat)
+
+
+## Usage
+
+Downloading a dataset requires just two lines of code:
+
+```python
+import thermostat
+data = thermostat.load("imdb-bert-lig")
+```
+
+Thermostat datasets can be addressed and loaded with an identifier string that contains three basic coordinates: Dataset, Model, and Explainer. In this example, the dataset is IMDb (sentiment analysis of movie reviews), the model is a BERT model fine-tuned on the IMDb data, the explanations are generated using a (Layer) Integrated Gradients explainer.
+
+`data` then contains the following columns/features:
+* `attributions` (the attributions for each token for each data point; type: List of floats)
+* `idx` (the index of the instance in the dataset)
+* `input_ids` (the token IDs of the original dataset; type: List of ints)
+* `label` (the label of the original dataset; type: int)
+* `predictions` (the class logits of the classifier/downstream model; type: List of floats)  
+
+This is the raw content stored in each of the instances of `data`:
+
+![instance-contents](figures/instance-contents.png)
+
+
+If we print `data`, we get more info such as the actual names of the dataset, the explainer and the model:
+```python
+print(data)
+> IMDb dataset, BERT model, Layer Integrated Gradients explanations
+> Explainer: LayerIntegratedGradients
+> Model: textattack/bert-base-uncased-imdb
+> Dataset: imdb
+```
+
+### Indexing an instance
+We can simply index the loaded dataset like a list:
+
+```python
+import thermostat
+instance = thermostat.load("imdb-bert-lig")[429]
+```
+
+
+
+
+### Visualizing attributions as a heatmap
+
+We can apply `.render()` to every instance to display a heatmap visualization generated by the [displaCy](https://spacy.io/usage/visualizers) library.
+
+```python
+instance.render()  # instance refers to the variable assigned in the last codebox
+```
+
+![heatmap-html](figures/imdb-429.png)
+
+
+### Get simple tuple-based heatmap
+
+The `explanation` attribute stores a tuple-based heatmap with the token, the attribution, and the token index as elements.
+
+```python
+print(instance.explanation)  # instance refers to the variable assigned in the second to last codebox
+
+> [('[CLS]', 0.0, 0),
+ ('amazing', 2.3141794204711914, 1),
+ ('movie', 0.06655970215797424, 2),
+ ('.', -0.47832658886909485, 3),
+ ('some', 0.15708176791667938, 4),
+ ('of', -0.02931656688451767, 5),
+ ('the', -0.08834744244813919, 6),
+ ('script', -0.2660972774028778, 7),
+ ('writing', -0.4021594822406769, 8),
+ ('could', -0.19280624389648438, 9),
+ ('have', -0.015477157197892666, 10),
+ ('been', -0.21898044645786285, 11),
+ ('better', -0.4095713794231415, 12),
+ ...]  # abbreviated
+```
+
+The `heatmap` attribute displays it as a `pandas` table:
+
+```python
+print(instance.heatmap)
+
+> token_index    0         1          2         3          4         5    \
+token        [CLS]         i       went       and        saw      this   
+attribution      0 -0.117371  0.0849944  0.165192  0.0362542 -0.029687   
+text_field    text      text       text      text       text      text   
+
+token_index       6         7         8          9          10         11   \
+token           movie      last     night      after      being     coaxed   
+attribution  0.533126  0.240222  0.171116 -0.0450005 -0.0103401  0.0166524   
+text_field       text      text      text       text       text       text   
+
+token_index        13         14          15         16         17   \
+token               to         by           a        few    friends   
+attribution  0.0269605 -0.0213463  0.00761083  0.0216749  0.0579834   
+text_field        text       text        text       text       text   
+
+# abbreviated
+```
+
+
+### Modifying the load function
+`thermostat.load()` is a wrapper around [`datasets.load_dataset()`](https://huggingface.co/docs/datasets/package_reference/loading_methods.html#datasets.load_dataset) and you can use any keyword arguments from `load_dataset()` in `load()`, too (except `path`, `name` and `split` which are reserved), e.g. if you want to use another cache directory, you can use the `cache_dir` argument in `thermostat.load()`.
+
+---
+
+## Explainers
+Name | captum implementation | Parameters
+--- | --- | ---
+Layer Gradient x Activation (`lgxa`) | [`.attr.LayerGradientXActivation`](https://captum.ai/api/layer.html#layer-gradient-x-activation) |
+Layer Integrated Gradients (`lig`) | [`.attr.LayerIntegratedGradients`](https://captum.ai/api/layer.html#layer-integrated-gradients) | # samples = 25
+LIME (`lime`) | [`.attr.LimeBase`](https://captum.ai/api/lime.html) | # samples = 25, <br>mask prob = 0.3
+Occlusion (`occ`) | [`.attr.Occlusion`](https://captum.ai/api/occlusion.html) | sliding window = 3
+Shapley Value Sampling (`svs`) | [`.attr.ShapleyValueSampling`](https://captum.ai/api/shapley_value_sampling.html) | # samples = 25
+Layer DeepLiftShap (`lds`) | [`.attr.LayerDeepLiftShap`](https://captum.ai/api/layer.html#layer-deepliftshap) |
+Layer GradientShap (`lgs`) | [`.attr.LayerGradientShap`](https://captum.ai/api/layer.html#layer-gradientshap) | # samples = 5
+
+
+
+
+## Datasets + Models
+
+![Overview](figures/overview_v1.png)
+
+✅ = Dataset is downloadable  
+⏏️ = Dataset is finished, but not uploaded yet  
+🔄 = Currently running on cluster (x n = number of jobs/screens)  
+⚠️ = Issue  
+
+### IMDb
+
+[`imdb`](https://huggingface.co/datasets/viewer/?dataset=imdb) is a sentiment analysis dataset with 2 classes (`pos` and `neg`). The available split is the `test` subset containing 25k examples.  
+Example configuration: `imdb-xlnet-lig`
+
+Name | 🤗 | `lgxa` | `lig` | `lime` | `occ` | `svs` | `lds` | `lgs` 
+--- | --- | --- | --- | --- | --- | --- | --- | ---
+ALBERT (`albert`) | [`textattack/albert-base-v2-imdb`](https://huggingface.co/textattack/albert-base-v2-imdb) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+BERT (`bert`) | [`textattack/bert-base-uncased-imdb`](https://huggingface.co/textattack/bert-base-uncased-imdb) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+ELECTRA (`electra`) | [`monologg/electra-small-finetuned-imdb`](https://huggingface.co/monologg/electra-small-finetuned-imdb) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+RoBERTa (`roberta`) | [`textattack/roberta-base-imdb`](https://huggingface.co/textattack/roberta-base-imdb) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+XLNet (`xlnet`) | [`textattack/xlnet-base-cased-imdb`](https://huggingface.co/textattack/xlnet-base-cased-imdb) | ✅ | ✅ | ✅ | ✅ | ✅ | ⚠️ | ⚠️
+
+
+### MultiNLI
+
+[`multi_nli`](https://huggingface.co/datasets/viewer/?dataset=multi_nli) is a textual entailment dataset. The available split is the `validation_matched` subset containing 9815 examples.  
+Example configuration: `multi_nli-roberta-lime`
+
+Name | 🤗 | `lgxa` | `lig` | `lime` | `occ` | `svs` | `lds` | `lgs`
+--- | --- | --- | --- | --- | --- | --- | --- | ---
+ALBERT (`albert`) | [`prajjwal1/albert-base-v2-mnli`](https://huggingface.co/prajjwal1/albert-base-v2-mnli) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+BERT (`bert`) | [`textattack/bert-base-uncased-MNLI`](https://huggingface.co/textattack/bert-base-uncased-MNLI) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+ELECTRA (`electra`) | [`howey/electra-base-mnli`](https://huggingface.co/howey/electra-base-mnli) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+RoBERTa (`roberta`) | [`textattack/roberta-base-MNLI`](https://huggingface.co/textattack/roberta-base-MNLI) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+XLNet (`xlnet`) | [`textattack/xlnet-base-cased-MNLI`](https://huggingface.co/textattack/xlnet-base-cased-MNLI) | ✅ | ✅ | ✅ | ✅ | ✅ | ⚠️ | ⚠️
+
+
+### XNLI
+
+[`xnli`](https://huggingface.co/datasets/viewer/?dataset=xnli) is a textual entailment dataset. It provides the test set of MultiNLI through the "en" configuration. The fine-tuned models used here are the same as the MultiNLI ones. The available split is the `test` subset containing 5010 examples.  
+Example configuration: `xnli-roberta-lime`
+
+Name | 🤗 | `lgxa` | `lig` | `lime` | `occ` | `svs` | `lds` | `lgs`
+--- | --- | --- | --- | --- | --- | --- | --- | ---
+ALBERT (`albert`) | [`prajjwal1/albert-base-v2-mnli`](https://huggingface.co/prajjwal1/albert-base-v2-mnli) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+BERT (`bert`) | [`textattack/bert-base-uncased-MNLI`](https://huggingface.co/textattack/bert-base-uncased-MNLI) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+ELECTRA (`electra`) | [`howey/electra-base-mnli`](https://huggingface.co/howey/electra-base-mnli) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+RoBERTa (`roberta`) | [`textattack/roberta-base-MNLI`](https://huggingface.co/textattack/roberta-base-MNLI) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+XLNet (`xlnet`) | [`textattack/xlnet-base-cased-MNLI`](https://huggingface.co/textattack/xlnet-base-cased-MNLI) | ✅ | ✅ | ✅ | ✅ | ✅ | ⚠️ | ⚠️
+
+
+### AG News
+
+[`ag_news`](https://huggingface.co/datasets/viewer/?dataset=ag_news) is a news topic classification dataset. The available split is the `test` subset containing 7600 examples.  
+Example configuration: `ag_news-albert-svs`
+
+Name | 🤗 | `lgxa` | `lig` | `lime` | `occ` | `svs` | `lds` | `lgs`
+--- | --- | --- | --- | --- | --- | --- | --- | ---
+ALBERT (`albert`) | [`textattack/albert-base-v2-ag-news`](https://huggingface.co/textattack/albert-base-v2-ag-news) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+BERT (`bert`) | [`textattack/bert-base-uncased-ag-news`](https://huggingface.co/textattack/bert-base-uncased-ag-news) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+RoBERTa (`roberta`) | [`textattack/roberta-base-ag-news`](https://huggingface.co/textattack/roberta-base-ag-news) | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅
+
+---
+
+### Contribute a dataset
+
+New explanation datasets must follow the JSONL format and include the five fields `attributions`, `idx`, `input_ids`, `label` and `predictions` as described above in "Usage".
+
+Please follow the instructions for writing a dataset loading script in the official docs of [datasets](https://huggingface.co/docs/datasets/add_dataset.html).
+
+Provide the additional Thermostat metadata via the list of builder configs ([click here to see the Thermostat implementation of builder configs](https://github.com/nfelnlp/thermostat/blob/c877ccf9155d42ec8a820ba9789cc84b8eb5f076/src/thermostat/data/thermostat_configs.py#L158)).
+
+Necessary fields include...
+* `name` : The unique identifier string, e.g. including the three coordinates `<DATASET>-<MODEL>-<EXPLAINER>`
+* `dataset` : The full name of the dataset, usually follows the naming convention in `datasets`, e.g. `"imdb"`
+* `explainer` : The full name of the explainer, usually follows the naming convention in `captum`, e.g. `"LayerIntegratedGradients"`
+* `model` : The full name of the model, usually follows the naming convention in `transformers`, e.g. `"textattack/bert-base-uncased-imdb"`
+* `label_column` : The name of the column in the JSONL file that contains the label, usually `"label"`
+* `label_classes` : The list of label names or classes, e.g. `["entailment", "neutral", "contradiction"]` for NLI datasets
+* `text_column` : Either a string (if there is only one text column) or a list of strings that identify the column in the JSONL file that contains the text(s), e.g. `"text"` (IMDb) or `["premise", "hypothesis"]` (NLI)
+* `description` : Should at least state the full names of the three coordinates, can optionally include more info such as hyperparameter choices
+* `data_url` : The URL to the data storage, e.g. a Google Drive link
+
+plus `features` which you can copy from the codebox below:
+```python
+features={"attributions": "attributions",
+          "predictions": "predictions",
+          "input_ids": "input_ids"}
+```
+
+
+While debugging, you can wrap your data with the `Thermopack` class and see if it correctly parses your data:
+
+```python
+import thermostat
+from datasets import load_dataset
+data = load_dataset('your_dataset')
+thermostat.Thermopack(data)
+```
+
+If you're successful, follow the official instructions for [sharing a community provided dataset at the HuggingFace hub](https://huggingface.co/docs/datasets/share_dataset.html).
+
+At first, all Thermostat contributions will have to be loaded via the code example above. Please notify us of existing explanation datasets by creating an [Issue](https://github.com/DFKI-NLP/thermostat/issues) with the tag [Contribution](https://github.com/DFKI-NLP/thermostat/labels/contribution) and a maintainer of this repository will add your dataset to the Thermostat configs s.t. it can be accessed by everyone via `thermostat.load()`.
+
+---
+
+## Cite Thermostat
+
+```
+@inproceedings{feldhus2021thermostat,
+    title={Thermostat: A Large Collection of NLP Model Explanations and Analysis Tools},
+    author={Nils Feldhus and Robert Schwarzenberg and Sebastian Möller},
+    year={2021},
+    editor = {Heike Adel and Shuming Shi},
+    booktitle = {Proceedings of the 2021 Conference on Empirical Methods in Natural Language Processing: System Demonstrations},
+}
+```
+
+
+## Disclaimer
+We give no warranties for the correctness of the heatmaps or any other part of the data. This is evolving work and will be hot-patched continuously.
+
+The Thermostat project follows the [ACL and ACM Code of Ethics](https://www.acm.org/code-of-ethics).
+
+
+## Acknowledgements
+
+The majority of the codebase, especially regarding the combination of transformers and captum, stems from our other recent project [Empirical Explainers](https://github.com/DFKI-NLP/emp-exp).
```

### Comparing `thermostat-datasets-1.0.2.1/setup.py` & `thermostat-datasets-1.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from setuptools import find_packages, setup
-# new change 
-from sys import platform
-
-if platform == "win32":
-    jsonnet = "jsonnet-binary"
-else:
-    jsonnet = "jsonnet"
-# new change
-
-REQUIRED_PKGS = [
-    "captum>=0.3",
-    "datasets>=1.5",
-    jsonnet,
-    "numpy>=1.20",
-    "overrides",
-    "pandas",
-    "protobuf",
-    "pytorch-ignite",
-    "scipy",
-    "sentencepiece",
-    "sklearn",
-    "spacy>=3.0",
-    "torch",
-    "tqdm>=4.49",
-    "transformers>=4.5",
-]
-
-setup(
-    name="thermostat-datasets",
-    version="1.0.2.1",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
-    description="Collection of NLP model explanations and accompanying analysis tools",
-    long_description="Thermostat is a large collection of NLP model explanations and accompanying analysis tools. "
-                     "Combines explainability methods from the captum library with Hugging Face's datasets and "
-                     "transformers. Mitigates repetitive execution of common experiments in Explainable NLP and thus "
-                     "reduces the environmental impact and financial roadblocks. Increases comparability and "
-                     "replicability of research. Reduces the implementational burden.",
-    author="DFKI-NLP",
-    author_email="nils.feldhus@dfki.de",
-    url="https://github.com/DFKI-NLP/thermostat",
-    download_url="https://github.com/DFKI-NLP/thermostat/tags",
-    license="Apache 2.0",
-    package_dir={"": "src"},
-    packages=find_packages(where="src"),
-    install_requires=REQUIRED_PKGS,
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Education",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Topic :: Scientific/Engineering :: Artificial Intelligence",
-    ],
-    keywords="explainability heatmaps feature-attribution natural-language-processing",
-    zip_safe=False,  # Required for mypy to find the py.typed file
-)
+from setuptools import find_packages, setup
+# new change 
+from sys import platform
+
+if platform == "win32":
+    jsonnet = "jsonnet-binary"
+else:
+    jsonnet = "jsonnet"
+# new change
+
+REQUIRED_PKGS = [
+    "captum>=0.3",
+    "datasets>=1.5",
+    jsonnet,
+    "numpy>=1.22",
+    "overrides",
+    "pandas",
+    "protobuf",
+    "pytorch-ignite",
+    "scipy",
+    "sentencepiece",
+    "scikit-learn",
+    "spacy>=3.0",
+    "torch",
+    "tqdm>=4.49",
+    "transformers>=4.5",
+]
+
+setup(
+    name="thermostat-datasets",
+    version="1.1.0",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+    description="Collection of NLP model explanations and accompanying analysis tools",
+    long_description="Thermostat is a large collection of NLP model explanations and accompanying analysis tools. "
+                     "Combines explainability methods from the captum library with Hugging Face's datasets and "
+                     "transformers. Mitigates repetitive execution of common experiments in Explainable NLP and thus "
+                     "reduces the environmental impact and financial roadblocks. Increases comparability and "
+                     "replicability of research. Reduces the implementational burden.",
+    author="DFKI-NLP",
+    author_email="nils.feldhus@dfki.de",
+    url="https://github.com/DFKI-NLP/thermostat",
+    download_url="https://github.com/DFKI-NLP/thermostat/tags",
+    license="Apache 2.0",
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
+    install_requires=REQUIRED_PKGS,
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Education",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    ],
+    keywords="explainability heatmaps feature-attribution natural-language-processing",
+    zip_safe=False,  # Required for mypy to find the py.typed file
+)
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat/data/additional_configs.py` & `thermostat-datasets-1.1.0/src/thermostat/data/additional_configs.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-CEN = ["contradiction", "entailment", "neutral"]
-CNE = ["contradiction", "neutral", "entailment"]
-ECN = ["entailment", "contradiction", "neutral"]
-ENC = ["entailment", "neutral", "contradiction"]  # Legacy / Default from HF datasets
-NCE = ["neutral", "contradiction", "entailment"]
-NEC = ["neutral", "entailment", "contradiction"]
-
-LC_MAP = {
-    "multi_nli-albert": CEN,
-    "multi_nli-bert": CEN,
-    "multi_nli-roberta": CNE,
-    "multi_nli-xlnet": CEN,
-    "xnli-albert": CEN,
-    "xnli-bert": CEN,
-    "xnli-roberta": CNE,
-    "xnli-xlnet": CEN,
-}
-
-
-def get_label_names(config_name):
-    cn_dataset_model = '-'.join(config_name.split('-')[:2])
-    if cn_dataset_model in LC_MAP.keys():
-        return LC_MAP[cn_dataset_model]
+CEN = ["contradiction", "entailment", "neutral"]
+CNE = ["contradiction", "neutral", "entailment"]
+ECN = ["entailment", "contradiction", "neutral"]
+ENC = ["entailment", "neutral", "contradiction"]  # Legacy / Default from HF datasets
+NCE = ["neutral", "contradiction", "entailment"]
+NEC = ["neutral", "entailment", "contradiction"]
+
+LC_MAP = {
+    "multi_nli-albert": CEN,
+    "multi_nli-bert": CEN,
+    "multi_nli-roberta": CNE,
+    "multi_nli-xlnet": CEN,
+    "xnli-albert": CEN,
+    "xnli-bert": CEN,
+    "xnli-roberta": CNE,
+    "xnli-xlnet": CEN,
+}
+
+
+def get_label_names(config_name):
+    cn_dataset_model = '-'.join(config_name.split('-')[:2])
+    if cn_dataset_model in LC_MAP.keys():
+        return LC_MAP[cn_dataset_model]
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat/data/dataset_utils.py` & `thermostat-datasets-1.1.0/src/thermostat/data/dataset_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,376 +1,376 @@
-import numpy as np
-import os
-# new change 
-from sys import platform
-# new change
-from datasets import Dataset, load_dataset
-from itertools import groupby
-from overrides import overrides
-from sklearn.metrics import classification_report
-from tqdm import tqdm
-from transformers import AutoTokenizer
-from typing import Dict, List
-
-from thermostat.data import additional_configs, thermostat_configs
-from thermostat.data.tokenization import fuse_subwords
-from thermostat.utils import lazy_property
-from thermostat.visualize import ColorToken, Heatmap, normalize_attributions
-
-
-class ThermopackMeta(type):
-    """ Inspired by: https://stackoverflow.com/a/65917858 """
-    def __new__(mcs, name, bases, dct):
-        child = super().__new__(mcs, name, bases, dct)
-        for base in bases:
-            for field_name, field in base.__dict__.items():
-                if callable(field) and not field_name.startswith('__'):
-                    setattr(child, field_name, mcs.force_child(field, field_name, base, child))
-        return child
-
-    @staticmethod
-    def force_child(fun, fun_name, base, child):
-        """Turn from Base- to Child-instance-returning function."""
-        def wrapper(*args, **kwargs):
-            result = fun(*args, **kwargs)
-            if not result:
-                # Ignore if returns None
-                return None
-            if type(result) == base:
-                print(fun_name)
-                # Return Child instance if the Base method tries to return Base instance.
-                return child(result)
-            return result
-        return wrapper
-
-
-class Thermopack(Dataset, metaclass=ThermopackMeta):
-    def __init__(self, hf_dataset):
-        # Init Dataset super class
-        super().__init__(hf_dataset.data, info=hf_dataset.info, split=hf_dataset.split,
-                         indices_table=hf_dataset._indices)
-
-        # Model
-        self.model_name = get_coordinate(hf_dataset, 'Model')
-        # Dataset
-        self.dataset_name = get_coordinate(hf_dataset, 'Dataset')
-        # Explainer
-        self.explainer_name = get_coordinate(hf_dataset, 'Explainer')
-
-        self.dataset: Dataset = hf_dataset
-        self.units: List = [PlaceholderThermounit(unit['attributions'],
-                                                  unit['idx'],
-                                                  unit['input_ids'],
-                                                  unit['label'],
-                                                  unit['predictions']) for unit in self.dataset]
-        self.legacy_label_names = get_config(self.config_name).label_classes
-
-    def __getattr__(self, name):
-        """ Only gets called if an attribute that is not part of the Thermopack is accessed.
-         In this case, if the name of the requested attribute is one of the five attributes of a Thermounit,
-         return the respective entries of all units as a list """
-        if name in list(self.units[0].__dict__.keys()):
-            return ThermounitAttributeArray([getattr(u, name) for u in self.units])
-        else:
-            raise AttributeError
-
-    @overrides
-    def __getitem__(self, idx):
-        """ Indexing a Thermopack by an integer instantiates a Thermounit and returns it.
-            Indexing by string returns the associated column if its exists (similar to HF datasets). """
-
-        if isinstance(idx, str):
-            """ String indexing """
-            if idx in list(self.units[0].__dict__.keys()):
-                """ Same behaviour as __getattr__: Return the requested attribute of all units as a list. """
-                return ThermounitAttributeArray([getattr(u, idx) for u in self.units])
-            elif not any([isinstance(unit, Thermounit) for unit in self.units]):
-                print(f'The instances (Thermounits) of this Thermopack are placeholders and have to be fully processed '
-                      f'before all attributes and metadata are available.')
-                self.decode()
-                return self[idx]  # Recursion
-            raise KeyError(f'Not a valid slice or column name: {idx}')
-
-        elif isinstance(idx, slice):
-            """ Slicing """
-            data_indices = range(len(self))
-            slice_indices = data_indices[slice(idx.start, idx.stop, idx.step)]
-            return Thermopack(self.dataset.select(slice_indices))
-
-        elif not isinstance(self.units[idx], Thermounit):
-            """ Decode labels and predictions """
-            instance = self.units[idx]
-
-            # Overwrite true (HF dataset) label indices with custom label indices from downstream model
-            #  (some MNLI and XNLI models have a different order in the label names)
-            true_label_index = self.label_names.index(self.legacy_label_names[instance.label])
-            true_label = {'index': true_label_index,
-                          'name': self.label_names[true_label_index]}
-
-            predicted_label_index = instance.predictions.index(max(instance.predictions))
-            predicted_label = {'index': predicted_label_index,
-                               'name': self.label_names[predicted_label_index]}
-
-            tunit = Thermounit(instance, true_label, predicted_label, self.model_name, self.dataset_name,
-                               self.explainer_name, self.tokenizer, self.config_name)
-            self.units[idx] = tunit
-        return self.units[idx]
-
-    @overrides
-    def __iter__(self):
-        """ Yields Thermounit instances """
-        for unit_index in range(len(self)):  # length of dataset
-            yield self[unit_index]  # uses __getitem__
-
-    @overrides
-    def __str__(self):
-        return self.info.description
-
-    @property
-    def label_names(self):
-        gold_label_names = additional_configs.get_label_names(self.config_name)
-        if gold_label_names:
-            return gold_label_names
-        else:
-            return self.legacy_label_names
-
-    def decode(self):
-        """ Replace all PlaceholderThermounit instances with fully processed Thermounit instances """
-        for unit in tqdm(self, desc='Decoding Thermounits', total=len(self)):
-            u = unit
-
-    @lazy_property
-    def tokenizer(self):
-        """ Initializes the tokenizer from the model name """
-        return AutoTokenizer.from_pretrained(self.model_name)
-
-    def accuracy(self):
-        return sum([u_i.true_label == u_i.predicted_label for u_i in self])/len(self)
-
-    def classification_report(self):
-        """ Uses sklearn to print the confusion matrix """
-        y_true = self['true_label_index']
-        y_pred = self['predicted_label_index']
-        print(classification_report(y_true, y_pred, target_names=self.label_names))
-
-    def true_pred_counter(self):
-        from collections import Counter
-        if 'true_label_index' not in self.units[0].__dict__:
-            self.decode()
-        return Counter([(m_i.true_label_index, m_i.predicted_label_index) for m_i in self.units])
-
-
-class PlaceholderThermounit:
-    """ Raw single instance of a Thermopack. Accessing units of a Thermopack will automatically cast these to
-     Thermounits. This class exists for efficiency purposes. Properly processing an entire dataset while loading it
-     takes too long. """
-    def __init__(self, attributions, idx, input_ids, label, predictions):
-        self.attributions = attributions
-        self.idx = idx
-        self.input_ids = input_ids
-        self.label = label
-        self.predictions = predictions
-
-
-class ThermounitAttributeArray(np.ndarray):
-    """ NumPy Array of a list of attribute values of Thermopack units
-     Follows: https://numpy.org/devdocs/user/basics.subclassing.html"""
-    def __new__(cls, array, info=None):
-        # Input array is an already formed ndarray instance
-        # We first cast to be our class type
-        obj = np.asarray(array).view(cls)
-        # add the new attribute to the created instance
-        obj.info = info
-        # Finally, we must return the newly created object:
-        return obj
-
-    def __array_finalize__(self, obj):
-        if obj is None:
-            return
-        self.info = getattr(obj, 'info', None)
-
-
-class Thermounit(PlaceholderThermounit):
-    """ Processed single instance of a Thermopack (Thermostat dataset/configuration) """
-    def __init__(self, instance, true_label, predicted_label, model_name, dataset_name, explainer_name, tokenizer,
-                 config_name):
-        if not isinstance(instance, Thermounit):
-            super().__init__(*instance.__dict__.values())
-        for key in instance.__dict__:
-            setattr(self, key, instance.__dict__[key])
-        self.true_label = true_label['name']
-        self.true_label_index = true_label['index']
-        self.predicted_label = predicted_label['name']
-        self.predicted_label_index = predicted_label['index']
-        self.model_name = model_name
-        self.dataset_name = dataset_name
-        self.explainer_name = explainer_name
-        self.tokenizer = tokenizer
-        self.config_name = config_name
-
-    def __len__(self):
-        return len(self.explanation)
-
-    @property
-    def tokens(self) -> Dict:
-        # "tokens" includes all special tokens, later used for the heatmap when aligning with attributions
-        tokens = self.tokenizer.convert_ids_to_tokens(self.input_ids)
-        # Make token index
-        tokens_enum = dict(enumerate(tokens))
-        return tokens_enum
-
-    @property
-    def text_fields(self):
-        # Set text_fields attribute, e.g. containing "premise" and "hypothesis"
-        return get_text_fields(self.config_name)
-
-    def fill_text_fields(self, fuse_subwords_strategy='salient'):
-        """ Use detokenizer to fill text fields """
-
-        # Determine groups of tokens split by [SEP] tokens
-        text_groups = []
-        for group in [list(g) for k, g in groupby(self.tokens.items(),
-                                                  lambda kt: kt[1] != self.tokenizer.sep_token) if k]:
-            # Remove groups that only contain special tokens
-            if len([t for t in group if t[1] not in self.tokenizer.all_special_tokens]) < len(group):
-                text_groups.append(group)
-
-        # Assign text field values based on groups
-        for text_field, field_tokens in zip(self.text_fields, text_groups):
-            # Create new list containing all non-special tokens
-            non_special_tokens_enum = [t for t in field_tokens if t[1] not in self.tokenizer.all_special_tokens]
-            # Select attributions according to token indices (tokens_enum keys)
-
-            selected_atts = [self.attributions[idx] for idx in [t[0] for t in non_special_tokens_enum]]
-            if fuse_subwords_strategy:
-                tokens_enum, atts = fuse_subwords(non_special_tokens_enum, selected_atts, self.tokenizer,
-                                                  strategy=fuse_subwords_strategy)
-            else:
-                tokens_enum, atts = non_special_tokens_enum, selected_atts
-
-            assert (len(tokens_enum) == len(atts))
-            # Cast each token into ColorToken objects with default color white which can later be overwritten
-            # by a Heatmap object
-            color_tokens = [ColorToken(token=token_enum[1],
-                                       attribution=att,
-                                       text_field=text_field,
-                                       token_index=token_enum[0],
-                                       thermounit_vars=vars(self))
-                            for token_enum, att in zip(tokens_enum, atts)]
-
-            # Set class attribute with the name of the text field
-            setattr(self, text_field, Heatmap(color_tokens))
-
-        # Introduce a texts attribute that also stores all assigned text fields into a dict with the key being the
-        # name of each text field
-        setattr(self, 'texts', {text_field: getattr(self, text_field) for text_field in self.text_fields})
-
-    @property
-    def explanation(self, keep_padding_tokens=False):
-        """ Token-attribution tuples of a Thermounit """
-        if keep_padding_tokens:
-            tokens = self.tokens
-        else:
-            tokens = [(idx, token) for idx, token in self.tokens.items() if token != self.tokenizer.pad_token]
-        attributions = [att for i, att in enumerate(self.attributions) if i in [t[0] for t in tokens]]
-        token_att_tuples = list(zip([t[1] for t in tokens], attributions, [t[0] for t in tokens]))
-
-        return token_att_tuples
-
-    @property
-    def heatmap(self, gamma=1.0, normalize=True, flip_attributions_idx=None, fuse_subwords_strategy='salient'):
-        """ Generate a heatmap from explanation (!) data (without instantiating text fields)
-         for a single data point of a Thermostat dataset """
-
-        # Handle attributions, apply normalization and sign flipping if needed
-        atts = [x[1] for x in self.explanation]
-        if normalize:
-            atts = normalize_attributions(atts)
-        if flip_attributions_idx == self.predicted_label:
-            atts = [att * -1 for att in atts]
-
-        non_pad_tokens_enum = [tuple(x[i] for i in [2, 0]) for x in self.explanation]
-        if fuse_subwords_strategy:
-            tokens_enum, atts = fuse_subwords(non_pad_tokens_enum, atts, self.tokenizer,
-                                              strategy=fuse_subwords_strategy)
-        else:
-            tokens_enum, atts = non_pad_tokens_enum, atts
-
-        assert (len(tokens_enum) == len(atts))
-        # Cast each token into ColorToken objects with default color white which can later be overwritten
-        # by a Heatmap object
-        color_tokens = [ColorToken(token=token_enum[1],
-                                   attribution=att,
-                                   text_field='text',
-                                   token_index=token_enum[0],
-                                   thermounit_vars=vars(self))
-                        for token_enum, att in zip(tokens_enum, atts)]
-        return Heatmap(color_tokens=color_tokens, attributions=atts, gamma=gamma)
-
-    def render(self, labels=False):
-        self.heatmap.render(labels=labels)
-
-
-def list_configs():
-    """ Returns the list of names of all available configs in the Thermostat HF dataset"""
-    return [config.name for config in thermostat_configs.builder_configs]
-
-
-def get_config(config_name):
-    """ Returns a ThermostatConfig if a config exists by the name of `config_name`, else returns None
-     based on : https://stackoverflow.com/a/7125547 """
-    return next((x for x in thermostat_configs.builder_configs if x.name == config_name), None)
-
-
-def get_text_fields(config_name):
-    """ Returns a list of the text fields in a Thermostat config """
-    text_fields = get_config(config_name).text_column
-    if type(text_fields) != list:
-        text_fields = [text_fields]
-    return text_fields
-
-
-def load(config_str: str = None, **kwargs) -> Thermopack:
-    """
-    Wrapper around the load_dataset method from the HF datasets library:
-    https://huggingface.co/docs/datasets/package_reference/loading_methods.html#datasets.load_dataset
-    :param config_str: equivalent to the second argument (`name`) of `datasets.load_dataset`. The value has to be one of
-    the available configs in `thermostat.data.thermostat_configs.builder_configs` (accessible via `list_configs()`).
-    :param kwargs: Additional keywords will all be passed to `datasets.load_dataset`. `path`, `name` and `split` are
-    already reserved.
-    """
-    assert config_str, f'Please enter a config. Available options: {list_configs()}'
-    assert config_str in list_configs(), f'Invalid config. Available options: {list_configs()}'
-
-    """ Following https://stackoverflow.com/a/23430335/6788442 """
-    ld_kwargs = {key: value for key, value in kwargs.items() if
-                 key in load_dataset.__code__.co_varnames and key not in ['path', 'name', 'split']}
-
-    print(f'Loading Thermostat configuration: {config_str}')
-    if ld_kwargs:
-        print(f'Additional parameters for loading: {ld_kwargs}')
-    # new change
-    if platform == "win32":
-       dataset_script_path = os.path.dirname(os.path.realpath(__file__)).replace('\\thermostat\\data',
-                                                                              '\\thermostat\\dataset.py')
-    else:
-        dataset_script_path = os.path.dirname(os.path.realpath(__file__)).replace('/thermostat/data',
-                                                                              '/thermostat/dataset.py')
-    # new change
-    
-    data = load_dataset(path=dataset_script_path,
-                        name=config_str, split="test", **ld_kwargs)
-
-    return Thermopack(data)
-
-
-def get_coordinate(thermostat_dataset: Dataset, coordinate: str) -> str:
-    """ Determine a coordinate (dataset, model, or explainer) of a Thermostat dataset from its description """
-    assert coordinate in ['Model', 'Dataset', 'Explainer']
-    coord_prefix = f'{coordinate}: '
-    assert coord_prefix in thermostat_dataset.description
-    str_post_coord_prefix = thermostat_dataset.description.split(coord_prefix)[1]
-    if '\n' in str_post_coord_prefix:
-        coord_value = str_post_coord_prefix.split('\n')[0]
-    else:
-        coord_value = str_post_coord_prefix
-    return coord_value
+import numpy as np
+import os
+# new change 
+from sys import platform
+# new change
+from datasets import Dataset, load_dataset
+from itertools import groupby
+from overrides import overrides
+from sklearn.metrics import classification_report
+from tqdm import tqdm
+from transformers import AutoTokenizer
+from typing import Dict, List
+
+from thermostat.data import additional_configs, thermostat_configs
+from thermostat.data.tokenization import fuse_subwords
+from thermostat.utils import lazy_property
+from thermostat.visualize import ColorToken, Heatmap, normalize_attributions
+
+
+class ThermopackMeta(type):
+    """ Inspired by: https://stackoverflow.com/a/65917858 """
+    def __new__(mcs, name, bases, dct):
+        child = super().__new__(mcs, name, bases, dct)
+        for base in bases:
+            for field_name, field in base.__dict__.items():
+                if callable(field) and not field_name.startswith('__'):
+                    setattr(child, field_name, mcs.force_child(field, field_name, base, child))
+        return child
+
+    @staticmethod
+    def force_child(fun, fun_name, base, child):
+        """Turn from Base- to Child-instance-returning function."""
+        def wrapper(*args, **kwargs):
+            result = fun(*args, **kwargs)
+            if result is None:
+                # Ignore if returns None
+                return None
+            if type(result) == base:
+                print(fun_name)
+                # Return Child instance if the Base method tries to return Base instance.
+                return child(result)
+            return result
+        return wrapper
+
+
+class Thermopack(Dataset, metaclass=ThermopackMeta):
+    def __init__(self, hf_dataset):
+        # Init Dataset super class
+        super().__init__(hf_dataset.data, info=hf_dataset.info, split=hf_dataset.split,
+                         indices_table=hf_dataset._indices)
+
+        # Model
+        self.model_name = get_coordinate(hf_dataset, 'Model')
+        # Dataset
+        self.dataset_name = get_coordinate(hf_dataset, 'Dataset')
+        # Explainer
+        self.explainer_name = get_coordinate(hf_dataset, 'Explainer')
+
+        self.dataset: Dataset = hf_dataset
+        self.units: List = [PlaceholderThermounit(unit['attributions'],
+                                                  unit['idx'],
+                                                  unit['input_ids'],
+                                                  unit['label'],
+                                                  unit['predictions']) for unit in self.dataset]
+        self.legacy_label_names = get_config(self.config_name).label_classes
+
+    def __getattr__(self, name):
+        """ Only gets called if an attribute that is not part of the Thermopack is accessed.
+         In this case, if the name of the requested attribute is one of the five attributes of a Thermounit,
+         return the respective entries of all units as a list """
+        if name in list(self.units[0].__dict__.keys()):
+            return ThermounitAttributeArray([getattr(u, name) for u in self.units])
+        else:
+            raise AttributeError
+
+    @overrides
+    def __getitem__(self, idx):
+        """ Indexing a Thermopack by an integer instantiates a Thermounit and returns it.
+            Indexing by string returns the associated column if its exists (similar to HF datasets). """
+
+        if isinstance(idx, str):
+            """ String indexing """
+            if idx in list(self.units[0].__dict__.keys()):
+                """ Same behaviour as __getattr__: Return the requested attribute of all units as a list. """
+                return ThermounitAttributeArray([getattr(u, idx) for u in self.units])
+            elif not any([isinstance(unit, Thermounit) for unit in self.units]):
+                print(f'The instances (Thermounits) of this Thermopack are placeholders and have to be fully processed '
+                      f'before all attributes and metadata are available.')
+                self.decode()
+                return self[idx]  # Recursion
+            raise KeyError(f'Not a valid slice or column name: {idx}')
+
+        elif isinstance(idx, slice):
+            """ Slicing """
+            data_indices = range(len(self))
+            slice_indices = data_indices[slice(idx.start, idx.stop, idx.step)]
+            return Thermopack(self.dataset.select(slice_indices))
+
+        elif not isinstance(self.units[idx], Thermounit):
+            """ Decode labels and predictions """
+            instance = self.units[idx]
+
+            # Overwrite true (HF dataset) label indices with custom label indices from downstream model
+            #  (some MNLI and XNLI models have a different order in the label names)
+            true_label_index = self.label_names.index(self.legacy_label_names[instance.label])
+            true_label = {'index': true_label_index,
+                          'name': self.label_names[true_label_index]}
+
+            predicted_label_index = instance.predictions.index(max(instance.predictions))
+            predicted_label = {'index': predicted_label_index,
+                               'name': self.label_names[predicted_label_index]}
+
+            tunit = Thermounit(instance, true_label, predicted_label, self.model_name, self.dataset_name,
+                               self.explainer_name, self.tokenizer, self.config_name)
+            self.units[idx] = tunit
+        return self.units[idx]
+
+    @overrides
+    def __iter__(self):
+        """ Yields Thermounit instances """
+        for unit_index in range(len(self)):  # length of dataset
+            yield self[unit_index]  # uses __getitem__
+
+    @overrides
+    def __str__(self):
+        return self.info.description
+
+    @property
+    def label_names(self):
+        gold_label_names = additional_configs.get_label_names(self.config_name)
+        if gold_label_names:
+            return gold_label_names
+        else:
+            return self.legacy_label_names
+
+    def decode(self):
+        """ Replace all PlaceholderThermounit instances with fully processed Thermounit instances """
+        for unit in tqdm(self, desc='Decoding Thermounits', total=len(self)):
+            u = unit
+
+    @lazy_property
+    def tokenizer(self):
+        """ Initializes the tokenizer from the model name """
+        return AutoTokenizer.from_pretrained(self.model_name)
+
+    def accuracy(self):
+        return sum([u_i.true_label == u_i.predicted_label for u_i in self])/len(self)
+
+    def classification_report(self):
+        """ Uses sklearn to print the confusion matrix """
+        y_true = self['true_label_index']
+        y_pred = self['predicted_label_index']
+        print(classification_report(y_true, y_pred, target_names=self.label_names))
+
+    def true_pred_counter(self):
+        from collections import Counter
+        if 'true_label_index' not in self.units[0].__dict__:
+            self.decode()
+        return Counter([(m_i.true_label_index, m_i.predicted_label_index) for m_i in self.units])
+
+
+class PlaceholderThermounit:
+    """ Raw single instance of a Thermopack. Accessing units of a Thermopack will automatically cast these to
+     Thermounits. This class exists for efficiency purposes. Properly processing an entire dataset while loading it
+     takes too long. """
+    def __init__(self, attributions, idx, input_ids, label, predictions):
+        self.attributions = attributions
+        self.idx = idx
+        self.input_ids = input_ids
+        self.label = label
+        self.predictions = predictions
+
+
+class ThermounitAttributeArray(np.ndarray):
+    """ NumPy Array of a list of attribute values of Thermopack units
+     Follows: https://numpy.org/devdocs/user/basics.subclassing.html"""
+    def __new__(cls, array, info=None):
+        # Input array is an already formed ndarray instance
+        # We first cast to be our class type
+        obj = np.asarray(array).view(cls)
+        # add the new attribute to the created instance
+        obj.info = info
+        # Finally, we must return the newly created object:
+        return obj
+
+    def __array_finalize__(self, obj):
+        if obj is None:
+            return
+        self.info = getattr(obj, 'info', None)
+
+
+class Thermounit(PlaceholderThermounit):
+    """ Processed single instance of a Thermopack (Thermostat dataset/configuration) """
+    def __init__(self, instance, true_label, predicted_label, model_name, dataset_name, explainer_name, tokenizer,
+                 config_name):
+        if not isinstance(instance, Thermounit):
+            super().__init__(*instance.__dict__.values())
+        for key in instance.__dict__:
+            setattr(self, key, instance.__dict__[key])
+        self.true_label = true_label['name']
+        self.true_label_index = true_label['index']
+        self.predicted_label = predicted_label['name']
+        self.predicted_label_index = predicted_label['index']
+        self.model_name = model_name
+        self.dataset_name = dataset_name
+        self.explainer_name = explainer_name
+        self.tokenizer = tokenizer
+        self.config_name = config_name
+
+    def __len__(self):
+        return len(self.explanation)
+
+    @property
+    def tokens(self) -> Dict:
+        # "tokens" includes all special tokens, later used for the heatmap when aligning with attributions
+        tokens = self.tokenizer.convert_ids_to_tokens(self.input_ids)
+        # Make token index
+        tokens_enum = dict(enumerate(tokens))
+        return tokens_enum
+
+    @property
+    def text_fields(self):
+        # Set text_fields attribute, e.g. containing "premise" and "hypothesis"
+        return get_text_fields(self.config_name)
+
+    def fill_text_fields(self, fuse_subwords_strategy='salient'):
+        """ Use detokenizer to fill text fields """
+
+        # Determine groups of tokens split by [SEP] tokens
+        text_groups = []
+        for group in [list(g) for k, g in groupby(self.tokens.items(),
+                                                  lambda kt: kt[1] != self.tokenizer.sep_token) if k]:
+            # Remove groups that only contain special tokens
+            if len([t for t in group if t[1] not in self.tokenizer.all_special_tokens]) < len(group):
+                text_groups.append(group)
+
+        # Assign text field values based on groups
+        for text_field, field_tokens in zip(self.text_fields, text_groups):
+            # Create new list containing all non-special tokens
+            non_special_tokens_enum = [t for t in field_tokens if t[1] not in self.tokenizer.all_special_tokens]
+            # Select attributions according to token indices (tokens_enum keys)
+
+            selected_atts = [self.attributions[idx] for idx in [t[0] for t in non_special_tokens_enum]]
+            if fuse_subwords_strategy:
+                tokens_enum, atts = fuse_subwords(non_special_tokens_enum, selected_atts, self.tokenizer,
+                                                  strategy=fuse_subwords_strategy)
+            else:
+                tokens_enum, atts = non_special_tokens_enum, selected_atts
+
+            assert (len(tokens_enum) == len(atts))
+            # Cast each token into ColorToken objects with default color white which can later be overwritten
+            # by a Heatmap object
+            color_tokens = [ColorToken(token=token_enum[1],
+                                       attribution=att,
+                                       text_field=text_field,
+                                       token_index=token_enum[0],
+                                       thermounit_vars=vars(self))
+                            for token_enum, att in zip(tokens_enum, atts)]
+
+            # Set class attribute with the name of the text field
+            setattr(self, text_field, Heatmap(color_tokens))
+
+        # Introduce a texts attribute that also stores all assigned text fields into a dict with the key being the
+        # name of each text field
+        setattr(self, 'texts', {text_field: getattr(self, text_field) for text_field in self.text_fields})
+
+    @property
+    def explanation(self, keep_padding_tokens=False):
+        """ Token-attribution tuples of a Thermounit """
+        if keep_padding_tokens:
+            tokens = self.tokens
+        else:
+            tokens = [(idx, token) for idx, token in self.tokens.items() if token != self.tokenizer.pad_token]
+        attributions = [att for i, att in enumerate(self.attributions) if i in [t[0] for t in tokens]]
+        token_att_tuples = list(zip([t[1] for t in tokens], attributions, [t[0] for t in tokens]))
+
+        return token_att_tuples
+
+    @property
+    def heatmap(self, gamma=1.0, normalize=True, flip_attributions_idx=None, fuse_subwords_strategy='salient'):
+        """ Generate a heatmap from explanation (!) data (without instantiating text fields)
+         for a single data point of a Thermostat dataset """
+
+        # Handle attributions, apply normalization and sign flipping if needed
+        atts = [x[1] for x in self.explanation]
+        if normalize:
+            atts = normalize_attributions(atts)
+        if flip_attributions_idx == self.predicted_label:
+            atts = [att * -1 for att in atts]
+
+        non_pad_tokens_enum = [tuple(x[i] for i in [2, 0]) for x in self.explanation]
+        if fuse_subwords_strategy:
+            tokens_enum, atts = fuse_subwords(non_pad_tokens_enum, atts, self.tokenizer,
+                                              strategy=fuse_subwords_strategy)
+        else:
+            tokens_enum, atts = non_pad_tokens_enum, atts
+
+        assert (len(tokens_enum) == len(atts))
+        # Cast each token into ColorToken objects with default color white which can later be overwritten
+        # by a Heatmap object
+        color_tokens = [ColorToken(token=token_enum[1],
+                                   attribution=att,
+                                   text_field='text',
+                                   token_index=token_enum[0],
+                                   thermounit_vars=vars(self))
+                        for token_enum, att in zip(tokens_enum, atts)]
+        return Heatmap(color_tokens=color_tokens, attributions=atts, gamma=gamma)
+
+    def render(self, labels=False):
+        self.heatmap.render(labels=labels)
+
+
+def list_configs():
+    """ Returns the list of names of all available configs in the Thermostat HF dataset"""
+    return [config.name for config in thermostat_configs.builder_configs]
+
+
+def get_config(config_name):
+    """ Returns a ThermostatConfig if a config exists by the name of `config_name`, else returns None
+     based on : https://stackoverflow.com/a/7125547 """
+    return next((x for x in thermostat_configs.builder_configs if x.name == config_name), None)
+
+
+def get_text_fields(config_name):
+    """ Returns a list of the text fields in a Thermostat config """
+    text_fields = get_config(config_name).text_column
+    if type(text_fields) != list:
+        text_fields = [text_fields]
+    return text_fields
+
+
+def load(config_str: str = None, **kwargs) -> Thermopack:
+    """
+    Wrapper around the load_dataset method from the HF datasets library:
+    https://huggingface.co/docs/datasets/package_reference/loading_methods.html#datasets.load_dataset
+    :param config_str: equivalent to the second argument (`name`) of `datasets.load_dataset`. The value has to be one of
+    the available configs in `thermostat.data.thermostat_configs.builder_configs` (accessible via `list_configs()`).
+    :param kwargs: Additional keywords will all be passed to `datasets.load_dataset`. `path`, `name` and `split` are
+    already reserved.
+    """
+    assert config_str, f'Please enter a config. Available options: {list_configs()}'
+    assert config_str in list_configs(), f'Invalid config. Available options: {list_configs()}'
+
+    """ Following https://stackoverflow.com/a/23430335/6788442 """
+    ld_kwargs = {key: value for key, value in kwargs.items() if
+                 key in load_dataset.__code__.co_varnames and key not in ['path', 'name', 'split']}
+
+    print(f'Loading Thermostat configuration: {config_str}')
+    if ld_kwargs:
+        print(f'Additional parameters for loading: {ld_kwargs}')
+    # new change
+    if platform == "win32":
+       dataset_script_path = os.path.dirname(os.path.realpath(__file__)).replace('\\thermostat\\data',
+                                                                              '\\thermostat\\dataset.py')
+    else:
+        dataset_script_path = os.path.dirname(os.path.realpath(__file__)).replace('/thermostat/data',
+                                                                              '/thermostat/dataset.py')
+    # new change
+    
+    data = load_dataset(path=dataset_script_path,
+                        name=config_str, split="test", **ld_kwargs)
+
+    return Thermopack(data)
+
+
+def get_coordinate(thermostat_dataset: Dataset, coordinate: str) -> str:
+    """ Determine a coordinate (dataset, model, or explainer) of a Thermostat dataset from its description """
+    assert coordinate in ['Model', 'Dataset', 'Explainer']
+    coord_prefix = f'{coordinate}: '
+    assert coord_prefix in thermostat_dataset.description
+    str_post_coord_prefix = thermostat_dataset.description.split(coord_prefix)[1]
+    if '\n' in str_post_coord_prefix:
+        coord_value = str_post_coord_prefix.split('\n')[0]
+    else:
+        coord_value = str_post_coord_prefix
+    return coord_value
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat/data/readers.py` & `thermostat-datasets-1.1.0/src/thermostat/data/readers.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-from datasets import load_dataset, load_from_disk
-from transformers import AutoTokenizer
-from typing import Dict, List
-
-
-def download_dataset(config: Dict, logger):
-    """
-    :param config: "dataset" sub-config of a jsonnet config
-    """
-    assert all(x in config for x in ['name', 'split', 'root_dir'])
-    if 'subset' in config:
-        dataset = load_dataset(config['name'], config['subset'], split=config['split'])
-        dataset.save_to_disk(dataset_path=f'{config["root_dir"]}/{config["name"]}_{config["subset"]}')
-    else:
-        dataset = load_dataset(config['name'], split=config['split'])
-        dataset.save_to_disk(dataset_path=f'{config["root_dir"]}/{config["name"]}')
-    logger.info(f'(Progress) Terminated normally')
-
-
-def get_dataset(config: Dict):
-    """ Returns a pytorch dataset from a config. """
-    assert 'tokenizer' in config
-    tokenizer = config['tokenizer']
-    dataset_config = config['dataset']
-    tokenization_config = config['model']['tokenization']
-
-    def encode(instances):
-        return tokenizer(instances[text_field],
-                         truncation=tokenization_config['truncation'],
-                         padding=tokenization_config['padding'],
-                         max_length=tokenization_config['max_length'],
-                         return_special_tokens_mask=tokenization_config['special_tokens_mask'])
-
-    def encode_pair(instances):
-        return tokenizer(instances[text_field[0]],
-                         instances[text_field[1]],
-                         truncation=tokenization_config['truncation'],
-                         padding=tokenization_config['padding'],
-                         max_length=tokenization_config['max_length'],
-                         return_special_tokens_mask=tokenization_config['special_tokens_mask'])
-
-    # Handle datasets with subsets correctly, e.g. "glue" has "sst2" and "qqp" as their subsets
-    dataset_dir = f'{dataset_config["name"]}_' \
-                  f'{dataset_config["subset"]}' if 'subset' in dataset_config else dataset_config['name']
-    try:
-        dataset = load_from_disk(f'{dataset_config["root_dir"]}/{dataset_dir}')
-    except FileNotFoundError:
-        raise FileNotFoundError(f'Execute download_data.py to first store the missing dataset ({dataset_dir}) '
-                                f'locally.')
-
-    dataset = dataset.select(indices=get_dataset_index_range(dataset, dataset_config))
-
-    if 'text_field' in dataset_config:
-        text_field = dataset_config['text_field']
-    else:
-        text_field = 'text'
-    encode_fn = encode_pair if type(text_field) == list and len(text_field) else encode
-    dataset = dataset.map(encode_fn, batched=True, batch_size=dataset_config['batch_size'])
-
-    if 'label_field' in dataset_config:
-        label_field = dataset_config['label_field']
-        expression = label_field['expression']
-    else:
-        label_field = 'label'
-
-    def get_label(example: Dict):
-        if type(label_field) == str:
-            return example[label_field]
-        else:
-            try:
-                return eval('example' + expression)
-            except IndexError:
-                return None
-
-    dataset = dataset.map(lambda examples: {'labels': get_label(examples)},
-                          batch_size=dataset_config['batch_size'])  # batched=True,
-    dataset.set_format(type='torch', columns=dataset_config['columns'])
-    return dataset
-
-
-def get_dataset_index_range(dataset, dataset_config):
-    start = 0 if 'start' not in dataset_config else dataset_config['start']
-    if start < 0:
-        start = 0
-
-    end = len(dataset) if 'end' not in dataset_config else dataset_config['end']
-    if end < 0:
-        end = len(dataset)
-
-    return range(start, end)
-
-
-def get_local_explanations(config: Dict):
-    """
-    :param config: visualization dict of config
-    :return:
-    """
-
-    dataset = load_dataset('json', data_files=config['path_explanations'])
-    dataset = dataset['train']
-
-    def encode_local(instances):
-        res = {k: instances[k] for k in config['columns']}
-        return res
-
-    dataset = dataset.map(encode_local, batched=True)
-    dataset.set_format(type='torch', columns=config['columns'])
-    return dataset
-
-
-def get_tokenizer(config: Dict):
-    """
-    :param config: model sub-config
-    :return:
-    """
-    tokenizer = AutoTokenizer.from_pretrained(config['name'])
-    return tokenizer
+from datasets import load_dataset, load_from_disk
+from transformers import AutoTokenizer
+from typing import Dict, List
+
+
+def download_dataset(config: Dict, logger):
+    """
+    :param config: "dataset" sub-config of a jsonnet config
+    """
+    assert all(x in config for x in ['name', 'split', 'root_dir'])
+    if 'subset' in config:
+        dataset = load_dataset(config['name'], config['subset'], split=config['split'])
+        dataset.save_to_disk(dataset_path=f'{config["root_dir"]}/{config["name"]}_{config["subset"]}')
+    else:
+        dataset = load_dataset(config['name'], split=config['split'])
+        dataset.save_to_disk(dataset_path=f'{config["root_dir"]}/{config["name"]}')
+    logger.info(f'(Progress) Terminated normally')
+
+
+def get_dataset(config: Dict):
+    """ Returns a pytorch dataset from a config. """
+    assert 'tokenizer' in config
+    tokenizer = config['tokenizer']
+    dataset_config = config['dataset']
+    tokenization_config = config['model']['tokenization']
+
+    def encode(instances):
+        return tokenizer(instances[text_field],
+                         truncation=tokenization_config['truncation'],
+                         padding=tokenization_config['padding'],
+                         max_length=tokenization_config['max_length'],
+                         return_special_tokens_mask=tokenization_config['special_tokens_mask'])
+
+    def encode_pair(instances):
+        return tokenizer(instances[text_field[0]],
+                         instances[text_field[1]],
+                         truncation=tokenization_config['truncation'],
+                         padding=tokenization_config['padding'],
+                         max_length=tokenization_config['max_length'],
+                         return_special_tokens_mask=tokenization_config['special_tokens_mask'])
+
+    # Handle datasets with subsets correctly, e.g. "glue" has "sst2" and "qqp" as their subsets
+    dataset_dir = f'{dataset_config["name"]}_' \
+                  f'{dataset_config["subset"]}' if 'subset' in dataset_config else dataset_config['name']
+    try:
+        dataset = load_from_disk(f'{dataset_config["root_dir"]}/{dataset_dir}')
+    except FileNotFoundError:
+        raise FileNotFoundError(f'Execute download_data.py to first store the missing dataset ({dataset_dir}) '
+                                f'locally.')
+
+    dataset = dataset.select(indices=get_dataset_index_range(dataset, dataset_config))
+
+    if 'text_field' in dataset_config:
+        text_field = dataset_config['text_field']
+    else:
+        text_field = 'text'
+    encode_fn = encode_pair if type(text_field) == list and len(text_field) else encode
+    dataset = dataset.map(encode_fn, batched=True, batch_size=dataset_config['batch_size'])
+
+    if 'label_field' in dataset_config:
+        label_field = dataset_config['label_field']
+        expression = label_field['expression']
+    else:
+        label_field = 'label'
+
+    def get_label(example: Dict):
+        if type(label_field) == str:
+            return example[label_field]
+        else:
+            try:
+                return eval('example' + expression)
+            except IndexError:
+                return None
+
+    dataset = dataset.map(lambda examples: {'labels': get_label(examples)},
+                          batch_size=dataset_config['batch_size'])  # batched=True,
+    dataset.set_format(type='torch', columns=dataset_config['columns'])
+    return dataset
+
+
+def get_dataset_index_range(dataset, dataset_config):
+    start = 0 if 'start' not in dataset_config else dataset_config['start']
+    if start < 0:
+        start = 0
+
+    end = len(dataset) if 'end' not in dataset_config else dataset_config['end']
+    if end < 0:
+        end = len(dataset)
+
+    return range(start, end)
+
+
+def get_local_explanations(config: Dict):
+    """
+    :param config: visualization dict of config
+    :return:
+    """
+
+    dataset = load_dataset('json', data_files=config['path_explanations'])
+    dataset = dataset['train']
+
+    def encode_local(instances):
+        res = {k: instances[k] for k in config['columns']}
+        return res
+
+    dataset = dataset.map(encode_local, batched=True)
+    dataset.set_format(type='torch', columns=config['columns'])
+    return dataset
+
+
+def get_tokenizer(config: Dict):
+    """
+    :param config: model sub-config
+    :return:
+    """
+    tokenizer = AutoTokenizer.from_pretrained(config['name'])
+    return tokenizer
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat/data/thermostat_configs.py` & `thermostat-datasets-1.1.0/src/thermostat/data/thermostat_configs.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,1191 +1,1191 @@
-import datasets
-
-
-_VERSION = datasets.Version('1.0.2', '')
-
-
-# Base arguments for any dataset
-_BASE_KWARGS = dict(
-    features={
-        "attributions": "attributions",
-        "predictions": "predictions",
-        "input_ids": "input_ids",
-    },
-    citation="Coming soon.",
-    url="https://github.com/DFKI-NLP/",
-)
-
-
-# Base arguments for AG News dataset
-_AGNEWS_KWARGS = dict(
-    dataset="ag_news",
-    label_classes=["World", "Sports", "Business", "Sci/Tech"],
-    label_column="label",
-    text_column="text",
-    **_BASE_KWARGS,
-)
-_AGNEWS_ALBERT_KWARGS = dict(
-    model="textattack/albert-base-v2-ag-news",
-    **_AGNEWS_KWARGS,
-)
-_AGNEWS_BERT_KWARGS = dict(
-    model="textattack/bert-base-uncased-ag-news",
-    **_AGNEWS_KWARGS,
-)
-_AGNEWS_ROBERTA_KWARGS = dict(
-    model="textattack/roberta-base-ag-news",
-    **_AGNEWS_KWARGS,
-)
-
-# Base arguments for IMDb dataset
-_IMDB_KWARGS = dict(
-    dataset="imdb",
-    label_classes=["neg", "pos"],
-    label_column="label",
-    text_column="text",
-    **_BASE_KWARGS,
-)
-_IMDB_ALBERT_KWARGS = dict(
-    model="textattack/albert-base-v2-imdb",
-    **_IMDB_KWARGS,
-)
-_IMDB_BERT_KWARGS = dict(
-    model="textattack/bert-base-uncased-imdb",
-    **_IMDB_KWARGS,
-)
-_IMDB_ELECTRA_KWARGS = dict(
-    model="monologg/electra-small-finetuned-imdb",
-    **_IMDB_KWARGS,
-)
-_IMDB_ROBERTA_KWARGS = dict(
-    model="textattack/roberta-base-imdb",
-    **_IMDB_KWARGS,
-)
-_IMDB_XLNET_KWARGS = dict(
-    model="textattack/xlnet-base-cased-imdb",
-    **_IMDB_KWARGS,
-)
-
-# Base arguments for MNLI dataset
-_MNLI_KWARGS = dict(
-    dataset="multi_nli",
-    label_column="label",
-    label_classes=["entailment", "neutral", "contradiction"],
-    text_column=["premise", "hypothesis"],
-    **_BASE_KWARGS,
-)
-_MNLI_ALBERT_KWARGS = dict(
-    model="prajjwal1/albert-base-v2-mnli",
-    **_MNLI_KWARGS,
-)
-_MNLI_BERT_KWARGS = dict(
-    model="textattack/bert-base-uncased-MNLI",
-    **_MNLI_KWARGS,
-)
-_MNLI_ELECTRA_KWARGS = dict(
-    model="howey/electra-base-mnli",
-    **_MNLI_KWARGS,
-)
-_MNLI_ROBERTA_KWARGS = dict(
-    model="textattack/roberta-base-MNLI",
-    **_MNLI_KWARGS,
-)
-_MNLI_XLNET_KWARGS = dict(
-    model="textattack/xlnet-base-cased-MNLI",
-    **_MNLI_KWARGS,
-)
-
-# Base arguments for XNLI dataset
-_XNLI_KWARGS = dict(
-    dataset="xnli",
-    label_column="label",
-    label_classes=["entailment", "neutral", "contradiction"],
-    text_column=["premise", "hypothesis"],
-    **_BASE_KWARGS,
-)
-_XNLI_ALBERT_KWARGS = dict(
-    model="prajjwal1/albert-base-v2-mnli",
-    **_XNLI_KWARGS,
-)
-_XNLI_BERT_KWARGS = dict(
-    model="textattack/bert-base-uncased-MNLI",
-    **_XNLI_KWARGS,
-)
-_XNLI_ELECTRA_KWARGS = dict(
-    model="howey/electra-base-mnli",
-    **_XNLI_KWARGS,
-)
-_XNLI_ROBERTA_KWARGS = dict(
-    model="textattack/roberta-base-MNLI",
-    **_XNLI_KWARGS,
-)
-_XNLI_XLNET_KWARGS = dict(
-    model="textattack/xlnet-base-cased-MNLI",
-    **_XNLI_KWARGS,
-)
-
-
-class ThermostatConfig(datasets.BuilderConfig):
-    """ BuilderConfig for Thermostat """
-
-    def __init__(
-        self,
-        explainer,
-        model,
-        dataset,
-        features,
-        label_column,
-        label_classes,
-        text_column,
-        data_url,
-        citation,
-        url,
-        **kwargs,
-    ):
-        super(ThermostatConfig, self).__init__(version=_VERSION, **kwargs)
-        self.explainer = explainer
-        self.model = model
-        self.dataset = dataset
-        self.features = features
-        self.label_column = label_column
-        self.label_classes = label_classes
-        self.text_column = text_column
-        self.data_url = data_url
-        self.citation = citation
-        self.url = url
-
-
-builder_configs = [
-    ThermostatConfig(
-        name="ag_news-albert-lgxa",
-        description="AG News dataset, ALBERT model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/8XPC557ePpWCBQY/download",
-        **_AGNEWS_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="ag_news-albert-lig",
-        description="AG News dataset, ALBERT model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/zS7mcMsdAp5ZENX/download",
-        **_AGNEWS_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="ag_news-albert-lime",
-        description="AG News dataset, ALBERT model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/8SLyHdDgRk2pXSL/download",
-        **_AGNEWS_ALBERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="ag_news-albert-lime-100",
-        description="AG News dataset, ALBERT model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/W3GT4ZDT2BzR5mj/download",
-        **_AGNEWS_ALBERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="ag_news-albert-occlusion",
-        description="AG News dataset, ALBERT model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/Li9HwfKfFqjCQTM/download",
-        **_AGNEWS_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="ag_news-albert-svs",
-        description="AG News dataset, ALBERT model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/GLppwQjeBTsLtTC/download",
-        **_AGNEWS_ALBERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="ag_news-albert-lds",
-        description="AG News dataset, ALBERT model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/nzriaZHxniNtJBN/download",
-        **_AGNEWS_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="ag_news-albert-lgs",
-        description="AG News dataset, ALBERT model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/EjCXxWCETQH9onj/download",
-        **_AGNEWS_ALBERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="ag_news-bert-lgxa",
-        description="AG News dataset, BERT model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/zn5mKsryyrX3e58/download",
-        **_AGNEWS_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="ag_news-bert-lig",
-        description="AG News dataset, BERT model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/Qq3dR7sHsfX9JXZ/download",
-        **_AGNEWS_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="ag_news-bert-lime",
-        description="AG News dataset, BERT model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/rW8MJyAjBGQxsK9/download",
-        **_AGNEWS_BERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="ag_news-bert-lime-100",
-        description="AG News dataset, BERT model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/FkSdXZPpN78HSHR/download",
-        **_AGNEWS_BERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="ag_news-bert-occlusion",
-        description="AG News dataset, BERT model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/Grf97s6bJwoZGyx/download",
-        **_AGNEWS_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="ag_news-bert-svs",
-        description="AG News dataset, BERT model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/dCbgsjdW6b9pzo3/download",
-        **_AGNEWS_BERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="ag_news-bert-lds",
-        description="AG News dataset, BERT model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/XQzBnRniEyC8NEF/download",
-        **_AGNEWS_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="ag_news-bert-lgs",
-        description="AG News dataset, BERT model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/nHt4Ld4AKfbG2ft/download",
-        **_AGNEWS_BERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="ag_news-roberta-lgxa",
-        description="AG News dataset, RoBERTa model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/Kz9GrYrMZB4gp7E/download",
-        **_AGNEWS_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="ag_news-roberta-lig",
-        description="AG News dataset, RoBERTa model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/mpH8sT6tXDoG5qi/download",
-        **_AGNEWS_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="ag_news-roberta-lime",
-        description="AG News dataset, RoBERTa model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/qRgBtwfjaXceJoL/download",
-        **_AGNEWS_ROBERTA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="ag_news-roberta-lime-100",
-        description="AG News dataset, RoBERTa model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/kFyjX2LqBdcW9bp/download",
-        **_AGNEWS_ROBERTA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="ag_news-roberta-occlusion",
-        description="AG News dataset, RoBERTa model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/78aZttqxKQNdW6J/download",
-        **_AGNEWS_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="ag_news-roberta-svs",
-        description="AG News dataset, RoBERTa model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/yabEAY5sLpjxKkW/download",
-        **_AGNEWS_ROBERTA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="ag_news-roberta-lds",
-        description="AG News dataset, RoBERTa model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/ZWoxq27s36For98/download",
-        **_AGNEWS_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="ag_news-roberta-lgs",
-        description="AG News dataset, RoBERTa model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/HgHjNFcMQbCC2Nb/download",
-        **_AGNEWS_ROBERTA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="imdb-albert-lgxa",
-        description="IMDb dataset, ALBERT model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/srbYBbmKBsGMXWn/download",
-        **_IMDB_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-albert-lig",
-        description="IMDb dataset, ALBERT model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/zjMddcqewEcwSPG/download",
-        **_IMDB_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-albert-lime",
-        description="IMDb dataset, ALBERT model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/Tgktb4fq4EdXJNx/download",
-        **_IMDB_ALBERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="imdb-albert-lime-100",
-        description="IMDb dataset, ALBERT model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/FzErcT9TcFcG2Pr/download",
-        **_IMDB_ALBERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="imdb-albert-occ",
-        description="IMDb dataset, ALBERT model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/98XqEgbZt9KiSfm/download",
-        **_IMDB_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-albert-svs",
-        description="IMDb dataset, ALBERT model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/sQMK2XsknbzK23a/download",
-        **_IMDB_ALBERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="imdb-albert-lds",
-        description="IMDb dataset, ALBERT model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/SYg2GjRkewW8fn7/download",
-        **_IMDB_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-albert-lgs",
-        description="IMDb dataset, ALBERT model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/rWZfSzPN7Gm3Cko/download",
-        **_IMDB_ALBERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="imdb-bert-lgxa",
-        description="IMDb dataset, BERT model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/NkPpnyMN8rdWE7L/download",
-        **_IMDB_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-bert-lig",
-        description="IMDb dataset, BERT model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/SdrPeJQQSExFQ8e/download",
-        **_IMDB_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-bert-lime",
-        description="IMDb dataset, BERT model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/ZQEdEmFtKeGkYWp/download",
-        **_IMDB_BERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="imdb-bert-lime-100",
-        description="IMDb dataset, BERT model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/Qx7z8SFcMTB5bFa/download",
-        **_IMDB_BERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="imdb-bert-occ",
-        description="IMDb dataset, BERT model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/PjMDBzaoHHqs2WF/download",
-        **_IMDB_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-bert-svs",
-        description="IMDb dataset, BERT model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/DjmCKdBoWHt8jbX/download",
-        **_IMDB_BERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="imdb-bert-lds",
-        description="IMDb dataset, BERT model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/dnqSfrgGPYcYsKt/download",
-        **_IMDB_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-bert-lgs",
-        description="IMDb dataset, BERT model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/fnBqKxEjfsScqwg/download",
-        **_IMDB_BERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="imdb-electra-lgxa",
-        description="IMDb dataset, ELECTRA model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/WdLYpQerXC5KrHK/download",
-        **_IMDB_ELECTRA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-electra-lig",
-        description="IMDb dataset, ELECTRA model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/e3Mibf9dqRfobYw/download",
-        **_IMDB_ELECTRA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-electra-lime",
-        description="IMDb dataset, ELECTRA model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/7p2576kFqiQLL9x/download",
-        **_IMDB_ELECTRA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="imdb-electra-lime-100",
-        description="IMDb dataset, ELECTRA model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/LBqzn6JiQNzwMAC/download",
-        **_IMDB_ELECTRA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="imdb-electra-occ",
-        description="IMDb dataset, ELECTRA model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/TZYTgnySrEbm5Xx/download",
-        **_IMDB_ELECTRA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-electra-svs",
-        description="IMDb dataset, ELECTRA model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/MPHqZwJCP97sA4D/download",
-        **_IMDB_ELECTRA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="imdb-electra-lds",
-        description="IMDb dataset, ELECTRA model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/cHdECMFjHacAnFk/download",
-        **_IMDB_ELECTRA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-electra-lgs",
-        description="IMDb dataset, ELECTRA model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/dRM6RKSwD5fKteG/download",
-        **_IMDB_ELECTRA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="imdb-roberta-lgxa",
-        description="IMDb dataset, RoBERTa model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/oWCkBFgsstPakKS/download",
-        **_IMDB_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-roberta-lig",
-        description="IMDb dataset, RoBERTa model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/qJBYkfwppGZ4NF5/download",
-        **_IMDB_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-roberta-lime",
-        description="IMDb dataset, RoBERTa model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/rpsMTw3S6JkQgcF/download",
-        **_IMDB_ROBERTA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="imdb-roberta-lime-100",
-        description="IMDb dataset, RoBERTa model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/YZsAoJmR4EcwnG2/download",
-        **_IMDB_ROBERTA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="imdb-roberta-occ",
-        description="IMDb dataset, RoBERTa model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/wDw9k7PRWwsfQPB/download",
-        **_IMDB_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-roberta-svs",
-        description="IMDb dataset, RoBERTa model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/339zLEttF6djtBR/download",
-        **_IMDB_ROBERTA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="imdb-roberta-lds",
-        description="IMDb dataset, RoBERTa model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/EzD7brEosFx4iW2/download",
-        **_IMDB_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-roberta-lgs",
-        description="IMDb dataset, RoBERTa model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/ptcfks7sTnpm85M/download",
-        **_IMDB_ROBERTA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="imdb-xlnet-lgxa",
-        description="IMDb dataset, XLNet model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/53g8Gw28BX9eiPQ/download",
-        **_IMDB_XLNET_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-xlnet-lig",
-        description="IMDb dataset, XLNet model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/sgn79wJgTWjoNjq/download",
-        **_IMDB_XLNET_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-xlnet-lime",
-        description="IMDb dataset, XLNet model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/YCDW67f49wj5NXg/download",
-        **_IMDB_XLNET_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="imdb-xlnet-lime-100",
-        description="IMDb dataset, XLNet model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/T2KsA8ragxPz6eL/download",
-        **_IMDB_XLNET_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="imdb-xlnet-occ",
-        description="IMDb dataset, XLNet model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/H46msX6FQfFrCpg/download",
-        **_IMDB_XLNET_KWARGS,
-    ),
-    ThermostatConfig(
-        name="imdb-xlnet-svs",
-        description="IMDb dataset, XLNet model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/y9grFyRQC2rDSaN/download",
-        **_IMDB_XLNET_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-albert-lgxa",
-        description="MultiNLI dataset, ALBERT model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/nkRmprdnbb5C4Tx/download",
-        **_MNLI_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-albert-lig",
-        description="MultiNLI dataset, ALBERT model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/3WAqbXa2DG2RCgz/download",
-        **_MNLI_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-albert-lime",
-        description="MultiNLI dataset, ALBERT model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/e6JRy9fidSAC5zK/download",
-        **_MNLI_ALBERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="multi_nli-albert-lime-100",
-        description="MultiNLI dataset, ALBERT model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/WB2N3nFkHTGkXY8/download",
-        **_MNLI_ALBERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="multi_nli-albert-occ",
-        description="MultiNLI dataset, ALBERT model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/F5xWYpyDpwaAPJs/download",
-        **_MNLI_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-albert-svs",
-        description="MultiNLI dataset, ALBERT model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/fffM7w64CnTSzHA/download",
-        **_MNLI_ALBERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="multi_nli-albert-lds",
-        description="MultiNLI dataset, ALBERT model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/LiMzjexGXc5PdAm/download",
-        **_MNLI_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-albert-lgs",
-        description="MultiNLI dataset, ALBERT model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/ZL9fN8QKy8Di58B/download",
-        **_MNLI_ALBERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="multi_nli-bert-lgxa",
-        description="MultiNLI dataset, BERT model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/MdjebgkdexA2ZDt/download",
-        **_MNLI_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-bert-lig",
-        description="MultiNLI dataset, BERT model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/g53nbtnXaFyPLM7/download",
-        **_MNLI_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-bert-lime",
-        description="MultiNLI dataset, BERT model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/ptspBexoHaXtqXD/download",
-        **_MNLI_BERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="multi_nli-bert-lime-100",
-        description="MultiNLI dataset, BERT model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/LjFccwQ2mCAnsmH/download",
-        **_MNLI_BERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="multi_nli-bert-occ",
-        description="MultiNLI dataset, BERT model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/cHK6YCAo4ESZ3xx/download",
-        **_MNLI_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-bert-svs",
-        description="MultiNLI dataset, BERT model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/d5TTHCkAb5TJmbg/download",
-        **_MNLI_BERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="multi_nli-bert-lds",
-        description="MultiNLI dataset, BERT model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/yBtF9ybEm5kCzeg/download",
-        **_MNLI_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-bert-lgs",
-        description="MultiNLI dataset, BERT model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/XMAgeYenwS7MSWP/download",
-        **_MNLI_BERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="multi_nli-electra-lgxa",
-        description="MultiNLI dataset, ELECTRA model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/2HrCmp9sxJNiKBc/download",
-        **_MNLI_ELECTRA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-electra-lig",
-        description="MultiNLI dataset, ELECTRA model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/2eZnJgCbWd2D4PB/download",
-        **_MNLI_ELECTRA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-electra-lime",
-        description="MultiNLI dataset, ELECTRA model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/WzBwpwC9FoQZCwB/download",
-        **_MNLI_ELECTRA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="multi_nli-electra-lime-100",
-        description="MultiNLI dataset, ELECTRA model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/TX6jWs9wBdsJA9w/download",
-        **_MNLI_ELECTRA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="multi_nli-electra-occ",
-        description="MultiNLI dataset, ELECTRA model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/MGjQmKK9kynZTQt/download",
-        **_MNLI_ELECTRA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-electra-svs",
-        description="MultiNLI dataset, ELECTRA model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/zx3rGTpMkRT68tk/download",
-        **_MNLI_ELECTRA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="multi_nli-electra-lds",
-        description="MultiNLI dataset, ELECTRA model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/PD578t8fzsR2Q6k/download",
-        **_MNLI_ELECTRA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-electra-lgs",
-        description="MultiNLI dataset, ELECTRA model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/iq2QNQRojpsoKwW/download",
-        **_MNLI_ELECTRA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="multi_nli-roberta-lgxa",
-        description="MultiNLI dataset, RoBERTa model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/SxDwtGCpPzi3DDz/download",
-        **_MNLI_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-roberta-lig",
-        description="MultiNLI dataset, RoBERTa model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/8zaTxTCijG6g7Y5/download",
-        **_MNLI_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-roberta-lime",
-        description="MultiNLI dataset, RoBERTa model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/dY4z4ptcMtiYzZs/download",
-        **_MNLI_ROBERTA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="multi_nli-roberta-lime-100",
-        description="MultiNLI dataset, RoBERTa model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/KTQWmCDX2EjHtQE/download",
-        **_MNLI_ROBERTA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="multi_nli-roberta-occ",
-        description="MultiNLI dataset, RoBERTa model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/w5YSxNc6L8QZisG/download",
-        **_MNLI_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-roberta-svs",
-        description="MultiNLI dataset, RoBERTa model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/3aPeTawM8cbAsEg/download",
-        **_MNLI_ROBERTA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="multi_nli-roberta-lds",
-        description="MultiNLI dataset, RoBERTa model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/Kg4eLx2SZWrf8MF/download",
-        **_MNLI_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-roberta-lgs",
-        description="MultiNLI dataset, RoBERTa model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/7Fxtawd3t8WXTWC/download",
-        **_MNLI_ROBERTA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="multi_nli-xlnet-lgxa",
-        description="MultiNLI dataset, XLNet model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/n79G9kf9jbNx8o7/download",
-        **_MNLI_XLNET_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-xlnet-lig",
-        description="MultiNLI dataset, XLNet model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/MZr8jTnaCBdMPGe/download",
-        **_MNLI_XLNET_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-xlnet-lime",
-        description="MultiNLI dataset, XLNet model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/B7tfLSRKBGYxJ3s/download",
-        **_MNLI_XLNET_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="multi_nli-xlnet-lime-100",
-        description="MultiNLI dataset, XLNet model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/SesZACA2AwyefFp/download",
-        **_MNLI_XLNET_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="multi_nli-xlnet-occ",
-        description="MultiNLI dataset, XLNet model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/YWjJ6T7n6oeKbJJ/download",
-        **_MNLI_XLNET_KWARGS,
-    ),
-    ThermostatConfig(
-        name="multi_nli-xlnet-svs",
-        description="MultiNLI dataset, XLNet model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/CXYRFGsR2NFeAZa/download",
-        **_MNLI_XLNET_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-albert-lgxa",
-        description="XNLI dataset, ALBERT model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/zCSq69Z853fs3ez/download",
-        **_XNLI_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-albert-lig",
-        description="XNLI dataset, ALBERT model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/ZcP34Eg6eb3TrWF/download",
-        **_XNLI_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-albert-lime",
-        description="XNLI dataset, ALBERT model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/sijLW3ceigxDsKY/download",
-        **_XNLI_ALBERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="xnli-albert-lime-100",
-        description="XNLI dataset, ALBERT model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/oQW5cRc6GbqHtB6/download",
-        **_XNLI_ALBERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="xnli-albert-occ",
-        description="XNLI dataset, ALBERT model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/bEg95CGBtzaFQij/download",
-        **_XNLI_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-albert-svs",
-        description="XNLI dataset, ALBERT model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/wekiPq7ijzsCQK4/download",
-        **_XNLI_ALBERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="xnli-albert-lds",
-        description="XNLI dataset, ALBERT model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/AzKmCQfEP6CmwTH/download",
-        **_XNLI_ALBERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-albert-lgs",
-        description="XNLI dataset, ALBERT model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/qWdK5YkSBxmMPKp/download",
-        **_XNLI_ALBERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="xnli-bert-lgxa",
-        description="XNLI dataset, BERT model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/pb3Q6GQodyMqkgJ/download",
-        **_XNLI_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-bert-lig",
-        description="XNLI dataset, BERT model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/MX8YkzjFtpd43PM/download",
-        **_XNLI_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-bert-lime",
-        description="XNLI dataset, BERT model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/KfjqkRTd7FSWSkx/download",
-        **_XNLI_BERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="xnli-bert-lime-100",
-        description="XNLI dataset, BERT model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/FXHt989a2En8aZZ/download",
-        **_XNLI_BERT_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="xnli-bert-occ",
-        description="XNLI dataset, BERT model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/AHoTKbtSCQ73QxN/download",
-        **_XNLI_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-bert-svs",
-        description="XNLI dataset, BERT model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/D4ctEijzerMoNT8/download",
-        **_XNLI_BERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="xnli-bert-lds",
-        description="XNLI dataset, BERT model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/LtARP8wA4mLCcL2/download",
-        **_XNLI_BERT_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-bert-lgs",
-        description="XNLI dataset, BERT model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/AHw6WdfNbYXP9zD/download",
-        **_XNLI_BERT_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="xnli-electra-lgxa",
-        description="XNLI dataset, ELECTRA model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/t4ge7pA57gy4dKr/download",
-        **_XNLI_ELECTRA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-electra-lig",
-        description="XNLI dataset, ELECTRA model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/fHBSRQoAXzo3EKj/download",
-        **_XNLI_ELECTRA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-electra-lime",
-        description="XNLI dataset, ELECTRA model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/XnkiHXgxNsptxTJ/download",
-        **_XNLI_ELECTRA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="xnli-electra-lime-100",
-        description="XNLI dataset, ELECTRA model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/7zNtxCHxEZk2tzC/download",
-        **_XNLI_ELECTRA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="xnli-electra-occ",
-        description="XNLI dataset, ELECTRA model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/2RtRaN8q5fDHWyF/download",
-        **_XNLI_ELECTRA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-electra-svs",
-        description="XNLI dataset, ELECTRA model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/T3KKsM5TtsHyCAL/download",
-        **_XNLI_ELECTRA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="xnli-electra-lds",
-        description="XNLI dataset, ELECTRA model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/MmHwGXa6EpzT3ns/download",
-        **_XNLI_ELECTRA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-electra-lgs",
-        description="XNLI dataset, ELECTRA model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/gLwPwAaJDCB956T/download",
-        **_XNLI_ELECTRA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="xnli-roberta-lgxa",
-        description="XNLI dataset, RoBERTa model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/aPoCzcXDCfya3Ww/download",
-        **_XNLI_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-roberta-lig",
-        description="XNLI dataset, RoBERTa model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/iPA6rCfjc49ofpN/download",
-        **_XNLI_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-roberta-lime",
-        description="XNLI dataset, RoBERTa model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/pZKo7m4g9WJXfoe/download",
-        **_XNLI_ROBERTA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="xnli-roberta-lime-100",
-        description="XNLI dataset, RoBERTa model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/CHSR7Arw8M56bxN/download",
-        **_XNLI_ROBERTA_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="xnli-roberta-occ",
-        description="XNLI dataset, RoBERTa model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/XB2tnATQW3tbxPW/download",
-        **_XNLI_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-roberta-svs",
-        description="XNLI dataset, RoBERTa model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/opYTzjSeWWL7eYg/download",
-        **_XNLI_ROBERTA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="xnli-roberta-lds",
-        description="XNLI dataset, RoBERTa model, Layer DeepLift Shap explanations",
-        explainer="LayerDeepLiftShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/zsrrBirPHY4gp2p/download",
-        **_XNLI_ROBERTA_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-roberta-lgs",
-        description="XNLI dataset, RoBERTa model, Layer Gradient Shap explanations",
-        explainer="LayerGradientShap",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/fxAMzqGzgBZb9b4/download",
-        **_XNLI_ROBERTA_KWARGS,
-    ),
-    # shap value inclusion
-    ThermostatConfig(
-        name="xnli-xlnet-lgxa",
-        description="XNLI dataset, XLNet model, Layer Gradient x Activation explanations",
-        explainer="LayerGradientXActivation",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/jBXEkQS7WTz3a7J/download",
-        **_XNLI_XLNET_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-xlnet-lig",
-        description="XNLI dataset, XLNet model, Layer Integrated Gradients explanations",
-        explainer="LayerIntegratedGradients",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/kx7cJYFbyCjy58z/download",
-        **_XNLI_XLNET_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-xlnet-lime",
-        description="XNLI dataset, XLNet model, LIME explanations",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/6s4DFPNYpzi8722/download",
-        **_XNLI_XLNET_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="xnli-xlnet-lime-100",
-        description="XNLI dataset, XLNet model, LIME explanations, 100 samples",
-        explainer="LimeBase",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/ZzN9PSkiRrJNza2/download",
-        **_XNLI_XLNET_KWARGS,
-    ),
-    # new change
-    ThermostatConfig(
-        name="xnli-xlnet-occ",
-        description="XNLI dataset, XLNet model, Occlusion explanations",
-        explainer="Occlusion",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/yEFEyrq4pbGKP4s/download",
-        **_XNLI_XLNET_KWARGS,
-    ),
-    ThermostatConfig(
-        name="xnli-xlnet-svs",
-        description="XNLI dataset, XLNet model, Shapley Value Sampling explanations",
-        explainer="ShapleyValueSampling",
-        data_url="https://cloud.dfki.de/owncloud/index.php/s/fT34Q7CD2GQkdxJ/download",
-        **_XNLI_XLNET_KWARGS,
-    ),
-]
+import datasets
+
+
+_VERSION = datasets.Version('1.0.2', '')
+
+
+# Base arguments for any dataset
+_BASE_KWARGS = dict(
+    features={
+        "attributions": "attributions",
+        "predictions": "predictions",
+        "input_ids": "input_ids",
+    },
+    citation="Coming soon.",
+    url="https://github.com/DFKI-NLP/",
+)
+
+
+# Base arguments for AG News dataset
+_AGNEWS_KWARGS = dict(
+    dataset="ag_news",
+    label_classes=["World", "Sports", "Business", "Sci/Tech"],
+    label_column="label",
+    text_column="text",
+    **_BASE_KWARGS,
+)
+_AGNEWS_ALBERT_KWARGS = dict(
+    model="textattack/albert-base-v2-ag-news",
+    **_AGNEWS_KWARGS,
+)
+_AGNEWS_BERT_KWARGS = dict(
+    model="textattack/bert-base-uncased-ag-news",
+    **_AGNEWS_KWARGS,
+)
+_AGNEWS_ROBERTA_KWARGS = dict(
+    model="textattack/roberta-base-ag-news",
+    **_AGNEWS_KWARGS,
+)
+
+# Base arguments for IMDb dataset
+_IMDB_KWARGS = dict(
+    dataset="imdb",
+    label_classes=["neg", "pos"],
+    label_column="label",
+    text_column="text",
+    **_BASE_KWARGS,
+)
+_IMDB_ALBERT_KWARGS = dict(
+    model="textattack/albert-base-v2-imdb",
+    **_IMDB_KWARGS,
+)
+_IMDB_BERT_KWARGS = dict(
+    model="textattack/bert-base-uncased-imdb",
+    **_IMDB_KWARGS,
+)
+_IMDB_ELECTRA_KWARGS = dict(
+    model="monologg/electra-small-finetuned-imdb",
+    **_IMDB_KWARGS,
+)
+_IMDB_ROBERTA_KWARGS = dict(
+    model="textattack/roberta-base-imdb",
+    **_IMDB_KWARGS,
+)
+_IMDB_XLNET_KWARGS = dict(
+    model="textattack/xlnet-base-cased-imdb",
+    **_IMDB_KWARGS,
+)
+
+# Base arguments for MNLI dataset
+_MNLI_KWARGS = dict(
+    dataset="multi_nli",
+    label_column="label",
+    label_classes=["entailment", "neutral", "contradiction"],
+    text_column=["premise", "hypothesis"],
+    **_BASE_KWARGS,
+)
+_MNLI_ALBERT_KWARGS = dict(
+    model="prajjwal1/albert-base-v2-mnli",
+    **_MNLI_KWARGS,
+)
+_MNLI_BERT_KWARGS = dict(
+    model="textattack/bert-base-uncased-MNLI",
+    **_MNLI_KWARGS,
+)
+_MNLI_ELECTRA_KWARGS = dict(
+    model="howey/electra-base-mnli",
+    **_MNLI_KWARGS,
+)
+_MNLI_ROBERTA_KWARGS = dict(
+    model="textattack/roberta-base-MNLI",
+    **_MNLI_KWARGS,
+)
+_MNLI_XLNET_KWARGS = dict(
+    model="textattack/xlnet-base-cased-MNLI",
+    **_MNLI_KWARGS,
+)
+
+# Base arguments for XNLI dataset
+_XNLI_KWARGS = dict(
+    dataset="xnli",
+    label_column="label",
+    label_classes=["entailment", "neutral", "contradiction"],
+    text_column=["premise", "hypothesis"],
+    **_BASE_KWARGS,
+)
+_XNLI_ALBERT_KWARGS = dict(
+    model="prajjwal1/albert-base-v2-mnli",
+    **_XNLI_KWARGS,
+)
+_XNLI_BERT_KWARGS = dict(
+    model="textattack/bert-base-uncased-MNLI",
+    **_XNLI_KWARGS,
+)
+_XNLI_ELECTRA_KWARGS = dict(
+    model="howey/electra-base-mnli",
+    **_XNLI_KWARGS,
+)
+_XNLI_ROBERTA_KWARGS = dict(
+    model="textattack/roberta-base-MNLI",
+    **_XNLI_KWARGS,
+)
+_XNLI_XLNET_KWARGS = dict(
+    model="textattack/xlnet-base-cased-MNLI",
+    **_XNLI_KWARGS,
+)
+
+
+class ThermostatConfig(datasets.BuilderConfig):
+    """ BuilderConfig for Thermostat """
+
+    def __init__(
+        self,
+        explainer,
+        model,
+        dataset,
+        features,
+        label_column,
+        label_classes,
+        text_column,
+        data_url,
+        citation,
+        url,
+        **kwargs,
+    ):
+        super(ThermostatConfig, self).__init__(version=_VERSION, **kwargs)
+        self.explainer = explainer
+        self.model = model
+        self.dataset = dataset
+        self.features = features
+        self.label_column = label_column
+        self.label_classes = label_classes
+        self.text_column = text_column
+        self.data_url = data_url
+        self.citation = citation
+        self.url = url
+
+
+builder_configs = [
+    ThermostatConfig(
+        name="ag_news-albert-lgxa",
+        description="AG News dataset, ALBERT model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/8XPC557ePpWCBQY/download",
+        **_AGNEWS_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="ag_news-albert-lig",
+        description="AG News dataset, ALBERT model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/zS7mcMsdAp5ZENX/download",
+        **_AGNEWS_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="ag_news-albert-lime",
+        description="AG News dataset, ALBERT model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/8SLyHdDgRk2pXSL/download",
+        **_AGNEWS_ALBERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="ag_news-albert-lime-100",
+        description="AG News dataset, ALBERT model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/W3GT4ZDT2BzR5mj/download",
+        **_AGNEWS_ALBERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="ag_news-albert-occlusion",
+        description="AG News dataset, ALBERT model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/Li9HwfKfFqjCQTM/download",
+        **_AGNEWS_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="ag_news-albert-svs",
+        description="AG News dataset, ALBERT model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/GLppwQjeBTsLtTC/download",
+        **_AGNEWS_ALBERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="ag_news-albert-lds",
+        description="AG News dataset, ALBERT model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/nzriaZHxniNtJBN/download",
+        **_AGNEWS_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="ag_news-albert-lgs",
+        description="AG News dataset, ALBERT model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/EjCXxWCETQH9onj/download",
+        **_AGNEWS_ALBERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="ag_news-bert-lgxa",
+        description="AG News dataset, BERT model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/zn5mKsryyrX3e58/download",
+        **_AGNEWS_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="ag_news-bert-lig",
+        description="AG News dataset, BERT model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/Qq3dR7sHsfX9JXZ/download",
+        **_AGNEWS_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="ag_news-bert-lime",
+        description="AG News dataset, BERT model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/rW8MJyAjBGQxsK9/download",
+        **_AGNEWS_BERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="ag_news-bert-lime-100",
+        description="AG News dataset, BERT model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/FkSdXZPpN78HSHR/download",
+        **_AGNEWS_BERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="ag_news-bert-occlusion",
+        description="AG News dataset, BERT model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/Grf97s6bJwoZGyx/download",
+        **_AGNEWS_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="ag_news-bert-svs",
+        description="AG News dataset, BERT model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/dCbgsjdW6b9pzo3/download",
+        **_AGNEWS_BERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="ag_news-bert-lds",
+        description="AG News dataset, BERT model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/XQzBnRniEyC8NEF/download",
+        **_AGNEWS_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="ag_news-bert-lgs",
+        description="AG News dataset, BERT model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/nHt4Ld4AKfbG2ft/download",
+        **_AGNEWS_BERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="ag_news-roberta-lgxa",
+        description="AG News dataset, RoBERTa model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/Kz9GrYrMZB4gp7E/download",
+        **_AGNEWS_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="ag_news-roberta-lig",
+        description="AG News dataset, RoBERTa model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/mpH8sT6tXDoG5qi/download",
+        **_AGNEWS_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="ag_news-roberta-lime",
+        description="AG News dataset, RoBERTa model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/qRgBtwfjaXceJoL/download",
+        **_AGNEWS_ROBERTA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="ag_news-roberta-lime-100",
+        description="AG News dataset, RoBERTa model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/kFyjX2LqBdcW9bp/download",
+        **_AGNEWS_ROBERTA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="ag_news-roberta-occlusion",
+        description="AG News dataset, RoBERTa model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/78aZttqxKQNdW6J/download",
+        **_AGNEWS_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="ag_news-roberta-svs",
+        description="AG News dataset, RoBERTa model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/yabEAY5sLpjxKkW/download",
+        **_AGNEWS_ROBERTA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="ag_news-roberta-lds",
+        description="AG News dataset, RoBERTa model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/ZWoxq27s36For98/download",
+        **_AGNEWS_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="ag_news-roberta-lgs",
+        description="AG News dataset, RoBERTa model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/HgHjNFcMQbCC2Nb/download",
+        **_AGNEWS_ROBERTA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="imdb-albert-lgxa",
+        description="IMDb dataset, ALBERT model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/srbYBbmKBsGMXWn/download",
+        **_IMDB_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-albert-lig",
+        description="IMDb dataset, ALBERT model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/zjMddcqewEcwSPG/download",
+        **_IMDB_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-albert-lime",
+        description="IMDb dataset, ALBERT model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/Tgktb4fq4EdXJNx/download",
+        **_IMDB_ALBERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="imdb-albert-lime-100",
+        description="IMDb dataset, ALBERT model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/FzErcT9TcFcG2Pr/download",
+        **_IMDB_ALBERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="imdb-albert-occ",
+        description="IMDb dataset, ALBERT model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/98XqEgbZt9KiSfm/download",
+        **_IMDB_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-albert-svs",
+        description="IMDb dataset, ALBERT model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/sQMK2XsknbzK23a/download",
+        **_IMDB_ALBERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="imdb-albert-lds",
+        description="IMDb dataset, ALBERT model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/SYg2GjRkewW8fn7/download",
+        **_IMDB_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-albert-lgs",
+        description="IMDb dataset, ALBERT model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/rWZfSzPN7Gm3Cko/download",
+        **_IMDB_ALBERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="imdb-bert-lgxa",
+        description="IMDb dataset, BERT model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/NkPpnyMN8rdWE7L/download",
+        **_IMDB_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-bert-lig",
+        description="IMDb dataset, BERT model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/SdrPeJQQSExFQ8e/download",
+        **_IMDB_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-bert-lime",
+        description="IMDb dataset, BERT model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/ZQEdEmFtKeGkYWp/download",
+        **_IMDB_BERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="imdb-bert-lime-100",
+        description="IMDb dataset, BERT model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/Qx7z8SFcMTB5bFa/download",
+        **_IMDB_BERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="imdb-bert-occ",
+        description="IMDb dataset, BERT model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/PjMDBzaoHHqs2WF/download",
+        **_IMDB_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-bert-svs",
+        description="IMDb dataset, BERT model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/DjmCKdBoWHt8jbX/download",
+        **_IMDB_BERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="imdb-bert-lds",
+        description="IMDb dataset, BERT model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/dnqSfrgGPYcYsKt/download",
+        **_IMDB_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-bert-lgs",
+        description="IMDb dataset, BERT model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/fnBqKxEjfsScqwg/download",
+        **_IMDB_BERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="imdb-electra-lgxa",
+        description="IMDb dataset, ELECTRA model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/WdLYpQerXC5KrHK/download",
+        **_IMDB_ELECTRA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-electra-lig",
+        description="IMDb dataset, ELECTRA model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/e3Mibf9dqRfobYw/download",
+        **_IMDB_ELECTRA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-electra-lime",
+        description="IMDb dataset, ELECTRA model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/7p2576kFqiQLL9x/download",
+        **_IMDB_ELECTRA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="imdb-electra-lime-100",
+        description="IMDb dataset, ELECTRA model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/LBqzn6JiQNzwMAC/download",
+        **_IMDB_ELECTRA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="imdb-electra-occ",
+        description="IMDb dataset, ELECTRA model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/TZYTgnySrEbm5Xx/download",
+        **_IMDB_ELECTRA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-electra-svs",
+        description="IMDb dataset, ELECTRA model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/MPHqZwJCP97sA4D/download",
+        **_IMDB_ELECTRA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="imdb-electra-lds",
+        description="IMDb dataset, ELECTRA model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/cHdECMFjHacAnFk/download",
+        **_IMDB_ELECTRA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-electra-lgs",
+        description="IMDb dataset, ELECTRA model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/dRM6RKSwD5fKteG/download",
+        **_IMDB_ELECTRA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="imdb-roberta-lgxa",
+        description="IMDb dataset, RoBERTa model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/oWCkBFgsstPakKS/download",
+        **_IMDB_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-roberta-lig",
+        description="IMDb dataset, RoBERTa model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/qJBYkfwppGZ4NF5/download",
+        **_IMDB_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-roberta-lime",
+        description="IMDb dataset, RoBERTa model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/rpsMTw3S6JkQgcF/download",
+        **_IMDB_ROBERTA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="imdb-roberta-lime-100",
+        description="IMDb dataset, RoBERTa model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/YZsAoJmR4EcwnG2/download",
+        **_IMDB_ROBERTA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="imdb-roberta-occ",
+        description="IMDb dataset, RoBERTa model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/wDw9k7PRWwsfQPB/download",
+        **_IMDB_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-roberta-svs",
+        description="IMDb dataset, RoBERTa model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/339zLEttF6djtBR/download",
+        **_IMDB_ROBERTA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="imdb-roberta-lds",
+        description="IMDb dataset, RoBERTa model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/EzD7brEosFx4iW2/download",
+        **_IMDB_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-roberta-lgs",
+        description="IMDb dataset, RoBERTa model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/ptcfks7sTnpm85M/download",
+        **_IMDB_ROBERTA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="imdb-xlnet-lgxa",
+        description="IMDb dataset, XLNet model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/53g8Gw28BX9eiPQ/download",
+        **_IMDB_XLNET_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-xlnet-lig",
+        description="IMDb dataset, XLNet model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/sgn79wJgTWjoNjq/download",
+        **_IMDB_XLNET_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-xlnet-lime",
+        description="IMDb dataset, XLNet model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/YCDW67f49wj5NXg/download",
+        **_IMDB_XLNET_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="imdb-xlnet-lime-100",
+        description="IMDb dataset, XLNet model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/T2KsA8ragxPz6eL/download",
+        **_IMDB_XLNET_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="imdb-xlnet-occ",
+        description="IMDb dataset, XLNet model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/H46msX6FQfFrCpg/download",
+        **_IMDB_XLNET_KWARGS,
+    ),
+    ThermostatConfig(
+        name="imdb-xlnet-svs",
+        description="IMDb dataset, XLNet model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/y9grFyRQC2rDSaN/download",
+        **_IMDB_XLNET_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-albert-lgxa",
+        description="MultiNLI dataset, ALBERT model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/nkRmprdnbb5C4Tx/download",
+        **_MNLI_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-albert-lig",
+        description="MultiNLI dataset, ALBERT model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/3WAqbXa2DG2RCgz/download",
+        **_MNLI_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-albert-lime",
+        description="MultiNLI dataset, ALBERT model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/e6JRy9fidSAC5zK/download",
+        **_MNLI_ALBERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="multi_nli-albert-lime-100",
+        description="MultiNLI dataset, ALBERT model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/WB2N3nFkHTGkXY8/download",
+        **_MNLI_ALBERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="multi_nli-albert-occ",
+        description="MultiNLI dataset, ALBERT model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/F5xWYpyDpwaAPJs/download",
+        **_MNLI_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-albert-svs",
+        description="MultiNLI dataset, ALBERT model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/fffM7w64CnTSzHA/download",
+        **_MNLI_ALBERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="multi_nli-albert-lds",
+        description="MultiNLI dataset, ALBERT model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/LiMzjexGXc5PdAm/download",
+        **_MNLI_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-albert-lgs",
+        description="MultiNLI dataset, ALBERT model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/ZL9fN8QKy8Di58B/download",
+        **_MNLI_ALBERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="multi_nli-bert-lgxa",
+        description="MultiNLI dataset, BERT model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/MdjebgkdexA2ZDt/download",
+        **_MNLI_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-bert-lig",
+        description="MultiNLI dataset, BERT model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/g53nbtnXaFyPLM7/download",
+        **_MNLI_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-bert-lime",
+        description="MultiNLI dataset, BERT model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/ptspBexoHaXtqXD/download",
+        **_MNLI_BERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="multi_nli-bert-lime-100",
+        description="MultiNLI dataset, BERT model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/LjFccwQ2mCAnsmH/download",
+        **_MNLI_BERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="multi_nli-bert-occ",
+        description="MultiNLI dataset, BERT model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/cHK6YCAo4ESZ3xx/download",
+        **_MNLI_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-bert-svs",
+        description="MultiNLI dataset, BERT model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/d5TTHCkAb5TJmbg/download",
+        **_MNLI_BERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="multi_nli-bert-lds",
+        description="MultiNLI dataset, BERT model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/yBtF9ybEm5kCzeg/download",
+        **_MNLI_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-bert-lgs",
+        description="MultiNLI dataset, BERT model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/XMAgeYenwS7MSWP/download",
+        **_MNLI_BERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="multi_nli-electra-lgxa",
+        description="MultiNLI dataset, ELECTRA model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/2HrCmp9sxJNiKBc/download",
+        **_MNLI_ELECTRA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-electra-lig",
+        description="MultiNLI dataset, ELECTRA model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/2eZnJgCbWd2D4PB/download",
+        **_MNLI_ELECTRA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-electra-lime",
+        description="MultiNLI dataset, ELECTRA model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/WzBwpwC9FoQZCwB/download",
+        **_MNLI_ELECTRA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="multi_nli-electra-lime-100",
+        description="MultiNLI dataset, ELECTRA model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/TX6jWs9wBdsJA9w/download",
+        **_MNLI_ELECTRA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="multi_nli-electra-occ",
+        description="MultiNLI dataset, ELECTRA model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/MGjQmKK9kynZTQt/download",
+        **_MNLI_ELECTRA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-electra-svs",
+        description="MultiNLI dataset, ELECTRA model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/zx3rGTpMkRT68tk/download",
+        **_MNLI_ELECTRA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="multi_nli-electra-lds",
+        description="MultiNLI dataset, ELECTRA model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/PD578t8fzsR2Q6k/download",
+        **_MNLI_ELECTRA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-electra-lgs",
+        description="MultiNLI dataset, ELECTRA model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/iq2QNQRojpsoKwW/download",
+        **_MNLI_ELECTRA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="multi_nli-roberta-lgxa",
+        description="MultiNLI dataset, RoBERTa model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/SxDwtGCpPzi3DDz/download",
+        **_MNLI_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-roberta-lig",
+        description="MultiNLI dataset, RoBERTa model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/8zaTxTCijG6g7Y5/download",
+        **_MNLI_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-roberta-lime",
+        description="MultiNLI dataset, RoBERTa model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/dY4z4ptcMtiYzZs/download",
+        **_MNLI_ROBERTA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="multi_nli-roberta-lime-100",
+        description="MultiNLI dataset, RoBERTa model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/KTQWmCDX2EjHtQE/download",
+        **_MNLI_ROBERTA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="multi_nli-roberta-occ",
+        description="MultiNLI dataset, RoBERTa model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/w5YSxNc6L8QZisG/download",
+        **_MNLI_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-roberta-svs",
+        description="MultiNLI dataset, RoBERTa model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/3aPeTawM8cbAsEg/download",
+        **_MNLI_ROBERTA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="multi_nli-roberta-lds",
+        description="MultiNLI dataset, RoBERTa model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/Kg4eLx2SZWrf8MF/download",
+        **_MNLI_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-roberta-lgs",
+        description="MultiNLI dataset, RoBERTa model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/7Fxtawd3t8WXTWC/download",
+        **_MNLI_ROBERTA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="multi_nli-xlnet-lgxa",
+        description="MultiNLI dataset, XLNet model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/n79G9kf9jbNx8o7/download",
+        **_MNLI_XLNET_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-xlnet-lig",
+        description="MultiNLI dataset, XLNet model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/MZr8jTnaCBdMPGe/download",
+        **_MNLI_XLNET_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-xlnet-lime",
+        description="MultiNLI dataset, XLNet model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/B7tfLSRKBGYxJ3s/download",
+        **_MNLI_XLNET_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="multi_nli-xlnet-lime-100",
+        description="MultiNLI dataset, XLNet model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/SesZACA2AwyefFp/download",
+        **_MNLI_XLNET_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="multi_nli-xlnet-occ",
+        description="MultiNLI dataset, XLNet model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/YWjJ6T7n6oeKbJJ/download",
+        **_MNLI_XLNET_KWARGS,
+    ),
+    ThermostatConfig(
+        name="multi_nli-xlnet-svs",
+        description="MultiNLI dataset, XLNet model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/CXYRFGsR2NFeAZa/download",
+        **_MNLI_XLNET_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-albert-lgxa",
+        description="XNLI dataset, ALBERT model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/zCSq69Z853fs3ez/download",
+        **_XNLI_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-albert-lig",
+        description="XNLI dataset, ALBERT model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/ZcP34Eg6eb3TrWF/download",
+        **_XNLI_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-albert-lime",
+        description="XNLI dataset, ALBERT model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/sijLW3ceigxDsKY/download",
+        **_XNLI_ALBERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="xnli-albert-lime-100",
+        description="XNLI dataset, ALBERT model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/oQW5cRc6GbqHtB6/download",
+        **_XNLI_ALBERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="xnli-albert-occ",
+        description="XNLI dataset, ALBERT model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/bEg95CGBtzaFQij/download",
+        **_XNLI_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-albert-svs",
+        description="XNLI dataset, ALBERT model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/wekiPq7ijzsCQK4/download",
+        **_XNLI_ALBERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="xnli-albert-lds",
+        description="XNLI dataset, ALBERT model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/AzKmCQfEP6CmwTH/download",
+        **_XNLI_ALBERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-albert-lgs",
+        description="XNLI dataset, ALBERT model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/qWdK5YkSBxmMPKp/download",
+        **_XNLI_ALBERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="xnli-bert-lgxa",
+        description="XNLI dataset, BERT model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/pb3Q6GQodyMqkgJ/download",
+        **_XNLI_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-bert-lig",
+        description="XNLI dataset, BERT model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/MX8YkzjFtpd43PM/download",
+        **_XNLI_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-bert-lime",
+        description="XNLI dataset, BERT model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/KfjqkRTd7FSWSkx/download",
+        **_XNLI_BERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="xnli-bert-lime-100",
+        description="XNLI dataset, BERT model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/FXHt989a2En8aZZ/download",
+        **_XNLI_BERT_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="xnli-bert-occ",
+        description="XNLI dataset, BERT model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/AHoTKbtSCQ73QxN/download",
+        **_XNLI_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-bert-svs",
+        description="XNLI dataset, BERT model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/D4ctEijzerMoNT8/download",
+        **_XNLI_BERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="xnli-bert-lds",
+        description="XNLI dataset, BERT model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/LtARP8wA4mLCcL2/download",
+        **_XNLI_BERT_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-bert-lgs",
+        description="XNLI dataset, BERT model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/AHw6WdfNbYXP9zD/download",
+        **_XNLI_BERT_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="xnli-electra-lgxa",
+        description="XNLI dataset, ELECTRA model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/t4ge7pA57gy4dKr/download",
+        **_XNLI_ELECTRA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-electra-lig",
+        description="XNLI dataset, ELECTRA model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/fHBSRQoAXzo3EKj/download",
+        **_XNLI_ELECTRA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-electra-lime",
+        description="XNLI dataset, ELECTRA model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/XnkiHXgxNsptxTJ/download",
+        **_XNLI_ELECTRA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="xnli-electra-lime-100",
+        description="XNLI dataset, ELECTRA model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/7zNtxCHxEZk2tzC/download",
+        **_XNLI_ELECTRA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="xnli-electra-occ",
+        description="XNLI dataset, ELECTRA model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/2RtRaN8q5fDHWyF/download",
+        **_XNLI_ELECTRA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-electra-svs",
+        description="XNLI dataset, ELECTRA model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/T3KKsM5TtsHyCAL/download",
+        **_XNLI_ELECTRA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="xnli-electra-lds",
+        description="XNLI dataset, ELECTRA model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/MmHwGXa6EpzT3ns/download",
+        **_XNLI_ELECTRA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-electra-lgs",
+        description="XNLI dataset, ELECTRA model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/gLwPwAaJDCB956T/download",
+        **_XNLI_ELECTRA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="xnli-roberta-lgxa",
+        description="XNLI dataset, RoBERTa model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/aPoCzcXDCfya3Ww/download",
+        **_XNLI_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-roberta-lig",
+        description="XNLI dataset, RoBERTa model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/iPA6rCfjc49ofpN/download",
+        **_XNLI_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-roberta-lime",
+        description="XNLI dataset, RoBERTa model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/pZKo7m4g9WJXfoe/download",
+        **_XNLI_ROBERTA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="xnli-roberta-lime-100",
+        description="XNLI dataset, RoBERTa model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/CHSR7Arw8M56bxN/download",
+        **_XNLI_ROBERTA_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="xnli-roberta-occ",
+        description="XNLI dataset, RoBERTa model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/XB2tnATQW3tbxPW/download",
+        **_XNLI_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-roberta-svs",
+        description="XNLI dataset, RoBERTa model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/opYTzjSeWWL7eYg/download",
+        **_XNLI_ROBERTA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="xnli-roberta-lds",
+        description="XNLI dataset, RoBERTa model, Layer DeepLift Shap explanations",
+        explainer="LayerDeepLiftShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/zsrrBirPHY4gp2p/download",
+        **_XNLI_ROBERTA_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-roberta-lgs",
+        description="XNLI dataset, RoBERTa model, Layer Gradient Shap explanations",
+        explainer="LayerGradientShap",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/fxAMzqGzgBZb9b4/download",
+        **_XNLI_ROBERTA_KWARGS,
+    ),
+    # shap value inclusion
+    ThermostatConfig(
+        name="xnli-xlnet-lgxa",
+        description="XNLI dataset, XLNet model, Layer Gradient x Activation explanations",
+        explainer="LayerGradientXActivation",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/jBXEkQS7WTz3a7J/download",
+        **_XNLI_XLNET_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-xlnet-lig",
+        description="XNLI dataset, XLNet model, Layer Integrated Gradients explanations",
+        explainer="LayerIntegratedGradients",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/kx7cJYFbyCjy58z/download",
+        **_XNLI_XLNET_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-xlnet-lime",
+        description="XNLI dataset, XLNet model, LIME explanations",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/6s4DFPNYpzi8722/download",
+        **_XNLI_XLNET_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="xnli-xlnet-lime-100",
+        description="XNLI dataset, XLNet model, LIME explanations, 100 samples",
+        explainer="LimeBase",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/ZzN9PSkiRrJNza2/download",
+        **_XNLI_XLNET_KWARGS,
+    ),
+    # new change
+    ThermostatConfig(
+        name="xnli-xlnet-occ",
+        description="XNLI dataset, XLNet model, Occlusion explanations",
+        explainer="Occlusion",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/yEFEyrq4pbGKP4s/download",
+        **_XNLI_XLNET_KWARGS,
+    ),
+    ThermostatConfig(
+        name="xnli-xlnet-svs",
+        description="XNLI dataset, XLNet model, Shapley Value Sampling explanations",
+        explainer="ShapleyValueSampling",
+        data_url="https://cloud.dfki.de/owncloud/index.php/s/fT34Q7CD2GQkdxJ/download",
+        **_XNLI_XLNET_KWARGS,
+    ),
+]
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat/data/tokenization.py` & `thermostat-datasets-1.1.0/src/thermostat/data/tokenization.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from tokenizers import models
-from typing import List, Tuple
-
-
-def fuse_subwords(tokens_enum: List[Tuple], atts: List, tokenizer, strategy=None) -> (List, List):
-    assert strategy in ['average', 'salient']
-    tokenizer_model = tokenizer.backend_tokenizer.model
-
-    fuse_index, fuse_token, fuse_att = [], '', []
-    cleaned_tokens, cleaned_atts = [], []
-
-    def append_cleaned(fuse_i, fuse_t, fuse_a, replace=None):
-        """ Append to results, replace tokenizer artifacts if necessary """
-        if len(fuse_i) == 1:
-            fuse_i = fuse_i[0]
-        if replace:
-            fuse_t = fuse_t.replace(*replace)
-        cleaned_fuse_token = fuse_t
-        cleaned_tokens.append((fuse_i, cleaned_fuse_token))
-        cleaned_atts.append(apply_fuse_strategy(fuse_a, strategy))
-
-    if type(tokenizer_model) == models.Unigram:  # ALBERT, XLNet
-        for i, (token_enum, a) in enumerate(zip(tokens_enum, atts)):
-            tidx, token = token_enum
-            if len(fuse_att) > 0:
-                if token.startswith('▁') and token != '▁':
-                    append_cleaned(fuse_index, fuse_token, fuse_att, replace=['▁', ''])
-                    fuse_index, fuse_token, fuse_att = [], '', []  # Reset
-            fuse_index.append(tidx)
-            fuse_token += token
-            fuse_att.append(a)
-        if fuse_att:
-            append_cleaned(fuse_index, fuse_token, fuse_att, replace=['▁', ''])
-
-    elif type(tokenizer_model) == models.WordPiece:  # BERT, ELECTRA
-        for i, (token_enum, a) in enumerate(zip(tokens_enum, atts)):
-            tidx, token = token_enum
-            if token.startswith('##'):
-                fuse_index.append(tidx)
-                # Append all subsequent '##' subword tokens
-                fuse_token += token.replace('##', '')
-                fuse_att.append(a)
-                if i < len(tokens_enum) - 1:
-                    if not tokens_enum[i + 1][1].startswith('##'):
-                        append_cleaned(fuse_index, fuse_token, fuse_att)
-                        fuse_index, fuse_token, fuse_att = [], '', []  # Reset
-            else:
-                if i < len(tokens_enum) - 1:
-                    if tokens_enum[i + 1][1].startswith('##'):
-                        fuse_index.append(tidx)
-                        # Add the one word before the first '##' token
-                        fuse_token += token
-                        fuse_att.append(a)
-                        continue
-                # Append to results ("nothing happens" case)
-                append_cleaned([tidx], token, [a])
-        if fuse_att:
-            append_cleaned(fuse_index, fuse_token, fuse_att, replace=['##', ''])
-
-    elif type(tokenizer_model) == models.BPE:  # RoBERTa
-        for i, (token_enum, a) in enumerate(zip(tokens_enum, atts)):
-            tidx, token = token_enum
-            if len(fuse_att) > 0:
-                if token != 'Ġ':
-                    append_cleaned(fuse_index, fuse_token, fuse_att)
-                    fuse_index, fuse_token, fuse_att = [], '', []  # Reset
-            fuse_index.append(tidx)
-            fuse_token += token.replace('Ġ', '')
-            fuse_att.append(a)
-        if fuse_att:
-            append_cleaned(fuse_index, fuse_token, fuse_att, replace=['Ġ', ''])
-
-    else:
-        raise NotImplementedError('Not a valid backend tokenizer model (Unigram, WordPiece, BPE).')
-
-    tokens = cleaned_tokens
-    atts = cleaned_atts
-
-    return tokens, atts
-
-
-def apply_fuse_strategy(fuse_att, strategy):
-    if strategy == 'average':
-        return sum(fuse_att) / len(fuse_att)
-    elif strategy == 'salient':
-        return max(fuse_att, key=abs)
+from tokenizers import models
+from typing import List, Tuple
+
+
+def fuse_subwords(tokens_enum: List[Tuple], atts: List, tokenizer, strategy=None) -> (List, List):
+    assert strategy in ['average', 'salient']
+    tokenizer_model = tokenizer.backend_tokenizer.model
+
+    fuse_index, fuse_token, fuse_att = [], '', []
+    cleaned_tokens, cleaned_atts = [], []
+
+    def append_cleaned(fuse_i, fuse_t, fuse_a, replace=None):
+        """ Append to results, replace tokenizer artifacts if necessary """
+        if len(fuse_i) == 1:
+            fuse_i = fuse_i[0]
+        if replace:
+            fuse_t = fuse_t.replace(*replace)
+        cleaned_fuse_token = fuse_t
+        cleaned_tokens.append((fuse_i, cleaned_fuse_token))
+        cleaned_atts.append(apply_fuse_strategy(fuse_a, strategy))
+
+    if type(tokenizer_model) == models.Unigram:  # ALBERT, XLNet
+        for i, (token_enum, a) in enumerate(zip(tokens_enum, atts)):
+            tidx, token = token_enum
+            if len(fuse_att) > 0:
+                if token.startswith('▁') and token != '▁':
+                    append_cleaned(fuse_index, fuse_token, fuse_att, replace=['▁', ''])
+                    fuse_index, fuse_token, fuse_att = [], '', []  # Reset
+            fuse_index.append(tidx)
+            fuse_token += token
+            fuse_att.append(a)
+        if fuse_att:
+            append_cleaned(fuse_index, fuse_token, fuse_att, replace=['▁', ''])
+
+    elif type(tokenizer_model) == models.WordPiece:  # BERT, ELECTRA
+        for i, (token_enum, a) in enumerate(zip(tokens_enum, atts)):
+            tidx, token = token_enum
+            if token.startswith('##'):
+                fuse_index.append(tidx)
+                # Append all subsequent '##' subword tokens
+                fuse_token += token.replace('##', '')
+                fuse_att.append(a)
+                if i < len(tokens_enum) - 1:
+                    if not tokens_enum[i + 1][1].startswith('##'):
+                        append_cleaned(fuse_index, fuse_token, fuse_att)
+                        fuse_index, fuse_token, fuse_att = [], '', []  # Reset
+            else:
+                if i < len(tokens_enum) - 1:
+                    if tokens_enum[i + 1][1].startswith('##'):
+                        fuse_index.append(tidx)
+                        # Add the one word before the first '##' token
+                        fuse_token += token
+                        fuse_att.append(a)
+                        continue
+                # Append to results ("nothing happens" case)
+                append_cleaned([tidx], token, [a])
+        if fuse_att:
+            append_cleaned(fuse_index, fuse_token, fuse_att, replace=['##', ''])
+
+    elif type(tokenizer_model) == models.BPE:  # RoBERTa
+        for i, (token_enum, a) in enumerate(zip(tokens_enum, atts)):
+            tidx, token = token_enum
+            if len(fuse_att) > 0:
+                if token != 'Ġ':
+                    append_cleaned(fuse_index, fuse_token, fuse_att)
+                    fuse_index, fuse_token, fuse_att = [], '', []  # Reset
+            fuse_index.append(tidx)
+            fuse_token += token.replace('Ġ', '')
+            fuse_att.append(a)
+        if fuse_att:
+            append_cleaned(fuse_index, fuse_token, fuse_att, replace=['Ġ', ''])
+
+    else:
+        raise NotImplementedError('Not a valid backend tokenizer model (Unigram, WordPiece, BPE).')
+
+    tokens = cleaned_tokens
+    atts = cleaned_atts
+
+    return tokens, atts
+
+
+def apply_fuse_strategy(fuse_att, strategy):
+    if strategy == 'average':
+        return sum(fuse_att) / len(fuse_att)
+    elif strategy == 'salient':
+        return max(fuse_att, key=abs)
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat/dataset.py` & `thermostat-datasets-1.1.0/src/thermostat/dataset.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-# coding=utf-8
-# Copyright 2020 The HuggingFace Datasets Authors and the current dataset script contributor.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-
-import datasets
-import json
-
-from thermostat.data.thermostat_configs import builder_configs
-
-# Find for instance the citation on arxiv or on the dataset repo/website
-_CITATION = """\
-@misc{feldhus2021thermostat,
-      title={Thermostat: A Large Collection of NLP Model Explanations and Analysis Tools}, 
-      author={Nils Feldhus and Robert Schwarzenberg and Sebastian Möller},
-      year={2021},
-      eprint={2108.13961},
-      archivePrefix={arXiv},
-      primaryClass={cs.CL}
-}
-"""
-
-_DESCRIPTION = "Thermostat is a large collection of NLP model explanations and accompanying analysis tools."
-
-# Link to an official homepage for the dataset
-_HOMEPAGE = 'https://github.com/DFKI-NLP/thermostat'
-
-# Licence for the dataset
-_LICENSE = 'Apache 2.0'
-
-
-class Thermostat(datasets.GeneratorBasedBuilder):
-    """One config (e.g. 'imdb-bert-lgxa') contains the attribution scores of a Layer Gradient x Activation explainer
-    applied on the IMDb dataset that has been classified by a BERT downstream model. """
-
-    BUILDER_CONFIGS = builder_configs
-
-    def _info(self):
-        features = {}
-        if self.config.label_classes:
-            features["label"] = datasets.features.ClassLabel(names=self.config.label_classes)
-        else:
-            features["label"] = datasets.Value("float32")
-        features["idx"] = datasets.Value("int32")
-
-        # Thermostat-specific fields: Explainer outputs
-        features["attributions"] = datasets.Sequence(datasets.Value("float32"))
-        features["predictions"] = datasets.Sequence(datasets.Value("float32"))
-        features["input_ids"] = datasets.Sequence(datasets.Value("int32"))
-
-        return datasets.DatasetInfo(
-            description=self.config.description + f'\nDataset: {self.config.dataset}\nModel: {self.config.model}'
-                                                  f'\nExplainer: {self.config.explainer}\n',
-            features=datasets.Features(features),
-            homepage=_HOMEPAGE,
-            citation=_CITATION,
-        )
-
-    @staticmethod
-    def _get_drive_url(url):
-        base_url = 'https://drive.google.com/uc?id='
-        split_url = url.split('/')
-        return base_url + split_url[5]
-
-    def _split_generators(self, dl_manager):
-        """Returns SplitGenerators."""
-        # This method is tasked with downloading/extracting the data and defining the splits depending on the
-        #  configuration
-        if self.config.data_url.startswith("https://drive.google.com"):
-            dl_path = dl_manager.download_and_extract(self._get_drive_url(self.config.data_url))
-        else:
-            dl_path = dl_manager.download(self.config.data_url)
-        return [
-            datasets.SplitGenerator(
-                name=datasets.Split.TEST,
-                gen_kwargs={
-                    "data_file": dl_path,
-                    "split": "test",
-                }
-            )
-        ]
-
-    def _generate_examples(
-        self, data_file, split  # method parameters are unpacked from `gen_kwargs` as given in `_split_generators`
-    ):
-        """ Yields examples as (key, example) tuples. """
-        # This method handles input defined in _split_generators to yield (key, example) tuples from the dataset.
-
-        with open(data_file, encoding="utf-8") as f:
-            for id_, row in enumerate(f):
-                data = json.loads(row)
-                example = {feat: data[col] for feat, col in self.config.features.items()}
-                example["idx"] = id_
-                example["label"] = data["label"]
-                yield example["idx"], example
+# coding=utf-8
+# Copyright 2020 The HuggingFace Datasets Authors and the current dataset script contributor.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+
+import datasets
+import json
+
+from thermostat.data.thermostat_configs import builder_configs
+
+# Find for instance the citation on arxiv or on the dataset repo/website
+_CITATION = """\
+@misc{feldhus2021thermostat,
+      title={Thermostat: A Large Collection of NLP Model Explanations and Analysis Tools}, 
+      author={Nils Feldhus and Robert Schwarzenberg and Sebastian Möller},
+      year={2021},
+      eprint={2108.13961},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
+}
+"""
+
+_DESCRIPTION = "Thermostat is a large collection of NLP model explanations and accompanying analysis tools."
+
+# Link to an official homepage for the dataset
+_HOMEPAGE = 'https://github.com/DFKI-NLP/thermostat'
+
+# Licence for the dataset
+_LICENSE = 'Apache 2.0'
+
+
+class Thermostat(datasets.GeneratorBasedBuilder):
+    """One config (e.g. 'imdb-bert-lgxa') contains the attribution scores of a Layer Gradient x Activation explainer
+    applied on the IMDb dataset that has been classified by a BERT downstream model. """
+
+    BUILDER_CONFIGS = builder_configs
+
+    def _info(self):
+        features = {}
+        if self.config.label_classes:
+            features["label"] = datasets.features.ClassLabel(names=self.config.label_classes)
+        else:
+            features["label"] = datasets.Value("float32")
+        features["idx"] = datasets.Value("int32")
+
+        # Thermostat-specific fields: Explainer outputs
+        features["attributions"] = datasets.Sequence(datasets.Value("float32"))
+        features["predictions"] = datasets.Sequence(datasets.Value("float32"))
+        features["input_ids"] = datasets.Sequence(datasets.Value("int32"))
+
+        return datasets.DatasetInfo(
+            description=self.config.description + f'\nDataset: {self.config.dataset}\nModel: {self.config.model}'
+                                                  f'\nExplainer: {self.config.explainer}\n',
+            features=datasets.Features(features),
+            homepage=_HOMEPAGE,
+            citation=_CITATION,
+        )
+
+    @staticmethod
+    def _get_drive_url(url):
+        base_url = 'https://drive.google.com/uc?id='
+        split_url = url.split('/')
+        return base_url + split_url[5]
+
+    def _split_generators(self, dl_manager):
+        """Returns SplitGenerators."""
+        # This method is tasked with downloading/extracting the data and defining the splits depending on the
+        #  configuration
+        if self.config.data_url.startswith("https://drive.google.com"):
+            dl_path = dl_manager.download_and_extract(self._get_drive_url(self.config.data_url))
+        else:
+            dl_path = dl_manager.download(self.config.data_url)
+        return [
+            datasets.SplitGenerator(
+                name=datasets.Split.TEST,
+                gen_kwargs={
+                    "data_file": dl_path,
+                    "split": "test",
+                }
+            )
+        ]
+
+    def _generate_examples(
+        self, data_file, split  # method parameters are unpacked from `gen_kwargs` as given in `_split_generators`
+    ):
+        """ Yields examples as (key, example) tuples. """
+        # This method handles input defined in _split_generators to yield (key, example) tuples from the dataset.
+
+        with open(data_file, encoding="utf-8") as f:
+            for id_, row in enumerate(f):
+                data = json.loads(row)
+                example = {feat: data[col] for feat, col in self.config.features.items()}
+                example["idx"] = id_
+                example["label"] = data["label"]
+                yield example["idx"], example
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat/explainers/grad.py` & `thermostat-datasets-1.1.0/src/thermostat/explainers/grad.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-import torch
-from captum.attr import (
-    GuidedBackprop, LayerDeepLift, LayerIntegratedGradients, LayerGradientXActivation,)
-from transformers import XLNetForSequenceClassification
-from typing import Dict
-
-from thermostat.explain import ExplainerAutoModelInitializer
-from thermostat.utils import HookableModelWrapper
-
-
-class ExplainerLayerIntegratedGradients(ExplainerAutoModelInitializer):
-    def __init__(self):
-        super().__init__()
-        self.name_layer: str = None
-        self.layer = None
-        self.n_samples: int = None
-        self.internal_batch_size = None
-
-    def validate_config(self, config: Dict) -> bool:
-        super().validate_config(config)
-        assert 'n_samples' in config['explainer'], \
-            'Define how many samples to take along the straight line path from the baseline.'
-        assert 'internal_batch_size' in config['explainer'], 'Define an internal batch size for the attribute method.'
-
-    @classmethod
-    def from_config(cls, config):
-        res = super().from_config(config)
-        res.validate_config(config)
-        res.n_samples = config['explainer']['n_samples']
-        res.internal_batch_size = config['explainer']['internal_batch_size']
-        res.explainer = LayerIntegratedGradients(forward_func=res.forward_func,
-                                                 layer=res.get_embedding_layer(res.model))
-        return res
-
-    def explain(self, batch):
-        self.model.eval()
-        self.model.zero_grad()
-        batch = {k: v.to(self.device) for k, v in batch.items()}
-        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
-                                                                              batch=batch)
-        predictions = self.forward_func(inputs, *additional_forward_args)
-        target = torch.argmax(predictions, dim=1)
-        base_line = self.get_baseline(batch=batch)
-        attributions = self.explainer.attribute(inputs=inputs,
-                                                n_steps=self.n_samples,
-                                                additional_forward_args=additional_forward_args,
-                                                target=target,
-                                                baselines=base_line,
-                                                internal_batch_size=self.internal_batch_size)
-        attributions = torch.sum(attributions, dim=2)
-        if isinstance(self.model, XLNetForSequenceClassification):
-            # for xlnet, attributions.shape = [seq_len, batch_dim]
-            # but [batch_dim, seq_len] is assumed
-            attributions = attributions.T
-        return attributions, predictions  # xlnet: [130, 1]
-
-
-class ExplainerLayerGradientXActivation(ExplainerAutoModelInitializer):
-    def __init__(self):
-        super().__init__()
-        self.name_layer: str = None
-        self.layer = None
-
-    def validate_config(self, config: Dict) -> bool:
-        super().validate_config(config)
-
-    @classmethod
-    def from_config(cls, config):
-        res = super().from_config(config)
-        res.validate_config(config)
-        res.explainer = LayerGradientXActivation(forward_func=res.forward_func,
-                                                 layer=res.get_embedding_layer(res.model))
-        return res
-
-    def explain(self, batch):
-        self.model.eval()
-        self.model.zero_grad()
-        batch = {k: v.to(self.device) for k, v in batch.items()}
-        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
-                                                                              batch=batch)
-        predictions = self.forward_func(inputs, *additional_forward_args)
-        target = torch.argmax(predictions, dim=1)
-        attributions = self.explainer.attribute(inputs=inputs,
-                                                additional_forward_args=additional_forward_args,
-                                                target=target)
-        attributions = torch.sum(attributions, dim=2)
-        if isinstance(self.model, XLNetForSequenceClassification):
-            # for xlnet, attributions.shape = [seq_len, batch_dim]
-            # but [batch_dim, seq_len] is assumed
-            attributions = attributions.T
-        return attributions, predictions  # xlnet: [130, 1]
-
-
-class ExplainerDeepLift(ExplainerAutoModelInitializer):
-    def __init__(self):
-        super().__init__()
-
-    @classmethod
-    def from_config(cls, config):
-        res = super().from_config(config)
-        res.explainer = LayerDeepLift(model=HookableModelWrapper(res), layer=res.get_embedding_layer(res.model))
-        return res
-
-    def explain(self, batch):
-        self.model.eval()
-        batch = {k: v.to(self.device) for k, v in batch.items()}
-        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
-                                                                              batch=batch)
-        base_line = self.get_baseline(batch)
-        predictions = self.forward_func(inputs, *additional_forward_args)
-        target = torch.argmax(predictions, dim=1)
-        attributions = self.explainer.attribute(
-            inputs=inputs,
-            additional_forward_args=additional_forward_args,
-            target=target,
-            baselines=base_line,
-        )
-        attributions = torch.sum(attributions, dim=2)
-        if isinstance(self.model, XLNetForSequenceClassification):
-            # for xlnet, attributions.shape = [seq_len, batch_dim]
-            # but [batch_dim, seq_len] is assumed
-            attributions = attributions.T
-        return attributions, predictions
+import torch
+from captum.attr import (
+    GuidedBackprop, LayerDeepLift, LayerIntegratedGradients, LayerGradientXActivation,)
+from transformers import XLNetForSequenceClassification
+from typing import Dict
+
+from thermostat.explain import ExplainerAutoModelInitializer
+from thermostat.utils import HookableModelWrapper
+
+
+class ExplainerLayerIntegratedGradients(ExplainerAutoModelInitializer):
+    def __init__(self):
+        super().__init__()
+        self.name_layer: str = None
+        self.layer = None
+        self.n_samples: int = None
+        self.internal_batch_size = None
+
+    def validate_config(self, config: Dict) -> bool:
+        super().validate_config(config)
+        assert 'n_samples' in config['explainer'], \
+            'Define how many samples to take along the straight line path from the baseline.'
+        assert 'internal_batch_size' in config['explainer'], 'Define an internal batch size for the attribute method.'
+
+    @classmethod
+    def from_config(cls, config):
+        res = super().from_config(config)
+        res.validate_config(config)
+        res.n_samples = config['explainer']['n_samples']
+        res.internal_batch_size = config['explainer']['internal_batch_size']
+        res.explainer = LayerIntegratedGradients(forward_func=res.forward_func,
+                                                 layer=res.get_embedding_layer(res.model))
+        return res
+
+    def explain(self, batch):
+        self.model.eval()
+        self.model.zero_grad()
+        batch = {k: v.to(self.device) for k, v in batch.items()}
+        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
+                                                                              batch=batch)
+        predictions = self.forward_func(inputs, *additional_forward_args)
+        target = torch.argmax(predictions, dim=1)
+        base_line = self.get_baseline(batch=batch)
+        attributions = self.explainer.attribute(inputs=inputs,
+                                                n_steps=self.n_samples,
+                                                additional_forward_args=additional_forward_args,
+                                                target=target,
+                                                baselines=base_line,
+                                                internal_batch_size=self.internal_batch_size)
+        attributions = torch.sum(attributions, dim=2)
+        if isinstance(self.model, XLNetForSequenceClassification):
+            # for xlnet, attributions.shape = [seq_len, batch_dim]
+            # but [batch_dim, seq_len] is assumed
+            attributions = attributions.T
+        return attributions, predictions  # xlnet: [130, 1]
+
+
+class ExplainerLayerGradientXActivation(ExplainerAutoModelInitializer):
+    def __init__(self):
+        super().__init__()
+        self.name_layer: str = None
+        self.layer = None
+
+    def validate_config(self, config: Dict) -> bool:
+        super().validate_config(config)
+
+    @classmethod
+    def from_config(cls, config):
+        res = super().from_config(config)
+        res.validate_config(config)
+        res.explainer = LayerGradientXActivation(forward_func=res.forward_func,
+                                                 layer=res.get_embedding_layer(res.model))
+        return res
+
+    def explain(self, batch):
+        self.model.eval()
+        self.model.zero_grad()
+        batch = {k: v.to(self.device) for k, v in batch.items()}
+        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
+                                                                              batch=batch)
+        predictions = self.forward_func(inputs, *additional_forward_args)
+        target = torch.argmax(predictions, dim=1)
+        attributions = self.explainer.attribute(inputs=inputs,
+                                                additional_forward_args=additional_forward_args,
+                                                target=target)
+        attributions = torch.sum(attributions, dim=2)
+        if isinstance(self.model, XLNetForSequenceClassification):
+            # for xlnet, attributions.shape = [seq_len, batch_dim]
+            # but [batch_dim, seq_len] is assumed
+            attributions = attributions.T
+        return attributions, predictions  # xlnet: [130, 1]
+
+
+class ExplainerDeepLift(ExplainerAutoModelInitializer):
+    def __init__(self):
+        super().__init__()
+
+    @classmethod
+    def from_config(cls, config):
+        res = super().from_config(config)
+        res.explainer = LayerDeepLift(model=HookableModelWrapper(res), layer=res.get_embedding_layer(res.model))
+        return res
+
+    def explain(self, batch):
+        self.model.eval()
+        batch = {k: v.to(self.device) for k, v in batch.items()}
+        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
+                                                                              batch=batch)
+        base_line = self.get_baseline(batch)
+        predictions = self.forward_func(inputs, *additional_forward_args)
+        target = torch.argmax(predictions, dim=1)
+        attributions = self.explainer.attribute(
+            inputs=inputs,
+            additional_forward_args=additional_forward_args,
+            target=target,
+            baselines=base_line,
+        )
+        attributions = torch.sum(attributions, dim=2)
+        if isinstance(self.model, XLNetForSequenceClassification):
+            # for xlnet, attributions.shape = [seq_len, batch_dim]
+            # but [batch_dim, seq_len] is assumed
+            attributions = attributions.T
+        return attributions, predictions
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat/explainers/iba.py` & `thermostat-datasets-1.1.0/src/thermostat/explainers/iba.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,284 +1,284 @@
-""" From: https://github.com/bazingagin/IBA/ """
-
-import numpy as np
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from scipy.stats import norm
-from tqdm import tqdm
-
-from thermostat.explain import ExplainerAutoModelInitializer
-
-
-class IBASequential(nn.Sequential):
-    def forward(self, *inp):
-        for module in self._modules.values():
-            inp = module(*inp)
-        return inp
-
-
-class Estimator:
-    """
-    Useful to calculate the empirical mean and variance of intermediate feature maps.
-    """
-    def __init__(self, layer):
-        self.layer = layer
-        self.M = None  # running mean for each entry
-        self.S = None  # running std for each entry
-        self.N = None  # running num_seen for each entry
-        self.num_seen = 0  # total samples seen
-        self.eps = 1e-5
-
-    def feed(self, z: np.ndarray):
-
-        # Initialize if this is the first datapoint
-        if self.N is None:
-            self.M = np.zeros_like(z, dtype=float)
-            self.S = np.zeros_like(z, dtype=float)
-            self.N = np.zeros_like(z, dtype=float)
-
-        self.num_seen += 1
-
-        diff = (z - self.M)
-        self.N += 1
-        self.M += diff / self.num_seen
-        self.S += diff * (z - self.M)
-
-    def feed_batch(self, batch: np.ndarray):
-        for point in batch:
-            self.feed(point)
-
-    def shape(self):
-        return self.M.shape
-
-    def is_complete(self):
-        return self.num_seen > 0
-
-    def get_layer(self):
-        return self.layer
-
-    def mean(self):
-        return self.M.squeeze()
-
-    def p_zero(self):
-        return 1 - self.N / (self.num_seen + 1)  # Adding 1 for stablility, so that p_zero > 0 everywhere
-
-    def std(self, stabilize=True):
-        if stabilize:
-            # Add small numbers, so that dead neurons are not a problem
-            return np.sqrt(np.maximum(self.S, self.eps) / np.maximum(self.N, 1.0))
-
-        else:
-            return np.sqrt(self.S / self.N)
-
-    def estimate_density(self, z):
-        z_norm = (z - self.mean()) / self.std()
-        p = norm.pdf(z_norm, 0, 1)
-        return p
-
-    def normalize(self, z):
-        return (z - self.mean()) / self.std()
-
-    def load(self, what):
-        state = what if not isinstance(what, str) else torch.load(what)
-        # Check if estimator classes match
-        if self.__class__.__name__ != state["class"]:
-            raise RuntimeError("This Estimator is {}, cannot load {}".format(self.__class__.__name__, state["class"]))
-        # Check if layer classes match
-        if self.layer.__class__.__name__ != state["layer_class"]:
-            raise RuntimeError("This Layer is {}, cannot load {}".format(self.layer.__class__.__name__,
-                                                                         state["layer_class"]))
-        self.N = state["N"]
-        self.S = state["S"]
-        self.M = state["M"]
-        self.num_seen = state["num_seen"]
-
-
-class InformationBottleneck(nn.Module):
-    def __init__(self, mean: np.ndarray, std: np.ndarray, device=None):
-        super().__init__()
-        self.device = device
-        self.initial_value = 5.0
-        self.std = torch.tensor(std, dtype=torch.float, device=self.device, requires_grad=False)
-        self.mean = torch.tensor(mean, dtype=torch.float, device=self.device, requires_grad=False)
-        self.alpha = nn.Parameter(torch.full((1, *self.mean.shape), fill_value=self.initial_value, device=self.device))
-        self.sigmoid = nn.Sigmoid()
-        self.buffer_capacity = None
-
-        self.reset_alpha()
-
-    @staticmethod
-    def _sample_t(mu, log_noise_var):
-        log_noise_var = torch.clamp(log_noise_var, -10, 10)
-        noise_std = (log_noise_var / 2).exp()
-        eps = mu.data.new(mu.size()).normal_()
-        return mu + noise_std * eps
-
-    @staticmethod
-    def _calc_capacity(mu, log_var):
-        # KL[Q(t|x)||P(t)]
-        return -0.5 * (1 + log_var - mu**2 - log_var.exp())
-
-    def reset_alpha(self):
-        with torch.no_grad():
-            self.alpha.fill_(self.initial_value)
-        return self.alpha
-
-    def forward(self, bert_out):
-        x = bert_out
-        lamb = self.sigmoid(self.alpha)
-        lamb = lamb.expand(x.shape[0], x.shape[1], -1)
-        # We normalize x to simplify the computation of the KL-divergence
-        x_norm = (x - self.mean) / self.std
-        # Get sampling parameters
-        noise_var = (1-lamb)**2
-        scaled_signal = x_norm * lamb
-        noise_log_var = torch.log(noise_var)
-        # Sample new output values from p(t|x)
-        t_norm = self._sample_t(scaled_signal, noise_log_var)
-        self.buffer_capacity = self._calc_capacity(scaled_signal, noise_log_var)
-        # Denormalize t to match x
-        t = t_norm * self.std + self.mean
-        return (t,)
-
-
-class ExplainerIBA(ExplainerAutoModelInitializer):
-    def __init__(self, beta=1e-5, steps=10, lr=1, batch_size=1, progbar=False):
-        super().__init__()
-        self.beta = beta
-        self.batch_size = batch_size
-        self.progbar = progbar
-        self.lr = lr
-        self.train_steps = steps
-        self.ce_loss = []
-        self.info_loss = []
-        self.total_loss = []
-        self.pred = []
-
-        self.layer_idx = None
-        self.original_layer = None
-        self.shape = None
-        self.bottleneck = None
-        self.sequential = None
-        self.estim = None
-
-    @classmethod
-    def from_config(cls, config):
-        res = super().from_config(config)
-
-        def extract_bert_layer(model, layer_idx):
-            desired_layer = ''
-            for name, submodule in model.named_children():
-                for n, s in submodule.named_children():
-                    if n == 'encoder':
-                        for n2, s2 in s.named_children():
-                            for n3, s3 in s2.named_children():
-                                if n3 == str(layer_idx):
-                                    desired_layer = s3
-                                    return desired_layer
-
-        res.layer_idx = config['explainer']['layer_idx']
-        res.layer = extract_bert_layer(res.model, res.layer_idx)
-
-        res.estim = Estimator(res.layer)
-
-        res.original_layer = res.estim.get_layer()
-        return res
-
-    def attribute(self, inputs, target, segment=None):
-        saliency = self.buff_cap(inputs, target, segment)
-        saliency = saliency[0]
-        saliency = saliency.cpu().detach().numpy()
-        saliency = saliency.sum(axis=1)
-        saliency = saliency - saliency.min()
-        saliency = saliency / saliency.max()
-        return torch.tensor(saliency).unsqueeze(0)
-
-    def buff_cap(self, input_t, target, segment=None):
-        target_t = torch.tensor([target]) if not isinstance(target, torch.Tensor) else target
-        self._run_training(input_t, target_t, segment)
-        return self.explainer.buffer_capacity
-
-    def _run_training(self, input_t, target_t, segment=None):
-        # Attach layer and train the bottleneck
-        replace_layer(self.model, self.original_layer, self.sequential)
-        input_t = input_t.to(self.device)
-        target_t = target_t.to(self.device)
-        self._train_bottleneck(input_t, target_t, segment)
-        replace_layer(self.model, self.sequential, self.original_layer)
-
-    def _train_bottleneck(self, input_t: torch.Tensor, target_t: torch.Tensor, segment=None):
-        batch = input_t.expand(self.batch_size, -1), target_t.expand(self.batch_size)
-        optimizer = torch.optim.Adam(lr=self.lr, params=self.explainer.parameters())
-        # Reset from previous run or modifications
-        self.explainer.reset_alpha()
-        # Train
-        self.model.eval()
-        for _ in tqdm(range(self.train_steps), desc="Training Bottleneck",
-                      disable=not self.progbar):
-            optimizer.zero_grad()
-            if segment is not None:
-                out = self.model(batch[0], token_type_ids=segment)
-            else:
-                out = self.model(batch[0])
-            # print(out[0])
-            loss_t = self.calc_loss(outputs=out[0], labels=batch[1])
-            loss_t.backward()
-            optimizer.step(closure=None)
-            self.pred = out[0]
-
-    def calc_loss(self, outputs, labels):
-        """ Calculate the combined loss expression for optimization of lambda """
-        information_loss = self.explainer.buffer_capacity.mean()  # Taking the mean is equivalent of scaling with 1/K
-        cross_entropy = F.cross_entropy(outputs, target=labels)
-        total = cross_entropy + self.beta * information_loss
-        self.ce_loss.append(cross_entropy.cpu().detach().numpy())
-        self.info_loss.append(information_loss.cpu().detach().numpy())
-        self.total_loss.append(total.cpu().detach().numpy())
-        return total
-
-    def return_loss(self):
-        return self.ce_loss, self.info_loss, self.total_loss
-
-    def explain(self, batch):
-        batch = {k: v.to(self.device) for k, v in batch.items()}
-        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
-                                                                              batch=batch)
-        predictions = self.forward_func(inputs, *additional_forward_args)
-        target = torch.argmax(predictions, dim=1)
-
-        feature_map = list(self.model.base_model(inputs)[1][0])[self.layer_idx]
-
-        self.estim.feed(feature_map.detach().cpu().numpy())
-        self.shape = self.estim.shape()
-        self.explainer = InformationBottleneck(self.estim.mean(), self.estim.std(), device=self.device)
-        self.sequential = IBASequential(self.original_layer, self.explainer)
-
-        attributions = self.attribute(inputs=inputs,
-                                      target=target)  # TODO: Add additional_forward_args
-        return attributions, predictions
-
-
-def replace_layer(model: nn.Module, target: nn.Module, replacement: nn.Module):
-    """
-    Replace a given module within a parent module with some third module
-    Useful for injecting new layers in an existing model.
-    """
-    def replace_in(model: nn.Module, target: nn.Module, replacement: nn.Module):
-        for name, submodule in model.named_children():
-            if submodule == target:
-                if isinstance(model, nn.ModuleList):
-                    model[int(name)] = replacement
-                elif isinstance(model, nn.Sequential):
-                    model[int(name)] = replacement
-                else:
-                    model.__setattr__(name, replacement)
-                return True
-            elif len(list(submodule.named_children())) > 0:
-                if replace_in(submodule, target, replacement):
-                    return True
-        return False
-
-    if not replace_in(model, target, replacement):
-        raise RuntimeError("Cannot substitute layer: Layer of type " + target.__class__.__name__ +
-                           " is not a child of given parent of type " + model.__class__.__name__)
+""" From: https://github.com/bazingagin/IBA/ """
+
+import numpy as np
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+from scipy.stats import norm
+from tqdm import tqdm
+
+from thermostat.explain import ExplainerAutoModelInitializer
+
+
+class IBASequential(nn.Sequential):
+    def forward(self, *inp):
+        for module in self._modules.values():
+            inp = module(*inp)
+        return inp
+
+
+class Estimator:
+    """
+    Useful to calculate the empirical mean and variance of intermediate feature maps.
+    """
+    def __init__(self, layer):
+        self.layer = layer
+        self.M = None  # running mean for each entry
+        self.S = None  # running std for each entry
+        self.N = None  # running num_seen for each entry
+        self.num_seen = 0  # total samples seen
+        self.eps = 1e-5
+
+    def feed(self, z: np.ndarray):
+
+        # Initialize if this is the first datapoint
+        if self.N is None:
+            self.M = np.zeros_like(z, dtype=float)
+            self.S = np.zeros_like(z, dtype=float)
+            self.N = np.zeros_like(z, dtype=float)
+
+        self.num_seen += 1
+
+        diff = (z - self.M)
+        self.N += 1
+        self.M += diff / self.num_seen
+        self.S += diff * (z - self.M)
+
+    def feed_batch(self, batch: np.ndarray):
+        for point in batch:
+            self.feed(point)
+
+    def shape(self):
+        return self.M.shape
+
+    def is_complete(self):
+        return self.num_seen > 0
+
+    def get_layer(self):
+        return self.layer
+
+    def mean(self):
+        return self.M.squeeze()
+
+    def p_zero(self):
+        return 1 - self.N / (self.num_seen + 1)  # Adding 1 for stablility, so that p_zero > 0 everywhere
+
+    def std(self, stabilize=True):
+        if stabilize:
+            # Add small numbers, so that dead neurons are not a problem
+            return np.sqrt(np.maximum(self.S, self.eps) / np.maximum(self.N, 1.0))
+
+        else:
+            return np.sqrt(self.S / self.N)
+
+    def estimate_density(self, z):
+        z_norm = (z - self.mean()) / self.std()
+        p = norm.pdf(z_norm, 0, 1)
+        return p
+
+    def normalize(self, z):
+        return (z - self.mean()) / self.std()
+
+    def load(self, what):
+        state = what if not isinstance(what, str) else torch.load(what)
+        # Check if estimator classes match
+        if self.__class__.__name__ != state["class"]:
+            raise RuntimeError("This Estimator is {}, cannot load {}".format(self.__class__.__name__, state["class"]))
+        # Check if layer classes match
+        if self.layer.__class__.__name__ != state["layer_class"]:
+            raise RuntimeError("This Layer is {}, cannot load {}".format(self.layer.__class__.__name__,
+                                                                         state["layer_class"]))
+        self.N = state["N"]
+        self.S = state["S"]
+        self.M = state["M"]
+        self.num_seen = state["num_seen"]
+
+
+class InformationBottleneck(nn.Module):
+    def __init__(self, mean: np.ndarray, std: np.ndarray, device=None):
+        super().__init__()
+        self.device = device
+        self.initial_value = 5.0
+        self.std = torch.tensor(std, dtype=torch.float, device=self.device, requires_grad=False)
+        self.mean = torch.tensor(mean, dtype=torch.float, device=self.device, requires_grad=False)
+        self.alpha = nn.Parameter(torch.full((1, *self.mean.shape), fill_value=self.initial_value, device=self.device))
+        self.sigmoid = nn.Sigmoid()
+        self.buffer_capacity = None
+
+        self.reset_alpha()
+
+    @staticmethod
+    def _sample_t(mu, log_noise_var):
+        log_noise_var = torch.clamp(log_noise_var, -10, 10)
+        noise_std = (log_noise_var / 2).exp()
+        eps = mu.data.new(mu.size()).normal_()
+        return mu + noise_std * eps
+
+    @staticmethod
+    def _calc_capacity(mu, log_var):
+        # KL[Q(t|x)||P(t)]
+        return -0.5 * (1 + log_var - mu**2 - log_var.exp())
+
+    def reset_alpha(self):
+        with torch.no_grad():
+            self.alpha.fill_(self.initial_value)
+        return self.alpha
+
+    def forward(self, bert_out):
+        x = bert_out
+        lamb = self.sigmoid(self.alpha)
+        lamb = lamb.expand(x.shape[0], x.shape[1], -1)
+        # We normalize x to simplify the computation of the KL-divergence
+        x_norm = (x - self.mean) / self.std
+        # Get sampling parameters
+        noise_var = (1-lamb)**2
+        scaled_signal = x_norm * lamb
+        noise_log_var = torch.log(noise_var)
+        # Sample new output values from p(t|x)
+        t_norm = self._sample_t(scaled_signal, noise_log_var)
+        self.buffer_capacity = self._calc_capacity(scaled_signal, noise_log_var)
+        # Denormalize t to match x
+        t = t_norm * self.std + self.mean
+        return (t,)
+
+
+class ExplainerIBA(ExplainerAutoModelInitializer):
+    def __init__(self, beta=1e-5, steps=10, lr=1, batch_size=1, progbar=False):
+        super().__init__()
+        self.beta = beta
+        self.batch_size = batch_size
+        self.progbar = progbar
+        self.lr = lr
+        self.train_steps = steps
+        self.ce_loss = []
+        self.info_loss = []
+        self.total_loss = []
+        self.pred = []
+
+        self.layer_idx = None
+        self.original_layer = None
+        self.shape = None
+        self.bottleneck = None
+        self.sequential = None
+        self.estim = None
+
+    @classmethod
+    def from_config(cls, config):
+        res = super().from_config(config)
+
+        def extract_bert_layer(model, layer_idx):
+            desired_layer = ''
+            for name, submodule in model.named_children():
+                for n, s in submodule.named_children():
+                    if n == 'encoder':
+                        for n2, s2 in s.named_children():
+                            for n3, s3 in s2.named_children():
+                                if n3 == str(layer_idx):
+                                    desired_layer = s3
+                                    return desired_layer
+
+        res.layer_idx = config['explainer']['layer_idx']
+        res.layer = extract_bert_layer(res.model, res.layer_idx)
+
+        res.estim = Estimator(res.layer)
+
+        res.original_layer = res.estim.get_layer()
+        return res
+
+    def attribute(self, inputs, target, segment=None):
+        saliency = self.buff_cap(inputs, target, segment)
+        saliency = saliency[0]
+        saliency = saliency.cpu().detach().numpy()
+        saliency = saliency.sum(axis=1)
+        saliency = saliency - saliency.min()
+        saliency = saliency / saliency.max()
+        return torch.tensor(saliency).unsqueeze(0)
+
+    def buff_cap(self, input_t, target, segment=None):
+        target_t = torch.tensor([target]) if not isinstance(target, torch.Tensor) else target
+        self._run_training(input_t, target_t, segment)
+        return self.explainer.buffer_capacity
+
+    def _run_training(self, input_t, target_t, segment=None):
+        # Attach layer and train the bottleneck
+        replace_layer(self.model, self.original_layer, self.sequential)
+        input_t = input_t.to(self.device)
+        target_t = target_t.to(self.device)
+        self._train_bottleneck(input_t, target_t, segment)
+        replace_layer(self.model, self.sequential, self.original_layer)
+
+    def _train_bottleneck(self, input_t: torch.Tensor, target_t: torch.Tensor, segment=None):
+        batch = input_t.expand(self.batch_size, -1), target_t.expand(self.batch_size)
+        optimizer = torch.optim.Adam(lr=self.lr, params=self.explainer.parameters())
+        # Reset from previous run or modifications
+        self.explainer.reset_alpha()
+        # Train
+        self.model.eval()
+        for _ in tqdm(range(self.train_steps), desc="Training Bottleneck",
+                      disable=not self.progbar):
+            optimizer.zero_grad()
+            if segment is not None:
+                out = self.model(batch[0], token_type_ids=segment)
+            else:
+                out = self.model(batch[0])
+            # print(out[0])
+            loss_t = self.calc_loss(outputs=out[0], labels=batch[1])
+            loss_t.backward()
+            optimizer.step(closure=None)
+            self.pred = out[0]
+
+    def calc_loss(self, outputs, labels):
+        """ Calculate the combined loss expression for optimization of lambda """
+        information_loss = self.explainer.buffer_capacity.mean()  # Taking the mean is equivalent of scaling with 1/K
+        cross_entropy = F.cross_entropy(outputs, target=labels)
+        total = cross_entropy + self.beta * information_loss
+        self.ce_loss.append(cross_entropy.cpu().detach().numpy())
+        self.info_loss.append(information_loss.cpu().detach().numpy())
+        self.total_loss.append(total.cpu().detach().numpy())
+        return total
+
+    def return_loss(self):
+        return self.ce_loss, self.info_loss, self.total_loss
+
+    def explain(self, batch):
+        batch = {k: v.to(self.device) for k, v in batch.items()}
+        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
+                                                                              batch=batch)
+        predictions = self.forward_func(inputs, *additional_forward_args)
+        target = torch.argmax(predictions, dim=1)
+
+        feature_map = list(self.model.base_model(inputs)[1][0])[self.layer_idx]
+
+        self.estim.feed(feature_map.detach().cpu().numpy())
+        self.shape = self.estim.shape()
+        self.explainer = InformationBottleneck(self.estim.mean(), self.estim.std(), device=self.device)
+        self.sequential = IBASequential(self.original_layer, self.explainer)
+
+        attributions = self.attribute(inputs=inputs,
+                                      target=target)  # TODO: Add additional_forward_args
+        return attributions, predictions
+
+
+def replace_layer(model: nn.Module, target: nn.Module, replacement: nn.Module):
+    """
+    Replace a given module within a parent module with some third module
+    Useful for injecting new layers in an existing model.
+    """
+    def replace_in(model: nn.Module, target: nn.Module, replacement: nn.Module):
+        for name, submodule in model.named_children():
+            if submodule == target:
+                if isinstance(model, nn.ModuleList):
+                    model[int(name)] = replacement
+                elif isinstance(model, nn.Sequential):
+                    model[int(name)] = replacement
+                else:
+                    model.__setattr__(name, replacement)
+                return True
+            elif len(list(submodule.named_children())) > 0:
+                if replace_in(submodule, target, replacement):
+                    return True
+        return False
+
+    if not replace_in(model, target, replacement):
+        raise RuntimeError("Cannot substitute layer: Layer of type " + target.__class__.__name__ +
+                           " is not a child of given parent of type " + model.__class__.__name__)
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat/explainers/lime.py` & `thermostat-datasets-1.1.0/src/thermostat/explainers/lime.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-import torch
-from captum.attr import KernelShap, Lime, LimeBase
-from captum._utils.models.linear_model import SkLearnLasso, SkLearnLinearModel
-from functools import partial
-from math import exp
-from typing import Any, Dict, List
-
-from thermostat.explain import ExplainerAutoModelInitializer
-from thermostat.utils import detach_to_list
-
-
-class ExplainerLime(ExplainerAutoModelInitializer):
-    def __init__(self):
-        super().__init__()
-        self.n_samples = None
-
-    @staticmethod
-    def token_similarity_kernel(
-            original_input: torch.Tensor,
-            perturbed_input: torch.Tensor,
-            perturbed_interpretable_input: torch.Tensor,
-            **kwargs) -> torch.Tensor:
-        """
-        Following https://github.com/copenlu/ALPS_2021
-        """
-        pad_token_id = 0
-        kernel_width = 1.1
-        assert original_input.shape[0] == perturbed_input.shape[0] == 1, 'This kernel assumes batch size 1'
-        original_input_list = detach_to_list(original_input[0])
-        perturbed_input_list = detach_to_list(perturbed_input[0])
-        number_pad_tokens_original = original_input_list.count(pad_token_id)
-        number_pad_tokens_perturbed = perturbed_input_list.count(pad_token_id)
-        distance = (number_pad_tokens_perturbed - number_pad_tokens_original) / number_pad_tokens_original
-        similarity = exp(-distance**2/kernel_width**2)
-        return similarity
-
-    @classmethod
-    def from_config(cls, config):
-        res = super().from_config(config)
-        res.n_samples = config['explainer']['n_samples']
-        res.explainer = Lime(forward_func=res.forward_func, interpretable_model=SkLearnLasso(alpha=0.0))
-        return res
-
-    def explain(self, batch):
-        self.model.eval()
-        assert len(batch['input_ids']) == 1, 'This implementation assumes that the batch size is 1.'
-        batch = {k: v.to(self.device) for k, v in batch.items()}
-        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
-                                                                              batch=batch)
-        base_line = self.get_baseline(batch)
-        predictions = self.forward_func(inputs, *additional_forward_args)
-        target = torch.argmax(predictions, dim=1)
-        attributions = self.explainer.attribute(
-            inputs=inputs,
-            additional_forward_args=additional_forward_args,
-            target=target.item(),
-            n_samples=self.n_samples,
-            baselines=base_line,
-        )
-        return attributions, predictions
-
-
-class ExplainerLimeBase(ExplainerAutoModelInitializer):
-    def __init__(self):
-        super().__init__()
-        self.n_samples = None
-
-    def validate_config(self, config: Dict) -> bool:
-        super().validate_config(config)
-        assert 'n_samples' in config['explainer'], 'Set number of samples for attribution function.'
-        assert 'mask_prob' in config['explainer'], 'Set probability of masking a token in perturbation function.'
-        assert 0 <= config['explainer']['mask_prob'] <= 1, 'Mask probability must be between 0 and 1.'
-
-    @classmethod
-    def from_config(cls, config):
-        res = super().from_config(config)
-        res.validate_config(config)
-        res.n_samples = config['explainer']['n_samples']
-        res.mask_prob = config['explainer']['mask_prob']
-        res.interpretable_model = SkLearnLinearModel("linear_model.Ridge")
-
-        res.explainer = LimeBase(forward_func=res.forward_func,
-                                 interpretable_model=res.interpretable_model,
-                                 similarity_func=cls.token_similarity_kernel,
-                                 perturb_func=partial(ExplainerLimeBase.perturb_func,
-                                                      res.mask_prob,
-                                                      res.special_token_ids,
-                                                      res.pad_token_id,
-                                                      res.device),
-                                 perturb_interpretable_space=False,
-                                 from_interp_rep_transform=None,
-                                 to_interp_rep_transform=cls.to_interp_rep_transform_custom)
-        return res
-
-    @staticmethod
-    def token_similarity_kernel(
-            original_input: torch.Tensor,
-            perturbed_input: torch.Tensor,
-            perturbed_interpretable_input: torch.Tensor,
-            **kwargs) -> torch.Tensor:
-        """
-        Following https://github.com/copenlu/ALPS_2021
-        """
-        assert original_input.shape[0] == perturbed_input.shape[0] == 1, 'Batch size for LIME needs to be 1'
-        return torch.sum(original_input[0] == perturbed_input[0]) / len(original_input[0])
-
-    @staticmethod
-    def perturb_func(
-            mask_prob: float,
-            special_token_ids: List[int],
-            pad_token_id: int,
-            device: str,
-            original_input: torch.Tensor,  # always needs to be last argument before **kwargs due to "partial"
-            **kwargs: Any) -> torch.Tensor:
-        """
-        Sampling function
-        Following https://github.com/copenlu/ALPS_2021
-        """
-        # Build mask for replacing random tokens with [PAD] token
-        mask_value_probs = torch.tensor([mask_prob, 1 - mask_prob])
-        mask_multinomial_binary = torch.multinomial(mask_value_probs,
-                                                    len(original_input[0]),
-                                                    replacement=True)
-
-        # Additionally remove special_token_ids
-        mask_special_token_ids = torch.Tensor([1 if id_ in special_token_ids else 0
-                                               for id_ in detach_to_list(original_input[0])]).int()
-
-        # Merge the binary mask (12.5% masks) with the special_token_ids mask
-        mask = torch.tensor([m + s if s == 0 else s for m, s in zip(
-            mask_multinomial_binary, mask_special_token_ids)]).to(device)
-        # TODO: Would it be faster if the other tensors above were also on the device (cuda)?
-
-        # Apply mask to original input
-        perturbed_input = original_input * mask + (1 - mask) * pad_token_id
-        return perturbed_input
-
-    @staticmethod
-    def to_interp_rep_transform_custom(curr_sample, original_input, **kwargs: Any):
-        return curr_sample
-
-    def explain(self, batch):
-        batch = {k: v.to(self.device) for k, v in batch.items()}
-        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
-                                                                              batch=batch)
-
-        predictions = self.forward_func(inputs, *additional_forward_args)
-        target = torch.argmax(predictions, dim=1)
-        attributions = self.explainer.attribute(inputs=inputs,
-                                                n_samples=self.n_samples,
-                                                additional_forward_args=additional_forward_args,
-                                                target=target)
-        return attributions, predictions
-
-
-class ExplainerKernelShap(ExplainerAutoModelInitializer):
-    def __init__(self):
-        raise NotImplementedError
-        super().__init__()
-        self.internal_batch_size = None
-        self.n_samples = None
-
-    def validate_config(self, config: Dict) -> bool:
-        super().validate_config(config)
-        assert 'n_samples' in config['explainer'], 'Set number of samples for attribution function.'
-
-    @classmethod
-    def from_config(cls, config):
-        res = super().from_config(config)
-        res.validate_config(config)
-        res.n_samples = config['explainer']['n_samples']
-        res.explainer = KernelShap(forward_func=res.forward_func, interpretable_model=SkLearnLasso(alpha=0.0))
-        return res
-
-    def explain(self, batch):
-        assert len(batch['input_ids']) == 1, 'This implementation assumes that the batch size is 1.'
-        batch = {k: v.to(self.device) for k, v in batch.items()}
-        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
-                                                                              batch=batch)
-
-        predictions = self.forward_func(inputs, *additional_forward_args)
-        target = torch.argmax(predictions, dim=1)
-        base_line = self.get_baseline(batch=batch)
-        attributions = self.explainer.attribute(inputs=inputs,
-                                                n_samples=self.n_samples,
-                                                additional_forward_args=additional_forward_args,
-                                                target=target,
-                                                baseline=base_line)
-        return attributions, predictions
+import torch
+from captum.attr import KernelShap, Lime, LimeBase
+from captum._utils.models.linear_model import SkLearnLasso, SkLearnLinearModel
+from functools import partial
+from math import exp
+from typing import Any, Dict, List
+
+from thermostat.explain import ExplainerAutoModelInitializer
+from thermostat.utils import detach_to_list
+
+
+class ExplainerLime(ExplainerAutoModelInitializer):
+    def __init__(self):
+        super().__init__()
+        self.n_samples = None
+
+    @staticmethod
+    def token_similarity_kernel(
+            original_input: torch.Tensor,
+            perturbed_input: torch.Tensor,
+            perturbed_interpretable_input: torch.Tensor,
+            **kwargs) -> torch.Tensor:
+        """
+        Following https://github.com/copenlu/ALPS_2021
+        """
+        pad_token_id = 0
+        kernel_width = 1.1
+        assert original_input.shape[0] == perturbed_input.shape[0] == 1, 'This kernel assumes batch size 1'
+        original_input_list = detach_to_list(original_input[0])
+        perturbed_input_list = detach_to_list(perturbed_input[0])
+        number_pad_tokens_original = original_input_list.count(pad_token_id)
+        number_pad_tokens_perturbed = perturbed_input_list.count(pad_token_id)
+        distance = (number_pad_tokens_perturbed - number_pad_tokens_original) / number_pad_tokens_original
+        similarity = exp(-distance**2/kernel_width**2)
+        return similarity
+
+    @classmethod
+    def from_config(cls, config):
+        res = super().from_config(config)
+        res.n_samples = config['explainer']['n_samples']
+        res.explainer = Lime(forward_func=res.forward_func, interpretable_model=SkLearnLasso(alpha=0.0))
+        return res
+
+    def explain(self, batch):
+        self.model.eval()
+        assert len(batch['input_ids']) == 1, 'This implementation assumes that the batch size is 1.'
+        batch = {k: v.to(self.device) for k, v in batch.items()}
+        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
+                                                                              batch=batch)
+        base_line = self.get_baseline(batch)
+        predictions = self.forward_func(inputs, *additional_forward_args)
+        target = torch.argmax(predictions, dim=1)
+        attributions = self.explainer.attribute(
+            inputs=inputs,
+            additional_forward_args=additional_forward_args,
+            target=target.item(),
+            n_samples=self.n_samples,
+            baselines=base_line,
+        )
+        return attributions, predictions
+
+
+class ExplainerLimeBase(ExplainerAutoModelInitializer):
+    def __init__(self):
+        super().__init__()
+        self.n_samples = None
+
+    def validate_config(self, config: Dict) -> bool:
+        super().validate_config(config)
+        assert 'n_samples' in config['explainer'], 'Set number of samples for attribution function.'
+        assert 'mask_prob' in config['explainer'], 'Set probability of masking a token in perturbation function.'
+        assert 0 <= config['explainer']['mask_prob'] <= 1, 'Mask probability must be between 0 and 1.'
+
+    @classmethod
+    def from_config(cls, config):
+        res = super().from_config(config)
+        res.validate_config(config)
+        res.n_samples = config['explainer']['n_samples']
+        res.mask_prob = config['explainer']['mask_prob']
+        res.interpretable_model = SkLearnLinearModel("linear_model.Ridge")
+
+        res.explainer = LimeBase(forward_func=res.forward_func,
+                                 interpretable_model=res.interpretable_model,
+                                 similarity_func=cls.token_similarity_kernel,
+                                 perturb_func=partial(ExplainerLimeBase.perturb_func,
+                                                      res.mask_prob,
+                                                      res.special_token_ids,
+                                                      res.pad_token_id,
+                                                      res.device),
+                                 perturb_interpretable_space=False,
+                                 from_interp_rep_transform=None,
+                                 to_interp_rep_transform=cls.to_interp_rep_transform_custom)
+        return res
+
+    @staticmethod
+    def token_similarity_kernel(
+            original_input: torch.Tensor,
+            perturbed_input: torch.Tensor,
+            perturbed_interpretable_input: torch.Tensor,
+            **kwargs) -> torch.Tensor:
+        """
+        Following https://github.com/copenlu/ALPS_2021
+        """
+        assert original_input.shape[0] == perturbed_input.shape[0] == 1, 'Batch size for LIME needs to be 1'
+        return torch.sum(original_input[0] == perturbed_input[0]) / len(original_input[0])
+
+    @staticmethod
+    def perturb_func(
+            mask_prob: float,
+            special_token_ids: List[int],
+            pad_token_id: int,
+            device: str,
+            original_input: torch.Tensor,  # always needs to be last argument before **kwargs due to "partial"
+            **kwargs: Any) -> torch.Tensor:
+        """
+        Sampling function
+        Following https://github.com/copenlu/ALPS_2021
+        """
+        # Build mask for replacing random tokens with [PAD] token
+        mask_value_probs = torch.tensor([mask_prob, 1 - mask_prob])
+        mask_multinomial_binary = torch.multinomial(mask_value_probs,
+                                                    len(original_input[0]),
+                                                    replacement=True)
+
+        # Additionally remove special_token_ids
+        mask_special_token_ids = torch.Tensor([1 if id_ in special_token_ids else 0
+                                               for id_ in detach_to_list(original_input[0])]).int()
+
+        # Merge the binary mask (12.5% masks) with the special_token_ids mask
+        mask = torch.tensor([m + s if s == 0 else s for m, s in zip(
+            mask_multinomial_binary, mask_special_token_ids)]).to(device)
+        # TODO: Would it be faster if the other tensors above were also on the device (cuda)?
+
+        # Apply mask to original input
+        perturbed_input = original_input * mask + (1 - mask) * pad_token_id
+        return perturbed_input
+
+    @staticmethod
+    def to_interp_rep_transform_custom(curr_sample, original_input, **kwargs: Any):
+        return curr_sample
+
+    def explain(self, batch):
+        batch = {k: v.to(self.device) for k, v in batch.items()}
+        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
+                                                                              batch=batch)
+
+        predictions = self.forward_func(inputs, *additional_forward_args)
+        target = torch.argmax(predictions, dim=1)
+        attributions = self.explainer.attribute(inputs=inputs,
+                                                n_samples=self.n_samples,
+                                                additional_forward_args=additional_forward_args,
+                                                target=target)
+        return attributions, predictions
+
+
+class ExplainerKernelShap(ExplainerAutoModelInitializer):
+    def __init__(self):
+        raise NotImplementedError
+        super().__init__()
+        self.internal_batch_size = None
+        self.n_samples = None
+
+    def validate_config(self, config: Dict) -> bool:
+        super().validate_config(config)
+        assert 'n_samples' in config['explainer'], 'Set number of samples for attribution function.'
+
+    @classmethod
+    def from_config(cls, config):
+        res = super().from_config(config)
+        res.validate_config(config)
+        res.n_samples = config['explainer']['n_samples']
+        res.explainer = KernelShap(forward_func=res.forward_func, interpretable_model=SkLearnLasso(alpha=0.0))
+        return res
+
+    def explain(self, batch):
+        assert len(batch['input_ids']) == 1, 'This implementation assumes that the batch size is 1.'
+        batch = {k: v.to(self.device) for k, v in batch.items()}
+        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
+                                                                              batch=batch)
+
+        predictions = self.forward_func(inputs, *additional_forward_args)
+        target = torch.argmax(predictions, dim=1)
+        base_line = self.get_baseline(batch=batch)
+        attributions = self.explainer.attribute(inputs=inputs,
+                                                n_samples=self.n_samples,
+                                                additional_forward_args=additional_forward_args,
+                                                target=target,
+                                                baseline=base_line)
+        return attributions, predictions
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat/explainers/shap.py` & `thermostat-datasets-1.1.0/src/thermostat/explainers/shap.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import torch
-from captum.attr import (
-    LayerGradientShap, LayerDeepLiftShap,)
-from transformers import XLNetForSequenceClassification
-from typing import Dict
-
-from thermostat.explain import ExplainerAutoModelInitializer
-from thermostat.utils import HookableModelWrapper
-
-
-class ExplainerLayerGradientShap(ExplainerAutoModelInitializer):
-    def __init__(self):
-        super().__init__()
-        self.name_layer: str = None
-        self.layer = None
-        self.n_samples: int = None
-
-    def validate_config(self, config: Dict) -> bool:
-        super().validate_config(config)
-        assert 'n_samples' in config['explainer'], \
-            'Define how many samples to take along the straight line path from the baseline.'
-
-    @classmethod
-    def from_config(cls, config):
-        res = super().from_config(config)
-        res.validate_config(config)
-        res.n_samples = config['explainer']['n_samples']
-        
-        res.model.eval() # setting the model to eval and zero grad 
-        res.model.zero_grad() # so we do not have to loop it in explainer for each batch.
-        
-        res.explainer = LayerGradientShap(forward_func=res.forward_func,
-                                                 layer=res.get_embedding_layer(res.model))
-        return res
-
-    def explain(self, batch):
-        
-        batch = {k: v.to(self.device) for k, v in batch.items()}
-        
-        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
-                                                                              batch=batch)
-        
-        predictions = self.forward_func(inputs, *additional_forward_args)
-        target = torch.argmax(predictions, dim=1)
-        
-        base_line = self.get_baseline(batch=batch)
-        
-        attributions = self.explainer.attribute(inputs=inputs,
-                                                baselines=base_line,
-                                                n_samples =self.n_samples,
-                                                target=target,
-                                                additional_forward_args=additional_forward_args)
-                                                
-        attributions = torch.sum(attributions, dim=2)
-        
-        if isinstance(self.model, XLNetForSequenceClassification):
-            # for xlnet, attributions.shape = [seq_len, batch_dim]
-            # but [batch_dim, seq_len] is assumed
-            attributions = attributions.T 
-            
-        return attributions, predictions  # xlnet: [130, 1]
-
-
-
-class ExplainerLayerDeepLiftShap(ExplainerAutoModelInitializer):
-    def __init__(self):
-        super().__init__()
-
-    @classmethod
-    def from_config(cls, config):
-        res = super().from_config(config)
-        
-        res.model.eval() # setting the model to eval and zero grad 
-        res.model.zero_grad() # so we do not have to loop it in explainer for each batch.
-        
-        res.explainer = LayerDeepLiftShap(model=HookableModelWrapper(res), layer=res.get_embedding_layer(res.model))
-        
-        return res
-
-    def explain(self, batch):
-
-        batch = {k: v.to(self.device) for k, v in batch.items()}
-        
-        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
-                                                                              batch=batch)
-        base_line = self.get_baseline(batch)
-        base_line = torch.stack((torch.zeros_like(inputs[0]), base_line[0])) # stacking to provide more than one example for base line
-        
-        predictions = self.forward_func(inputs, *additional_forward_args)
-        target = torch.argmax(predictions, dim=1)
-        
-        attributions = self.explainer.attribute(
-            inputs=inputs.float(),
-            additional_forward_args=additional_forward_args,
-            target=target,
-            baselines=base_line.float(),
-        )
-        
-        attributions = torch.sum(attributions, dim=2)
-        
-        if isinstance(self.model, XLNetForSequenceClassification):
-            # for xlnet, attributions.shape = [seq_len, batch_dim]
-            # but [batch_dim, seq_len] is assumed
-            attributions = attributions.T
-        
-        return attributions, predictions
+import torch
+from captum.attr import (
+    LayerGradientShap, LayerDeepLiftShap,)
+from transformers import XLNetForSequenceClassification
+from typing import Dict
+
+from thermostat.explain import ExplainerAutoModelInitializer
+from thermostat.utils import HookableModelWrapper
+
+
+class ExplainerLayerGradientShap(ExplainerAutoModelInitializer):
+    def __init__(self):
+        super().__init__()
+        self.name_layer: str = None
+        self.layer = None
+        self.n_samples: int = None
+
+    def validate_config(self, config: Dict) -> bool:
+        super().validate_config(config)
+        assert 'n_samples' in config['explainer'], \
+            'Define how many samples to take along the straight line path from the baseline.'
+
+    @classmethod
+    def from_config(cls, config):
+        res = super().from_config(config)
+        res.validate_config(config)
+        res.n_samples = config['explainer']['n_samples']
+        
+        res.model.eval() # setting the model to eval and zero grad 
+        res.model.zero_grad() # so we do not have to loop it in explainer for each batch.
+        
+        res.explainer = LayerGradientShap(forward_func=res.forward_func,
+                                                 layer=res.get_embedding_layer(res.model))
+        return res
+
+    def explain(self, batch):
+        
+        batch = {k: v.to(self.device) for k, v in batch.items()}
+        
+        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
+                                                                              batch=batch)
+        
+        predictions = self.forward_func(inputs, *additional_forward_args)
+        target = torch.argmax(predictions, dim=1)
+        
+        base_line = self.get_baseline(batch=batch)
+        
+        attributions = self.explainer.attribute(inputs=inputs,
+                                                baselines=base_line,
+                                                n_samples =self.n_samples,
+                                                target=target,
+                                                additional_forward_args=additional_forward_args)
+                                                
+        attributions = torch.sum(attributions, dim=2)
+        
+        if isinstance(self.model, XLNetForSequenceClassification):
+            # for xlnet, attributions.shape = [seq_len, batch_dim]
+            # but [batch_dim, seq_len] is assumed
+            attributions = attributions.T 
+            
+        return attributions, predictions  # xlnet: [130, 1]
+
+
+
+class ExplainerLayerDeepLiftShap(ExplainerAutoModelInitializer):
+    def __init__(self):
+        super().__init__()
+
+    @classmethod
+    def from_config(cls, config):
+        res = super().from_config(config)
+        
+        res.model.eval() # setting the model to eval and zero grad 
+        res.model.zero_grad() # so we do not have to loop it in explainer for each batch.
+        
+        res.explainer = LayerDeepLiftShap(model=HookableModelWrapper(res), layer=res.get_embedding_layer(res.model))
+        
+        return res
+
+    def explain(self, batch):
+
+        batch = {k: v.to(self.device) for k, v in batch.items()}
+        
+        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
+                                                                              batch=batch)
+        base_line = self.get_baseline(batch)
+        base_line = torch.stack((torch.zeros_like(inputs[0]), base_line[0])) # stacking to provide more than one example for base line
+        
+        predictions = self.forward_func(inputs, *additional_forward_args)
+        target = torch.argmax(predictions, dim=1)
+        
+        attributions = self.explainer.attribute(
+            inputs=inputs.float(),
+            additional_forward_args=additional_forward_args,
+            target=target,
+            baselines=base_line.float(),
+        )
+        
+        attributions = torch.sum(attributions, dim=2)
+        
+        if isinstance(self.model, XLNetForSequenceClassification):
+            # for xlnet, attributions.shape = [seq_len, batch_dim]
+            # but [batch_dim, seq_len] is assumed
+            attributions = attributions.T
+        
+        return attributions, predictions
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat/explainers/svs.py` & `thermostat-datasets-1.1.0/src/thermostat/explainers/svs.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import torch
-from captum.attr import ShapleyValueSampling
-from typing import Dict
-
-from thermostat.explain import ExplainerAutoModelInitializer
-
-
-class ExplainerShapleyValueSampling(ExplainerAutoModelInitializer):
-
-    def __init__(self):
-        super().__init__()
-        self.n_samples = None
-
-    def validate_config(self, config: Dict) -> bool:
-        super().validate_config(config)
-        assert 'n_samples' in config['explainer'], 'Define how many samples to take along the straight line path ' \
-                                                   'from the baseline.'
-
-    @classmethod
-    def from_config(cls, config):
-        res = super().from_config(config)
-        res.n_samples = config['explainer']['n_samples']
-        res.explainer = ShapleyValueSampling(res.forward_func)
-        return res
-
-    def explain(self, batch):
-        # todo: set model.eval() ? -> in a test self.model.training was False
-        batch = {k: v.to(self.device) for k, v in batch.items()}
-        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
-                                                                              batch=batch)
-        predictions = self.forward_func(inputs, *additional_forward_args)
-        target = torch.argmax(predictions, dim=1)
-        base_line = self.get_baseline(batch=batch)
-        attributions = self.explainer.attribute(inputs=inputs,
-                                                n_samples=self.n_samples,
-                                                additional_forward_args=additional_forward_args,
-                                                target=target,
-                                                baselines=base_line)
-        return attributions, predictions
+import torch
+from captum.attr import ShapleyValueSampling
+from typing import Dict
+
+from thermostat.explain import ExplainerAutoModelInitializer
+
+
+class ExplainerShapleyValueSampling(ExplainerAutoModelInitializer):
+
+    def __init__(self):
+        super().__init__()
+        self.n_samples = None
+
+    def validate_config(self, config: Dict) -> bool:
+        super().validate_config(config)
+        assert 'n_samples' in config['explainer'], 'Define how many samples to take along the straight line path ' \
+                                                   'from the baseline.'
+
+    @classmethod
+    def from_config(cls, config):
+        res = super().from_config(config)
+        res.n_samples = config['explainer']['n_samples']
+        res.explainer = ShapleyValueSampling(res.forward_func)
+        return res
+
+    def explain(self, batch):
+        # todo: set model.eval() ? -> in a test self.model.training was False
+        batch = {k: v.to(self.device) for k, v in batch.items()}
+        inputs, additional_forward_args = self.get_inputs_and_additional_args(base_model=type(self.model.base_model),
+                                                                              batch=batch)
+        predictions = self.forward_func(inputs, *additional_forward_args)
+        target = torch.argmax(predictions, dim=1)
+        base_line = self.get_baseline(batch=batch)
+        attributions = self.explainer.attribute(inputs=inputs,
+                                                n_samples=self.n_samples,
+                                                additional_forward_args=additional_forward_args,
+                                                target=target,
+                                                baselines=base_line)
+        return attributions, predictions
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat/visualize.py` & `thermostat-datasets-1.1.0/src/thermostat/visualize.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-import math
-import numpy as np
-import os
-import pandas as pd
-import torch
-from tqdm import tqdm
-from spacy import displacy
-from spacy.util import is_in_jupyter
-from transformers import AutoTokenizer
-from typing import Dict
-
-from thermostat.data import get_local_explanations
-from thermostat.utils import delistify, detach_to_list, read_path
-
-
-class ColorToken:
-    def __init__(self, token, attribution, text_field, token_index, thermounit_vars: Dict):
-        self.token = token
-        self.attribution = attribution
-        self.text_field = text_field
-        self.token_index = token_index
-        for var_name, value in thermounit_vars.items():
-            if var_name not in ['texts']:
-                setattr(self, var_name, value)
-
-        # White color per default
-        self.red = '255'
-        self.green = '255'
-        self.blue = '255'
-        self.score = None
-
-        assert not math.isnan(self.attribution), 'Attribution of token {} is NaN'.format(self.token)
-
-    def add_color(self, gamma, threshold=0):
-        """ Needs to be explicitly called to calculate the color of a token """
-        score = self.gamma_correction(self.attribution, gamma)
-        if score >= threshold:
-            r = str(int(255))
-            g = str(int(255 * (1 - score)))
-            b = str(int(255 * (1 - score)))
-        else:
-            b = str(int(255))
-            r = str(int(255 * (1 + score)))
-            g = str(int(255 * (1 + score)))
-
-        # TODO: Add more color schemes from: https://colorbrewer2.org/#type=diverging&scheme=RdBu&n=5
-        self.red = r
-        self.green = g
-        self.blue = b
-        setattr(self, 'score', round(score, ndigits=3))
-
-    def __repr__(self):
-        if "score" in vars(self):
-            score_str = f'Score: {self.score}'
-        else:
-            score_str = f'Attribution: {self.attribution}'
-        return f'{self.token} (Index: {self.token_index}, {score_str}, Color: {self.hex()}, ' \
-               f'Text field: {self.text_field})'
-
-    def __str__(self):
-        return repr(self)
-
-    @staticmethod
-    def gamma_correction(score, gamma):
-        return np.sign(score) * np.power(np.abs(score), gamma)
-
-    def hex(self):
-        return '#%02x%02x%02x' % (int(self.red), int(self.green), int(self.blue))
-
-
-class TextField(list):
-    def __init__(self, color_tokens):
-        super().__init__(color_tokens)
-
-    def __repr__(self):
-        return ' '.join([ctok.token for ctok in self])
-
-
-class Heatmap(TextField):
-    def __init__(self, color_tokens, attributions=None, gamma=1.0):
-        super().__init__(color_tokens)
-        for i in range(len(self)):
-            if attributions:
-                self[i].attribution = attributions[i]
-            self[i].add_color(gamma=gamma)
-        self.table = pd.DataFrame({
-            'token_index': delistify(self['token_index']),
-            'token': delistify(self['token']),
-            'attribution': delistify(self['attribution']),
-            'text_field': delistify(self['text_field'])}
-        ).set_index('token_index').T
-
-    def __getitem__(self, idx):
-        if isinstance(idx, str):
-            """ String indexing """
-            if idx in list(self[0].__dict__.keys()):
-                return [getattr(u, idx) for u in self]
-        return list(self)[idx]
-
-    def __repr__(self):
-        return repr(self.table)
-
-    def render(self, labels=False):
-        """ Uses the displaCy visualization tool to render a HTML from the heatmap """
-
-        # Call this function once for every text field
-        if len(set([t.text_field for t in self])) > 1:
-            for field in self[0].text_fields:
-                print(f'Heatmap "{field}"')
-                Heatmap([t for t in self if t.text_field == field]).render(labels=labels)
-            return
-
-        ents = []
-        colors = {}
-        ii = 0
-        for color_token in self:
-            ff = ii + len(color_token.token)
-
-            # One entity in displaCy contains start and end markers (character index) and optionally a label
-            # The label can be added by setting "attribution_labels" to True
-            ent = {
-                'start': ii,
-                'end': ff,
-                'label': str(color_token.score),
-            }
-
-            ents.append(ent)
-            # A "colors" dict takes care of the mapping between attribution labels and hex colors
-            colors[str(color_token.score)] = color_token.hex()
-            ii = ff
-
-        to_render = {
-            'text': ''.join([t.token for t in self]),
-            'ents': ents,
-        }
-
-        if labels:
-            template = """
-            <mark class="entity" style="background: {bg}; padding: 0.45em 0.6em; margin: 0 0.25em; line-height: 2; 
-            border-radius: 0.35em; box-decoration-break: clone; -webkit-box-decoration-break: clone">
-                {text}
-                <span style="font-size: 0.8em; font-weight: bold; line-height: 1; border-radius: 0.35em; text-transform: 
-                uppercase; vertical-align: middle; margin-left: 0.5rem">{label}</span>
-            </mark>
-            """
-        else:
-            template = """
-            <mark class="entity" style="background: {bg}; padding: 0.15em 0.3em; margin: 0 0.2em; line-height: 2.2;
-            border-radius: 0.25em; box-decoration-break: clone; -webkit-box-decoration-break: clone">
-                {text}
-            </mark>
-            """
-
-        html = displacy.render(
-            to_render,
-            style='ent',
-            manual=True,
-            jupyter=is_in_jupyter(),
-            options={'template': template,
-                     'colors': colors,
-                     }
-        )
-        return html if not is_in_jupyter() else None
-
-
-def token_to_html(token, rgb):
-    return f"<span style=\"background-color: {rgb}\"> {token.replace('<', '').replace('>', '')} </span>"
-
-
-def summarize(summary: Dict):
-    res = "<h4>"
-    for k, v in summary.items():
-        res += f"{k}: {summary[k]} <br/>"
-    res += "</h4>"
-    return res
-
-
-def append_heatmap(tokens, scores, latex, gamma, caption, pad_token, formatting="colorbox", truncate_pad=True):
-    """
-    Produce a heatmap for LaTeX
-    Format options: colorbox, text"""
-    if gamma != 1:
-        raise NotImplementedError
-    latex += "\n\\begin{figure}[!htb]"
-    for token, score in zip(tokens, scores):
-        if token == pad_token and truncate_pad:
-            continue
-        color = "blue"
-        if score >= 0:
-            color = "red"
-        latex += f"\\{formatting}" + "{" + f"{color}!{abs(score) * 100}" + "}" + "{" + token + "}"
-    latex += "\\caption{" + f"{caption}" + "}"
-    latex += "\\end{figure}\n"
-    return latex
-
-
-def normalize_attributions(attributions):
-    max_abs_score = max(max(attributions), abs(min(attributions)))
-    return [(score / max_abs_score) for score in attributions]
-
-
-def run_visualize(config: Dict, dataset=None):
-    raise NotImplementedError("Deprecated due to Heatmap and ColorToken refactoring")
-    tokenizer = AutoTokenizer.from_pretrained(config['model']['name'])
-    visualization_config = config['visualization']
-
-    if not dataset:
-        dataset = get_local_explanations(config=visualization_config)
-    dataset_name = f'{config["dataset"]["name"]}' \
-                   f': {config["dataset"]["subset"]}' if 'subset' in config['dataset'] else \
-        config['dataset']['name']
-    str_dataset_name = f'{dataset_name} ({config["dataset"]["split"]})'
-
-    file_out = open(read_path(config['path_html']), 'w+')
-
-    tokenizer_str = str(type(tokenizer)).split('.')[-1].strip("'>")
-    for idx_instance in tqdm(range(len(dataset))):
-        instance = dataset[idx_instance]
-
-        html = f"<html><h3>"
-        html += f"<h2>Instance: {instance['idx']} | Dataset: {str_dataset_name} |" \
-                f" Model: {config['model']['name']} | Tokenizer: {tokenizer_str}"
-        html += '</h3><div style=\"border:3px solid #000;\">'
-
-        html += "<div>"
-
-        tokens = [tokenizer.decode(token_ids=token_ids) for token_ids in instance['input_ids']]
-        atts = detach_to_list(instance['attributions'])
-
-        if visualization_config['normalize']:
-            atts = normalize_attributions(atts)
-
-        heatmap = Heatmap(words=tokens, scores=atts, gamma=visualization_config['gamma'])
-
-        summary = {'Sum of Attribution Scores': str(sum(atts))}
-
-        if 'dataset' in dataset:
-            label_names = dataset['dataset'][0]['label_names']
-        else:
-            label_names = dataset.info.features['label'].names
-        if 'labels' in instance or 'label' in instance:
-            if 'labels' in instance:
-                label = detach_to_list(instance['labels'])
-            else:
-                label = instance['label']
-            summary['True Label Index'] = str(label)
-            summary['True Label'] = str(label_names[label])
-        if 'predictions' in instance:
-            preds = instance['predictions']
-            summary['Logits'] = detach_to_list(preds)
-            preds_max = torch.argmax(preds) if type(preds) == torch.Tensor else preds.index(max(preds))
-            preds_max_detached = detach_to_list(preds_max)
-            summary['Predicted Label'] = str(label_names[preds_max_detached])
-        html += summarize(summary)
-
-        for instance in heatmap:  # brackets to reuse iterator
-            html += token_to_html(instance['token'], instance['color'])
-        html += "</br></br>"
-        html += "</div>"
-        html += "</div></br></br></br></html>"
-        file_out.write(html + os.linesep)
+import math
+import numpy as np
+import os
+import pandas as pd
+import torch
+from tqdm import tqdm
+from spacy import displacy
+from spacy.util import is_in_jupyter
+from transformers import AutoTokenizer
+from typing import Dict
+
+from thermostat.data import get_local_explanations
+from thermostat.utils import delistify, detach_to_list, read_path
+
+
+class ColorToken:
+    def __init__(self, token, attribution, text_field, token_index, thermounit_vars: Dict):
+        self.token = token
+        self.attribution = attribution
+        self.text_field = text_field
+        self.token_index = token_index
+        for var_name, value in thermounit_vars.items():
+            if var_name not in ['texts']:
+                setattr(self, var_name, value)
+
+        # White color per default
+        self.red = '255'
+        self.green = '255'
+        self.blue = '255'
+        self.score = None
+
+        assert not math.isnan(self.attribution), 'Attribution of token {} is NaN'.format(self.token)
+
+    def add_color(self, gamma, threshold=0):
+        """ Needs to be explicitly called to calculate the color of a token """
+        score = self.gamma_correction(self.attribution, gamma)
+        if score >= threshold:
+            r = str(int(255))
+            g = str(int(255 * (1 - score)))
+            b = str(int(255 * (1 - score)))
+        else:
+            b = str(int(255))
+            r = str(int(255 * (1 + score)))
+            g = str(int(255 * (1 + score)))
+
+        # TODO: Add more color schemes from: https://colorbrewer2.org/#type=diverging&scheme=RdBu&n=5
+        self.red = r
+        self.green = g
+        self.blue = b
+        setattr(self, 'score', round(score, ndigits=3))
+
+    def __repr__(self):
+        if "score" in vars(self):
+            score_str = f'Score: {self.score}'
+        else:
+            score_str = f'Attribution: {self.attribution}'
+        return f'{self.token} (Index: {self.token_index}, {score_str}, Color: {self.hex()}, ' \
+               f'Text field: {self.text_field})'
+
+    def __str__(self):
+        return repr(self)
+
+    @staticmethod
+    def gamma_correction(score, gamma):
+        return np.sign(score) * np.power(np.abs(score), gamma)
+
+    def hex(self):
+        return '#%02x%02x%02x' % (int(self.red), int(self.green), int(self.blue))
+
+
+class TextField(list):
+    def __init__(self, color_tokens):
+        super().__init__(color_tokens)
+
+    def __repr__(self):
+        return ' '.join([ctok.token for ctok in self])
+
+
+class Heatmap(TextField):
+    def __init__(self, color_tokens, attributions=None, gamma=1.0):
+        super().__init__(color_tokens)
+        for i in range(len(self)):
+            if attributions:
+                self[i].attribution = attributions[i]
+            self[i].add_color(gamma=gamma)
+        self.table = pd.DataFrame({
+            'token_index': delistify(self['token_index']),
+            'token': delistify(self['token']),
+            'attribution': delistify(self['attribution']),
+            'text_field': delistify(self['text_field'])}
+        ).set_index('token_index').T
+
+    def __getitem__(self, idx):
+        if isinstance(idx, str):
+            """ String indexing """
+            if idx in list(self[0].__dict__.keys()):
+                return [getattr(u, idx) for u in self]
+        return list(self)[idx]
+
+    def __repr__(self):
+        return repr(self.table)
+
+    def render(self, labels=False):
+        """ Uses the displaCy visualization tool to render a HTML from the heatmap """
+
+        # Call this function once for every text field
+        if len(set([t.text_field for t in self])) > 1:
+            for field in self[0].text_fields:
+                print(f'Heatmap "{field}"')
+                Heatmap([t for t in self if t.text_field == field]).render(labels=labels)
+            return
+
+        ents = []
+        colors = {}
+        ii = 0
+        for color_token in self:
+            ff = ii + len(color_token.token)
+
+            # One entity in displaCy contains start and end markers (character index) and optionally a label
+            # The label can be added by setting "attribution_labels" to True
+            ent = {
+                'start': ii,
+                'end': ff,
+                'label': str(color_token.score),
+            }
+
+            ents.append(ent)
+            # A "colors" dict takes care of the mapping between attribution labels and hex colors
+            colors[str(color_token.score)] = color_token.hex()
+            ii = ff
+
+        to_render = {
+            'text': ''.join([t.token for t in self]),
+            'ents': ents,
+        }
+
+        if labels:
+            template = """
+            <mark class="entity" style="background: {bg}; padding: 0.45em 0.6em; margin: 0 0.25em; line-height: 2; 
+            border-radius: 0.35em; box-decoration-break: clone; -webkit-box-decoration-break: clone">
+                {text}
+                <span style="font-size: 0.8em; font-weight: bold; line-height: 1; border-radius: 0.35em; text-transform: 
+                uppercase; vertical-align: middle; margin-left: 0.5rem">{label}</span>
+            </mark>
+            """
+        else:
+            template = """
+            <mark class="entity" style="background: {bg}; padding: 0.15em 0.3em; margin: 0 0.2em; line-height: 2.2;
+            border-radius: 0.25em; box-decoration-break: clone; -webkit-box-decoration-break: clone">
+                {text}
+            </mark>
+            """
+
+        html = displacy.render(
+            to_render,
+            style='ent',
+            manual=True,
+            jupyter=is_in_jupyter(),
+            options={'template': template,
+                     'colors': colors,
+                     }
+        )
+        return html if not is_in_jupyter() else None
+
+
+def token_to_html(token, rgb):
+    return f"<span style=\"background-color: {rgb}\"> {token.replace('<', '').replace('>', '')} </span>"
+
+
+def summarize(summary: Dict):
+    res = "<h4>"
+    for k, v in summary.items():
+        res += f"{k}: {summary[k]} <br/>"
+    res += "</h4>"
+    return res
+
+
+def append_heatmap(tokens, scores, latex, gamma, caption, pad_token, formatting="colorbox", truncate_pad=True):
+    """
+    Produce a heatmap for LaTeX
+    Format options: colorbox, text"""
+    if gamma != 1:
+        raise NotImplementedError
+    latex += "\n\\begin{figure}[!htb]"
+    for token, score in zip(tokens, scores):
+        if token == pad_token and truncate_pad:
+            continue
+        color = "blue"
+        if score >= 0:
+            color = "red"
+        latex += f"\\{formatting}" + "{" + f"{color}!{abs(score) * 100}" + "}" + "{" + token + "}"
+    latex += "\\caption{" + f"{caption}" + "}"
+    latex += "\\end{figure}\n"
+    return latex
+
+
+def normalize_attributions(attributions):
+    max_abs_score = max(max(attributions), abs(min(attributions)))
+    return [(score / max_abs_score) for score in attributions]
+
+
+def run_visualize(config: Dict, dataset=None):
+    raise NotImplementedError("Deprecated due to Heatmap and ColorToken refactoring")
+    tokenizer = AutoTokenizer.from_pretrained(config['model']['name'])
+    visualization_config = config['visualization']
+
+    if not dataset:
+        dataset = get_local_explanations(config=visualization_config)
+    dataset_name = f'{config["dataset"]["name"]}' \
+                   f': {config["dataset"]["subset"]}' if 'subset' in config['dataset'] else \
+        config['dataset']['name']
+    str_dataset_name = f'{dataset_name} ({config["dataset"]["split"]})'
+
+    file_out = open(read_path(config['path_html']), 'w+')
+
+    tokenizer_str = str(type(tokenizer)).split('.')[-1].strip("'>")
+    for idx_instance in tqdm(range(len(dataset))):
+        instance = dataset[idx_instance]
+
+        html = f"<html><h3>"
+        html += f"<h2>Instance: {instance['idx']} | Dataset: {str_dataset_name} |" \
+                f" Model: {config['model']['name']} | Tokenizer: {tokenizer_str}"
+        html += '</h3><div style=\"border:3px solid #000;\">'
+
+        html += "<div>"
+
+        tokens = [tokenizer.decode(token_ids=token_ids) for token_ids in instance['input_ids']]
+        atts = detach_to_list(instance['attributions'])
+
+        if visualization_config['normalize']:
+            atts = normalize_attributions(atts)
+
+        heatmap = Heatmap(words=tokens, scores=atts, gamma=visualization_config['gamma'])
+
+        summary = {'Sum of Attribution Scores': str(sum(atts))}
+
+        if 'dataset' in dataset:
+            label_names = dataset['dataset'][0]['label_names']
+        else:
+            label_names = dataset.info.features['label'].names
+        if 'labels' in instance or 'label' in instance:
+            if 'labels' in instance:
+                label = detach_to_list(instance['labels'])
+            else:
+                label = instance['label']
+            summary['True Label Index'] = str(label)
+            summary['True Label'] = str(label_names[label])
+        if 'predictions' in instance:
+            preds = instance['predictions']
+            summary['Logits'] = detach_to_list(preds)
+            preds_max = torch.argmax(preds) if type(preds) == torch.Tensor else preds.index(max(preds))
+            preds_max_detached = detach_to_list(preds_max)
+            summary['Predicted Label'] = str(label_names[preds_max_detached])
+        html += summarize(summary)
+
+        for instance in heatmap:  # brackets to reuse iterator
+            html += token_to_html(instance['token'], instance['color'])
+        html += "</br></br>"
+        html += "</div>"
+        html += "</div></br></br></br></html>"
+        file_out.write(html + os.linesep)
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat_datasets.egg-info/PKG-INFO` & `thermostat-datasets-1.1.0/src/thermostat_datasets.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-Metadata-Version: 2.1
-Name: thermostat-datasets
-Version: 1.0.2.1
-Summary: Collection of NLP model explanations and accompanying analysis tools
-Home-page: https://github.com/DFKI-NLP/thermostat
-Download-URL: https://github.com/DFKI-NLP/thermostat/tags
-Author: DFKI-NLP
-Author-email: nils.feldhus@dfki.de
-License: Apache 2.0
-Keywords: explainability heatmaps feature-attribution natural-language-processing
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-License-File: LICENSE
-
-Thermostat is a large collection of NLP model explanations and accompanying analysis tools. Combines explainability methods from the captum library with Hugging Face's datasets and transformers. Mitigates repetitive execution of common experiments in Explainable NLP and thus reduces the environmental impact and financial roadblocks. Increases comparability and replicability of research. Reduces the implementational burden.
-
+Metadata-Version: 2.1
+Name: thermostat-datasets
+Version: 1.1.0
+Summary: Collection of NLP model explanations and accompanying analysis tools
+Home-page: https://github.com/DFKI-NLP/thermostat
+Download-URL: https://github.com/DFKI-NLP/thermostat/tags
+Author: DFKI-NLP
+Author-email: nils.feldhus@dfki.de
+License: Apache 2.0
+Keywords: explainability heatmaps feature-attribution natural-language-processing
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+License-File: LICENSE
+
+Thermostat is a large collection of NLP model explanations and accompanying analysis tools. Combines explainability methods from the captum library with Hugging Face's datasets and transformers. Mitigates repetitive execution of common experiments in Explainable NLP and thus reduces the environmental impact and financial roadblocks. Increases comparability and replicability of research. Reduces the implementational burden.
```

### Comparing `thermostat-datasets-1.0.2.1/src/thermostat_datasets.egg-info/SOURCES.txt` & `thermostat-datasets-1.1.0/src/thermostat_datasets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/thermostat/explain.py
 src/thermostat/utils.py
 src/thermostat/visualize.py
 src/thermostat/data/__init__.py
 src/thermostat/data/additional_configs.py
 src/thermostat/data/dataset_utils.py
 src/thermostat/data/readers.py
+src/thermostat/data/stats.py
 src/thermostat/data/thermostat_configs.py
 src/thermostat/data/tokenization.py
 src/thermostat/explainers/__init__.py
 src/thermostat/explainers/grad.py
 src/thermostat/explainers/iba.py
 src/thermostat/explainers/lime.py
 src/thermostat/explainers/occlusion.py
```


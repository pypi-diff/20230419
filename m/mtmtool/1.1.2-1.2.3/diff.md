# Comparing `tmp/mtmtool-1.1.2.tar.gz` & `tmp/mtmtool-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtmtool-1.1.2.tar", last modified: Mon Apr 17 03:26:31 2023, max compression
+gzip compressed data, was "mtmtool-1.2.3.tar", last modified: Wed Apr 19 14:29:08 2023, max compression
```

## Comparing `mtmtool-1.1.2.tar` & `mtmtool-1.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 03:26:31.234565 mtmtool-1.1.2/
--rw-rw-rw-   0        0        0    11524 2022-08-15 09:04:59.000000 mtmtool-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      111 2022-08-15 08:52:36.000000 mtmtool-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      660 2023-04-17 03:26:31.233566 mtmtool-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       81 2022-08-15 12:44:58.000000 mtmtool-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 03:26:31.234565 mtmtool-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2048 2023-04-17 03:26:15.000000 mtmtool-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:26:31.206565 mtmtool-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 03:26:31.224568 mtmtool-1.1.2/src/mtmtool/
--rw-rw-rw-   0        0        0        0 2023-04-17 03:06:16.000000 mtmtool-1.1.2/src/mtmtool/__init__.py
--rw-rw-rw-   0        0        0      685 2023-04-17 01:37:42.000000 mtmtool-1.1.2/src/mtmtool/functool.py
--rw-rw-rw-   0        0        0     1789 2023-04-17 02:36:55.000000 mtmtool-1.1.2/src/mtmtool/io.py
--rw-rw-rw-   0        0        0      455 2022-04-22 10:44:55.000000 mtmtool-1.1.2/src/mtmtool/itertools.py
--rw-rw-rw-   0        0        0     2218 2023-04-17 02:34:55.000000 mtmtool-1.1.2/src/mtmtool/log.py
--rw-rw-rw-   0        0        0     1477 2023-02-07 13:55:47.000000 mtmtool-1.1.2/src/mtmtool/pool.py
--rw-rw-rw-   0        0        0     3727 2022-08-15 08:20:51.000000 mtmtool-1.1.2/src/mtmtool/projection.py
--rw-rw-rw-   0        0        0     1587 2022-11-04 09:07:39.000000 mtmtool-1.1.2/src/mtmtool/time.py
--rw-rw-rw-   0        0        0     2337 2023-04-17 02:37:31.000000 mtmtool-1.1.2/src/mtmtool/webhook.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:26:31.231565 mtmtool-1.1.2/src/mtmtool.egg-info/
--rw-rw-rw-   0        0        0      660 2023-04-17 03:26:31.000000 mtmtool-1.1.2/src/mtmtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-04-17 03:26:31.000000 mtmtool-1.1.2/src/mtmtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 03:26:31.000000 mtmtool-1.1.2/src/mtmtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 03:06:03.000000 mtmtool-1.1.2/src/mtmtool.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-04-17 03:26:31.000000 mtmtool-1.1.2/src/mtmtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 03:26:31.000000 mtmtool-1.1.2/src/mtmtool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 03:26:31.232565 mtmtool-1.1.2/test/
--rw-rw-rw-   0        0        0     1371 2023-04-07 11:28:25.000000 mtmtool-1.1.2/test/test_args2kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:29:08.484391 mtmtool-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-04-19 14:28:55.000000 mtmtool-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-19 14:28:55.000000 mtmtool-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-19 14:29:08.484391 mtmtool-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-04-19 14:28:55.000000 mtmtool-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 14:29:08.484391 mtmtool-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-04-19 14:28:55.000000 mtmtool-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:29:08.480391 mtmtool-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:29:08.484391 mtmtool-1.2.3/src/mtmtool/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/functool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2322 2023-04-19 14:28:55.000000 mtmtool-1.2.3/src/mtmtool/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:29:08.484391 mtmtool-1.2.3/src/mtmtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-19 14:29:08.000000 mtmtool-1.2.3/src/mtmtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-04-19 14:29:08.000000 mtmtool-1.2.3/src/mtmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 14:29:08.000000 mtmtool-1.2.3/src/mtmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 14:29:08.000000 mtmtool-1.2.3/src/mtmtool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-19 14:29:08.000000 mtmtool-1.2.3/src/mtmtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-19 14:29:08.000000 mtmtool-1.2.3/src/mtmtool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:29:08.484391 mtmtool-1.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-04-19 14:28:55.000000 mtmtool-1.2.3/test/test_args2kwargs.py
```

### Comparing `mtmtool-1.1.2/LICENSE` & `mtmtool-1.2.3/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-Apache License
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
+Apache License
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
    limitations under the License.
```

### Comparing `mtmtool-1.1.2/PKG-INFO` & `mtmtool-1.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1
-Name: mtmtool
-Version: 1.1.2
-Summary:  A Personal Python Tool Library.
-Home-page: https://github.com/imutum/imutum_python_tool
-Author: imutum
-Author-email: 
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# mdfpytool
-
-A personal code tool
-
-个人使用的简单的Python代码片段
+Metadata-Version: 2.1
+Name: mtmtool
+Version: 1.2.3
+Summary:  A Personal Python Tool Library.
+Home-page: https://github.com/imutum/imutum_python_tool
+Author: imutum
+Author-email: 
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mdfpytool
+
+A personal code tool
+
+个人使用的简单的Python代码片段
```

### Comparing `mtmtool-1.1.2/setup.py` & `mtmtool-1.2.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,66 @@
-import os, shutil, sys, glob
-
-package_name = "imutum_python_tool"
-abbreviation_name = "mtmtool"
-description = " A Personal Python Tool Library."
-version = "1.1.2"
-
-
-def check_requires(requires: list):
-    pip_file = "pip.exe" if "win" in sys.platform else "pip"
-    pip_paths = [
-        os.path.join(os.path.dirname(sys.executable), "Scripts", pip_file),
-        os.path.join(os.path.dirname(sys.executable), pip_file),
-    ]
-    for _path in pip_paths:
-        if os.path.exists(_path):
-            pip_exe = _path
-            break
-    for require in requires:
-        try:
-            __import__(require)
-        except:
-            os.system(f"{pip_exe} install {require}")
-
-
-# Setiptools Support
-check_requires(["setuptools"])
-import setuptools
-
-# Path Support
-os.chdir(os.path.dirname(__file__))
-if os.path.isdir('build'):
-    print('INFO del dir ', 'build')
-    shutil.rmtree('build')
-
-# README Doc
-with open("README.md", encoding="utf-8") as f:
-    long_description = f.read()
-
-# Setup
-setuptools.setup(
-    name=abbreviation_name,  #应用名
-    author="imutum",
-    author_email="",
-    version=version,  #版本号
-    description=(f"{package_name}" if not len(description) else description),
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url=f"https://github.com/imutum/{package_name}",
-    packages=setuptools.find_packages("src"),  #包括在安装包内的Python包
-    package_dir={"": "src"},
-    zip_safe=False,
-    include_package_data=True,  #启用清单文件MANIFEST.in,包含数据文件
-    install_requires=["requests", "pyyaml"],
-    # ext_modules=ext_modules,
-    python_requires='>=3.8',
-    classifiers=[
-        "Programming Language :: Python :: 3.8",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: MacOS",
-        "Operating System :: POSIX :: Linux",
-        "Operating System :: Microsoft :: Windows",
-    ],
-)
+import os, shutil, sys, glob
+
+package_name = "imutum_python_tool"
+abbreviation_name = "mtmtool"
+description = " A Personal Python Tool Library."
+version = "1.2.3"
+
+
+def check_requires(requires: list):
+    pip_file = "pip.exe" if "win" in sys.platform else "pip"
+    pip_paths = [
+        os.path.join(os.path.dirname(sys.executable), "Scripts", pip_file),
+        os.path.join(os.path.dirname(sys.executable), pip_file),
+    ]
+    for _path in pip_paths:
+        if os.path.exists(_path):
+            pip_exe = _path
+            break
+    for require in requires:
+        try:
+            __import__(require)
+        except:
+            os.system(f"{pip_exe} install {require}")
+
+
+# Setiptools Support
+check_requires(["setuptools"])
+import setuptools
+
+# Path Support
+os.chdir(os.path.dirname(__file__))
+if os.path.isdir('build'):
+    print('INFO del dir ', 'build')
+    shutil.rmtree('build')
+
+# README Doc
+with open("README.md", encoding="utf-8") as f:
+    long_description = f.read()
+
+# Setup
+setuptools.setup(
+    name=abbreviation_name,  #应用名
+    author="imutum",
+    author_email="",
+    version=version,  #版本号
+    description=(f"{package_name}" if not len(description) else description),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url=f"https://github.com/imutum/{package_name}",
+    packages=setuptools.find_packages("src"),  #包括在安装包内的Python包
+    package_dir={"": "src"},
+    zip_safe=False,
+    include_package_data=True,  #启用清单文件MANIFEST.in,包含数据文件
+    install_requires=["requests", "pyyaml"],
+    # ext_modules=ext_modules,
+    python_requires='>=3.8',
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Programming Language :: Python :: 3.8",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: MacOS",
+        "Operating System :: POSIX :: Linux",
+        "Operating System :: Microsoft :: Windows",
+    ],
+)
```

### Comparing `mtmtool-1.1.2/src/mtmtool/functool.py` & `mtmtool-1.2.3/src/mtmtool/functool.py`

 * *Files identical despite different names*

### Comparing `mtmtool-1.1.2/src/mtmtool/log.py` & `mtmtool-1.2.3/src/mtmtool/log.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,65 @@
-import os
-import logging
-from functools import wraps
-from .functool import func_args2kwargs
-
-level_dict = {
-    "DEBUG": logging.DEBUG,
-    "INFO": logging.INFO,
-    "WARNING": logging.WARNING,
-    "ERROR": logging.ERROR,
-    "CRITICAL": logging.CRITICAL,
-}
-
-# 默认的日志格式
-datefmt_classic = "%Y-%m-%d %H:%M:%S"
-fmt_classic = '%(asctime)s.%(msecs)03d UTC %(levelname)s %(name)s: %(message)s'
-
-
-# 装饰器，自动获取函数的name参数，如果是文件路径，则自动提取文件名作为logger的name
-def auto_logger_name(func):
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        kwargs_new = func_args2kwargs(func, *args, **kwargs)
-        name = kwargs_new.get("name", "Logger")
-        if os.path.exists(name):
-            name = os.path.splitext(os.path.basename(name))[0]
-        return name
-
-    return wrapper
-
-
-@auto_logger_name
-def getLogger(name="Logger", level=None, isNamePath=True):
-    level = logging.INFO if level is None else level
-    name = os.path.splitext(os.path.basename(name))[0] if isNamePath else name
-    logger = logging.getLogger(name)
-    logger.setLevel(level_dict.get(level, logging.DEBUG))
-    return logger
-
-
-@auto_logger_name
-def create_stream_logger(name="Logger", log_level=logging.INFO):
-    formatter = logging.Formatter(fmt=fmt_classic, datefmt=datefmt_classic)
-    handler = logging.StreamHandler()
-    handler.setFormatter(formatter)
-    logger = logging.getLogger(name)
-    logger.setLevel(log_level)
-    logger.addHandler(handler)
-    return logger
-
-
-@auto_logger_name
-def create_file_logger(name, filename, log_level=logging.INFO):
-    logger = logging.getLogger(name)
-    logger.setLevel(log_level)
-    formatter = logging.Formatter(fmt=fmt_classic, datefmt=datefmt_classic)
-    handler = logging.FileHandler(filename, mode='a', encoding=None, delay=False)
-    handler.setFormatter(formatter)
-    logger.addHandler(handler)
-    handler = logging.StreamHandler()
-    handler.setFormatter(formatter)
-    logger.addHandler(handler)
-    return logger
-
-
-# logging.basicConfig(level=logging.INFO,
-#                     format=fmt_classic,
+import os
+import logging
+from functools import wraps
+from .functool import func_args2kwargs
+
+level_dict = {
+    "DEBUG": logging.DEBUG,
+    "INFO": logging.INFO,
+    "WARNING": logging.WARNING,
+    "ERROR": logging.ERROR,
+    "CRITICAL": logging.CRITICAL,
+}
+
+# 默认的日志格式
+datefmt_classic = "%Y-%m-%d %H:%M:%S"
+fmt_classic = '%(asctime)s.%(msecs)03d UTC %(levelname)s %(name)s: %(message)s'
+
+
+# 装饰器，自动获取函数的name参数，如果是文件路径，则自动提取文件名作为logger的name
+def auto_logger_name(func):
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        kwargs_new = func_args2kwargs(func, *args, **kwargs)
+        name = kwargs_new.get("name", "Logger")
+        if os.path.exists(name):
+            name = os.path.splitext(os.path.basename(name))[0]
+        return name
+
+    return wrapper
+
+
+def getLogger(name="Logger", level=None, isNamePath=True):
+    level = logging.INFO if level is None else level
+    name = os.path.splitext(os.path.basename(name))[0] if isNamePath else name
+    logger = logging.getLogger(name)
+    logger.setLevel(level_dict.get(level, logging.DEBUG))
+    return logger
+
+
+def create_stream_logger(name="Logger", log_level=logging.INFO):
+    formatter = logging.Formatter(fmt=fmt_classic, datefmt=datefmt_classic)
+    handler = logging.StreamHandler()
+    handler.setFormatter(formatter)
+    logger = logging.getLogger(name)
+    logger.setLevel(log_level)
+    logger.addHandler(handler)
+    return logger
+
+
+def create_file_logger(name, filename, log_level=logging.INFO):
+    logger = logging.getLogger(name)
+    logger.setLevel(log_level)
+    formatter = logging.Formatter(fmt=fmt_classic, datefmt=datefmt_classic)
+    handler = logging.FileHandler(filename, mode='a', encoding=None, delay=False)
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
+    handler = logging.StreamHandler()
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
+    return logger
+
+
+# logging.basicConfig(level=logging.INFO,
+#                     format=fmt_classic,
 #                     datefmt=datefmt_classic)
```

### Comparing `mtmtool-1.1.2/src/mtmtool/pool.py` & `mtmtool-1.2.3/src/mtmtool/pool.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from functools import partial
-from itertools import product
-from multiprocessing import Pool
-from multiprocessing.pool import ThreadPool
-import os
-
-CPUNUM = os.cpu_count() - 2
-
-
-def parfunc(func, *args, **kargs):
-    return partial(func, *args, **kargs)
-
-
-""" 
-map 与 starmap 函数的区别:
-    map只展开一次, 只能向函数掺入一个参数
-    starmap可展开两次, 可以向函数传入多个参数
-product 函数:
-    输入多个可迭代参数, 返回所有笛卡尔积元组
-"""
-def pool_process(par_func, iterables, worker_num=CPUNUM):
-    with Pool(worker_num) as p:
-        res_list = p.map(par_func, iterables)
-    return res_list
-
-
-def pool_thread(par_func, iterables, worker_num=CPUNUM):
-    with ThreadPool(worker_num) as p:
-        res_list = p.map(par_func, iterables)
-    return res_list
-
-
-def starmap(func, *args, is_test=False, worker_num=None, ptype="Process"):
-    """输入args必须可迭代
-    usage:
-        >>> result = starmap(pow, [10,15], [3,5], worker_num=4, ptype="Thread")
-        >>> result
-        [1000, 100000, 3375, 759375]
-    """
-    iters = product(*args)
-    pool = Pool if ptype == "Process" else ThreadPool
-    worker_num = CPUNUM if worker_num is None else worker_num
-    if is_test:
-        res = []
-        for args_t in iters:
-            res.append(func(*args_t))
-    else:
-        with pool(worker_num) as p:
-            res = p.starmap(func, iters)
-    return res
+from functools import partial
+from itertools import product
+from multiprocessing import Pool
+from multiprocessing.pool import ThreadPool
+import os
+
+CPUNUM = os.cpu_count() - 2
+
+
+def parfunc(func, *args, **kargs):
+    return partial(func, *args, **kargs)
+
+
+""" 
+map 与 starmap 函数的区别:
+    map只展开一次, 只能向函数掺入一个参数
+    starmap可展开两次, 可以向函数传入多个参数
+product 函数:
+    输入多个可迭代参数, 返回所有笛卡尔积元组
+"""
+def pool_process(par_func, iterables, worker_num=CPUNUM):
+    with Pool(worker_num) as p:
+        res_list = p.map(par_func, iterables)
+    return res_list
+
+
+def pool_thread(par_func, iterables, worker_num=CPUNUM):
+    with ThreadPool(worker_num) as p:
+        res_list = p.map(par_func, iterables)
+    return res_list
+
+
+def starmap(func, *args, is_test=False, worker_num=None, ptype="Process"):
+    """输入args必须可迭代
+    usage:
+        >>> result = starmap(pow, [10,15], [3,5], worker_num=4, ptype="Thread")
+        >>> result
+        [1000, 100000, 3375, 759375]
+    """
+    iters = product(*args)
+    pool = Pool if ptype == "Process" else ThreadPool
+    worker_num = CPUNUM if worker_num is None else worker_num
+    if is_test:
+        res = []
+        for args_t in iters:
+            res.append(func(*args_t))
+    else:
+        with pool(worker_num) as p:
+            res = p.starmap(func, iters)
+    return res
```

### Comparing `mtmtool-1.1.2/src/mtmtool/projection.py` & `mtmtool-1.2.3/src/mtmtool/projection.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-"""
-参数含义定义：
-    地理坐标参数为lat(南北向, 北为正), lon(东西向, 东为正)。
-    大地坐标参数为X(东西向, 东为正), Y(南北向, 北为正)。
-    矩阵行列参数为row(南北向, 南为正), col(东西向, 东为正)
-    x(东西向), y(南北向); (GDAL同样)
-仿射变换六参数:
-    0：图像左上角的X坐标(东西向)或lon坐标(东西向)；
-    1：图像东西方向分辨率；
-    2：旋转角度，如果图像北方朝上，该值为0；
-    3：图像左上角的Y坐标(南北向)或lat坐标(南北向)；
-    4：旋转角度，如果图像北方朝上，该值为0；
-    5：图像南北方向分辨率；
-"""
-
-def XYcoord2Plines(coordinate, affine_trans):
-    """投影坐标下XY坐标转像素行列位置
-
-    Args:
-        coordinate: (X, Y)   经纬度或大地坐标->(东西向, 南北向)
-        affine_trans (list): 仿射变换六参数
-    
-    Returns:
-        tuple: 数据矩阵的行号,列号
-        
-    Note: 由于左上角点中心位置为 (0.5,0.5)，故直接int就可以取值
-    """
-    X, Y = coordinate
-    x0, dx, rx, y0, ry, dy = affine_trans
-    a = X - x0
-    b = Y - y0
-    c = (dx * dy - ry * rx)
-    # 注意, 左上角点中心位置为 (0.5,0.5)
-    col = (a * dy - b * rx) / c
-    row = (b * dx - a * ry) / c
-    return row, col
-
-
-def Plines2XYcoord(rasterXYPixel, affine_trans):
-    """像素行列位置转投影坐标下XY坐标
-
-    Args:
-        rasterXYPixel (tuple): 数据矩阵的行列号->(南北向, 东西向)
-        affine_trans (list): 仿射变换六参数
-    
-    Returns:
-        tuple: (X, Y)   东西向, 南北向
-    """
-    col = rasterXYPixel[1] # 东西向
-    row = rasterXYPixel[0] # 南北向
-    # 获得东西向结果
-    lon = X = affine_trans[0] + affine_trans[1] * col + affine_trans[2] * row
-    # 获得南北向结果
-    lat = Y = affine_trans[3] + affine_trans[4] * col + affine_trans[5] * row
-    return [X, Y]
-
-def destination(point, bearing, distance:float):
-    """
-        lat, lon
-    """
-    try:
-        import geopy.distance
-    except:
-        raise Exception("导入geopy失败，请先安装")
-    return geopy.distance.distance(kilometers=distance).destination(point, bearing=bearing)
-    
-
-def toOrientationEN(sr, point):
-    """
-        北为1， 东为3
-    """
-    orient = [sr.GetAxisOrientation(None, i) for i in range(2)]
-    if orient == [3, 1]:
-        return point[:2]
-    if orient == [1, 3]:
-        return reversed(point[:2])
-    raise ValueError("ERROR: toOrientationEN: 特殊的投影坐标系，请检查!")
-
-def bounding(datarange, brange):
-    row_min_1, row_max_1, col_min_1, col_max_1 = [int(i) for i in datarange]
-    row_min_2, row_max_2, col_min_2, col_max_2 = [int(i) for i in brange]
-
-    row_min_3 = row_min_1 if row_min_1 >= row_min_2 else row_min_2
-    row_max_3 = row_max_1 if row_max_1 < row_max_2 else row_max_2 - 1
-    col_min_3 = col_min_1 if col_min_1 >= col_min_2 else col_min_2
-    col_max_3 = col_max_1 if col_max_1 < col_max_2 else col_max_2 - 1
-    width_from_data = col_max_3 - col_min_3 + 1
-    height_from_data = row_max_3 - row_min_3 + 1
-
-    row_min_array = row_min_3 - row_min_1
-    row_max_array = row_max_3 - row_min_1
-    col_min_array = col_min_3 - col_min_1
-    col_max_array = col_max_3 - col_min_1
-        
-
-    bounding_range = (row_min_3, row_max_3, col_min_3, col_max_3)
-    data_get_setting = (col_min_3, row_min_3, width_from_data, height_from_data)
-    array_get_setting = (row_min_array, row_max_array+1, col_min_array, col_max_array+1)
-    return bounding_range, data_get_setting, array_get_setting
+"""
+参数含义定义：
+    地理坐标参数为lat(南北向, 北为正), lon(东西向, 东为正)。
+    大地坐标参数为X(东西向, 东为正), Y(南北向, 北为正)。
+    矩阵行列参数为row(南北向, 南为正), col(东西向, 东为正)
+    x(东西向), y(南北向); (GDAL同样)
+仿射变换六参数:
+    0：图像左上角的X坐标(东西向)或lon坐标(东西向)；
+    1：图像东西方向分辨率；
+    2：旋转角度，如果图像北方朝上，该值为0；
+    3：图像左上角的Y坐标(南北向)或lat坐标(南北向)；
+    4：旋转角度，如果图像北方朝上，该值为0；
+    5：图像南北方向分辨率；
+"""
+
+def XYcoord2Plines(coordinate, affine_trans):
+    """投影坐标下XY坐标转像素行列位置
+
+    Args:
+        coordinate: (X, Y)   经纬度或大地坐标->(东西向, 南北向)
+        affine_trans (list): 仿射变换六参数
+    
+    Returns:
+        tuple: 数据矩阵的行号,列号
+        
+    Note: 由于左上角点中心位置为 (0.5,0.5)，故直接int就可以取值
+    """
+    X, Y = coordinate
+    x0, dx, rx, y0, ry, dy = affine_trans
+    a = X - x0
+    b = Y - y0
+    c = (dx * dy - ry * rx)
+    # 注意, 左上角点中心位置为 (0.5,0.5)
+    col = (a * dy - b * rx) / c
+    row = (b * dx - a * ry) / c
+    return row, col
+
+
+def Plines2XYcoord(rasterXYPixel, affine_trans):
+    """像素行列位置转投影坐标下XY坐标
+
+    Args:
+        rasterXYPixel (tuple): 数据矩阵的行列号->(南北向, 东西向)
+        affine_trans (list): 仿射变换六参数
+    
+    Returns:
+        tuple: (X, Y)   东西向, 南北向
+    """
+    col = rasterXYPixel[1] # 东西向
+    row = rasterXYPixel[0] # 南北向
+    # 获得东西向结果
+    lon = X = affine_trans[0] + affine_trans[1] * col + affine_trans[2] * row
+    # 获得南北向结果
+    lat = Y = affine_trans[3] + affine_trans[4] * col + affine_trans[5] * row
+    return [X, Y]
+
+def destination(point, bearing, distance:float):
+    """
+        lat, lon
+    """
+    try:
+        import geopy.distance
+    except:
+        raise Exception("导入geopy失败，请先安装")
+    return geopy.distance.distance(kilometers=distance).destination(point, bearing=bearing)
+    
+
+def toOrientationEN(sr, point):
+    """
+        北为1， 东为3
+    """
+    orient = [sr.GetAxisOrientation(None, i) for i in range(2)]
+    if orient == [3, 1]:
+        return point[:2]
+    if orient == [1, 3]:
+        return reversed(point[:2])
+    raise ValueError("ERROR: toOrientationEN: 特殊的投影坐标系，请检查!")
+
+def bounding(datarange, brange):
+    row_min_1, row_max_1, col_min_1, col_max_1 = [int(i) for i in datarange]
+    row_min_2, row_max_2, col_min_2, col_max_2 = [int(i) for i in brange]
+
+    row_min_3 = row_min_1 if row_min_1 >= row_min_2 else row_min_2
+    row_max_3 = row_max_1 if row_max_1 < row_max_2 else row_max_2 - 1
+    col_min_3 = col_min_1 if col_min_1 >= col_min_2 else col_min_2
+    col_max_3 = col_max_1 if col_max_1 < col_max_2 else col_max_2 - 1
+    width_from_data = col_max_3 - col_min_3 + 1
+    height_from_data = row_max_3 - row_min_3 + 1
+
+    row_min_array = row_min_3 - row_min_1
+    row_max_array = row_max_3 - row_min_1
+    col_min_array = col_min_3 - col_min_1
+    col_max_array = col_max_3 - col_min_1
+        
+
+    bounding_range = (row_min_3, row_max_3, col_min_3, col_max_3)
+    data_get_setting = (col_min_3, row_min_3, width_from_data, height_from_data)
+    array_get_setting = (row_min_array, row_max_array+1, col_min_array, col_max_array+1)
+    return bounding_range, data_get_setting, array_get_setting
```

### Comparing `mtmtool-1.1.2/src/mtmtool/time.py` & `mtmtool-1.2.3/src/mtmtool/time.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import time
-import datetime, calendar
-
-
-class sTime:
-    def __init__(self, srctime=None):
-        self.datetime = srctime
-
-    def __call__(self, srctime):
-        self.datetime = srctime
-        return self
-
-    def fromstr(self, timestr, format="%Y-%m-%d"):
-        self.datetime = datetime.datetime.strptime(timestr, format)
-        return self
-
-    def tostr(self, format="%Y-%m-%d"):
-        return self.datetime.strftime(format)
-
-    def last_month(self, objday=1):
-        self.datetime = (self.datetime.replace(day=1) - datetime.timedelta(days=1)).replace(day=objday)
-        return self
-
-    def next_month(self, objday=1):
-        week, days_num = calendar.monthrange(self.datetime.year, self.datetime.month)
-        self.datetime = (self.datetime.replace(day=days_num) + datetime.timedelta(days=1)).replace(day=objday)
-        return self
-
-    def next_day(self):
-        self.datetime = self.datetime + datetime.timedelta(days=1)
-        return self
-
-    def last_day(self):
-        self.datetime = self.datetime - datetime.timedelta(days=1)
-        return self
-
-
-def timestamp2timestr(timeStamp, format="%Y-%m-%d %H:%M:%S", isMicroSecond=True, isUtc=False):
-    time_function = time.gmtime if isUtc else time.localtime
-    return time.strftime(format, time_function(timeStamp / (1000 if isMicroSecond else 1)))
-
-
-def timestr2timestamp(timestr, format="%Y-%m-%d %H:%M:%S", isMicroSecond=True):
-    timeArray = time.strptime(timestr, format)
-    return int(time.mktime(timeArray)) * (1000 if isMicroSecond else 1)
-
-
+import time
+import datetime, calendar
+
+
+class sTime:
+    def __init__(self, srctime=None):
+        self.datetime = srctime
+
+    def __call__(self, srctime):
+        self.datetime = srctime
+        return self
+
+    def fromstr(self, timestr, format="%Y-%m-%d"):
+        self.datetime = datetime.datetime.strptime(timestr, format)
+        return self
+
+    def tostr(self, format="%Y-%m-%d"):
+        return self.datetime.strftime(format)
+
+    def last_month(self, objday=1):
+        self.datetime = (self.datetime.replace(day=1) - datetime.timedelta(days=1)).replace(day=objday)
+        return self
+
+    def next_month(self, objday=1):
+        week, days_num = calendar.monthrange(self.datetime.year, self.datetime.month)
+        self.datetime = (self.datetime.replace(day=days_num) + datetime.timedelta(days=1)).replace(day=objday)
+        return self
+
+    def next_day(self):
+        self.datetime = self.datetime + datetime.timedelta(days=1)
+        return self
+
+    def last_day(self):
+        self.datetime = self.datetime - datetime.timedelta(days=1)
+        return self
+
+
+def timestamp2timestr(timeStamp, format="%Y-%m-%d %H:%M:%S", isMicroSecond=True, isUtc=False):
+    time_function = time.gmtime if isUtc else time.localtime
+    return time.strftime(format, time_function(timeStamp / (1000 if isMicroSecond else 1)))
+
+
+def timestr2timestamp(timestr, format="%Y-%m-%d %H:%M:%S", isMicroSecond=True):
+    timeArray = time.strptime(timestr, format)
+    return int(time.mktime(timeArray)) * (1000 if isMicroSecond else 1)
+
+
 st = sTime()
```

### Comparing `mtmtool-1.1.2/src/mtmtool/webhook.py` & `mtmtool-1.2.3/src/mtmtool/webhook.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import requests
-import json
-
-
-def auto_send(message, *args, **kwargs):
-    if args[0].lower() == "telegram":
-        return telegram(message, *args[1:], **kwargs)
-    if args[0].lower() == "pushplus":
-        return pushplus(message, *args[1:], **kwargs)
-    if args[0].lower() == "wechat":
-        return wechat(message, *args[1:], **kwargs)
-    if args[0].lower() == "qq":
-        return qq(message, *args[1:], **kwargs)
-    raise ValueError(f"Not Support API Type {args[0]}")
-
-
-def dingding(text, key: str = ""):
-    url = 'https://oapi.dingtalk.com/robot/send?access_token=' + key
-    if ':' not in text and "." not in text and "," not in text and "。" not in text:
-        text += "."
-    data = {
-        "msgtype": "text",
-        "text": {
-            "content": text
-        },
-    }
-    headers = {"Content-Type": "application/json ;charset=utf-8 "}
-    html = requests.post(url, data=json.dumps(data), headers=headers)
-    return html.ok
-
-
-def wechat(text, key: str = ""):
-    url = 'https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=' + key
-    data = {
-        "msgtype": "text",
-        "text": {
-            "content": text
-        },
-    }
-    headers = {"Content-Type": "application/json ;charset=utf-8 "}
-    html = requests.post(url, data=json.dumps(data), headers=headers)
-    return html.ok
-
-
-def qq(text, key: str = ""):
-    url = "https://qmsg.zendee.cn/send/" + key
-    data = {'msg': text}
-    html = requests.post(url, data=data)
-    return html.ok
-
-
-def mi(text, key: str = "", title="bot"):
-    url = "https://tdtt.top/send"
-    data = {"title": title, "content": text, "alias": key}
-    response = requests.post(url, data=data)
-    return response.ok
-
-
-def telegram(text: str, bot: str, chat: str, protect_content=False):
-    bot_token = bot
-    chat_id = chat
-    url = f"https://api.telegram.org/bot{bot_token}/sendMessage"
-    data = {
-        "chat_id": chat_id,
-        "text": text,
-        "protect_content": protect_content,
-    }
-    res = requests.get(url, data=data)
-    return res.json()
-
-
-def pushplus(message, token, title="default", template="html"):
-    url = f'http://www.pushplus.plus/send?token={token}&title={title}&content={message}&template={template}'
-    resq = requests.get(url=url)
-    return resq.text
+import requests
+import json
+
+
+def auto_send(message, *args, **kwargs):
+    if args[0].lower() == "telegram":
+        return telegram(message, *args[1:], **kwargs)
+    if args[0].lower() == "pushplus":
+        return pushplus(message, *args[1:], **kwargs)
+    if args[0].lower() == "wechat":
+        return wechat(message, *args[1:], **kwargs)
+    if args[0].lower() == "qq":
+        return qq(message, *args[1:], **kwargs)
+    raise ValueError(f"Not Support API Type {args[0]}")
+
+
+def dingding(text, key: str = "", **kargs):
+    url = 'https://oapi.dingtalk.com/robot/send?access_token=' + key
+    if ':' not in text and "." not in text and "," not in text and "。" not in text:
+        text += "."
+    data = {
+        "msgtype": "text",
+        "text": {
+            "content": text
+        },
+    }
+    headers = {"Content-Type": "application/json ;charset=utf-8 "}
+    html = requests.post(url, data=json.dumps(data), headers=headers)
+    return html.ok
+
+
+def wechat(text, key: str = "", **kargs):
+    url = 'https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=' + key
+    data = {
+        "msgtype": "text",
+        "text": {
+            "content": text
+        },
+    }
+    headers = {"Content-Type": "application/json ;charset=utf-8 "}
+    html = requests.post(url, data=json.dumps(data), headers=headers)
+    return html.ok
+
+
+def qq(text, key: str = ""):
+    url = "https://qmsg.zendee.cn/send/" + key
+    data = {'msg': text}
+    html = requests.post(url, data=data)
+    return html.ok
+
+
+def mi(text, key: str = "", title="bot", **kargs):
+    url = "https://tdtt.top/send"
+    data = {"title": title, "content": text, "alias": key}
+    response = requests.post(url, data=data)
+    return response.ok
+
+
+def telegram(text: str, bot: str, chat: str, protect_content=False, host="api.telegram.org", **kargs):
+    bot_token = bot
+    chat_id = chat
+    url = f"https://{host}/bot{bot_token}/sendMessage"
+    data = {
+        "chat_id": chat_id,
+        "text": text,
+        "protect_content": protect_content,
+    }
+    res = requests.get(url, data=data)
+    return res.json()
+
+
+def pushplus(message, token, title="default", template="html", **kargs):
+    url = f'http://www.pushplus.plus/send?token={token}&title={title}&content={message}&template={template}'
+    resq = requests.get(url=url)
+    return resq.text
```

### Comparing `mtmtool-1.1.2/src/mtmtool.egg-info/PKG-INFO` & `mtmtool-1.2.3/src/mtmtool.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1
-Name: mtmtool
-Version: 1.1.2
-Summary:  A Personal Python Tool Library.
-Home-page: https://github.com/imutum/imutum_python_tool
-Author: imutum
-Author-email: 
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# mdfpytool
-
-A personal code tool
-
-个人使用的简单的Python代码片段
+Metadata-Version: 2.1
+Name: mtmtool
+Version: 1.2.3
+Summary:  A Personal Python Tool Library.
+Home-page: https://github.com/imutum/imutum_python_tool
+Author: imutum
+Author-email: 
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mdfpytool
+
+A personal code tool
+
+个人使用的简单的Python代码片段
```

### Comparing `mtmtool-1.1.2/test/test_args2kwargs.py` & `mtmtool-1.2.3/test/test_args2kwargs.py`

 * *Files identical despite different names*


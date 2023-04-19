# Comparing `tmp/cspyce-2.0.7.tar.gz` & `tmp/cspyce-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cspyce-2.0.7.tar", last modified: Thu Nov  3 18:17:56 2022, max compression
+gzip compressed data, was "cspyce-2.0.8.tar", last modified: Wed Apr 19 20:55:58 2023, max compression
```

## Comparing `cspyce-2.0.7.tar` & `cspyce-2.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 18:17:56.187257 cspyce-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)    10269 2022-11-03 18:17:24.000000 cspyce-2.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-03 18:17:24.000000 cspyce-2.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-11-03 18:17:56.187257 cspyce-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15050 2022-11-03 18:17:24.000000 cspyce-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 18:17:56.179257 cspyce-2.0.7/cspyce/
--rw-r--r--   0 runner    (1001) docker     (121)    10127 2022-11-03 18:17:24.000000 cspyce-2.0.7/cspyce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21355 2022-11-03 18:17:24.000000 cspyce-2.0.7/cspyce/alias_support.py
--rw-r--r--   0 runner    (1001) docker     (121)     4416 2022-11-03 18:17:24.000000 cspyce-2.0.7/cspyce/aliases.py
--rw-r--r--   0 runner    (1001) docker     (121)    14332 2022-11-03 18:17:24.000000 cspyce-2.0.7/cspyce/array_support.py
--rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-11-03 18:17:24.000000 cspyce-2.0.7/cspyce/arrays.py
--rw-r--r--   0 runner    (1001) docker     (121)   144839 2022-11-03 18:17:54.000000 cspyce-2.0.7/cspyce/cspyce0.py
--rw-r--r--   0 runner    (1001) docker     (121)   392081 2022-11-03 18:17:36.000000 cspyce-2.0.7/cspyce/cspyce0_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    44615 2022-11-03 18:17:24.000000 cspyce-2.0.7/cspyce/cspyce1.py
--rw-r--r--   0 runner    (1001) docker     (121)     7536 2022-11-03 18:17:24.000000 cspyce-2.0.7/cspyce/cspyce1_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     3258 2022-11-03 18:17:24.000000 cspyce-2.0.7/cspyce/cspyce2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4570 2022-11-03 18:17:55.000000 cspyce-2.0.7/cspyce/typemap_samples.py
--rw-r--r--   0 runner    (1001) docker     (121)    25919 2022-11-03 18:17:24.000000 cspyce-2.0.7/cspyce/typemap_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 18:17:56.183257 cspyce-2.0.7/cspyce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-11-03 18:17:55.000000 cspyce-2.0.7/cspyce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)   164695 2022-11-03 18:17:56.000000 cspyce-2.0.7/cspyce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 18:17:55.000000 cspyce-2.0.7/cspyce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-03 18:17:55.000000 cspyce-2.0.7/cspyce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-03 18:17:55.000000 cspyce-2.0.7/cspyce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5560 2022-11-03 18:17:24.000000 cspyce-2.0.7/get_spice.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-03 18:17:56.187257 cspyce-2.0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     4314 2022-11-03 18:17:24.000000 cspyce-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 18:17:56.187257 cspyce-2.0.7/swig/
--rw-r--r--   0 runner    (1001) docker     (121)  4108215 2022-11-03 18:17:54.000000 cspyce-2.0.7/swig/cspyce0_wrap.c
--rw-r--r--   0 runner    (1001) docker     (121)   220796 2022-11-03 18:17:55.000000 cspyce-2.0.7/swig/typemap_samples_wrap.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:55:58.505477 cspyce-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-04-19 20:55:42.000000 cspyce-2.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 20:55:42.000000 cspyce-2.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-19 20:55:58.505477 cspyce-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15641 2023-04-19 20:55:42.000000 cspyce-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:55:58.501477 cspyce-2.0.8/cspyce/
+-rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21684 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/alias_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/array_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144839 2023-04-19 20:55:57.000000 cspyce-2.0.8/cspyce/cspyce0.py
+-rw-r--r--   0 runner    (1001) docker     (123)   392102 2023-04-19 20:55:52.000000 cspyce-2.0.8/cspyce/cspyce0_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39226 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/cspyce1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/cspyce1_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/cspyce2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-19 20:55:58.000000 cspyce-2.0.8/cspyce/typemap_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25919 2023-04-19 20:55:42.000000 cspyce-2.0.8/cspyce/typemap_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:55:58.501477 cspyce-2.0.8/cspyce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-19 20:55:58.000000 cspyce-2.0.8/cspyce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   164695 2023-04-19 20:55:58.000000 cspyce-2.0.8/cspyce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:55:58.000000 cspyce-2.0.8/cspyce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 20:55:58.000000 cspyce-2.0.8/cspyce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 20:55:58.000000 cspyce-2.0.8/cspyce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-19 20:55:42.000000 cspyce-2.0.8/get_spice.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:55:58.505477 cspyce-2.0.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4167 2023-04-19 20:55:42.000000 cspyce-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:55:58.505477 cspyce-2.0.8/swig/
+-rw-r--r--   0 runner    (1001) docker     (123)  4109483 2023-04-19 20:55:57.000000 cspyce-2.0.8/swig/cspyce0_wrap.c
+-rw-r--r--   0 runner    (1001) docker     (123)   222160 2023-04-19 20:55:58.000000 cspyce-2.0.8/swig/typemap_samples_wrap.c
```

### Comparing `cspyce-2.0.7/LICENSE.txt` & `cspyce-2.0.8/LICENSE.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,186 @@
 Academic Free License ("AFL") v. 3.0
 
-This Academic Free License (the "License") applies to any original work of authorship (the "Original Work") whose owner (the "Licensor") has placed the following licensing notice adjacent to the copyright notice for the Original Work:
+This Academic Free License (the "License") applies to any original
+work of authorship (the "Original Work") whose owner (the "Licensor")
+has placed the following licensing notice adjacent to the copyright
+notice for the Original Work:
 
 Licensed under the Academic Free License version 3.0
 
-1) Grant of Copyright License. Licensor grants You a worldwide, royalty-free, non-exclusive, sublicensable license, for the duration of the copyright, to do the following:
-a) to reproduce the Original Work in copies, either alone or as part of a collective work;
-b) to translate, adapt, alter, transform, modify, or arrange the Original Work, thereby creating derivative works ("Derivative Works") based upon the Original Work;
-c) to distribute or communicate copies of the Original Work and Derivative Works to the public, under any license of your choice that does not contradict the terms and conditions, including Licensor's reserved rights and remedies, in this Academic Free License;
+1) Grant of Copyright License. Licensor grants You a worldwide,
+royalty-free, non-exclusive, sublicensable license, for the duration
+of the copyright, to do the following:
+
+a) to reproduce the Original Work in copies, either alone or as part
+of a collective work;
+
+b) to translate, adapt, alter, transform, modify, or arrange the
+Original Work, thereby creating derivative works ("Derivative Works")
+based upon the Original Work;
+
+c) to distribute or communicate copies of the Original Work and
+Derivative Works to the public, under any license of your choice that
+does not contradict the terms and conditions, including Licensor's
+reserved rights and remedies, in this Academic Free License;
+
 d) to perform the Original Work publicly; and
+
 e) to display the Original Work publicly.
-2) Grant of Patent License. Licensor grants You a worldwide, royalty-free, non-exclusive, sublicensable license, under patent claims owned or controlled by the Licensor that are embodied in the Original Work as furnished by the Licensor, for the duration of the patents, to make, use, sell, offer for sale, have made, and import the Original Work and Derivative Works.
-3) Grant of Source Code License. The term "Source Code" means the preferred form of the Original Work for making modifications to it and all available documentation describing how to modify the Original Work. Licensor agrees to provide a machine-readable copy of the Source Code of the Original Work along with each copy of the Original Work that Licensor distributes. Licensor reserves the right to satisfy this obligation by placing a machine-readable copy of the Source Code in an information repository reasonably calculated to permit inexpensive and convenient access by You for as long as Licensor continues to distribute the Original Work.
-4) Exclusions From License Grant. Neither the names of Licensor, nor the names of any contributors to the Original Work, nor any of their trademarks or service marks, may be used to endorse or promote products derived from this Original Work without express prior permission of the Licensor. Except as expressly stated herein, nothing in this License grants any license to Licensor's trademarks, copyrights, patents, trade secrets or any other intellectual property. No patent license is granted to make, use, sell, offer for sale, have made, or import embodiments of any patent claims other than the licensed claims defined in Section 2. No license is granted to the trademarks of Licensor even if such marks are included in the Original Work. Nothing in this License shall be interpreted to prohibit Licensor from licensing under terms different from this License any Original Work that Licensor otherwise would have a right to license.
-5) External Deployment. The term "External Deployment" means the use, distribution, or communication of the Original Work or Derivative Works in any way such that the Original Work or Derivative Works may be used by anyone other than You, whether those works are distributed or communicated to those persons or made available as an application intended for use over a network. As an express condition for the grants of license hereunder, You must treat any External Deployment by You of the Original Work or a Derivative Work as a distribution under section 1(c).
-6) Attribution Rights. You must retain, in the Source Code of any Derivative Works that You create, all copyright, patent, or trademark notices from the Source Code of the Original Work, as well as any notices of licensing and any descriptive text identified therein as an "Attribution Notice." You must cause the Source Code for any Derivative Works that You create to carry a prominent Attribution Notice reasonably calculated to inform recipients that You have modified the Original Work.
-7) Warranty of Provenance and Disclaimer of Warranty. Licensor warrants that the copyright in and to the Original Work and the patent rights granted herein by Licensor are owned by the Licensor or are sublicensed to You under the terms of this License with the permission of the contributor(s) of those copyrights and patent rights. Except as expressly stated in the immediately preceding sentence, the Original Work is provided under this License on an "AS IS" BASIS and WITHOUT WARRANTY, either express or implied, including, without limitation, the warranties of non-infringement, merchantability or fitness for a particular purpose. THE ENTIRE RISK AS TO THE QUALITY OF THE ORIGINAL WORK IS WITH YOU. This DISCLAIMER OF WARRANTY constitutes an essential part of this License. No license to the Original Work is granted by this License except under this disclaimer.
-8) Limitation of Liability. Under no circumstances and under no legal theory, whether in tort (including negligence), contract, or otherwise, shall the Licensor be liable to anyone for any indirect, special, incidental, or consequential damages of any character arising as a result of this License or the use of the Original Work including, without limitation, damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses. This limitation of liability shall not apply to the extent applicable law prohibits such limitation.
-9) Acceptance and Termination. If, at any time, You expressly assented to this License, that assent indicates your clear and irrevocable acceptance of this License and all of its terms and conditions. If You distribute or communicate copies of the Original Work or a Derivative Work, You must make a reasonable effort under the circumstances to obtain the express assent of recipients to the terms of this License. This License conditions your rights to undertake the activities listed in Section 1, including your right to create Derivative Works based upon the Original Work, and doing so without honoring these terms and conditions is prohibited by copyright law and international treaty. Nothing in this License is intended to affect copyright exceptions and limitations (including "fair use" or "fair dealing"). This License shall terminate immediately and You may no longer exercise any of the rights granted to You by this License upon your failure to honor the conditions in Section 1(c).
-10) Termination for Patent Action. This License shall terminate automatically and You may no longer exercise any of the rights granted to You by this License as of the date You commence an action, including a cross-claim or counterclaim, against Licensor or any licensee alleging that the Original Work infringes a patent. This termination provision shall not apply for an action alleging patent infringement by combinations of the Original Work with other software or hardware.
-11) Jurisdiction, Venue and Governing Law. Any action or suit relating to this License may be brought only in the courts of a jurisdiction wherein the Licensor resides or in which Licensor conducts its primary business, and under the laws of that jurisdiction excluding its conflict-of-law provisions. The application of the United Nations Convention on Contracts for the International Sale of Goods is expressly excluded. Any use of the Original Work outside the scope of this License or after its termination shall be subject to the requirements and penalties of copyright or patent law in the appropriate jurisdiction. This section shall survive the termination of this License.
-12) Attorneys' Fees. In any action to enforce the terms of this License or seeking damages relating thereto, the prevailing party shall be entitled to recover its costs and expenses, including, without limitation, reasonable attorneys' fees and costs incurred in connection with such action, including any appeal of such action. This section shall survive the termination of this License.
-13) Miscellaneous. If any provision of this License is held to be unenforceable, such provision shall be reformed only to the extent necessary to make it enforceable.
-14) Definition of "You" in This License. "You" throughout this License, whether in upper or lower case, means an individual or a legal entity exercising rights under, and complying with all of the terms of, this License. For legal entities, "You" includes any entity that controls, is controlled by, or is under common control with you. For purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
-15) Right to Use. You may use the Original Work in all ways not otherwise restricted or conditioned by this License or by law, and Licensor promises not to interfere with or be responsible for such uses by You.
-16) Modification of This License. This License is Copyright © 2005 Lawrence Rosen. Permission is granted to copy, distribute, or communicate this License without modification. Nothing in this License permits You to modify this License as applied to the Original Work or to Derivative Works. However, You may modify the text of this License and copy, distribute or communicate your modified version (the "Modified License") and apply it to other original works of authorship subject to the following conditions: (i) You may not indicate in any way that your Modified License is the "Academic Free License" or "AFL" and you may not use those names in the name of your Modified License; (ii) You must replace the notice specified in the first paragraph above with the notice "Licensed under <insert your license name here>" or with a notice of your own that is not confusingly similar to the notice in this License; and (iii) You may not claim that your original works are open source software unless your Modified License has been approved by Open Source Initiative (OSI) and You comply with its license review and certification process.
+
+2) Grant of Patent License. Licensor grants You a worldwide,
+royalty-free, non-exclusive, sublicensable license, under patent
+claims owned or controlled by the Licensor that are embodied in the
+Original Work as furnished by the Licensor, for the duration of the
+patents, to make, use, sell, offer for sale, have made, and import the
+Original Work and Derivative Works.
+
+3) Grant of Source Code License. The term "Source Code" means the
+preferred form of the Original Work for making modifications to it and
+all available documentation describing how to modify the Original
+Work. Licensor agrees to provide a machine-readable copy of the Source
+Code of the Original Work along with each copy of the Original Work
+that Licensor distributes. Licensor reserves the right to satisfy this
+obligation by placing a machine-readable copy of the Source Code in an
+information repository reasonably calculated to permit inexpensive and
+convenient access by You for as long as Licensor continues to
+distribute the Original Work.
+
+4) Exclusions From License Grant. Neither the names of Licensor, nor
+the names of any contributors to the Original Work, nor any of their
+trademarks or service marks, may be used to endorse or promote
+products derived from this Original Work without express prior
+permission of the Licensor. Except as expressly stated herein, nothing
+in this License grants any license to Licensor's trademarks,
+copyrights, patents, trade secrets or any other intellectual
+property. No patent license is granted to make, use, sell, offer for
+sale, have made, or import embodiments of any patent claims other than
+the licensed claims defined in Section 2. No license is granted to the
+trademarks of Licensor even if such marks are included in the Original
+Work. Nothing in this License shall be interpreted to prohibit
+Licensor from licensing under terms different from this License any
+Original Work that Licensor otherwise would have a right to license.
+
+5) External Deployment. The term "External Deployment" means the use,
+distribution, or communication of the Original Work or Derivative
+Works in any way such that the Original Work or Derivative Works may
+be used by anyone other than You, whether those works are distributed
+or communicated to those persons or made available as an application
+intended for use over a network. As an express condition for the
+grants of license hereunder, You must treat any External Deployment by
+You of the Original Work or a Derivative Work as a distribution under
+section 1(c).
+
+6) Attribution Rights. You must retain, in the Source Code of any
+Derivative Works that You create, all copyright, patent, or trademark
+notices from the Source Code of the Original Work, as well as any
+notices of licensing and any descriptive text identified therein as an
+"Attribution Notice." You must cause the Source Code for any
+Derivative Works that You create to carry a prominent Attribution
+Notice reasonably calculated to inform recipients that You have
+modified the Original Work.
+
+7) Warranty of Provenance and Disclaimer of Warranty. Licensor
+warrants that the copyright in and to the Original Work and the patent
+rights granted herein by Licensor are owned by the Licensor or are
+sublicensed to You under the terms of this License with the permission
+of the contributor(s) of those copyrights and patent rights. Except as
+expressly stated in the immediately preceding sentence, the Original
+Work is provided under this License on an "AS IS" BASIS and WITHOUT
+WARRANTY, either express or implied, including, without limitation,
+the warranties of non-infringement, merchantability or fitness for a
+particular purpose. THE ENTIRE RISK AS TO THE QUALITY OF THE ORIGINAL
+WORK IS WITH YOU. This DISCLAIMER OF WARRANTY constitutes an essential
+part of this License. No license to the Original Work is granted by
+this License except under this disclaimer.
+
+8) Limitation of Liability. Under no circumstances and under no legal
+theory, whether in tort (including negligence), contract, or
+otherwise, shall the Licensor be liable to anyone for any indirect,
+special, incidental, or consequential damages of any character arising
+as a result of this License or the use of the Original Work including,
+without limitation, damages for loss of goodwill, work stoppage,
+computer failure or malfunction, or any and all other commercial
+damages or losses. This limitation of liability shall not apply to the
+extent applicable law prohibits such limitation.
+
+9) Acceptance and Termination. If, at any time, You expressly assented
+to this License, that assent indicates your clear and irrevocable
+acceptance of this License and all of its terms and conditions. If You
+distribute or communicate copies of the Original Work or a Derivative
+Work, You must make a reasonable effort under the circumstances to
+obtain the express assent of recipients to the terms of this
+License. This License conditions your rights to undertake the
+activities listed in Section 1, including your right to create
+Derivative Works based upon the Original Work, and doing so without
+honoring these terms and conditions is prohibited by copyright law and
+international treaty. Nothing in this License is intended to affect
+copyright exceptions and limitations (including "fair use" or "fair
+dealing"). This License shall terminate immediately and You may no
+longer exercise any of the rights granted to You by this License upon
+your failure to honor the conditions in Section 1(c).
+
+10) Termination for Patent Action. This License shall terminate
+automatically and You may no longer exercise any of the rights granted
+to You by this License as of the date You commence an action,
+including a cross-claim or counterclaim, against Licensor or any
+licensee alleging that the Original Work infringes a patent. This
+termination provision shall not apply for an action alleging patent
+infringement by combinations of the Original Work with other software
+or hardware.
+
+11) Jurisdiction, Venue and Governing Law. Any action or suit relating
+to this License may be brought only in the courts of a jurisdiction
+wherein the Licensor resides or in which Licensor conducts its primary
+business, and under the laws of that jurisdiction excluding its
+conflict-of-law provisions. The application of the United Nations
+Convention on Contracts for the International Sale of Goods is
+expressly excluded. Any use of the Original Work outside the scope of
+this License or after its termination shall be subject to the
+requirements and penalties of copyright or patent law in the
+appropriate jurisdiction. This section shall survive the termination
+of this License.
+
+12) Attorneys' Fees. In any action to enforce the terms of this
+License or seeking damages relating thereto, the prevailing party
+shall be entitled to recover its costs and expenses, including,
+without limitation, reasonable attorneys' fees and costs incurred in
+connection with such action, including any appeal of such action. This
+section shall survive the termination of this License.
+
+13) Miscellaneous. If any provision of this License is held to be
+unenforceable, such provision shall be reformed only to the extent
+necessary to make it enforceable.
+
+14) Definition of "You" in This License. "You" throughout this
+License, whether in upper or lower case, means an individual or a
+legal entity exercising rights under, and complying with all of the
+terms of, this License. For legal entities, "You" includes any entity
+that controls, is controlled by, or is under common control with
+you. For purposes of this definition, "control" means (i) the power,
+direct or indirect, to cause the direction or management of such
+entity, whether by contract or otherwise, or (ii) ownership of fifty
+percent (50%) or more of the outstanding shares, or (iii) beneficial
+ownership of such entity.
+
+15) Right to Use. You may use the Original Work in all ways not
+otherwise restricted or conditioned by this License or by law, and
+Licensor promises not to interfere with or be responsible for such
+uses by You.
+
+16) Modification of This License. This License is Copyright © 2005
+Lawrence Rosen. Permission is granted to copy, distribute, or
+communicate this License without modification. Nothing in this License
+permits You to modify this License as applied to the Original Work or
+to Derivative Works. However, You may modify the text of this License
+and copy, distribute or communicate your modified version (the
+"Modified License") and apply it to other original works of authorship
+subject to the following conditions: (i) You may not indicate in any
+way that your Modified License is the "Academic Free License" or "AFL"
+and you may not use those names in the name of your Modified License;
+(ii) You must replace the notice specified in the first paragraph
+above with the notice "Licensed under <insert your license name here>"
+or with a notice of your own that is not confusingly similar to the
+notice in this License; and (iii) You may not claim that your original
+works are open source software unless your Modified License has been
+approved by Open Source Initiative (OSI) and You comply with its
+license review and certification process.
```

### Comparing `cspyce-2.0.7/README.md` & `cspyce-2.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # `cspyce` MODULE OVERVIEW
 Version 2.0
 
 March, 2022
 
 Mark Showalter, PDS Ring-Moon Systems Node, SETI Institute
 
-Spyce is a Python module that provides an interface to the CSPICE library. It
-implements the most widely-used functions of CSPICE in a Python-like way. It
-also supports numerous enhancements, including support for Python exceptions,
-array inputs, and aliases.
+`cspyce` is a Python module that provides an interface to the C-language CSPICE
+library produced by the Navigation and Ancillary Information Facility
+([NAIF](https://naif.jpl.nasa.gov/naif/)) of NASA's Planetary Data System (PDS).
+It implements the most widely-used functions of CSPICE in a Python-like way,
+while also supporting numerous enhancements, including support for Python
+exceptions, array inputs, and aliases.
 
 If you are looking for information on running or distributing this code from
-the github sources, look at the file `README-developers.md` in this directory.
+the GitHub sources, look at the file `README-developers.md` in this directory.
 
 ## PYTHONIZATION
 
-This module has been designed to replicate the core features of CSPICE for
+`cspyce` has been designed to replicate the core features of CSPICE for
 users who wish to translate a program that already exists. Function names in
 `cspyce` match their CSPICE names.
 
 However, it is also designed to behave as much as possible like a normal
 Python module. To that end, it has the following features.
 
 - The C language requires buffers to be allocated for output and it requires
-  array sizes to be include for both input and output. The `cspyce` module,
+  array sizes to be included for both input and output. The `cspyce` module,
   instead, eliminates all extraneous inputs, and all output arguments are
   returned as a list (or as a single object if the function only returns one
   item).
 
-- The module has been fully integrated with Python's exception handling,
+- `cspyce` has been fully integrated with Python's exception handling;
   programmers can still opt to use CSPICE's error handling mechanism if they
   wish to.
 
 - All `cspyce` functions can handle positional arguments as well as arguments
   passed by name.
 
 - All `cspyce` functions have informative docstrings, so typing
-      help(function)
-  provides useful information.
+  `help(function)` provides useful information.
 
 - Many `cspyce` functions take sensible default values if input arguments are
   omitted.
 
 - The CSPICE concepts of "windows" and "cells" are not needed in Python. In
   CSPICE, these allow a function to return a variable amount of information,
   which the program can then iterate through. The `cspyce` counterpart of each of
@@ -67,280 +68,284 @@
 
 - Whether to allow `cspyce` to support aliases, in which the same body or frame
   is associated with alternative names or IDs.
 
 ---
 ## EXCEPTION HANDLING
 
-As in CSPICE, the user can designate what to do in the event of an error
-condition using function erract(). In CSPICE, those options are "RETURN",
-"REPORT", "IGNORE", "ABORT", and "DEFAULT". This function adds new options
-"EXCEPTION" and "RUNTIME" to the suite of error handling options supported by
-CPICE.
+In CSPICE, the user can designate what to do in the event of an error condition
+using the function `erract()`. In CSPICE, the available options are "RETURN",
+"REPORT", "IGNORE", "ABORT", and "DEFAULT". The `cspyce` version of this
+function adds new options "EXCEPTION" and "RUNTIME" to the suite of error
+handling options supported by CSPICE.
 
 - As usual, the user can select the exception handling mechanism to use by
   calling the function erract(). In `cspyce`, the default is "EXCEPTION".
 
-- When using one of CSPICE's error handling methods, a call to failed() will
-  reveal whethen an error has occurred, and a call to reset() is needed to
-  clear the error.
-
-- Care has been taken to reduce the chances that the "dangerous" options
-  "IGNORE" and "REPORT" will cause a segmentation fault. However, this
-  possibility cannot be entirely ruled out, so caution is advised.
-
-- Because it would be a highly questionable thing to do, the "ABORT" and
-  "DEFAULT" options are overridden by "EXCEPTION" when the user is running
-  `cspyce` from an interactive shell. However, they resume their standard effects
-  during non-interactive runs.
-
 - When using the "EXCEPTION" option, each CSPICE error condition raises a
-  Python exception rather than setting the failed() flag. The exception
+  Python exception rather than setting the `failed()` flag. The exception
   contains the text of the CSPICE error, in the form (short message + " -- " +
-  long message).
-
-- The CSPICE error conditions are mapped to standard Python exception types in
-  a sensible way:
-  - KeyError indicates that a SPICE ID or name is unrecognized.
-  - ValueError indicates that one of the inputs to a function had an invalid
+  long message). The CSPICE error conditions are mapped to standard Python
+  exception types in a sensible way:
+  - `KeyError` indicates that a SPICE ID or name is unrecognized.
+  - `ValueError` indicates that one of the inputs to a function had an invalid
     value.
-  - TypeError indicates that one of the inputs to a function had an invalid
+  - `TypeError` indicates that one of the inputs to a function had an invalid
     type.
-  - IndexError indicates that an integer index is out of range.
-  - IOError indicates errors with reading and writing files, including SPICE
+  - `IndexError` indicates that an integer index is out of range.
+  - `IOError` indicates errors with reading and writing files, including SPICE
     kernels. IOError can also indicate that needed information was not in one
     of the furnished kernels.
-  - MemoryError indicates that adequate memory could not be allocated, or
+  - `MemoryError` indicates that adequate memory could not be allocated, or
     that the defined size of a memory buffer in C is too small.
-  - ZeroDivisionError indicates that a divide-by-zero has occurred.
-  - RuntimeError indicates that an action is incompatible with some aspect
+  - `ZeroDivisionError` indicates that a divide-by-zero has occurred.
+  - `RuntimeError` indicates that an action is incompatible with some aspect
     of the CSPICE module's internal configuration.
 
+- When using one of CSPICE's intrinsic error handling methods, no exception
+  will be raised, but a call to `failed()` will reveal whether an error has
+  occurred. A call to `reset()` is needed to clear the error.
+
+- Care has been taken to reduce the chances that the "dangerous" options
+  "IGNORE" and "REPORT" will cause a segmentation fault. However, this
+  possibility cannot be entirely ruled out, so caution is advised.
+
+- Because it would be a highly questionable thing to do, the "ABORT" and
+  "DEFAULT" options are overridden by "EXCEPTION" when the user is running
+  `cspyce` from an interactive shell. However, they resume their standard
+  effects during non-interactive runs.
+
 - When using the "RUNTIME" option, each CSPICE error condition raises a
-  Python RuntimeError exception rather than setting the failed() flag. This is
-  similar to the "EXCEPTION" option except the type of exception is always the
-  same.
+  Python `RuntimeError` exception rather than setting the `failed()` flag. This
+  is similar to the "EXCEPTION" option except the type of exception is always
+  the same.
 
 - Certain out-of-memory conditions are beyond the control of the CSPICE
   library. These will always raise a MemoryError exception, regardless of the
   exception handling method chosen.
 
-HANDLING OF ERROR FLAGS: Many CSPICE functions bypass the library's own error
-handling mechanism; instead they return a status flag, sometimes called "found"
-or "ok", or perhaps an empty response to indicate failure. The `cspyce` module
-provides alternative options for these functions.
+### HANDLING OF ERROR FLAGS
+
+Many CSPICE functions bypass the library's own error handling mechanism; instead
+they return a status flag, sometimes called "found" or "ok", or perhaps an empty
+response to indicate failure. The `cspyce` module provides alternative options
+for these functions.
 
 Within `cspyce`, functions that return error flags have an alternative
 implementation with a suffix of "_error", which uses the CSPICE/`cspyce` error
-handling mechanism instead.
+handling mechanism detailed above instead.
 
-Note that most _error versions of functions have fewer return values than the
+Note that most `_error` versions of functions have fewer return values than the
 associated non-error versions. The user should be certain which version is being
 used before interpreting the returned value(s).
 
-The `cspyce` module provides several ways to control which version of the function
-to use:
+The `cspyce` module provides several ways to control which version of the
+function to use:
 
-- The function use_flags() takes a function name or list of names and designates
-  the original version of each function as the default. If the input argument is
-  missing.
-
-- The function use_errors() takes a function name or list of names and
-  designates the _error version of each function as the default. If the input
-  argument is missing, _error versions are selected universally. With this
-  option, for example, a call to `cspyce`1.bodn2c() will actually call
-  `cspyce`1.bodn2c_error() instead.
-
-For backward compatibilty with our original Python cspice library, the _error
-versions of all cspice functions are selected by default.
-
-You can also choose between the "flag" and "error" versions of a function using
-`cspyce` function attributes, as discussed below.
+- The function `use_flags()` takes a function name or list of names and
+  designates the original version of each function as the default. If the input
+  argument is missing, original versions are selected universally.
+
+- The function `use_errors()` takes a function name or list of names and
+  designates the `_error` version of each function as the default. If the input
+  argument is missing, `_error` versions are selected universally.
+
+To provide a more consistent Python interface, the `_error` versions of all
+`cspyce` functions are selected by default. You can also choose between the
+"flag" and "error" versions of a function using `cspyce` function attributes,
+as discussed below.
 
 ---
 ## VECTORS AND ARRAYS
 
 ### VECTORIZATION
 Nearly every function that takes floating-point input (be it a
-scalar, 1-D array, or 2-D array) has a vectorized version, which allows you to
+scalar, 1-D array, or 2-D array) has a vectorized version that allows you to
 pass a vector of these items in place of a single value. The CSPICE function is
-called for each of the provided inputs and the function returns a vector of
-results.
+called for each of the provided inputs, the results are collected, and the
+`cspyce` function returns a vector of results.
 
-- Vectorized versions have the same name but with "_vector" appended.
+- Vectorized versions have the same name but with `_vector` appended.
 
 - In a vectorized function, you can replace any or all floating-point input
-  parameters with a array having one extra leading dimension. Integer, boolean,
+  parameters with an array having one extra leading dimension. Integer, boolean,
   and string inputs cannot be replaced by arrays.
 
 - If no inputs have an extra dimension, then the result is the same as
   calling the original, un-vectorized function.
 
 - Otherwise, all returned quantities are replaced by arrays having the size of
   the largest leading axis.
 
 - Note that it is permissible to pass arrays with different leading axis sizes
   to the function. The vectorized function cycles through the elements of each
   array repeatedly if necessary. It may make sense to do this if each leading
   axis is an integer fraction of the largest axis size. For example, if the
-  first input array has size 100 and the second has size 25, then the the
-  returned arrays(s) will have 100 elements and the values of the second
-  will each be used four times. However, caution is advised when using this
-  capability.
+  first input array has size 100 and the second has size 25, then the returned
+  arrays(s) will have 100 elements and the values of the second will each be
+  used four times. However, caution is advised when using this capability.
 
 - Some functions are not vectorized. These include:
   - Functions that have no floating-point inputs.
   - Functions that include strings among the returned quantities.
-  - Functions athat already return arrays where the leading axis could be
+  - Functions that already return arrays where the leading axis could be
     variable in size.
 
-- In the two cases (ckgp and ckgpav) where a function can be both vectorized
-  and either raise an error or return a flag, the "_vector" suffix comes
-  before "_error".
+- In the two cases (`ckgp` and `ckgpav`) where a function can be both vectorized
+  and either raise an error or return a flag, the `_vector` suffix comes
+  before `_error`.
 
 ### ARRAYS
 An optional import allows the `cspyce` module to support multidimensional
 arrays:
 
 ```python
 import cspyce
 import cspyce.arrays
 ```
 
-The latter import creates a new function in which the suffix "_array" replaces
-"_vector" for every vectorized function. Whereas _vector function support only
-a single extra dimension, _array functions follow all the standard rules of
-shape broadcasting as defined in NumPy. For example, if one input has leading
+The latter import creates a new function in which the suffix `_array` replaces
+`_vector` for every vectorized function. Whereas `_vector` functions support
+only a single extra dimension, `_array` functions follow all the standard rules
+of shape broadcasting as defined in NumPy. For example, if one input has leading
 dimension (10,4) and another has dimension (4,), then the two shapes will be
 broadcasted together and returned quantities will be arrays with shape (10,4).
 
 You can choose between the scalar, vector, and array versions of a function by
 using their explicit names, or by using `cspyce` function attributes, as discussed
 below.
 
 ---
 ## ALIASES
 
-Aliases allow the user to associate multiple names or codes with the same CSPICE
-body or frame. Aliases can be used for a variety of purposes.
+Aliases allow the user to associate multiple names or SPICE codes with the same
+CSPICE body or frame. Aliases can be used for a variety of purposes.
 
 - You can use names and codes interchangeably as input arguments to any `cspyce`
   function.
 - You can use a body name or code in place of a frame name or code, and the
   primary frame associated with that identified body will be used.
 - Strings that represent integers are equivalent to the integers themselves.
 
 Most importantly, you can allow multiple names or codes to refer to the same
-CPSICE body or frame. For bodies and frames that have multiple names or codes,
+CSPICE body or frame. For bodies and frames that have multiple names or codes,
 calls to a `cspyce` function will try each option in sequence until it finds one
-that works. Options are always tried in the order of they were defined, so
+that works. Options are always tried in the order in which they were defined, so
 higher-priority names and codes are tried first.
 
-Example 1: Jupiter's moon Dia uses code = 553, but it previously used code
+Example 1: Jupiter's moon Dia uses code 553, but it previously used code
 55076. With 55076 defined as an alias for 553, a `cspyce` call will return
 information about Dia under either of its codes.
 
 Example 2: The Earth's rotation is, by default, modeled by frame "IAU_EARTH".
 However, "ITRF93" is the name of a much more precise description of Earth's
 rotation. If you define "IAU_EARTH" as an alias for "ITRF93", then the `cspyce`
 toolkit will use ITRF93 if it is available, and otherwise IAU_EARTH.
 
 Immediately after a `cspyce` call involving aliases, you can find out what value
 or values were actually used by looking at attributes of the function. For
-example, the first input to `cspyce` function spkez is called "targ" and it
-identifies the code of a target being observed. After a call to
+example, the first input to the `cspyce` function `spkez` is called `targ` and
+it identifies the code of a target being observed. After a call to
 
 ```python
 cspyce.spkez(553, ...
 ```
-the value of `cspyce`.spkez.targ will be the code actually used, in this case
+the value of `cspyce.spkez.targ` will be the code actually used, in this case
 either 553 or 55076.
 
 To enable aliases, you must import an additional module
 
 ```python
 import cspyce
 import cspyce.aliases
 ```
 
-(Note that `cspyce`.aliases and `cspyce`.arrays can both be imported, and in either
-order. Note also that these are unconventional modules, in that they introduce
-new functionality into the "`cspyce`" namespace rather than creating new
-namespaces called "`cspyce`.aliases" and "`cspyce`.arrays".)
+(Note that `cspyce.aliases` and `cspyce.arrays` can both be imported, and in
+either order. Note also that these are unconventional modules, in that they
+introduce new functionality into the `cspyce` namespace rather than creating
+new namespaces called `cspyce.aliases` and `cspyce.arrays`.)
 
 With this import, a new function is defined for every `cspyce` function that takes
 a frame or body as input. The new function has the same name as the pre-existing
-`cspyce` function, but with "_alias" inserted immediately after the original
-`cspyce` name (and before any other suffix such as "_vector" or "_error").
+`cspyce` function, but with `_alias` inserted immediately after the original
+`cspyce` name (and before any other suffix such as `_vector` or `_error`).
 
 You can make alias support the default for individual `cspyce` functions or for
-the entire `cspyce` module by calling:
-  `cspyce`.use_aliases()
-These versions can subsequently be disabled as the default by calling:
-  `cspyce`.use_noaliases()
+the entire `cspyce` module by calling `cspyce.use_aliases()`. These versions
+can subsequently be disabled as the default by calling `cspyce.use_noaliases()`
+(see more detailed discussion below).
 
 To define a body alias or frame alias, call
-  `cspyce`.define_body_aliases(name_or_code, name_or_code, ...)
-  `cspyce`.define_frame_aliases(name_or_code, name_or_code, ...)
+
+    cspyce.define_body_aliases(name_or_code, name_or_code, ...)
+    cspyce.define_frame_aliases(name_or_code, name_or_code, ...)
+
 where the arguments are an arbitrary list of codes and names.
 
 To determine the aliases associated with a name or code, call
-  `cspyce`.get_body_aliases(name_or_code)
-  `cspyce`.get_frame_aliases(name_or_code)
+
+    cspyce.get_body_aliases(name_or_code)
+    cspyce.get_frame_aliases(name_or_code)
+
 where the argument is either a name or a code.
 
 You can also select between the alias-supporting and alias-nonsupporting
-versions of a function using function attributes.
+versions of a function using function attributes as discussed below.
 
 ---
 ## FUNCTION NAMES, VERSIONS AND SELECTION METHODS
 
 A `cspyce` function can accumulate several suffixes, based on the particular
 behavior, as so:
 ```python
 basename[_alias][_vector|_array][_error]
 ```
 Only functions that are truly distinct are defined. For example, if a function
 does not have a vector option, then no function will exist containing the
-"_vector" suffix.
+`_vector` suffix.
+
+You can use these functions to set defaults:
 
-Note that you can use these functions to set defaults:
-* `cspyce.use_flags()`
-* `cspyce.use_errors()`
-* `cspyce.use_scalars()`
-* `cspyce.use_vectors()`
-* `cspyce.use_arrays()`
-* `cspyce.use_aliases()`
-* `cspyce.use_noaliases()`
-
-FUNCTION ATTRIBUTES: These provide a simpler mechanism for choosing the needed
-version of a function, without remembering the suffix rules. Every `cspyce`
-function has these attributes, each of which identifies another (or possibly the
-same) `cspyce` function:
-
-| Attribute | Docstring |
-|-----------|-----------|
-| `func.flag`|   the equivalent function without the _error suffix, if any.|
-| `func.error`|  the equivalent function with the _error suffix, if any.|
-| `func.flag`|   the equivalent function without the _error suffix, if a.|
-| `func.error`|  the equivalent function with the _error suffix, if any
-| `func.scalar`| the equivalent function without _array or _vector suffes.|
-| `func.vector`| the equivalent function with the _vector suffix, if any
-| `func.array`|  the equivalent function with the _array suffix, if any.|
-| `func.alias`|  the equivalent function with the _alias suffix, if any.|
-| `func.noalias`| the equivalent function without the _alias suffix, if any.|
+    cspyce.use_flags()
+    cspyce.use_errors()
+    cspyce.use_scalars()
+    cspyce.use_vectors()
+    cspyce.use_arrays()
+    cspyce.use_aliases()
+    cspyce.use_noaliases()
+
+Each function can take one or more arguments referencing specific `cspyce`
+functions, in which case the defaults only apply to those functions. If no
+arguments are specified, the default applies to all functions. For example,
+to use "flags" as the default for all functions except `ckgp`, you could use:
+
+    cspyce.use_flags()
+    cspyce.use_errors(cspyce.ckgp)
+
+### FUNCTION ATTRIBUTES
+
+Function attributes provide a simpler mechanism for choosing the needed
+version of a function, without needing to remember the suffix rules. Every
+`cspyce` function has these attributes, each of which identifies another
+(or possibly the same) `cspyce` function:
+
+| Attribute      | Meaning                                                    |
+|----------------|------------------------------------------------------------|
+| `func.flag`    | the equivalent function without the _error suffix, if any. |
+| `func.error`   | the equivalent function with the _error suffix, if any.    |
+| `func.scalar`  | the equivalent function without _array or _vector suffixes.|
+| `func.vector`  | the equivalent function with the _vector suffix, if any.   |
+| `func.array`   | the equivalent function with the _array suffix, if any.    |
+| `func.alias`   | the equivalent function with the _alias suffix, if any.    |
+| `func.noalias` | the equivalent function without the _alias suffix, if any. |
 
 These attributes are always defined, even if the particular option is not
 supported by that function. This saves the programmer the effort of remembering,
 for example, which functions support aliases or which functions support flags.
 
-Thus, if the programmer wishes to be sure s/he is using the error version of
-function bodn2c, and wants the vector version if it exists (but it doesn't!),
-can call
+Thus, if the programmer wishes to be sure they are using the error version of
+function `bodn2c`, and wants the vector version if it exists (but it doesn't!),
+they can call
 
 ```python
 cspyce.bodn2c.error.vector(args...)
 ```
-
-Thus, it is never strictly necessary to refer to any function with its suffixes.
-
----
```

### Comparing `cspyce-2.0.7/cspyce/__init__.py` & `cspyce-2.0.8/cspyce/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,122 @@
-################################################################################
-# cspyce/__init__.py
-################################################################################
-# CSPYCE OVERVIEW
-#
-# cspyce is a Python module that provides an interface to the CSPICE library. It
-# implements the most widely-used functions of CSPICE in a Python-like way. It
-# also supports numerous enhancements, including support for Python exceptions,
-# array inputs, and aliases.
-#
-# This version of the library has been built for the CSPICE toolkit v. 66.
-#
-# See the file AAREADME.txt for more information.
-#
-# Mark Showalter, PDS Ring-Moons Systems Node, SETI Institute, December 2017.
-#   - Adapted for Python 3, February 2022.
-################################################################################
+"""
+cspyce/__init__.py
+
+CSPYCE OVERVIEW
+
+cspyce is a Python module that provides an interface to the CSPICE library. It
+implements the most widely-used functions of CSPICE in a Python-like way. It
+also supports numerous enhancements, including support for Python exceptions,
+array inputs, and aliases.
+
+This version of the library has been built for the CSPICE toolkit v. 67.
+
+cspyce contains Python interfaces to all CSPICE functions likely to be useful
+to a Python programmer. Excluded are deprecated functions and various low-level
+functions supporting character strings, cells, sets, file I/O, and also all
+low-level "geometry finder" functions that can only be implemented in C. It
+also includes vectorized versions (with suffix "_vector") for nearly every
+function that receives floating-point input and does not perform I/O.
+
+ADDED FEATURES
+
+DOCSTRINGS
+- All cspyce functions have informative docstrings, so typing
+      help(function)
+  provides useful information. However, the call signature appearing in the
+  first line of the help text is still defined by cspyce0 and may not make
+  sense to the reader. This issue is fixed by module cspyce2.
+
+DEFAULTS
+- Many cspyce functions take sensible default values if input arguments are
+  omitted.
+  - In gcpool, gdpool, gipool, and gnpool, start values default to 1.
+  - The functions that take "SET" or "GET" as their first argument (erract,
+    errdev, errprt, and timdef) have simplified calling options, which are
+    summarized in their docstrings.
+
+RUNTIME ERROR HANDLING
+
+In the CSPICE error handling mechanism, the programmer must check the value
+of function failed() regularly to determine if an error has occurred. However,
+Python's exception handling mechanism obviates the need for this approach. In
+cspyce1, all CSPICE errors raise Python exceptions.
+
+In CSPICE, the programmer can control how C errors are handled using the
+function erract(). Options include "IGNORE", "REPORT", "ABORT", "DEFAULT",
+and "RETURN", In cspyce1, the "IGNORE" and "REPORT" options are disabled,
+because they can leave behind corrupted memory. In interactive Python, the
+"ABORT" and "DEFAULT" options are also disabled, because aborting an
+interactive session would be pointless. The "ABORT" and "DEFAULT" options are
+still available, though not recommended, when running programs
+non-interactively.
+
+The cspyce1 module supports two additional error actions, which are variants
+on "RETURN". These are "EXCEPTION" and "RUNTIME". The only difference between
+them is that "RUNTIME" consistently raises RuntimeError exceptions, whereas
+"EXCEPTION" tailors the type of the exception to the situation.
+
+HANDLING OF ERROR FLAGS
+
+Many CSPICE functions bypass the library's own error handling mechanism;
+instead they return a status flag, sometimes called "found" or "ok", or else
+an empty response might indicate failure. The cspyce module provides
+alternative options for these functions.
+
+Within cspyce1, functions that return error flags have an alternative
+implementation with a suffix of "_error", which uses cspyce1's Python
+exception handling instead. For example, bodn2c(name) is the function that
+returns two values given the name of a body, its body ID and a True/False flag
+indicating whether the name was recognized. bodn2c_error() instead just
+returns a single value, the body ID. However, it raises a Python exception
+(KeyError or RuntimeError, depending on the erract setting) if the name is not
+recognized.
+
+The cspyce1 module provides several ways to control which version of the
+function to use:
+
+- The function use_flags() takes a function name or list of names and
+  designates the original version of each function as the default. If the
+  input argument is missing, _flag versions are selected universally.  With
+  this option, for example, a call to cspyce.bodn2c() will actually call
+  cspyce1.bodn2c_flag().
+
+- The function use_errors() takes a function name or list of names and
+  designates the _error version of each function as the default. If the input
+  argument is missing, _error versions are selected universally. With this
+  option, for example, a call to cspyce1.bodn2c() will actually call
+  cspyce1.bodn2c_error() instead.
+
+You can also choose between the "flag" and "error" versions of a function
+using cspyce function attributes, as discussed below.
+
+FUNCTION ATTRIBUTES
+
+Like any other Python class, functions can have attributes. These are used to
+simplify the choices of function options in cspyce1. Every cspyce1 function
+has these attributes:
+
+  error   = the version of this function that raises exceptions intead of
+            returning flags.
+  flag    = the version that returns flags instead of raising exceptions.
+  vector  = the vectorized version of this function.
+  scalar  = the un-vectorized version of this function.
+
+If a particular option is not relevant to a function, the attribute still
+exists, and instead simply returns the function itself. This makes it trivial
+to choose a particular combination of features for a particular function call.
+For example:
+  ckgpav.vector()         same as ckgpav_vector()
+  ckgpav.vector.flag()    same as ckgpav_vector()
+  ckgpav.vector.error()   same as ckgpav_vector_error()
+  ckgpav.error.scalar()   same as ckgpav_error()
+  ckgpav.flag()           same as ckgpav()
+  bodn2c.vector()         same as bodn2c()
+  bodn2c.flag()           same as bodn2c()
+"""
 
 import inspect
 import sys
 import os
 
 PYTHON2 = sys.version_info[0] < 3
 
@@ -173,15 +271,15 @@
     return validated
 
 ################################################################################
 # Functions to track down cspyce functions
 ################################################################################
 
 def get_all_funcs(source=None, cspyce_dict=None):
-    """ dictionary of all cspyce functions, keyed by their names.
+    """Return a dictionary of all cspyce functions, keyed by their names.
 
     Inputs:
         source      the dictionary to search, which defaults to globals().
         cspyce_dict is used internally for recursion; it should not be
                     referenced in external calls.
     """
 
@@ -208,28 +306,28 @@
 
         # Use the internal dictionary of this function as a recursive source
         _ = get_all_funcs(func.__dict__, cspyce_dict)
 
     return cspyce_dict
 
 def get_all_versions(func, source=None):
-    """A dictionary of all cspyce functions associated with this one, keyed by
-    their names.
+    """Return a dictionary of all cspyce functions associated with this one,
+    keyed by their names.
 
     Inputs:
         func        a cspyce function or the name of a cspyce function.
         source      the dictionary to search if func is specified by name;
                     default is globals().
     """
 
     func = validate_func(func, source)
     return get_all_funcs(func.__dict__)
 
 def validate_func(func, source=None):
-    """A cspyce function, given either its name or the function itself.
+    """Return a cspyce function, given either its name or the function itself.
     Otherwise, raise an exception.
 
     Inputs:
         func        a cspyce function or the name of a cspyce function.
         source      the dictionary to search if func is specified by name;
                     default is globals().
     """
```

### Comparing `cspyce-2.0.7/cspyce/alias_support.py` & `cspyce-2.0.8/cspyce/alias_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,18 +77,28 @@
         return ([item], [cspyce1.frmnam_error(item)])
     except (KeyError, ValueError):
         pass
 
     # If it's not a frame, see if it's a body with an associated frame
     body_codes = get_body_aliases(item)[0]
     for body_code in body_codes:
-        frame_code = cspyce.cidfrm_error(body_code)[0]
-        results = get_frame_aliases(frame_code)
-        if results[0]:
-            return results
+
+        # If it's a spacecraft, the bus frame code is body code * 1000
+        if body_code < 0:
+            results = get_frame_aliases(body_code * 1000)
+            if results[0]:
+                return results
+
+        # If it's a planetary body...
+        else:
+            (frame_code, frame_name, found) = cspyce.cidfrm.flag(body_code)
+            if found:
+                results = get_frame_aliases(frame_code)
+                if results[0]:
+                    return results
 
     return ([], [])
 
 ########################################
 
 def define_body_aliases(*items):
     """Define a list of items (integer codes or strings) as aliases of the same
@@ -321,16 +331,15 @@
             name = indx if isinstance(indx, str) else func.ARGNAMES[indx]
             body_or_frame = argtype.split('_')[0]
             cspyce1.setmsg('%s name "%s" not found in kernel pool' %
                            (body_or_frame, arg))
             cspyce1.sigerr('SPICE(' + body_or_frame.upper() + 'NAMENOTFOUND)')
 
 def alias_version(func):
-    """Wrapper function to support aliasing of SPICE body names or codes.
-    """
+    """Wrapper function to support aliasing of SPICE body names or codes."""
 
     if hasattr(func, 'alias'):
         return func.alias
 
     if not hasattr(func, 'ALIAS_ARGS'):
         alias_args = {}
         for k in range(len(func.ARGNAMES)):
```

### Comparing `cspyce-2.0.7/cspyce/aliases.py` & `cspyce-2.0.8/cspyce/aliases.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-################################################################################
-# cspyce/aliases.py
-################################################################################
-# Alias handler for the cspyce library
-#
-# Aliases allow the user to associate multiple names or codes with the same
-# CSPICE body or frame. Aliases can be used for a variety of purposes.
-#
-# - You can use names and codes interchangeably as input arguments to any cspyce
-#   function.
-# - You can use a body name or code in place of a frame name or code, and the
-#   primary frame associated with that identified body will be used.
-# - Strings that represent integers are equivalent to the integers themselves.
-#
-# Most importantly, you can allow multiple names or codes to refer to the same
-# CPSICE body or frame. For bodies and frames that have multiple names or codes,
-# calls to a cspyce function will try each option in sequence until it finds one
-# that works. Options are always tried in the order of they were defined, so
-# higher-priority names and codes are tried first.
-#
-# Example 1: Jupiter's moon Dia uses code = 553, but it previously used code
-# 55076. With 55076 defined as an alias for 553, a cspyce call will return
-# information about Dia under either of its codes.
-#
-# Example 2: The Earth's rotation is, by default, modeled by frame "IAU_EARTH".
-# However, "ITRF93" is the name of a much more precise description of Earth's
-# rotation. If you define "IAU_EARTH" as an alias for "ITRF93", then the cspyce
-# toolkit will use ITRF93 if it is available, and otherwise IAU_EARTH.
-#
-# Immediately after a cspyce call involving aliases, you can find out what value
-# or values were actually used by looking at attributes of the function. For
-# example, the first input to cspyce function spkez is called "targ" and it
-# identifies the code of a target being observed. After a call to
-#   cspyce.spkez(553, ...
-# the value of cspyce.spkez.targ will be the code actually used, in this case
-# either 553 or 55076.
-#
-# Upon importing this module, a new function is defined for every cspyce
-# function that takes a frame or body as input. The new function has the same
-# name as the pre-existing cspyce function, but with "_alias" inserted
-# immediately after the original cspyce name (and before any other suffix such
-# as "_vector" or "_error").
-#
-# You can make alias support the default for individual cspyce functions or for
-# the entire cspyce module by calling:
-#   cspyce.use_aliases()
-# These versions can subsequently be disabled as the default by calling:
-#   cspyce.use_noaliases()
-#
-# You can also select the specific version of the cspyce function via a function
-# attribute. For example, after calling
-#   cspyce.use_aliases('spkez')
-# the function cspyce.spkez will support aliases. However, calling
-#   cspyce.spkez.noalias(...)
-# will use the un-aliased version. You can also use the aliased version
-# explicitly by calling
-#   cspyce.spkez.alias(...)
-#
-# To define a body alias or frame alias, call
-#   cspyce.define_body_aliases(name_or_code, name_or_code, ...)
-#   cspyce.define_frame_aliases(name_or_code, name_or_code, ...)
-# where the arguments are an arbitrary list of codes and names.
-#
-# To determine the aliases associated with a name or code, call
-#   cspyce.get_body_aliases(name_or_code)
-#   cspyce.get_frame_aliases(name_or_code)
-# where the argument is either a name or a code.
-################################################################################
+"""
+cspyce/aliases.py
+
+Alias handler for the cspyce library
+
+Aliases allow the user to associate multiple names or codes with the same
+CSPICE body or frame. Aliases can be used for a variety of purposes.
+
+- You can use names and codes interchangeably as input arguments to any cspyce
+  function.
+- You can use a body name or code in place of a frame name or code, and the
+  primary frame associated with that identified body will be used.
+- Strings that represent integers are equivalent to the integers themselves.
+
+Most importantly, you can allow multiple names or codes to refer to the same
+CPSICE body or frame. For bodies and frames that have multiple names or codes,
+calls to a cspyce function will try each option in sequence until it finds one
+that works. Options are always tried in the order of they were defined, so
+higher-priority names and codes are tried first.
+
+Example 1: Jupiter's moon Dia uses code = 553, but it previously used code
+55076. With 55076 defined as an alias for 553, a cspyce call will return
+information about Dia under either of its codes.
+
+Example 2: The Earth's rotation is, by default, modeled by frame "IAU_EARTH".
+However, "ITRF93" is the name of a much more precise description of Earth's
+rotation. If you define "IAU_EARTH" as an alias for "ITRF93", then the cspyce
+toolkit will use ITRF93 if it is available, and otherwise IAU_EARTH.
+
+Immediately after a cspyce call involving aliases, you can find out what value
+or values were actually used by looking at attributes of the function. For
+example, the first input to cspyce function spkez is called "targ" and it
+identifies the code of a target being observed. After a call to
+  cspyce.spkez(553, ...
+the value of cspyce.spkez.targ will be the code actually used, in this case
+either 553 or 55076.
+
+Upon importing this module, a new function is defined for every cspyce
+function that takes a frame or body as input. The new function has the same
+name as the pre-existing cspyce function, but with "_alias" inserted
+immediately after the original cspyce name (and before any other suffix such
+as "_vector" or "_error").
+
+You can make alias support the default for individual cspyce functions or for
+the entire cspyce module by calling:
+  cspyce.use_aliases()
+These versions can subsequently be disabled as the default by calling:
+  cspyce.use_noaliases()
+
+You can also select the specific version of the cspyce function via a function
+attribute. For example, after calling
+  cspyce.use_aliases('spkez')
+the function cspyce.spkez will support aliases. However, calling
+  cspyce.spkez.noalias(...)
+will use the un-aliased version. You can also use the aliased version
+explicitly by calling
+  cspyce.spkez.alias(...)
+
+To define a body alias or frame alias, call
+  cspyce.define_body_aliases(name_or_code, name_or_code, ...)
+  cspyce.define_frame_aliases(name_or_code, name_or_code, ...)
+where the arguments are an arbitrary list of codes and names.
+
+To determine the aliases associated with a name or code, call
+  cspyce.get_body_aliases(name_or_code)
+  cspyce.get_frame_aliases(name_or_code)
+where the argument is either a name or a code.
+"""
 
 import cspyce
 import cspyce.alias_support as support
 
 if not hasattr(cspyce, 'ALIASES_IMPORTED'):
 
     # Upon import, define all missing alias versions
```

### Comparing `cspyce-2.0.7/cspyce/array_support.py` & `cspyce-2.0.8/cspyce/array_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 ################################################################################
 
 from __future__ import print_function
 
 import numpy as np
 import sys
 import inspect
+import warnings
 
 import cspyce
 import cspyce.cspyce1 as cspyce1
 from cspyce.alias_support import alias_version
 
 PYTHON2 = sys.version_info[0] < 3
 
 # This isn't how we want to handle a ragged array
-np.warnings.filterwarnings('ignore', category=np.VisibleDeprecationWarning)
+warnings.filterwarnings('ignore', category=np.VisibleDeprecationWarning)
 
 ################################################################################
 # cspyce array function wrapper
 ################################################################################
 
 ARRAY_NOTE = """
 This version supports array inputs in place of any floating-point inputs. Array
@@ -36,16 +37,20 @@
     arrayized = []
     for arg in arglist:
         arrayized.append(arg.replace('[_', '[...'))
 
     return arrayized
 
 def array_version(func):
-    """Wrapper function to apply NumPy broadcasting rules to the vectorized
-    inputs of any cspyce function.
+    """Create and return the array version of a cspyce function.
+
+    The array version is a wrapper function that applies NumPy broadcasting
+    rules to the inputs of a vector function. If the array version already
+    exists, just return it. If there is no vector version, the array version is
+    simply the scalar version.
     """
 
     if hasattr(func, 'array'):
         return func.array
 
     # Handle vector-free functions quickly
     if '_vector' not in func.__name__ and func.vector is func:
@@ -137,15 +142,15 @@
 
     # After copy, revise SIGNATURE, RETURNS, and NOTES
     wrapper.SIGNATURE = _arrayize_arglist(func.SIGNATURE)
     wrapper.RETURNS   = _arrayize_arglist(func.RETURNS)
     wrapper.NOTES     = [ARRAY_NOTE] + wrapper.NOTES[1:] # replace vector note
 
     # Save key attributes of the wrapper function before returning
-    cspyce.assign_docstring(wrapper)
+    cspyce1.assign_docstring(wrapper)
     wrapper.__name__ = _array_name(func.__name__)
     if PYTHON2:
         wrapper.func_defaults = func.func_defaults
     else:
         wrapper.__defaults__ = func.__defaults__
         wrapper.__signature__ = inspect.signature(func)
 
@@ -179,15 +184,15 @@
 
     # Identify arguments needing broadcasting, convert to arrays
     array_args = []     # list of tuples (index or key of arg, array, rank)
     shapes = []
     for indx in list(range(len(args))) + list(keywords.keys()):
 
         item = func.INPUT_ITEMS.get(indx, None)
-        if not item:
+        if item is None:
             continue
 
         rank = len(item)
 
         # Get argument
         arg = _getarg(indx, args, keywords)
 
@@ -236,15 +241,15 @@
             continue
 
         shapes.append(shape)
         array_args.append((indx, arg, rank))
 
     # Call function now if iteration is not needed
     if not array_args:
-        return func.scalar.__call__(*args, **keywords)
+        return func.vector.__call__(*args, **keywords)
 
     # Determine the broadcasted shape
     try:
         broadcasted_shape = np.broadcast_shapes(*shapes)
     except ValueError:
         cspyce1.chkin(func.array.__name__)
         cspyce1.setmsg('Incompatible shapes for broadcasting: ' +
```

### Comparing `cspyce-2.0.7/cspyce/arrays.py` & `cspyce-2.0.8/cspyce/arrays.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-################################################################################
-# cspyce/arrays.py
-################################################################################
-# Array handler for the cspyce library
-#
-# This module implements support for multidimensional arrays by building upon
-# all of the vectorized functions in the cspyce module. Upon importing this
-# module, a new function is defined for each "_vector" function, with the same
-# name except "_array" replacing "_vector".
-#
-# The key difference is that the "_array" functions follow all of the standard
-# NumPy rules for array broadcasting. Input arguments to cspyce _array functions
-# can have arbitrary additional dimensions, as long as all those dimensions
-# broadcast together properly. The returned arrays will all have the
-# broadcasted shape.
-################################################################################
+"""
+cspyce/arrays.py
+
+Array handler for the cspyce library
+
+This module implements support for multidimensional arrays by building upon
+all of the vectorized functions in the cspyce module. Upon importing this
+module, a new function is defined for each "_vector" function, with the same
+name except "_array" replacing "_vector".
+
+The key difference is that the "_array" functions follow all of the standard
+NumPy rules for array broadcasting. Input arguments to cspyce _array functions
+can have arbitrary additional dimensions, as long as all those dimensions
+broadcast together properly. The returned arrays will all have the
+broadcasted shape.
+"""
 
 import cspyce
 import cspyce.array_support as support
 
 # Upon import, define all array versions
 support._define_all_array_versions()
 
@@ -32,8 +32,7 @@
 ################################################################################
 # Record the fact that this module was imported
 ################################################################################
 
 cspyce.ARRAYS_IMPORTED = True
 
 ################################################################################
-
```

### Comparing `cspyce-2.0.7/cspyce/cspyce0.py` & `cspyce-2.0.8/cspyce/cspyce0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file was automatically generated by SWIG (http://www.swig.org).
-# Version 4.0.1
+# Version 4.0.2
 #
 # Do not make changes to this file unless you know what you are doing--modify
 # the SWIG interface file instead.
 
 from sys import version_info as _swig_python_version_info
 if _swig_python_version_info < (2, 7, 0):
     raise RuntimeError("Python 2.7 or later required")
```

### Comparing `cspyce-2.0.7/cspyce/cspyce0_info.py` & `cspyce-2.0.8/cspyce/cspyce0_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -4305,15 +4305,15 @@
 """
 CSPYCE_DEFINITIONS["ckcov"] = {
 'ck'    : ("string", "Name of CK file."),
 'idcode': ("body_code", "ID code of object."),
 'needav': ("bool", "Flag indicating whether angular velocity is needed."),
 'level' : ("string", "Coverage level: \"SEGMENT\" OR \"INTERVAL\"."),
 'tol'   : ("float", "Tolerance in ticks."),
-'timsys': ("string", "Time system used to represent coverage."),
+'timsys': ("string", "Time system used to represent coverage: \"SCLK\" or \"TDB\"."),
 'cover' : ("time[*,2]", "Array giving start/stop time pairs for the intervals covered."),
 }
 CSPYCE_URL["ckcov"] = "https://naif.jpl.nasa.gov/pub/naif/toolkit_docs/C/cspice/ckcov_c.html"
 #########################################
 CSPYCE_ARGNAMES["ckgp"] = ["inst", "sclkdp", "tol", "ref"]
 CSPYCE_RETNAMES["ckgp"] = ["cmat", "clkout", "found"]
 CSPYCE_ABSTRACT["ckgp"] = """
```

### Comparing `cspyce-2.0.7/cspyce/cspyce1.py` & `cspyce-2.0.8/cspyce/cspyce1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,125 +1,16 @@
 ################################################################################
 # cspyce/cspyce1.py
-################################################################################
-# module cspyce.cspyce1
 #
 # This module provides several enhancements over the low-level cspyce0 interface
-# to the CSPICE library.
-#
-# The cspyce1 module contains Python interfaces to all CSPICE functions likely
-# to be useful to a Python programmer. Excluded are deprecated functions and
-# various low-level functions supporting character strings, cells, sets, file
-# I/O, and also all low-level "geometry finder" functions that can only be
-# implemented in C. It also includes vectorized versions (with suffix "_vector")
-# for nearly every function that receives floating-point input and does not
-# perform I/O. As of April 2022, however, some of the less-used cspice
-# functions have not yet been fully tested.
-#
-# To use cspyce1:
-#   import cspyce.cspyce1
-# or
-#   import cspyce.cspyce1 as cspyce
-#
-# ADDED FEATURES
-#
-# DOCSTRINGS
-# - All cspyce functions have informative docstrings, so typing
-#       help(function)
-#   provides useful information. However, the call signature appearing in the
-#   first line of the help text is still defined by cspyce0 and may not make
-#   sense to the reader. This issue is fixed by module cspyce2.
-#
-# DEFAULTS
-# - Many cspyce functions take sensible default values if input arguments are
-#   omitted.
-#   - In gcpool, gdpool, gipool, and gnpool, start values default to 1.
-#   - The functions that take "SET" or "GET" as their first argument (erract,
-#     errdev, errprt, and timdef) have simplified calling options, which are
-#     summarized in their docstrings.
-#
-# RUNTIME ERROR HANDLING
-#
-# In the CSPICE error handling mechanism, the programmer must check the value
-# of function failed() regularly to determine if an error has occurred. However,
-# Python's exception handling mechanism obviates the need for this approach. In
-# cspyce1, all CSPICE errors raise Python exceptions.
-#
-# In CSPICE, the programmer can control how C errors are handled using the
-# function erract(). Options include "IGNORE", "REPORT", "ABORT", "DEFAULT",
-# and "RETURN", In cspyce1, the "IGNORE" and "REPORT" options are disabled,
-# because they can leave behind corrupted memory. In interactive Python, the
-# "ABORT" and "DEFAULT" options are also disabled, because aborting an
-# interactive session would be pointless. The "ABORT" and "DEFAULT" options are
-# still available, though not recommended, when running programs
-# non-interactively.
-#
-# The cspyce1 module supports two additional error actions, which are variants
-# on "RETURN". These are "EXCEPTION" and "RUNTIME". The only difference between
-# them is that "RUNTIME" consistently raises RuntimeError exceptions, whereas
-# "EXCEPTION" tailors the type of the exception to the situation.
-#
-# HANDLING OF ERROR FLAGS
+# to the CSPICE library. See cspyce/__init__.py for a full explanation.
 #
-# Many CSPICE functions bypass the library's own error handling mechanism;
-# instead they return a status flag, sometimes called "found" or "ok", or else
-# an empty response might indicate failure. The cspyce module provides
-# alternative options for these functions.
-#
-# Within cspyce1, functions that return error flags have an alternative
-# implementation with a suffix of "_error", which uses cspyce1's Python
-# exception handling instead. For example, bodn2c(name) is the function that
-# returns two values given the name of a body, its body ID and a True/False flag
-# indicating whether the name was recognized. bodn2c_error() instead just
-# returns a single value, the body ID. However, it raises a Python exception
-# (KeyError or RuntimeError, depending on the erract setting) if the name is not
-# recognized.
-#
-# The cspyce1 module provides several ways to control which version of the
-# function to use:
-#
-# - The function use_flags() takes a function name or list of names and
-#   designates the original version of each function as the default. If the
-#   input argument is missing, _flag versions are selected universally.  With this
-#   option, for example, a call to cspyce.bodn2c() will actually call
-#   cspyce1.bodn2c_flag().
-#
-# - The function use_errors() takes a function name or list of names and
-#   designates the _error version of each function as the default. If the input
-#   argument is missing, _error versions are selected universally. With this
-#   option, for example, a call to cspyce1.bodn2c() will actuall call
-#   cspyce1.bodn2c_error() instead.
-#
-# You can also close between the "flag" and "error" versions of a function using
-# cspyce function attributes, as discussed below.
-#
-# FUNCTION ATTRIBUTES
-#
-# Like any other Python class, functions can have attributes. These are used to
-# simplify the choices of function options in cspyce1. Every cspyce1 function
-# has these attributes:
-#
-#   error   = the version of this function that raises errors intead of
-#             returning flags.
-#   flag    = the version that returns flags instead of raising errors.
-#   vector  = the vectorized version of this function.
-#   scalar  = the un-vectorized version of this function.
-#
-# If a particular option is not relevant to a function, the attribute still
-# exists, and instead simply returns the function itself. This makes it trivial
-# to choose a particular combination of features for a particular function call.
-# For example:
-#   ckgpav.vector()         same as ckgpav_vector()
-#   ckgpav.vector.flag()    same as ckgpav_vector()
-#   ckgpav.vector.error()   same as ckgpav_vector_error()
-#   ckgpav.error.scalar()   same as ckgpav_error()
-#   ckgpav.flag()           same as ckgpav()
-#   bodn2c.vector()         same as bodn2c()
-#   bodn2c.flag()           same as bodn2c()
+# Used internally by cspyce; not intended for direct import.
 ################################################################################
+
 from __future__ import print_function
 
 import sys
 import numpy as np
 import textwrap
 
 from cspyce import cspyce0
```

### Comparing `cspyce-2.0.7/cspyce/cspyce1_info.py` & `cspyce-2.0.8/cspyce/cspyce1_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # cspyce/cspyce1_info.py
 #
 # A dictionary of docstrings and call signatures, keyed by the name of the
 # CSPICE function name.
 #
 # This function reads the associated cspyce0 dictionaries and updates them for
 # the cspyce1 "_error" versions.
+#
+# Used internally by cspyce; not intended for direct import.
 ################################################################################
 
 from cspyce.cspyce0_info import \
     CSPYCE_SIGNATURES, CSPYCE_ARGNAMES, CSPYCE_DEFAULTS, \
     CSPYCE_RETURNS, CSPYCE_RETNAMES, CSPYCE_DEFINITIONS, \
     CSPYCE_ABSTRACT, CSPYCE_PS, CSPYCE_URL
```

### Comparing `cspyce-2.0.7/cspyce/cspyce2.py` & `cspyce-2.0.8/cspyce/cspyce2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 ################################################################################
 # cspyce/cspyce2.py
-################################################################################
-# module cspyce.cspyce2
 #
 # This module re-declares every cspyce1 function explicitly, with its list of
 # argument names as used by CSPICE. The practical effect is that functions in
 # cspyce2 module can be called in a fully Python-like way, the rightmost inputs
 # in any order and identified by their names.
 #
-# NOTE: This file is generated automatically using program make_cspyce2.py:
-#   python make_cspyce2.py > cspyce2.py
-#
+# Used internally by cspyce; not intended for direct import.
 ################################################################################
 
 import sys
 import cspyce.cspyce1 as cspyce1
 import keyword
 
 PYTHON2 = sys.version_info[0] < 3
 
 # This function makes cspyce2 look the same as cspyce1. It ensures that every
-# location in the global dictionary and every function's internal link point
+# location in the global dictionary and every function's internal link point to
 # a new function of the same name.
 
 CSPYCE_FUNCTION_LOOKUP = {}
 
 
 def relink_all(new_dict, old_dict):
```

### Comparing `cspyce-2.0.7/cspyce/typemap_samples.py` & `cspyce-2.0.8/cspyce/typemap_samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file was automatically generated by SWIG (http://www.swig.org).
-# Version 4.0.1
+# Version 4.0.2
 #
 # Do not make changes to this file unless you know what you are doing--modify
 # the SWIG interface file instead.
 
 from sys import version_info as _swig_python_version_info
 if _swig_python_version_info < (2, 7, 0):
     raise RuntimeError("Python 2.7 or later required")
```

### Comparing `cspyce-2.0.7/cspyce/typemap_test.py` & `cspyce-2.0.8/cspyce/typemap_test.py`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.7/cspyce.egg-info/SOURCES.txt` & `cspyce-2.0.8/cspyce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cspyce-2.0.7/get_spice.py` & `cspyce-2.0.8/get_spice.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ################################################################################
 # get_spice.py
 ################################################################################
 #
-# This module is responsible for downloading the cspice source files based on whatever
-# hardware and software it is currently running on.
+# This module is responsible for downloading the CSPICE source files based on
+# whatever hardware and software it is currently running on.
 #
 # The contents of the directories
 #        <download>/cspice/src/cspice
 #        <download>/include
 # are put into the two directories
 #        cspice/<os>-<arch>/src
 #        cspice/<os>-<arch>/include
 #
 # This module should only be called by setup.py.
 #
-# This file owes a big debt to Andrew Annex and his file:
+# This file owes a big debt to Dr. Andrew Annex and his file:
 #      https://github.com/AndrewAnnex/SpiceyPy/blob/main/get_spice.py
-# His version is much more ambitious than this and also compiles the files into a
-# shared library.
+# His version is much more ambitious than this and also compiles the files into
+# a shared library.
 ################################################################################
 
 
 from __future__ import absolute_import, with_statement
 
 import os
 import platform
@@ -70,18 +70,18 @@
         # Get directory that this file is in.
         self.root_dir = str(Path(os.path.realpath(__file__)).parent)
         # Get directory into which we want to put all our files
         self.target_directory = os.path.join(
             self.root_dir, "cspice", self.host_OS + "-" + self.architecture)
 
     def download(self):
-        if Path(os.path.join(self.target_directory, "src")).is_dir() and \
-           Path(os.path.join(self.target_directory, "include")).is_dir():
+        if (Path(os.path.join(self.target_directory, "src")).is_dir() and
+            Path(os.path.join(self.target_directory, "include")).is_dir()):
             return self.target_directory
-        # Note.  Once we toss 2.7 support, this can be rewritten as "with ...."
+        # Note: Once we toss 2.7 support, this can be rewritten as "with ...."
         tmpdir = tempfile.mkdtemp()
         try:
             self.download_cspice(destination=tmpdir)
             shutil.copytree(os.path.join(tmpdir, "cspice", "src", "cspice"),
                             os.path.join(self.target_directory, "src"))
             shutil.copytree(os.path.join(tmpdir, "cspice", "include"),
                             os.path.join(self.target_directory, "include"))
@@ -114,15 +114,16 @@
                     # Do we want --connect_timeout? This curl either seems to take
                     # 3s or several minutes, somewhat randomly.
                     subprocess.check_call(["curl", url, "-o", target_file])
                     with ZipFile(target_file, "r") as archive:
                         archive.extractall(destination)
                 else:
                     target_file = target_file[:-2] # remove the .Z
-                    subprocess.check_call("curl {} | gzip -d > {}".format(url, target_file), shell=True)
+                    subprocess.check_call("curl {} | gzip -d > {}".format(
+                        url, target_file), shell=True)
                     with TarFile.open(target_file, "r") as archive:
                         archive.extractall(destination)
                 os.unlink(target_file)
                 break
             except (RuntimeError, subprocess.CalledProcessError) as error:
                 attempts -= 1
                 if attempts == 0:
```

### Comparing `cspyce-2.0.7/setup.py` & `cspyce-2.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 #!/usr/bin/env python
 
-# If you are installing this code via "pip install pds-cspyce", then you should
+# If you are installing this code via "pip install cspyce", then you should
 # never see this file.  pip automatically determines whether you need a binary
 # distribution or source distribution, and automatically builds it as needed for
 # your machine.
 #
-# If you are doing a build from sources, please read README-developers.md in this
-# directory.
+# If you are doing a build from sources, please read README-developers.md in
+# this directory.
 
 
 # We prefer setuptools, but will use distutils if setuptools isn't available
 import os
 from glob import glob
 import os
+import platform
 import subprocess
 import sys
 
 from setuptools.command.build_ext import build_ext
 
 from get_spice import GetCspice
 
 try:
     from setuptools import Command, setup, Extension
-    from setuptools.command.build_py import build_py
 except ImportError:
     from distutils.core import Command, setup, Extension
-    from distutils.core import setup, Extension, build_py
 
 try:
     import numpy
 except ImportError:
     subprocess.check_call([sys.executable, "-m", "pip", "install", "numpy"])
     import numpy
 
 
-import subprocess
-import sys
-import platform
-
 PYTHON2 = sys.version_info[0] < 3
-IS_LINUX = platform.system() == 'Linux'
-IS_MACOS = platform.system() == 'Darwin'
-IS_WINDOWS = platform.system() == 'Windows'
+IS_LINUX = platform.system() == "Linux"
+IS_MACOS = platform.system() == "Darwin"
+IS_WINDOWS = platform.system() == "Windows"
 assert IS_LINUX or IS_MACOS or IS_WINDOWS
 
 
 class GenerateCommand(Command):
     user_options = []
 
     def initialize_options(self):
@@ -67,15 +62,15 @@
                       "-o swig/typemap_samples_wrap.c swig/typemap_samples.i".split(' ')
             subprocess.check_call(command)
         else:
             command = "echo Cannot rebuild files in Python2".split(' ')
             subprocess.check_call(command)
 
 
-# Some linkers seem to have trouble with 2400 files.  So we break it up into
+# Some linkers seem to have trouble with 2400 files, so we break it up into
 # smaller libraries with a maximum of 250 files apiece.
 
 cspice_directory = GetCspice().download()
 
 def get_c_libraries():
     files = sorted(glob(os.path.join(cspice_directory, "src", "*.c")))
     splits = 1 if IS_LINUX else 1 + (len(files) // 250)
@@ -118,22 +113,21 @@
 def do_setup():
     prerelease_version = os.getenv('PRERELEASE_VERSION', '')
     if prerelease_version == 'release':
         prerelease_version = ''
 
     setup(
         name='cspyce',
-        version='2.0.7' + prerelease_version,
+        version='2.0.8' + prerelease_version,
         author="Mark Showalter/PDS Ring-Moon Systems Node",
         description="Low-level SWIG interface to the CSPICE library",
         ext_modules=get_extensions(),
         libraries=get_c_libraries(),
         packages=["cspyce"],
         install_requires=['numpy'],
         cmdclass={
             'build_ext': MyBuildExt,
             'generate': GenerateCommand,
         }
     )
 
 do_setup()
-
```

### Comparing `cspyce-2.0.7/swig/cspyce0_wrap.c` & `cspyce-2.0.8/swig/cspyce0_wrap.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /* ----------------------------------------------------------------------------
  * This file was automatically generated by SWIG (http://www.swig.org).
- * Version 4.0.1
+ * Version 4.0.2
  *
  * This file is not intended to be easily readable and contains a number of
  * coding conventions designed to improve portability and efficiency. Do not make
  * changes to this file unless you know what you are doing--modify the SWIG
  * interface file instead.
  * ----------------------------------------------------------------------------- */
 
@@ -780,35 +780,39 @@
 
 /* Warning: This function will allocate a new string in Python 3,
  * so please call SWIG_Python_str_DelForPy3(x) to free the space.
  */
 SWIGINTERN char*
 SWIG_Python_str_AsChar(PyObject *str)
 {
-#if PY_VERSION_HEX >= 0x03000000
+#if PY_VERSION_HEX >= 0x03030000
+  return (char *)PyUnicode_AsUTF8(str);
+#elif PY_VERSION_HEX >= 0x03000000
   char *newstr = 0;
   str = PyUnicode_AsUTF8String(str);
   if (str) {
     char *cstr;
     Py_ssize_t len;
-    PyBytes_AsStringAndSize(str, &cstr, &len);
-    newstr = (char *) malloc(len+1);
-    memcpy(newstr, cstr, len+1);
+    if (PyBytes_AsStringAndSize(str, &cstr, &len) != -1) {
+      newstr = (char *) malloc(len+1);
+      if (newstr)
+        memcpy(newstr, cstr, len+1);
+    }
     Py_XDECREF(str);
   }
   return newstr;
 #else
   return PyString_AsString(str);
 #endif
 }
 
-#if PY_VERSION_HEX >= 0x03000000
-#  define SWIG_Python_str_DelForPy3(x) free( (void*) (x) )
+#if PY_VERSION_HEX >= 0x03030000 || PY_VERSION_HEX < 0x03000000
+#  define SWIG_Python_str_DelForPy3(x)
 #else
-#  define SWIG_Python_str_DelForPy3(x) 
+#  define SWIG_Python_str_DelForPy3(x) free( (void*) (x) )
 #endif
 
 
 SWIGINTERN PyObject*
 SWIG_Python_str_FromChar(const char *c)
 {
 #if PY_VERSION_HEX >= 0x03000000
@@ -1215,14 +1219,27 @@
 	objs[l] = 0;
       }
       return i + 1;
     }    
   }
 }
 
+SWIGINTERN int
+SWIG_Python_CheckNoKeywords(PyObject *kwargs, const char *name) {
+  int no_kwargs = 1;
+  if (kwargs) {
+    assert(PyDict_Check(kwargs));
+    if (PyDict_Size(kwargs) > 0) {
+      PyErr_Format(PyExc_TypeError, "%s() does not take keyword arguments", name);
+      no_kwargs = 0;
+    }
+  }
+  return no_kwargs;
+}
+
 /* A functor is a function object with one single object argument */
 #define SWIG_Python_CallFunctor(functor, obj)	        PyObject_CallFunctionObjArgs(functor, obj, NULL);
 
 /*
   Helper for static pointer initialization for both C and C++ code, for example
   static PyObject *SWIG_STATIC_POINTER(MyVar) = NewSomething(...);
 */
@@ -1728,14 +1745,20 @@
       0,                                    /* tp_subclasses */
       0,                                    /* tp_weaklist */
       0,                                    /* tp_del */
       0,                                    /* tp_version_tag */
 #if PY_VERSION_HEX >= 0x03040000
       0,                                    /* tp_finalize */
 #endif
+#if PY_VERSION_HEX >= 0x03080000
+      0,                                    /* tp_vectorcall */
+#endif
+#if (PY_VERSION_HEX >= 0x03080000) && (PY_VERSION_HEX < 0x03090000)
+      0,                                    /* tp_print */
+#endif
 #ifdef COUNT_ALLOCS
       0,                                    /* tp_allocs */
       0,                                    /* tp_frees */
       0,                                    /* tp_maxalloc */
       0,                                    /* tp_prev */
       0                                     /* tp_next */
 #endif
@@ -1889,14 +1912,20 @@
       0,                                    /* tp_subclasses */
       0,                                    /* tp_weaklist */
       0,                                    /* tp_del */
       0,                                    /* tp_version_tag */
 #if PY_VERSION_HEX >= 0x03040000
       0,                                    /* tp_finalize */
 #endif
+#if PY_VERSION_HEX >= 0x03080000
+      0,                                    /* tp_vectorcall */
+#endif
+#if (PY_VERSION_HEX >= 0x03080000) && (PY_VERSION_HEX < 0x03090000)
+      0,                                    /* tp_print */
+#endif
 #ifdef COUNT_ALLOCS
       0,                                    /* tp_allocs */
       0,                                    /* tp_frees */
       0,                                    /* tp_maxalloc */
       0,                                    /* tp_prev */
       0                                     /* tp_next */
 #endif
@@ -2215,29 +2244,35 @@
 	if (dict == NULL) {
 	  dict = PyDict_New();
 	  *dictptr = dict;
 	  PyDict_SetItem(dict, SWIG_This(), swig_this);
 	}
       }
 #else
-      PyObject *key = SWIG_This();
-      PyObject_SetAttr(inst, key, swig_this);
+      if (PyObject_SetAttr(inst, SWIG_This(), swig_this) == -1) {
+        Py_DECREF(inst);
+        inst = 0;
+      }
 #endif
     }
   } else {
 #if PY_VERSION_HEX >= 0x03000000
     PyObject *empty_args = PyTuple_New(0);
     if (empty_args) {
       PyObject *empty_kwargs = PyDict_New();
       if (empty_kwargs) {
         inst = ((PyTypeObject *)data->newargs)->tp_new((PyTypeObject *)data->newargs, empty_args, empty_kwargs);
         Py_DECREF(empty_kwargs);
         if (inst) {
-          PyObject_SetAttr(inst, SWIG_This(), swig_this);
-          Py_TYPE(inst)->tp_flags &= ~Py_TPFLAGS_VALID_VERSION_TAG;
+          if (PyObject_SetAttr(inst, SWIG_This(), swig_this) == -1) {
+            Py_DECREF(inst);
+            inst = 0;
+          } else {
+            Py_TYPE(inst)->tp_flags &= ~Py_TPFLAGS_VALID_VERSION_TAG;
+          }
         }
       }
       Py_DECREF(empty_args);
     }
 #else
     PyObject *dict = PyDict_New();
     if (dict) {
@@ -2246,47 +2281,44 @@
       Py_DECREF(dict);
     }
 #endif
   }
   return inst;
 }
 
-SWIGRUNTIME void
+SWIGRUNTIME int
 SWIG_Python_SetSwigThis(PyObject *inst, PyObject *swig_this)
 {
- PyObject *dict;
 #if !defined(SWIG_PYTHON_SLOW_GETSET_THIS)
- PyObject **dictptr = _PyObject_GetDictPtr(inst);
- if (dictptr != NULL) {
-   dict = *dictptr;
-   if (dict == NULL) {
-     dict = PyDict_New();
-     *dictptr = dict;
-   }
-   PyDict_SetItem(dict, SWIG_This(), swig_this);
-   return;
- }
+  PyObject **dictptr = _PyObject_GetDictPtr(inst);
+  if (dictptr != NULL) {
+    PyObject *dict = *dictptr;
+    if (dict == NULL) {
+      dict = PyDict_New();
+      *dictptr = dict;
+    }
+    return PyDict_SetItem(dict, SWIG_This(), swig_this);
+  }
 #endif
- dict = PyObject_GetAttrString(inst, "__dict__");
- PyDict_SetItem(dict, SWIG_This(), swig_this);
- Py_DECREF(dict);
+  return PyObject_SetAttr(inst, SWIG_This(), swig_this);
 } 
 
 
 SWIGINTERN PyObject *
 SWIG_Python_InitShadowInstance(PyObject *args) {
   PyObject *obj[2];
   if (!SWIG_Python_UnpackTuple(args, "swiginit", 2, 2, obj)) {
     return NULL;
   } else {
     SwigPyObject *sthis = SWIG_Python_GetSwigThis(obj[0]);
     if (sthis) {
       SwigPyObject_append((PyObject*) sthis, obj[1]);
     } else {
-      SWIG_Python_SetSwigThis(obj[0], obj[1]);
+      if (SWIG_Python_SetSwigThis(obj[0], obj[1]) != 0)
+        return NULL;
     }
     return SWIG_Py_Void();
   }
 }
 
 /* Create a new pointer object */
 
@@ -2680,15 +2712,15 @@
 
 #else
 #  define SWIG_init    init_cspyce0
 
 #endif
 #define SWIG_name    "_cspyce0"
 
-#define SWIGVERSION 0x040001 
+#define SWIGVERSION 0x040002 
 #define SWIG_VERSION SWIGVERSION
 
 
 #define SWIG_as_voidptr(a) (void *)((const void *)(a)) 
 #define SWIG_as_voidptrptr(a) ((void)SWIG_as_voidptr(*a),(void**)(a)) 
 
 
@@ -2712,24 +2744,24 @@
 #define COMMENTLEN 256  // max length of a comment including null
 #define COMMENTS 100    // max number of comments read at a time
 #define FILELEN 1000    // max length of a file path including null
 #define FOVSHAPE 40     // max number of vertices in the shape of an FOV
 #define KERVALLEN 80    // max length of a kernel string value
 #define KERVALS 40      // max number of values associated with a kernel name
 #define LONGMSGLEN 10000// max length of a long error message including null
-#define MAXIDS 200      // max body or frame IDs returned
+#define MAXIDS 500      // max body or frame IDs returned
 #define MAXRECS 1000    // max number of records returned in a DAS read
 #define MAXROWS 1000    // max number of records/rows returned in an EK query
 #define MAXVALS 100     // max number of values in a column or parsed string
 #define MAXFOV 100      // max number of vertices in a FOV
 #define MESSAGELEN 1024 // max length of an error message including null
 #define NAMELEN 65      // table names can be 64 plus one null
 #define NPLATES 10000   // max number of DSK plates or vertices
 #define TIMELEN 60      // max length of a time string including null
-#define WINDOWS 30000   // max time windows returned
+#define WINDOWS 120000  // max time windows returned
 
 /* Define NAN for Microsoft C compiler if necessary */
 #ifdef _MSC_VER
 #define INFINITY (DBL_MAX+DBL_MAX)
 #define NAN (INFINITY-INFINITY)
 #endif
 
@@ -8401,17 +8433,19 @@
     }
     obj = PyUnicode_AsUTF8String(obj);
     if (!obj)
       return SWIG_TypeError;
     if (alloc)
       *alloc = SWIG_NEWOBJ;
 #endif
-    PyBytes_AsStringAndSize(obj, &cstr, &len);
+    if (PyBytes_AsStringAndSize(obj, &cstr, &len) == -1)
+      return SWIG_TypeError;
 #else
-    PyString_AsStringAndSize(obj, &cstr, &len);
+    if (PyString_AsStringAndSize(obj, &cstr, &len) == -1)
+      return SWIG_TypeError;
 #endif
     if (cptr) {
       if (alloc) {
 	if (*alloc == SWIG_NEWOBJ) {
 	  *cptr = (char *)memcpy(malloc((len + 1)*sizeof(char)), cstr, sizeof(char)*(len + 1));
 	  *alloc = SWIG_NEWOBJ;
 	} else {
@@ -14058,14 +14092,21 @@
                 in11[i % in11_dim1]);
         }
 
         *out11 = out11_buffer; *out11_dim1 = maxdim;
     }
 
 
+    void my_lmpool_c(
+        ConstSpiceChar *cvals, SpiceInt n, SpiceInt cvalen)
+    {
+        lmpool_c(cvals, cvalen, n);
+    }
+
+
     void my_nextwd_c(
         ConstSpiceChar *string,
         SpiceInt       nexlen, SpiceChar next[COLLEN],
         SpiceInt       reslen, SpiceChar rest[MESSAGELEN])
     {
         nextwd_c(string, nexlen, reslen, next, rest);
     }
@@ -115283,27 +115324,16 @@
       }
       arg1 = (ConstSpiceChar *)buffer1;
       arg2 = (int) count;
       arg3 = (int)(maxlen + 1);
     }
     /*@SWIG@*/
   }
-  lmpool_c(arg1,arg2,arg3);
-  {
-    /*@SWIG:swig/cspyce_typemaps.i,479,TEST_FOR_EXCEPTION@*/{
-      if (failed_c()) {
-        handle_swig_exception("lmpool");
-        SWIG_fail;
-      }
-    }
-    /*@SWIG@*/;
-    if (!resultobj) {
-      resultobj = (Py_INCREF(Py_None), Py_None);
-    }
-  }
+  my_lmpool_c(arg1,arg2,arg3);
+  resultobj = SWIG_Py_Void();
   
   {
     Py_XDECREF(list1);
     PyMem_Free((void *) buffer1);
   }
   return resultobj;
 fail:
@@ -131850,14 +131880,20 @@
         0,                                  /* tp_weaklistoffset */
         0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0, /* tp_iter -> tp_weaklist */
         0,                                  /* tp_del */
         0,                                  /* tp_version_tag */
 #if PY_VERSION_HEX >= 0x03040000
         0,                                  /* tp_finalize */
 #endif
+#if PY_VERSION_HEX >= 0x03080000
+        0,                                  /* tp_vectorcall */
+#endif
+#if (PY_VERSION_HEX >= 0x03080000) && (PY_VERSION_HEX < 0x03090000)
+        0,                                  /* tp_print */
+#endif
 #ifdef COUNT_ALLOCS
         0,                                  /* tp_allocs */
         0,                                  /* tp_frees */
         0,                                  /* tp_maxalloc */
         0,                                  /* tp_prev */
         0                                   /* tp_next */
 #endif
```

### Comparing `cspyce-2.0.7/swig/typemap_samples_wrap.c` & `cspyce-2.0.8/swig/typemap_samples_wrap.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /* ----------------------------------------------------------------------------
  * This file was automatically generated by SWIG (http://www.swig.org).
- * Version 4.0.1
+ * Version 4.0.2
  *
  * This file is not intended to be easily readable and contains a number of
  * coding conventions designed to improve portability and efficiency. Do not make
  * changes to this file unless you know what you are doing--modify the SWIG
  * interface file instead.
  * ----------------------------------------------------------------------------- */
 
@@ -780,35 +780,39 @@
 
 /* Warning: This function will allocate a new string in Python 3,
  * so please call SWIG_Python_str_DelForPy3(x) to free the space.
  */
 SWIGINTERN char*
 SWIG_Python_str_AsChar(PyObject *str)
 {
-#if PY_VERSION_HEX >= 0x03000000
+#if PY_VERSION_HEX >= 0x03030000
+  return (char *)PyUnicode_AsUTF8(str);
+#elif PY_VERSION_HEX >= 0x03000000
   char *newstr = 0;
   str = PyUnicode_AsUTF8String(str);
   if (str) {
     char *cstr;
     Py_ssize_t len;
-    PyBytes_AsStringAndSize(str, &cstr, &len);
-    newstr = (char *) malloc(len+1);
-    memcpy(newstr, cstr, len+1);
+    if (PyBytes_AsStringAndSize(str, &cstr, &len) != -1) {
+      newstr = (char *) malloc(len+1);
+      if (newstr)
+        memcpy(newstr, cstr, len+1);
+    }
     Py_XDECREF(str);
   }
   return newstr;
 #else
   return PyString_AsString(str);
 #endif
 }
 
-#if PY_VERSION_HEX >= 0x03000000
-#  define SWIG_Python_str_DelForPy3(x) free( (void*) (x) )
+#if PY_VERSION_HEX >= 0x03030000 || PY_VERSION_HEX < 0x03000000
+#  define SWIG_Python_str_DelForPy3(x)
 #else
-#  define SWIG_Python_str_DelForPy3(x) 
+#  define SWIG_Python_str_DelForPy3(x) free( (void*) (x) )
 #endif
 
 
 SWIGINTERN PyObject*
 SWIG_Python_str_FromChar(const char *c)
 {
 #if PY_VERSION_HEX >= 0x03000000
@@ -1215,14 +1219,27 @@
 	objs[l] = 0;
       }
       return i + 1;
     }    
   }
 }
 
+SWIGINTERN int
+SWIG_Python_CheckNoKeywords(PyObject *kwargs, const char *name) {
+  int no_kwargs = 1;
+  if (kwargs) {
+    assert(PyDict_Check(kwargs));
+    if (PyDict_Size(kwargs) > 0) {
+      PyErr_Format(PyExc_TypeError, "%s() does not take keyword arguments", name);
+      no_kwargs = 0;
+    }
+  }
+  return no_kwargs;
+}
+
 /* A functor is a function object with one single object argument */
 #define SWIG_Python_CallFunctor(functor, obj)	        PyObject_CallFunctionObjArgs(functor, obj, NULL);
 
 /*
   Helper for static pointer initialization for both C and C++ code, for example
   static PyObject *SWIG_STATIC_POINTER(MyVar) = NewSomething(...);
 */
@@ -1728,14 +1745,20 @@
       0,                                    /* tp_subclasses */
       0,                                    /* tp_weaklist */
       0,                                    /* tp_del */
       0,                                    /* tp_version_tag */
 #if PY_VERSION_HEX >= 0x03040000
       0,                                    /* tp_finalize */
 #endif
+#if PY_VERSION_HEX >= 0x03080000
+      0,                                    /* tp_vectorcall */
+#endif
+#if (PY_VERSION_HEX >= 0x03080000) && (PY_VERSION_HEX < 0x03090000)
+      0,                                    /* tp_print */
+#endif
 #ifdef COUNT_ALLOCS
       0,                                    /* tp_allocs */
       0,                                    /* tp_frees */
       0,                                    /* tp_maxalloc */
       0,                                    /* tp_prev */
       0                                     /* tp_next */
 #endif
@@ -1889,14 +1912,20 @@
       0,                                    /* tp_subclasses */
       0,                                    /* tp_weaklist */
       0,                                    /* tp_del */
       0,                                    /* tp_version_tag */
 #if PY_VERSION_HEX >= 0x03040000
       0,                                    /* tp_finalize */
 #endif
+#if PY_VERSION_HEX >= 0x03080000
+      0,                                    /* tp_vectorcall */
+#endif
+#if (PY_VERSION_HEX >= 0x03080000) && (PY_VERSION_HEX < 0x03090000)
+      0,                                    /* tp_print */
+#endif
 #ifdef COUNT_ALLOCS
       0,                                    /* tp_allocs */
       0,                                    /* tp_frees */
       0,                                    /* tp_maxalloc */
       0,                                    /* tp_prev */
       0                                     /* tp_next */
 #endif
@@ -2215,29 +2244,35 @@
 	if (dict == NULL) {
 	  dict = PyDict_New();
 	  *dictptr = dict;
 	  PyDict_SetItem(dict, SWIG_This(), swig_this);
 	}
       }
 #else
-      PyObject *key = SWIG_This();
-      PyObject_SetAttr(inst, key, swig_this);
+      if (PyObject_SetAttr(inst, SWIG_This(), swig_this) == -1) {
+        Py_DECREF(inst);
+        inst = 0;
+      }
 #endif
     }
   } else {
 #if PY_VERSION_HEX >= 0x03000000
     PyObject *empty_args = PyTuple_New(0);
     if (empty_args) {
       PyObject *empty_kwargs = PyDict_New();
       if (empty_kwargs) {
         inst = ((PyTypeObject *)data->newargs)->tp_new((PyTypeObject *)data->newargs, empty_args, empty_kwargs);
         Py_DECREF(empty_kwargs);
         if (inst) {
-          PyObject_SetAttr(inst, SWIG_This(), swig_this);
-          Py_TYPE(inst)->tp_flags &= ~Py_TPFLAGS_VALID_VERSION_TAG;
+          if (PyObject_SetAttr(inst, SWIG_This(), swig_this) == -1) {
+            Py_DECREF(inst);
+            inst = 0;
+          } else {
+            Py_TYPE(inst)->tp_flags &= ~Py_TPFLAGS_VALID_VERSION_TAG;
+          }
         }
       }
       Py_DECREF(empty_args);
     }
 #else
     PyObject *dict = PyDict_New();
     if (dict) {
@@ -2246,47 +2281,44 @@
       Py_DECREF(dict);
     }
 #endif
   }
   return inst;
 }
 
-SWIGRUNTIME void
+SWIGRUNTIME int
 SWIG_Python_SetSwigThis(PyObject *inst, PyObject *swig_this)
 {
- PyObject *dict;
 #if !defined(SWIG_PYTHON_SLOW_GETSET_THIS)
- PyObject **dictptr = _PyObject_GetDictPtr(inst);
- if (dictptr != NULL) {
-   dict = *dictptr;
-   if (dict == NULL) {
-     dict = PyDict_New();
-     *dictptr = dict;
-   }
-   PyDict_SetItem(dict, SWIG_This(), swig_this);
-   return;
- }
-#endif
- dict = PyObject_GetAttrString(inst, "__dict__");
- PyDict_SetItem(dict, SWIG_This(), swig_this);
- Py_DECREF(dict);
+  PyObject **dictptr = _PyObject_GetDictPtr(inst);
+  if (dictptr != NULL) {
+    PyObject *dict = *dictptr;
+    if (dict == NULL) {
+      dict = PyDict_New();
+      *dictptr = dict;
+    }
+    return PyDict_SetItem(dict, SWIG_This(), swig_this);
+  }
+#endif
+  return PyObject_SetAttr(inst, SWIG_This(), swig_this);
 } 
 
 
 SWIGINTERN PyObject *
 SWIG_Python_InitShadowInstance(PyObject *args) {
   PyObject *obj[2];
   if (!SWIG_Python_UnpackTuple(args, "swiginit", 2, 2, obj)) {
     return NULL;
   } else {
     SwigPyObject *sthis = SWIG_Python_GetSwigThis(obj[0]);
     if (sthis) {
       SwigPyObject_append((PyObject*) sthis, obj[1]);
     } else {
-      SWIG_Python_SetSwigThis(obj[0], obj[1]);
+      if (SWIG_Python_SetSwigThis(obj[0], obj[1]) != 0)
+        return NULL;
     }
     return SWIG_Py_Void();
   }
 }
 
 /* Create a new pointer object */
 
@@ -2663,15 +2695,15 @@
 
 #else
 #  define SWIG_init    init_typemap_samples
 
 #endif
 #define SWIG_name    "_typemap_samples"
 
-#define SWIGVERSION 0x040001 
+#define SWIGVERSION 0x040002 
 #define SWIG_VERSION SWIGVERSION
 
 
 #define SWIG_as_voidptr(a) (void *)((const void *)(a)) 
 #define SWIG_as_voidptrptr(a) ((void)SWIG_as_voidptr(*a),(void**)(a)) 
 
 
@@ -4194,17 +4226,19 @@
     }
     obj = PyUnicode_AsUTF8String(obj);
     if (!obj)
       return SWIG_TypeError;
     if (alloc)
       *alloc = SWIG_NEWOBJ;
 #endif
-    PyBytes_AsStringAndSize(obj, &cstr, &len);
+    if (PyBytes_AsStringAndSize(obj, &cstr, &len) == -1)
+      return SWIG_TypeError;
 #else
-    PyString_AsStringAndSize(obj, &cstr, &len);
+    if (PyString_AsStringAndSize(obj, &cstr, &len) == -1)
+      return SWIG_TypeError;
 #endif
     if (cptr) {
       if (alloc) {
 	if (*alloc == SWIG_NEWOBJ) {
 	  *cptr = (char *)memcpy(malloc((len + 1)*sizeof(char)), cstr, sizeof(char)*(len + 1));
 	  *alloc = SWIG_NEWOBJ;
 	} else {
@@ -6881,14 +6915,20 @@
         0,                                  /* tp_weaklistoffset */
         0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0, /* tp_iter -> tp_weaklist */
         0,                                  /* tp_del */
         0,                                  /* tp_version_tag */
 #if PY_VERSION_HEX >= 0x03040000
         0,                                  /* tp_finalize */
 #endif
+#if PY_VERSION_HEX >= 0x03080000
+        0,                                  /* tp_vectorcall */
+#endif
+#if (PY_VERSION_HEX >= 0x03080000) && (PY_VERSION_HEX < 0x03090000)
+        0,                                  /* tp_print */
+#endif
 #ifdef COUNT_ALLOCS
         0,                                  /* tp_allocs */
         0,                                  /* tp_frees */
         0,                                  /* tp_maxalloc */
         0,                                  /* tp_prev */
         0                                   /* tp_next */
 #endif
```


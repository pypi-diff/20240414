# Comparing `tmp/npsam-1.4.5.tar.gz` & `tmp/npsam-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npsam-1.4.5.tar", last modified: Tue Mar 12 12:57:22 2024, max compression
+gzip compressed data, was "npsam-1.4.6.tar", last modified: Sun Apr 14 19:37:08 2024, max compression
```

## Comparing `npsam-1.4.5.tar` & `npsam-1.4.6.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 12:57:22.916469 npsam-1.4.5/
--rw-rw-rw-   0        0        0    11558 2024-01-17 13:46:57.000000 npsam-1.4.5/LICENSE.txt
--rw-rw-rw-   0        0        0    16068 2024-03-12 12:57:22.916469 npsam-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     1855 2024-01-19 09:12:52.000000 npsam-1.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-12 12:57:22.731571 npsam-1.4.5/npsam/
--rw-rw-rw-   0        0        0      328 2024-02-05 12:38:38.000000 npsam-1.4.5/npsam/__init__.py
--rw-rw-rw-   0        0        0    58941 2024-03-12 12:56:41.000000 npsam-1.4.5/npsam/npsam.py
-drwxrwxrwx   0        0        0        0 2024-03-12 12:57:22.800567 npsam-1.4.5/npsam/segment_anything/
--rw-rw-rw-   0        0        0      442 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/__init__.py
--rw-rw-rw-   0        0        0    15520 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/automatic_mask_generator.py
--rw-rw-rw-   0        0        0     3048 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/build_sam.py
-drwxrwxrwx   0        0        0        0 2024-03-12 12:57:22.869598 npsam-1.4.5/npsam/segment_anything/modeling/
--rw-rw-rw-   0        0        0      396 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/modeling/__init__.py
--rw-rw-rw-   0        0        0     1522 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/modeling/common.py
--rw-rw-rw-   0        0        0    14815 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/modeling/image_encoder.py
--rw-rw-rw-   0        0        0     6791 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/modeling/mask_decoder.py
--rw-rw-rw-   0        0        0     8808 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/modeling/prompt_encoder.py
--rw-rw-rw-   0        0        0     7400 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/modeling/sam.py
--rw-rw-rw-   0        0        0     8637 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/modeling/transformer.py
--rw-rw-rw-   0        0        0    11958 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/predictor.py
-drwxrwxrwx   0        0        0        0 2024-03-12 12:57:22.916469 npsam-1.4.5/npsam/segment_anything/utils/
--rw-rw-rw-   0        0        0      202 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/utils/__init__.py
--rw-rw-rw-   0        0        0    13058 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/utils/amg.py
--rw-rw-rw-   0        0        0     5956 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/utils/onnx.py
--rw-rw-rw-   0        0        0     4074 2024-01-19 09:12:52.000000 npsam-1.4.5/npsam/segment_anything/utils/transforms.py
--rw-rw-rw-   0        0        0    20164 2024-02-09 10:37:33.000000 npsam-1.4.5/npsam/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-12 12:57:22.916469 npsam-1.4.5/npsam.egg-info/
--rw-rw-rw-   0        0        0    16068 2024-03-12 12:57:22.000000 npsam-1.4.5/npsam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      862 2024-03-12 12:57:22.000000 npsam-1.4.5/npsam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 12:57:22.000000 npsam-1.4.5/npsam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      249 2024-03-12 12:57:22.000000 npsam-1.4.5/npsam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-12 12:57:22.000000 npsam-1.4.5/npsam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1043 2024-03-12 10:01:35.000000 npsam-1.4.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-12 12:57:22.916469 npsam-1.4.5/setup.cfg
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:37:08.016373 npsam-1.4.6/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11357 2023-12-17 19:55:46.000000 npsam-1.4.6/LICENSE.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15166 2024-04-14 19:37:08.016115 npsam-1.4.6/PKG-INFO
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1184 2023-12-17 21:10:36.000000 npsam-1.4.6/README.md
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:37:08.008980 npsam-1.4.6/npsam/
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)      329 2024-04-14 19:07:23.000000 npsam-1.4.6/npsam/__init__.py
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    62035 2024-04-14 19:08:51.000000 npsam-1.4.6/npsam/npsam.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:37:08.012029 npsam-1.4.6/npsam/segment_anything/
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    63209 2024-01-02 10:53:37.000000 npsam-1.4.6/npsam/segment_anything/NPSAM.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      427 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/__init__.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    15148 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/automatic_mask_generator.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     2941 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/build_sam.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:37:08.014522 npsam-1.4.6/npsam/segment_anything/modeling/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      385 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/__init__.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     1479 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/common.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    14420 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/image_encoder.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     6615 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/mask_decoder.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8594 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/prompt_encoder.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     7226 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/sam.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     8397 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/modeling/transformer.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    11649 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/predictor.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:37:08.015585 npsam-1.4.6/npsam/segment_anything/utils/
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)      197 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/utils/__init__.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)    12712 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/utils/amg.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     5812 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/utils/onnx.py
+-rw-rw-r--   0 torbenvilladsen   (501) staff       (20)     3972 2023-12-17 19:55:46.000000 npsam-1.4.6/npsam/segment_anything/utils/transforms.py
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    20417 2024-04-14 19:08:03.000000 npsam-1.4.6/npsam/utils.py
+drwxr-xr-x   0 torbenvilladsen   (501) staff       (20)        0 2024-04-14 19:37:08.015797 npsam-1.4.6/npsam.egg-info/
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)    15166 2024-04-14 19:37:08.000000 npsam-1.4.6/npsam.egg-info/PKG-INFO
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)      894 2024-04-14 19:37:08.000000 npsam-1.4.6/npsam.egg-info/SOURCES.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)        1 2024-04-14 19:37:08.000000 npsam-1.4.6/npsam.egg-info/dependency_links.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)      249 2024-04-14 19:37:08.000000 npsam-1.4.6/npsam.egg-info/requires.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)        6 2024-04-14 19:37:08.000000 npsam-1.4.6/npsam.egg-info/top_level.txt
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)     1005 2024-04-14 19:11:59.000000 npsam-1.4.6/pyproject.toml
+-rw-r--r--   0 torbenvilladsen   (501) staff       (20)       38 2024-04-14 19:37:08.016430 npsam-1.4.6/setup.cfg
```

### Comparing `npsam-1.4.5/LICENSE.txt` & `npsam-1.4.6/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
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

### Comparing `npsam-1.4.5/PKG-INFO` & `npsam-1.4.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,273 +1,258 @@
-Metadata-Version: 2.1
-Name: npsam
-Version: 1.4.5
-Summary: NP-SAM is an easy-to-use segmentation and analysis tool for nanoparticles and more.
-Author-email: "Larsen, R. & Villadsen, T." <rasmus@inano.au.dk>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Keywords: nanoparticles,segmentation
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: numba==0.58.1
-Requires-Dist: opencv-python==4.9.0.80
-Requires-Dist: pandas==2.1.4
-Requires-Dist: matplotlib==3.8.2
-Requires-Dist: scikit-image==0.22.0
-Requires-Dist: ipympl==0.9.3
-Requires-Dist: PyQt5==5.15.10
-Requires-Dist: ultralytics==8.1.2
-Requires-Dist: jupyterlab==4.0.10
-Requires-Dist: clip==0.2.0
-Requires-Dist: piexif==1.1.3
-Requires-Dist: rosettasciio==0.1
-Requires-Dist: parse==1.20.1
-Requires-Dist: h5py==3.10.0
-Requires-Dist: tifffile==2024.1.30
-
-# NP-SAM
-
-## Introduction
-
-In this project we propose an easily implementable workflow for a fast, accurate and seamless experience of segmentation of nanoparticles.
-
-The project's experience can be significantly enhanced with the presence of a CUDA-compatible device; alternatively, Google Colab can be utilized if such a device is not accessible. For a quick access to the program and a CUDA-GPU try our Google Colab notebook. <br>
-[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/TorbenVilladsen/np-sam/blob/main/NPSAM_GoogleColab.ipynb)
-
-## Installation
-Create a new conda environment called `npsam` and activate it.
-```
-conda create -n npsam python=3.10
-conda activate npsam
-```
-**Install [PyTorch](https://pytorch.org/get-started/locally/)**. NP-SAM has been tested with Pytorch 2.1.2 and CUDA 11.8.
-
-Then install NP-SAM, and make a static link to the ipykernel
-```
-pip install npsam
-python -m ipykernel install --user --name npsam --display-name npsam
-```
-
-### Get started
-In the npsam environment execute `jupyter lab` in the terminal. This will launch jupyterlab. Try out one of the example notebooks on our GitLab.
-
-## Citation
-```
-@article{NPSAM,
-   author = {Larsen, Rasmus and Villadsen, Torben L. and Mathiesen, Jette K. and Jensen, Kirsten M. Ø and Bøjesen, Espen D.},
-   title = {NP-SAM: Implementing the Segment Anything Model for Easy Nanoparticle Segmentation in Electron Microscopy Images},
-   journal = {ChemRxiv},
-   DOI = {10.26434/chemrxiv-2023-k73qz-v2},
-   year = {2023},
-   type = {Journal Article}
-}
-```
-
-## Acknowledgment
-This repo benefits from Meta's [Segment Anything](https://github.com/facebookresearch/segment-anything) and [FastSAM](https://github.com/CASIA-IVA-Lab/FastSAM). Thanks for their great work.
-
-
+Metadata-Version: 2.1
+Name: npsam
+Version: 1.4.6
+Summary: NP-SAM is an easy-to-use segmentation and analysis tool for nanoparticles and more.
+Author-email: "Larsen, R. & Villadsen, T." <rasmus@inano.au.dk>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Keywords: nanoparticles,segmentation
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numba==0.58.1
+Requires-Dist: opencv-python==4.9.0.80
+Requires-Dist: pandas==2.1.4
+Requires-Dist: matplotlib==3.8.2
+Requires-Dist: scikit-image==0.22.0
+Requires-Dist: ipympl==0.9.3
+Requires-Dist: PyQt5==5.15.10
+Requires-Dist: ultralytics==8.1.2
+Requires-Dist: jupyterlab==4.0.10
+Requires-Dist: clip==0.2.0
+Requires-Dist: piexif==1.1.3
+Requires-Dist: rosettasciio==0.1
+Requires-Dist: parse==1.20.1
+Requires-Dist: h5py==3.10.0
+Requires-Dist: tifffile==2024.1.30
+
+# NP-SAM
+
+## Introduction
+
+In this project we propose an easily implementable workflow for a fast, accurate and seamless experience of segmentation of nanoparticles.
+
+The project's experience could be significantly enhanced with the presence of a CUDA-compatible device; alternatively, Google Colab can be utilized if such a device is not accessible. For a quick access to the program and a CUDA-GPU try our Google Colab notebook.
+
+### Get started
+In the working directory and NPSAM environment execute `jupyter lab` in the terminal. This will launch jupyterlab. 
+
+## Citation
+```
+@article{NPSAM,
+   author = {Larsen, Rasmus and Villadsen, Torben L. and Mathiesen, Jette K. and Jensen, Kirsten M. Ø and Bøjesen, Espen D.},
+   title = {NP-SAM: Implementing the Segment Anything Model for Easy Nanoparticle Segmentation in Electron Microscopy Images},
+   journal = {ChemRxiv},
+   DOI = {10.26434/chemrxiv-2023-k73qz-v2},
+   year = {2023},
+   type = {Journal Article}
+}
+```
+
+## Acknowledgment
+This repo benefits from Meta's [Segment Anything](https://github.com/facebookresearch/segment-anything) and [FastSAM](https://github.com/CASIA-IVA-Lab/FastSAM). Thanks for their great work.
+
+
```

### Comparing `npsam-1.4.5/npsam/npsam.py` & `npsam-1.4.6/npsam/npsam.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from datetime import datetime
 from PIL import Image
 from rsciio import emd, digitalmicrograph, tia
 
 from .utils import *
 
 
-
 def get_file_path(directory='./'):
     app = QApplication(sys.argv)
     fname = QFileDialog.getOpenFileNames(None, "Select a file...", directory,
                                          filter="Image files (*.png *.jpg *.jpeg *.tif *.tiff);;All files (*)")
     print(f'filepath = {fname[0]}'.replace(', ', ',\n'))
     return fname[0]
 
@@ -50,15 +49,16 @@
     try:
         if filepath.suffix == '.emd':
             file_dict = emd.file_reader(filepath.as_posix())
             for i in range(len(file_dict)):
                 data_type = file_dict[i].get('metadata').get('General').get('title')
 
                 if data_type in {'HAADF', 'Ceta'}:
-                    title = file_dict[i].get('metadata').get('General').get('original_filename').split('.')[0] + '_' + data_type
+                    title = file_dict[i].get('metadata').get('General').get('original_filename').split('.')[
+                                0] + '_' + data_type
                     data = file_dict[i].get('data')
                     data = data.astype(np.uint16)
                     image = Image.fromarray(data)
                     image.save(Path(folder_path, f'{title}.png'))
                     image_list.append(str(Path(folder_path, f"{title}.png")))
                     try:
                         scale = round(file_dict[i].get('axes')[0].get('scale'), 3)
@@ -68,15 +68,16 @@
                     except:
                         print('Could not find scaling.')
 
         elif filepath.suffix in {'.dm3', '.dm4'}:
             file_dict = digitalmicrograph.file_reader(filepath.as_posix())
             for i in range(len(file_dict)):
                 data_type = file_dict[i].get('metadata').get('General').get('title')
-                title = file_dict[i].get('metadata').get('General').get('original_filename').split('.')[0] + '_' + data_type
+                title = file_dict[i].get('metadata').get('General').get('original_filename').split('.')[
+                            0] + '_' + data_type
                 data = file_dict[i].get('data')[0]
                 data = data.astype(np.uint32)
                 image = Image.fromarray(data)
                 image.save(Path(folder_path, f'{title}.png'))
                 image_list.append(str(Path(folder_path, f"{title}.png")))
                 for j in range(len(file_dict[i].get('axes'))):
                     if file_dict[i].get('axes')[j].get('name') in {'y', 'x'}:
@@ -120,15 +121,15 @@
     Saves the masks as a compressed numpy array file to easier load it later
     '''
     filepaths = process_filepath(filepath)
     try:
         sam_checkpoint, model_type, model_name = choose_SAM_model(SAM_model, device)
     except TypeError:
         return print('Cannot run SAM because no weight is chosen.')
-    
+
     for n, filepath in enumerate(filepaths):
         files_folder = Path(filepath).parent / (Path(filepath).stem + '_files')
         files_folder.mkdir(exist_ok=True)
         if crop_and_enlarge or invert:
             image_filepaths = preprocess(filepath, crop_and_enlarge=crop_and_enlarge, invert=invert, double=double)
         else:
             image_filepaths = [filepath]
@@ -154,50 +155,56 @@
                     imgsz=int(np.ceil(max(image.shape[0], image.shape[1]) / 32) * 32),
                     conf=0.2,
                     iou=0.9,
                     verbose=False)
 
                 prompt_process = FastSAMPrompt(image, results, device=device)
 
-                masks = prompt_process.everything_prompt()[0].masks.data.cpu().numpy().transpose(1, 2, 0).astype(np.uint8)
+                masks = prompt_process.everything_prompt()[0].masks.data.cpu().numpy().transpose(1, 2, 0).astype(
+                    np.uint8)
 
                 list_of_masks = [masks[:, :, i] for i in range(masks.shape[2]) if masks[:, :, i][:, 0].sum() +
-                                 masks[:, :, i][:, -1].sum() + masks[:, :, i][0, :].sum() + masks[:, :, i][-1, :].sum() == 0]
+                                 masks[:, :, i][:, -1].sum() + masks[:, :, i][0, :].sum() + masks[:, :, i][-1,
+                                                                                            :].sum() == 0]
             else:
                 start = time()
 
                 # set up model
                 sam = sam_model_registry[model_type](checkpoint=sam_checkpoint).to(device=device)
 
-                mask_generator = SamAutomaticMaskGenerator(sam, points_per_side=PPS, min_mask_region_area=min_mask_area, **kwargs)
+                mask_generator = SamAutomaticMaskGenerator(sam, points_per_side=PPS, min_mask_region_area=min_mask_area,
+                                                           **kwargs)
 
                 masks = mask_generator.generate(image)
 
-                list_of_masks = [mask['segmentation'].astype(np.uint8) for mask in masks if mask['segmentation'][:, 0].sum() +
+                list_of_masks = [mask['segmentation'].astype(np.uint8) for mask in masks if
+                                 mask['segmentation'][:, 0].sum() +
                                  mask['segmentation'][:, -1].sum() + mask['segmentation'][0, :].sum() +
                                  mask['segmentation'][-1, :].sum() == 0]
 
             if shape_filter:
                 list_of_filtered_masks = []
                 for i in range(len(list_of_masks)):
                     labels_of_masks = skimage.measure.label(list_of_masks[i])
                     props = skimage.measure.regionprops_table(labels_of_masks, properties=['label', 'area', 'solidity'])
                     if len(props.get('label')) == 1 and (props.get('area') < 400 or props.get('solidity') > 0.95):
                         list_of_filtered_masks.append(list_of_masks[i])
                 list_of_masks = list_of_filtered_masks
 
             if len(list_of_masks) == 0:
                 elapsed_time = time() - start
-                print(f'{len(list_of_masks)} masks found for {Path(image_filepath).name}, so no masks were saved.\nIt took {format_time(elapsed_time)}')
+                print(
+                    f'{len(list_of_masks)} masks found for {Path(image_filepath).name}, so no masks were saved.\nIt took {format_time(elapsed_time)}')
             else:
                 array_of_masks = np.stack(list_of_masks, axis=-1)
                 file_p = files_folder / (Path(image_filepath).stem + '_array_of_masks.npz')
                 np.savez_compressed(file_p, array=array_of_masks)
                 segmentation = (model_name + f', PPS={PPS}' if model_name != 'fast' else model_name) + \
-                               (', C&E' if crop_and_enlarge else '') + (', invert' if invert else '') + (' x 2' if double else '')
+                               (', C&E' if crop_and_enlarge else '') + (', invert' if invert else '') + (
+                                   ' x 2' if double else '')
                 save_dictionary(filepath, {'segmentation': segmentation})
                 elapsed_time = time() - start
                 print(f'{len(list_of_masks)} masks found. It took {format_time(elapsed_time)}')
             if crop_and_enlarge:
                 os.remove(image_filepath)
             if device in {'cuda', 'cuda:0'}:
                 gc.collect()
@@ -425,22 +432,22 @@
             'moments_hu-0': 3, 'moments_hu-1': 3, 'moments_hu-2': 3,
             'moments_hu-3': 3, 'moments_hu-4': 3, 'moments_hu-5': 3,
             'moments_hu-6': 3, 'moments_weighted_hu-0': 3,
             'moments_weighted_hu-1': 3, 'moments_weighted_hu-2': 3,
             'moments_weighted_hu-3': 3, 'moments_weighted_hu-4': 3,
             'moments_weighted_hu-5': 3, 'moments_weighted_hu-6': 3,
             'orientation': 3, 'perimeter': 1, 'perimeter_crofton': 1,
-            'scaling [px/unit]':2, 'solidity': 3})
+            'scaling [px/unit]': 2, 'solidity': 3})
 
         print('Detecting areas with overlap.')
         flattened_multiple_masks = masks[masks.sum(axis=-1) > 1]
         unique_multiple_masks = nb_unique_caller(flattened_multiple_masks[::stepsize])
 
         print('Processing areas with overlap:')
-        
+
         df['overlap'] = 0
         df['overlapping_masks'] = [set() for _ in range(len(df))]
 
         overlap_counts = np.zeros(len(df), dtype=int)
 
         for n, unique in enumerate(unique_multiple_masks):
             print(f'Area {n + 1}/{len(unique_multiple_masks)}', sep=',',
@@ -479,47 +486,58 @@
         self.filepaths = process_filepath(filepath)
 
         self.labels = None
         self.vmax = None
         self.image = None
         self.fig = None
         self.ax = None
-        self.textvar = None
+        self.text = None
         self.filtered_label_image = None
+        self.buttons = {}
 
         self.min_area = None
         self.max_area = None
         self.min_solidity = None
         self.max_solidity = None
         self.min_intensity = None
         self.max_intensity = None
         self.min_eccentricity = None
         self.max_eccentricity = None
         self.max_overlap = None
         self.overlapping_masks = None
         self.overlapping_masks_dict = {'All': "Not applied", '0': 0, '1': 2, '2': 3}
+        self.removed_index = []
 
         self.ax_slider_area = None
         self.unit = None
         self.ax_slider_solidity = None
         self.ax_slider_intensity = None
         self.ax_slider_eccentricity = None
         self.ax_slider_overlap = None
         self.ax_radio_overlapping_masks = None
         self.ax_save = None
         self.ax_next = None
         self.ax_previous = None
+        self.ax_return_all_removed = None
+        self.ax_return_last_removed = None
         self.pressed_keys = set()
         self.last_interacted_slider = None
 
+        self.slider_color = '#65B6F3'
+        self.radio_color = '#387FBE'
+
+        self.directory = Path(__file__).resolve().parent / 'button_images'
+
     def get_df_params(self):
         return ((self.df['area'] >= self.min_area) & (self.df['area'] <= self.max_area) &
                 (self.df['solidity'] >= self.min_solidity) & (self.df['solidity'] <= self.max_solidity) &
                 (self.df['intensity_mean'] >= self.min_intensity) & (self.df['intensity_mean'] <= self.max_intensity) &
-                (self.df['eccentricity'] >= self.min_eccentricity) & (self.df['eccentricity'] <= self.max_eccentricity) &
+                (self.df['eccentricity'] >= self.min_eccentricity) & (
+                            self.df['eccentricity'] <= self.max_eccentricity) &
+                (~self.df['mask_index'].isin(self.removed_index)) &
                 (self.df['number_of_overlapping_masks'] == self.overlapping_masks if type(self.overlapping_masks) == int
                  else self.df['number_of_overlapping_masks'] >= 0) & (self.df['overlap'] <= self.max_overlap))
 
     def plot_df(self, df):
         mask_indices = df.index.to_numpy().astype(np.uint16)
 
         selected_masks = self.weighted_masks_rebinned[mask_indices]
@@ -527,118 +545,146 @@
         self.filtered_label_image = np.sum(selected_masks, axis=0, dtype=np.uint16)
 
         self.fig.canvas.restore_region(self.background)
         self.im_lab.set_data(self.filtered_label_image)
         self.ax['left2'].draw_artist(self.im_lab)
         self.fig.canvas.blit(self.ax['left2'].bbox)
 
+    def plot_text(self, df):
+        self.text.remove()
+        self.text = self.fig.text(0.704, 0.12, f'{self.df.shape[0] - df.shape[0]} masks removed. {df.shape[0]} remain.',
+                                  fontsize=16, horizontalalignment='center', verticalalignment='center')
+
+    def create_button(self, x, y, w, h, default_img_path, hover_img_path, click_action, rotate=False):
+        ax = plt.axes([x, y, w, h], frameon=False)
+        ax.set_axis_off()
+
+        default_img = mpimg.imread(self.directory / default_img_path)
+        hover_img = mpimg.imread(self.directory / hover_img_path)
+        if rotate:
+            default_img = np.flipud(np.fliplr(default_img))
+            hover_img = np.flipud(np.fliplr(hover_img))
+
+        img_display = ax.imshow(default_img)
+
+        self.buttons[ax] = {'default': default_img, 'hover': hover_img, 'display': img_display}
+        ax.figure.canvas.mpl_connect('button_press_event', lambda event: self.on_button_click(event, ax, click_action))
+
+    def on_hover(self, event):
+        redraw_required = False
+        for ax, img_info in self.buttons.items():
+            if event.inaxes == ax:
+                if not np.array_equal(img_info['display'].get_array(), img_info['hover']):
+                    img_info['display'].set_data(img_info['hover'])
+                    ax.draw_artist(img_info['display'])
+                    redraw_required = True
+            elif not np.array_equal(img_info['display'].get_array(), img_info['default']):
+                img_info['display'].set_data(img_info['default'])
+                ax.draw_artist(img_info['display'])
+                redraw_required = True
+        if redraw_required:
+            self.fig.canvas.update()
+
+    def on_button_click(self, event, ax, action):
+        if event.inaxes == ax:
+            action()
+
     def update_area(self, slider_area):
         self.last_interacted_slider = self.slider_area
         self.min_area = int(slider_area[0])
         self.max_area = int(slider_area[1])
 
         self.area_val_text.set_text(f"Area ({self.unit2}): ({self.min_area}, {self.max_area})")
 
         df_area = self.df.loc[self.get_df_params()]
 
-        self.textvar.remove()
-        self.textvar = self.fig.text(0.704, 0.12, f'{self.df.shape[0] - df_area.shape[0]} labels removed.'
-                                                  f' {df_area.shape[0]} remain.', fontsize=16,
-                                     horizontalalignment='center', verticalalignment='center')
+        self.plot_text(df_area)
+
         self.plot_df(df_area)
 
     def update_solidity(self, slider_solidity):
         self.last_interacted_slider = self.slider_solidity
         self.min_solidity = float(slider_solidity[0])
         self.max_solidity = float(slider_solidity[1])
 
         self.solidity_val_text.set_text(f"Solidity: ({self.min_solidity:.3f}, {self.max_solidity:.3f})")
 
         df_solidity = self.df.loc[self.get_df_params()]
 
-        self.textvar.remove()
-        self.textvar = self.fig.text(0.704, 0.12, f'{self.df.shape[0] - df_solidity.shape[0]} labels removed.'
-                                                  f' {df_solidity.shape[0]} remain.', fontsize=16,
-                                     horizontalalignment='center', verticalalignment='center')
+        self.plot_text(df_solidity)
+
         self.plot_df(df_solidity)
 
     def update_intensity(self, slider_intensity):
         self.last_interacted_slider = self.slider_intensity
         self.min_intensity = int(slider_intensity[0])
         self.max_intensity = int(slider_intensity[1])
 
         self.intensity_val_text.set_text(f"Intensity: ({self.min_intensity}, {self.max_intensity})")
 
         df_intensity = self.df.loc[self.get_df_params()]
 
-        self.textvar.remove()
-        self.textvar = self.fig.text(0.704, 0.12, f'{self.df.shape[0] - df_intensity.shape[0]} labels removed.'
-                                                  f' {df_intensity.shape[0]} remain.', fontsize=16,
-                                     horizontalalignment='center', verticalalignment='center')
+        self.plot_text(df_intensity)
+
         self.plot_df(df_intensity)
 
     def update_eccentricity(self, slider_eccentricity):
         self.last_interacted_slider = self.slider_eccentricity
         self.min_eccentricity = float(slider_eccentricity[0])
         self.max_eccentricity = float(slider_eccentricity[1])
 
         self.eccentricity_val_text.set_text(f"Eccentricity: ({self.min_eccentricity:.2f}, {self.max_eccentricity:.2f})")
 
         df_eccentricity = self.df.loc[self.get_df_params()]
 
-        self.textvar.remove()
-        self.textvar = self.fig.text(0.704, 0.12, f'{self.df.shape[0] - df_eccentricity.shape[0]} labels removed.'
-                                                  f' {df_eccentricity.shape[0]} remain.', fontsize=16,
-                                     horizontalalignment='center', verticalalignment='center')
+        self.plot_text(df_eccentricity)
 
         self.plot_df(df_eccentricity)
 
     def update_overlap(self, slider_overlap):
         self.last_interacted_slider = self.slider_overlap
         self.max_overlap = slider_overlap
 
         self.overlap_val_text.set_text(f"Overlap: {self.max_overlap}")
 
         df_overlap = self.df.loc[self.get_df_params()]
 
-        self.textvar.remove()
-        self.textvar = self.fig.text(0.704, 0.12, f'{self.df.shape[0] - df_overlap.shape[0]} labels removed.'
-                                                  f' {df_overlap.shape[0]} remain.', fontsize=16,
-                                     horizontalalignment='center', verticalalignment='center')
+        self.plot_text(df_overlap)
 
         self.plot_df(df_overlap)
 
     def update_overlapping_masks(self, label):
         self.overlapping_masks = self.overlapping_masks_dict[label]
 
         df_overlapping_masks = self.df.loc[self.get_df_params()]
 
-        self.textvar.remove()
-        self.textvar = self.fig.text(0.704, 0.12, f'{self.df.shape[0] - df_overlapping_masks.shape[0]} labels removed.'
-                                                  f' {df_overlapping_masks.shape[0]} remain.', fontsize=16,
-                                     horizontalalignment='center', verticalalignment='center')
+        self.plot_text(df_overlapping_masks)
 
         self.plot_df(df_overlapping_masks)
 
         self.fig.canvas.draw()
 
     def on_key_press(self, event):
         if self.last_interacted_slider == self.slider_overlap:
             high = self.last_interacted_slider.val
         else:
             low, high = self.last_interacted_slider.val
         self.pressed_keys.add(event.key)
 
-        if self.last_interacted_slider in {self.slider_solidity, self.slider_eccentricity}:
+        if self.last_interacted_slider == self.slider_eccentricity:
             step = 0.01
+        elif self.last_interacted_slider == self.slider_solidity:
+            step = 0.001
         else:
             step = 1
         if 'shift' in self.pressed_keys:
-            if self.last_interacted_slider in {self.slider_solidity, self.slider_eccentricity}:
+            if self.last_interacted_slider == self.slider_eccentricity:
                 step = 0.1
+            elif self.last_interacted_slider == self.slider_solidity:
+                step = 0.005
             else:
                 step = 10
 
         if event.key in {'left', 'right', 'up', 'down', 'shift+left', 'shift+right', 'shift+up', 'shift+down'}:
             if self.last_interacted_slider == self.slider_overlap:
                 if event.key in {'up', 'shift+up'}:
                     val = high
@@ -661,14 +707,54 @@
                     val = (low, high - step)
                 self.last_interacted_slider.set_val(val)
 
     def on_key_release(self, event):
         if event.key in self.pressed_keys:
             self.pressed_keys.remove(event.key)
 
+    def on_click(self, event):
+        if event.inaxes == self.ax['left2']:
+            for idx, row in self.df.iterrows():
+                if row['bbox-1'] <= event.xdata <= row['bbox-3'] and row['bbox-0'] <= event.ydata <= row['bbox-2']:
+                    self.removed_index.append(idx)
+
+                    df_removed = self.df.loc[self.get_df_params()]
+
+                    self.plot_text(df_removed)
+
+                    self.fig.canvas.draw_idle()
+
+                    self.plot_df(df_removed)
+                    break
+
+    def return_all_removed(self):
+        self.removed_index = []
+
+        df_removed = self.df.loc[self.get_df_params()]
+
+        self.plot_text(df_removed)
+
+        self.fig.canvas.draw_idle()
+
+        self.plot_df(df_removed)
+
+    def return_last_removed(self):
+        try:
+            self.removed_index.pop()
+
+            df_removed = self.df.loc[self.get_df_params()]
+
+            self.plot_text(df_removed)
+
+            self.fig.canvas.draw_idle()
+
+            self.plot_df(df_removed)
+        except IndexError:
+            pass
+
     def update_button(self):
         df_filtered = self.df.loc[self.get_df_params()]
         self.plot_df(df_filtered)
 
         filters = {
             'min_area': self.min_area,
             'max_area': self.max_area,
@@ -697,46 +783,46 @@
         self.file_p = self.files_folder / (Path(self.filepath).stem + '_filtered_masks.tif')
         tifffile.imwrite(self.file_p, self.filtered_label_image.astype('uint16'))
         self.file_p = self.files_folder / (Path(self.filepath).stem + '_filtered_binary_labels.tif')
         tifffile.imwrite(self.file_p, ((self.filtered_label_image > 0) * 255).astype('uint8'))
 
         plt.close()
 
-    def final_save(self, save_button):
+    def final_save(self):
         self.update_button()
 
-    def update_next(self, next_button):
+    def update_next(self):
         self.update_button()
 
         self.image_number += 1
 
         self.filter()
 
-    def update_previous(self, previous_button):
+    def update_previous(self):
         self.update_button()
 
         self.image_number -= 1
 
         self.filter()
 
-    def create_area_slider(self, ax, df):
+    def create_area_slider(self, ax):
         self.unit = self.df.loc[0, 'unit']
         self.unit2 = self.unit + "$^2$" if self.unit != "px" else self.unit
 
         self.slider_area = RangeSlider(ax, '', valmin=self.min_area, valmax=self.max_area, valstep=1,
                                        valinit=(self.min_area_init, self.max_area_init))
         self.slider_area.on_changed(self.update_area)
 
         self.area_val_text = ax.text(0, 1.12, f"Area ({self.unit2}): ({self.min_area}, {self.max_area})",
                                      fontsize=14, ha='left', va='center', transform=ax.transAxes)
         self.slider_area.valtext.set_visible(False)
         self.update_area((self.min_area_init, self.max_area_init))
 
     def create_solidity_slider(self, ax):
-        self.slider_solidity = RangeSlider(ax, "", valmin=self.min_solidity, valmax=1, valstep=0.001,
+        self.slider_solidity = RangeSlider(ax, "", valmin=self.min_solidity, valmax=self.max_solidity, valstep=0.001,
                                            valinit=(self.min_solidity_init, self.max_solidity_init))
         self.slider_solidity.on_changed(self.update_solidity)
 
         self.solidity_val_text = ax.text(0, 1.12, f"Solidity: ({self.min_solidity:.3f}, {self.max_solidity:.3f})",
                                          fontsize=14, ha='left', va='center', transform=ax.transAxes)
         self.slider_solidity.valtext.set_visible(False)
         self.update_solidity((self.min_solidity_init, self.max_solidity_init))
@@ -748,19 +834,21 @@
 
         self.intensity_val_text = ax.text(0, 1.12, f"Intensity slider: ({self.min_intensity}, {self.max_intensity})",
                                           fontsize=14, ha='left', va='center', transform=ax.transAxes)
         self.slider_intensity.valtext.set_visible(False)
         self.update_intensity((self.min_intensity_init, self.max_intensity_init))
 
     def create_eccentricity_slider(self, ax):
-        self.slider_eccentricity = RangeSlider(ax, "", valmin=self.min_eccentricity, valmax=self.max_eccentricity, valstep=0.01,
+        self.slider_eccentricity = RangeSlider(ax, "", valmin=self.min_eccentricity, valmax=self.max_eccentricity,
+                                               valstep=0.01,
                                                valinit=(self.min_eccentricity_init, self.max_eccentricity_init))
         self.slider_eccentricity.on_changed(self.update_eccentricity)
 
-        self.eccentricity_val_text = ax.text(0, 1.12, f"Eccentricity: ({self.min_eccentricity:.2f}, {self.max_eccentricity:.2f})",
+        self.eccentricity_val_text = ax.text(0, 1.12,
+                                             f"Eccentricity: ({self.min_eccentricity:.2f}, {self.max_eccentricity:.2f})",
                                              fontsize=14, ha='left', va='center', transform=ax.transAxes)
         self.slider_eccentricity.valtext.set_visible(False)
         self.update_eccentricity((self.min_eccentricity_init, self.max_eccentricity_init))
 
     def create_overlap_slider(self, ax):
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", UserWarning)
@@ -777,15 +865,16 @@
     def create_overlapping_masks_radio(self, ax):
         ax.set_aspect('equal')
         if type(self.overlapping_masks_init) == str:
             self.overlapping_masks_init = -1
         elif self.overlapping_masks_init > 2:
             self.overlapping_masks_init = -1
         self.radio_overlapping_masks = RadioButtons(ax, ('All', '0', '1', '2'),
-                                                    active=self.overlapping_masks_init + 1, activecolor='#1F77B4')
+                                                    active=self.overlapping_masks_init + 1,
+                                                    activecolor=self.radio_color)
 
         dists = [0, 0.12, 0.235, 0.35]
         for i, (circle, label) in enumerate(
                 zip(self.radio_overlapping_masks.circles, self.radio_overlapping_masks.labels)):
             new_x = 0.6 + dists[i]
             new_y = 0.5
             circle.set_center((new_x, new_y))
@@ -795,29 +884,14 @@
 
         self.overlapping_masks_val_text = ax.text(0, 0.5, "Number of overlapping masks:",
                                                   fontsize=14, ha='left', va='center', transform=ax.transAxes)
 
         self.radio_overlapping_masks.on_clicked(self.update_overlapping_masks)
         self.update_overlapping_masks(['All', '0', '1', '2'][self.overlapping_masks_init + 1])
 
-    def create_save_button(self, ax):
-        self.save_button = Button(ax, 'Save and\nclose', color='#A2CD56', hovercolor='#79B356')
-        self.save_button.label.set_fontsize(18)
-        self.save_button.on_clicked(self.final_save)
-
-    def create_next_button(self, ax):
-        self.next_button = Button(ax, 'Next', color='#A2CD56', hovercolor='#79B356')
-        self.next_button.label.set_fontsize(18)
-        self.next_button.on_clicked(self.update_next)
-
-    def create_previous_button(self, ax):
-        self.previous_button = Button(ax, 'Previous', color='#F0B54A', hovercolor='#DC9834')
-        self.previous_button.label.set_fontsize(18)
-        self.previous_button.on_clicked(self.update_previous)
-
     def initiate_filter_values(self):
         self.min_area_init = self.min_area
         self.max_area_init = self.max_area
         self.min_solidity_init = self.min_solidity
         self.max_solidity_init = self.max_solidity
         self.min_intensity_init = self.min_intensity
         self.max_intensity_init = self.max_intensity
@@ -834,55 +908,60 @@
             self.max_intensity_init = self.filters_init['max_intensity']
             self.min_eccentricity_init = self.filters_init['min_eccentricity']
             self.max_eccentricity_init = self.filters_init['max_eccentricity']
             self.max_overlap_init = self.filters_init['overlap']
             self.overlapping_masks_init = self.filters_init['overlapping_masks']
 
     def start_plot(self, image, labels):
-        self.fig, self.ax = plt.subplot_mosaic([['left', 'right'], ['left2', 'right2']],
-                                               constrained_layout=True, figsize=(12, 9))
+        self.fig, self.ax = plt.subplot_mosaic([['left', 'right'], ['left2', 'right2'], ['.', '.']],
+                                               gridspec_kw=dict(height_ratios=[1, 1, 0.1]),
+                                               constrained_layout=True, figsize=(12, 10))
 
         self.ax['left'].imshow(image, cmap='gray')
         self.vmax = labels.max()
         self.ax['right'].imshow(labels, cmap=self.label_cmap, interpolation='nearest', vmin=0, vmax=self.vmax)
         self.im_lab = self.ax['left2'].imshow(self.filtered_masks_rebinned, cmap=self.label_cmap,
                                               interpolation='nearest', vmin=0, vmax=self.vmax)
 
         self.fig.canvas.draw()
         self.background = self.fig.canvas.copy_from_bbox(self.ax['left2'].bbox)
 
         for axis in self.ax:
             self.ax[axis].axis('off')
 
-        self.ax_slider_area = plt.axes([0.525, 0.430, 0.45, 0.03], facecolor='teal')
-        self.ax_slider_solidity = plt.axes([0.525, 0.375, 0.45, 0.03], facecolor='teal')
-        self.ax_slider_intensity = plt.axes([0.525, 0.320, 0.45, 0.03], facecolor='teal')
-        self.ax_slider_eccentricity = plt.axes([0.525, 0.265, 0.45, 0.03], facecolor='teal')
-        self.ax_slider_overlap = plt.axes([0.525, 0.210, 0.45, 0.03], facecolor='teal')
+        self.ax_slider_area = plt.axes([0.525, 0.430, 0.45, 0.03], facecolor=self.slider_color)
+        self.ax_slider_solidity = plt.axes([0.525, 0.375, 0.45, 0.03], facecolor=self.slider_color)
+        self.ax_slider_intensity = plt.axes([0.525, 0.320, 0.45, 0.03], facecolor=self.slider_color)
+        self.ax_slider_eccentricity = plt.axes([0.525, 0.265, 0.45, 0.03], facecolor=self.slider_color)
+        self.ax_slider_overlap = plt.axes([0.525, 0.210, 0.45, 0.03], facecolor=self.slider_color)
         self.ax_radio_overlapping_masks = plt.axes([0.5, -0.12, 0.5, 0.6], frameon=False)
 
-        self.ax_save = plt.axes([0.835, 0.01, 0.14, 0.085])
-        self.create_save_button(self.ax_save)
+        self.create_button(0.835, 0.01, 0.14, 0.085, 'Save_close.png', 'Save_close_dark.png', self.final_save)
+
         if self.image_number < len(self.filepaths):
-            self.ax_next = plt.axes([0.68, 0.01, 0.14, 0.085])
-            self.create_next_button(self.ax_next)
+            self.create_button(0.68, 0.01, 0.14, 0.085, 'arrow.png', 'arrow_dark.png', self.update_next)
+
         if self.image_number != 1:
-            self.ax_previous = plt.axes([0.525, 0.01, 0.14, 0.085])
-            self.create_previous_button(self.ax_previous)
+            self.create_button(0.525, 0.01, 0.14, 0.085, 'arrow.png', 'arrow_dark.png', self.update_previous,
+                               rotate=True)
+
+        self.create_button(0.1, 0.0, 0.10, 0.05, 'plus_one.png', 'plus_one_dark.png', self.return_last_removed)
+
+        self.create_button(0.3, 0.0, 0.10, 0.05, 'plus_all.png', 'plus_all_dark.png', self.return_all_removed)
 
         self.min_area = math.floor(self.df['area'].min())
         self.max_area = math.ceil(self.df['area'].max())
 
         self.min_intensity = math.floor(self.df['intensity_mean'].min())
         self.max_intensity = math.ceil(self.df['intensity_mean'].max())
 
         self.max_overlap = math.ceil(self.df['overlap'].max())
 
-        self.textvar = self.fig.text(0.704, 0.12, f'{self.df.shape[0]} labels found.',
-                                     horizontalalignment='center', verticalalignment='center', fontsize=16)
+        self.text = self.fig.text(0.704, 0.12, f'{self.df.shape[0]} masks found.',
+                                  horizontalalignment='center', verticalalignment='center', fontsize=16)
 
         self.min_solidity = self.df['solidity'].min()
         self.max_solidity = self.df['solidity'].max()
 
         self.min_eccentricity = self.df['eccentricity'].min()
         self.max_eccentricity = self.df['eccentricity'].max()
 
@@ -890,45 +969,48 @@
 
         self.initiate_filter_values()
 
         self.create_solidity_slider(self.ax_slider_solidity)
         self.create_intensity_slider(self.ax_slider_intensity)
         self.create_eccentricity_slider(self.ax_slider_eccentricity)
         self.create_overlap_slider(self.ax_slider_overlap)
-        self.create_area_slider(self.ax_slider_area, self.df)
+        self.create_area_slider(self.ax_slider_area)
         self.create_overlapping_masks_radio(self.ax_radio_overlapping_masks)
 
         string_title = f'Image number {self.image_number} out of {len(self.filepaths)} - {Path(self.filepath).name}'
 
         plt.suptitle(string_title, fontsize=16)
 
         self.fig.canvas.mpl_connect('key_press_event', self.on_key_press)
         self.fig.canvas.mpl_connect('key_release_event', self.on_key_release)
+        self.fig.canvas.mpl_connect('button_press_event', self.on_click)
+        self.fig.canvas.mpl_connect('motion_notify_event', self.on_hover)
 
         plt.show()
 
     def filter(self):
         self.filepath = self.filepaths[self.image_number - 1]
         self.files_folder = Path(self.filepath).parent / (Path(self.filepath).stem + '_files')
         self.file_p = self.files_folder / (Path(self.filepath).stem + '_raw_dataframe.csv')
         self.df = pd.read_csv(self.file_p)
+        self.removed_rows = pd.DataFrame(columns=self.df.columns)
 
         self.file_p = self.files_folder / (Path(self.filepath).stem + '_array_of_masks.npz')
-        
+
         self.masks = np.load(self.file_p)['array']
         self.masks = np.moveaxis(self.masks, -1, 0)
 
         self.weights = (np.arange(1, self.masks.shape[0] + 1)[:, np.newaxis, np.newaxis]).astype(np.uint16)
 
         self.weighted_masks = self.masks * self.weights
 
-        self.weighted_masks_rebinned = self.weighted_masks[:,::4,::4]
+        self.weighted_masks_rebinned = self.weighted_masks[:, ::4, ::4]
 
         self.labels = np.sum(self.weighted_masks, axis=0, dtype=np.uint16)
-        
+
         self.filtered_masks_rebinned = self.labels
 
         self.image = load_image(self.filepath)
 
         self.filters_init = load_dictionary(str(self.filepath))
 
         self.start_plot(self.image, self.labels)
@@ -949,15 +1031,16 @@
                 if type(entry) != dict:
                     print('The list entries must be dictionaries containing the filter conditions.')
                     return None
         elif len(conditions) == 1:
             conditions = conditions * len(filepaths)
             print('The filtering conditions will be used for all images.')
         else:
-            print('The length of the list with filtering conditions does not have the same length as the list with image filepaths.')
+            print(
+                'The length of the list with filtering conditions does not have the same length as the list with image filepaths.')
             return None
 
     for filter_conditions, filepath in zip(conditions, filepaths):
         files_folder = Path(filepath).parent / (Path(filepath).stem + '_files')
         file_p = files_folder / (Path(filepath).stem + '_raw_dataframe.csv')
         df = pd.read_csv(file_p)
 
@@ -978,17 +1061,20 @@
                    'overlapping_masks': "Not applied",
                    'scaling': df['scaling [px/unit]'].to_list()[1]}
 
         filters.update(filter_conditions)
 
         filtered_df = df[((df['area'] >= filters['min_area']) & (df['area'] <= filters['max_area']) &
                           (df['solidity'] >= filters['min_solidity']) & (df['solidity'] <= filters['max_solidity']) &
-                          (df['intensity_mean'] >= filters['min_intensity']) & (df['intensity_mean'] <= filters['max_intensity']) &
-                          (df['eccentricity'] >= filters['min_eccentricity']) & (df['eccentricity'] <= filters['max_eccentricity']) &
-                          (df['number_of_overlapping_masks'] == filters['overlapping_masks'] if type(filters['overlapping_masks']) == int
+                          (df['intensity_mean'] >= filters['min_intensity']) & (
+                                      df['intensity_mean'] <= filters['max_intensity']) &
+                          (df['eccentricity'] >= filters['min_eccentricity']) & (
+                                      df['eccentricity'] <= filters['max_eccentricity']) &
+                          (df['number_of_overlapping_masks'] == filters['overlapping_masks'] if type(
+                              filters['overlapping_masks']) == int
                            else df['number_of_overlapping_masks'] >= 0) & (df['overlap'] <= filters['overlap']))]
 
         filters.update({'removed': df.shape[0] - filtered_df.shape[0], 'remain': filtered_df.shape[0]})
 
         filtered_label_image = np.zeros(weighted_masks[0].shape)
         for n in filtered_df.index.to_list():
             filtered_label_image += weighted_masks[n]
@@ -1009,15 +1095,14 @@
 
     if property_list == ['all']:
         property_list = ['area', 'area_convex', 'axis_major_length', 'axis_minor_length',
                          'eccentricity', 'equivalent_diameter_area', 'extent', 'feret_diameter_max',
                          'intensity_max', 'intensity_mean', 'intensity_min', 'orientation',
                          'perimeter', 'perimeter_crofton', 'solidity', 'overlap']
 
-
     for n, property in enumerate(property_list):
         if property == 'intensity':
             property_list[n] = 'intensity_mean'
         elif property == 'diameter':
             property_list[n] = 'equivalent_diameter_area'
         elif property == 'max diameter':
             property_list[n] = 'feret_diameter_max'
@@ -1056,25 +1141,49 @@
         else:
             file_p = files_folder / (Path(filepath).stem + '_overview' + stamp + '.pdf')
     else:
         if len(filepaths) > 1:
             file_p = Path(filepaths[0]).parent / (Path(filepaths[0]).parent.name + '_overview' + '.pdf')
         else:
             file_p = files_folder / (Path(filepath).stem + '_overview' + '.pdf')
-    master_pp = PdfPages(file_p)
+
+    def save_image():
+        if timestamp:
+            d = datetime.now()
+            stamp = str(d.year) + str(d.month) + str(d.day) + '-' + str(d.hour) + str(d.minute) + str(d.second)
+            if len(filepaths) > 1:
+                file_p = Path(filepaths[0]).parent / (Path(filepaths[0]).parent.name + '_overview' + stamp + '.pdf')
+            else:
+                file_p = files_folder / (Path(filepath).stem + '_overview' + stamp + '.pdf')
+        else:
+            if len(filepaths) > 1:
+                file_p = Path(filepaths[0]).parent / (Path(filepaths[0]).parent.name + '_overview' + '.pdf')
+            else:
+                file_p = files_folder / (Path(filepath).stem + '_overview' + '.pdf')
+
+        p = PdfPages(file_p)
+
+        fig_nums = plt.get_fignums()
+        figs = [plt.figure(n) for n in fig_nums]
+
+        for fig in figs:
+            fig.savefig(p, format='pdf')
+
+        p.close()
 
     unit = master_df['unit'].to_list()[0]
     unit2 = unit + '$^2$' if unit != 'px' else unit
     name_dict = {'area': f'area ({unit2})', 'area_convex': f'convex area ({unit2})', 'eccentricity': 'eccentricity',
                  'solidity': 'solidity', 'intensity_mean': 'mean intensity', 'overlap': 'overlap (px)',
                  'equivalent_diameter_area': f'area equivalent diameter ({unit})',
                  'feret_diameter_max': f'Max diameter (Feret) ({unit})', 'orientation': 'orientation',
                  'perimeter': f'perimeter ({unit})', 'perimeter_crofton': f'crofton perimeter ({unit})',
                  'axis_major_length': f'Major axis length ({unit})', 'axis_minor_length': f'Minor axis length ({unit})',
-                 'extent': 'Ratio of pixels in the mask the pixels in the bounding box', 'intensity_max':'Max intensity of the mask',
+                 'extent': 'Ratio of pixels in the mask the pixels in the bounding box',
+                 'intensity_max': 'Max intensity of the mask',
                  'intensity_min': 'minimum intensity of the mask', 'overlap': f'amount of overlap ({unit2})'}
     for n, prop in enumerate(property_list):
         fig, ax = plt.subplots(figsize=(12, 9))
         ax.set_xlabel(name_dict.get(prop).capitalize(), fontsize=16)
         ax.set_title(f'Histogram of {name_dict.get(prop)} for all images', fontsize=18)
         master_df[prop].hist(bins=bin_list[n], ax=ax)
         ax.grid(False)
@@ -1103,50 +1212,48 @@
             elif val < 10:
                 return f"{val:.2f}"
             elif 10 <= val < 100:
                 return f"{val:.1f}"
             elif 100 <= val:
                 return f"{int(val)}"
 
-
         x_r = 1 - len(f'Upper quantile: {format_value(q3)}') * 0.0108
         x_m = x_r - 0.025 - len(f'Sum: {format_value(total_sum)}') * 0.0108 if total_sum > 100000000 else x_r - 0.155
         x_l = x_m - 0.055 - len(f'Sum: {format_value(variance)}') * 0.0108 if variance > 1000000000000 else x_m - 0.22
 
         stats_text_left = (f"Mean: {format_value(mean)}\nStd Dev: {format_value(std_dev)}\n"
                            f"Median: {format_value(median)}\nVariance: {format_value(variance)}\n"
-                           f"Coeff of Variation: {format_value(coeff_variation)}")
+                           f"Coeff of Variation: {format_value(coeff_variation)}\n"
+                           f"Total number of masks: {len(master_df['area'].to_list())}")
 
         stats_text_middle = (f"Skewness: {format_value(skewness)}\nKurtosis: {format_value(kurtosis)}\n"
                              f"Count: {count}\nSum: {format_value(total_sum)}\nIQR: {format_value(iqr)}")
 
         stats_text_right = (f"Lower quantile: {format_value(q1)}\nUpper quantile: {format_value(q3)}\n"
                             f"Min: {format_value(minimum)}\nMax: {format_value(maximum)}\n"
                             f"Range: {format_value(data_range)}")
         n = 'i' * int((194 * (1 - x_l + 0.011)))
 
-        text = f"{n}\n{n}\n{n}\n{n}\n{n}"
+        text = f"{n}\n{n}\n{n}\n{n}\n{n}\n{n}"
         text_properties = {
             'fontsize': 12,
-            'color':'none',
+            'color': 'none',
             'verticalalignment': 'top',
             'bbox': dict(boxstyle="round,pad=0.3", edgecolor="black", facecolor="white", alpha=0.5)
         }
 
         plt.text(x_l, 0.98, text, transform=plt.gca().transAxes, **text_properties)
         plt.text(x_l, 0.98, stats_text_left, horizontalalignment='left',
                  verticalalignment='top', transform=plt.gca().transAxes, fontsize=12)
         plt.text(x_m, 0.98, stats_text_middle, horizontalalignment='left',
                  verticalalignment='top', transform=plt.gca().transAxes, fontsize=12)
         plt.text(x_r, 0.98, stats_text_right, horizontalalignment='left',
                  verticalalignment='top', transform=plt.gca().transAxes, fontsize=12)
 
-
         plt.show()
-        master_pp.savefig(fig)
 
     for filepath in filepaths:
         img = load_image(filepath)
         files_folder = Path(filepath).parent / (Path(filepath).stem + '_files')
         file_p = files_folder / (Path(filepath).stem + '_filtered_dataframe.csv')
         df_filtered = pd.read_csv(file_p)
         file_p = files_folder / (Path(filepath).stem + '_filtered_masks.png')
@@ -1187,15 +1294,15 @@
         segmentation = filters['segmentation']
 
         x1 = 0.5845
         x2 = 0.8
         fig.text(x1, 0.495, 'Used parameter values:', fontsize=18)
 
         fig.text(x1, 0.455, 'Segmentation:', fontsize=18)
-        fig.text(x2, 0.455, segmentation, fontsize=18)
+        fig.text(0.75, 0.455, segmentation, fontsize=18)
 
         fig.text(x1, 0.415, f'Area ({unit2}):', fontsize=18)
         fig.text(x2, 0.415, f'({round(min_area, 1)}, {round(max_area, 1)})', fontsize=18)
 
         fig.text(x1, 0.375, 'Solidity:', fontsize=18)
         fig.text(x2, 0.375, f'({min_solidity}, {max_solidity})', fontsize=18)
 
@@ -1213,10 +1320,8 @@
 
         fig.text(x1, 0.145, f'Scaling (px/{unit}):', fontsize=18)
         fig.text(x2, 0.145, f'{scaling}', fontsize=18)
         fig.text(0.63, 0.055, f'{removed} masks removed.\n {remain} remain.', fontsize=18, multialignment='center')
 
         plt.show()
 
-        master_pp.savefig(fig)
-
-    master_pp.close()
+    save_image()
```

### Comparing `npsam-1.4.5/npsam/segment_anything/automatic_mask_generator.py` & `npsam-1.4.6/npsam/segment_anything/automatic_mask_generator.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,372 +1,372 @@
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-# All rights reserved.
-
-# This source code is licensed under the license found in the
-# LICENSE file in the root directory of this source tree.
-
-import numpy as np
-import torch
-from torchvision.ops.boxes import batched_nms, box_area  # type: ignore
-
-from typing import Any, Dict, List, Optional, Tuple
-
-from .modeling import Sam
-from .predictor import SamPredictor
-from .utils.amg import (
-    MaskData,
-    area_from_rle,
-    batch_iterator,
-    batched_mask_to_box,
-    box_xyxy_to_xywh,
-    build_all_layer_point_grids,
-    calculate_stability_score,
-    coco_encode_rle,
-    generate_crop_boxes,
-    is_box_near_crop_edge,
-    mask_to_rle_pytorch,
-    remove_small_regions,
-    rle_to_mask,
-    uncrop_boxes_xyxy,
-    uncrop_masks,
-    uncrop_points,
-)
-
-
-class SamAutomaticMaskGenerator:
-    def __init__(
-        self,
-        model: Sam,
-        points_per_side: Optional[int] = 32,
-        points_per_batch: int = 64,
-        pred_iou_thresh: float = 0.88,
-        stability_score_thresh: float = 0.95,
-        stability_score_offset: float = 1.0,
-        box_nms_thresh: float = 0.7,
-        crop_n_layers: int = 0,
-        crop_nms_thresh: float = 0.7,
-        crop_overlap_ratio: float = 512 / 1500,
-        crop_n_points_downscale_factor: int = 1,
-        point_grids: Optional[List[np.ndarray]] = None,
-        min_mask_region_area: int = 0,
-        output_mode: str = "binary_mask",
-    ) -> None:
-        """
-        Using a SAM model, generates masks for the entire image.
-        Generates a grid of point prompts over the image, then filters
-        low quality and duplicate masks. The default settings are chosen
-        for SAM with a ViT-H backbone.
-
-        Arguments:
-          model (Sam): The SAM model to use for mask prediction.
-          points_per_side (int or None): The number of points to be sampled
-            along one side of the image. The total number of points is
-            points_per_side**2. If None, 'point_grids' must provide explicit
-            point sampling.
-          points_per_batch (int): Sets the number of points run simultaneously
-            by the model. Higher numbers may be faster but use more GPU memory.
-          pred_iou_thresh (float): A filtering threshold in [0,1], using the
-            model's predicted mask quality.
-          stability_score_thresh (float): A filtering threshold in [0,1], using
-            the stability of the mask under changes to the cutoff used to binarize
-            the model's mask predictions.
-          stability_score_offset (float): The amount to shift the cutoff when
-            calculated the stability score.
-          box_nms_thresh (float): The box IoU cutoff used by non-maximal
-            suppression to filter duplicate masks.
-          crop_n_layers (int): If >0, mask prediction will be run again on
-            crops of the image. Sets the number of layers to run, where each
-            layer has 2**i_layer number of image crops.
-          crop_nms_thresh (float): The box IoU cutoff used by non-maximal
-            suppression to filter duplicate masks between different crops.
-          crop_overlap_ratio (float): Sets the degree to which crops overlap.
-            In the first crop layer, crops will overlap by this fraction of
-            the image length. Later layers with more crops scale down this overlap.
-          crop_n_points_downscale_factor (int): The number of points-per-side
-            sampled in layer n is scaled down by crop_n_points_downscale_factor**n.
-          point_grids (list(np.ndarray) or None): A list over explicit grids
-            of points used for sampling, normalized to [0,1]. The nth grid in the
-            list is used in the nth crop layer. Exclusive with points_per_side.
-          min_mask_region_area (int): If >0, postprocessing will be applied
-            to remove disconnected regions and holes in masks with area smaller
-            than min_mask_region_area. Requires opencv.
-          output_mode (str): The form masks are returned in. Can be 'binary_mask',
-            'uncompressed_rle', or 'coco_rle'. 'coco_rle' requires pycocotools.
-            For large resolutions, 'binary_mask' may consume large amounts of
-            memory.
-        """
-
-        assert (points_per_side is None) != (
-            point_grids is None
-        ), "Exactly one of points_per_side or point_grid must be provided."
-        if points_per_side is not None:
-            self.point_grids = build_all_layer_point_grids(
-                points_per_side,
-                crop_n_layers,
-                crop_n_points_downscale_factor,
-            )
-        elif point_grids is not None:
-            self.point_grids = point_grids
-        else:
-            raise ValueError("Can't have both points_per_side and point_grid be None.")
-
-        assert output_mode in [
-            "binary_mask",
-            "uncompressed_rle",
-            "coco_rle",
-        ], f"Unknown output_mode {output_mode}."
-        if output_mode == "coco_rle":
-            from pycocotools import mask as mask_utils  # type: ignore # noqa: F401
-
-        if min_mask_region_area > 0:
-            import cv2  # type: ignore # noqa: F401
-
-        self.predictor = SamPredictor(model)
-        self.points_per_batch = points_per_batch
-        self.pred_iou_thresh = pred_iou_thresh
-        self.stability_score_thresh = stability_score_thresh
-        self.stability_score_offset = stability_score_offset
-        self.box_nms_thresh = box_nms_thresh
-        self.crop_n_layers = crop_n_layers
-        self.crop_nms_thresh = crop_nms_thresh
-        self.crop_overlap_ratio = crop_overlap_ratio
-        self.crop_n_points_downscale_factor = crop_n_points_downscale_factor
-        self.min_mask_region_area = min_mask_region_area
-        self.output_mode = output_mode
-
-    @torch.no_grad()
-    def generate(self, image: np.ndarray) -> List[Dict[str, Any]]:
-        """
-        Generates masks for the given image.
-
-        Arguments:
-          image (np.ndarray): The image to generate masks for, in HWC uint8 format.
-
-        Returns:
-           list(dict(str, any)): A list over records for masks. Each record is
-             a dict containing the following keys:
-               segmentation (dict(str, any) or np.ndarray): The mask. If
-                 output_mode='binary_mask', is an array of shape HW. Otherwise,
-                 is a dictionary containing the RLE.
-               bbox (list(float)): The box around the mask, in XYWH format.
-               area (int): The area in pixels of the mask.
-               predicted_iou (float): The model's own prediction of the mask's
-                 quality. This is filtered by the pred_iou_thresh parameter.
-               point_coords (list(list(float))): The point coordinates input
-                 to the model to generate this mask.
-               stability_score (float): A measure of the mask's quality. This
-                 is filtered on using the stability_score_thresh parameter.
-               crop_box (list(float)): The crop of the image used to generate
-                 the mask, given in XYWH format.
-        """
-
-        # Generate masks
-        mask_data = self._generate_masks(image)
-
-        # Filter small disconnected regions and holes in masks
-        if self.min_mask_region_area > 0:
-            mask_data = self.postprocess_small_regions(
-                mask_data,
-                self.min_mask_region_area,
-                max(self.box_nms_thresh, self.crop_nms_thresh),
-            )
-
-        # Encode masks
-        if self.output_mode == "coco_rle":
-            mask_data["segmentations"] = [coco_encode_rle(rle) for rle in mask_data["rles"]]
-        elif self.output_mode == "binary_mask":
-            mask_data["segmentations"] = [rle_to_mask(rle) for rle in mask_data["rles"]]
-        else:
-            mask_data["segmentations"] = mask_data["rles"]
-
-        # Write mask records
-        curr_anns = []
-        for idx in range(len(mask_data["segmentations"])):
-            ann = {
-                "segmentation": mask_data["segmentations"][idx],
-                "area": area_from_rle(mask_data["rles"][idx]),
-                "bbox": box_xyxy_to_xywh(mask_data["boxes"][idx]).tolist(),
-                "predicted_iou": mask_data["iou_preds"][idx].item(),
-                "point_coords": [mask_data["points"][idx].tolist()],
-                "stability_score": mask_data["stability_score"][idx].item(),
-                "crop_box": box_xyxy_to_xywh(mask_data["crop_boxes"][idx]).tolist(),
-            }
-            curr_anns.append(ann)
-
-        return curr_anns
-
-    def _generate_masks(self, image: np.ndarray) -> MaskData:
-        orig_size = image.shape[:2]
-        crop_boxes, layer_idxs = generate_crop_boxes(
-            orig_size, self.crop_n_layers, self.crop_overlap_ratio
-        )
-
-        # Iterate over image crops
-        data = MaskData()
-        for crop_box, layer_idx in zip(crop_boxes, layer_idxs):
-            crop_data = self._process_crop(image, crop_box, layer_idx, orig_size)
-            data.cat(crop_data)
-
-        # Remove duplicate masks between crops
-        if len(crop_boxes) > 1:
-            # Prefer masks from smaller crops
-            scores = 1 / box_area(data["crop_boxes"])
-            scores = scores.to(data["boxes"].device)
-            keep_by_nms = batched_nms(
-                data["boxes"].float(),
-                scores,
-                torch.zeros_like(data["boxes"][:, 0]),  # categories
-                iou_threshold=self.crop_nms_thresh,
-            )
-            data.filter(keep_by_nms)
-
-        data.to_numpy()
-        return data
-
-    def _process_crop(
-        self,
-        image: np.ndarray,
-        crop_box: List[int],
-        crop_layer_idx: int,
-        orig_size: Tuple[int, ...],
-    ) -> MaskData:
-        # Crop the image and calculate embeddings
-        x0, y0, x1, y1 = crop_box
-        cropped_im = image[y0:y1, x0:x1, :]
-        cropped_im_size = cropped_im.shape[:2]
-        self.predictor.set_image(cropped_im)
-
-        # Get points for this crop
-        points_scale = np.array(cropped_im_size)[None, ::-1]
-        points_for_image = self.point_grids[crop_layer_idx] * points_scale
-
-        # Generate masks for this crop in batches
-        data = MaskData()
-        for (points,) in batch_iterator(self.points_per_batch, points_for_image):
-            batch_data = self._process_batch(points, cropped_im_size, crop_box, orig_size)
-            data.cat(batch_data)
-            del batch_data
-        self.predictor.reset_image()
-
-        # Remove duplicates within this crop.
-        keep_by_nms = batched_nms(
-            data["boxes"].float(),
-            data["iou_preds"],
-            torch.zeros_like(data["boxes"][:, 0]),  # categories
-            iou_threshold=self.box_nms_thresh,
-        )
-        data.filter(keep_by_nms)
-
-        # Return to the original image frame
-        data["boxes"] = uncrop_boxes_xyxy(data["boxes"], crop_box)
-        data["points"] = uncrop_points(data["points"], crop_box)
-        data["crop_boxes"] = torch.tensor([crop_box for _ in range(len(data["rles"]))])
-
-        return data
-
-    def _process_batch(
-        self,
-        points: np.ndarray,
-        im_size: Tuple[int, ...],
-        crop_box: List[int],
-        orig_size: Tuple[int, ...],
-    ) -> MaskData:
-        orig_h, orig_w = orig_size
-
-        # Run model on this batch
-        transformed_points = self.predictor.transform.apply_coords(points, im_size)
-        in_points = torch.as_tensor(transformed_points, device=self.predictor.device)
-        in_labels = torch.ones(in_points.shape[0], dtype=torch.int, device=in_points.device)
-        masks, iou_preds, _ = self.predictor.predict_torch(
-            in_points[:, None, :],
-            in_labels[:, None],
-            multimask_output=True,
-            return_logits=True,
-        )
-
-        # Serialize predictions and store in MaskData
-        data = MaskData(
-            masks=masks.flatten(0, 1),
-            iou_preds=iou_preds.flatten(0, 1),
-            points=torch.as_tensor(points.repeat(masks.shape[1], axis=0)),
-        )
-        del masks
-
-        # Filter by predicted IoU
-        if self.pred_iou_thresh > 0.0:
-            keep_mask = data["iou_preds"] > self.pred_iou_thresh
-            data.filter(keep_mask)
-
-        # Calculate stability score
-        data["stability_score"] = calculate_stability_score(
-            data["masks"], self.predictor.model.mask_threshold, self.stability_score_offset
-        )
-        if self.stability_score_thresh > 0.0:
-            keep_mask = data["stability_score"] >= self.stability_score_thresh
-            data.filter(keep_mask)
-
-        # Threshold masks and calculate boxes
-        data["masks"] = data["masks"] > self.predictor.model.mask_threshold
-        data["boxes"] = batched_mask_to_box(data["masks"])
-
-        # Filter boxes that touch crop boundaries
-        keep_mask = ~is_box_near_crop_edge(data["boxes"], crop_box, [0, 0, orig_w, orig_h])
-        if not torch.all(keep_mask):
-            data.filter(keep_mask)
-
-        # Compress to RLE
-        data["masks"] = uncrop_masks(data["masks"], crop_box, orig_h, orig_w)
-        data["rles"] = mask_to_rle_pytorch(data["masks"])
-        del data["masks"]
-
-        return data
-
-    @staticmethod
-    def postprocess_small_regions(
-        mask_data: MaskData, min_area: int, nms_thresh: float
-    ) -> MaskData:
-        """
-        Removes small disconnected regions and holes in masks, then reruns
-        box NMS to remove any new duplicates.
-
-        Edits mask_data in place.
-
-        Requires open-cv as a dependency.
-        """
-        if len(mask_data["rles"]) == 0:
-            return mask_data
-
-        # Filter small disconnected regions and holes
-        new_masks = []
-        scores = []
-        for rle in mask_data["rles"]:
-            mask = rle_to_mask(rle)
-
-            mask, changed = remove_small_regions(mask, min_area, mode="holes")
-            unchanged = not changed
-            mask, changed = remove_small_regions(mask, min_area, mode="islands")
-            unchanged = unchanged and not changed
-
-            new_masks.append(torch.as_tensor(mask).unsqueeze(0))
-            # Give score=0 to changed masks and score=1 to unchanged masks
-            # so NMS will prefer ones that didn't need postprocessing
-            scores.append(float(unchanged))
-
-        # Recalculate boxes and remove any new duplicates
-        masks = torch.cat(new_masks, dim=0)
-        boxes = batched_mask_to_box(masks)
-        keep_by_nms = batched_nms(
-            boxes.float(),
-            torch.as_tensor(scores),
-            torch.zeros_like(boxes[:, 0]),  # categories
-            iou_threshold=nms_thresh,
-        )
-
-        # Only recalculate RLEs for masks that have changed
-        for i_mask in keep_by_nms:
-            if scores[i_mask] == 0.0:
-                mask_torch = masks[i_mask].unsqueeze(0)
-                mask_data["rles"][i_mask] = mask_to_rle_pytorch(mask_torch)[0]
-                mask_data["boxes"][i_mask] = boxes[i_mask]  # update res directly
-        mask_data.filter(keep_by_nms)
-
-        return mask_data
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
+import numpy as np
+import torch
+from torchvision.ops.boxes import batched_nms, box_area  # type: ignore
+
+from typing import Any, Dict, List, Optional, Tuple
+
+from .modeling import Sam
+from .predictor import SamPredictor
+from .utils.amg import (
+    MaskData,
+    area_from_rle,
+    batch_iterator,
+    batched_mask_to_box,
+    box_xyxy_to_xywh,
+    build_all_layer_point_grids,
+    calculate_stability_score,
+    coco_encode_rle,
+    generate_crop_boxes,
+    is_box_near_crop_edge,
+    mask_to_rle_pytorch,
+    remove_small_regions,
+    rle_to_mask,
+    uncrop_boxes_xyxy,
+    uncrop_masks,
+    uncrop_points,
+)
+
+
+class SamAutomaticMaskGenerator:
+    def __init__(
+        self,
+        model: Sam,
+        points_per_side: Optional[int] = 32,
+        points_per_batch: int = 64,
+        pred_iou_thresh: float = 0.88,
+        stability_score_thresh: float = 0.95,
+        stability_score_offset: float = 1.0,
+        box_nms_thresh: float = 0.7,
+        crop_n_layers: int = 0,
+        crop_nms_thresh: float = 0.7,
+        crop_overlap_ratio: float = 512 / 1500,
+        crop_n_points_downscale_factor: int = 1,
+        point_grids: Optional[List[np.ndarray]] = None,
+        min_mask_region_area: int = 0,
+        output_mode: str = "binary_mask",
+    ) -> None:
+        """
+        Using a SAM model, generates masks for the entire image.
+        Generates a grid of point prompts over the image, then filters
+        low quality and duplicate masks. The default settings are chosen
+        for SAM with a ViT-H backbone.
+
+        Arguments:
+          model (Sam): The SAM model to use for mask prediction.
+          points_per_side (int or None): The number of points to be sampled
+            along one side of the image. The total number of points is
+            points_per_side**2. If None, 'point_grids' must provide explicit
+            point sampling.
+          points_per_batch (int): Sets the number of points run simultaneously
+            by the model. Higher numbers may be faster but use more GPU memory.
+          pred_iou_thresh (float): A filtering threshold in [0,1], using the
+            model's predicted mask quality.
+          stability_score_thresh (float): A filtering threshold in [0,1], using
+            the stability of the mask under changes to the cutoff used to binarize
+            the model's mask predictions.
+          stability_score_offset (float): The amount to shift the cutoff when
+            calculated the stability score.
+          box_nms_thresh (float): The box IoU cutoff used by non-maximal
+            suppression to filter duplicate masks.
+          crop_n_layers (int): If >0, mask prediction will be run again on
+            crops of the image. Sets the number of layers to run, where each
+            layer has 2**i_layer number of image crops.
+          crop_nms_thresh (float): The box IoU cutoff used by non-maximal
+            suppression to filter duplicate masks between different crops.
+          crop_overlap_ratio (float): Sets the degree to which crops overlap.
+            In the first crop layer, crops will overlap by this fraction of
+            the image length. Later layers with more crops scale down this overlap.
+          crop_n_points_downscale_factor (int): The number of points-per-side
+            sampled in layer n is scaled down by crop_n_points_downscale_factor**n.
+          point_grids (list(np.ndarray) or None): A list over explicit grids
+            of points used for sampling, normalized to [0,1]. The nth grid in the
+            list is used in the nth crop layer. Exclusive with points_per_side.
+          min_mask_region_area (int): If >0, postprocessing will be applied
+            to remove disconnected regions and holes in masks with area smaller
+            than min_mask_region_area. Requires opencv.
+          output_mode (str): The form masks are returned in. Can be 'binary_mask',
+            'uncompressed_rle', or 'coco_rle'. 'coco_rle' requires pycocotools.
+            For large resolutions, 'binary_mask' may consume large amounts of
+            memory.
+        """
+
+        assert (points_per_side is None) != (
+            point_grids is None
+        ), "Exactly one of points_per_side or point_grid must be provided."
+        if points_per_side is not None:
+            self.point_grids = build_all_layer_point_grids(
+                points_per_side,
+                crop_n_layers,
+                crop_n_points_downscale_factor,
+            )
+        elif point_grids is not None:
+            self.point_grids = point_grids
+        else:
+            raise ValueError("Can't have both points_per_side and point_grid be None.")
+
+        assert output_mode in [
+            "binary_mask",
+            "uncompressed_rle",
+            "coco_rle",
+        ], f"Unknown output_mode {output_mode}."
+        if output_mode == "coco_rle":
+            from pycocotools import mask as mask_utils  # type: ignore # noqa: F401
+
+        if min_mask_region_area > 0:
+            import cv2  # type: ignore # noqa: F401
+
+        self.predictor = SamPredictor(model)
+        self.points_per_batch = points_per_batch
+        self.pred_iou_thresh = pred_iou_thresh
+        self.stability_score_thresh = stability_score_thresh
+        self.stability_score_offset = stability_score_offset
+        self.box_nms_thresh = box_nms_thresh
+        self.crop_n_layers = crop_n_layers
+        self.crop_nms_thresh = crop_nms_thresh
+        self.crop_overlap_ratio = crop_overlap_ratio
+        self.crop_n_points_downscale_factor = crop_n_points_downscale_factor
+        self.min_mask_region_area = min_mask_region_area
+        self.output_mode = output_mode
+
+    @torch.no_grad()
+    def generate(self, image: np.ndarray) -> List[Dict[str, Any]]:
+        """
+        Generates masks for the given image.
+
+        Arguments:
+          image (np.ndarray): The image to generate masks for, in HWC uint8 format.
+
+        Returns:
+           list(dict(str, any)): A list over records for masks. Each record is
+             a dict containing the following keys:
+               segmentation (dict(str, any) or np.ndarray): The mask. If
+                 output_mode='binary_mask', is an array of shape HW. Otherwise,
+                 is a dictionary containing the RLE.
+               bbox (list(float)): The box around the mask, in XYWH format.
+               area (int): The area in pixels of the mask.
+               predicted_iou (float): The model's own prediction of the mask's
+                 quality. This is filtered by the pred_iou_thresh parameter.
+               point_coords (list(list(float))): The point coordinates input
+                 to the model to generate this mask.
+               stability_score (float): A measure of the mask's quality. This
+                 is filtered on using the stability_score_thresh parameter.
+               crop_box (list(float)): The crop of the image used to generate
+                 the mask, given in XYWH format.
+        """
+
+        # Generate masks
+        mask_data = self._generate_masks(image)
+
+        # Filter small disconnected regions and holes in masks
+        if self.min_mask_region_area > 0:
+            mask_data = self.postprocess_small_regions(
+                mask_data,
+                self.min_mask_region_area,
+                max(self.box_nms_thresh, self.crop_nms_thresh),
+            )
+
+        # Encode masks
+        if self.output_mode == "coco_rle":
+            mask_data["segmentations"] = [coco_encode_rle(rle) for rle in mask_data["rles"]]
+        elif self.output_mode == "binary_mask":
+            mask_data["segmentations"] = [rle_to_mask(rle) for rle in mask_data["rles"]]
+        else:
+            mask_data["segmentations"] = mask_data["rles"]
+
+        # Write mask records
+        curr_anns = []
+        for idx in range(len(mask_data["segmentations"])):
+            ann = {
+                "segmentation": mask_data["segmentations"][idx],
+                "area": area_from_rle(mask_data["rles"][idx]),
+                "bbox": box_xyxy_to_xywh(mask_data["boxes"][idx]).tolist(),
+                "predicted_iou": mask_data["iou_preds"][idx].item(),
+                "point_coords": [mask_data["points"][idx].tolist()],
+                "stability_score": mask_data["stability_score"][idx].item(),
+                "crop_box": box_xyxy_to_xywh(mask_data["crop_boxes"][idx]).tolist(),
+            }
+            curr_anns.append(ann)
+
+        return curr_anns
+
+    def _generate_masks(self, image: np.ndarray) -> MaskData:
+        orig_size = image.shape[:2]
+        crop_boxes, layer_idxs = generate_crop_boxes(
+            orig_size, self.crop_n_layers, self.crop_overlap_ratio
+        )
+
+        # Iterate over image crops
+        data = MaskData()
+        for crop_box, layer_idx in zip(crop_boxes, layer_idxs):
+            crop_data = self._process_crop(image, crop_box, layer_idx, orig_size)
+            data.cat(crop_data)
+
+        # Remove duplicate masks between crops
+        if len(crop_boxes) > 1:
+            # Prefer masks from smaller crops
+            scores = 1 / box_area(data["crop_boxes"])
+            scores = scores.to(data["boxes"].device)
+            keep_by_nms = batched_nms(
+                data["boxes"].float(),
+                scores,
+                torch.zeros_like(data["boxes"][:, 0]),  # categories
+                iou_threshold=self.crop_nms_thresh,
+            )
+            data.filter(keep_by_nms)
+
+        data.to_numpy()
+        return data
+
+    def _process_crop(
+        self,
+        image: np.ndarray,
+        crop_box: List[int],
+        crop_layer_idx: int,
+        orig_size: Tuple[int, ...],
+    ) -> MaskData:
+        # Crop the image and calculate embeddings
+        x0, y0, x1, y1 = crop_box
+        cropped_im = image[y0:y1, x0:x1, :]
+        cropped_im_size = cropped_im.shape[:2]
+        self.predictor.set_image(cropped_im)
+
+        # Get points for this crop
+        points_scale = np.array(cropped_im_size)[None, ::-1]
+        points_for_image = self.point_grids[crop_layer_idx] * points_scale
+
+        # Generate masks for this crop in batches
+        data = MaskData()
+        for (points,) in batch_iterator(self.points_per_batch, points_for_image):
+            batch_data = self._process_batch(points, cropped_im_size, crop_box, orig_size)
+            data.cat(batch_data)
+            del batch_data
+        self.predictor.reset_image()
+
+        # Remove duplicates within this crop.
+        keep_by_nms = batched_nms(
+            data["boxes"].float(),
+            data["iou_preds"],
+            torch.zeros_like(data["boxes"][:, 0]),  # categories
+            iou_threshold=self.box_nms_thresh,
+        )
+        data.filter(keep_by_nms)
+
+        # Return to the original image frame
+        data["boxes"] = uncrop_boxes_xyxy(data["boxes"], crop_box)
+        data["points"] = uncrop_points(data["points"], crop_box)
+        data["crop_boxes"] = torch.tensor([crop_box for _ in range(len(data["rles"]))])
+
+        return data
+
+    def _process_batch(
+        self,
+        points: np.ndarray,
+        im_size: Tuple[int, ...],
+        crop_box: List[int],
+        orig_size: Tuple[int, ...],
+    ) -> MaskData:
+        orig_h, orig_w = orig_size
+
+        # Run model on this batch
+        transformed_points = self.predictor.transform.apply_coords(points, im_size)
+        in_points = torch.as_tensor(transformed_points, device=self.predictor.device)
+        in_labels = torch.ones(in_points.shape[0], dtype=torch.int, device=in_points.device)
+        masks, iou_preds, _ = self.predictor.predict_torch(
+            in_points[:, None, :],
+            in_labels[:, None],
+            multimask_output=True,
+            return_logits=True,
+        )
+
+        # Serialize predictions and store in MaskData
+        data = MaskData(
+            masks=masks.flatten(0, 1),
+            iou_preds=iou_preds.flatten(0, 1),
+            points=torch.as_tensor(points.repeat(masks.shape[1], axis=0)),
+        )
+        del masks
+
+        # Filter by predicted IoU
+        if self.pred_iou_thresh > 0.0:
+            keep_mask = data["iou_preds"] > self.pred_iou_thresh
+            data.filter(keep_mask)
+
+        # Calculate stability score
+        data["stability_score"] = calculate_stability_score(
+            data["masks"], self.predictor.model.mask_threshold, self.stability_score_offset
+        )
+        if self.stability_score_thresh > 0.0:
+            keep_mask = data["stability_score"] >= self.stability_score_thresh
+            data.filter(keep_mask)
+
+        # Threshold masks and calculate boxes
+        data["masks"] = data["masks"] > self.predictor.model.mask_threshold
+        data["boxes"] = batched_mask_to_box(data["masks"])
+
+        # Filter boxes that touch crop boundaries
+        keep_mask = ~is_box_near_crop_edge(data["boxes"], crop_box, [0, 0, orig_w, orig_h])
+        if not torch.all(keep_mask):
+            data.filter(keep_mask)
+
+        # Compress to RLE
+        data["masks"] = uncrop_masks(data["masks"], crop_box, orig_h, orig_w)
+        data["rles"] = mask_to_rle_pytorch(data["masks"])
+        del data["masks"]
+
+        return data
+
+    @staticmethod
+    def postprocess_small_regions(
+        mask_data: MaskData, min_area: int, nms_thresh: float
+    ) -> MaskData:
+        """
+        Removes small disconnected regions and holes in masks, then reruns
+        box NMS to remove any new duplicates.
+
+        Edits mask_data in place.
+
+        Requires open-cv as a dependency.
+        """
+        if len(mask_data["rles"]) == 0:
+            return mask_data
+
+        # Filter small disconnected regions and holes
+        new_masks = []
+        scores = []
+        for rle in mask_data["rles"]:
+            mask = rle_to_mask(rle)
+
+            mask, changed = remove_small_regions(mask, min_area, mode="holes")
+            unchanged = not changed
+            mask, changed = remove_small_regions(mask, min_area, mode="islands")
+            unchanged = unchanged and not changed
+
+            new_masks.append(torch.as_tensor(mask).unsqueeze(0))
+            # Give score=0 to changed masks and score=1 to unchanged masks
+            # so NMS will prefer ones that didn't need postprocessing
+            scores.append(float(unchanged))
+
+        # Recalculate boxes and remove any new duplicates
+        masks = torch.cat(new_masks, dim=0)
+        boxes = batched_mask_to_box(masks)
+        keep_by_nms = batched_nms(
+            boxes.float(),
+            torch.as_tensor(scores),
+            torch.zeros_like(boxes[:, 0]),  # categories
+            iou_threshold=nms_thresh,
+        )
+
+        # Only recalculate RLEs for masks that have changed
+        for i_mask in keep_by_nms:
+            if scores[i_mask] == 0.0:
+                mask_torch = masks[i_mask].unsqueeze(0)
+                mask_data["rles"][i_mask] = mask_to_rle_pytorch(mask_torch)[0]
+                mask_data["boxes"][i_mask] = boxes[i_mask]  # update res directly
+        mask_data.filter(keep_by_nms)
+
+        return mask_data
```

### Comparing `npsam-1.4.5/npsam/segment_anything/modeling/common.py` & `npsam-1.4.6/npsam/segment_anything/modeling/common.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-# All rights reserved.
-
-# This source code is licensed under the license found in the
-# LICENSE file in the root directory of this source tree.
-
-import torch
-import torch.nn as nn
-
-from typing import Type
-
-
-class MLPBlock(nn.Module):
-    def __init__(
-        self,
-        embedding_dim: int,
-        mlp_dim: int,
-        act: Type[nn.Module] = nn.GELU,
-    ) -> None:
-        super().__init__()
-        self.lin1 = nn.Linear(embedding_dim, mlp_dim)
-        self.lin2 = nn.Linear(mlp_dim, embedding_dim)
-        self.act = act()
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        return self.lin2(self.act(self.lin1(x)))
-
-
-# From https://github.com/facebookresearch/detectron2/blob/main/detectron2/layers/batch_norm.py # noqa
-# Itself from https://github.com/facebookresearch/ConvNeXt/blob/d1fa8f6fef0a165b27399986cc2bdacc92777e40/models/convnext.py#L119  # noqa
-class LayerNorm2d(nn.Module):
-    def __init__(self, num_channels: int, eps: float = 1e-6) -> None:
-        super().__init__()
-        self.weight = nn.Parameter(torch.ones(num_channels))
-        self.bias = nn.Parameter(torch.zeros(num_channels))
-        self.eps = eps
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        u = x.mean(1, keepdim=True)
-        s = (x - u).pow(2).mean(1, keepdim=True)
-        x = (x - u) / torch.sqrt(s + self.eps)
-        x = self.weight[:, None, None] * x + self.bias[:, None, None]
-        return x
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
+import torch
+import torch.nn as nn
+
+from typing import Type
+
+
+class MLPBlock(nn.Module):
+    def __init__(
+        self,
+        embedding_dim: int,
+        mlp_dim: int,
+        act: Type[nn.Module] = nn.GELU,
+    ) -> None:
+        super().__init__()
+        self.lin1 = nn.Linear(embedding_dim, mlp_dim)
+        self.lin2 = nn.Linear(mlp_dim, embedding_dim)
+        self.act = act()
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        return self.lin2(self.act(self.lin1(x)))
+
+
+# From https://github.com/facebookresearch/detectron2/blob/main/detectron2/layers/batch_norm.py # noqa
+# Itself from https://github.com/facebookresearch/ConvNeXt/blob/d1fa8f6fef0a165b27399986cc2bdacc92777e40/models/convnext.py#L119  # noqa
+class LayerNorm2d(nn.Module):
+    def __init__(self, num_channels: int, eps: float = 1e-6) -> None:
+        super().__init__()
+        self.weight = nn.Parameter(torch.ones(num_channels))
+        self.bias = nn.Parameter(torch.zeros(num_channels))
+        self.eps = eps
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        u = x.mean(1, keepdim=True)
+        s = (x - u).pow(2).mean(1, keepdim=True)
+        x = (x - u) / torch.sqrt(s + self.eps)
+        x = self.weight[:, None, None] * x + self.bias[:, None, None]
+        return x
```

### Comparing `npsam-1.4.5/npsam/segment_anything/modeling/image_encoder.py` & `npsam-1.4.6/npsam/segment_anything/modeling/image_encoder.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,395 +1,395 @@
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-# All rights reserved.
-
-# This source code is licensed under the license found in the
-# LICENSE file in the root directory of this source tree.
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from typing import Optional, Tuple, Type
-
-from .common import LayerNorm2d, MLPBlock
-
-
-# This class and its supporting functions below lightly adapted from the ViTDet backbone available at: https://github.com/facebookresearch/detectron2/blob/main/detectron2/modeling/backbone/vit.py # noqa
-class ImageEncoderViT(nn.Module):
-    def __init__(
-        self,
-        img_size: int = 1024,
-        patch_size: int = 16,
-        in_chans: int = 3,
-        embed_dim: int = 768,
-        depth: int = 12,
-        num_heads: int = 12,
-        mlp_ratio: float = 4.0,
-        out_chans: int = 256,
-        qkv_bias: bool = True,
-        norm_layer: Type[nn.Module] = nn.LayerNorm,
-        act_layer: Type[nn.Module] = nn.GELU,
-        use_abs_pos: bool = True,
-        use_rel_pos: bool = False,
-        rel_pos_zero_init: bool = True,
-        window_size: int = 0,
-        global_attn_indexes: Tuple[int, ...] = (),
-    ) -> None:
-        """
-        Args:
-            img_size (int): Input image size.
-            patch_size (int): Patch size.
-            in_chans (int): Number of input image channels.
-            embed_dim (int): Patch embedding dimension.
-            depth (int): Depth of ViT.
-            num_heads (int): Number of attention heads in each ViT block.
-            mlp_ratio (float): Ratio of mlp hidden dim to embedding dim.
-            qkv_bias (bool): If True, add a learnable bias to query, key, value.
-            norm_layer (nn.Module): Normalization layer.
-            act_layer (nn.Module): Activation layer.
-            use_abs_pos (bool): If True, use absolute positional embeddings.
-            use_rel_pos (bool): If True, add relative positional embeddings to the attention map.
-            rel_pos_zero_init (bool): If True, zero initialize relative positional parameters.
-            window_size (int): Window size for window attention blocks.
-            global_attn_indexes (list): Indexes for blocks using global attention.
-        """
-        super().__init__()
-        self.img_size = img_size
-
-        self.patch_embed = PatchEmbed(
-            kernel_size=(patch_size, patch_size),
-            stride=(patch_size, patch_size),
-            in_chans=in_chans,
-            embed_dim=embed_dim,
-        )
-
-        self.pos_embed: Optional[nn.Parameter] = None
-        if use_abs_pos:
-            # Initialize absolute positional embedding with pretrain image size.
-            self.pos_embed = nn.Parameter(
-                torch.zeros(1, img_size // patch_size, img_size // patch_size, embed_dim)
-            )
-
-        self.blocks = nn.ModuleList()
-        for i in range(depth):
-            block = Block(
-                dim=embed_dim,
-                num_heads=num_heads,
-                mlp_ratio=mlp_ratio,
-                qkv_bias=qkv_bias,
-                norm_layer=norm_layer,
-                act_layer=act_layer,
-                use_rel_pos=use_rel_pos,
-                rel_pos_zero_init=rel_pos_zero_init,
-                window_size=window_size if i not in global_attn_indexes else 0,
-                input_size=(img_size // patch_size, img_size // patch_size),
-            )
-            self.blocks.append(block)
-
-        self.neck = nn.Sequential(
-            nn.Conv2d(
-                embed_dim,
-                out_chans,
-                kernel_size=1,
-                bias=False,
-            ),
-            LayerNorm2d(out_chans),
-            nn.Conv2d(
-                out_chans,
-                out_chans,
-                kernel_size=3,
-                padding=1,
-                bias=False,
-            ),
-            LayerNorm2d(out_chans),
-        )
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        x = self.patch_embed(x)
-        if self.pos_embed is not None:
-            x = x + self.pos_embed
-
-        for blk in self.blocks:
-            x = blk(x)
-
-        x = self.neck(x.permute(0, 3, 1, 2))
-
-        return x
-
-
-class Block(nn.Module):
-    """Transformer blocks with support of window attention and residual propagation blocks"""
-
-    def __init__(
-        self,
-        dim: int,
-        num_heads: int,
-        mlp_ratio: float = 4.0,
-        qkv_bias: bool = True,
-        norm_layer: Type[nn.Module] = nn.LayerNorm,
-        act_layer: Type[nn.Module] = nn.GELU,
-        use_rel_pos: bool = False,
-        rel_pos_zero_init: bool = True,
-        window_size: int = 0,
-        input_size: Optional[Tuple[int, int]] = None,
-    ) -> None:
-        """
-        Args:
-            dim (int): Number of input channels.
-            num_heads (int): Number of attention heads in each ViT block.
-            mlp_ratio (float): Ratio of mlp hidden dim to embedding dim.
-            qkv_bias (bool): If True, add a learnable bias to query, key, value.
-            norm_layer (nn.Module): Normalization layer.
-            act_layer (nn.Module): Activation layer.
-            use_rel_pos (bool): If True, add relative positional embeddings to the attention map.
-            rel_pos_zero_init (bool): If True, zero initialize relative positional parameters.
-            window_size (int): Window size for window attention blocks. If it equals 0, then
-                use global attention.
-            input_size (tuple(int, int) or None): Input resolution for calculating the relative
-                positional parameter size.
-        """
-        super().__init__()
-        self.norm1 = norm_layer(dim)
-        self.attn = Attention(
-            dim,
-            num_heads=num_heads,
-            qkv_bias=qkv_bias,
-            use_rel_pos=use_rel_pos,
-            rel_pos_zero_init=rel_pos_zero_init,
-            input_size=input_size if window_size == 0 else (window_size, window_size),
-        )
-
-        self.norm2 = norm_layer(dim)
-        self.mlp = MLPBlock(embedding_dim=dim, mlp_dim=int(dim * mlp_ratio), act=act_layer)
-
-        self.window_size = window_size
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        shortcut = x
-        x = self.norm1(x)
-        # Window partition
-        if self.window_size > 0:
-            H, W = x.shape[1], x.shape[2]
-            x, pad_hw = window_partition(x, self.window_size)
-
-        x = self.attn(x)
-        # Reverse window partition
-        if self.window_size > 0:
-            x = window_unpartition(x, self.window_size, pad_hw, (H, W))
-
-        x = shortcut + x
-        x = x + self.mlp(self.norm2(x))
-
-        return x
-
-
-class Attention(nn.Module):
-    """Multi-head Attention block with relative position embeddings."""
-
-    def __init__(
-        self,
-        dim: int,
-        num_heads: int = 8,
-        qkv_bias: bool = True,
-        use_rel_pos: bool = False,
-        rel_pos_zero_init: bool = True,
-        input_size: Optional[Tuple[int, int]] = None,
-    ) -> None:
-        """
-        Args:
-            dim (int): Number of input channels.
-            num_heads (int): Number of attention heads.
-            qkv_bias (bool):  If True, add a learnable bias to query, key, value.
-            rel_pos (bool): If True, add relative positional embeddings to the attention map.
-            rel_pos_zero_init (bool): If True, zero initialize relative positional parameters.
-            input_size (tuple(int, int) or None): Input resolution for calculating the relative
-                positional parameter size.
-        """
-        super().__init__()
-        self.num_heads = num_heads
-        head_dim = dim // num_heads
-        self.scale = head_dim**-0.5
-
-        self.qkv = nn.Linear(dim, dim * 3, bias=qkv_bias)
-        self.proj = nn.Linear(dim, dim)
-
-        self.use_rel_pos = use_rel_pos
-        if self.use_rel_pos:
-            assert (
-                input_size is not None
-            ), "Input size must be provided if using relative positional encoding."
-            # initialize relative positional embeddings
-            self.rel_pos_h = nn.Parameter(torch.zeros(2 * input_size[0] - 1, head_dim))
-            self.rel_pos_w = nn.Parameter(torch.zeros(2 * input_size[1] - 1, head_dim))
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        B, H, W, _ = x.shape
-        # qkv with shape (3, B, nHead, H * W, C)
-        qkv = self.qkv(x).reshape(B, H * W, 3, self.num_heads, -1).permute(2, 0, 3, 1, 4)
-        # q, k, v with shape (B * nHead, H * W, C)
-        q, k, v = qkv.reshape(3, B * self.num_heads, H * W, -1).unbind(0)
-
-        attn = (q * self.scale) @ k.transpose(-2, -1)
-
-        if self.use_rel_pos:
-            attn = add_decomposed_rel_pos(attn, q, self.rel_pos_h, self.rel_pos_w, (H, W), (H, W))
-
-        attn = attn.softmax(dim=-1)
-        x = (attn @ v).view(B, self.num_heads, H, W, -1).permute(0, 2, 3, 1, 4).reshape(B, H, W, -1)
-        x = self.proj(x)
-
-        return x
-
-
-def window_partition(x: torch.Tensor, window_size: int) -> Tuple[torch.Tensor, Tuple[int, int]]:
-    """
-    Partition into non-overlapping windows with padding if needed.
-    Args:
-        x (tensor): input tokens with [B, H, W, C].
-        window_size (int): window size.
-
-    Returns:
-        windows: windows after partition with [B * num_windows, window_size, window_size, C].
-        (Hp, Wp): padded height and width before partition
-    """
-    B, H, W, C = x.shape
-
-    pad_h = (window_size - H % window_size) % window_size
-    pad_w = (window_size - W % window_size) % window_size
-    if pad_h > 0 or pad_w > 0:
-        x = F.pad(x, (0, 0, 0, pad_w, 0, pad_h))
-    Hp, Wp = H + pad_h, W + pad_w
-
-    x = x.view(B, Hp // window_size, window_size, Wp // window_size, window_size, C)
-    windows = x.permute(0, 1, 3, 2, 4, 5).contiguous().view(-1, window_size, window_size, C)
-    return windows, (Hp, Wp)
-
-
-def window_unpartition(
-    windows: torch.Tensor, window_size: int, pad_hw: Tuple[int, int], hw: Tuple[int, int]
-) -> torch.Tensor:
-    """
-    Window unpartition into original sequences and removing padding.
-    Args:
-        windows (tensor): input tokens with [B * num_windows, window_size, window_size, C].
-        window_size (int): window size.
-        pad_hw (Tuple): padded height and width (Hp, Wp).
-        hw (Tuple): original height and width (H, W) before padding.
-
-    Returns:
-        x: unpartitioned sequences with [B, H, W, C].
-    """
-    Hp, Wp = pad_hw
-    H, W = hw
-    B = windows.shape[0] // (Hp * Wp // window_size // window_size)
-    x = windows.view(B, Hp // window_size, Wp // window_size, window_size, window_size, -1)
-    x = x.permute(0, 1, 3, 2, 4, 5).contiguous().view(B, Hp, Wp, -1)
-
-    if Hp > H or Wp > W:
-        x = x[:, :H, :W, :].contiguous()
-    return x
-
-
-def get_rel_pos(q_size: int, k_size: int, rel_pos: torch.Tensor) -> torch.Tensor:
-    """
-    Get relative positional embeddings according to the relative positions of
-        query and key sizes.
-    Args:
-        q_size (int): size of query q.
-        k_size (int): size of key k.
-        rel_pos (Tensor): relative position embeddings (L, C).
-
-    Returns:
-        Extracted positional embeddings according to relative positions.
-    """
-    max_rel_dist = int(2 * max(q_size, k_size) - 1)
-    # Interpolate rel pos if needed.
-    if rel_pos.shape[0] != max_rel_dist:
-        # Interpolate rel pos.
-        rel_pos_resized = F.interpolate(
-            rel_pos.reshape(1, rel_pos.shape[0], -1).permute(0, 2, 1),
-            size=max_rel_dist,
-            mode="linear",
-        )
-        rel_pos_resized = rel_pos_resized.reshape(-1, max_rel_dist).permute(1, 0)
-    else:
-        rel_pos_resized = rel_pos
-
-    # Scale the coords with short length if shapes for q and k are different.
-    q_coords = torch.arange(q_size)[:, None] * max(k_size / q_size, 1.0)
-    k_coords = torch.arange(k_size)[None, :] * max(q_size / k_size, 1.0)
-    relative_coords = (q_coords - k_coords) + (k_size - 1) * max(q_size / k_size, 1.0)
-
-    return rel_pos_resized[relative_coords.long()]
-
-
-def add_decomposed_rel_pos(
-    attn: torch.Tensor,
-    q: torch.Tensor,
-    rel_pos_h: torch.Tensor,
-    rel_pos_w: torch.Tensor,
-    q_size: Tuple[int, int],
-    k_size: Tuple[int, int],
-) -> torch.Tensor:
-    """
-    Calculate decomposed Relative Positional Embeddings from :paper:`mvitv2`.
-    https://github.com/facebookresearch/mvit/blob/19786631e330df9f3622e5402b4a419a263a2c80/mvit/models/attention.py   # noqa B950
-    Args:
-        attn (Tensor): attention map.
-        q (Tensor): query q in the attention layer with shape (B, q_h * q_w, C).
-        rel_pos_h (Tensor): relative position embeddings (Lh, C) for height axis.
-        rel_pos_w (Tensor): relative position embeddings (Lw, C) for width axis.
-        q_size (Tuple): spatial sequence size of query q with (q_h, q_w).
-        k_size (Tuple): spatial sequence size of key k with (k_h, k_w).
-
-    Returns:
-        attn (Tensor): attention map with added relative positional embeddings.
-    """
-    q_h, q_w = q_size
-    k_h, k_w = k_size
-    Rh = get_rel_pos(q_h, k_h, rel_pos_h)
-    Rw = get_rel_pos(q_w, k_w, rel_pos_w)
-
-    B, _, dim = q.shape
-    r_q = q.reshape(B, q_h, q_w, dim)
-    rel_h = torch.einsum("bhwc,hkc->bhwk", r_q, Rh)
-    rel_w = torch.einsum("bhwc,wkc->bhwk", r_q, Rw)
-
-    attn = (
-        attn.view(B, q_h, q_w, k_h, k_w) + rel_h[:, :, :, :, None] + rel_w[:, :, :, None, :]
-    ).view(B, q_h * q_w, k_h * k_w)
-
-    return attn
-
-
-class PatchEmbed(nn.Module):
-    """
-    Image to Patch Embedding.
-    """
-
-    def __init__(
-        self,
-        kernel_size: Tuple[int, int] = (16, 16),
-        stride: Tuple[int, int] = (16, 16),
-        padding: Tuple[int, int] = (0, 0),
-        in_chans: int = 3,
-        embed_dim: int = 768,
-    ) -> None:
-        """
-        Args:
-            kernel_size (Tuple): kernel size of the projection layer.
-            stride (Tuple): stride of the projection layer.
-            padding (Tuple): padding size of the projection layer.
-            in_chans (int): Number of input image channels.
-            embed_dim (int): Patch embedding dimension.
-        """
-        super().__init__()
-
-        self.proj = nn.Conv2d(
-            in_chans, embed_dim, kernel_size=kernel_size, stride=stride, padding=padding
-        )
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        x = self.proj(x)
-        # B C H W -> B H W C
-        x = x.permute(0, 2, 3, 1)
-        return x
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from typing import Optional, Tuple, Type
+
+from .common import LayerNorm2d, MLPBlock
+
+
+# This class and its supporting functions below lightly adapted from the ViTDet backbone available at: https://github.com/facebookresearch/detectron2/blob/main/detectron2/modeling/backbone/vit.py # noqa
+class ImageEncoderViT(nn.Module):
+    def __init__(
+        self,
+        img_size: int = 1024,
+        patch_size: int = 16,
+        in_chans: int = 3,
+        embed_dim: int = 768,
+        depth: int = 12,
+        num_heads: int = 12,
+        mlp_ratio: float = 4.0,
+        out_chans: int = 256,
+        qkv_bias: bool = True,
+        norm_layer: Type[nn.Module] = nn.LayerNorm,
+        act_layer: Type[nn.Module] = nn.GELU,
+        use_abs_pos: bool = True,
+        use_rel_pos: bool = False,
+        rel_pos_zero_init: bool = True,
+        window_size: int = 0,
+        global_attn_indexes: Tuple[int, ...] = (),
+    ) -> None:
+        """
+        Args:
+            img_size (int): Input image size.
+            patch_size (int): Patch size.
+            in_chans (int): Number of input image channels.
+            embed_dim (int): Patch embedding dimension.
+            depth (int): Depth of ViT.
+            num_heads (int): Number of attention heads in each ViT block.
+            mlp_ratio (float): Ratio of mlp hidden dim to embedding dim.
+            qkv_bias (bool): If True, add a learnable bias to query, key, value.
+            norm_layer (nn.Module): Normalization layer.
+            act_layer (nn.Module): Activation layer.
+            use_abs_pos (bool): If True, use absolute positional embeddings.
+            use_rel_pos (bool): If True, add relative positional embeddings to the attention map.
+            rel_pos_zero_init (bool): If True, zero initialize relative positional parameters.
+            window_size (int): Window size for window attention blocks.
+            global_attn_indexes (list): Indexes for blocks using global attention.
+        """
+        super().__init__()
+        self.img_size = img_size
+
+        self.patch_embed = PatchEmbed(
+            kernel_size=(patch_size, patch_size),
+            stride=(patch_size, patch_size),
+            in_chans=in_chans,
+            embed_dim=embed_dim,
+        )
+
+        self.pos_embed: Optional[nn.Parameter] = None
+        if use_abs_pos:
+            # Initialize absolute positional embedding with pretrain image size.
+            self.pos_embed = nn.Parameter(
+                torch.zeros(1, img_size // patch_size, img_size // patch_size, embed_dim)
+            )
+
+        self.blocks = nn.ModuleList()
+        for i in range(depth):
+            block = Block(
+                dim=embed_dim,
+                num_heads=num_heads,
+                mlp_ratio=mlp_ratio,
+                qkv_bias=qkv_bias,
+                norm_layer=norm_layer,
+                act_layer=act_layer,
+                use_rel_pos=use_rel_pos,
+                rel_pos_zero_init=rel_pos_zero_init,
+                window_size=window_size if i not in global_attn_indexes else 0,
+                input_size=(img_size // patch_size, img_size // patch_size),
+            )
+            self.blocks.append(block)
+
+        self.neck = nn.Sequential(
+            nn.Conv2d(
+                embed_dim,
+                out_chans,
+                kernel_size=1,
+                bias=False,
+            ),
+            LayerNorm2d(out_chans),
+            nn.Conv2d(
+                out_chans,
+                out_chans,
+                kernel_size=3,
+                padding=1,
+                bias=False,
+            ),
+            LayerNorm2d(out_chans),
+        )
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        x = self.patch_embed(x)
+        if self.pos_embed is not None:
+            x = x + self.pos_embed
+
+        for blk in self.blocks:
+            x = blk(x)
+
+        x = self.neck(x.permute(0, 3, 1, 2))
+
+        return x
+
+
+class Block(nn.Module):
+    """Transformer blocks with support of window attention and residual propagation blocks"""
+
+    def __init__(
+        self,
+        dim: int,
+        num_heads: int,
+        mlp_ratio: float = 4.0,
+        qkv_bias: bool = True,
+        norm_layer: Type[nn.Module] = nn.LayerNorm,
+        act_layer: Type[nn.Module] = nn.GELU,
+        use_rel_pos: bool = False,
+        rel_pos_zero_init: bool = True,
+        window_size: int = 0,
+        input_size: Optional[Tuple[int, int]] = None,
+    ) -> None:
+        """
+        Args:
+            dim (int): Number of input channels.
+            num_heads (int): Number of attention heads in each ViT block.
+            mlp_ratio (float): Ratio of mlp hidden dim to embedding dim.
+            qkv_bias (bool): If True, add a learnable bias to query, key, value.
+            norm_layer (nn.Module): Normalization layer.
+            act_layer (nn.Module): Activation layer.
+            use_rel_pos (bool): If True, add relative positional embeddings to the attention map.
+            rel_pos_zero_init (bool): If True, zero initialize relative positional parameters.
+            window_size (int): Window size for window attention blocks. If it equals 0, then
+                use global attention.
+            input_size (tuple(int, int) or None): Input resolution for calculating the relative
+                positional parameter size.
+        """
+        super().__init__()
+        self.norm1 = norm_layer(dim)
+        self.attn = Attention(
+            dim,
+            num_heads=num_heads,
+            qkv_bias=qkv_bias,
+            use_rel_pos=use_rel_pos,
+            rel_pos_zero_init=rel_pos_zero_init,
+            input_size=input_size if window_size == 0 else (window_size, window_size),
+        )
+
+        self.norm2 = norm_layer(dim)
+        self.mlp = MLPBlock(embedding_dim=dim, mlp_dim=int(dim * mlp_ratio), act=act_layer)
+
+        self.window_size = window_size
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        shortcut = x
+        x = self.norm1(x)
+        # Window partition
+        if self.window_size > 0:
+            H, W = x.shape[1], x.shape[2]
+            x, pad_hw = window_partition(x, self.window_size)
+
+        x = self.attn(x)
+        # Reverse window partition
+        if self.window_size > 0:
+            x = window_unpartition(x, self.window_size, pad_hw, (H, W))
+
+        x = shortcut + x
+        x = x + self.mlp(self.norm2(x))
+
+        return x
+
+
+class Attention(nn.Module):
+    """Multi-head Attention block with relative position embeddings."""
+
+    def __init__(
+        self,
+        dim: int,
+        num_heads: int = 8,
+        qkv_bias: bool = True,
+        use_rel_pos: bool = False,
+        rel_pos_zero_init: bool = True,
+        input_size: Optional[Tuple[int, int]] = None,
+    ) -> None:
+        """
+        Args:
+            dim (int): Number of input channels.
+            num_heads (int): Number of attention heads.
+            qkv_bias (bool):  If True, add a learnable bias to query, key, value.
+            rel_pos (bool): If True, add relative positional embeddings to the attention map.
+            rel_pos_zero_init (bool): If True, zero initialize relative positional parameters.
+            input_size (tuple(int, int) or None): Input resolution for calculating the relative
+                positional parameter size.
+        """
+        super().__init__()
+        self.num_heads = num_heads
+        head_dim = dim // num_heads
+        self.scale = head_dim**-0.5
+
+        self.qkv = nn.Linear(dim, dim * 3, bias=qkv_bias)
+        self.proj = nn.Linear(dim, dim)
+
+        self.use_rel_pos = use_rel_pos
+        if self.use_rel_pos:
+            assert (
+                input_size is not None
+            ), "Input size must be provided if using relative positional encoding."
+            # initialize relative positional embeddings
+            self.rel_pos_h = nn.Parameter(torch.zeros(2 * input_size[0] - 1, head_dim))
+            self.rel_pos_w = nn.Parameter(torch.zeros(2 * input_size[1] - 1, head_dim))
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        B, H, W, _ = x.shape
+        # qkv with shape (3, B, nHead, H * W, C)
+        qkv = self.qkv(x).reshape(B, H * W, 3, self.num_heads, -1).permute(2, 0, 3, 1, 4)
+        # q, k, v with shape (B * nHead, H * W, C)
+        q, k, v = qkv.reshape(3, B * self.num_heads, H * W, -1).unbind(0)
+
+        attn = (q * self.scale) @ k.transpose(-2, -1)
+
+        if self.use_rel_pos:
+            attn = add_decomposed_rel_pos(attn, q, self.rel_pos_h, self.rel_pos_w, (H, W), (H, W))
+
+        attn = attn.softmax(dim=-1)
+        x = (attn @ v).view(B, self.num_heads, H, W, -1).permute(0, 2, 3, 1, 4).reshape(B, H, W, -1)
+        x = self.proj(x)
+
+        return x
+
+
+def window_partition(x: torch.Tensor, window_size: int) -> Tuple[torch.Tensor, Tuple[int, int]]:
+    """
+    Partition into non-overlapping windows with padding if needed.
+    Args:
+        x (tensor): input tokens with [B, H, W, C].
+        window_size (int): window size.
+
+    Returns:
+        windows: windows after partition with [B * num_windows, window_size, window_size, C].
+        (Hp, Wp): padded height and width before partition
+    """
+    B, H, W, C = x.shape
+
+    pad_h = (window_size - H % window_size) % window_size
+    pad_w = (window_size - W % window_size) % window_size
+    if pad_h > 0 or pad_w > 0:
+        x = F.pad(x, (0, 0, 0, pad_w, 0, pad_h))
+    Hp, Wp = H + pad_h, W + pad_w
+
+    x = x.view(B, Hp // window_size, window_size, Wp // window_size, window_size, C)
+    windows = x.permute(0, 1, 3, 2, 4, 5).contiguous().view(-1, window_size, window_size, C)
+    return windows, (Hp, Wp)
+
+
+def window_unpartition(
+    windows: torch.Tensor, window_size: int, pad_hw: Tuple[int, int], hw: Tuple[int, int]
+) -> torch.Tensor:
+    """
+    Window unpartition into original sequences and removing padding.
+    Args:
+        windows (tensor): input tokens with [B * num_windows, window_size, window_size, C].
+        window_size (int): window size.
+        pad_hw (Tuple): padded height and width (Hp, Wp).
+        hw (Tuple): original height and width (H, W) before padding.
+
+    Returns:
+        x: unpartitioned sequences with [B, H, W, C].
+    """
+    Hp, Wp = pad_hw
+    H, W = hw
+    B = windows.shape[0] // (Hp * Wp // window_size // window_size)
+    x = windows.view(B, Hp // window_size, Wp // window_size, window_size, window_size, -1)
+    x = x.permute(0, 1, 3, 2, 4, 5).contiguous().view(B, Hp, Wp, -1)
+
+    if Hp > H or Wp > W:
+        x = x[:, :H, :W, :].contiguous()
+    return x
+
+
+def get_rel_pos(q_size: int, k_size: int, rel_pos: torch.Tensor) -> torch.Tensor:
+    """
+    Get relative positional embeddings according to the relative positions of
+        query and key sizes.
+    Args:
+        q_size (int): size of query q.
+        k_size (int): size of key k.
+        rel_pos (Tensor): relative position embeddings (L, C).
+
+    Returns:
+        Extracted positional embeddings according to relative positions.
+    """
+    max_rel_dist = int(2 * max(q_size, k_size) - 1)
+    # Interpolate rel pos if needed.
+    if rel_pos.shape[0] != max_rel_dist:
+        # Interpolate rel pos.
+        rel_pos_resized = F.interpolate(
+            rel_pos.reshape(1, rel_pos.shape[0], -1).permute(0, 2, 1),
+            size=max_rel_dist,
+            mode="linear",
+        )
+        rel_pos_resized = rel_pos_resized.reshape(-1, max_rel_dist).permute(1, 0)
+    else:
+        rel_pos_resized = rel_pos
+
+    # Scale the coords with short length if shapes for q and k are different.
+    q_coords = torch.arange(q_size)[:, None] * max(k_size / q_size, 1.0)
+    k_coords = torch.arange(k_size)[None, :] * max(q_size / k_size, 1.0)
+    relative_coords = (q_coords - k_coords) + (k_size - 1) * max(q_size / k_size, 1.0)
+
+    return rel_pos_resized[relative_coords.long()]
+
+
+def add_decomposed_rel_pos(
+    attn: torch.Tensor,
+    q: torch.Tensor,
+    rel_pos_h: torch.Tensor,
+    rel_pos_w: torch.Tensor,
+    q_size: Tuple[int, int],
+    k_size: Tuple[int, int],
+) -> torch.Tensor:
+    """
+    Calculate decomposed Relative Positional Embeddings from :paper:`mvitv2`.
+    https://github.com/facebookresearch/mvit/blob/19786631e330df9f3622e5402b4a419a263a2c80/mvit/models/attention.py   # noqa B950
+    Args:
+        attn (Tensor): attention map.
+        q (Tensor): query q in the attention layer with shape (B, q_h * q_w, C).
+        rel_pos_h (Tensor): relative position embeddings (Lh, C) for height axis.
+        rel_pos_w (Tensor): relative position embeddings (Lw, C) for width axis.
+        q_size (Tuple): spatial sequence size of query q with (q_h, q_w).
+        k_size (Tuple): spatial sequence size of key k with (k_h, k_w).
+
+    Returns:
+        attn (Tensor): attention map with added relative positional embeddings.
+    """
+    q_h, q_w = q_size
+    k_h, k_w = k_size
+    Rh = get_rel_pos(q_h, k_h, rel_pos_h)
+    Rw = get_rel_pos(q_w, k_w, rel_pos_w)
+
+    B, _, dim = q.shape
+    r_q = q.reshape(B, q_h, q_w, dim)
+    rel_h = torch.einsum("bhwc,hkc->bhwk", r_q, Rh)
+    rel_w = torch.einsum("bhwc,wkc->bhwk", r_q, Rw)
+
+    attn = (
+        attn.view(B, q_h, q_w, k_h, k_w) + rel_h[:, :, :, :, None] + rel_w[:, :, :, None, :]
+    ).view(B, q_h * q_w, k_h * k_w)
+
+    return attn
+
+
+class PatchEmbed(nn.Module):
+    """
+    Image to Patch Embedding.
+    """
+
+    def __init__(
+        self,
+        kernel_size: Tuple[int, int] = (16, 16),
+        stride: Tuple[int, int] = (16, 16),
+        padding: Tuple[int, int] = (0, 0),
+        in_chans: int = 3,
+        embed_dim: int = 768,
+    ) -> None:
+        """
+        Args:
+            kernel_size (Tuple): kernel size of the projection layer.
+            stride (Tuple): stride of the projection layer.
+            padding (Tuple): padding size of the projection layer.
+            in_chans (int): Number of input image channels.
+            embed_dim (int): Patch embedding dimension.
+        """
+        super().__init__()
+
+        self.proj = nn.Conv2d(
+            in_chans, embed_dim, kernel_size=kernel_size, stride=stride, padding=padding
+        )
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        x = self.proj(x)
+        # B C H W -> B H W C
+        x = x.permute(0, 2, 3, 1)
+        return x
```

### Comparing `npsam-1.4.5/npsam/segment_anything/modeling/prompt_encoder.py` & `npsam-1.4.6/npsam/segment_anything/modeling/prompt_encoder.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-# All rights reserved.
-
-# This source code is licensed under the license found in the
-# LICENSE file in the root directory of this source tree.
-
-import numpy as np
-import torch
-from torch import nn
-
-from typing import Any, Optional, Tuple, Type
-
-from .common import LayerNorm2d
-
-
-class PromptEncoder(nn.Module):
-    def __init__(
-        self,
-        embed_dim: int,
-        image_embedding_size: Tuple[int, int],
-        input_image_size: Tuple[int, int],
-        mask_in_chans: int,
-        activation: Type[nn.Module] = nn.GELU,
-    ) -> None:
-        """
-        Encodes prompts for input to SAM's mask decoder.
-
-        Arguments:
-          embed_dim (int): The prompts' embedding dimension
-          image_embedding_size (tuple(int, int)): The spatial size of the
-            image embedding, as (H, W).
-          input_image_size (int): The padded size of the image as input
-            to the image encoder, as (H, W).
-          mask_in_chans (int): The number of hidden channels used for
-            encoding input masks.
-          activation (nn.Module): The activation to use when encoding
-            input masks.
-        """
-        super().__init__()
-        self.embed_dim = embed_dim
-        self.input_image_size = input_image_size
-        self.image_embedding_size = image_embedding_size
-        self.pe_layer = PositionEmbeddingRandom(embed_dim // 2)
-
-        self.num_point_embeddings: int = 4  # pos/neg point + 2 box corners
-        point_embeddings = [nn.Embedding(1, embed_dim) for i in range(self.num_point_embeddings)]
-        self.point_embeddings = nn.ModuleList(point_embeddings)
-        self.not_a_point_embed = nn.Embedding(1, embed_dim)
-
-        self.mask_input_size = (4 * image_embedding_size[0], 4 * image_embedding_size[1])
-        self.mask_downscaling = nn.Sequential(
-            nn.Conv2d(1, mask_in_chans // 4, kernel_size=2, stride=2),
-            LayerNorm2d(mask_in_chans // 4),
-            activation(),
-            nn.Conv2d(mask_in_chans // 4, mask_in_chans, kernel_size=2, stride=2),
-            LayerNorm2d(mask_in_chans),
-            activation(),
-            nn.Conv2d(mask_in_chans, embed_dim, kernel_size=1),
-        )
-        self.no_mask_embed = nn.Embedding(1, embed_dim)
-
-    def get_dense_pe(self) -> torch.Tensor:
-        """
-        Returns the positional encoding used to encode point prompts,
-        applied to a dense set of points the shape of the image encoding.
-
-        Returns:
-          torch.Tensor: Positional encoding with shape
-            1x(embed_dim)x(embedding_h)x(embedding_w)
-        """
-        return self.pe_layer(self.image_embedding_size).unsqueeze(0)
-
-    def _embed_points(
-        self,
-        points: torch.Tensor,
-        labels: torch.Tensor,
-        pad: bool,
-    ) -> torch.Tensor:
-        """Embeds point prompts."""
-        points = points + 0.5  # Shift to center of pixel
-        if pad:
-            padding_point = torch.zeros((points.shape[0], 1, 2), device=points.device)
-            padding_label = -torch.ones((labels.shape[0], 1), device=labels.device)
-            points = torch.cat([points, padding_point], dim=1)
-            labels = torch.cat([labels, padding_label], dim=1)
-        point_embedding = self.pe_layer.forward_with_coords(points, self.input_image_size)
-        point_embedding[labels == -1] = 0.0
-        point_embedding[labels == -1] += self.not_a_point_embed.weight
-        point_embedding[labels == 0] += self.point_embeddings[0].weight
-        point_embedding[labels == 1] += self.point_embeddings[1].weight
-        return point_embedding
-
-    def _embed_boxes(self, boxes: torch.Tensor) -> torch.Tensor:
-        """Embeds box prompts."""
-        boxes = boxes + 0.5  # Shift to center of pixel
-        coords = boxes.reshape(-1, 2, 2)
-        corner_embedding = self.pe_layer.forward_with_coords(coords, self.input_image_size)
-        corner_embedding[:, 0, :] += self.point_embeddings[2].weight
-        corner_embedding[:, 1, :] += self.point_embeddings[3].weight
-        return corner_embedding
-
-    def _embed_masks(self, masks: torch.Tensor) -> torch.Tensor:
-        """Embeds mask inputs."""
-        mask_embedding = self.mask_downscaling(masks)
-        return mask_embedding
-
-    def _get_batch_size(
-        self,
-        points: Optional[Tuple[torch.Tensor, torch.Tensor]],
-        boxes: Optional[torch.Tensor],
-        masks: Optional[torch.Tensor],
-    ) -> int:
-        """
-        Gets the batch size of the output given the batch size of the input prompts.
-        """
-        if points is not None:
-            return points[0].shape[0]
-        elif boxes is not None:
-            return boxes.shape[0]
-        elif masks is not None:
-            return masks.shape[0]
-        else:
-            return 1
-
-    def _get_device(self) -> torch.device:
-        return self.point_embeddings[0].weight.device
-
-    def forward(
-        self,
-        points: Optional[Tuple[torch.Tensor, torch.Tensor]],
-        boxes: Optional[torch.Tensor],
-        masks: Optional[torch.Tensor],
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
-        """
-        Embeds different types of prompts, returning both sparse and dense
-        embeddings.
-
-        Arguments:
-          points (tuple(torch.Tensor, torch.Tensor) or none): point coordinates
-            and labels to embed.
-          boxes (torch.Tensor or none): boxes to embed
-          masks (torch.Tensor or none): masks to embed
-
-        Returns:
-          torch.Tensor: sparse embeddings for the points and boxes, with shape
-            BxNx(embed_dim), where N is determined by the number of input points
-            and boxes.
-          torch.Tensor: dense embeddings for the masks, in the shape
-            Bx(embed_dim)x(embed_H)x(embed_W)
-        """
-        bs = self._get_batch_size(points, boxes, masks)
-        sparse_embeddings = torch.empty((bs, 0, self.embed_dim), device=self._get_device())
-        if points is not None:
-            coords, labels = points
-            point_embeddings = self._embed_points(coords, labels, pad=(boxes is None))
-            sparse_embeddings = torch.cat([sparse_embeddings, point_embeddings], dim=1)
-        if boxes is not None:
-            box_embeddings = self._embed_boxes(boxes)
-            sparse_embeddings = torch.cat([sparse_embeddings, box_embeddings], dim=1)
-
-        if masks is not None:
-            dense_embeddings = self._embed_masks(masks)
-        else:
-            dense_embeddings = self.no_mask_embed.weight.reshape(1, -1, 1, 1).expand(
-                bs, -1, self.image_embedding_size[0], self.image_embedding_size[1]
-            )
-
-        return sparse_embeddings, dense_embeddings
-
-
-class PositionEmbeddingRandom(nn.Module):
-    """
-    Positional encoding using random spatial frequencies.
-    """
-
-    def __init__(self, num_pos_feats: int = 64, scale: Optional[float] = None) -> None:
-        super().__init__()
-        if scale is None or scale <= 0.0:
-            scale = 1.0
-        self.register_buffer(
-            "positional_encoding_gaussian_matrix",
-            scale * torch.randn((2, num_pos_feats)),
-        )
-
-    def _pe_encoding(self, coords: torch.Tensor) -> torch.Tensor:
-        """Positionally encode points that are normalized to [0,1]."""
-        # assuming coords are in [0, 1]^2 square and have d_1 x ... x d_n x 2 shape
-        coords = 2 * coords - 1
-        coords = coords @ self.positional_encoding_gaussian_matrix
-        coords = 2 * np.pi * coords
-        # outputs d_1 x ... x d_n x C shape
-        return torch.cat([torch.sin(coords), torch.cos(coords)], dim=-1)
-
-    def forward(self, size: Tuple[int, int]) -> torch.Tensor:
-        """Generate positional encoding for a grid of the specified size."""
-        h, w = size
-        device: Any = self.positional_encoding_gaussian_matrix.device
-        grid = torch.ones((h, w), device=device, dtype=torch.float32)
-        y_embed = grid.cumsum(dim=0) - 0.5
-        x_embed = grid.cumsum(dim=1) - 0.5
-        y_embed = y_embed / h
-        x_embed = x_embed / w
-
-        pe = self._pe_encoding(torch.stack([x_embed, y_embed], dim=-1))
-        return pe.permute(2, 0, 1)  # C x H x W
-
-    def forward_with_coords(
-        self, coords_input: torch.Tensor, image_size: Tuple[int, int]
-    ) -> torch.Tensor:
-        """Positionally encode points that are not normalized to [0,1]."""
-        coords = coords_input.clone()
-        coords[:, :, 0] = coords[:, :, 0] / image_size[1]
-        coords[:, :, 1] = coords[:, :, 1] / image_size[0]
-        return self._pe_encoding(coords.to(torch.float))  # B x N x C
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
+import numpy as np
+import torch
+from torch import nn
+
+from typing import Any, Optional, Tuple, Type
+
+from .common import LayerNorm2d
+
+
+class PromptEncoder(nn.Module):
+    def __init__(
+        self,
+        embed_dim: int,
+        image_embedding_size: Tuple[int, int],
+        input_image_size: Tuple[int, int],
+        mask_in_chans: int,
+        activation: Type[nn.Module] = nn.GELU,
+    ) -> None:
+        """
+        Encodes prompts for input to SAM's mask decoder.
+
+        Arguments:
+          embed_dim (int): The prompts' embedding dimension
+          image_embedding_size (tuple(int, int)): The spatial size of the
+            image embedding, as (H, W).
+          input_image_size (int): The padded size of the image as input
+            to the image encoder, as (H, W).
+          mask_in_chans (int): The number of hidden channels used for
+            encoding input masks.
+          activation (nn.Module): The activation to use when encoding
+            input masks.
+        """
+        super().__init__()
+        self.embed_dim = embed_dim
+        self.input_image_size = input_image_size
+        self.image_embedding_size = image_embedding_size
+        self.pe_layer = PositionEmbeddingRandom(embed_dim // 2)
+
+        self.num_point_embeddings: int = 4  # pos/neg point + 2 box corners
+        point_embeddings = [nn.Embedding(1, embed_dim) for i in range(self.num_point_embeddings)]
+        self.point_embeddings = nn.ModuleList(point_embeddings)
+        self.not_a_point_embed = nn.Embedding(1, embed_dim)
+
+        self.mask_input_size = (4 * image_embedding_size[0], 4 * image_embedding_size[1])
+        self.mask_downscaling = nn.Sequential(
+            nn.Conv2d(1, mask_in_chans // 4, kernel_size=2, stride=2),
+            LayerNorm2d(mask_in_chans // 4),
+            activation(),
+            nn.Conv2d(mask_in_chans // 4, mask_in_chans, kernel_size=2, stride=2),
+            LayerNorm2d(mask_in_chans),
+            activation(),
+            nn.Conv2d(mask_in_chans, embed_dim, kernel_size=1),
+        )
+        self.no_mask_embed = nn.Embedding(1, embed_dim)
+
+    def get_dense_pe(self) -> torch.Tensor:
+        """
+        Returns the positional encoding used to encode point prompts,
+        applied to a dense set of points the shape of the image encoding.
+
+        Returns:
+          torch.Tensor: Positional encoding with shape
+            1x(embed_dim)x(embedding_h)x(embedding_w)
+        """
+        return self.pe_layer(self.image_embedding_size).unsqueeze(0)
+
+    def _embed_points(
+        self,
+        points: torch.Tensor,
+        labels: torch.Tensor,
+        pad: bool,
+    ) -> torch.Tensor:
+        """Embeds point prompts."""
+        points = points + 0.5  # Shift to center of pixel
+        if pad:
+            padding_point = torch.zeros((points.shape[0], 1, 2), device=points.device)
+            padding_label = -torch.ones((labels.shape[0], 1), device=labels.device)
+            points = torch.cat([points, padding_point], dim=1)
+            labels = torch.cat([labels, padding_label], dim=1)
+        point_embedding = self.pe_layer.forward_with_coords(points, self.input_image_size)
+        point_embedding[labels == -1] = 0.0
+        point_embedding[labels == -1] += self.not_a_point_embed.weight
+        point_embedding[labels == 0] += self.point_embeddings[0].weight
+        point_embedding[labels == 1] += self.point_embeddings[1].weight
+        return point_embedding
+
+    def _embed_boxes(self, boxes: torch.Tensor) -> torch.Tensor:
+        """Embeds box prompts."""
+        boxes = boxes + 0.5  # Shift to center of pixel
+        coords = boxes.reshape(-1, 2, 2)
+        corner_embedding = self.pe_layer.forward_with_coords(coords, self.input_image_size)
+        corner_embedding[:, 0, :] += self.point_embeddings[2].weight
+        corner_embedding[:, 1, :] += self.point_embeddings[3].weight
+        return corner_embedding
+
+    def _embed_masks(self, masks: torch.Tensor) -> torch.Tensor:
+        """Embeds mask inputs."""
+        mask_embedding = self.mask_downscaling(masks)
+        return mask_embedding
+
+    def _get_batch_size(
+        self,
+        points: Optional[Tuple[torch.Tensor, torch.Tensor]],
+        boxes: Optional[torch.Tensor],
+        masks: Optional[torch.Tensor],
+    ) -> int:
+        """
+        Gets the batch size of the output given the batch size of the input prompts.
+        """
+        if points is not None:
+            return points[0].shape[0]
+        elif boxes is not None:
+            return boxes.shape[0]
+        elif masks is not None:
+            return masks.shape[0]
+        else:
+            return 1
+
+    def _get_device(self) -> torch.device:
+        return self.point_embeddings[0].weight.device
+
+    def forward(
+        self,
+        points: Optional[Tuple[torch.Tensor, torch.Tensor]],
+        boxes: Optional[torch.Tensor],
+        masks: Optional[torch.Tensor],
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        """
+        Embeds different types of prompts, returning both sparse and dense
+        embeddings.
+
+        Arguments:
+          points (tuple(torch.Tensor, torch.Tensor) or none): point coordinates
+            and labels to embed.
+          boxes (torch.Tensor or none): boxes to embed
+          masks (torch.Tensor or none): masks to embed
+
+        Returns:
+          torch.Tensor: sparse embeddings for the points and boxes, with shape
+            BxNx(embed_dim), where N is determined by the number of input points
+            and boxes.
+          torch.Tensor: dense embeddings for the masks, in the shape
+            Bx(embed_dim)x(embed_H)x(embed_W)
+        """
+        bs = self._get_batch_size(points, boxes, masks)
+        sparse_embeddings = torch.empty((bs, 0, self.embed_dim), device=self._get_device())
+        if points is not None:
+            coords, labels = points
+            point_embeddings = self._embed_points(coords, labels, pad=(boxes is None))
+            sparse_embeddings = torch.cat([sparse_embeddings, point_embeddings], dim=1)
+        if boxes is not None:
+            box_embeddings = self._embed_boxes(boxes)
+            sparse_embeddings = torch.cat([sparse_embeddings, box_embeddings], dim=1)
+
+        if masks is not None:
+            dense_embeddings = self._embed_masks(masks)
+        else:
+            dense_embeddings = self.no_mask_embed.weight.reshape(1, -1, 1, 1).expand(
+                bs, -1, self.image_embedding_size[0], self.image_embedding_size[1]
+            )
+
+        return sparse_embeddings, dense_embeddings
+
+
+class PositionEmbeddingRandom(nn.Module):
+    """
+    Positional encoding using random spatial frequencies.
+    """
+
+    def __init__(self, num_pos_feats: int = 64, scale: Optional[float] = None) -> None:
+        super().__init__()
+        if scale is None or scale <= 0.0:
+            scale = 1.0
+        self.register_buffer(
+            "positional_encoding_gaussian_matrix",
+            scale * torch.randn((2, num_pos_feats)),
+        )
+
+    def _pe_encoding(self, coords: torch.Tensor) -> torch.Tensor:
+        """Positionally encode points that are normalized to [0,1]."""
+        # assuming coords are in [0, 1]^2 square and have d_1 x ... x d_n x 2 shape
+        coords = 2 * coords - 1
+        coords = coords @ self.positional_encoding_gaussian_matrix
+        coords = 2 * np.pi * coords
+        # outputs d_1 x ... x d_n x C shape
+        return torch.cat([torch.sin(coords), torch.cos(coords)], dim=-1)
+
+    def forward(self, size: Tuple[int, int]) -> torch.Tensor:
+        """Generate positional encoding for a grid of the specified size."""
+        h, w = size
+        device: Any = self.positional_encoding_gaussian_matrix.device
+        grid = torch.ones((h, w), device=device, dtype=torch.float32)
+        y_embed = grid.cumsum(dim=0) - 0.5
+        x_embed = grid.cumsum(dim=1) - 0.5
+        y_embed = y_embed / h
+        x_embed = x_embed / w
+
+        pe = self._pe_encoding(torch.stack([x_embed, y_embed], dim=-1))
+        return pe.permute(2, 0, 1)  # C x H x W
+
+    def forward_with_coords(
+        self, coords_input: torch.Tensor, image_size: Tuple[int, int]
+    ) -> torch.Tensor:
+        """Positionally encode points that are not normalized to [0,1]."""
+        coords = coords_input.clone()
+        coords[:, :, 0] = coords[:, :, 0] / image_size[1]
+        coords[:, :, 1] = coords[:, :, 1] / image_size[0]
+        return self._pe_encoding(coords.to(torch.float))  # B x N x C
```

### Comparing `npsam-1.4.5/npsam/segment_anything/modeling/transformer.py` & `npsam-1.4.6/npsam/segment_anything/modeling/transformer.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,240 +1,240 @@
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-# All rights reserved.
-
-# This source code is licensed under the license found in the
-# LICENSE file in the root directory of this source tree.
-
-import torch
-from torch import Tensor, nn
-
-import math
-from typing import Tuple, Type
-
-from .common import MLPBlock
-
-
-class TwoWayTransformer(nn.Module):
-    def __init__(
-        self,
-        depth: int,
-        embedding_dim: int,
-        num_heads: int,
-        mlp_dim: int,
-        activation: Type[nn.Module] = nn.ReLU,
-        attention_downsample_rate: int = 2,
-    ) -> None:
-        """
-        A transformer decoder that attends to an input image using
-        queries whose positional embedding is supplied.
-
-        Args:
-          depth (int): number of layers in the transformer
-          embedding_dim (int): the channel dimension for the input embeddings
-          num_heads (int): the number of heads for multihead attention. Must
-            divide embedding_dim
-          mlp_dim (int): the channel dimension internal to the MLP block
-          activation (nn.Module): the activation to use in the MLP block
-        """
-        super().__init__()
-        self.depth = depth
-        self.embedding_dim = embedding_dim
-        self.num_heads = num_heads
-        self.mlp_dim = mlp_dim
-        self.layers = nn.ModuleList()
-
-        for i in range(depth):
-            self.layers.append(
-                TwoWayAttentionBlock(
-                    embedding_dim=embedding_dim,
-                    num_heads=num_heads,
-                    mlp_dim=mlp_dim,
-                    activation=activation,
-                    attention_downsample_rate=attention_downsample_rate,
-                    skip_first_layer_pe=(i == 0),
-                )
-            )
-
-        self.final_attn_token_to_image = Attention(
-            embedding_dim, num_heads, downsample_rate=attention_downsample_rate
-        )
-        self.norm_final_attn = nn.LayerNorm(embedding_dim)
-
-    def forward(
-        self,
-        image_embedding: Tensor,
-        image_pe: Tensor,
-        point_embedding: Tensor,
-    ) -> Tuple[Tensor, Tensor]:
-        """
-        Args:
-          image_embedding (torch.Tensor): image to attend to. Should be shape
-            B x embedding_dim x h x w for any h and w.
-          image_pe (torch.Tensor): the positional encoding to add to the image. Must
-            have the same shape as image_embedding.
-          point_embedding (torch.Tensor): the embedding to add to the query points.
-            Must have shape B x N_points x embedding_dim for any N_points.
-
-        Returns:
-          torch.Tensor: the processed point_embedding
-          torch.Tensor: the processed image_embedding
-        """
-        # BxCxHxW -> BxHWxC == B x N_image_tokens x C
-        bs, c, h, w = image_embedding.shape
-        image_embedding = image_embedding.flatten(2).permute(0, 2, 1)
-        image_pe = image_pe.flatten(2).permute(0, 2, 1)
-
-        # Prepare queries
-        queries = point_embedding
-        keys = image_embedding
-
-        # Apply transformer blocks and final layernorm
-        for layer in self.layers:
-            queries, keys = layer(
-                queries=queries,
-                keys=keys,
-                query_pe=point_embedding,
-                key_pe=image_pe,
-            )
-
-        # Apply the final attention layer from the points to the image
-        q = queries + point_embedding
-        k = keys + image_pe
-        attn_out = self.final_attn_token_to_image(q=q, k=k, v=keys)
-        queries = queries + attn_out
-        queries = self.norm_final_attn(queries)
-
-        return queries, keys
-
-
-class TwoWayAttentionBlock(nn.Module):
-    def __init__(
-        self,
-        embedding_dim: int,
-        num_heads: int,
-        mlp_dim: int = 2048,
-        activation: Type[nn.Module] = nn.ReLU,
-        attention_downsample_rate: int = 2,
-        skip_first_layer_pe: bool = False,
-    ) -> None:
-        """
-        A transformer block with four layers: (1) self-attention of sparse
-        inputs, (2) cross attention of sparse inputs to dense inputs, (3) mlp
-        block on sparse inputs, and (4) cross attention of dense inputs to sparse
-        inputs.
-
-        Arguments:
-          embedding_dim (int): the channel dimension of the embeddings
-          num_heads (int): the number of heads in the attention layers
-          mlp_dim (int): the hidden dimension of the mlp block
-          activation (nn.Module): the activation of the mlp block
-          skip_first_layer_pe (bool): skip the PE on the first layer
-        """
-        super().__init__()
-        self.self_attn = Attention(embedding_dim, num_heads)
-        self.norm1 = nn.LayerNorm(embedding_dim)
-
-        self.cross_attn_token_to_image = Attention(
-            embedding_dim, num_heads, downsample_rate=attention_downsample_rate
-        )
-        self.norm2 = nn.LayerNorm(embedding_dim)
-
-        self.mlp = MLPBlock(embedding_dim, mlp_dim, activation)
-        self.norm3 = nn.LayerNorm(embedding_dim)
-
-        self.norm4 = nn.LayerNorm(embedding_dim)
-        self.cross_attn_image_to_token = Attention(
-            embedding_dim, num_heads, downsample_rate=attention_downsample_rate
-        )
-
-        self.skip_first_layer_pe = skip_first_layer_pe
-
-    def forward(
-        self, queries: Tensor, keys: Tensor, query_pe: Tensor, key_pe: Tensor
-    ) -> Tuple[Tensor, Tensor]:
-        # Self attention block
-        if self.skip_first_layer_pe:
-            queries = self.self_attn(q=queries, k=queries, v=queries)
-        else:
-            q = queries + query_pe
-            attn_out = self.self_attn(q=q, k=q, v=queries)
-            queries = queries + attn_out
-        queries = self.norm1(queries)
-
-        # Cross attention block, tokens attending to image embedding
-        q = queries + query_pe
-        k = keys + key_pe
-        attn_out = self.cross_attn_token_to_image(q=q, k=k, v=keys)
-        queries = queries + attn_out
-        queries = self.norm2(queries)
-
-        # MLP block
-        mlp_out = self.mlp(queries)
-        queries = queries + mlp_out
-        queries = self.norm3(queries)
-
-        # Cross attention block, image embedding attending to tokens
-        q = queries + query_pe
-        k = keys + key_pe
-        attn_out = self.cross_attn_image_to_token(q=k, k=q, v=queries)
-        keys = keys + attn_out
-        keys = self.norm4(keys)
-
-        return queries, keys
-
-
-class Attention(nn.Module):
-    """
-    An attention layer that allows for downscaling the size of the embedding
-    after projection to queries, keys, and values.
-    """
-
-    def __init__(
-        self,
-        embedding_dim: int,
-        num_heads: int,
-        downsample_rate: int = 1,
-    ) -> None:
-        super().__init__()
-        self.embedding_dim = embedding_dim
-        self.internal_dim = embedding_dim // downsample_rate
-        self.num_heads = num_heads
-        assert self.internal_dim % num_heads == 0, "num_heads must divide embedding_dim."
-
-        self.q_proj = nn.Linear(embedding_dim, self.internal_dim)
-        self.k_proj = nn.Linear(embedding_dim, self.internal_dim)
-        self.v_proj = nn.Linear(embedding_dim, self.internal_dim)
-        self.out_proj = nn.Linear(self.internal_dim, embedding_dim)
-
-    def _separate_heads(self, x: Tensor, num_heads: int) -> Tensor:
-        b, n, c = x.shape
-        x = x.reshape(b, n, num_heads, c // num_heads)
-        return x.transpose(1, 2)  # B x N_heads x N_tokens x C_per_head
-
-    def _recombine_heads(self, x: Tensor) -> Tensor:
-        b, n_heads, n_tokens, c_per_head = x.shape
-        x = x.transpose(1, 2)
-        return x.reshape(b, n_tokens, n_heads * c_per_head)  # B x N_tokens x C
-
-    def forward(self, q: Tensor, k: Tensor, v: Tensor) -> Tensor:
-        # Input projections
-        q = self.q_proj(q)
-        k = self.k_proj(k)
-        v = self.v_proj(v)
-
-        # Separate into heads
-        q = self._separate_heads(q, self.num_heads)
-        k = self._separate_heads(k, self.num_heads)
-        v = self._separate_heads(v, self.num_heads)
-
-        # Attention
-        _, _, _, c_per_head = q.shape
-        attn = q @ k.permute(0, 1, 3, 2)  # B x N_heads x N_tokens x N_tokens
-        attn = attn / math.sqrt(c_per_head)
-        attn = torch.softmax(attn, dim=-1)
-
-        # Get output
-        out = attn @ v
-        out = self._recombine_heads(out)
-        out = self.out_proj(out)
-
-        return out
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
+import torch
+from torch import Tensor, nn
+
+import math
+from typing import Tuple, Type
+
+from .common import MLPBlock
+
+
+class TwoWayTransformer(nn.Module):
+    def __init__(
+        self,
+        depth: int,
+        embedding_dim: int,
+        num_heads: int,
+        mlp_dim: int,
+        activation: Type[nn.Module] = nn.ReLU,
+        attention_downsample_rate: int = 2,
+    ) -> None:
+        """
+        A transformer decoder that attends to an input image using
+        queries whose positional embedding is supplied.
+
+        Args:
+          depth (int): number of layers in the transformer
+          embedding_dim (int): the channel dimension for the input embeddings
+          num_heads (int): the number of heads for multihead attention. Must
+            divide embedding_dim
+          mlp_dim (int): the channel dimension internal to the MLP block
+          activation (nn.Module): the activation to use in the MLP block
+        """
+        super().__init__()
+        self.depth = depth
+        self.embedding_dim = embedding_dim
+        self.num_heads = num_heads
+        self.mlp_dim = mlp_dim
+        self.layers = nn.ModuleList()
+
+        for i in range(depth):
+            self.layers.append(
+                TwoWayAttentionBlock(
+                    embedding_dim=embedding_dim,
+                    num_heads=num_heads,
+                    mlp_dim=mlp_dim,
+                    activation=activation,
+                    attention_downsample_rate=attention_downsample_rate,
+                    skip_first_layer_pe=(i == 0),
+                )
+            )
+
+        self.final_attn_token_to_image = Attention(
+            embedding_dim, num_heads, downsample_rate=attention_downsample_rate
+        )
+        self.norm_final_attn = nn.LayerNorm(embedding_dim)
+
+    def forward(
+        self,
+        image_embedding: Tensor,
+        image_pe: Tensor,
+        point_embedding: Tensor,
+    ) -> Tuple[Tensor, Tensor]:
+        """
+        Args:
+          image_embedding (torch.Tensor): image to attend to. Should be shape
+            B x embedding_dim x h x w for any h and w.
+          image_pe (torch.Tensor): the positional encoding to add to the image. Must
+            have the same shape as image_embedding.
+          point_embedding (torch.Tensor): the embedding to add to the query points.
+            Must have shape B x N_points x embedding_dim for any N_points.
+
+        Returns:
+          torch.Tensor: the processed point_embedding
+          torch.Tensor: the processed image_embedding
+        """
+        # BxCxHxW -> BxHWxC == B x N_image_tokens x C
+        bs, c, h, w = image_embedding.shape
+        image_embedding = image_embedding.flatten(2).permute(0, 2, 1)
+        image_pe = image_pe.flatten(2).permute(0, 2, 1)
+
+        # Prepare queries
+        queries = point_embedding
+        keys = image_embedding
+
+        # Apply transformer blocks and final layernorm
+        for layer in self.layers:
+            queries, keys = layer(
+                queries=queries,
+                keys=keys,
+                query_pe=point_embedding,
+                key_pe=image_pe,
+            )
+
+        # Apply the final attention layer from the points to the image
+        q = queries + point_embedding
+        k = keys + image_pe
+        attn_out = self.final_attn_token_to_image(q=q, k=k, v=keys)
+        queries = queries + attn_out
+        queries = self.norm_final_attn(queries)
+
+        return queries, keys
+
+
+class TwoWayAttentionBlock(nn.Module):
+    def __init__(
+        self,
+        embedding_dim: int,
+        num_heads: int,
+        mlp_dim: int = 2048,
+        activation: Type[nn.Module] = nn.ReLU,
+        attention_downsample_rate: int = 2,
+        skip_first_layer_pe: bool = False,
+    ) -> None:
+        """
+        A transformer block with four layers: (1) self-attention of sparse
+        inputs, (2) cross attention of sparse inputs to dense inputs, (3) mlp
+        block on sparse inputs, and (4) cross attention of dense inputs to sparse
+        inputs.
+
+        Arguments:
+          embedding_dim (int): the channel dimension of the embeddings
+          num_heads (int): the number of heads in the attention layers
+          mlp_dim (int): the hidden dimension of the mlp block
+          activation (nn.Module): the activation of the mlp block
+          skip_first_layer_pe (bool): skip the PE on the first layer
+        """
+        super().__init__()
+        self.self_attn = Attention(embedding_dim, num_heads)
+        self.norm1 = nn.LayerNorm(embedding_dim)
+
+        self.cross_attn_token_to_image = Attention(
+            embedding_dim, num_heads, downsample_rate=attention_downsample_rate
+        )
+        self.norm2 = nn.LayerNorm(embedding_dim)
+
+        self.mlp = MLPBlock(embedding_dim, mlp_dim, activation)
+        self.norm3 = nn.LayerNorm(embedding_dim)
+
+        self.norm4 = nn.LayerNorm(embedding_dim)
+        self.cross_attn_image_to_token = Attention(
+            embedding_dim, num_heads, downsample_rate=attention_downsample_rate
+        )
+
+        self.skip_first_layer_pe = skip_first_layer_pe
+
+    def forward(
+        self, queries: Tensor, keys: Tensor, query_pe: Tensor, key_pe: Tensor
+    ) -> Tuple[Tensor, Tensor]:
+        # Self attention block
+        if self.skip_first_layer_pe:
+            queries = self.self_attn(q=queries, k=queries, v=queries)
+        else:
+            q = queries + query_pe
+            attn_out = self.self_attn(q=q, k=q, v=queries)
+            queries = queries + attn_out
+        queries = self.norm1(queries)
+
+        # Cross attention block, tokens attending to image embedding
+        q = queries + query_pe
+        k = keys + key_pe
+        attn_out = self.cross_attn_token_to_image(q=q, k=k, v=keys)
+        queries = queries + attn_out
+        queries = self.norm2(queries)
+
+        # MLP block
+        mlp_out = self.mlp(queries)
+        queries = queries + mlp_out
+        queries = self.norm3(queries)
+
+        # Cross attention block, image embedding attending to tokens
+        q = queries + query_pe
+        k = keys + key_pe
+        attn_out = self.cross_attn_image_to_token(q=k, k=q, v=queries)
+        keys = keys + attn_out
+        keys = self.norm4(keys)
+
+        return queries, keys
+
+
+class Attention(nn.Module):
+    """
+    An attention layer that allows for downscaling the size of the embedding
+    after projection to queries, keys, and values.
+    """
+
+    def __init__(
+        self,
+        embedding_dim: int,
+        num_heads: int,
+        downsample_rate: int = 1,
+    ) -> None:
+        super().__init__()
+        self.embedding_dim = embedding_dim
+        self.internal_dim = embedding_dim // downsample_rate
+        self.num_heads = num_heads
+        assert self.internal_dim % num_heads == 0, "num_heads must divide embedding_dim."
+
+        self.q_proj = nn.Linear(embedding_dim, self.internal_dim)
+        self.k_proj = nn.Linear(embedding_dim, self.internal_dim)
+        self.v_proj = nn.Linear(embedding_dim, self.internal_dim)
+        self.out_proj = nn.Linear(self.internal_dim, embedding_dim)
+
+    def _separate_heads(self, x: Tensor, num_heads: int) -> Tensor:
+        b, n, c = x.shape
+        x = x.reshape(b, n, num_heads, c // num_heads)
+        return x.transpose(1, 2)  # B x N_heads x N_tokens x C_per_head
+
+    def _recombine_heads(self, x: Tensor) -> Tensor:
+        b, n_heads, n_tokens, c_per_head = x.shape
+        x = x.transpose(1, 2)
+        return x.reshape(b, n_tokens, n_heads * c_per_head)  # B x N_tokens x C
+
+    def forward(self, q: Tensor, k: Tensor, v: Tensor) -> Tensor:
+        # Input projections
+        q = self.q_proj(q)
+        k = self.k_proj(k)
+        v = self.v_proj(v)
+
+        # Separate into heads
+        q = self._separate_heads(q, self.num_heads)
+        k = self._separate_heads(k, self.num_heads)
+        v = self._separate_heads(v, self.num_heads)
+
+        # Attention
+        _, _, _, c_per_head = q.shape
+        attn = q @ k.permute(0, 1, 3, 2)  # B x N_heads x N_tokens x N_tokens
+        attn = attn / math.sqrt(c_per_head)
+        attn = torch.softmax(attn, dim=-1)
+
+        # Get output
+        out = attn @ v
+        out = self._recombine_heads(out)
+        out = self.out_proj(out)
+
+        return out
```

### Comparing `npsam-1.4.5/npsam/segment_anything/predictor.py` & `npsam-1.4.6/npsam/segment_anything/predictor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,270 +1,269 @@
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-# All rights reserved.
-
-# This source code is licensed under the license found in the
-# LICENSE file in the root directory of this source tree.
-
-import numpy as np
-import torch
-
-# Original: from .segment_anything.modeling import Sam
-from .modeling import Sam
-
-from typing import Optional, Tuple
-
-from .utils.transforms import ResizeLongestSide
-
-
-class SamPredictor:
-    def __init__(
-        self,
-        sam_model: Sam,
-    ) -> None:
-        """
-        Uses SAM to calculate the image embedding for an image, and then
-        allow repeated, efficient mask prediction given prompts.
-
-        Arguments:
-          sam_model (Sam): The model to use for mask prediction.
-        """
-        super().__init__()
-        self.model = sam_model
-        self.transform = ResizeLongestSide(sam_model.image_encoder.img_size)
-        self.reset_image()
-
-    def set_image(
-        self,
-        image: np.ndarray,
-        image_format: str = "RGB",
-    ) -> None:
-        """
-        Calculates the image embeddings for the provided image, allowing
-        masks to be predicted with the 'predict' method.
-
-        Arguments:
-          image (np.ndarray): The image for calculating masks. Expects an
-            image in HWC uint8 format, with pixel values in [0, 255].
-          image_format (str): The color format of the image, in ['RGB', 'BGR'].
-        """
-        assert image_format in [
-            "RGB",
-            "BGR",
-        ], f"image_format must be in ['RGB', 'BGR'], is {image_format}."
-        if image_format != self.model.image_format:
-            image = image[..., ::-1]
-
-        # Transform the image to the form expected by the model
-        input_image = self.transform.apply_image(image)
-        input_image_torch = torch.as_tensor(input_image, device=self.device)
-        input_image_torch = input_image_torch.permute(2, 0, 1).contiguous()[None, :, :, :]
-
-        self.set_torch_image(input_image_torch, image.shape[:2])
-
-    @torch.no_grad()
-    def set_torch_image(
-        self,
-        transformed_image: torch.Tensor,
-        original_image_size: Tuple[int, ...],
-    ) -> None:
-        """
-        Calculates the image embeddings for the provided image, allowing
-        masks to be predicted with the 'predict' method. Expects the input
-        image to be already transformed to the format expected by the model.
-
-        Arguments:
-          transformed_image (torch.Tensor): The input image, with shape
-            1x3xHxW, which has been transformed with ResizeLongestSide.
-          original_image_size (tuple(int, int)): The size of the image
-            before transformation, in (H, W) format.
-        """
-        assert (
-            len(transformed_image.shape) == 4
-            and transformed_image.shape[1] == 3
-            and max(*transformed_image.shape[2:]) == self.model.image_encoder.img_size
-        ), f"set_torch_image input must be BCHW with long side {self.model.image_encoder.img_size}."
-        self.reset_image()
-
-        self.original_size = original_image_size
-        self.input_size = tuple(transformed_image.shape[-2:])
-        input_image = self.model.preprocess(transformed_image)
-        self.features = self.model.image_encoder(input_image)
-        self.is_image_set = True
-
-    def predict(
-        self,
-        point_coords: Optional[np.ndarray] = None,
-        point_labels: Optional[np.ndarray] = None,
-        box: Optional[np.ndarray] = None,
-        mask_input: Optional[np.ndarray] = None,
-        multimask_output: bool = True,
-        return_logits: bool = False,
-    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-        """
-        Predict masks for the given input prompts, using the currently set image.
-
-        Arguments:
-          point_coords (np.ndarray or None): A Nx2 array of point prompts to the
-            model. Each point is in (X,Y) in pixels.
-          point_labels (np.ndarray or None): A length N array of labels for the
-            point prompts. 1 indicates a foreground point and 0 indicates a
-            background point.
-          box (np.ndarray or None): A length 4 array given a box prompt to the
-            model, in XYXY format.
-          mask_input (np.ndarray): A low resolution mask input to the model, typically
-            coming from a previous prediction iteration. Has form 1xHxW, where
-            for SAM, H=W=256.
-          multimask_output (bool): If true, the model will return three masks.
-            For ambiguous input prompts (such as a single click), this will often
-            produce better masks than a single prediction. If only a single
-            mask is needed, the model's predicted quality score can be used
-            to select the best mask. For non-ambiguous prompts, such as multiple
-            input prompts, multimask_output=False can give better results.
-          return_logits (bool): If true, returns un-thresholded masks logits
-            instead of a binary mask.
-
-        Returns:
-          (np.ndarray): The output masks in CxHxW format, where C is the
-            number of masks, and (H, W) is the original image size.
-          (np.ndarray): An array of length C containing the model's
-            predictions for the quality of each mask.
-          (np.ndarray): An array of shape CxHxW, where C is the number
-            of masks and H=W=256. These low resolution logits can be passed to
-            a subsequent iteration as mask input.
-        """
-        if not self.is_image_set:
-            raise RuntimeError("An image must be set with .set_image(...) before mask prediction.")
-
-        # Transform input prompts
-        coords_torch, labels_torch, box_torch, mask_input_torch = None, None, None, None
-        if point_coords is not None:
-            assert (
-                point_labels is not None
-            ), "point_labels must be supplied if point_coords is supplied."
-            point_coords = self.transform.apply_coords(point_coords, self.original_size)
-            coords_torch = torch.as_tensor(point_coords, dtype=torch.float, device=self.device)
-            labels_torch = torch.as_tensor(point_labels, dtype=torch.int, device=self.device)
-            coords_torch, labels_torch = coords_torch[None, :, :], labels_torch[None, :]
-        if box is not None:
-            box = self.transform.apply_boxes(box, self.original_size)
-            box_torch = torch.as_tensor(box, dtype=torch.float, device=self.device)
-            box_torch = box_torch[None, :]
-        if mask_input is not None:
-            mask_input_torch = torch.as_tensor(mask_input, dtype=torch.float, device=self.device)
-            mask_input_torch = mask_input_torch[None, :, :, :]
-
-        masks, iou_predictions, low_res_masks = self.predict_torch(
-            coords_torch,
-            labels_torch,
-            box_torch,
-            mask_input_torch,
-            multimask_output,
-            return_logits=return_logits,
-        )
-
-        masks_np = masks[0].detach().cpu().numpy()
-        iou_predictions_np = iou_predictions[0].detach().cpu().numpy()
-        low_res_masks_np = low_res_masks[0].detach().cpu().numpy()
-        return masks_np, iou_predictions_np, low_res_masks_np
-
-    @torch.no_grad()
-    def predict_torch(
-        self,
-        point_coords: Optional[torch.Tensor],
-        point_labels: Optional[torch.Tensor],
-        boxes: Optional[torch.Tensor] = None,
-        mask_input: Optional[torch.Tensor] = None,
-        multimask_output: bool = True,
-        return_logits: bool = False,
-    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        """
-        Predict masks for the given input prompts, using the currently set image.
-        Input prompts are batched torch tensors and are expected to already be
-        transformed to the input frame using ResizeLongestSide.
-
-        Arguments:
-          point_coords (torch.Tensor or None): A BxNx2 array of point prompts to the
-            model. Each point is in (X,Y) in pixels.
-          point_labels (torch.Tensor or None): A BxN array of labels for the
-            point prompts. 1 indicates a foreground point and 0 indicates a
-            background point.
-          boxes (np.ndarray or None): A Bx4 array given a box prompt to the
-            model, in XYXY format.
-          mask_input (np.ndarray): A low resolution mask input to the model, typically
-            coming from a previous prediction iteration. Has form Bx1xHxW, where
-            for SAM, H=W=256. Masks returned by a previous iteration of the
-            predict method do not need further transformation.
-          multimask_output (bool): If true, the model will return three masks.
-            For ambiguous input prompts (such as a single click), this will often
-            produce better masks than a single prediction. If only a single
-            mask is needed, the model's predicted quality score can be used
-            to select the best mask. For non-ambiguous prompts, such as multiple
-            input prompts, multimask_output=False can give better results.
-          return_logits (bool): If true, returns un-thresholded masks logits
-            instead of a binary mask.
-
-        Returns:
-          (torch.Tensor): The output masks in BxCxHxW format, where C is the
-            number of masks, and (H, W) is the original image size.
-          (torch.Tensor): An array of shape BxC containing the model's
-            predictions for the quality of each mask.
-          (torch.Tensor): An array of shape BxCxHxW, where C is the number
-            of masks and H=W=256. These low res logits can be passed to
-            a subsequent iteration as mask input.
-        """
-        if not self.is_image_set:
-            raise RuntimeError("An image must be set with .set_image(...) before mask prediction.")
-
-        if point_coords is not None:
-            points = (point_coords, point_labels)
-        else:
-            points = None
-
-        # Embed prompts
-        sparse_embeddings, dense_embeddings = self.model.prompt_encoder(
-            points=points,
-            boxes=boxes,
-            masks=mask_input,
-        )
-
-        # Predict masks
-        low_res_masks, iou_predictions = self.model.mask_decoder(
-            image_embeddings=self.features,
-            image_pe=self.model.prompt_encoder.get_dense_pe(),
-            sparse_prompt_embeddings=sparse_embeddings,
-            dense_prompt_embeddings=dense_embeddings,
-            multimask_output=multimask_output,
-        )
-
-        # Upscale the masks to the original image resolution
-        masks = self.model.postprocess_masks(low_res_masks, self.input_size, self.original_size)
-
-        if not return_logits:
-            masks = masks > self.model.mask_threshold
-
-        return masks, iou_predictions, low_res_masks
-
-    def get_image_embedding(self) -> torch.Tensor:
-        """
-        Returns the image embeddings for the currently set image, with
-        shape 1xCxHxW, where C is the embedding dimension and (H,W) are
-        the embedding spatial dimension of SAM (typically C=256, H=W=64).
-        """
-        if not self.is_image_set:
-            raise RuntimeError(
-                "An image must be set with .set_image(...) to generate an embedding."
-            )
-        assert self.features is not None, "Features must exist if an image has been set."
-        return self.features
-
-    @property
-    def device(self) -> torch.device:
-        return self.model.device
-
-    def reset_image(self) -> None:
-        """Resets the currently set image."""
-        self.is_image_set = False
-        self.features = None
-        self.orig_h = None
-        self.orig_w = None
-        self.input_h = None
-        self.input_w = None
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
+import numpy as np
+import torch
+
+from segment_anything.modeling import Sam
+
+from typing import Optional, Tuple
+
+from .utils.transforms import ResizeLongestSide
+
+
+class SamPredictor:
+    def __init__(
+        self,
+        sam_model: Sam,
+    ) -> None:
+        """
+        Uses SAM to calculate the image embedding for an image, and then
+        allow repeated, efficient mask prediction given prompts.
+
+        Arguments:
+          sam_model (Sam): The model to use for mask prediction.
+        """
+        super().__init__()
+        self.model = sam_model
+        self.transform = ResizeLongestSide(sam_model.image_encoder.img_size)
+        self.reset_image()
+
+    def set_image(
+        self,
+        image: np.ndarray,
+        image_format: str = "RGB",
+    ) -> None:
+        """
+        Calculates the image embeddings for the provided image, allowing
+        masks to be predicted with the 'predict' method.
+
+        Arguments:
+          image (np.ndarray): The image for calculating masks. Expects an
+            image in HWC uint8 format, with pixel values in [0, 255].
+          image_format (str): The color format of the image, in ['RGB', 'BGR'].
+        """
+        assert image_format in [
+            "RGB",
+            "BGR",
+        ], f"image_format must be in ['RGB', 'BGR'], is {image_format}."
+        if image_format != self.model.image_format:
+            image = image[..., ::-1]
+
+        # Transform the image to the form expected by the model
+        input_image = self.transform.apply_image(image)
+        input_image_torch = torch.as_tensor(input_image, device=self.device)
+        input_image_torch = input_image_torch.permute(2, 0, 1).contiguous()[None, :, :, :]
+
+        self.set_torch_image(input_image_torch, image.shape[:2])
+
+    @torch.no_grad()
+    def set_torch_image(
+        self,
+        transformed_image: torch.Tensor,
+        original_image_size: Tuple[int, ...],
+    ) -> None:
+        """
+        Calculates the image embeddings for the provided image, allowing
+        masks to be predicted with the 'predict' method. Expects the input
+        image to be already transformed to the format expected by the model.
+
+        Arguments:
+          transformed_image (torch.Tensor): The input image, with shape
+            1x3xHxW, which has been transformed with ResizeLongestSide.
+          original_image_size (tuple(int, int)): The size of the image
+            before transformation, in (H, W) format.
+        """
+        assert (
+            len(transformed_image.shape) == 4
+            and transformed_image.shape[1] == 3
+            and max(*transformed_image.shape[2:]) == self.model.image_encoder.img_size
+        ), f"set_torch_image input must be BCHW with long side {self.model.image_encoder.img_size}."
+        self.reset_image()
+
+        self.original_size = original_image_size
+        self.input_size = tuple(transformed_image.shape[-2:])
+        input_image = self.model.preprocess(transformed_image)
+        self.features = self.model.image_encoder(input_image)
+        self.is_image_set = True
+
+    def predict(
+        self,
+        point_coords: Optional[np.ndarray] = None,
+        point_labels: Optional[np.ndarray] = None,
+        box: Optional[np.ndarray] = None,
+        mask_input: Optional[np.ndarray] = None,
+        multimask_output: bool = True,
+        return_logits: bool = False,
+    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """
+        Predict masks for the given input prompts, using the currently set image.
+
+        Arguments:
+          point_coords (np.ndarray or None): A Nx2 array of point prompts to the
+            model. Each point is in (X,Y) in pixels.
+          point_labels (np.ndarray or None): A length N array of labels for the
+            point prompts. 1 indicates a foreground point and 0 indicates a
+            background point.
+          box (np.ndarray or None): A length 4 array given a box prompt to the
+            model, in XYXY format.
+          mask_input (np.ndarray): A low resolution mask input to the model, typically
+            coming from a previous prediction iteration. Has form 1xHxW, where
+            for SAM, H=W=256.
+          multimask_output (bool): If true, the model will return three masks.
+            For ambiguous input prompts (such as a single click), this will often
+            produce better masks than a single prediction. If only a single
+            mask is needed, the model's predicted quality score can be used
+            to select the best mask. For non-ambiguous prompts, such as multiple
+            input prompts, multimask_output=False can give better results.
+          return_logits (bool): If true, returns un-thresholded masks logits
+            instead of a binary mask.
+
+        Returns:
+          (np.ndarray): The output masks in CxHxW format, where C is the
+            number of masks, and (H, W) is the original image size.
+          (np.ndarray): An array of length C containing the model's
+            predictions for the quality of each mask.
+          (np.ndarray): An array of shape CxHxW, where C is the number
+            of masks and H=W=256. These low resolution logits can be passed to
+            a subsequent iteration as mask input.
+        """
+        if not self.is_image_set:
+            raise RuntimeError("An image must be set with .set_image(...) before mask prediction.")
+
+        # Transform input prompts
+        coords_torch, labels_torch, box_torch, mask_input_torch = None, None, None, None
+        if point_coords is not None:
+            assert (
+                point_labels is not None
+            ), "point_labels must be supplied if point_coords is supplied."
+            point_coords = self.transform.apply_coords(point_coords, self.original_size)
+            coords_torch = torch.as_tensor(point_coords, dtype=torch.float, device=self.device)
+            labels_torch = torch.as_tensor(point_labels, dtype=torch.int, device=self.device)
+            coords_torch, labels_torch = coords_torch[None, :, :], labels_torch[None, :]
+        if box is not None:
+            box = self.transform.apply_boxes(box, self.original_size)
+            box_torch = torch.as_tensor(box, dtype=torch.float, device=self.device)
+            box_torch = box_torch[None, :]
+        if mask_input is not None:
+            mask_input_torch = torch.as_tensor(mask_input, dtype=torch.float, device=self.device)
+            mask_input_torch = mask_input_torch[None, :, :, :]
+
+        masks, iou_predictions, low_res_masks = self.predict_torch(
+            coords_torch,
+            labels_torch,
+            box_torch,
+            mask_input_torch,
+            multimask_output,
+            return_logits=return_logits,
+        )
+
+        masks_np = masks[0].detach().cpu().numpy()
+        iou_predictions_np = iou_predictions[0].detach().cpu().numpy()
+        low_res_masks_np = low_res_masks[0].detach().cpu().numpy()
+        return masks_np, iou_predictions_np, low_res_masks_np
+
+    @torch.no_grad()
+    def predict_torch(
+        self,
+        point_coords: Optional[torch.Tensor],
+        point_labels: Optional[torch.Tensor],
+        boxes: Optional[torch.Tensor] = None,
+        mask_input: Optional[torch.Tensor] = None,
+        multimask_output: bool = True,
+        return_logits: bool = False,
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        """
+        Predict masks for the given input prompts, using the currently set image.
+        Input prompts are batched torch tensors and are expected to already be
+        transformed to the input frame using ResizeLongestSide.
+
+        Arguments:
+          point_coords (torch.Tensor or None): A BxNx2 array of point prompts to the
+            model. Each point is in (X,Y) in pixels.
+          point_labels (torch.Tensor or None): A BxN array of labels for the
+            point prompts. 1 indicates a foreground point and 0 indicates a
+            background point.
+          boxes (np.ndarray or None): A Bx4 array given a box prompt to the
+            model, in XYXY format.
+          mask_input (np.ndarray): A low resolution mask input to the model, typically
+            coming from a previous prediction iteration. Has form Bx1xHxW, where
+            for SAM, H=W=256. Masks returned by a previous iteration of the
+            predict method do not need further transformation.
+          multimask_output (bool): If true, the model will return three masks.
+            For ambiguous input prompts (such as a single click), this will often
+            produce better masks than a single prediction. If only a single
+            mask is needed, the model's predicted quality score can be used
+            to select the best mask. For non-ambiguous prompts, such as multiple
+            input prompts, multimask_output=False can give better results.
+          return_logits (bool): If true, returns un-thresholded masks logits
+            instead of a binary mask.
+
+        Returns:
+          (torch.Tensor): The output masks in BxCxHxW format, where C is the
+            number of masks, and (H, W) is the original image size.
+          (torch.Tensor): An array of shape BxC containing the model's
+            predictions for the quality of each mask.
+          (torch.Tensor): An array of shape BxCxHxW, where C is the number
+            of masks and H=W=256. These low res logits can be passed to
+            a subsequent iteration as mask input.
+        """
+        if not self.is_image_set:
+            raise RuntimeError("An image must be set with .set_image(...) before mask prediction.")
+
+        if point_coords is not None:
+            points = (point_coords, point_labels)
+        else:
+            points = None
+
+        # Embed prompts
+        sparse_embeddings, dense_embeddings = self.model.prompt_encoder(
+            points=points,
+            boxes=boxes,
+            masks=mask_input,
+        )
+
+        # Predict masks
+        low_res_masks, iou_predictions = self.model.mask_decoder(
+            image_embeddings=self.features,
+            image_pe=self.model.prompt_encoder.get_dense_pe(),
+            sparse_prompt_embeddings=sparse_embeddings,
+            dense_prompt_embeddings=dense_embeddings,
+            multimask_output=multimask_output,
+        )
+
+        # Upscale the masks to the original image resolution
+        masks = self.model.postprocess_masks(low_res_masks, self.input_size, self.original_size)
+
+        if not return_logits:
+            masks = masks > self.model.mask_threshold
+
+        return masks, iou_predictions, low_res_masks
+
+    def get_image_embedding(self) -> torch.Tensor:
+        """
+        Returns the image embeddings for the currently set image, with
+        shape 1xCxHxW, where C is the embedding dimension and (H,W) are
+        the embedding spatial dimension of SAM (typically C=256, H=W=64).
+        """
+        if not self.is_image_set:
+            raise RuntimeError(
+                "An image must be set with .set_image(...) to generate an embedding."
+            )
+        assert self.features is not None, "Features must exist if an image has been set."
+        return self.features
+
+    @property
+    def device(self) -> torch.device:
+        return self.model.device
+
+    def reset_image(self) -> None:
+        """Resets the currently set image."""
+        self.is_image_set = False
+        self.features = None
+        self.orig_h = None
+        self.orig_w = None
+        self.input_h = None
+        self.input_w = None
```

### Comparing `npsam-1.4.5/npsam/segment_anything/utils/amg.py` & `npsam-1.4.6/npsam/segment_anything/utils/amg.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,346 +1,346 @@
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-# All rights reserved.
-
-# This source code is licensed under the license found in the
-# LICENSE file in the root directory of this source tree.
-
-import numpy as np
-import torch
-
-import math
-from copy import deepcopy
-from itertools import product
-from typing import Any, Dict, Generator, ItemsView, List, Tuple
-
-
-class MaskData:
-    """
-    A structure for storing masks and their related data in batched format.
-    Implements basic filtering and concatenation.
-    """
-
-    def __init__(self, **kwargs) -> None:
-        for v in kwargs.values():
-            assert isinstance(
-                v, (list, np.ndarray, torch.Tensor)
-            ), "MaskData only supports list, numpy arrays, and torch tensors."
-        self._stats = dict(**kwargs)
-
-    def __setitem__(self, key: str, item: Any) -> None:
-        assert isinstance(
-            item, (list, np.ndarray, torch.Tensor)
-        ), "MaskData only supports list, numpy arrays, and torch tensors."
-        self._stats[key] = item
-
-    def __delitem__(self, key: str) -> None:
-        del self._stats[key]
-
-    def __getitem__(self, key: str) -> Any:
-        return self._stats[key]
-
-    def items(self) -> ItemsView[str, Any]:
-        return self._stats.items()
-
-    def filter(self, keep: torch.Tensor) -> None:
-        for k, v in self._stats.items():
-            if v is None:
-                self._stats[k] = None
-            elif isinstance(v, torch.Tensor):
-                self._stats[k] = v[torch.as_tensor(keep, device=v.device)]
-            elif isinstance(v, np.ndarray):
-                self._stats[k] = v[keep.detach().cpu().numpy()]
-            elif isinstance(v, list) and keep.dtype == torch.bool:
-                self._stats[k] = [a for i, a in enumerate(v) if keep[i]]
-            elif isinstance(v, list):
-                self._stats[k] = [v[i] for i in keep]
-            else:
-                raise TypeError(f"MaskData key {k} has an unsupported type {type(v)}.")
-
-    def cat(self, new_stats: "MaskData") -> None:
-        for k, v in new_stats.items():
-            if k not in self._stats or self._stats[k] is None:
-                self._stats[k] = deepcopy(v)
-            elif isinstance(v, torch.Tensor):
-                self._stats[k] = torch.cat([self._stats[k], v], dim=0)
-            elif isinstance(v, np.ndarray):
-                self._stats[k] = np.concatenate([self._stats[k], v], axis=0)
-            elif isinstance(v, list):
-                self._stats[k] = self._stats[k] + deepcopy(v)
-            else:
-                raise TypeError(f"MaskData key {k} has an unsupported type {type(v)}.")
-
-    def to_numpy(self) -> None:
-        for k, v in self._stats.items():
-            if isinstance(v, torch.Tensor):
-                self._stats[k] = v.detach().cpu().numpy()
-
-
-def is_box_near_crop_edge(
-    boxes: torch.Tensor, crop_box: List[int], orig_box: List[int], atol: float = 20.0
-) -> torch.Tensor:
-    """Filter masks at the edge of a crop, but not at the edge of the original image."""
-    crop_box_torch = torch.as_tensor(crop_box, dtype=torch.float, device=boxes.device)
-    orig_box_torch = torch.as_tensor(orig_box, dtype=torch.float, device=boxes.device)
-    boxes = uncrop_boxes_xyxy(boxes, crop_box).float()
-    near_crop_edge = torch.isclose(boxes, crop_box_torch[None, :], atol=atol, rtol=0)
-    near_image_edge = torch.isclose(boxes, orig_box_torch[None, :], atol=atol, rtol=0)
-    near_crop_edge = torch.logical_and(near_crop_edge, ~near_image_edge)
-    return torch.any(near_crop_edge, dim=1)
-
-
-def box_xyxy_to_xywh(box_xyxy: torch.Tensor) -> torch.Tensor:
-    box_xywh = deepcopy(box_xyxy)
-    box_xywh[2] = box_xywh[2] - box_xywh[0]
-    box_xywh[3] = box_xywh[3] - box_xywh[1]
-    return box_xywh
-
-
-def batch_iterator(batch_size: int, *args) -> Generator[List[Any], None, None]:
-    assert len(args) > 0 and all(
-        len(a) == len(args[0]) for a in args
-    ), "Batched iteration must have inputs of all the same size."
-    n_batches = len(args[0]) // batch_size + int(len(args[0]) % batch_size != 0)
-    for b in range(n_batches):
-        yield [arg[b * batch_size : (b + 1) * batch_size] for arg in args]
-
-
-def mask_to_rle_pytorch(tensor: torch.Tensor) -> List[Dict[str, Any]]:
-    """
-    Encodes masks to an uncompressed RLE, in the format expected by
-    pycoco tools.
-    """
-    # Put in fortran order and flatten h,w
-    b, h, w = tensor.shape
-    tensor = tensor.permute(0, 2, 1).flatten(1)
-
-    # Compute change indices
-    diff = tensor[:, 1:] ^ tensor[:, :-1]
-    change_indices = diff.nonzero()
-
-    # Encode run length
-    out = []
-    for i in range(b):
-        cur_idxs = change_indices[change_indices[:, 0] == i, 1]
-        cur_idxs = torch.cat(
-            [
-                torch.tensor([0], dtype=cur_idxs.dtype, device=cur_idxs.device),
-                cur_idxs + 1,
-                torch.tensor([h * w], dtype=cur_idxs.dtype, device=cur_idxs.device),
-            ]
-        )
-        btw_idxs = cur_idxs[1:] - cur_idxs[:-1]
-        counts = [] if tensor[i, 0] == 0 else [0]
-        counts.extend(btw_idxs.detach().cpu().tolist())
-        out.append({"size": [h, w], "counts": counts})
-    return out
-
-
-def rle_to_mask(rle: Dict[str, Any]) -> np.ndarray:
-    """Compute a binary mask from an uncompressed RLE."""
-    h, w = rle["size"]
-    mask = np.empty(h * w, dtype=bool)
-    idx = 0
-    parity = False
-    for count in rle["counts"]:
-        mask[idx : idx + count] = parity
-        idx += count
-        parity ^= True
-    mask = mask.reshape(w, h)
-    return mask.transpose()  # Put in C order
-
-
-def area_from_rle(rle: Dict[str, Any]) -> int:
-    return sum(rle["counts"][1::2])
-
-
-def calculate_stability_score(
-    masks: torch.Tensor, mask_threshold: float, threshold_offset: float
-) -> torch.Tensor:
-    """
-    Computes the stability score for a batch of masks. The stability
-    score is the IoU between the binary masks obtained by thresholding
-    the predicted mask logits at high and low values.
-    """
-    # One mask is always contained inside the other.
-    # Save memory by preventing unnecessary cast to torch.int64
-    intersections = (
-        (masks > (mask_threshold + threshold_offset))
-        .sum(-1, dtype=torch.int16)
-        .sum(-1, dtype=torch.int32)
-    )
-    unions = (
-        (masks > (mask_threshold - threshold_offset))
-        .sum(-1, dtype=torch.int16)
-        .sum(-1, dtype=torch.int32)
-    )
-    return intersections / unions
-
-
-def build_point_grid(n_per_side: int) -> np.ndarray:
-    """Generates a 2D grid of points evenly spaced in [0,1]x[0,1]."""
-    offset = 1 / (2 * n_per_side)
-    points_one_side = np.linspace(offset, 1 - offset, n_per_side)
-    points_x = np.tile(points_one_side[None, :], (n_per_side, 1))
-    points_y = np.tile(points_one_side[:, None], (1, n_per_side))
-    points = np.stack([points_x, points_y], axis=-1).reshape(-1, 2)
-    return points
-
-
-def build_all_layer_point_grids(
-    n_per_side: int, n_layers: int, scale_per_layer: int
-) -> List[np.ndarray]:
-    """Generates point grids for all crop layers."""
-    points_by_layer = []
-    for i in range(n_layers + 1):
-        n_points = int(n_per_side / (scale_per_layer**i))
-        points_by_layer.append(build_point_grid(n_points))
-    return points_by_layer
-
-
-def generate_crop_boxes(
-    im_size: Tuple[int, ...], n_layers: int, overlap_ratio: float
-) -> Tuple[List[List[int]], List[int]]:
-    """
-    Generates a list of crop boxes of different sizes. Each layer
-    has (2**i)**2 boxes for the ith layer.
-    """
-    crop_boxes, layer_idxs = [], []
-    im_h, im_w = im_size
-    short_side = min(im_h, im_w)
-
-    # Original image
-    crop_boxes.append([0, 0, im_w, im_h])
-    layer_idxs.append(0)
-
-    def crop_len(orig_len, n_crops, overlap):
-        return int(math.ceil((overlap * (n_crops - 1) + orig_len) / n_crops))
-
-    for i_layer in range(n_layers):
-        n_crops_per_side = 2 ** (i_layer + 1)
-        overlap = int(overlap_ratio * short_side * (2 / n_crops_per_side))
-
-        crop_w = crop_len(im_w, n_crops_per_side, overlap)
-        crop_h = crop_len(im_h, n_crops_per_side, overlap)
-
-        crop_box_x0 = [int((crop_w - overlap) * i) for i in range(n_crops_per_side)]
-        crop_box_y0 = [int((crop_h - overlap) * i) for i in range(n_crops_per_side)]
-
-        # Crops in XYWH format
-        for x0, y0 in product(crop_box_x0, crop_box_y0):
-            box = [x0, y0, min(x0 + crop_w, im_w), min(y0 + crop_h, im_h)]
-            crop_boxes.append(box)
-            layer_idxs.append(i_layer + 1)
-
-    return crop_boxes, layer_idxs
-
-
-def uncrop_boxes_xyxy(boxes: torch.Tensor, crop_box: List[int]) -> torch.Tensor:
-    x0, y0, _, _ = crop_box
-    offset = torch.tensor([[x0, y0, x0, y0]], device=boxes.device)
-    # Check if boxes has a channel dimension
-    if len(boxes.shape) == 3:
-        offset = offset.unsqueeze(1)
-    return boxes + offset
-
-
-def uncrop_points(points: torch.Tensor, crop_box: List[int]) -> torch.Tensor:
-    x0, y0, _, _ = crop_box
-    offset = torch.tensor([[x0, y0]], device=points.device)
-    # Check if points has a channel dimension
-    if len(points.shape) == 3:
-        offset = offset.unsqueeze(1)
-    return points + offset
-
-
-def uncrop_masks(
-    masks: torch.Tensor, crop_box: List[int], orig_h: int, orig_w: int
-) -> torch.Tensor:
-    x0, y0, x1, y1 = crop_box
-    if x0 == 0 and y0 == 0 and x1 == orig_w and y1 == orig_h:
-        return masks
-    # Coordinate transform masks
-    pad_x, pad_y = orig_w - (x1 - x0), orig_h - (y1 - y0)
-    pad = (x0, pad_x - x0, y0, pad_y - y0)
-    return torch.nn.functional.pad(masks, pad, value=0)
-
-
-def remove_small_regions(
-    mask: np.ndarray, area_thresh: float, mode: str
-) -> Tuple[np.ndarray, bool]:
-    """
-    Removes small disconnected regions and holes in a mask. Returns the
-    mask and an indicator of if the mask has been modified.
-    """
-    import cv2  # type: ignore
-
-    assert mode in ["holes", "islands"]
-    correct_holes = mode == "holes"
-    working_mask = (correct_holes ^ mask).astype(np.uint8)
-    n_labels, regions, stats, _ = cv2.connectedComponentsWithStats(working_mask, 8)
-    sizes = stats[:, -1][1:]  # Row 0 is background label
-    small_regions = [i + 1 for i, s in enumerate(sizes) if s < area_thresh]
-    if len(small_regions) == 0:
-        return mask, False
-    fill_labels = [0] + small_regions
-    if not correct_holes:
-        fill_labels = [i for i in range(n_labels) if i not in fill_labels]
-        # If every region is below threshold, keep largest
-        if len(fill_labels) == 0:
-            fill_labels = [int(np.argmax(sizes)) + 1]
-    mask = np.isin(regions, fill_labels)
-    return mask, True
-
-
-def coco_encode_rle(uncompressed_rle: Dict[str, Any]) -> Dict[str, Any]:
-    from pycocotools import mask as mask_utils  # type: ignore
-
-    h, w = uncompressed_rle["size"]
-    rle = mask_utils.frPyObjects(uncompressed_rle, h, w)
-    rle["counts"] = rle["counts"].decode("utf-8")  # Necessary to serialize with json
-    return rle
-
-
-def batched_mask_to_box(masks: torch.Tensor) -> torch.Tensor:
-    """
-    Calculates boxes in XYXY format around masks. Return [0,0,0,0] for
-    an empty mask. For input shape C1xC2x...xHxW, the output shape is C1xC2x...x4.
-    """
-    # torch.max below raises an error on empty inputs, just skip in this case
-    if torch.numel(masks) == 0:
-        return torch.zeros(*masks.shape[:-2], 4, device=masks.device)
-
-    # Normalize shape to CxHxW
-    shape = masks.shape
-    h, w = shape[-2:]
-    if len(shape) > 2:
-        masks = masks.flatten(0, -3)
-    else:
-        masks = masks.unsqueeze(0)
-
-    # Get top and bottom edges
-    in_height, _ = torch.max(masks, dim=-1)
-    in_height_coords = in_height * torch.arange(h, device=in_height.device)[None, :]
-    bottom_edges, _ = torch.max(in_height_coords, dim=-1)
-    in_height_coords = in_height_coords + h * (~in_height)
-    top_edges, _ = torch.min(in_height_coords, dim=-1)
-
-    # Get left and right edges
-    in_width, _ = torch.max(masks, dim=-2)
-    in_width_coords = in_width * torch.arange(w, device=in_width.device)[None, :]
-    right_edges, _ = torch.max(in_width_coords, dim=-1)
-    in_width_coords = in_width_coords + w * (~in_width)
-    left_edges, _ = torch.min(in_width_coords, dim=-1)
-
-    # If the mask is empty the right edge will be to the left of the left edge.
-    # Replace these boxes with [0, 0, 0, 0]
-    empty_filter = (right_edges < left_edges) | (bottom_edges < top_edges)
-    out = torch.stack([left_edges, top_edges, right_edges, bottom_edges], dim=-1)
-    out = out * (~empty_filter).unsqueeze(-1)
-
-    # Return to original shape
-    if len(shape) > 2:
-        out = out.reshape(*shape[:-2], 4)
-    else:
-        out = out[0]
-
-    return out
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
+import numpy as np
+import torch
+
+import math
+from copy import deepcopy
+from itertools import product
+from typing import Any, Dict, Generator, ItemsView, List, Tuple
+
+
+class MaskData:
+    """
+    A structure for storing masks and their related data in batched format.
+    Implements basic filtering and concatenation.
+    """
+
+    def __init__(self, **kwargs) -> None:
+        for v in kwargs.values():
+            assert isinstance(
+                v, (list, np.ndarray, torch.Tensor)
+            ), "MaskData only supports list, numpy arrays, and torch tensors."
+        self._stats = dict(**kwargs)
+
+    def __setitem__(self, key: str, item: Any) -> None:
+        assert isinstance(
+            item, (list, np.ndarray, torch.Tensor)
+        ), "MaskData only supports list, numpy arrays, and torch tensors."
+        self._stats[key] = item
+
+    def __delitem__(self, key: str) -> None:
+        del self._stats[key]
+
+    def __getitem__(self, key: str) -> Any:
+        return self._stats[key]
+
+    def items(self) -> ItemsView[str, Any]:
+        return self._stats.items()
+
+    def filter(self, keep: torch.Tensor) -> None:
+        for k, v in self._stats.items():
+            if v is None:
+                self._stats[k] = None
+            elif isinstance(v, torch.Tensor):
+                self._stats[k] = v[torch.as_tensor(keep, device=v.device)]
+            elif isinstance(v, np.ndarray):
+                self._stats[k] = v[keep.detach().cpu().numpy()]
+            elif isinstance(v, list) and keep.dtype == torch.bool:
+                self._stats[k] = [a for i, a in enumerate(v) if keep[i]]
+            elif isinstance(v, list):
+                self._stats[k] = [v[i] for i in keep]
+            else:
+                raise TypeError(f"MaskData key {k} has an unsupported type {type(v)}.")
+
+    def cat(self, new_stats: "MaskData") -> None:
+        for k, v in new_stats.items():
+            if k not in self._stats or self._stats[k] is None:
+                self._stats[k] = deepcopy(v)
+            elif isinstance(v, torch.Tensor):
+                self._stats[k] = torch.cat([self._stats[k], v], dim=0)
+            elif isinstance(v, np.ndarray):
+                self._stats[k] = np.concatenate([self._stats[k], v], axis=0)
+            elif isinstance(v, list):
+                self._stats[k] = self._stats[k] + deepcopy(v)
+            else:
+                raise TypeError(f"MaskData key {k} has an unsupported type {type(v)}.")
+
+    def to_numpy(self) -> None:
+        for k, v in self._stats.items():
+            if isinstance(v, torch.Tensor):
+                self._stats[k] = v.detach().cpu().numpy()
+
+
+def is_box_near_crop_edge(
+    boxes: torch.Tensor, crop_box: List[int], orig_box: List[int], atol: float = 20.0
+) -> torch.Tensor:
+    """Filter masks at the edge of a crop, but not at the edge of the original image."""
+    crop_box_torch = torch.as_tensor(crop_box, dtype=torch.float, device=boxes.device)
+    orig_box_torch = torch.as_tensor(orig_box, dtype=torch.float, device=boxes.device)
+    boxes = uncrop_boxes_xyxy(boxes, crop_box).float()
+    near_crop_edge = torch.isclose(boxes, crop_box_torch[None, :], atol=atol, rtol=0)
+    near_image_edge = torch.isclose(boxes, orig_box_torch[None, :], atol=atol, rtol=0)
+    near_crop_edge = torch.logical_and(near_crop_edge, ~near_image_edge)
+    return torch.any(near_crop_edge, dim=1)
+
+
+def box_xyxy_to_xywh(box_xyxy: torch.Tensor) -> torch.Tensor:
+    box_xywh = deepcopy(box_xyxy)
+    box_xywh[2] = box_xywh[2] - box_xywh[0]
+    box_xywh[3] = box_xywh[3] - box_xywh[1]
+    return box_xywh
+
+
+def batch_iterator(batch_size: int, *args) -> Generator[List[Any], None, None]:
+    assert len(args) > 0 and all(
+        len(a) == len(args[0]) for a in args
+    ), "Batched iteration must have inputs of all the same size."
+    n_batches = len(args[0]) // batch_size + int(len(args[0]) % batch_size != 0)
+    for b in range(n_batches):
+        yield [arg[b * batch_size : (b + 1) * batch_size] for arg in args]
+
+
+def mask_to_rle_pytorch(tensor: torch.Tensor) -> List[Dict[str, Any]]:
+    """
+    Encodes masks to an uncompressed RLE, in the format expected by
+    pycoco tools.
+    """
+    # Put in fortran order and flatten h,w
+    b, h, w = tensor.shape
+    tensor = tensor.permute(0, 2, 1).flatten(1)
+
+    # Compute change indices
+    diff = tensor[:, 1:] ^ tensor[:, :-1]
+    change_indices = diff.nonzero()
+
+    # Encode run length
+    out = []
+    for i in range(b):
+        cur_idxs = change_indices[change_indices[:, 0] == i, 1]
+        cur_idxs = torch.cat(
+            [
+                torch.tensor([0], dtype=cur_idxs.dtype, device=cur_idxs.device),
+                cur_idxs + 1,
+                torch.tensor([h * w], dtype=cur_idxs.dtype, device=cur_idxs.device),
+            ]
+        )
+        btw_idxs = cur_idxs[1:] - cur_idxs[:-1]
+        counts = [] if tensor[i, 0] == 0 else [0]
+        counts.extend(btw_idxs.detach().cpu().tolist())
+        out.append({"size": [h, w], "counts": counts})
+    return out
+
+
+def rle_to_mask(rle: Dict[str, Any]) -> np.ndarray:
+    """Compute a binary mask from an uncompressed RLE."""
+    h, w = rle["size"]
+    mask = np.empty(h * w, dtype=bool)
+    idx = 0
+    parity = False
+    for count in rle["counts"]:
+        mask[idx : idx + count] = parity
+        idx += count
+        parity ^= True
+    mask = mask.reshape(w, h)
+    return mask.transpose()  # Put in C order
+
+
+def area_from_rle(rle: Dict[str, Any]) -> int:
+    return sum(rle["counts"][1::2])
+
+
+def calculate_stability_score(
+    masks: torch.Tensor, mask_threshold: float, threshold_offset: float
+) -> torch.Tensor:
+    """
+    Computes the stability score for a batch of masks. The stability
+    score is the IoU between the binary masks obtained by thresholding
+    the predicted mask logits at high and low values.
+    """
+    # One mask is always contained inside the other.
+    # Save memory by preventing unnecessary cast to torch.int64
+    intersections = (
+        (masks > (mask_threshold + threshold_offset))
+        .sum(-1, dtype=torch.int16)
+        .sum(-1, dtype=torch.int32)
+    )
+    unions = (
+        (masks > (mask_threshold - threshold_offset))
+        .sum(-1, dtype=torch.int16)
+        .sum(-1, dtype=torch.int32)
+    )
+    return intersections / unions
+
+
+def build_point_grid(n_per_side: int) -> np.ndarray:
+    """Generates a 2D grid of points evenly spaced in [0,1]x[0,1]."""
+    offset = 1 / (2 * n_per_side)
+    points_one_side = np.linspace(offset, 1 - offset, n_per_side)
+    points_x = np.tile(points_one_side[None, :], (n_per_side, 1))
+    points_y = np.tile(points_one_side[:, None], (1, n_per_side))
+    points = np.stack([points_x, points_y], axis=-1).reshape(-1, 2)
+    return points
+
+
+def build_all_layer_point_grids(
+    n_per_side: int, n_layers: int, scale_per_layer: int
+) -> List[np.ndarray]:
+    """Generates point grids for all crop layers."""
+    points_by_layer = []
+    for i in range(n_layers + 1):
+        n_points = int(n_per_side / (scale_per_layer**i))
+        points_by_layer.append(build_point_grid(n_points))
+    return points_by_layer
+
+
+def generate_crop_boxes(
+    im_size: Tuple[int, ...], n_layers: int, overlap_ratio: float
+) -> Tuple[List[List[int]], List[int]]:
+    """
+    Generates a list of crop boxes of different sizes. Each layer
+    has (2**i)**2 boxes for the ith layer.
+    """
+    crop_boxes, layer_idxs = [], []
+    im_h, im_w = im_size
+    short_side = min(im_h, im_w)
+
+    # Original image
+    crop_boxes.append([0, 0, im_w, im_h])
+    layer_idxs.append(0)
+
+    def crop_len(orig_len, n_crops, overlap):
+        return int(math.ceil((overlap * (n_crops - 1) + orig_len) / n_crops))
+
+    for i_layer in range(n_layers):
+        n_crops_per_side = 2 ** (i_layer + 1)
+        overlap = int(overlap_ratio * short_side * (2 / n_crops_per_side))
+
+        crop_w = crop_len(im_w, n_crops_per_side, overlap)
+        crop_h = crop_len(im_h, n_crops_per_side, overlap)
+
+        crop_box_x0 = [int((crop_w - overlap) * i) for i in range(n_crops_per_side)]
+        crop_box_y0 = [int((crop_h - overlap) * i) for i in range(n_crops_per_side)]
+
+        # Crops in XYWH format
+        for x0, y0 in product(crop_box_x0, crop_box_y0):
+            box = [x0, y0, min(x0 + crop_w, im_w), min(y0 + crop_h, im_h)]
+            crop_boxes.append(box)
+            layer_idxs.append(i_layer + 1)
+
+    return crop_boxes, layer_idxs
+
+
+def uncrop_boxes_xyxy(boxes: torch.Tensor, crop_box: List[int]) -> torch.Tensor:
+    x0, y0, _, _ = crop_box
+    offset = torch.tensor([[x0, y0, x0, y0]], device=boxes.device)
+    # Check if boxes has a channel dimension
+    if len(boxes.shape) == 3:
+        offset = offset.unsqueeze(1)
+    return boxes + offset
+
+
+def uncrop_points(points: torch.Tensor, crop_box: List[int]) -> torch.Tensor:
+    x0, y0, _, _ = crop_box
+    offset = torch.tensor([[x0, y0]], device=points.device)
+    # Check if points has a channel dimension
+    if len(points.shape) == 3:
+        offset = offset.unsqueeze(1)
+    return points + offset
+
+
+def uncrop_masks(
+    masks: torch.Tensor, crop_box: List[int], orig_h: int, orig_w: int
+) -> torch.Tensor:
+    x0, y0, x1, y1 = crop_box
+    if x0 == 0 and y0 == 0 and x1 == orig_w and y1 == orig_h:
+        return masks
+    # Coordinate transform masks
+    pad_x, pad_y = orig_w - (x1 - x0), orig_h - (y1 - y0)
+    pad = (x0, pad_x - x0, y0, pad_y - y0)
+    return torch.nn.functional.pad(masks, pad, value=0)
+
+
+def remove_small_regions(
+    mask: np.ndarray, area_thresh: float, mode: str
+) -> Tuple[np.ndarray, bool]:
+    """
+    Removes small disconnected regions and holes in a mask. Returns the
+    mask and an indicator of if the mask has been modified.
+    """
+    import cv2  # type: ignore
+
+    assert mode in ["holes", "islands"]
+    correct_holes = mode == "holes"
+    working_mask = (correct_holes ^ mask).astype(np.uint8)
+    n_labels, regions, stats, _ = cv2.connectedComponentsWithStats(working_mask, 8)
+    sizes = stats[:, -1][1:]  # Row 0 is background label
+    small_regions = [i + 1 for i, s in enumerate(sizes) if s < area_thresh]
+    if len(small_regions) == 0:
+        return mask, False
+    fill_labels = [0] + small_regions
+    if not correct_holes:
+        fill_labels = [i for i in range(n_labels) if i not in fill_labels]
+        # If every region is below threshold, keep largest
+        if len(fill_labels) == 0:
+            fill_labels = [int(np.argmax(sizes)) + 1]
+    mask = np.isin(regions, fill_labels)
+    return mask, True
+
+
+def coco_encode_rle(uncompressed_rle: Dict[str, Any]) -> Dict[str, Any]:
+    from pycocotools import mask as mask_utils  # type: ignore
+
+    h, w = uncompressed_rle["size"]
+    rle = mask_utils.frPyObjects(uncompressed_rle, h, w)
+    rle["counts"] = rle["counts"].decode("utf-8")  # Necessary to serialize with json
+    return rle
+
+
+def batched_mask_to_box(masks: torch.Tensor) -> torch.Tensor:
+    """
+    Calculates boxes in XYXY format around masks. Return [0,0,0,0] for
+    an empty mask. For input shape C1xC2x...xHxW, the output shape is C1xC2x...x4.
+    """
+    # torch.max below raises an error on empty inputs, just skip in this case
+    if torch.numel(masks) == 0:
+        return torch.zeros(*masks.shape[:-2], 4, device=masks.device)
+
+    # Normalize shape to CxHxW
+    shape = masks.shape
+    h, w = shape[-2:]
+    if len(shape) > 2:
+        masks = masks.flatten(0, -3)
+    else:
+        masks = masks.unsqueeze(0)
+
+    # Get top and bottom edges
+    in_height, _ = torch.max(masks, dim=-1)
+    in_height_coords = in_height * torch.arange(h, device=in_height.device)[None, :]
+    bottom_edges, _ = torch.max(in_height_coords, dim=-1)
+    in_height_coords = in_height_coords + h * (~in_height)
+    top_edges, _ = torch.min(in_height_coords, dim=-1)
+
+    # Get left and right edges
+    in_width, _ = torch.max(masks, dim=-2)
+    in_width_coords = in_width * torch.arange(w, device=in_width.device)[None, :]
+    right_edges, _ = torch.max(in_width_coords, dim=-1)
+    in_width_coords = in_width_coords + w * (~in_width)
+    left_edges, _ = torch.min(in_width_coords, dim=-1)
+
+    # If the mask is empty the right edge will be to the left of the left edge.
+    # Replace these boxes with [0, 0, 0, 0]
+    empty_filter = (right_edges < left_edges) | (bottom_edges < top_edges)
+    out = torch.stack([left_edges, top_edges, right_edges, bottom_edges], dim=-1)
+    out = out * (~empty_filter).unsqueeze(-1)
+
+    # Return to original shape
+    if len(shape) > 2:
+        out = out.reshape(*shape[:-2], 4)
+    else:
+        out = out[0]
+
+    return out
```

### Comparing `npsam-1.4.5/npsam/segment_anything/utils/transforms.py` & `npsam-1.4.6/npsam/segment_anything/utils/transforms.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-# All rights reserved.
-
-# This source code is licensed under the license found in the
-# LICENSE file in the root directory of this source tree.
-
-import numpy as np
-import torch
-from torch.nn import functional as F
-from torchvision.transforms.functional import resize, to_pil_image  # type: ignore
-
-from copy import deepcopy
-from typing import Tuple
-
-
-class ResizeLongestSide:
-    """
-    Resizes images to the longest side 'target_length', as well as provides
-    methods for resizing coordinates and boxes. Provides methods for
-    transforming both numpy array and batched torch tensors.
-    """
-
-    def __init__(self, target_length: int) -> None:
-        self.target_length = target_length
-
-    def apply_image(self, image: np.ndarray) -> np.ndarray:
-        """
-        Expects a numpy array with shape HxWxC in uint8 format.
-        """
-        target_size = self.get_preprocess_shape(image.shape[0], image.shape[1], self.target_length)
-        return np.array(resize(to_pil_image(image), target_size))
-
-    def apply_coords(self, coords: np.ndarray, original_size: Tuple[int, ...]) -> np.ndarray:
-        """
-        Expects a numpy array of length 2 in the final dimension. Requires the
-        original image size in (H, W) format.
-        """
-        old_h, old_w = original_size
-        new_h, new_w = self.get_preprocess_shape(
-            original_size[0], original_size[1], self.target_length
-        )
-        coords = deepcopy(coords).astype(float)
-        coords[..., 0] = coords[..., 0] * (new_w / old_w)
-        coords[..., 1] = coords[..., 1] * (new_h / old_h)
-        return coords
-
-    def apply_boxes(self, boxes: np.ndarray, original_size: Tuple[int, ...]) -> np.ndarray:
-        """
-        Expects a numpy array shape Bx4. Requires the original image size
-        in (H, W) format.
-        """
-        boxes = self.apply_coords(boxes.reshape(-1, 2, 2), original_size)
-        return boxes.reshape(-1, 4)
-
-    def apply_image_torch(self, image: torch.Tensor) -> torch.Tensor:
-        """
-        Expects batched images with shape BxCxHxW and float format. This
-        transformation may not exactly match apply_image. apply_image is
-        the transformation expected by the model.
-        """
-        # Expects an image in BCHW format. May not exactly match apply_image.
-        target_size = self.get_preprocess_shape(image.shape[2], image.shape[3], self.target_length)
-        return F.interpolate(
-            image, target_size, mode="bilinear", align_corners=False, antialias=True
-        )
-
-    def apply_coords_torch(
-        self, coords: torch.Tensor, original_size: Tuple[int, ...]
-    ) -> torch.Tensor:
-        """
-        Expects a torch tensor with length 2 in the last dimension. Requires the
-        original image size in (H, W) format.
-        """
-        old_h, old_w = original_size
-        new_h, new_w = self.get_preprocess_shape(
-            original_size[0], original_size[1], self.target_length
-        )
-        coords = deepcopy(coords).to(torch.float)
-        coords[..., 0] = coords[..., 0] * (new_w / old_w)
-        coords[..., 1] = coords[..., 1] * (new_h / old_h)
-        return coords
-
-    def apply_boxes_torch(
-        self, boxes: torch.Tensor, original_size: Tuple[int, ...]
-    ) -> torch.Tensor:
-        """
-        Expects a torch tensor with shape Bx4. Requires the original image
-        size in (H, W) format.
-        """
-        boxes = self.apply_coords_torch(boxes.reshape(-1, 2, 2), original_size)
-        return boxes.reshape(-1, 4)
-
-    @staticmethod
-    def get_preprocess_shape(oldh: int, oldw: int, long_side_length: int) -> Tuple[int, int]:
-        """
-        Compute the output size given input size and target long side length.
-        """
-        scale = long_side_length * 1.0 / max(oldh, oldw)
-        newh, neww = oldh * scale, oldw * scale
-        neww = int(neww + 0.5)
-        newh = int(newh + 0.5)
-        return (newh, neww)
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
+import numpy as np
+import torch
+from torch.nn import functional as F
+from torchvision.transforms.functional import resize, to_pil_image  # type: ignore
+
+from copy import deepcopy
+from typing import Tuple
+
+
+class ResizeLongestSide:
+    """
+    Resizes images to the longest side 'target_length', as well as provides
+    methods for resizing coordinates and boxes. Provides methods for
+    transforming both numpy array and batched torch tensors.
+    """
+
+    def __init__(self, target_length: int) -> None:
+        self.target_length = target_length
+
+    def apply_image(self, image: np.ndarray) -> np.ndarray:
+        """
+        Expects a numpy array with shape HxWxC in uint8 format.
+        """
+        target_size = self.get_preprocess_shape(image.shape[0], image.shape[1], self.target_length)
+        return np.array(resize(to_pil_image(image), target_size))
+
+    def apply_coords(self, coords: np.ndarray, original_size: Tuple[int, ...]) -> np.ndarray:
+        """
+        Expects a numpy array of length 2 in the final dimension. Requires the
+        original image size in (H, W) format.
+        """
+        old_h, old_w = original_size
+        new_h, new_w = self.get_preprocess_shape(
+            original_size[0], original_size[1], self.target_length
+        )
+        coords = deepcopy(coords).astype(float)
+        coords[..., 0] = coords[..., 0] * (new_w / old_w)
+        coords[..., 1] = coords[..., 1] * (new_h / old_h)
+        return coords
+
+    def apply_boxes(self, boxes: np.ndarray, original_size: Tuple[int, ...]) -> np.ndarray:
+        """
+        Expects a numpy array shape Bx4. Requires the original image size
+        in (H, W) format.
+        """
+        boxes = self.apply_coords(boxes.reshape(-1, 2, 2), original_size)
+        return boxes.reshape(-1, 4)
+
+    def apply_image_torch(self, image: torch.Tensor) -> torch.Tensor:
+        """
+        Expects batched images with shape BxCxHxW and float format. This
+        transformation may not exactly match apply_image. apply_image is
+        the transformation expected by the model.
+        """
+        # Expects an image in BCHW format. May not exactly match apply_image.
+        target_size = self.get_preprocess_shape(image.shape[2], image.shape[3], self.target_length)
+        return F.interpolate(
+            image, target_size, mode="bilinear", align_corners=False, antialias=True
+        )
+
+    def apply_coords_torch(
+        self, coords: torch.Tensor, original_size: Tuple[int, ...]
+    ) -> torch.Tensor:
+        """
+        Expects a torch tensor with length 2 in the last dimension. Requires the
+        original image size in (H, W) format.
+        """
+        old_h, old_w = original_size
+        new_h, new_w = self.get_preprocess_shape(
+            original_size[0], original_size[1], self.target_length
+        )
+        coords = deepcopy(coords).to(torch.float)
+        coords[..., 0] = coords[..., 0] * (new_w / old_w)
+        coords[..., 1] = coords[..., 1] * (new_h / old_h)
+        return coords
+
+    def apply_boxes_torch(
+        self, boxes: torch.Tensor, original_size: Tuple[int, ...]
+    ) -> torch.Tensor:
+        """
+        Expects a torch tensor with shape Bx4. Requires the original image
+        size in (H, W) format.
+        """
+        boxes = self.apply_coords_torch(boxes.reshape(-1, 2, 2), original_size)
+        return boxes.reshape(-1, 4)
+
+    @staticmethod
+    def get_preprocess_shape(oldh: int, oldw: int, long_side_length: int) -> Tuple[int, int]:
+        """
+        Compute the output size given input size and target long side length.
+        """
+        scale = long_side_length * 1.0 / max(oldh, oldw)
+        newh, neww = oldh * scale, oldw * scale
+        neww = int(neww + 0.5)
+        newh = int(newh + 0.5)
+        return (newh, neww)
```

### Comparing `npsam-1.4.5/npsam/utils.py` & `npsam-1.4.6/npsam/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Standard library imports
-import os, sys, requests, ast 
+import os, sys, requests, ast
 from pathlib import Path
 from time import time
 
 # Third-party imports
 import cv2
 import matplotlib
 import matplotlib.image as mpimg
@@ -19,15 +19,14 @@
 from tqdm import tqdm
 from numba.extending import overload, register_jitable
 from skimage.measure import regionprops
 from PIL import Image
 from PIL.PngImagePlugin import PngInfo
 
 
-
 def save_dictionary(filepath, new_data):
     filepath = Path(filepath).absolute()
     try:
         existing_metadata = load_dictionary(filepath)
     except KeyError:
         existing_metadata = {}
 
@@ -108,15 +107,14 @@
         for i in range(n, len(axes)):
             axes[i].axis('off')
 
     plt.tight_layout()
     plt.show()
 
 
-
 def process_filepath(filepath):
     if type(filepath) == str:
         filepath = Path(filepath).absolute()
 
         if filepath.is_file():
             if filepath.suffix in {'.png', '.jpg', '.jpeg', '.tif', '.tiff'}:
                 list_of_images = [filepath.as_posix()]
@@ -129,35 +127,45 @@
                               if filename.suffix in {'.png', '.jpg', '.jpeg', '.tif', '.tiff'}]
         else:
             print('Error: The string did not contain a path to a folder or an image.')
 
     elif type(filepath) == list:
         for filename in filepath:
             if not Path(filename).is_file():
-                print(f'Error: Not all list entries are valid filenames. \nThe issue is: {Path(filename).as_posix()} \nINFO: Folder paths should be given as a string, not a list.')
+                print(
+                    f'Error: Not all list entries are valid filenames. \nThe issue is: {Path(filename).as_posix()} \nINFO: Folder paths should be given as a string, not a list.')
                 return None
         list_of_images = [Path(filename).absolute().as_posix() for filename in filepath
                           if Path(filename).suffix in {'.png', '.jpg', '.jpeg', '.tif', '.tiff'}]
     else:
         print('Unexpected error')
         return None
 
     return list_of_images
 
 
 def load_image(filepath):
     if Path(filepath).suffix in {'.tif', '.tiff'}:
-        im = tifffile.imread(filepath)
+        try:
+            im = tifffile.imread(filepath)
+        except ValueError:
+            im = cv2.imread(filepath, cv2.IMREAD_UNCHANGED)
+
+        if im.ndim == 3 and im.shape[-1] in {3, 4}:
+            im = im[:, :, 0]
+        elif im.ndim == 3:
+            im = np.mean(im, axis=-1)
+
         im_shift_to_zero = im - im.min()
         im_max = im_shift_to_zero.max()
         im_normalized = im_shift_to_zero / im_max
         im_max_255 = im_normalized * 255
         im_8bit = im_max_255.astype('uint8')
         im_RGB = np.dstack([im_8bit] * 3)
-    elif Path(filepath).suffix in {'.png', '.jpg', '.jpeg',}:
+    elif Path(filepath).suffix in {'.png', '.jpg', '.jpeg', }:
         im = cv2.imread(filepath)
         im_RGB = cv2.cvtColor(im, cv2.COLOR_BGR2RGB)
     return im_RGB
 
 
 def make_randomized_cmap(cmap='viridis', seed=42):
     '''Genarates randomized colormap with the first color being black'''
@@ -185,15 +193,16 @@
     if crop_and_enlarge:
         imshapex = image.shape[0]
         imshapey = image.shape[1]
 
         crop1 = np.kron(image[:int((imshapex / 2) * 1.25), : int((imshapey / 2) * 1.25), :], np.ones((2, 2, 1)))
         crop2 = np.kron(image[math.ceil((imshapex / 2) * 0.75):, :int((imshapey / 2) * 1.25), :], np.ones((2, 2, 1)))
         crop3 = np.kron(image[:int((imshapex / 2) * 1.25), math.ceil((imshapey / 2) * 0.75):, :], np.ones((2, 2, 1)))
-        crop4 = np.kron(image[math.ceil((imshapex / 2) * 0.75):, math.ceil((imshapey / 2) * 0.75):, :], np.ones((2, 2, 1)))
+        crop4 = np.kron(image[math.ceil((imshapex / 2) * 0.75):, math.ceil((imshapey / 2) * 0.75):, :],
+                        np.ones((2, 2, 1)))
         images = [crop1, crop2, crop3, crop4]
         filenames = [filename + '_crop' + str(number) + '.png' for number in [1, 2, 3, 4]]
         if invert:
             image_ = cv2.bitwise_not(image)
             filename_ = filename + '_inverted.png'
             cv2.imwrite((files_folder / filename_).as_posix(), image_)
     else:
@@ -262,15 +271,14 @@
         np.savez_compressed(file_p, array=array_of_masks)
 
         array_of_bbox = np.array(list_of_bbox2)
         file_p = files_folder / (Path(image_filepath).stem + '_array_of_bbox.npz')
         np.savez_compressed(file_p, array=array_of_bbox)
 
 
-
 def bb_iou(boxA, boxB):
     xA = np.maximum(boxA[0], boxB[0])
     yA = np.maximum(boxA[1], boxB[1])
     xB = np.minimum(boxA[2], boxB[2])
     yB = np.minimum(boxA[3], boxB[3])
 
     interArea = np.maximum(0, xB - xA) * np.maximum(0, yB - yA)
@@ -305,15 +313,15 @@
         bboxes = np.load(files_folder / (Path(image_filepath).stem + '_array_of_bbox.npz'))['array']
         all_bboxes.append(bboxes)
         array_of_masks = np.load(files_folder / (Path(image_filepath).stem + '_array_of_masks_rearranged.npz'))['array']
         for mask in np.moveaxis(array_of_masks, -1, 0):
             all_masks.append(mask)
         os.remove(files_folder / (Path(image_filepath).stem + '_array_of_bbox.npz'))
         os.remove(files_folder / (Path(image_filepath).stem + '_array_of_masks_rearranged.npz'))
- 
+
     all_bboxes = np.vstack(all_bboxes)
 
     all_masks = np.stack(all_masks, axis=-1)
 
     # This will store the indices of the bboxes to keep
     to_keep = []
     for i, boxA in enumerate(all_bboxes):
@@ -366,21 +374,19 @@
     image_filepaths = []
     for image_filepath in image_filepaths_raw:
         if Path(image_filepath.replace('.png', '_array_of_masks.npz')).is_file() or double:
             image_filepaths.append(image_filepath)
 
     print('Finding bounding boxes and rearranging masks.')
     find_array_of_bboxes_and_rearrange_masks(filepath, image_filepaths, double)
-    
+
     print('Removing masks with identical bounding boxes.')
     unique_masks = remove_overlapping_bb(image_filepaths, iou_threshold=iou_threshold)
-    
-    print('Creating the final array of masks.')
-    bin_masks(filepath, unique_masks, binning=not double)
 
+    bin_masks(filepath, unique_masks, binning=not double)
 
 
 def format_time(elapsed_time):
     minutes, seconds = divmod(elapsed_time, 60)
     time_string = ""
     if minutes >= 1:
         minute_label = "minute" if minutes == 1 else "minutes"
@@ -432,29 +438,30 @@
     SAM_model = SAM_model.lower()
     SAM_model = model_mapping.get(SAM_model, SAM_model)
 
     directory = Path(os.path.dirname(__file__))
     available_SAM_models = [fname.name for fname in directory.glob('*.pt*') if fname.is_file()]
 
     model_info = {'fast': ['fast', 'FastSAM.pt', '144 MB'],
-                   'base': ['vit_b', 'sam_vit_b_01ec64.pth', '366 MB'],
-                   'large': ['vit_l', 'sam_vit_l_0b3195.pth', '1.2 GB'],
-                   'huge': ['vit_h', 'sam_vit_h_4b8939.pth', '2.5 GB']}
+                  'base': ['vit_b', 'sam_vit_b_01ec64.pth', '366 MB'],
+                  'large': ['vit_l', 'sam_vit_l_0b3195.pth', '1.2 GB'],
+                  'huge': ['vit_h', 'sam_vit_h_4b8939.pth', '2.5 GB']}
 
     if SAM_model == 'auto':
         if device == 'cpu':
             model = 'fast'
         elif device == 'cuda':
             model = 'base'
             if torch.cuda.get_device_properties(0).total_memory / 1024 ** 3 > 4:
                 model = 'huge'
     elif SAM_model in {'fast', 'base', 'large', 'huge'}:
         model = SAM_model
     else:
-        print("Invalid input. Valid inputs are 'a' for auto, 'h' for huge, 'l' for large, 'b' for base and 'f' for fast.")
+        print(
+            "Invalid input. Valid inputs are 'a' for auto, 'h' for huge, 'l' for large, 'b' for base and 'f' for fast.")
         return None
 
     if model_info.get(model)[1] in available_SAM_models:
         print(f'The {model} SAM weight ({model_info.get(model)[1]}) were chosen.')
         return directory / model_info.get(model)[1], model_info.get(model)[0], model
     else:
         ask_for_download = input(f'SAM weights were not found. This is probably because it is the first time running '
```

### Comparing `npsam-1.4.5/npsam.egg-info/PKG-INFO` & `npsam-1.4.6/npsam.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,273 +1,258 @@
-Metadata-Version: 2.1
-Name: npsam
-Version: 1.4.5
-Summary: NP-SAM is an easy-to-use segmentation and analysis tool for nanoparticles and more.
-Author-email: "Larsen, R. & Villadsen, T." <rasmus@inano.au.dk>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Keywords: nanoparticles,segmentation
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: numba==0.58.1
-Requires-Dist: opencv-python==4.9.0.80
-Requires-Dist: pandas==2.1.4
-Requires-Dist: matplotlib==3.8.2
-Requires-Dist: scikit-image==0.22.0
-Requires-Dist: ipympl==0.9.3
-Requires-Dist: PyQt5==5.15.10
-Requires-Dist: ultralytics==8.1.2
-Requires-Dist: jupyterlab==4.0.10
-Requires-Dist: clip==0.2.0
-Requires-Dist: piexif==1.1.3
-Requires-Dist: rosettasciio==0.1
-Requires-Dist: parse==1.20.1
-Requires-Dist: h5py==3.10.0
-Requires-Dist: tifffile==2024.1.30
-
-# NP-SAM
-
-## Introduction
-
-In this project we propose an easily implementable workflow for a fast, accurate and seamless experience of segmentation of nanoparticles.
-
-The project's experience can be significantly enhanced with the presence of a CUDA-compatible device; alternatively, Google Colab can be utilized if such a device is not accessible. For a quick access to the program and a CUDA-GPU try our Google Colab notebook. <br>
-[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/TorbenVilladsen/np-sam/blob/main/NPSAM_GoogleColab.ipynb)
-
-## Installation
-Create a new conda environment called `npsam` and activate it.
-```
-conda create -n npsam python=3.10
-conda activate npsam
-```
-**Install [PyTorch](https://pytorch.org/get-started/locally/)**. NP-SAM has been tested with Pytorch 2.1.2 and CUDA 11.8.
-
-Then install NP-SAM, and make a static link to the ipykernel
-```
-pip install npsam
-python -m ipykernel install --user --name npsam --display-name npsam
-```
-
-### Get started
-In the npsam environment execute `jupyter lab` in the terminal. This will launch jupyterlab. Try out one of the example notebooks on our GitLab.
-
-## Citation
-```
-@article{NPSAM,
-   author = {Larsen, Rasmus and Villadsen, Torben L. and Mathiesen, Jette K. and Jensen, Kirsten M. Ø and Bøjesen, Espen D.},
-   title = {NP-SAM: Implementing the Segment Anything Model for Easy Nanoparticle Segmentation in Electron Microscopy Images},
-   journal = {ChemRxiv},
-   DOI = {10.26434/chemrxiv-2023-k73qz-v2},
-   year = {2023},
-   type = {Journal Article}
-}
-```
-
-## Acknowledgment
-This repo benefits from Meta's [Segment Anything](https://github.com/facebookresearch/segment-anything) and [FastSAM](https://github.com/CASIA-IVA-Lab/FastSAM). Thanks for their great work.
-
-
+Metadata-Version: 2.1
+Name: npsam
+Version: 1.4.6
+Summary: NP-SAM is an easy-to-use segmentation and analysis tool for nanoparticles and more.
+Author-email: "Larsen, R. & Villadsen, T." <rasmus@inano.au.dk>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Keywords: nanoparticles,segmentation
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numba==0.58.1
+Requires-Dist: opencv-python==4.9.0.80
+Requires-Dist: pandas==2.1.4
+Requires-Dist: matplotlib==3.8.2
+Requires-Dist: scikit-image==0.22.0
+Requires-Dist: ipympl==0.9.3
+Requires-Dist: PyQt5==5.15.10
+Requires-Dist: ultralytics==8.1.2
+Requires-Dist: jupyterlab==4.0.10
+Requires-Dist: clip==0.2.0
+Requires-Dist: piexif==1.1.3
+Requires-Dist: rosettasciio==0.1
+Requires-Dist: parse==1.20.1
+Requires-Dist: h5py==3.10.0
+Requires-Dist: tifffile==2024.1.30
+
+# NP-SAM
+
+## Introduction
+
+In this project we propose an easily implementable workflow for a fast, accurate and seamless experience of segmentation of nanoparticles.
+
+The project's experience could be significantly enhanced with the presence of a CUDA-compatible device; alternatively, Google Colab can be utilized if such a device is not accessible. For a quick access to the program and a CUDA-GPU try our Google Colab notebook.
+
+### Get started
+In the working directory and NPSAM environment execute `jupyter lab` in the terminal. This will launch jupyterlab. 
+
+## Citation
+```
+@article{NPSAM,
+   author = {Larsen, Rasmus and Villadsen, Torben L. and Mathiesen, Jette K. and Jensen, Kirsten M. Ø and Bøjesen, Espen D.},
+   title = {NP-SAM: Implementing the Segment Anything Model for Easy Nanoparticle Segmentation in Electron Microscopy Images},
+   journal = {ChemRxiv},
+   DOI = {10.26434/chemrxiv-2023-k73qz-v2},
+   year = {2023},
+   type = {Journal Article}
+}
+```
+
+## Acknowledgment
+This repo benefits from Meta's [Segment Anything](https://github.com/facebookresearch/segment-anything) and [FastSAM](https://github.com/CASIA-IVA-Lab/FastSAM). Thanks for their great work.
+
+
```

### Comparing `npsam-1.4.5/npsam.egg-info/SOURCES.txt` & `npsam-1.4.6/npsam.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 npsam/npsam.py
 npsam/utils.py
 npsam.egg-info/PKG-INFO
 npsam.egg-info/SOURCES.txt
 npsam.egg-info/dependency_links.txt
 npsam.egg-info/requires.txt
 npsam.egg-info/top_level.txt
+npsam/segment_anything/NPSAM.py
 npsam/segment_anything/__init__.py
 npsam/segment_anything/automatic_mask_generator.py
 npsam/segment_anything/build_sam.py
 npsam/segment_anything/predictor.py
 npsam/segment_anything/modeling/__init__.py
 npsam/segment_anything/modeling/common.py
 npsam/segment_anything/modeling/image_encoder.py
```


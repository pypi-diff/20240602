# Comparing `tmp/gsnodegraph-0.5.5.tar.gz` & `tmp/gsnodegraph-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsnodegraph-0.5.5.tar", last modified: Mon Feb  6 19:31:23 2023, max compression
+gzip compressed data, was "gsnodegraph-0.5.6.tar", last modified: Sun Jun  2 18:12:36 2024, max compression
```

## Comparing `gsnodegraph-0.5.5.tar` & `gsnodegraph-0.5.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-02-06 19:31:23.000692 gsnodegraph-0.5.5/
--rw-rw-rw-   0        0        0    11556 2021-10-20 22:56:44.000000 gsnodegraph-0.5.5/LICENSE
--rw-rw-rw-   0        0        0      834 2023-02-06 19:31:23.000692 gsnodegraph-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     6028 2022-02-16 17:38:37.000000 gsnodegraph-0.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-02-06 19:31:22.962689 gsnodegraph-0.5.5/gsnodegraph/
--rw-rw-rw-   0        0        0      436 2022-01-20 18:42:53.000000 gsnodegraph-0.5.5/gsnodegraph/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-06 19:31:22.982695 gsnodegraph-0.5.5/gsnodegraph/assets/
--rw-rw-rw-   0        0        0       24 2021-11-11 18:53:58.000000 gsnodegraph-0.5.5/gsnodegraph/assets/__init__.py
--rw-rw-rw-   0        0        0     2457 2022-02-16 17:22:59.000000 gsnodegraph-0.5.5/gsnodegraph/assets/bitmaps.py
--rw-rw-rw-   0        0        0     1692 2022-02-16 16:51:59.000000 gsnodegraph-0.5.5/gsnodegraph/constants.py
-drwxrwxrwx   0        0        0        0 2023-02-06 19:31:22.986693 gsnodegraph-0.5.5/gsnodegraph/graph/
--rw-rw-rw-   0        0        0      377 2022-01-20 18:42:46.000000 gsnodegraph-0.5.5/gsnodegraph/graph/__init__.py
--rw-rw-rw-   0        0        0    34866 2023-02-06 19:07:29.000000 gsnodegraph-0.5.5/gsnodegraph/graph/base.py
--rw-rw-rw-   0        0        0     1508 2021-11-19 21:19:14.000000 gsnodegraph-0.5.5/gsnodegraph/graph/btn.py
-drwxrwxrwx   0        0        0        0 2023-02-06 19:31:22.990688 gsnodegraph-0.5.5/gsnodegraph/graph/utils/
--rw-rw-rw-   0        0        0       31 2021-03-28 06:14:08.000000 gsnodegraph-0.5.5/gsnodegraph/graph/utils/__init__.py
--rw-rw-rw-   0        0        0     2402 2020-12-11 22:07:46.000000 gsnodegraph-0.5.5/gsnodegraph/graph/utils/z_matrix.py
-drwxrwxrwx   0        0        0        0 2023-02-06 19:31:22.998690 gsnodegraph-0.5.5/gsnodegraph/node/
--rw-rw-rw-   0        0        0      119 2022-02-16 16:56:10.000000 gsnodegraph-0.5.5/gsnodegraph/node/__init__.py
--rw-rw-rw-   0        0        0    11979 2023-02-06 19:05:37.000000 gsnodegraph-0.5.5/gsnodegraph/node/node.py
--rw-rw-rw-   0        0        0     2928 2023-02-06 19:03:03.000000 gsnodegraph-0.5.5/gsnodegraph/node/socket.py
--rw-rw-rw-   0        0        0     1170 2022-02-16 16:56:22.000000 gsnodegraph-0.5.5/gsnodegraph/node/utils.py
--rw-rw-rw-   0        0        0     2764 2022-01-30 21:59:59.000000 gsnodegraph-0.5.5/gsnodegraph/node/wire.py
-drwxrwxrwx   0        0        0        0 2023-02-06 19:31:22.979689 gsnodegraph-0.5.5/gsnodegraph.egg-info/
--rw-rw-rw-   0        0        0      834 2023-02-06 19:31:22.000000 gsnodegraph-0.5.5/gsnodegraph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      620 2023-02-06 19:31:22.000000 gsnodegraph-0.5.5/gsnodegraph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-06 19:31:22.000000 gsnodegraph-0.5.5/gsnodegraph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-02-06 19:31:22.000000 gsnodegraph-0.5.5/gsnodegraph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-06 19:31:22.000000 gsnodegraph-0.5.5/gsnodegraph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2021-10-20 22:55:36.000000 gsnodegraph-0.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-02-06 19:31:23.007691 gsnodegraph-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1120 2023-02-06 19:30:37.000000 gsnodegraph-0.5.5/setup.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-06-02 18:12:36.326783 gsnodegraph-0.5.6/
+-rw-rw-r--   0 noah      (1000) noah      (1000)    11356 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/LICENSE
+-rw-r--r--   0 noah      (1000) noah      (1000)      947 2024-06-02 18:12:36.326783 gsnodegraph-0.5.6/PKG-INFO
+-rw-rw-r--   0 noah      (1000) noah      (1000)     6028 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/README.md
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-06-02 18:12:36.326783 gsnodegraph-0.5.6/gsnodegraph/
+-rw-rw-r--   0 noah      (1000) noah      (1000)      427 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/__init__.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-06-02 18:12:36.326783 gsnodegraph-0.5.6/gsnodegraph/assets/
+-rw-rw-r--   0 noah      (1000) noah      (1000)       23 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/assets/__init__.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     2419 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/assets/bitmaps.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1638 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/constants.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-06-02 18:12:36.326783 gsnodegraph-0.5.6/gsnodegraph/graph/
+-rw-rw-r--   0 noah      (1000) noah      (1000)      369 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/graph/__init__.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)    33962 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/graph/base.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1453 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/graph/btn.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-06-02 18:12:36.326783 gsnodegraph-0.5.6/gsnodegraph/graph/utils/
+-rw-rw-r--   0 noah      (1000) noah      (1000)       30 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/graph/utils/__init__.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     2315 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/graph/utils/z_matrix.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-06-02 18:12:36.326783 gsnodegraph-0.5.6/gsnodegraph/node/
+-rw-rw-r--   0 noah      (1000) noah      (1000)      116 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/node/__init__.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)    11645 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/node/node.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     2845 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/node/socket.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1140 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/node/utils.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     2686 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/gsnodegraph/node/wire.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-06-02 18:12:36.326783 gsnodegraph-0.5.6/gsnodegraph.egg-info/
+-rw-r--r--   0 noah      (1000) noah      (1000)      947 2024-06-02 18:12:36.000000 gsnodegraph-0.5.6/gsnodegraph.egg-info/PKG-INFO
+-rw-rw-r--   0 noah      (1000) noah      (1000)      620 2024-06-02 18:12:36.000000 gsnodegraph-0.5.6/gsnodegraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)        1 2024-06-02 18:12:36.000000 gsnodegraph-0.5.6/gsnodegraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)       16 2024-06-02 18:12:36.000000 gsnodegraph-0.5.6/gsnodegraph.egg-info/requires.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)       12 2024-06-02 18:12:36.000000 gsnodegraph-0.5.6/gsnodegraph.egg-info/top_level.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)      104 2024-06-02 17:59:21.000000 gsnodegraph-0.5.6/pyproject.toml
+-rw-rw-r--   0 noah      (1000) noah      (1000)       79 2024-06-02 18:12:36.330783 gsnodegraph-0.5.6/setup.cfg
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1179 2024-06-02 18:11:04.000000 gsnodegraph-0.5.6/setup.py
```

### Comparing `gsnodegraph-0.5.5/LICENSE` & `gsnodegraph-0.5.6/LICENSE`

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
    limitations under the License.
```

### Comparing `gsnodegraph-0.5.5/README.md` & `gsnodegraph-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `gsnodegraph-0.5.5/gsnodegraph/assets/bitmaps.py` & `gsnodegraph-0.5.6/gsnodegraph/assets/bitmaps.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from wx.lib.embeddedimage import PyEmbeddedImage
-#--------------------
-ICON_ADD_NODE = PyEmbeddedImage(
-    b'iVBORw0KGgoAAAANSUhEUgAAAC0AAAAtCAYAAAA6GuKaAAAABHNCSVQICAgIfAhkiAAAA9ZJ'
-    b'REFUWIXtWUF24jgQ/WVpP7lBe04w0cPs6ROEPkHICZqcoDMnSPcJEk7Q5ASh14gncoIxNyB7'
-    b'yzULZKIHklsmkJkFf0MsS/rfJVVJVQHOOOOM/xx0jEmMMRfW2isiygGAmQcAQEQz91wKIZ6U'
-    b'Uutj8B0s2gm9BjAEMEgcNgMwFUJM3vMBB4nWWl8D+A7gIvD6lZmXAEBElwD+CPQpAdwVRTE5'
-    b'hL+TaGPMZVVVD05MgxcAMyHEo1JqGRtnrR1hsyJ/Ne3MvJRSflFKlScRPZ/PB0T0E2/WXQEY'
-    b'F0Ux7UKotR5is0qfXNOamb/0+/1Z6hxJoheLxYiZH7aDiG57vd73LmIDc46Z+d6b86bX6z2m'
-    b'jP2taLe0z9hY+BXAqKt1Y3BWf8Rm36+FEJ9jW8xHq2gXIf5xgiGEUCmTdoEzinGPpeNojSxZ'
-    b'20tr7TZCENFNqmCt9Vet9deUvkqpJRHduMfccbYiaukdC0yKohiliHAO+wwAzPw51cG01lMA'
-    b'VwAghPizLaJELW2t3TqJEOIuhfg9EEKMPe6Htr5B0caYHO6UY+a/u8bRQ+A4frjHgTEmdHAB'
-    b'iIiu63p7LEspjxIpUiCE2Ia8uq6HsX5B0czcDFgdO1q0wXGtdjTsIbanr9zvh1nZQ8N5FevQ'
-    b'GvKY+ShXyS5I4ZS7DcaY3FoLACCi4NaYz+f3O5cmn9R3oHutdVAEMy/7/f7tbrvPaYzJQ0Fg'
-    b'T3RVVTkRNRMHCYloHGp37/y/gx/m3g0A7Ilm5nUzR1VVOTbX2HbRUsrSs3Qs7Pxg5qAgN6a5'
-    b'fr60fHhwFX1OKWUw1O6JVkqVWmsAgBO254xFUUQtvXMijrtcORvOxtKx86HVEVssfTJ4nK+x'
-    b'PjHRT+43GnZOiIYzukJB0UTUbIncGBN1pmPDceU7GvYQFJ1l2fYrq6qKnkzHhrV26ytZlnUT'
-    b'rZQqmfkXABDRN3eBOikcxzUAMPOvtkQg6ohSyu392b+mngo+h88dQlS0CzdNXWK4WCySkoB+'
-    b'vz8jolsiuk0Nd27uZhtOfncVTskRS7iCywfkiCshxOW7ckSl1FoIMYCLmdbaZ5dBHwVa66HL'
-    b'9AHgVQgxTCmXtYoGtoln49UXAH6mJq1tWCwW3wD4xZ9R6ip2rTBN8VabKwHcHlhhuoeLx9hY'
-    b'eNBl23Wt5eXW2im8ehyAkpmnUspJWy2vqqprIhp6YgHgxW2J09TyfLgy2R3e6nE+1gAa8ZcI'
-    b'V1ZXRHSXWgbbxbvq03Vdj1wBPfWO8kREsyzLHj+8Pr0L9wHDuq6bpW+y+RkAZFlWZlk2PdZ/'
-    b'As4444z/Af4FELLNYCJ7/vwAAAAASUVORK5CYII=')
-
-#----------------------------------------------------------------------
-ICON_BRUSH_CHECKERBOARD = PyEmbeddedImage(
-    b'iVBORw0KGgoAAAANSUhEUgAAAGQAAABkAQMAAABKLAcXAAAABlBMVEVfYWQnLjUoH6AuAAAA'
-    b'KElEQVQ4y2NgsP/A/B9GDDDv/wH+PzCCYWB5o+EyGi6j4TIaLrTiAQDYaoSnfkBkDwAAAABJ'
-    b'RU5ErkJggg==')
-
-#----------------------------------------------------------------------
-ICON_IMAGE = PyEmbeddedImage(
-    b'iVBORw0KGgoAAAANSUhEUgAAAA8AAAAPCAYAAAA71pVKAAAACXBIWXMAAA7DAAAOwwHHb6hk'
-    b'AAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAHBJREFUKJHVkksOgCAM'
-    b'RJ/GExDLYUw8vXga4Azjyg0QDcGNs2z6+pkWBjQBpJROSVsHF8xsByDGqJ6Od/7cA5VaGlUz'
-    b'4Mq4pOy9Xx9hwJnZ1CharTY09k/hyjBJuWWOpPwKl+d40idjh84XPUaaAnAB0HEs5elgUi0A'
-    b'AAAASUVORK5CYII=')
-
+from wx.lib.embeddedimage import PyEmbeddedImage
+#--------------------
+ICON_ADD_NODE = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAAC0AAAAtCAYAAAA6GuKaAAAABHNCSVQICAgIfAhkiAAAA9ZJ'
+    b'REFUWIXtWUF24jgQ/WVpP7lBe04w0cPs6ROEPkHICZqcoDMnSPcJEk7Q5ASh14gncoIxNyB7'
+    b'yzULZKIHklsmkJkFf0MsS/rfJVVJVQHOOOOM/xx0jEmMMRfW2isiygGAmQcAQEQz91wKIZ6U'
+    b'Uutj8B0s2gm9BjAEMEgcNgMwFUJM3vMBB4nWWl8D+A7gIvD6lZmXAEBElwD+CPQpAdwVRTE5'
+    b'hL+TaGPMZVVVD05MgxcAMyHEo1JqGRtnrR1hsyJ/Ne3MvJRSflFKlScRPZ/PB0T0E2/WXQEY'
+    b'F0Ux7UKotR5is0qfXNOamb/0+/1Z6hxJoheLxYiZH7aDiG57vd73LmIDc46Z+d6b86bX6z2m'
+    b'jP2taLe0z9hY+BXAqKt1Y3BWf8Rm36+FEJ9jW8xHq2gXIf5xgiGEUCmTdoEzinGPpeNojSxZ'
+    b'20tr7TZCENFNqmCt9Vet9deUvkqpJRHduMfccbYiaukdC0yKohiliHAO+wwAzPw51cG01lMA'
+    b'VwAghPizLaJELW2t3TqJEOIuhfg9EEKMPe6Htr5B0caYHO6UY+a/u8bRQ+A4frjHgTEmdHAB'
+    b'iIiu63p7LEspjxIpUiCE2Ia8uq6HsX5B0czcDFgdO1q0wXGtdjTsIbanr9zvh1nZQ8N5FevQ'
+    b'GvKY+ShXyS5I4ZS7DcaY3FoLACCi4NaYz+f3O5cmn9R3oHutdVAEMy/7/f7tbrvPaYzJQ0Fg'
+    b'T3RVVTkRNRMHCYloHGp37/y/gx/m3g0A7Ilm5nUzR1VVOTbX2HbRUsrSs3Qs7Pxg5qAgN6a5'
+    b'fr60fHhwFX1OKWUw1O6JVkqVWmsAgBO254xFUUQtvXMijrtcORvOxtKx86HVEVssfTJ4nK+x'
+    b'PjHRT+43GnZOiIYzukJB0UTUbIncGBN1pmPDceU7GvYQFJ1l2fYrq6qKnkzHhrV26ytZlnUT'
+    b'rZQqmfkXABDRN3eBOikcxzUAMPOvtkQg6ohSyu392b+mngo+h88dQlS0CzdNXWK4WCySkoB+'
+    b'vz8jolsiuk0Nd27uZhtOfncVTskRS7iCywfkiCshxOW7ckSl1FoIMYCLmdbaZ5dBHwVa66HL'
+    b'9AHgVQgxTCmXtYoGtoln49UXAH6mJq1tWCwW3wD4xZ9R6ip2rTBN8VabKwHcHlhhuoeLx9hY'
+    b'eNBl23Wt5eXW2im8ehyAkpmnUspJWy2vqqprIhp6YgHgxW2J09TyfLgy2R3e6nE+1gAa8ZcI'
+    b'V1ZXRHSXWgbbxbvq03Vdj1wBPfWO8kREsyzLHj+8Pr0L9wHDuq6bpW+y+RkAZFlWZlk2PdZ/'
+    b'As4444z/Af4FELLNYCJ7/vwAAAAASUVORK5CYII=')
+
+#----------------------------------------------------------------------
+ICON_BRUSH_CHECKERBOARD = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAAGQAAABkAQMAAABKLAcXAAAABlBMVEVfYWQnLjUoH6AuAAAA'
+    b'KElEQVQ4y2NgsP/A/B9GDDDv/wH+PzCCYWB5o+EyGi6j4TIaLrTiAQDYaoSnfkBkDwAAAABJ'
+    b'RU5ErkJggg==')
+
+#----------------------------------------------------------------------
+ICON_IMAGE = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAAA8AAAAPCAYAAAA71pVKAAAACXBIWXMAAA7DAAAOwwHHb6hk'
+    b'AAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAHBJREFUKJHVkksOgCAM'
+    b'RJ/GExDLYUw8vXga4Azjyg0QDcGNs2z6+pkWBjQBpJROSVsHF8xsByDGqJ6Od/7cA5VaGlUz'
+    b'4Mq4pOy9Xx9hwJnZ1CharTY09k/hyjBJuWWOpPwKl+d40idjh84XPUaaAnAB0HEs5elgUi0A'
+    b'AAAASUVORK5CYII=')
+
```

### Comparing `gsnodegraph-0.5.5/gsnodegraph/graph/utils/z_matrix.py` & `gsnodegraph-0.5.6/gsnodegraph/graph/utils/z_matrix.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-# ----------------------------------------------------------------------------
-# This file is code from EmbroidePy
-# which is licensed under the MIT License
-# Copyright (c) 2018 Metallicow
-# ----------------------------------------------------------------------------
-
-from wx import AffineMatrix2D
-
-
-class ZMatrix(AffineMatrix2D):
-    def __init__(self, *args, **kwds):
-        AffineMatrix2D.__init__(self)
-
-    def Reset(self):
-        AffineMatrix2D.__init__(self)
-
-    def PostScale(self, sx, sy=None, ax=0, ay=0):
-        self.Invert()
-        if sy is None:
-            sy = sx
-        if ax == 0 and ay == 0:
-            self.Scale(1.0 / sx, 1.0 / sy)
-        else:
-            self.Translate(ax, ay)
-            self.Scale(1.0 / sx, 1.0 / sy)
-            self.Translate(-ax, -ay)
-        self.Invert()
-
-    def PostTranslate(self, px, py):
-        self.Invert()
-        self.Translate(-px, -py)
-        self.Invert()
-
-    def PostRotate(self, radians, rx=0, ry=0):
-        self.Invert()
-        if rx == 0 and ry == 0:
-            self.Rotate(-radians)
-        else:
-            self.Translate(rx, ry)
-            self.Rotate(-radians)
-            self.Translate(-rx, -ry)
-        self.Invert()
-
-    def PreScale(self, sx, sy=None, ax=0, ay=0):
-        if sy is None:
-            sy = sx
-        if ax == 0 and ay == 0:
-            self.Scale(sx, sy)
-        else:
-            self.Translate(ax, ay)
-            self.Scale(sx, sy)
-            self.Translate(-ax, -ay)
-
-    def PreTranslate(self, px, py):
-        self.Translate(px, py)
-
-    def PreRotate(self, radians, rx=0, ry=0):
-        if rx == 0 and ry == 0:
-            self.Rotate(radians)
-        else:
-            self.Translate(rx, ry)
-            self.Rotate(radians)
-            self.Translate(-rx, -ry)
-
-    def GetScaleX(self):
-        return self.Get()[0].m_11
-
-    def GetScaleY(self):
-        return self.Get()[0].m_22
-
-    def GetSkewX(self):
-        return self.Get()[0].m_12
-
-    def GetSkewY(self):
-        return self.Get()[0].m_21
-
-    def GetTranslateX(self):
-        return self.Get()[1].x
-
-    def GetTranslateY(self):
-        return self.Get()[1].y
-
-    def InverseTransformPoint(self, position):
-        self.Invert()
-        converted_point = self.TransformPoint(position)
-        self.Invert()
-        return converted_point
+# ----------------------------------------------------------------------------
+# This file is code from EmbroidePy
+# which is licensed under the MIT License
+# Copyright (c) 2018 Metallicow
+# ----------------------------------------------------------------------------
+
+from wx import AffineMatrix2D
+
+
+class ZMatrix(AffineMatrix2D):
+    def __init__(self, *args, **kwds):
+        AffineMatrix2D.__init__(self)
+
+    def Reset(self):
+        AffineMatrix2D.__init__(self)
+
+    def PostScale(self, sx, sy=None, ax=0, ay=0):
+        self.Invert()
+        if sy is None:
+            sy = sx
+        if ax == 0 and ay == 0:
+            self.Scale(1.0 / sx, 1.0 / sy)
+        else:
+            self.Translate(ax, ay)
+            self.Scale(1.0 / sx, 1.0 / sy)
+            self.Translate(-ax, -ay)
+        self.Invert()
+
+    def PostTranslate(self, px, py):
+        self.Invert()
+        self.Translate(-px, -py)
+        self.Invert()
+
+    def PostRotate(self, radians, rx=0, ry=0):
+        self.Invert()
+        if rx == 0 and ry == 0:
+            self.Rotate(-radians)
+        else:
+            self.Translate(rx, ry)
+            self.Rotate(-radians)
+            self.Translate(-rx, -ry)
+        self.Invert()
+
+    def PreScale(self, sx, sy=None, ax=0, ay=0):
+        if sy is None:
+            sy = sx
+        if ax == 0 and ay == 0:
+            self.Scale(sx, sy)
+        else:
+            self.Translate(ax, ay)
+            self.Scale(sx, sy)
+            self.Translate(-ax, -ay)
+
+    def PreTranslate(self, px, py):
+        self.Translate(px, py)
+
+    def PreRotate(self, radians, rx=0, ry=0):
+        if rx == 0 and ry == 0:
+            self.Rotate(radians)
+        else:
+            self.Translate(rx, ry)
+            self.Rotate(radians)
+            self.Translate(-rx, -ry)
+
+    def GetScaleX(self):
+        return self.Get()[0].m_11
+
+    def GetScaleY(self):
+        return self.Get()[0].m_22
+
+    def GetSkewX(self):
+        return self.Get()[0].m_12
+
+    def GetSkewY(self):
+        return self.Get()[0].m_21
+
+    def GetTranslateX(self):
+        return self.Get()[1].x
+
+    def GetTranslateY(self):
+        return self.Get()[1].y
+
+    def InverseTransformPoint(self, position):
+        self.Invert()
+        converted_point = self.TransformPoint(position)
+        self.Invert()
+        return converted_point
```

### Comparing `gsnodegraph-0.5.5/gsnodegraph/node/node.py` & `gsnodegraph-0.5.6/gsnodegraph/node/node.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,334 +1,334 @@
-# ----------------------------------------------------------------------------
-# gsnodegraph Copyright 2019-2022 by Noah Rahm and contributors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ----------------------------------------------------------------------------
-
-import wx
-
-from gsnodegraph.assets.bitmaps import ICON_IMAGE
-
-from .socket import NodeSocket
-from .utils import TruncateText
-from ..constants import (NODE_DEFAULT_WIDTH, NODE_DEFAULT_HEIGHT,
-                         NODE_HEADER_MUTED_COLOR,
-                         SOCKET_INPUT, SOCKET_OUTPUT, NODE_THUMB_PADDING, NODE_Y_PADDING,
-                         NODE_NORMAL_COLOR, NODE_MUTED_COLOR, NODE_THUMB_BORDER_COLOR,
-                         NODE_BORDER_NORMAL_COLOR, NODE_BORDER_SELECTED_COLOR)
-from ..assets import (ICON_BRUSH_CHECKERBOARD, ICON_IMAGE)
-
-
-class NodeBase(object):
-    def __init__(self, nodegraph, id):
-        self.nodegraph = nodegraph
-        self.id = id
-        self.idname = None
-        self.pos = wx.Point(0, 0)
-        self.size = wx.Size(NODE_DEFAULT_WIDTH, NODE_DEFAULT_HEIGHT)
-        self.header_color = wx.Colour("#242424")
-
-        self.expanded = False
-        self.selected = False
-        self.active = False
-        self.muted = False
-        self.is_output = False
-
-        self.sockets = []
-        self.properties = {}
-        self.outputs = {}
-
-        self.label = ""
-        self.category = None
-        self.has_thumbnail = False
-
-        self.thumbnail = self.CreateEmptyBitmap()
-        self.expandicon_bmp = ICON_IMAGE.GetBitmap()
-        self.checkerboard_bmp = ICON_BRUSH_CHECKERBOARD.GetBitmap()
-
-    @property
-    def NodeGraph(self):
-        return self.nodegraph
-
-    @property
-    def NodeDatatypes(self):
-        return self.nodegraph.node_datatypes
-
-    @property
-    def NodeCategories(self):
-        return self.nodegraph.node_categories
-
-    @property
-    def NodeImageDatatype(self):
-        return self.nodegraph.image_datatype
-
-    def Init(self, idname) -> None:
-        self.InitSockets()
-        self.InitHeaderColor()
-        self.InitSize()
-        self.InitLabel()
-        self.SetIdName(idname)
-
-    def CreateEmptyBitmap(self) -> wx.Bitmap:
-        img = wx.Image(120, 120)
-        img.SetMaskColour(0,0,0)
-        img.InitAlpha()
-        return img.ConvertToBitmap()
-
-    def AddSocket(self, label, color, direction) -> None:
-        self.ArrangeSockets()
-
-    def HitTest(self, pos: wx.Point) -> None:
-        # Handle expanding the node to show thumbnail hittest
-        if self.HasThumbnail() and wx.GetMouseState().LeftIsDown():
-            icon_rect = self.expandicon_rect.Inflate(10, 10)
-            mouse_rect = wx.Rect(pos[0], pos[1], 2, 2)
-            if mouse_rect.Intersects(icon_rect):
-                self.ToggleExpand()
-
-        # Handle socket hittest
-        for socket in self.sockets:
-            if socket.HitTest(pos - self.pos):
-                return socket
-
-    def EditConnection(self, name, binding, socket):
-        pass
-
-    def InitHeaderColor(self) -> None:
-        self.header_color = wx.Colour(self.NodeCategories[self.GetCategory()])
-
-    def InitSockets(self) -> None:
-        sockets = []
-        ins = []
-        outs = []
-
-        # Create a list of input and output sockets with the format:
-        # [(label, idname, datatype), ...]
-        for prop_id in self.properties:
-            prop = self.properties[prop_id]
-            if prop.exposed and prop.can_be_exposed:
-                ins.append((prop.label, prop.idname, prop.datatype))
-
-        if self.IsOutputNode() is not True:
-            for output_id in self.outputs:
-                output = self.outputs[output_id]
-                outs.append((output.label, output.idname, output.datatype))
-                # If there is an image datatype then we know there 
-                # should be a thumbnail for this node.
-                if output.datatype == self.NodeImageDatatype:
-                    self.has_thumbnail = True
-
-        x, y, w, h = self.GetRect()
-        x, y = self.pos
-        w, h = self.size
-
-        for i, p in enumerate(outs + ins):
-            socket_type = SOCKET_INPUT  # Socket type IN
-            x = 0  # socket margin
-            if (p[0], p[1], p[2]) in outs:
-                x = w - x - 1
-                socket_type = SOCKET_OUTPUT  # Socket type OUT
-
-            # We keep track of where the last socket is placed
-            self.lastsocket_pos = 60 + 14 * i
-
-            # Create the node sockets
-            socket = NodeSocket(label=p[0], idname=p[1], datatype=p[2],
-                                node=self, direction=socket_type)
-            socket.pos = wx.Point(x, int(45 + (19 * i)))
-            socket.SetColor(self.NodeDatatypes[socket.datatype])
-            sockets.append(socket)
-
-        self.sockets = sockets
-
-    def InitSize(self) -> None:
-        # Calculate the normal size of the node to fit
-        # the amount of sockets the node has. The expanded size
-        # is calculated to be the normal size plus the image thumbnail size.
-        calc_height = self.lastsocket_pos + self.thumbnail.Height + NODE_THUMB_PADDING * 2
-        self.expanded_size = wx.Size(NODE_DEFAULT_WIDTH, calc_height)
-
-        self.normal_size = wx.Size(NODE_DEFAULT_WIDTH,
-                                   self.lastsocket_pos+(NODE_Y_PADDING*2))
-
-        # Set the initial node size
-        if self.IsExpanded():
-            self.SetSize(self.expanded_size)
-        else:
-            self.SetSize(self.normal_size)
-
-    def InitLabel(self):
-        # Number of chars to truncate from the label is based on 
-        # whether there is a toggle icon taking up space on this node.
-        if self.HasThumbnail() == True:
-            chars = 15
-        else:
-            chars = 20
-        self.label = TruncateText(self.GetLabel(), chars)
-
-    def HasThumbnail(self) -> bool:
-        return self.has_thumbnail
-
-    def IsOutputNode(self) -> bool:
-        """ Override method to set whether the node is the output or not. """
-        return self.is_output
-
-    def GetLabel(self) -> str:
-        """ Get the node label. """
-        return self.label
-
-    def GetCategory(self) -> str:
-        """ Override method to set the node category. """
-        return self.category
-
-    def GetIdname(self) -> str:
-        return self.idname
-
-    def SetIdName(self, idname) -> None:
-        self.idname = idname
-
-    def GetPosition(self) -> wx.Point:
-        return self.pos
-
-    def SetPosition(self, x: int, y: int) -> None:
-        self.pos = wx.Point(x, y)
-
-    def GetSize(self) -> wx.Size:
-        return (self.size[0], self.size[1])
-
-    def SetSize(self, size: wx.Size) -> None:
-        self.size = size
-
-    def GetRect(self) -> wx.Rect:
-        return wx.Rect(self.pos[0], self.pos[1], self.size[0], self.size[1])
-
-    def IsSelected(self) -> bool:
-        return self.selected
-
-    def SetSelected(self, selected=True) -> None:
-        self.selected = selected
-
-    def IsActive(self) -> bool:
-        return self.active
-
-    def SetActive(self, active=True) -> None:
-        self.active = active
-
-    def IsMuted(self) -> bool:
-        return self.muted
-
-    def SetMuted(self, muted=True) -> None:
-        self.muted = muted
-        self.SetExpanded(False)
-        self.SetSize(self.normal_size)
-
-    def IsExpanded(self) -> bool:
-        return self.expanded
-
-    def SetExpanded(self, expanded=True) -> None:
-        self.expanded = expanded
-
-    def ToggleExpand(self) -> None:
-        if self.HasThumbnail():
-            if self.IsExpanded() is True:
-                self.SetExpanded(False)
-                self.SetSize(self.normal_size)
-            elif self.IsExpanded() is False:
-                self.SetExpanded(True)
-                self.SetSize(self.expanded_size)
-
-    def GetSockets(self) -> list:
-        return self.sockets
-
-    def SetThumbnail(self, thumb) -> None:
-        if self.HasThumbnail():
-            self.thumbnail = thumb
-            self.UpdateExpandSize()
-
-    def UpdateExpandSize(self) -> None:
-        calc_height = self.lastsocket_pos + self.thumbnail.Height + NODE_THUMB_PADDING * 2
-        self.expanded_size = wx.Size(NODE_DEFAULT_WIDTH, calc_height)
-        self.SetSize(self.expanded_size)
-
-    def FindSocket(self, idname):
-        """ Return the node socket with the given name.
-        :param idname: the socket idname as a string
-        :returns: Socket object
-        """
-        for socket in self.GetSockets():
-            if socket.idname == idname:
-                return socket
-
-    def Draw(self, dc) -> None:
-        x, y = self.GetPosition()
-        w, h = self.GetSize()
-
-        # Node body and border
-        if self.IsSelected() or self.IsActive():
-            border_color = NODE_BORDER_SELECTED_COLOR
-        else:
-            border_color = NODE_BORDER_NORMAL_COLOR
-        if self.IsMuted():
-            node_color = NODE_MUTED_COLOR
-        else:
-            node_color = NODE_NORMAL_COLOR
-        dc.SetPen(wx.Pen(wx.Colour(border_color), 1))
-        dc.SetBrush(wx.Brush(wx.Colour(node_color)))
-        dc.DrawRoundedRectangle(x, y, w, h, 3)
-
-        # Node header
-        dc.SetPen(wx.Pen(wx.TRANSPARENT_PEN))
-        if self.IsMuted():
-            header_color = wx.Colour(NODE_HEADER_MUTED_COLOR)
-            bottom_color = wx.Colour(NODE_HEADER_MUTED_COLOR).ChangeLightness(80)
-        else:
-            header_color = wx.Colour(self.header_color).ChangeLightness(70)
-            bottom_color = wx.Colour(self.header_color).ChangeLightness(55)
-        dc.SetBrush(wx.Brush(header_color))
-        dc.DrawRoundedRectangle(x+1, y+1, w-2, 25, 3)
-
-        # Bottom border of the node header (to cover up the rounded bottom)
-        dc.SetBrush(wx.Brush(bottom_color))
-        dc.DrawRectangle(x+1, y+24, w-2, 2)
-
-        # Node name label
-        if self.IsMuted():
-            color = wx.Colour('#fff').ChangeLightness(60)
-        else:
-            color = wx.Colour('#fff').ChangeLightness(85)
-        dc.SetTextForeground(color)
-        dc.DrawText(self.GetLabel(), x+10, y+1)
-
-        # Node sockets
-        [socket.Draw(dc) for socket in self.sockets]
-
-        # Expand node thumbnail icon
-        if self.HasThumbnail() == True and self.IsMuted() != True:
-            self.expandicon_rect = wx.Rect(x+NODE_DEFAULT_WIDTH-28, y+5, 16, 16)
-            dc.DrawBitmap(self.expandicon_bmp, self.expandicon_rect[0],
-                        self.expandicon_rect[1], True)
-
-        # Thumbnail
-        if self.IsExpanded() and self.HasThumbnail():
-            # Calculate the coords for the placement of the thumbnail
-            thumb_rect = wx.Rect(int(x+NODE_THUMB_PADDING/2),
-                                 int(y+self.lastsocket_pos+(NODE_Y_PADDING*2)),
-                                 NODE_DEFAULT_WIDTH-NODE_THUMB_PADDING,
-                                 self.thumbnail.Height)
-
-            # Draw thumbnail border and background
-            dc.SetPen(wx.Pen(wx.Colour(NODE_THUMB_BORDER_COLOR), 1))
-            dc.SetBrush(wx.Brush(self.checkerboard_bmp))
-            dc.DrawRectangle(thumb_rect)
-
-            # Draw the thumbnail
-            dc.DrawBitmap(self.thumbnail, thumb_rect[0], thumb_rect[1], True)
+# ----------------------------------------------------------------------------
+# gsnodegraph Copyright 2019-2022 by Noah Rahm and contributors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ----------------------------------------------------------------------------
+
+import wx
+
+from gsnodegraph.assets.bitmaps import ICON_IMAGE
+
+from .socket import NodeSocket
+from .utils import TruncateText
+from ..constants import (NODE_DEFAULT_WIDTH, NODE_DEFAULT_HEIGHT,
+                         NODE_HEADER_MUTED_COLOR,
+                         SOCKET_INPUT, SOCKET_OUTPUT, NODE_THUMB_PADDING, NODE_Y_PADDING,
+                         NODE_NORMAL_COLOR, NODE_MUTED_COLOR, NODE_THUMB_BORDER_COLOR,
+                         NODE_BORDER_NORMAL_COLOR, NODE_BORDER_SELECTED_COLOR)
+from ..assets import (ICON_BRUSH_CHECKERBOARD, ICON_IMAGE)
+
+
+class NodeBase(object):
+    def __init__(self, nodegraph, id):
+        self.nodegraph = nodegraph
+        self.id = id
+        self.idname = None
+        self.pos = wx.Point(0, 0)
+        self.size = wx.Size(NODE_DEFAULT_WIDTH, NODE_DEFAULT_HEIGHT)
+        self.header_color = wx.Colour("#242424")
+
+        self.expanded = False
+        self.selected = False
+        self.active = False
+        self.muted = False
+        self.is_output = False
+
+        self.sockets = []
+        self.properties = {}
+        self.outputs = {}
+
+        self.label = ""
+        self.category = None
+        self.has_thumbnail = False
+
+        self.thumbnail = self.CreateEmptyBitmap()
+        self.expandicon_bmp = ICON_IMAGE.GetBitmap()
+        self.checkerboard_bmp = ICON_BRUSH_CHECKERBOARD.GetBitmap()
+
+    @property
+    def NodeGraph(self):
+        return self.nodegraph
+
+    @property
+    def NodeDatatypes(self):
+        return self.nodegraph.node_datatypes
+
+    @property
+    def NodeCategories(self):
+        return self.nodegraph.node_categories
+
+    @property
+    def NodeImageDatatype(self):
+        return self.nodegraph.image_datatype
+
+    def Init(self, idname) -> None:
+        self.InitSockets()
+        self.InitHeaderColor()
+        self.InitSize()
+        self.InitLabel()
+        self.SetIdName(idname)
+
+    def CreateEmptyBitmap(self) -> wx.Bitmap:
+        img = wx.Image(120, 120)
+        img.SetMaskColour(0,0,0)
+        img.InitAlpha()
+        return img.ConvertToBitmap()
+
+    def AddSocket(self, label, color, direction) -> None:
+        self.ArrangeSockets()
+
+    def HitTest(self, pos: wx.Point) -> None:
+        # Handle expanding the node to show thumbnail hittest
+        if self.HasThumbnail() and wx.GetMouseState().LeftIsDown():
+            icon_rect = self.expandicon_rect.Inflate(10, 10)
+            mouse_rect = wx.Rect(pos[0], pos[1], 2, 2)
+            if mouse_rect.Intersects(icon_rect):
+                self.ToggleExpand()
+
+        # Handle socket hittest
+        for socket in self.sockets:
+            if socket.HitTest(pos - self.pos):
+                return socket
+
+    def EditConnection(self, name, binding, socket):
+        pass
+
+    def InitHeaderColor(self) -> None:
+        self.header_color = wx.Colour(self.NodeCategories[self.GetCategory()])
+
+    def InitSockets(self) -> None:
+        sockets = []
+        ins = []
+        outs = []
+
+        # Create a list of input and output sockets with the format:
+        # [(label, idname, datatype), ...]
+        for prop_id in self.properties:
+            prop = self.properties[prop_id]
+            if prop.exposed and prop.can_be_exposed:
+                ins.append((prop.label, prop.idname, prop.datatype))
+
+        if self.IsOutputNode() is not True:
+            for output_id in self.outputs:
+                output = self.outputs[output_id]
+                outs.append((output.label, output.idname, output.datatype))
+                # If there is an image datatype then we know there 
+                # should be a thumbnail for this node.
+                if output.datatype == self.NodeImageDatatype:
+                    self.has_thumbnail = True
+
+        x, y, w, h = self.GetRect()
+        x, y = self.pos
+        w, h = self.size
+
+        for i, p in enumerate(outs + ins):
+            socket_type = SOCKET_INPUT  # Socket type IN
+            x = 0  # socket margin
+            if (p[0], p[1], p[2]) in outs:
+                x = w - x - 1
+                socket_type = SOCKET_OUTPUT  # Socket type OUT
+
+            # We keep track of where the last socket is placed
+            self.lastsocket_pos = 60 + 14 * i
+
+            # Create the node sockets
+            socket = NodeSocket(label=p[0], idname=p[1], datatype=p[2],
+                                node=self, direction=socket_type)
+            socket.pos = wx.Point(x, int(45 + (19 * i)))
+            socket.SetColor(self.NodeDatatypes[socket.datatype])
+            sockets.append(socket)
+
+        self.sockets = sockets
+
+    def InitSize(self) -> None:
+        # Calculate the normal size of the node to fit
+        # the amount of sockets the node has. The expanded size
+        # is calculated to be the normal size plus the image thumbnail size.
+        calc_height = self.lastsocket_pos + self.thumbnail.Height + NODE_THUMB_PADDING * 2
+        self.expanded_size = wx.Size(NODE_DEFAULT_WIDTH, calc_height)
+
+        self.normal_size = wx.Size(NODE_DEFAULT_WIDTH,
+                                   self.lastsocket_pos+(NODE_Y_PADDING*2))
+
+        # Set the initial node size
+        if self.IsExpanded():
+            self.SetSize(self.expanded_size)
+        else:
+            self.SetSize(self.normal_size)
+
+    def InitLabel(self):
+        # Number of chars to truncate from the label is based on 
+        # whether there is a toggle icon taking up space on this node.
+        if self.HasThumbnail() == True:
+            chars = 15
+        else:
+            chars = 20
+        self.label = TruncateText(self.GetLabel(), chars)
+
+    def HasThumbnail(self) -> bool:
+        return self.has_thumbnail
+
+    def IsOutputNode(self) -> bool:
+        """ Override method to set whether the node is the output or not. """
+        return self.is_output
+
+    def GetLabel(self) -> str:
+        """ Get the node label. """
+        return self.label
+
+    def GetCategory(self) -> str:
+        """ Override method to set the node category. """
+        return self.category
+
+    def GetIdname(self) -> str:
+        return self.idname
+
+    def SetIdName(self, idname) -> None:
+        self.idname = idname
+
+    def GetPosition(self) -> wx.Point:
+        return self.pos
+
+    def SetPosition(self, x: int, y: int) -> None:
+        self.pos = wx.Point(x, y)
+
+    def GetSize(self) -> wx.Size:
+        return (self.size[0], self.size[1])
+
+    def SetSize(self, size: wx.Size) -> None:
+        self.size = size
+
+    def GetRect(self) -> wx.Rect:
+        return wx.Rect(self.pos[0], self.pos[1], self.size[0], self.size[1])
+
+    def IsSelected(self) -> bool:
+        return self.selected
+
+    def SetSelected(self, selected=True) -> None:
+        self.selected = selected
+
+    def IsActive(self) -> bool:
+        return self.active
+
+    def SetActive(self, active=True) -> None:
+        self.active = active
+
+    def IsMuted(self) -> bool:
+        return self.muted
+
+    def SetMuted(self, muted=True) -> None:
+        self.muted = muted
+        self.SetExpanded(False)
+        self.SetSize(self.normal_size)
+
+    def IsExpanded(self) -> bool:
+        return self.expanded
+
+    def SetExpanded(self, expanded=True) -> None:
+        self.expanded = expanded
+
+    def ToggleExpand(self) -> None:
+        if self.HasThumbnail():
+            if self.IsExpanded() is True:
+                self.SetExpanded(False)
+                self.SetSize(self.normal_size)
+            elif self.IsExpanded() is False:
+                self.SetExpanded(True)
+                self.SetSize(self.expanded_size)
+
+    def GetSockets(self) -> list:
+        return self.sockets
+
+    def SetThumbnail(self, thumb) -> None:
+        if self.HasThumbnail():
+            self.thumbnail = thumb
+            self.UpdateExpandSize()
+
+    def UpdateExpandSize(self) -> None:
+        calc_height = self.lastsocket_pos + self.thumbnail.Height + NODE_THUMB_PADDING * 2
+        self.expanded_size = wx.Size(NODE_DEFAULT_WIDTH, calc_height)
+        self.SetSize(self.expanded_size)
+
+    def FindSocket(self, idname):
+        """ Return the node socket with the given name.
+        :param idname: the socket idname as a string
+        :returns: Socket object
+        """
+        for socket in self.GetSockets():
+            if socket.idname == idname:
+                return socket
+
+    def Draw(self, dc) -> None:
+        x, y = self.GetPosition()
+        w, h = self.GetSize()
+
+        # Node body and border
+        if self.IsSelected() or self.IsActive():
+            border_color = NODE_BORDER_SELECTED_COLOR
+        else:
+            border_color = NODE_BORDER_NORMAL_COLOR
+        if self.IsMuted():
+            node_color = NODE_MUTED_COLOR
+        else:
+            node_color = NODE_NORMAL_COLOR
+        dc.SetPen(wx.Pen(wx.Colour(border_color), 1))
+        dc.SetBrush(wx.Brush(wx.Colour(node_color)))
+        dc.DrawRoundedRectangle(x, y, w, h, 3)
+
+        # Node header
+        dc.SetPen(wx.Pen(wx.TRANSPARENT_PEN))
+        if self.IsMuted():
+            header_color = wx.Colour(NODE_HEADER_MUTED_COLOR)
+            bottom_color = wx.Colour(NODE_HEADER_MUTED_COLOR).ChangeLightness(80)
+        else:
+            header_color = wx.Colour(self.header_color).ChangeLightness(70)
+            bottom_color = wx.Colour(self.header_color).ChangeLightness(55)
+        dc.SetBrush(wx.Brush(header_color))
+        dc.DrawRoundedRectangle(x+1, y+1, w-2, 25, 3)
+
+        # Bottom border of the node header (to cover up the rounded bottom)
+        dc.SetBrush(wx.Brush(bottom_color))
+        dc.DrawRectangle(x+1, y+24, w-2, 2)
+
+        # Node name label
+        if self.IsMuted():
+            color = wx.Colour('#fff').ChangeLightness(60)
+        else:
+            color = wx.Colour('#fff').ChangeLightness(85)
+        dc.SetTextForeground(color)
+        dc.DrawText(self.GetLabel(), x+10, y+1)
+
+        # Node sockets
+        [socket.Draw(dc) for socket in self.sockets]
+
+        # Expand node thumbnail icon
+        if self.HasThumbnail() == True and self.IsMuted() != True:
+            self.expandicon_rect = wx.Rect(x+NODE_DEFAULT_WIDTH-28, y+5, 16, 16)
+            dc.DrawBitmap(self.expandicon_bmp, self.expandicon_rect[0],
+                        self.expandicon_rect[1], True)
+
+        # Thumbnail
+        if self.IsExpanded() and self.HasThumbnail():
+            # Calculate the coords for the placement of the thumbnail
+            thumb_rect = wx.Rect(int(x+NODE_THUMB_PADDING/2),
+                                 int(y+self.lastsocket_pos+(NODE_Y_PADDING*2)),
+                                 NODE_DEFAULT_WIDTH-NODE_THUMB_PADDING,
+                                 self.thumbnail.Height)
+
+            # Draw thumbnail border and background
+            dc.SetPen(wx.Pen(wx.Colour(NODE_THUMB_BORDER_COLOR), 1))
+            dc.SetBrush(wx.Brush(self.checkerboard_bmp))
+            dc.DrawRectangle(thumb_rect)
+
+            # Draw the thumbnail
+            dc.DrawBitmap(self.thumbnail, thumb_rect[0], thumb_rect[1], True)
```

### Comparing `gsnodegraph-0.5.5/gsnodegraph/node/socket.py` & `gsnodegraph-0.5.6/gsnodegraph/node/socket.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-# ----------------------------------------------------------------------------
-# gsnodegraph Copyright 2019-2022 by Noah Rahm and contributors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ----------------------------------------------------------------------------
-
-import math
-import wx
-
-from ..constants import (SOCKET_BORDER_COLOR, SOCKET_INPUT, SOCKET_HIT_RADIUS, 
-                         SOCKET_RADIUS, SOCKET_BORDER_COLOR)
-
-
-class NodeSocket(object):
-    """ 
-    Node socket showing the datatypes and flow of the node relative to
-    the graph. Wires are dropped into the socket to connect nodes. 
-    """
-    def __init__(self, label, idname, datatype, node, direction):
-        self.label = label
-        self.idname = idname
-        self.node = node
-        self.direction = direction
-        self.datatype = datatype
-
-        self.wires = []
-        self.pos = wx.Point(0, 0)
-        self.color = wx.Colour("#fff")
-        self.tdc = wx.WindowDC(wx.GetApp().GetTopWindow())
-
-        #self.SetColorByDataType(self.datatype)
-
-    def GetWires(self) -> list:
-        """ Get the wires for this socket. """
-        return self.wires
-
-    def SetColor(self, color) -> None:
-        """ Set the socket base color based on the datatype. """
-        self.color = wx.Colour(color)  
-
-    def CurrentSocketPos(self) -> wx.Point:
-        """ Return the current coords of the node socket. """
-        return self.pos + self.node.pos
-      
-    def HitTest(self, pos) -> bool:
-        """ Returns True if the node socket was hit. """
-        pnt = pos - self.pos
-        distance = math.sqrt(math.pow(pnt.x, 2) + math.pow(pnt.y, 2))
-
-        # Socket hit radius
-        if math.fabs(distance) < SOCKET_HIT_RADIUS:
-            return True
-
-    def Draw(self, dc) -> None:
-        """ Draw the node socket. """
-        pos = self.CurrentSocketPos()
-        w, h = self.tdc.GetTextExtent(self.label)
-
-        # Set the socket color
-        dc.SetPen(wx.Pen(wx.Colour(SOCKET_BORDER_COLOR), 1))
-        dc.SetBrush(wx.Brush(self.color))
-
-        # Draw the socket
-        dc.DrawCircle(pos.x, pos.y, SOCKET_RADIUS)
-
-        # Socket label margin
-        if self.direction == SOCKET_INPUT:
-            x = int(pos.x + 12)
-        else:
-            x = int(pos.x - w - 12)
-
-        # Draw the label
-        dc.DrawText(self.label, x, int(pos.y - h / 2))
+# ----------------------------------------------------------------------------
+# gsnodegraph Copyright 2019-2022 by Noah Rahm and contributors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ----------------------------------------------------------------------------
+
+import math
+import wx
+
+from ..constants import (SOCKET_BORDER_COLOR, SOCKET_INPUT, SOCKET_HIT_RADIUS, 
+                         SOCKET_RADIUS, SOCKET_BORDER_COLOR)
+
+
+class NodeSocket(object):
+    """ 
+    Node socket showing the datatypes and flow of the node relative to
+    the graph. Wires are dropped into the socket to connect nodes. 
+    """
+    def __init__(self, label, idname, datatype, node, direction):
+        self.label = label
+        self.idname = idname
+        self.node = node
+        self.direction = direction
+        self.datatype = datatype
+
+        self.wires = []
+        self.pos = wx.Point(0, 0)
+        self.color = wx.Colour("#fff")
+        self.tdc = wx.WindowDC(wx.GetApp().GetTopWindow())
+
+        #self.SetColorByDataType(self.datatype)
+
+    def GetWires(self) -> list:
+        """ Get the wires for this socket. """
+        return self.wires
+
+    def SetColor(self, color) -> None:
+        """ Set the socket base color based on the datatype. """
+        self.color = wx.Colour(color)  
+
+    def CurrentSocketPos(self) -> wx.Point:
+        """ Return the current coords of the node socket. """
+        return self.pos + self.node.pos
+      
+    def HitTest(self, pos) -> bool:
+        """ Returns True if the node socket was hit. """
+        pnt = pos - self.pos
+        distance = math.sqrt(math.pow(pnt.x, 2) + math.pow(pnt.y, 2))
+
+        # Socket hit radius
+        if math.fabs(distance) < SOCKET_HIT_RADIUS:
+            return True
+
+    def Draw(self, dc) -> None:
+        """ Draw the node socket. """
+        pos = self.CurrentSocketPos()
+        w, h = self.tdc.GetTextExtent(self.label)
+
+        # Set the socket color
+        dc.SetPen(wx.Pen(wx.Colour(SOCKET_BORDER_COLOR), 1))
+        dc.SetBrush(wx.Brush(self.color))
+
+        # Draw the socket
+        dc.DrawCircle(pos.x, pos.y, SOCKET_RADIUS)
+
+        # Socket label margin
+        if self.direction == SOCKET_INPUT:
+            x = int(pos.x + 12)
+        else:
+            x = int(pos.x - w - 12)
+
+        # Draw the label
+        dc.DrawText(self.label, x, int(pos.y - h / 2))
```

### Comparing `gsnodegraph-0.5.5/gsnodegraph/node/utils.py` & `gsnodegraph-0.5.6/gsnodegraph/node/utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# ----------------------------------------------------------------------------
-# gsnodegraph Copyright 2019-2022 by Noah Rahm and contributors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ----------------------------------------------------------------------------
-
-
-def TruncateText(text_string, str_length=18):
-    """ Truncate the text string after a certain
-    number of characters.
-    """
-    chars = []
-    for char in text_string:
-        chars.append(char)
-
-    if len(chars) > str_length:
-        words = chars[:str_length - 1]
-        text = "".join(words)
-        return "{}...".format(text)
-    else:
+# ----------------------------------------------------------------------------
+# gsnodegraph Copyright 2019-2022 by Noah Rahm and contributors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ----------------------------------------------------------------------------
+
+
+def TruncateText(text_string, str_length=18):
+    """ Truncate the text string after a certain
+    number of characters.
+    """
+    chars = []
+    for char in text_string:
+        chars.append(char)
+
+    if len(chars) > str_length:
+        words = chars[:str_length - 1]
+        text = "".join(words)
+        return "{}...".format(text)
+    else:
         return text_string
```

### Comparing `gsnodegraph-0.5.5/gsnodegraph/node/wire.py` & `gsnodegraph-0.5.6/gsnodegraph/node/wire.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-# ----------------------------------------------------------------------------
-# gsnodegraph Copyright 2019-2022 by Noah Rahm and contributors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ----------------------------------------------------------------------------
-
-import wx
-
-from ..constants import WIRE_NORMAL_COLOR, WIRE_ACTIVE_COLOR
-
-
-class NodeWire(object):
-    """ Wire for showing a connection between two nodes. """
-    def __init__(self, parent, pnt1, pnt2, srcsocket, dstsocket, direction, curvature):
-        self.parent = parent
-        self.pnt1 = pnt1
-        self.pnt2 = pnt2
-        self.srcsocket = srcsocket
-        self.dstsocket = dstsocket
-        self.curvature = curvature
-        self.direction = direction
-
-        self.srcnode = None
-        self.dstnode = None
-        self.active = False
-
-    def SetCurvature(self, curvature) -> None:
-        """ Set the curvature of the wire. """
-        self.curvature = curvature
-
-    def GetRect(self) -> wx.Rect:
-        """ Get the bounding box rect of the wire. """
-        min_x = min(self.pnt1[0], self.pnt2[0])
-        min_y = min(self.pnt1[1], self.pnt2[1])
-        size = self.pnt2 - self.pnt1
-        rect = wx.Rect(min_x - 10, min_y, abs(size[0]) + 20, abs(size[1]))
-        return rect.Inflate(2, 2)
-
-    def Draw(self, dc) -> None:
-        """ Draw the node wire. """
-        # Direction of wire
-        sign = 1
-        if self.direction == 0:
-            sign = -1
-
-        # Curvature of the wire
-        curvature = int(self.curvature * 2)
-
-        # Wire color
-        if self.active is True:
-            color = WIRE_ACTIVE_COLOR
-        else:
-            color = WIRE_NORMAL_COLOR
-        dc.SetPen(wx.Pen(wx.Colour(color), 3))
-
-        # If the wire has curvature, use a spline
-        if self.curvature > 0:
-            pnts = []
-            pnts.append(self.pnt1)
-            pnts.append(self.pnt1 + wx.Point(curvature * sign, 0))
-            pnts.append(self.pnt2 - wx.Point(curvature * sign, 0))
-            pnts.append(self.pnt2)
-
-            dc.DrawSpline(pnts)
-
-        else:
-            # Otherwise, use a line
-            dc.DrawLine(self.pnt1[0], self.pnt1[1], self.pnt2[0], self.pnt2[1])
+# ----------------------------------------------------------------------------
+# gsnodegraph Copyright 2019-2022 by Noah Rahm and contributors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ----------------------------------------------------------------------------
+
+import wx
+
+from ..constants import WIRE_NORMAL_COLOR, WIRE_ACTIVE_COLOR
+
+
+class NodeWire(object):
+    """ Wire for showing a connection between two nodes. """
+    def __init__(self, parent, pnt1, pnt2, srcsocket, dstsocket, direction, curvature):
+        self.parent = parent
+        self.pnt1 = pnt1
+        self.pnt2 = pnt2
+        self.srcsocket = srcsocket
+        self.dstsocket = dstsocket
+        self.curvature = curvature
+        self.direction = direction
+
+        self.srcnode = None
+        self.dstnode = None
+        self.active = False
+
+    def SetCurvature(self, curvature) -> None:
+        """ Set the curvature of the wire. """
+        self.curvature = curvature
+
+    def GetRect(self) -> wx.Rect:
+        """ Get the bounding box rect of the wire. """
+        min_x = min(self.pnt1[0], self.pnt2[0])
+        min_y = min(self.pnt1[1], self.pnt2[1])
+        size = self.pnt2 - self.pnt1
+        rect = wx.Rect(min_x - 10, min_y, abs(size[0]) + 20, abs(size[1]))
+        return rect.Inflate(2, 2)
+
+    def Draw(self, dc) -> None:
+        """ Draw the node wire. """
+        # Direction of wire
+        sign = 1
+        if self.direction == 0:
+            sign = -1
+
+        # Curvature of the wire
+        curvature = int(self.curvature * 2)
+
+        # Wire color
+        if self.active is True:
+            color = WIRE_ACTIVE_COLOR
+        else:
+            color = WIRE_NORMAL_COLOR
+        dc.SetPen(wx.Pen(wx.Colour(color), 3))
+
+        # If the wire has curvature, use a spline
+        if self.curvature > 0:
+            pnts = []
+            pnts.append(self.pnt1)
+            pnts.append(self.pnt1 + wx.Point(curvature * sign, 0))
+            pnts.append(self.pnt2 - wx.Point(curvature * sign, 0))
+            pnts.append(self.pnt2)
+
+            dc.DrawSpline(pnts)
+
+        else:
+            # Otherwise, use a line
+            dc.DrawLine(self.pnt1[0], self.pnt1[1], self.pnt2[0], self.pnt2[1])
```

### Comparing `gsnodegraph-0.5.5/gsnodegraph.egg-info/SOURCES.txt` & `gsnodegraph-0.5.6/gsnodegraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gsnodegraph-0.5.5/setup.py` & `gsnodegraph-0.5.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-from setuptools import setup
-
-
-setup(
-  name = 'gsnodegraph',
-  packages = ['gsnodegraph',
-              'gsnodegraph.graph',
-              'gsnodegraph.graph.utils',
-              'gsnodegraph.node',
-              'gsnodegraph.assets'],
-  version = '0.5.5',
-  license = 'Apache 2.0',
-  description = 'Powerful node graph widget for wxPython GUIs',
-  long_description_content_type="text/markdown",
-  author = 'Noah Rahm and contributors',
-  author_email = 'correctsyntax@yahoo.com',
-  url = 'https://github.com/GimelStudio/gsnodegraph',
-  keywords = ['nodegraph', 'nodes', 'graph', 'node-based', 'widget'],
-  install_requires = [
-      'wxpython==4.2.0'
-    ],
-  classifiers = [
-    'Development Status :: 2 - Pre-Alpha',
-    'Intended Audience :: Developers',
-    'Operating System :: OS Independent',
-    'Topic :: Desktop Environment',
-    'Topic :: Multimedia :: Graphics :: Editors',
-    'License :: OSI Approved :: Apache Software License',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-  ],
-)
+from setuptools import setup
+
+
+setup(
+  name = 'gsnodegraph',
+  packages = ['gsnodegraph',
+              'gsnodegraph.graph',
+              'gsnodegraph.graph.utils',
+              'gsnodegraph.node',
+              'gsnodegraph.assets'],
+  version = '0.5.6',
+  license = 'Apache 2.0',
+  description = 'Powerful node graph widget for wxPython GUIs',
+  long_description_content_type="text/markdown",
+  author = 'Noah Rahm and contributors',
+  author_email = 'correctsyntax@yahoo.com',
+  url = 'https://github.com/GimelStudio/gsnodegraph',
+  keywords = ['nodegraph', 'nodes', 'graph', 'node-based', 'widget'],
+  install_requires = [
+      'wxpython==4.2.1'
+    ],
+  classifiers = [
+    'Development Status :: 2 - Pre-Alpha',
+    'Intended Audience :: Developers',
+    'Operating System :: OS Independent',
+    'Topic :: Desktop Environment',
+    'Topic :: Multimedia :: Graphics :: Editors',
+    'License :: OSI Approved :: Apache Software License',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+  ],
+)
```


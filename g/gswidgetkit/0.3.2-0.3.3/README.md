# Comparing `tmp/gswidgetkit-0.3.2.tar.gz` & `tmp/gswidgetkit-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gswidgetkit-0.3.2.tar", last modified: Fri Jan 27 15:06:28 2023, max compression
+gzip compressed data, was "gswidgetkit-0.3.3.tar", last modified: Sun Jun  2 18:03:59 2024, max compression
```

## Comparing `gswidgetkit-0.3.2.tar` & `gswidgetkit-0.3.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-01-27 15:06:28.039591 gswidgetkit-0.3.2/
--rw-rw-rw-   0        0        0    11556 2021-12-17 04:06:58.000000 gswidgetkit-0.3.2/LICENSE
--rw-rw-rw-   0        0        0      826 2023-01-27 15:06:28.039591 gswidgetkit-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2546 2022-11-27 16:39:52.000000 gswidgetkit-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-27 15:06:28.007584 gswidgetkit-0.3.2/gswidgetkit/
--rw-rw-rw-   0        0        0      558 2022-01-17 23:05:11.000000 gswidgetkit-0.3.2/gswidgetkit/__init__.py
--rw-rw-rw-   0        0        0    10771 2023-01-27 14:57:20.000000 gswidgetkit-0.3.2/gswidgetkit/buttons.py
--rw-rw-rw-   0        0        0    20970 2022-01-18 00:05:04.000000 gswidgetkit-0.3.2/gswidgetkit/checkbox.py
--rw-rw-rw-   0        0        0     5799 2022-01-18 00:05:04.000000 gswidgetkit-0.3.2/gswidgetkit/color_picker.py
--rw-rw-rw-   0        0        0     1027 2022-02-15 17:26:05.000000 gswidgetkit-0.3.2/gswidgetkit/constants.py
--rw-rw-rw-   0        0        0     7619 2022-02-15 17:58:55.000000 gswidgetkit-0.3.2/gswidgetkit/dropdown.py
--rw-rw-rw-   0        0        0    81582 2022-01-18 00:05:04.000000 gswidgetkit-0.3.2/gswidgetkit/foldpanelbar.py
-drwxrwxrwx   0        0        0        0 2023-01-27 15:06:28.031585 gswidgetkit-0.3.2/gswidgetkit/icons/
--rw-rw-rw-   0        0        0       22 2021-06-22 17:27:38.000000 gswidgetkit-0.3.2/gswidgetkit/icons/__init__.py
--rw-rw-rw-   0        0        0    10652 2022-02-16 17:41:24.000000 gswidgetkit-0.3.2/gswidgetkit/icons/icons.py
--rw-rw-rw-   0        0        0     1829 2022-01-18 00:05:04.000000 gswidgetkit-0.3.2/gswidgetkit/label.py
--rw-rw-rw-   0        0        0    14564 2022-11-27 16:37:59.000000 gswidgetkit-0.3.2/gswidgetkit/number_field.py
--rw-rw-rw-   0        0        0      360 2021-11-15 19:26:20.000000 gswidgetkit-0.3.2/gswidgetkit/panel.py
--rw-rw-rw-   0        0        0     1120 2022-01-18 00:05:04.000000 gswidgetkit-0.3.2/gswidgetkit/popups.py
--rw-rw-rw-   0        0        0      779 2022-01-18 00:05:04.000000 gswidgetkit-0.3.2/gswidgetkit/scrollbar.py
--rw-rw-rw-   0        0        0     8165 2022-02-15 17:49:20.000000 gswidgetkit-0.3.2/gswidgetkit/textctrl.py
--rw-rw-rw-   0        0        0    17591 2022-01-18 00:05:04.000000 gswidgetkit-0.3.2/gswidgetkit/tooltip.py
--rw-rw-rw-   0        0        0      926 2022-01-18 00:05:04.000000 gswidgetkit-0.3.2/gswidgetkit/utils.py
--rw-rw-rw-   0        0        0     3036 2022-01-18 00:06:33.000000 gswidgetkit-0.3.2/gswidgetkit/z_matrix.py
--rw-rw-rw-   0        0        0     6559 2022-01-18 00:05:04.000000 gswidgetkit-0.3.2/gswidgetkit/zoom_panel.py
-drwxrwxrwx   0        0        0        0 2023-01-27 15:06:28.031585 gswidgetkit-0.3.2/gswidgetkit.egg-info/
--rw-rw-rw-   0        0        0      826 2023-01-27 15:06:27.000000 gswidgetkit-0.3.2/gswidgetkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      678 2023-01-27 15:06:27.000000 gswidgetkit-0.3.2/gswidgetkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-27 15:06:27.000000 gswidgetkit-0.3.2/gswidgetkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-01-27 15:06:27.000000 gswidgetkit-0.3.2/gswidgetkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-01-27 15:06:27.000000 gswidgetkit-0.3.2/gswidgetkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-01-27 15:06:28.047587 gswidgetkit-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      955 2023-01-27 15:05:53.000000 gswidgetkit-0.3.2/setup.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-06-02 18:03:59.369795 gswidgetkit-0.3.3/
+-rw-rw-r--   0 noah      (1000) noah      (1000)    11356 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/LICENSE
+-rw-r--r--   0 noah      (1000) noah      (1000)      939 2024-06-02 18:03:59.369795 gswidgetkit-0.3.3/PKG-INFO
+-rw-rw-r--   0 noah      (1000) noah      (1000)     2546 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/README.md
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-06-02 18:03:59.369795 gswidgetkit-0.3.3/gswidgetkit/
+-rw-rw-r--   0 noah      (1000) noah      (1000)      545 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/__init__.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)    10464 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/buttons.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)    20970 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/checkbox.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     5628 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/color_picker.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1001 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/constants.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     7401 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/dropdown.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)    79283 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/foldpanelbar.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-06-02 18:03:59.369795 gswidgetkit-0.3.3/gswidgetkit/icons/
+-rw-rw-r--   0 noah      (1000) noah      (1000)       21 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/icons/__init__.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)    10507 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/icons/icons.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1787 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/label.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)    14177 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/number_field.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)      348 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/panel.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1094 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/popups.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)      764 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/scrollbar.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     7933 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/textctrl.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)    17113 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/tooltip.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)      903 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/utils.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     2935 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/z_matrix.py
+-rw-rw-r--   0 noah      (1000) noah      (1000)     6367 2024-06-02 17:59:37.000000 gswidgetkit-0.3.3/gswidgetkit/zoom_panel.py
+drwxrwxr-x   0 noah      (1000) noah      (1000)        0 2024-06-02 18:03:59.369795 gswidgetkit-0.3.3/gswidgetkit.egg-info/
+-rw-r--r--   0 noah      (1000) noah      (1000)      939 2024-06-02 18:03:59.000000 gswidgetkit-0.3.3/gswidgetkit.egg-info/PKG-INFO
+-rw-rw-r--   0 noah      (1000) noah      (1000)      678 2024-06-02 18:03:59.000000 gswidgetkit-0.3.3/gswidgetkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)        1 2024-06-02 18:03:59.000000 gswidgetkit-0.3.3/gswidgetkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)       16 2024-06-02 18:03:59.000000 gswidgetkit-0.3.3/gswidgetkit.egg-info/requires.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)       12 2024-06-02 18:03:59.000000 gswidgetkit-0.3.3/gswidgetkit.egg-info/top_level.txt
+-rw-rw-r--   0 noah      (1000) noah      (1000)       79 2024-06-02 18:03:59.369795 gswidgetkit-0.3.3/setup.cfg
+-rw-rw-r--   0 noah      (1000) noah      (1000)     1018 2024-06-02 18:03:18.000000 gswidgetkit-0.3.3/setup.py
```

### Comparing `gswidgetkit-0.3.2/LICENSE` & `gswidgetkit-0.3.3/LICENSE`

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

### Comparing `gswidgetkit-0.3.2/README.md` & `gswidgetkit-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gswidgetkit-0.3.2/gswidgetkit/__init__.py` & `gswidgetkit-0.3.3/gswidgetkit/__init__.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from .number_field import (NumberField, EVT_NUMBERFIELD,
-                           EVT_NUMBERFIELD_CHANGE)
-from .buttons import Button, EVT_BUTTON
-from .color_picker import ColorPickerButton, EVT_COLORPICKER_BUTTON
-from .textctrl import TextCtrl, NativeTextCtrl, StyledTextCtrl
-from .checkbox import CheckBox
-from .tooltip import ToolTip
-from .dropdown import DropDown, EVT_DROPDOWN
-from .label import Label
-from .utils import GetTextExtent
-from .zoom_panel import ZoomPanel
-from .foldpanelbar import FoldPanelBar
-from .z_matrix import ZMatrix
+from .number_field import (NumberField, EVT_NUMBERFIELD,
+                           EVT_NUMBERFIELD_CHANGE)
+from .buttons import Button, EVT_BUTTON
+from .color_picker import ColorPickerButton, EVT_COLORPICKER_BUTTON
+from .textctrl import TextCtrl, NativeTextCtrl, StyledTextCtrl
+from .checkbox import CheckBox
+from .tooltip import ToolTip
+from .dropdown import DropDown, EVT_DROPDOWN
+from .label import Label
+from .utils import GetTextExtent
+from .zoom_panel import ZoomPanel
+from .foldpanelbar import FoldPanelBar
+from .z_matrix import ZMatrix
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/buttons.py` & `gswidgetkit-0.3.3/gswidgetkit/buttons.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,307 +1,307 @@
-# ----------------------------------------------------------------------------
-# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
-from wx.lib.newevent import NewCommandEvent
-
-from .constants import TEXT_COLOR, ACCENT_COLOR, BUTTON_BG_COLOR
-
-button_cmd_event, EVT_BUTTON = NewCommandEvent()
-
-
-class Button(wx.Control):
-    """ 
-    Button with support for the following combinations:
-    1. text
-    2. icon + text
-    3. icon
-
-    :param wx.Window `parent`: parent window. Must not be ``None``.
-    :param integer `id`: window identifier. A value of -1 indicates a default value.
-    :param string `label`: the displayed button label.
-    :param tuple `bmp`: the button icon as (wx.Bitmap, pos). pos can be one of 'top', 'left', 'right', 'bottom'.
-    :param bool `center`: if True the contents of the button will be centered rather than left-aligned.
-    :param bool `flat`: if True, the background will take on the color of the parent window.
-    """
-    def __init__(self, parent, id=wx.ID_ANY, label="", bmp=None, center=True,
-                 flat=False, pos=wx.DefaultPosition, size=wx.DefaultSize,
-                 style=wx.NO_BORDER, *args, **kwargs):
-        wx.Control.__init__(self, parent, id, pos, size, style, *args, **kwargs)
-
-        self.parent = parent
-
-        # Add spaces around a button with text
-        if label != "":
-            self.label = " {} ".format(label)
-            self.padding = (10, 20, 10, 20)
-        else:
-            # Icon button
-            self.label = label
-            self.padding = (5, 6, 5, 6)
-
-        self.buffer = None
-        self.center = center
-        self.flat = flat
-        self.outer_padding = 4
-        self.size = None
-        self.bmp = bmp
-
-        self.mouse_in = False
-        self.mouse_down = False
-        self.focused = False
-        self.highlighted = False
-
-        self.Bind(wx.EVT_PAINT, self.OnPaint)
-        self.Bind(wx.EVT_ERASE_BACKGROUND, lambda x: None)
-        self.Bind(wx.EVT_SET_FOCUS, self.OnSetFocus)
-        self.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
-        self.Bind(wx.EVT_LEAVE_WINDOW, self.OnMouseLeave)
-        self.Bind(wx.EVT_ENTER_WINDOW, self.OnMouseEnter)
-        self.Bind(wx.EVT_LEFT_DOWN, self.OnMouseDown)
-        self.Bind(wx.EVT_LEFT_UP, self.OnMouseUp)
-        self.Bind(wx.EVT_SIZE, self.OnSize)
-
-    def OnPaint(self, event):
-        wx.BufferedPaintDC(self, self.buffer)
-
-    def OnSize(self, event):
-        size = self.GetClientSize()
-
-        # Make sure size is at least 1px to avoid
-        # strange "invalid bitmap size" errors.
-        if size[0] < 1:
-            size = (1, 1)
-        self.buffer = wx.Bitmap(*size)
-        self.UpdateDrawing()
-
-    def UpdateDrawing(self):
-        dc = wx.MemoryDC()
-        dc.SelectObject(self.buffer)
-        dc = wx.GCDC(dc)
-        self.OnDrawBackground(dc)
-        self.OnDrawWidget(dc)
-        del dc  # need to get rid of the MemoryDC before Update() is called.
-        self.Refresh()
-        self.Update()
-
-    def OnDrawBackground(self, dc):
-        dc.SetBackground(wx.Brush(self.parent.GetBackgroundColour()))
-        dc.Clear()
-
-    def OnDrawWidget(self, dc):
-        fnt = self.parent.GetFont()
-        dc.SetFont(fnt)
-        dc.SetPen(wx.TRANSPARENT_PEN)
-
-        w, h = self.GetSize()
-
-        if self.mouse_down or self.highlighted:
-            dc.SetBrush(wx.Brush(wx.Colour(ACCENT_COLOR)))
-
-        elif self.mouse_in:
-            if self.flat is True:
-                color = self.parent.GetBackgroundColour().ChangeLightness(110)
-            else:
-                color = wx.Colour(BUTTON_BG_COLOR)
-            dc.SetBrush(wx.Brush(color))
-
-        else:
-            if self.flat is True:
-                color = self.parent.GetBackgroundColour()
-            else:
-                color = wx.Colour(BUTTON_BG_COLOR).ChangeLightness(85)
-            dc.SetBrush(wx.Brush(color))
-
-        dc.DrawRoundedRectangle(0, 0, w, h, 4)
-
-        txt_w, txt_h = dc.GetTextExtent(self.label)
-
-        if self.bmp is not None:
-            bmp = self.bmp
-            bmp_w, bmp_h = bmp[0].GetSize()
-            position = bmp[1]
-        else:
-            bmp = False
-
-        if bmp:
-
-            if position == "left":
-                if self.center:
-                    bmp_x = (w - txt_w - bmp_w) / 2
-                    bmp_y = (h - bmp_h) / 2
-
-                    txt_x = (w - txt_w - bmp_w) / 2 + bmp_w
-                    txt_y = (h - txt_h) / 2
-                else:
-                    bmp_x = self.padding[3]
-                    bmp_y = self.padding[0]
-
-                    txt_x = self.padding[3] + bmp_w
-                    if bmp_h > txt_h:
-                        txt_y = (bmp_h - txt_h) / 2 + self.padding[0]
-                    else:
-                        txt_y = self.padding[0]
-
-            if position == "right":
-                if self.center:
-                    bmp_x = (w - txt_w - bmp_w) / 2 + txt_w
-                    bmp_y = (h - bmp_h) / 2
-
-                    txt_x = (w - txt_w - bmp_w) / 2
-                    txt_y = (h - txt_h) / 2
-                else:
-                    bmp_x = self.padding[3] + txt_w
-                    bmp_y = self.padding[0]
-
-                    txt_x = self.padding[3]
-                    if bmp_h > txt_h:
-                        txt_y = (bmp_h - txt_h) / 2 + self.padding[0]
-                    else:
-                        txt_y = self.padding[0]
-
-            elif position == "top":
-                if self.center:
-                    bmp_x = (w - bmp_w) / 2
-                    bmp_y = (h - bmp_h - txt_h) / 2
-
-                    txt_x = (w - txt_w) / 2
-                    txt_y = (h - bmp_h - txt_h) / 2 + bmp_h
-                else:
-                    if bmp_w > txt_w:
-                        bmp_x = self.padding[3]
-                        bmp_y = self.padding[0]
-
-                        txt_x = (bmp_w - txt_w) / 2 + self.padding[3]
-                        txt_y = self.padding[0] + bmp_h
-                    else:
-                        bmp_x = (txt_w - bmp_w) / 2 + self.padding[3]
-                        bmp_y = self.padding[0]
-
-                        txt_x = self.padding[3]
-                        txt_y = self.padding[0] + bmp_h
-
-            elif position == "bottom":
-                if self.center:
-                    bmp_x = (w - bmp_w) / 2
-                    bmp_y = (h - txt_h - bmp_h) / 2 + txt_h
-
-                    txt_x = (w - txt_w) / 2
-                    txt_y = (h - txt_h - bmp_h) / 2
-                else:
-                    if bmp_w > txt_w:
-                        bmp_x = self.padding[3]
-                        bmp_y = self.padding[0] + txt_h
-
-                        txt_x = (bmp_w - txt_w) / 2 + self.padding[3]
-                        txt_y = self.padding[0]
-                    else:
-                        bmp_x = (txt_w - bmp_w) / 2 + self.padding[3]
-                        bmp_y = self.padding[0] + txt_h
-
-                        txt_x = self.padding[3]
-                        txt_y = self.padding[0]
-
-            dc.DrawBitmap(bmp[0], int(bmp_x), int(bmp_y))
-        else:
-            if self.center:
-                txt_x = (w - txt_w) / 2
-                txt_y = (h - txt_h) / 2
-            else:
-                txt_x = self.padding[3]
-                txt_y = self.padding[0]
-
-        # Text color
-        if self.mouse_down or self.focused or self.mouse_in:
-            color = wx.Colour(TEXT_COLOR).ChangeLightness(120)
-        else:
-            color = wx.Colour(TEXT_COLOR)
-
-        dc.SetTextForeground(color)
-
-        # Draw text
-        dc.DrawText(self.label, int(txt_x), int(txt_y))
-
-    def OnSetFocus(self, event):
-        self.focused = True
-        self.Refresh()
-
-    def OnKillFocus(self, event):
-        self.focused = False
-        self.Refresh()
-
-    def OnMouseEnter(self, event):
-        self.mouse_in = True
-        self.UpdateDrawing()
-
-    def OnMouseLeave(self, event):
-        self.mouse_in = False
-        self.UpdateDrawing()
-
-    def OnMouseDown(self, event):
-        self.mouse_down = True
-        self.SetFocus()
-        self.UpdateDrawing()
-
-    def OnMouseUp(self, event):
-        self.mouse_down = False
-        self.SendButtonEvent()
-        self.UpdateDrawing()
-
-    def SendButtonEvent(self):
-        wx.PostEvent(self, button_cmd_event(id=self.GetId(), value=0))
-
-    def SetHighlighted(self, highlighted=True):
-        self.highlighted = highlighted
-        try:
-            self.UpdateDrawing()
-        except Exception:
-            pass
-
-    def DoGetBestSize(self):
-        font = wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT)
-
-        dc = wx.ClientDC(self)
-        dc.SetFont(font)
-
-        txt_w, txt_h = dc.GetTextExtent(self.label)
-
-        if self.bmp is not None:
-            bmp = self.bmp
-            bmp_w, bmp_h = bmp[0].GetSize()
-            position = bmp[1]
-        else:
-            bmp = False
-
-        if bmp:
-            if position == "left" or position == "right":
-                if bmp_h > txt_h:
-                    size = (self.padding[3] + bmp_w + txt_w + self.padding[1],
-                            self.padding[0] + bmp_h + self.padding[2])
-                else:
-                    size = (self.padding[3] + bmp_w + txt_w + self.padding[1],
-                            self.padding[0] + txt_h + self.padding[2])
-            else:
-                if bmp_w > txt_w:
-                    size = (self.padding[3] + bmp_w + self.padding[1],
-                            self.padding[0] + bmp_h + txt_h + self.padding[2])
-                else:
-                    size = (self.padding[3] + txt_w + self.padding[1],
-                            self.padding[0] + bmp_h + txt_h + self.padding[2])
-        else:
-            size = (self.padding[3] + txt_w + self.padding[1],
-                    self.padding[0] + txt_h + self.padding[2])
-
-        return wx.Size(size)
+# ----------------------------------------------------------------------------
+# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
+from wx.lib.newevent import NewCommandEvent
+
+from .constants import TEXT_COLOR, ACCENT_COLOR, BUTTON_BG_COLOR
+
+button_cmd_event, EVT_BUTTON = NewCommandEvent()
+
+
+class Button(wx.Control):
+    """ 
+    Button with support for the following combinations:
+    1. text
+    2. icon + text
+    3. icon
+
+    :param wx.Window `parent`: parent window. Must not be ``None``.
+    :param integer `id`: window identifier. A value of -1 indicates a default value.
+    :param string `label`: the displayed button label.
+    :param tuple `bmp`: the button icon as (wx.Bitmap, pos). pos can be one of 'top', 'left', 'right', 'bottom'.
+    :param bool `center`: if True the contents of the button will be centered rather than left-aligned.
+    :param bool `flat`: if True, the background will take on the color of the parent window.
+    """
+    def __init__(self, parent, id=wx.ID_ANY, label="", bmp=None, center=True,
+                 flat=False, pos=wx.DefaultPosition, size=wx.DefaultSize,
+                 style=wx.NO_BORDER, *args, **kwargs):
+        wx.Control.__init__(self, parent, id, pos, size, style, *args, **kwargs)
+
+        self.parent = parent
+
+        # Add spaces around a button with text
+        if label != "":
+            self.label = " {} ".format(label)
+            self.padding = (10, 20, 10, 20)
+        else:
+            # Icon button
+            self.label = label
+            self.padding = (5, 6, 5, 6)
+
+        self.buffer = None
+        self.center = center
+        self.flat = flat
+        self.outer_padding = 4
+        self.size = None
+        self.bmp = bmp
+
+        self.mouse_in = False
+        self.mouse_down = False
+        self.focused = False
+        self.highlighted = False
+
+        self.Bind(wx.EVT_PAINT, self.OnPaint)
+        self.Bind(wx.EVT_ERASE_BACKGROUND, lambda x: None)
+        self.Bind(wx.EVT_SET_FOCUS, self.OnSetFocus)
+        self.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
+        self.Bind(wx.EVT_LEAVE_WINDOW, self.OnMouseLeave)
+        self.Bind(wx.EVT_ENTER_WINDOW, self.OnMouseEnter)
+        self.Bind(wx.EVT_LEFT_DOWN, self.OnMouseDown)
+        self.Bind(wx.EVT_LEFT_UP, self.OnMouseUp)
+        self.Bind(wx.EVT_SIZE, self.OnSize)
+
+    def OnPaint(self, event):
+        wx.BufferedPaintDC(self, self.buffer)
+
+    def OnSize(self, event):
+        size = self.GetClientSize()
+
+        # Make sure size is at least 1px to avoid
+        # strange "invalid bitmap size" errors.
+        if size[0] < 1:
+            size = (1, 1)
+        self.buffer = wx.Bitmap(*size)
+        self.UpdateDrawing()
+
+    def UpdateDrawing(self):
+        dc = wx.MemoryDC()
+        dc.SelectObject(self.buffer)
+        dc = wx.GCDC(dc)
+        self.OnDrawBackground(dc)
+        self.OnDrawWidget(dc)
+        del dc  # need to get rid of the MemoryDC before Update() is called.
+        self.Refresh()
+        self.Update()
+
+    def OnDrawBackground(self, dc):
+        dc.SetBackground(wx.Brush(self.parent.GetBackgroundColour()))
+        dc.Clear()
+
+    def OnDrawWidget(self, dc):
+        fnt = self.parent.GetFont()
+        dc.SetFont(fnt)
+        dc.SetPen(wx.TRANSPARENT_PEN)
+
+        w, h = self.GetSize()
+
+        if self.mouse_down or self.highlighted:
+            dc.SetBrush(wx.Brush(wx.Colour(ACCENT_COLOR)))
+
+        elif self.mouse_in:
+            if self.flat is True:
+                color = self.parent.GetBackgroundColour().ChangeLightness(110)
+            else:
+                color = wx.Colour(BUTTON_BG_COLOR)
+            dc.SetBrush(wx.Brush(color))
+
+        else:
+            if self.flat is True:
+                color = self.parent.GetBackgroundColour()
+            else:
+                color = wx.Colour(BUTTON_BG_COLOR).ChangeLightness(85)
+            dc.SetBrush(wx.Brush(color))
+
+        dc.DrawRoundedRectangle(0, 0, w, h, 4)
+
+        txt_w, txt_h = dc.GetTextExtent(self.label)
+
+        if self.bmp is not None:
+            bmp = self.bmp
+            bmp_w, bmp_h = bmp[0].GetSize()
+            position = bmp[1]
+        else:
+            bmp = False
+
+        if bmp:
+
+            if position == "left":
+                if self.center:
+                    bmp_x = (w - txt_w - bmp_w) / 2
+                    bmp_y = (h - bmp_h) / 2
+
+                    txt_x = (w - txt_w - bmp_w) / 2 + bmp_w
+                    txt_y = (h - txt_h) / 2
+                else:
+                    bmp_x = self.padding[3]
+                    bmp_y = self.padding[0]
+
+                    txt_x = self.padding[3] + bmp_w
+                    if bmp_h > txt_h:
+                        txt_y = (bmp_h - txt_h) / 2 + self.padding[0]
+                    else:
+                        txt_y = self.padding[0]
+
+            if position == "right":
+                if self.center:
+                    bmp_x = (w - txt_w - bmp_w) / 2 + txt_w
+                    bmp_y = (h - bmp_h) / 2
+
+                    txt_x = (w - txt_w - bmp_w) / 2
+                    txt_y = (h - txt_h) / 2
+                else:
+                    bmp_x = self.padding[3] + txt_w
+                    bmp_y = self.padding[0]
+
+                    txt_x = self.padding[3]
+                    if bmp_h > txt_h:
+                        txt_y = (bmp_h - txt_h) / 2 + self.padding[0]
+                    else:
+                        txt_y = self.padding[0]
+
+            elif position == "top":
+                if self.center:
+                    bmp_x = (w - bmp_w) / 2
+                    bmp_y = (h - bmp_h - txt_h) / 2
+
+                    txt_x = (w - txt_w) / 2
+                    txt_y = (h - bmp_h - txt_h) / 2 + bmp_h
+                else:
+                    if bmp_w > txt_w:
+                        bmp_x = self.padding[3]
+                        bmp_y = self.padding[0]
+
+                        txt_x = (bmp_w - txt_w) / 2 + self.padding[3]
+                        txt_y = self.padding[0] + bmp_h
+                    else:
+                        bmp_x = (txt_w - bmp_w) / 2 + self.padding[3]
+                        bmp_y = self.padding[0]
+
+                        txt_x = self.padding[3]
+                        txt_y = self.padding[0] + bmp_h
+
+            elif position == "bottom":
+                if self.center:
+                    bmp_x = (w - bmp_w) / 2
+                    bmp_y = (h - txt_h - bmp_h) / 2 + txt_h
+
+                    txt_x = (w - txt_w) / 2
+                    txt_y = (h - txt_h - bmp_h) / 2
+                else:
+                    if bmp_w > txt_w:
+                        bmp_x = self.padding[3]
+                        bmp_y = self.padding[0] + txt_h
+
+                        txt_x = (bmp_w - txt_w) / 2 + self.padding[3]
+                        txt_y = self.padding[0]
+                    else:
+                        bmp_x = (txt_w - bmp_w) / 2 + self.padding[3]
+                        bmp_y = self.padding[0] + txt_h
+
+                        txt_x = self.padding[3]
+                        txt_y = self.padding[0]
+
+            dc.DrawBitmap(bmp[0], int(bmp_x), int(bmp_y))
+        else:
+            if self.center:
+                txt_x = (w - txt_w) / 2
+                txt_y = (h - txt_h) / 2
+            else:
+                txt_x = self.padding[3]
+                txt_y = self.padding[0]
+
+        # Text color
+        if self.mouse_down or self.focused or self.mouse_in:
+            color = wx.Colour(TEXT_COLOR).ChangeLightness(120)
+        else:
+            color = wx.Colour(TEXT_COLOR)
+
+        dc.SetTextForeground(color)
+
+        # Draw text
+        dc.DrawText(self.label, int(txt_x), int(txt_y))
+
+    def OnSetFocus(self, event):
+        self.focused = True
+        self.Refresh()
+
+    def OnKillFocus(self, event):
+        self.focused = False
+        self.Refresh()
+
+    def OnMouseEnter(self, event):
+        self.mouse_in = True
+        self.UpdateDrawing()
+
+    def OnMouseLeave(self, event):
+        self.mouse_in = False
+        self.UpdateDrawing()
+
+    def OnMouseDown(self, event):
+        self.mouse_down = True
+        self.SetFocus()
+        self.UpdateDrawing()
+
+    def OnMouseUp(self, event):
+        self.mouse_down = False
+        self.SendButtonEvent()
+        self.UpdateDrawing()
+
+    def SendButtonEvent(self):
+        wx.PostEvent(self, button_cmd_event(id=self.GetId(), value=0))
+
+    def SetHighlighted(self, highlighted=True):
+        self.highlighted = highlighted
+        try:
+            self.UpdateDrawing()
+        except Exception:
+            pass
+
+    def DoGetBestSize(self):
+        font = wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT)
+
+        dc = wx.ClientDC(self)
+        dc.SetFont(font)
+
+        txt_w, txt_h = dc.GetTextExtent(self.label)
+
+        if self.bmp is not None:
+            bmp = self.bmp
+            bmp_w, bmp_h = bmp[0].GetSize()
+            position = bmp[1]
+        else:
+            bmp = False
+
+        if bmp:
+            if position == "left" or position == "right":
+                if bmp_h > txt_h:
+                    size = (self.padding[3] + bmp_w + txt_w + self.padding[1],
+                            self.padding[0] + bmp_h + self.padding[2])
+                else:
+                    size = (self.padding[3] + bmp_w + txt_w + self.padding[1],
+                            self.padding[0] + txt_h + self.padding[2])
+            else:
+                if bmp_w > txt_w:
+                    size = (self.padding[3] + bmp_w + self.padding[1],
+                            self.padding[0] + bmp_h + txt_h + self.padding[2])
+                else:
+                    size = (self.padding[3] + txt_w + self.padding[1],
+                            self.padding[0] + bmp_h + txt_h + self.padding[2])
+        else:
+            size = (self.padding[3] + txt_w + self.padding[1],
+                    self.padding[0] + txt_h + self.padding[2])
+
+        return wx.Size(size)
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/checkbox.py` & `gswidgetkit-0.3.3/gswidgetkit/checkbox.py`

 * *Files identical despite different names*

### Comparing `gswidgetkit-0.3.2/gswidgetkit/color_picker.py` & `gswidgetkit-0.3.3/gswidgetkit/color_picker.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-# ----------------------------------------------------------------------------
-# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
-from wx.lib.newevent import NewCommandEvent
-import wx.lib.agw.cubecolourdialog as colordialog
-
-from .constants import TEXT_COLOR
-from .icons import ICON_BRUSH_CHECKERBOARD
-
-button_cmd_event, EVT_COLORPICKER_BUTTON = NewCommandEvent()
-
-
-class ColorPickerButton(wx.Control):
-    """ 
-    Color picker widget for selecting an RGBA color.
-
-    :param wx.Window `parent`: parent window. Must not be ``None``.
-    :param integer `id`: window identifier. A value of -1 indicates a default value.
-    :param string `label`: the label displayed beside the color select button.
-    :param tuple `default`: tuple of the default RGBA color.
-    """
-    def __init__(self, parent, id=wx.ID_ANY, label="", default=(213, 219, 213, 177),
-                 pos=wx.DefaultPosition, size=wx.Size(400, -1), style=wx.NO_BORDER, 
-                 *args, **kwargs):
-        wx.Control.__init__(self, parent, id, pos, size, style, *args, **kwargs)
-
-        self.parent = parent
-
-        self.cur_color = default
-
-        self.label = label
-        self.padding = (5, 10, 5, 10)
- 
-        self.buffer = None
-        self.size = None
-
-        self.mouse_in = False
-        self.mouse_down = False
-        self.focused = False
-
-        self.Bind(wx.EVT_PAINT, self.OnPaint)
-        self.Bind(wx.EVT_ERASE_BACKGROUND, lambda x: None)
-        self.Bind(wx.EVT_SET_FOCUS, self.OnSetFocus)
-        self.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
-        self.Bind(wx.EVT_LEAVE_WINDOW, self.OnMouseLeave)
-        self.Bind(wx.EVT_ENTER_WINDOW, self.OnMouseEnter)
-        self.Bind(wx.EVT_LEFT_DOWN, self.OnMouseDown)
-        self.Bind(wx.EVT_LEFT_UP, self.OnMouseUp)
-        self.Bind(wx.EVT_SIZE, self.OnSize)
-
-    def OnPaint(self, event):
-        wx.BufferedPaintDC(self, self.buffer)
-
-    def OnSize(self, event):
-        size = self.GetClientSize()
-
-        # Make sure size is at least 1px to avoid
-        # strange "invalid bitmap size" errors.
-        if size[0] < 1:
-            size = (1, 1)
-        self.buffer = wx.Bitmap(*size)
-        self.UpdateDrawing()
-
-    def UpdateDrawing(self):
-        dc = wx.MemoryDC()
-        dc.SelectObject(self.buffer)
-        dc = wx.GCDC(dc)
-        self.OnDrawBackground(dc)
-        self.OnDrawWidget(dc)
-        del dc  # need to get rid of the MemoryDC before Update() is called.
-        self.Refresh()
-        self.Update()
-
-    def OnDrawBackground(self, dc):
-        dc.SetBackground(wx.Brush(self.parent.GetBackgroundColour()))
-        dc.Clear()
-
-    def OnDrawWidget(self, dc):
-        fnt = self.parent.GetFont()
-        dc.SetFont(fnt)
-        dc.SetPen(wx.TRANSPARENT_PEN)
-
-        w, h = self.GetSize()
-
-        txt_w, txt_h = dc.GetTextExtent(self.label)
-
-        txt_x = self.padding[3]
-        txt_y = self.padding[0]
-
-        txt_w = txt_w + self.padding[1] + self.padding[3]
-
-        dc.SetBrush(wx.Brush(ICON_BRUSH_CHECKERBOARD.GetBitmap()))
-        dc.DrawRoundedRectangle(txt_w, 0, w-txt_w, h, 4)
-
-        dc.SetBrush(wx.Brush(wx.Colour(self.cur_color)))
-        dc.DrawRoundedRectangle(txt_w, 0, w-txt_w, h, 4)
-
-        # Draw text
-        if self.mouse_down or self.focused or self.mouse_in:
-            color = wx.Colour(TEXT_COLOR).ChangeLightness(120)
-        else:
-            color = wx.Colour(TEXT_COLOR)
-        dc.SetTextForeground(color)
-
-        dc.DrawText(self.label, int(txt_x), int(txt_y))
-
-    def OnSetFocus(self, event):
-        self.focused = True
-        self.Refresh()
-
-    def OnKillFocus(self, event):
-        self.focused = False
-        self.Refresh()
-
-    def OnMouseEnter(self, event):
-        self.mouse_in = True
-        self.UpdateDrawing()
-
-    def OnMouseLeave(self, event):
-        self.mouse_in = False
-        self.UpdateDrawing()
-
-    def OnMouseDown(self, event):
-        self.mouse_down = True
-        self.SetFocus()
-        self.UpdateDrawing()
-
-    def OnMouseUp(self, event):
-        self.mouse_down = False
-        self.ShowDialog()
-        self.SendButtonEvent()
-        self.UpdateDrawing()
-
-    def SendButtonEvent(self):
-        wx.PostEvent(self, button_cmd_event(id=self.GetId(), value=self.cur_color))
-
-    def ShowDialog(self):
-        self.color_data = wx.ColourData()
-        self.color_data.SetColour(self.cur_color)
-        self.color_dialog = colordialog.CubeColourDialog(None, self.color_data)
-        if self.color_dialog.ShowModal() == wx.ID_OK:
-            self.color_data = self.color_dialog.GetColourData()
-            self.cur_color = self.color_data.GetColour()
-        self.color_dialog.Destroy()
-
-    def DoGetBestSize(self):
-        font = wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT)
-
-        dc = wx.ClientDC(self)
-        dc.SetFont(font)
-
-        txt_w, txt_h = dc.GetTextExtent(self.label)
-
-        size = (self.padding[3] + txt_w + self.padding[1],
-                self.padding[0] + txt_h + self.padding[2])
-
-        return wx.Size(size)
+# ----------------------------------------------------------------------------
+# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
+from wx.lib.newevent import NewCommandEvent
+import wx.lib.agw.cubecolourdialog as colordialog
+
+from .constants import TEXT_COLOR
+from .icons import ICON_BRUSH_CHECKERBOARD
+
+button_cmd_event, EVT_COLORPICKER_BUTTON = NewCommandEvent()
+
+
+class ColorPickerButton(wx.Control):
+    """ 
+    Color picker widget for selecting an RGBA color.
+
+    :param wx.Window `parent`: parent window. Must not be ``None``.
+    :param integer `id`: window identifier. A value of -1 indicates a default value.
+    :param string `label`: the label displayed beside the color select button.
+    :param tuple `default`: tuple of the default RGBA color.
+    """
+    def __init__(self, parent, id=wx.ID_ANY, label="", default=(213, 219, 213, 177),
+                 pos=wx.DefaultPosition, size=wx.Size(400, -1), style=wx.NO_BORDER, 
+                 *args, **kwargs):
+        wx.Control.__init__(self, parent, id, pos, size, style, *args, **kwargs)
+
+        self.parent = parent
+
+        self.cur_color = default
+
+        self.label = label
+        self.padding = (5, 10, 5, 10)
+ 
+        self.buffer = None
+        self.size = None
+
+        self.mouse_in = False
+        self.mouse_down = False
+        self.focused = False
+
+        self.Bind(wx.EVT_PAINT, self.OnPaint)
+        self.Bind(wx.EVT_ERASE_BACKGROUND, lambda x: None)
+        self.Bind(wx.EVT_SET_FOCUS, self.OnSetFocus)
+        self.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
+        self.Bind(wx.EVT_LEAVE_WINDOW, self.OnMouseLeave)
+        self.Bind(wx.EVT_ENTER_WINDOW, self.OnMouseEnter)
+        self.Bind(wx.EVT_LEFT_DOWN, self.OnMouseDown)
+        self.Bind(wx.EVT_LEFT_UP, self.OnMouseUp)
+        self.Bind(wx.EVT_SIZE, self.OnSize)
+
+    def OnPaint(self, event):
+        wx.BufferedPaintDC(self, self.buffer)
+
+    def OnSize(self, event):
+        size = self.GetClientSize()
+
+        # Make sure size is at least 1px to avoid
+        # strange "invalid bitmap size" errors.
+        if size[0] < 1:
+            size = (1, 1)
+        self.buffer = wx.Bitmap(*size)
+        self.UpdateDrawing()
+
+    def UpdateDrawing(self):
+        dc = wx.MemoryDC()
+        dc.SelectObject(self.buffer)
+        dc = wx.GCDC(dc)
+        self.OnDrawBackground(dc)
+        self.OnDrawWidget(dc)
+        del dc  # need to get rid of the MemoryDC before Update() is called.
+        self.Refresh()
+        self.Update()
+
+    def OnDrawBackground(self, dc):
+        dc.SetBackground(wx.Brush(self.parent.GetBackgroundColour()))
+        dc.Clear()
+
+    def OnDrawWidget(self, dc):
+        fnt = self.parent.GetFont()
+        dc.SetFont(fnt)
+        dc.SetPen(wx.TRANSPARENT_PEN)
+
+        w, h = self.GetSize()
+
+        txt_w, txt_h = dc.GetTextExtent(self.label)
+
+        txt_x = self.padding[3]
+        txt_y = self.padding[0]
+
+        txt_w = txt_w + self.padding[1] + self.padding[3]
+
+        dc.SetBrush(wx.Brush(ICON_BRUSH_CHECKERBOARD.GetBitmap()))
+        dc.DrawRoundedRectangle(txt_w, 0, w-txt_w, h, 4)
+
+        dc.SetBrush(wx.Brush(wx.Colour(self.cur_color)))
+        dc.DrawRoundedRectangle(txt_w, 0, w-txt_w, h, 4)
+
+        # Draw text
+        if self.mouse_down or self.focused or self.mouse_in:
+            color = wx.Colour(TEXT_COLOR).ChangeLightness(120)
+        else:
+            color = wx.Colour(TEXT_COLOR)
+        dc.SetTextForeground(color)
+
+        dc.DrawText(self.label, int(txt_x), int(txt_y))
+
+    def OnSetFocus(self, event):
+        self.focused = True
+        self.Refresh()
+
+    def OnKillFocus(self, event):
+        self.focused = False
+        self.Refresh()
+
+    def OnMouseEnter(self, event):
+        self.mouse_in = True
+        self.UpdateDrawing()
+
+    def OnMouseLeave(self, event):
+        self.mouse_in = False
+        self.UpdateDrawing()
+
+    def OnMouseDown(self, event):
+        self.mouse_down = True
+        self.SetFocus()
+        self.UpdateDrawing()
+
+    def OnMouseUp(self, event):
+        self.mouse_down = False
+        self.ShowDialog()
+        self.SendButtonEvent()
+        self.UpdateDrawing()
+
+    def SendButtonEvent(self):
+        wx.PostEvent(self, button_cmd_event(id=self.GetId(), value=self.cur_color))
+
+    def ShowDialog(self):
+        self.color_data = wx.ColourData()
+        self.color_data.SetColour(self.cur_color)
+        self.color_dialog = colordialog.CubeColourDialog(None, self.color_data)
+        if self.color_dialog.ShowModal() == wx.ID_OK:
+            self.color_data = self.color_dialog.GetColourData()
+            self.cur_color = self.color_data.GetColour()
+        self.color_dialog.Destroy()
+
+    def DoGetBestSize(self):
+        font = wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT)
+
+        dc = wx.ClientDC(self)
+        dc.SetFont(font)
+
+        txt_w, txt_h = dc.GetTextExtent(self.label)
+
+        size = (self.padding[3] + txt_w + self.padding[1],
+                self.padding[0] + txt_h + self.padding[2])
+
+        return wx.Size(size)
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/constants.py` & `gswidgetkit-0.3.3/gswidgetkit/constants.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# ----------------------------------------------------------------------------
-# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
-TEXT_COLOR = "#dfdfdf"
-ACCENT_COLOR = "#3D7DC5"
-
-DROPDOWN_BG_COLOR = "#1B2226"
-NUMBERFIELD_BG_COLOR = "#1B2226"
-BUTTON_BG_COLOR = "#1B2226"
-TEXTCTRL_BG_COLOR = "#1B2226"
-TEXTCTRL_BORDER_COLOR = "#111517"
-FOLDPANEL_BG_COLOR = "#1E2429"
+# ----------------------------------------------------------------------------
+# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
+TEXT_COLOR = "#dfdfdf"
+ACCENT_COLOR = "#3D7DC5"
+
+DROPDOWN_BG_COLOR = "#1B2226"
+NUMBERFIELD_BG_COLOR = "#1B2226"
+BUTTON_BG_COLOR = "#1B2226"
+TEXTCTRL_BG_COLOR = "#1B2226"
+TEXTCTRL_BORDER_COLOR = "#111517"
+FOLDPANEL_BG_COLOR = "#1E2429"
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/dropdown.py` & `gswidgetkit-0.3.3/gswidgetkit/dropdown.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,218 +1,218 @@
-# ----------------------------------------------------------------------------
-# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
-import wx.lib.agw.flatmenu as flatmenu
-from wx.lib.newevent import NewCommandEvent
-
-from .constants import ACCENT_COLOR, TEXT_COLOR, DROPDOWN_BG_COLOR
-from .utils import GetTextExtent
-from .icons import ICON_DROPDOWN_ARROW
-
-# Max number of items that can be added to the menu is 100
-DROPDOWNMENU_ITEM_IDS = wx.NewIdRef(100)
-
-# Create new event for selecting dropdown item
-dropdown_cmd_event, EVT_DROPDOWN = NewCommandEvent()
-
-
-class DropDown(wx.Control):
-    """ 
-    Dropdown widget for selecting a value from a list of choices.
-
-    :param wx.Window `parent`: parent window. Must not be ``None``.
-    :param integer `id`: window identifier. A value of -1 indicates a default value.
-    :param list `items`: the list of items in the dropdown.
-    :param `default`: the default selected item in the dropdown. Must exist in `items`.
-    """
-    def __init__(self, parent, items, default, id=wx.ID_ANY,
-                 pos=wx.DefaultPosition, size=wx.DefaultSize,
-                 style=wx.NO_BORDER, *args,**kwargs):
-        wx.Control.__init__(self, parent, id, pos, size, style, *args, **kwargs)
-        self.parent = parent
-        self.items = items
-        self.default = default
-        self.value = default
-        self.longest_str = max(items, key=len)  # Longest string in the choices
-
-        self.buffer = None
-        self.padding_x = 20
-        self.padding_y = 10
-
-        self.mouse_in = False
-        self.mouse_down = False
-        self.focused = False
-
-        self.menuidmapping = {}
-
-        # Init menu
-        self.CreateMenu()
-
-        self.Bind(wx.EVT_PAINT, self.OnPaint)
-        self.Bind(wx.EVT_ERASE_BACKGROUND, lambda x: None)
-        self.Bind(wx.EVT_SET_FOCUS, self.OnSetFocus)
-        self.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
-        self.Bind(wx.EVT_LEAVE_WINDOW, self.OnMouseLeave)
-        self.Bind(wx.EVT_ENTER_WINDOW, self.OnMouseEnter)
-        self.Bind(wx.EVT_LEFT_DOWN, self.OnMouseDown)
-        self.Bind(wx.EVT_LEFT_UP, self.OnMouseUp)
-        self.Bind(wx.EVT_SIZE, self.OnSize)
-
-    def OnPaint(self, event):
-        wx.BufferedPaintDC(self, self.buffer)
-
-    def OnSize(self, event):
-        size = self.GetClientSize()
-
-        # Make sure size is at least 1px to avoid
-        # strange "invalid bitmap size" errors.
-        if size[0] < 1:
-            size = (1, 1)
-        self.buffer = wx.Bitmap(*size)
-        self.UpdateDrawing()
-
-    def UpdateDrawing(self):
-        dc = wx.MemoryDC()
-        dc.SelectObject(self.buffer)
-        dc = wx.GCDC(dc)
-        self.OnDrawBackground(dc)
-        self.OnDrawWidget(dc)
-        del dc  # need to get rid of the MemoryDC before Update() is called.
-        self.Refresh()
-        self.Update()
-
-    def OnDrawBackground(self, dc):
-        dc.SetBackground(wx.Brush(self.parent.GetBackgroundColour()))
-        dc.Clear()
-
-    def OnDrawWidget(self, dc):
-        fnt = self.parent.GetFont()
-        dc.SetFont(fnt)
-        dc.SetTextForeground(TEXT_COLOR)
-        dc.SetPen(wx.TRANSPARENT_PEN)
-
-        w, h = self.GetSize()
-        lbl_w, lbl_h = GetTextExtent(self.GetValue())
-
-        if self.mouse_down:
-            bg_color = wx.Colour(ACCENT_COLOR)
-        elif self.mouse_in:
-            bg_color = wx.Colour(DROPDOWN_BG_COLOR)
-        else:
-            bg_color = wx.Colour(DROPDOWN_BG_COLOR).ChangeLightness(85)
-
-        dc.SetBrush(wx.Brush(bg_color))
-        dc.DrawRoundedRectangle(0, 0, w, h, 4)
-        dc.DrawText(self.GetValue(), self.padding_x, int((h/2) - (lbl_h/2)))
-        dc.DrawBitmap(ICON_DROPDOWN_ARROW.GetBitmap(), (w-28), int((h/2) - (lbl_h/2) - 2))
-
-    def OnSetFocus(self, event):
-        self.focused = True
-        self.Refresh()
-
-    def OnKillFocus(self, event):
-        self.focused = False
-        self.Refresh()
-
-    def OnMouseEnter(self, event):
-        self.mouse_in = True
-        self.UpdateDrawing()
-
-    def OnMouseLeave(self, event):
-        self.mouse_in = False
-        self.UpdateDrawing()
-
-    def OnMouseDown(self, event):
-        self.mouse_down = True
-        self.SetFocus()
-        self.UpdateDrawing()
-
-    def OnMouseUp(self, event):
-        self.mouse_down = False
-        self.OnClick()
-        self.UpdateDrawing()
-
-    def DoGetBestSize(self):
-        """
-        Overridden base class virtual.  Determines the best size of the control
-        based on the label size, the bitmap size and the current font.
-        """
-        font = wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT)
-        dc = wx.ClientDC(self)
-        dc.SetFont(font)
-
-        val_text_w, val_text_h = dc.GetTextExtent(self.longest_str)
-
-        totalwidth = val_text_w + self.padding_x + 65
-
-        totalheight = val_text_h + self.padding_y
-
-        best = wx.Size(totalwidth, totalheight)
-
-        # Cache the best size so it doesn't need to be calculated again,
-        # at least until some properties of the window change
-        self.CacheBestSize(best)
-
-        return best
-
-    def SetValue(self, value):
-        self.value = value
-
-    def GetValue(self):
-        return self.value
-
-    def ComputeMenuPos(self):
-        y = self.GetSize()[1] + self.GetScreenPosition()[1] + 1
-        x = self.GetScreenPosition()[0]
-        return wx.Point(x, y)
-
-    def OnClick(self):
-        # Set the size of the menu
-        w, h = self.GetSize()
-        self.dropdown_menu._menuWidth = w
-        h = (self.dropdown_menu._itemHeight)*(len(self.items))+4
-        self.dropdown_menu.SetSize(wx.Size(w, h))
-        
-        # Popup the menu
-        pos = self.ComputeMenuPos()
-        self.dropdown_menu.Popup(pos, self)
-
-    def SendDropdownSelectEvent(self):
-        wx.PostEvent(self, dropdown_cmd_event(id=self.GetId(), value=self.GetValue()))
-
-    def CreateMenu(self):
-        self.dropdown_menu = flatmenu.FlatMenu()
-
-        # Make the margin width to be the same as in the dropdown button
-        # and the margin height to be consistent with standards.
-        self.dropdown_menu._marginWidth = 10
-        self.dropdown_menu._marginHeight = 26
-
-        i = 0
-        for item in self.items:
-            menu_item = flatmenu.FlatMenuItem(self.dropdown_menu,
-                                              DROPDOWNMENU_ITEM_IDS[i],
-                                              item, "", wx.ITEM_NORMAL)
-            self.dropdown_menu.AppendItem(menu_item)
-            self.menuidmapping[DROPDOWNMENU_ITEM_IDS[i]] = item
-
-            self.Bind(wx.EVT_MENU, self.OnSelectMenuItem, id=DROPDOWNMENU_ITEM_IDS[i])
-            i += 1
-
-    def OnSelectMenuItem(self, event):
-        self.SetValue(self.menuidmapping[event.GetId()])
-        self.SendDropdownSelectEvent()
-        self.UpdateDrawing()
+# ----------------------------------------------------------------------------
+# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
+import wx.lib.agw.flatmenu as flatmenu
+from wx.lib.newevent import NewCommandEvent
+
+from .constants import ACCENT_COLOR, TEXT_COLOR, DROPDOWN_BG_COLOR
+from .utils import GetTextExtent
+from .icons import ICON_DROPDOWN_ARROW
+
+# Max number of items that can be added to the menu is 100
+DROPDOWNMENU_ITEM_IDS = wx.NewIdRef(100)
+
+# Create new event for selecting dropdown item
+dropdown_cmd_event, EVT_DROPDOWN = NewCommandEvent()
+
+
+class DropDown(wx.Control):
+    """ 
+    Dropdown widget for selecting a value from a list of choices.
+
+    :param wx.Window `parent`: parent window. Must not be ``None``.
+    :param integer `id`: window identifier. A value of -1 indicates a default value.
+    :param list `items`: the list of items in the dropdown.
+    :param `default`: the default selected item in the dropdown. Must exist in `items`.
+    """
+    def __init__(self, parent, items, default, id=wx.ID_ANY,
+                 pos=wx.DefaultPosition, size=wx.DefaultSize,
+                 style=wx.NO_BORDER, *args,**kwargs):
+        wx.Control.__init__(self, parent, id, pos, size, style, *args, **kwargs)
+        self.parent = parent
+        self.items = items
+        self.default = default
+        self.value = default
+        self.longest_str = max(items, key=len)  # Longest string in the choices
+
+        self.buffer = None
+        self.padding_x = 20
+        self.padding_y = 10
+
+        self.mouse_in = False
+        self.mouse_down = False
+        self.focused = False
+
+        self.menuidmapping = {}
+
+        # Init menu
+        self.CreateMenu()
+
+        self.Bind(wx.EVT_PAINT, self.OnPaint)
+        self.Bind(wx.EVT_ERASE_BACKGROUND, lambda x: None)
+        self.Bind(wx.EVT_SET_FOCUS, self.OnSetFocus)
+        self.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
+        self.Bind(wx.EVT_LEAVE_WINDOW, self.OnMouseLeave)
+        self.Bind(wx.EVT_ENTER_WINDOW, self.OnMouseEnter)
+        self.Bind(wx.EVT_LEFT_DOWN, self.OnMouseDown)
+        self.Bind(wx.EVT_LEFT_UP, self.OnMouseUp)
+        self.Bind(wx.EVT_SIZE, self.OnSize)
+
+    def OnPaint(self, event):
+        wx.BufferedPaintDC(self, self.buffer)
+
+    def OnSize(self, event):
+        size = self.GetClientSize()
+
+        # Make sure size is at least 1px to avoid
+        # strange "invalid bitmap size" errors.
+        if size[0] < 1:
+            size = (1, 1)
+        self.buffer = wx.Bitmap(*size)
+        self.UpdateDrawing()
+
+    def UpdateDrawing(self):
+        dc = wx.MemoryDC()
+        dc.SelectObject(self.buffer)
+        dc = wx.GCDC(dc)
+        self.OnDrawBackground(dc)
+        self.OnDrawWidget(dc)
+        del dc  # need to get rid of the MemoryDC before Update() is called.
+        self.Refresh()
+        self.Update()
+
+    def OnDrawBackground(self, dc):
+        dc.SetBackground(wx.Brush(self.parent.GetBackgroundColour()))
+        dc.Clear()
+
+    def OnDrawWidget(self, dc):
+        fnt = self.parent.GetFont()
+        dc.SetFont(fnt)
+        dc.SetTextForeground(TEXT_COLOR)
+        dc.SetPen(wx.TRANSPARENT_PEN)
+
+        w, h = self.GetSize()
+        lbl_w, lbl_h = GetTextExtent(self.GetValue())
+
+        if self.mouse_down:
+            bg_color = wx.Colour(ACCENT_COLOR)
+        elif self.mouse_in:
+            bg_color = wx.Colour(DROPDOWN_BG_COLOR)
+        else:
+            bg_color = wx.Colour(DROPDOWN_BG_COLOR).ChangeLightness(85)
+
+        dc.SetBrush(wx.Brush(bg_color))
+        dc.DrawRoundedRectangle(0, 0, w, h, 4)
+        dc.DrawText(self.GetValue(), self.padding_x, int((h/2) - (lbl_h/2)))
+        dc.DrawBitmap(ICON_DROPDOWN_ARROW.GetBitmap(), (w-28), int((h/2) - (lbl_h/2) - 2))
+
+    def OnSetFocus(self, event):
+        self.focused = True
+        self.Refresh()
+
+    def OnKillFocus(self, event):
+        self.focused = False
+        self.Refresh()
+
+    def OnMouseEnter(self, event):
+        self.mouse_in = True
+        self.UpdateDrawing()
+
+    def OnMouseLeave(self, event):
+        self.mouse_in = False
+        self.UpdateDrawing()
+
+    def OnMouseDown(self, event):
+        self.mouse_down = True
+        self.SetFocus()
+        self.UpdateDrawing()
+
+    def OnMouseUp(self, event):
+        self.mouse_down = False
+        self.OnClick()
+        self.UpdateDrawing()
+
+    def DoGetBestSize(self):
+        """
+        Overridden base class virtual.  Determines the best size of the control
+        based on the label size, the bitmap size and the current font.
+        """
+        font = wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT)
+        dc = wx.ClientDC(self)
+        dc.SetFont(font)
+
+        val_text_w, val_text_h = dc.GetTextExtent(self.longest_str)
+
+        totalwidth = val_text_w + self.padding_x + 65
+
+        totalheight = val_text_h + self.padding_y
+
+        best = wx.Size(totalwidth, totalheight)
+
+        # Cache the best size so it doesn't need to be calculated again,
+        # at least until some properties of the window change
+        self.CacheBestSize(best)
+
+        return best
+
+    def SetValue(self, value):
+        self.value = value
+
+    def GetValue(self):
+        return self.value
+
+    def ComputeMenuPos(self):
+        y = self.GetSize()[1] + self.GetScreenPosition()[1] + 1
+        x = self.GetScreenPosition()[0]
+        return wx.Point(x, y)
+
+    def OnClick(self):
+        # Set the size of the menu
+        w, h = self.GetSize()
+        self.dropdown_menu._menuWidth = w
+        h = (self.dropdown_menu._itemHeight)*(len(self.items))+4
+        self.dropdown_menu.SetSize(wx.Size(w, h))
+        
+        # Popup the menu
+        pos = self.ComputeMenuPos()
+        self.dropdown_menu.Popup(pos, self)
+
+    def SendDropdownSelectEvent(self):
+        wx.PostEvent(self, dropdown_cmd_event(id=self.GetId(), value=self.GetValue()))
+
+    def CreateMenu(self):
+        self.dropdown_menu = flatmenu.FlatMenu()
+
+        # Make the margin width to be the same as in the dropdown button
+        # and the margin height to be consistent with standards.
+        self.dropdown_menu._marginWidth = 10
+        self.dropdown_menu._marginHeight = 26
+
+        i = 0
+        for item in self.items:
+            menu_item = flatmenu.FlatMenuItem(self.dropdown_menu,
+                                              DROPDOWNMENU_ITEM_IDS[i],
+                                              item, "", wx.ITEM_NORMAL)
+            self.dropdown_menu.AppendItem(menu_item)
+            self.menuidmapping[DROPDOWNMENU_ITEM_IDS[i]] = item
+
+            self.Bind(wx.EVT_MENU, self.OnSelectMenuItem, id=DROPDOWNMENU_ITEM_IDS[i])
+            i += 1
+
+    def OnSelectMenuItem(self, event):
+        self.SetValue(self.menuidmapping[event.GetId()])
+        self.SendDropdownSelectEvent()
+        self.UpdateDrawing()
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/foldpanelbar.py` & `gswidgetkit-0.3.3/gswidgetkit/foldpanelbar.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,2299 +1,2299 @@
-# --------------------------------------------------------------------------- #
-# FOLDPANELBAR wxPython IMPLEMENTATION
-# Ported From Jorgen Bodde & Julian Smart (Extended Demo) C++ Code By:
-#
-# Andrea Gavana, @ 23 Mar 2005
-# Latest Revision: 16 Jul 2012, 15.00 GMT
-# 
-# Edited version in gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
-#
-# TODO List
-#
-# All The C++ TODOs Are Still Alive. I Am Not Able to Read Jorges's Mind
-# So I Don't Really Know What Will Be The New Features/Additions He Will
-# Make On His Code. At The Moment They Are:
-#
-# 1. OnPaint Function In CaptionBar Class:
-# TODO: Maybe First A Memory Dc Should Draw All, And Then Paint It On The
-# Caption. This Way A Flickering Arrow During Resize Is Not Visible.
-#
-# 2. OnChar Function In CaptionBar Class:
-# TODO: This Is Easy To Do But I Don't Have Any Useful Idea On Which Kind
-# Of Features To Add. Does Anyone Have An Intelligent Idea?
-#
-# 3. AddFoldPanelWindow Function In FoldPanelBar Class:
-# TODO: Take Old And New Heights, And If Difference, Reposition All The
-# Lower Panels. This Is Because The User Can Add New wxWindow Controls
-# Somewhere In Between When Other Panels Are Already Present.
-# Don't Know What It Means. Probably Is My Poor English...
-#
-# 4. OnSizePanel Function In FoldPanelBar Class:
-# TODO: A Smart Way To Check Wether The Old - New Width Of The
-# Panel Changed, If So No Need To Resize The Fold Panel Items
-#
-#
-# DONE List:
-#
-# 1. Implemented Styles Like FPB_SINGLE_FOLD and FPB_EXCLUSIVE_FOLD
-# Thanks To E. A. Tacao For His Nice Suggestions.
-#
-# 2. Added Some Maquillage To FoldPanelBar: When The Mouse Enters The Icon
-# Region, It Is Changed To wx.CURSOR_HAND.
-#
-#
-# For The Original TODO List From Jorgen, Please Refer To:
-# http://www.solidsteel.nl/jorg/components/foldpanel/wxFoldPanelBar.php#todo_list
-#
-#
-#
-# For All Kind Of Problems, Requests Of Enhancements And Bug Reports, Please
-# Write To Me At:
-#
-# andrea.gavana@gmail.com
-# andrea.gavana@maerskoil.com
-#
-# Or, Obviously, To The wxPython Mailing List!!!
-#
-# Tags:        phoenix-port, unittest, documented, py3-port
-#
-# End Of Comments
-# --------------------------------------------------------------------------- #
-
-
-"""
-:class:`~wx.lib.agw.foldpanelbar.FoldPanelBar` is a control that contains multiple panels, which can be expanded
-or collapsed.
-
-
-Description
-===========
-
-The :class:`FoldPanelBar` is a control that contains multiple panels (of type
-:class:`FoldPanelItem`) that can be expanded or collapsed. The captionbar of
-the :class:`FoldPanelBar` can be customized by setting it to a horizontal gradient
-style, vertical gradient style, a single colour, a rectangle or filled
-rectangle. The `FoldPanel` items can be collapsed in place or to the
-bottom of the control. :class:`wx.Window` derived controls can be added
-dynamically, and separated by separator lines.
-
-
-How does it work
-----------------
-
-The internals of the :class:`FoldPanelBar` is a list of :class:`FoldPanelItem` objects. Through
-the reference of `FoldPanel` these panels can be controlled by adding new controls
-to a FoldPanel or adding new FoldPanels to the :class:`FoldPanelBar`.
-
-The :class:`CaptionBar` fires events to the parent (container of all panel items) when a
-sub-panel needs resizing (either folding or expanding). The fold or expand process
-is simply a resize of the panel so it looks like all controls on it are gone. All
-controls are still child of the `FoldPanel` they are located on. If they don't
-handle the event (and they won't) then the owner of the :class:`FoldPanelBar` gets the
-events.
-
-This is what you need to handle the controls. There isn't much to it just
-a lot of calculations to see what panel belongs where. There are no sizers
-involved in the panels, everything is purely x-y positioning.
-
-
-What can it do and what not?
-----------------------------
-
-a) What it can do:
-
-   * Run-time addition of panels (no deletion just yet);
-   * Run time addition of controls to the panel (it will be resized accordingly);
-   * Creating panels in collapsed mode or expanded mode;
-   * Various modes of caption behaviour and filling to make it more appealing;
-   * Panels can be folded and collapsed (or all of them) to allow more space.
-
-b) What it cannot do:
-
-   * Selection of a panel like in a listctrl;
-   * Dragging and dropping the panels;
-   * Re-ordering the panels (not yet).
-
-
-Usage
-=====
-
-Usage example::
-
-    import wx
-    import wx.lib.agw.foldpanelbar as fpb
-
-    class MyFrame(wx.Frame):
-
-        def __init__(self, parent):
-
-            wx.Frame.__init__(self, parent, -1, "FoldPanelBar Demo")
-
-            text_ctrl = wx.TextCtrl(self, -1, size=(400, 100), style=wx.TE_MULTILINE)
-
-            panel_bar = fpb.FoldPanelBar(self, -1, agwStyle=fpb.FPB_VERTICAL)
-
-            fold_panel = panel_bar.AddFoldPanel("Thing")
-            thing = wx.TextCtrl(fold_panel, -1, size=(400, -1), style=wx.TE_MULTILINE)
-
-            panel_bar.AddFoldPanelWindow(fold_panel, thing)
-
-            main_sizer = wx.BoxSizer(wx.VERTICAL)
-            main_sizer.Add(text_ctrl, 1, wx.EXPAND)
-            main_sizer.Add(panel_bar, 1, wx.EXPAND)
-            self.SetSizer(main_sizer)
-
-
-    # our normal wxApp-derived class, as usual
-
-    app = wx.App(0)
-
-    frame = MyFrame(None)
-    app.SetTopWindow(frame)
-    frame.Show()
-
-    app.MainLoop()
-
-
-
-Supported Platforms
-===================
-
-:class:`FoldPanelBar` is supported on the following platforms:
-  * Windows (Verified on Windows XP, 2000)
-  * Linux/Unix (GTK2) (Thanks to Toni Brkic and Robin Dunn)
-  * Mac OSX (Thanks to Robin Dunn for the :class:`CaptionBar` size patch)
-
-
-Window Styles
-=============
-
-This class supports the following window styles:
-
-========================== =========== ==================================================
-Window Styles              Hex Value   Description
-========================== =========== ==================================================
-``FPB_SINGLE_FOLD``                0x1 Single fold forces other panels to close when they are open, and only opens the current panel. This will allow the open panel to gain the full size left in the client area.
-``FPB_COLLAPSE_TO_BOTTOM``         0x2 All panels are stacked to the bottom. When they are expanded again they show up at the top.
-``FPB_EXCLUSIVE_FOLD``             0x4 ``FPB_SINGLE_FOLD`` style plus the panels will be stacked at the bottom.
-``FPB_HORIZONTAL``                 0x8 :class:`FoldPanelBar` will be horizontal.
-``FPB_VERTICAL``                  0x10 :class:`FoldPanelBar` will be vertical.
-========================== =========== ==================================================
-
-
-Events Processing
-=================
-
-This class processes the following events:
-
-================== ==================================================
-Event Name         Description
-================== ==================================================
-``EVT_CAPTIONBAR`` The user has pressed the caption bar: :class:`FoldPanelBar` will either expand or collapse the underlying panel.
-================== ==================================================
-
-
-License And Version
-===================
-
-:class:`FoldPanelBar` is distributed under the wxPython license.
-
-Latest Revision: Andrea Gavana @ 16 Jul 2012, 15.00 GMT
-
-Version 0.6
-
-"""
-
-import wx
-
-from .constants import FOLDPANEL_BG_COLOR
-    
-#----------------------------------------------------------------------
-# Collapsed And Expanded Bitmap Images
-# Created With img2py.py
-#----------------------------------------------------------------------
-from wx.lib.embeddedimage import PyEmbeddedImage
-
-CollapsedIcon = PyEmbeddedImage(
-    "iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABHNCSVQICAgIfAhkiAAAADdJ"
-    "REFUOI1jZGRiZqAEMFGke/Ab8P/f3/8D5wKY7YRcQRsXoNuKzxXUdwEu23CJU+wCxtG8wAAA"
-    "mvUb+vltJD8AAAAASUVORK5CYII=")
-
-ExpandedIcon = PyEmbeddedImage(
-    "iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABHNCSVQICAgIfAhkiAAAAEJJ"
-    "REFUOI1jZGRiZqAEMFGke1AYwIIu8P/f3/+4FDMyMTNS3QUYBmCzBZ84bQIR3TZcttPOBci2"
-    "4rOdKi5gHM0LDACevARXGc9htQAAAABJRU5ErkJggg==")
-
-#----------------------------------------------------------------------
-# FOLDPANELBAR Starts Here
-#----------------------------------------------------------------------
-
-# CAPTIONBAR STYLES
-#
-#- CAPTIONBAR_GRADIENT_V: Draws a vertical gradient from top to bottom
-#- CAPTIONBAR_GRADIENT_H: Draws a horizontal gradient from left to right
-#- CAPTIONBAR_SINGLE: Draws a single filled rectangle to draw the caption
-#- CAPTIONBAR_RECTANGLE: Draws a single colour with a rectangle around the caption
-#- CAPTIONBAR_FILLED_RECTANGLE: Draws a filled rectangle and a border around it
-
-CAPTIONBAR_NOSTYLE            = 0
-""" The :class:`CaptionBar` has no style bit set. """
-CAPTIONBAR_GRADIENT_V         = 1
-""" Draws a vertical gradient from top to bottom. """
-CAPTIONBAR_GRADIENT_H         = 2
-""" Draws a vertical gradient from left to right. """
-CAPTIONBAR_SINGLE             = 3
-""" Draws a single filled rectangle to draw the caption. """
-CAPTIONBAR_RECTANGLE          = 4
-""" Draws a single colour with a rectangle around the caption. """
-CAPTIONBAR_FILLED_RECTANGLE   = 5
-""" Draws a filled rectangle and a border around it. """
-
-FPB_EXTRA_X = 10
-""" Extra horizontal padding, in pixels. """
-FPB_EXTRA_Y = 8
-""" Extra vertical padding, in pixels. """
-
-# pixels of the bmp to be aligned from the right filled with space
-FPB_BMP_RIGHTSPACE = 2
-""" Pixels of the bmp to be aligned from the right filled with space. """
-
-# Now supported! Single fold forces
-# other panels to close when they are open, and only opens the current panel.
-# This will allow the open panel to gain the full size left in the client area
-FPB_SINGLE_FOLD = 0x0001
-""" Single fold forces other panels to close when they are open, and only opens the current panel. This will allow the open panel to gain the full size left in the client area."""
-
-# All panels are stacked to the bottom. When they are expanded again they
-# show up at the top
-FPB_COLLAPSE_TO_BOTTOM = 0x0002
-""" All panels are stacked to the bottom. When they are expanded again they show up at the top. """
-
-# Now supported! Single fold plus panels
-# will be stacked at the bottom
-FPB_EXCLUSIVE_FOLD = 0x0004
-""" ``FPB_SINGLE_FOLD`` style plus the panels will be stacked at the bottom. """
-
-# Orientation Flag
-FPB_HORIZONTAL = 0x0008
-""" :class:`FoldPanelBar` will be horizontal. """
-FPB_VERTICAL = 0x0010
-""" :class:`FoldPanelBar` will be vertical. """
-
-# FoldPanelItem default settings
-FPB_ALIGN_LEFT = 0
-""" Aligns left instead of fitting the width of the child window to be added. Use either this one or ``FPB_ALIGN_WIDTH``. """
-FPB_ALIGN_WIDTH = 1
-""" The :class:`wx.Window` to be added will be aligned to fit the width of the FoldPanel when it is resized. Very handy for sizer items, buttons and text boxes. """
-
-FPB_DEFAULT_LEFTSPACING = 10
-FPB_DEFAULT_RIGHTSPACING = 10
-FPB_DEFAULT_SPACING = 8
-
-FPB_DEFAULT_LEFTLINESPACING = 20
-FPB_DEFAULT_RIGHTLINESPACING = 20
-
-
-# ------------------------------------------------------------------------------ #
-# class CaptionBarStyle
-# ------------------------------------------------------------------------------ #
-
-class CaptionBarStyle(object):
-    """
-    This class encapsulates the styles you wish to set for the
-    :class:`CaptionBar` (this is the part of the `FoldPanel` where the caption
-    is displayed). It can either be applied at creation time be
-    reapplied when styles need to be changed.
-
-    At construction time, all styles are set to their default
-    transparency.  This means none of the styles will be applied to
-    the :class:`CaptionBar` in question, meaning it will be created using the
-    default internals. When setting i.e the colour, font or panel
-    style, these styles become active to be used.
-    """
-
-    def __init__(self):
-        """ Default constructor for this class. """
-
-        self.ResetDefaults()
-
-
-    def ResetDefaults(self):
-        """ Resets default :class:`CaptionBarStyle`. """
-        self._firstColourUsed = False
-        self._secondColourUsed = False
-        self._textColourUsed = False
-        self._captionFontUsed = False
-        self._captionStyleUsed = False
-        self._captionStyle = CAPTIONBAR_GRADIENT_V
-
-
-    # ------- CaptionBar Font -------
-
-    def SetCaptionFont(self, font):
-        """
-        Sets font for the caption bar.
-
-        :param `font`: a valid :class:`wx.Font` object.
-
-        :note: If this is not set, the font property is undefined and will not be used.
-         Use :meth:`~CaptionBarStyle.CaptionFontUsed` to check if this style is used.
-        """
-
-        self._captionFont = font
-        self._captionFontUsed = True
-
-
-    def CaptionFontUsed(self):
-        """ Checks if the caption bar font is set. """
-
-        return self._captionFontUsed
-
-
-    def GetCaptionFont(self):
-        """
-        Returns the font for the caption bar.
-
-        :note: Please be warned this will result in an assertion failure when
-         this property is not previously set.
-
-        :see: :meth:`~CaptionBarStyle.SetCaptionFont`, :meth:`~CaptionBarStyle.CaptionFontUsed`
-        """
-
-        return self._captionFont
-
-
-    # ------- First Colour -------
-
-    def SetFirstColour(self, colour):
-        """
-        Sets first colour for the caption bar.
-
-        :param `colour`: a valid :class:`wx.Colour` object.
-
-        :note: If this is not set, the colour property is undefined and will not be used.
-         Use :meth:`~CaptionBarStyle.FirstColourUsed` to check if this style is used.
-        """
-
-        self._firstColour = colour
-        self._firstColourUsed = True
-
-
-    def FirstColourUsed(self):
-        """ Checks if the first colour of the caption bar is set."""
-
-        return self._firstColourUsed
-
-
-    def GetFirstColour(self):
-        """
-        Returns the first colour for the caption bar.
-
-        :note: Please be warned this will result in an assertion failure when
-         this property is not previously set.
-
-        :see: :meth:`~CaptionBarStyle.SetFirstColour`, :meth:`~CaptionBarStyle.FirstColourUsed`
-        """
-
-        return self._firstColour
-
-
-    # ------- Second Colour -------
-
-    def SetSecondColour(self, colour):
-        """
-        Sets second colour for the caption bar.
-
-        :param `colour`: a valid :class:`wx.Colour` object.
-
-        :note: If this is not set, the colour property is undefined and will not be used.
-         Use :meth:`~CaptionBarStyle.SecondColourUsed` to check if this style is used.
-        """
-
-        self._secondColour = colour
-        self._secondColourUsed = True
-
-
-    def SecondColourUsed(self):
-        """ Checks if the second colour of the caption bar is set."""
-
-        return self._secondColourUsed
-
-
-    def GetSecondColour(self):
-        """
-        Returns the second colour for the caption bar.
-
-        :note: Please be warned this will result in an assertion failure when
-         this property is not previously set.
-
-        :see: :meth:`~CaptionBarStyle.SetSecondColour`, :meth:`~CaptionBarStyle.SecondColourUsed`
-        """
-
-        return self._secondColour
-
-
-    # ------- Caption Text Colour -------
-
-    def SetCaptionColour(self, colour):
-        """
-        Sets caption colour for the caption bar.
-
-        :param `colour`: a valid :class:`wx.Colour` object.
-
-        :note: If this is not set, the colour property is undefined and will not be used.
-         Use :meth:`~CaptionBarStyle.CaptionColourUsed` to check if this style is used.
-        """
-
-        self._textColour = colour
-        self._textColourUsed = True
-
-
-    def CaptionColourUsed(self):
-        """ Checks if the caption colour of the caption bar is set."""
-
-        return self._textColourUsed
-
-
-    def GetCaptionColour(self):
-        """
-        Returns the caption colour for the caption bar.
-
-        :note: Please be warned this will result in an assertion failure
-         when this property is not previously set.
-
-        :see: :meth:`~CaptionBarStyle.SetCaptionColour`, :meth:`~CaptionBarStyle.CaptionColourUsed`
-        """
-
-        return self._textColour
-
-
-    # ------- CaptionStyle  -------
-
-    def SetCaptionStyle(self, style):
-        """
-        Sets caption style for the caption bar.
-
-        :param `style`: can be one of the following bits:
-
-         =============================== ======= =============================
-         Caption Style                    Value  Description
-         =============================== ======= =============================
-         ``CAPTIONBAR_GRADIENT_V``             1 Draws a vertical gradient from top to bottom
-         ``CAPTIONBAR_GRADIENT_H``             2 Draws a horizontal gradient from left to right
-         ``CAPTIONBAR_SINGLE``                 3 Draws a single filled rectangle to draw the caption
-         ``CAPTIONBAR_RECTANGLE``              4 Draws a single colour with a rectangle around the caption
-         ``CAPTIONBAR_FILLED_RECTANGLE``       5 Draws a filled rectangle and a border around it
-         =============================== ======= =============================
-
-        :note: If this is not set, the property is undefined and will not be used.
-         Use :meth:`~CaptionBarStyle.CaptionStyleUsed` to check if this style is used.
-        """
-
-        self._captionStyle = style
-        self._captionStyleUsed = True
-
-
-    def CaptionStyleUsed(self):
-        """ Checks if the caption style of the caption bar is set."""
-
-        return self._captionStyleUsed
-
-
-    def GetCaptionStyle(self):
-        """
-        Returns the caption style for the caption bar.
-
-        :note: Please be warned this will result in an assertion failure
-         when this property is not previously set.
-
-        :see: :meth:`~CaptionBarStyle.SetCaptionStyle`, :meth:`~CaptionBarStyle.CaptionStyleUsed`
-        """
-
-        return self._captionStyle
-
-
-#-----------------------------------#
-#        CaptionBarEvent
-#-----------------------------------#
-wxEVT_CAPTIONBAR = wx.NewEventType()
-EVT_CAPTIONBAR = wx.PyEventBinder(wxEVT_CAPTIONBAR, 0)
-""" The user has pressed the caption bar: :class:`FoldPanelBar` will either expand or""" \
-""" collapse the underlying panel. """
-
-# Define Empty CaptionBar Style
-EmptyCaptionBarStyle = CaptionBarStyle()
-
-# ---------------------------------------------------------------------------- #
-# class CaptionBarEvent
-# ---------------------------------------------------------------------------- #
-
-class CaptionBarEvent(wx.CommandEvent):
-    """
-    This event will be sent when a ``EVT_CAPTIONBAR`` is mapped in the parent.
-    It is to notify the parent that the bar is now in collapsed or expanded
-    state. The parent should re-arrange the associated windows accordingly
-    """
-
-    def __init__(self, evtType):
-        """
-        Default class constructor.
-
-        :param `evtType`: the event type.
-        """
-
-        wx.CommandEvent.__init__(self, evtType)
-
-
-    def GetFoldStatus(self):
-        """
-        Returns whether the bar is expanded or collapsed. ``True`` means
-        expanded.
-        """
-
-        return not self._bar.IsCollapsed()
-
-
-    def GetBar(self):
-        """ Returns the selected :class:`CaptionBar`. """
-
-        return self._bar
-
-
-    def SetTag(self, tag):
-        """
-        Assigns a tag to the selected :class:`CaptionBar`.
-
-        :param `tag`: an instance of :class:`FoldPanelBar`.
-        """
-
-        self._tag = tag
-
-
-    def GetTag(self):
-        """ Returns the tag assigned to the selected :class:`CaptionBar`. """
-
-        return self._tag
-
-
-    def SetBar(self, bar):
-        """
-        Sets the bar associated with this event.
-
-        :param `bar`: an instance of :class:`CaptionBar`.
-
-        :note: Should not be used by any other than the originator of the event.
-        """
-
-        self._bar = bar
-
-
-# -------------------------------------------------------------------------------- #
-# class CaptionBar
-# -------------------------------------------------------------------------------- #
-
-class CaptionBar(wx.Window):
-    """
-    This class is a graphical caption component that consists of a
-    caption and a clickable arrow.
-
-    The :class:`CaptionBar` fires an event ``EVT_CAPTIONBAR`` which is a
-    :class:`CaptionBarEvent`. This event can be caught and the parent window
-    can act upon the collapsed or expanded state of the bar (which is
-    actually just the icon which changed). The parent panel can
-    reduce size or expand again.
-    """
-
-    def __init__(self, parent, id, pos, size, caption="",
-                 foldIcons=None, cbstyle=None,
-                 rightIndent=FPB_BMP_RIGHTSPACE,
-                 iconWidth=16, iconHeight=16, collapsed=False):
-        """
-        Default class constructor.
-
-        :param `parent`: the :class:`CaptionBar` parent window;
-        :param `id`: an identifier for the control: a value of -1 is taken to mean a default;
-        :param `pos`: the control position. A value of (-1, -1) indicates a default position,
-         chosen by either the windowing system or wxPython, depending on platform;
-        :param `size`: the control size. A value of (-1, -1) indicates a default size,
-         chosen by either the windowing system or wxPython, depending on platform;
-        :param `caption`: the string to be displayed in :class:`CaptionBar`;
-        :param `foldIcons`: an instance of :class:`wx.ImageList` containing the icons to display
-         next to the caption text;
-        :param `cbstyle`: the :class:`CaptionBar` window style. Must be an instance of
-         :class:`CaptionBarStyle`;
-        :param `rightIndent`: number of pixels of the bmp to be aligned from the right filled
-         with space;
-        :param `iconWidth`: the :class:`CaptionBar` icon width;
-        :param `iconHeight`: the :class:`CaptionBar` icon height;
-        :param `collapsed`: ``True`` if the :class:`CaptionBar` should start in the collapsed state,
-         ``False`` otherwise.
-        """
-
-        wx.Window.__init__(self, parent, wx.ID_ANY, pos=pos,
-                           size=(20,20), style=wx.NO_BORDER)
-
-        self._controlCreated = False
-        self._collapsed = collapsed
-        self.ApplyCaptionStyle(cbstyle, True)
-
-        if foldIcons is None:
-            foldIcons = wx.ImageList(16, 16)
-
-            bmp = ExpandedIcon.GetBitmap()
-            foldIcons.Add(bmp)
-            bmp = CollapsedIcon.GetBitmap()
-            foldIcons.Add(bmp)
-
-        # set initial size
-        if foldIcons:
-            assert foldIcons.GetImageCount() > 1
-            iconWidth, iconHeight = foldIcons.GetSize(0)
-
-        self._caption = caption
-        self._foldIcons = foldIcons
-        self._style = cbstyle
-        self._rightIndent = rightIndent
-        self._iconWidth = iconWidth
-        self._iconHeight = iconHeight
-        self._oldSize = wx.Size(20,20)
-
-        self._controlCreated = True
-        
-        self.SetBackgroundColour(FOLDPANEL_BG_COLOR)
-
-        self.Bind(wx.EVT_PAINT, self.OnPaint)
-        self.Bind(wx.EVT_SIZE, self.OnSize)
-        self.Bind(wx.EVT_MOUSE_EVENTS, self.OnMouseEvent)
-        self.Bind(wx.EVT_CHAR, self.OnChar)
-
-
-    def ApplyCaptionStyle(self, cbstyle=None, applyDefault=True):
-        """
-        Applies the style defined in `cbstyle` to the :class:`CaptionBar`.
-
-        :param `cbstyle`: an instance of :class:`CaptionBarStyle`;
-        :param `applyDefault`: if ``True``, the colours used in the :class:`CaptionBarStyle`
-         will be reset to their default values.
-        """
-
-        if cbstyle is None:
-            cbstyle = EmptyCaptionBarStyle
-
-        newstyle = cbstyle
-
-        if applyDefault:
-
-            # get first colour from style or make it default
-            if not newstyle.FirstColourUsed():
-                newstyle.SetFirstColour(wx.WHITE)
-
-            # get second colour from style or make it default
-            if not newstyle.SecondColourUsed():
-                # make the second colour slightly darker then the background
-                colour = self.GetParent().GetBackgroundColour()
-                r, g, b = int(colour.Red()), int(colour.Green()), int(colour.Blue())
-                colour = ((r >> 1) + 20, (g >> 1) + 20, (b >> 1) + 20)
-                newstyle.SetSecondColour(wx.Colour(colour[0], colour[1], colour[2]))
-
-            # get text colour
-            if not newstyle.CaptionColourUsed():
-                newstyle.SetCaptionColour(wx.BLACK)
-
-            # get font colour
-            if not newstyle.CaptionFontUsed():
-                newstyle.SetCaptionFont(self.GetParent().GetFont())
-
-            # apply caption style
-            if not newstyle.CaptionStyleUsed():
-                newstyle.SetCaptionStyle(CAPTIONBAR_GRADIENT_V)
-
-        self._style = newstyle
-
-
-    def SetCaptionStyle(self, cbstyle=None, applyDefault=True):
-        """
-        Sets :class:`CaptionBar` styles with :class:`CaptionBarStyle` class.
-
-        :param `cbstyle`: an instance of :class:`CaptionBarStyle`;
-        :param `applyDefault`: if ``True``, the colours used in the :class:`CaptionBarStyle`
-         will be reset to their default values.
-
-        :note: All styles that are actually set, are applied. If you set `applyDefault`
-         to ``True``, all other (not defined) styles will be set to default. If it is
-         ``False``, the styles which are not set in the :class:`CaptionBarStyle` will be ignored.
-        """
-
-        if cbstyle is None:
-            cbstyle = EmptyCaptionBarStyle
-
-        self.ApplyCaptionStyle(cbstyle, applyDefault)
-        self.Refresh()
-
-
-    def GetCaptionStyle(self):
-        """
-        Returns the current style of the captionbar in a :class:`CaptionBarStyle` class.
-
-        :note: This can be used to change and set back the changes.
-        """
-
-        return self._style
-
-
-    def IsCollapsed(self):
-        """ Returns wether the status of the bar is expanded or collapsed. """
-
-        return self._collapsed
-
-
-    def SetRightIndent(self, pixels):
-        """
-        Sets the amount of pixels on the right from which the bitmap
-        is trailing.
-
-        :param `pixels`: the number of pixels on the right from which the bitmap
-         is trailing. If this is 0, it will be drawn all the way to the right,
-         default is equal to ``FPB_BMP_RIGHTSPACE``. Assign this before
-         assigning an image list to prevent a redraw.
-        """
-
-        assert pixels >= 0
-        self._rightIndent = pixels
-        if self._foldIcons:
-            self.Refresh()
-
-
-    def Collapse(self):
-        """
-        This sets the internal state/representation to collapsed.
-
-        :note: This does not trigger a :class:`CaptionBarEvent` to be sent to the
-         parent.
-        """
-
-        self._collapsed = True
-        self.RedrawIconBitmap()
-
-
-    def Expand(self):
-        """
-        This sets the internal state/representation to expanded.
-
-        :note: This does not trigger a :class:`CaptionBarEvent` to be sent to the
-         parent.
-        """
-
-        self._collapsed = False
-        self.RedrawIconBitmap()
-
-
-    def SetBoldFont(self):
-        """ Sets the :class:`CaptionBar` font weight to bold."""
-
-        self.GetFont().SetWeight(wx.FONTWEIGHT_BOLD)
-
-
-    def SetNormalFont(self):
-        """ Sets the :class:`CaptionBar` font weight to normal."""
-
-        self.GetFont().SetWeight(wx.FONTWEIGHT_NORMAL)
-
-
-    def IsVertical(self):
-        """
-        Returns wether the :class:`CaptionBar` has a default orientation or not.
-        Default is vertical.
-        """
-
-        fld = self.GetParent().GetGrandParent()
-        if isinstance(fld, FoldPanelBar):
-            return self.GetParent().GetGrandParent().IsVertical()
-        else:
-            raise Exception("ERROR: Wrong Parent " + repr(fld))
-
-
-    def OnPaint(self, event):
-        """
-        Handles the ``wx.EVT_PAINT`` event for :class:`CaptionBar`.
-
-        :param `event`: a :class:`PaintEvent` event to be processed.
-        """
-
-        if not self._controlCreated:
-            event.Skip()
-            return
-
-        dc = wx.PaintDC(self)
-        wndRect = self.GetRect()
-        vertical = self.IsVertical()
-
-        # TODO: Maybe first a memory DC should draw all, and then paint it on
-        # the caption. This way a flickering arrow during resize is not visible
-
-        self.FillCaptionBackground(dc)
-        dc.SetFont(self._style.GetCaptionFont())
-        dc.SetTextForeground(self._style.GetCaptionColour())
-
-        # draw small icon, either collapsed or expanded
-        # based on the state of the bar. If we have any bmp's
-
-        if self._foldIcons:
-
-            index = self._collapsed
-
-            if vertical:
-                drw = self._iconWidth - self._rightIndent - 10
-                self._foldIcons.Draw(index, dc, drw,
-                                     (wndRect.GetHeight() - self._iconHeight)//2,
-                                     wx.IMAGELIST_DRAW_TRANSPARENT)
-            else:
-                self._foldIcons.Draw(index, dc,
-                                     (wndRect.GetWidth() - self._iconWidth)//2,
-                                     self._rightIndent, wx.IMAGELIST_DRAW_TRANSPARENT)
-
-        else:
-            pass
-
-        txt_w, txt_h = dc.GetTextExtent(self._caption)
-
-        if vertical:
-            dc.DrawText(self._caption,
-                        10 + self._rightIndent + self._iconWidth,
-                        FPB_EXTRA_Y//2)
-        else:
-            dc.DrawRotatedText(self._caption, FPB_EXTRA_Y//2,
-                               wndRect.GetBottom() - 4, 90)
-
-##        event.Skip()
-
-
-    def FillCaptionBackground(self, dc):
-        """
-        Fills the background of the caption with either a gradient or
-        a solid colour.
-
-        :param `dc`: an instance of :class:`wx.DC`.
-        """
-
-        style = self._style.GetCaptionStyle()
-
-        if style == CAPTIONBAR_GRADIENT_V:
-            if self.IsVertical():
-                self.DrawVerticalGradient(dc, self.GetRect())
-            else:
-                self.DrawHorizontalGradient(dc, self.GetRect())
-
-        elif style == CAPTIONBAR_GRADIENT_H:
-            if self.IsVertical():
-                self.DrawHorizontalGradient(dc, self.GetRect())
-            else:
-                self.DrawVerticalGradient(dc, self.GetRect())
-
-        elif style == CAPTIONBAR_SINGLE:
-            self.DrawSingleColour(dc, self.GetRect())
-        elif style == CAPTIONBAR_RECTANGLE or style == CAPTIONBAR_FILLED_RECTANGLE:
-            self.DrawSingleRectangle(dc, self.GetRect())
-        else:
-            raise Exception("STYLE Error: Undefined Style Selected: " + repr(style))
-
-
-    def OnMouseEvent(self, event):
-        """
-        Handles the ``wx.EVT_MOUSE_EVENTS`` event for :class:`CaptionBar`.
-
-        :param `event`: a :class:`MouseEvent` event to be processed.
-
-        :note: This method catches the mouse click-double click. If clicked on
-         the arrow (single) or double on the caption we change state and an event
-         must be fired to let this panel collapse or expand.
-        """
-
-        send_event = False
-        vertical = self.IsVertical()
-
-        if event.LeftDown() and self._foldIcons:
-
-            pt = event.GetPosition()
-            rect = self.GetRect()
-
-            drw = 0
-            if vertical and pt.x > 0 or not vertical and \
-               pt.y < (self._iconHeight + self._rightIndent):
-                send_event = True
-
-        elif event.LeftDClick():
-            # self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
-            send_event = True
-
-        # elif event.Entering() and self._foldIcons:
-        #     self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
-
-        #     pt = event.GetPosition()
-        #     rect = self.GetRect()
-
-        #     drw = 0
-        #     if vertical and pt.x > drw or not vertical and \
-        #        pt.y < (self._iconHeight + self._rightIndent):
-        #         self.SetCursor(wx.Cursor(wx.CURSOR_HAND))
-        #     else:
-        #         self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
-
-        # elif event.Leaving():
-        #     self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
-
-        # elif event.Moving():
-        #     pt = event.GetPosition()
-        #     rect = self.GetRect()
-
-        #     drw = 0
-        #     if vertical and pt.x > drw or not vertical and \
-        #        pt.y < (self._iconHeight + self._rightIndent):
-        #         self.SetCursor(wx.Cursor(wx.CURSOR_HAND))
-        #     else:
-        #         self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
-
-        # send the collapse, expand event to the parent
-
-        if send_event:
-            event = CaptionBarEvent(wxEVT_CAPTIONBAR)
-            event.SetId(self.GetId())
-            event.SetEventObject(self)
-            event.SetBar(self)
-            self.GetEventHandler().ProcessEvent(event)
-
-
-    def OnChar(self, event):
-        """
-        Handles the ``wx.EVT_CHAR`` event for :class:`CaptionBar`.
-
-        :param `event`: a :class:`KeyEvent` event to be processed.
-
-        :note: This method currently does nothing.
-        """
-
-        # TODO: Anything here?
-        event.Skip()
-
-
-    def DoGetBestSize(self):
-        """
-        Returns the best size for this panel, based upon the font
-        assigned to this window, and the caption string.
-
-        :note: Overridden from :class:`wx.Window`.
-        """
-
-        if self.IsVertical():
-            x, y = self.GetTextExtent(self._caption)
-        else:
-            y, x = self.GetTextExtent(self._caption)
-
-        if x < self._iconWidth:
-            x = self._iconWidth
-
-        if y < self._iconHeight:
-            y = self._iconHeight
-
-        # TODO: The extra FPB_EXTRA_X constants should be adjustable as well
-
-        return wx.Size(x + FPB_EXTRA_X, y + FPB_EXTRA_Y)
-
-
-    # def DrawVerticalGradient(self, dc, rect):
-    #     """
-    #     Gradient fill from colour 1 to colour 2 from top to bottom.
-
-    #     :param `dc`: an instance of :class:`wx.DC`;
-    #     :param `rect`: the :class:`CaptionBar` client rectangle.
-    #     """
-
-    #     if  rect.height < 1 or rect.width < 1:
-    #         return
-
-    #     dc.SetPen(wx.TRANSPARENT_PEN)
-
-    #     # calculate gradient coefficients
-    #     col2 = self._style.GetSecondColour()
-    #     col1 = self._style.GetFirstColour()
-
-    #     r1, g1, b1 = int(col1.Red()), int(col1.Green()), int(col1.Blue())
-    #     r2, g2, b2 = int(col2.Red()), int(col2.Green()), int(col2.Blue())
-
-    #     flrect = float(rect.height)
-
-    #     rstep = float((r2 - r1)) / flrect
-    #     gstep = float((g2 - g1)) / flrect
-    #     bstep = float((b2 - b1)) / flrect
-
-    #     rf, gf, bf = 0, 0, 0
-
-    #     for y in range(rect.y, rect.y + rect.height):
-    #         currCol = (r1 + rf, g1 + gf, b1 + bf)
-
-    #         dc.SetBrush(wx.Brush(currCol, wx.BRUSHSTYLE_SOLID))
-    #         dc.DrawRoundedRectangle(rect.x, rect.y + (y - rect.y), rect.width, rect.height, 4)
-    #         rf = rf + rstep
-    #         gf = gf + gstep
-    #         bf = bf + bstep
-
-
-    # def DrawHorizontalGradient(self, dc, rect):
-    #     """
-    #     Gradient fill from colour 1 to colour 2 from left to right.
-
-    #     :param `dc`: an instance of :class:`wx.DC`;
-    #     :param `rect`: the :class:`CaptionBar` client rectangle.
-    #     """
-
-    #     if rect.height < 1 or rect.width < 1:
-    #         return
-
-    #     dc.SetPen(wx.TRANSPARENT_PEN)
-
-    #     # calculate gradient coefficients
-    #     col2 = self._style.GetSecondColour()
-    #     col1 = self._style.GetFirstColour()
-
-    #     r1, g1, b1 = int(col1.Red()), int(col1.Green()), int(col1.Blue())
-    #     r2, g2, b2 = int(col2.Red()), int(col2.Green()), int(col2.Blue())
-
-    #     flrect = float(rect.width)
-
-    #     rstep = float((r2 - r1)) / flrect
-    #     gstep = float((g2 - g1)) / flrect
-    #     bstep = float((b2 - b1)) / flrect
-
-    #     rf, gf, bf = 0, 0, 0
-
-    #     for x in range(rect.x, rect.x + rect.width):
-    #         currCol = (r1 + rf, g1 + gf, b1 + bf)
-
-    #         dc.SetBrush(wx.Brush(currCol, wx.BRUSHSTYLE_SOLID))
-    #         dc.DrawRectangle(rect.x + (x - rect.x), rect.y, 1, rect.height)
-    #         rf = rf + rstep
-    #         gf = gf + gstep
-    #         bf = bf + bstep
-
-
-    def DrawSingleColour(self, dc, rect):
-        """
-        Single colour fill for :class:`CaptionBar`.
-
-        :param `dc`: an instance of :class:`wx.DC`;
-        :param `rect`: the :class:`CaptionBar` client rectangle.
-        """
-
-        if rect.height < 1 or rect.width < 1:
-            return
-
-        dc.SetPen(wx.TRANSPARENT_PEN)
-
-        # draw simple rectangle
-        dc.SetBrush(wx.Brush(self._style.GetFirstColour(), wx.BRUSHSTYLE_SOLID))
-        dc.DrawRoundedRectangle(rect.x, rect.y, rect.width, rect.height, 4)
-
-        if self.IsCollapsed() is not True:
-            dc.DrawRectangle(rect.x, rect.y+rect.height-2, rect.width, 4)
-
-
-    # def DrawSingleRectangle(self, dc, rect):
-    #     """
-    #     Single rectangle for :class:`CaptionBar`.
-
-    #     :param `dc`: an instance of :class:`wx.DC`;
-    #     :param `rect`: the :class:`CaptionBar` client rectangle.
-    #     """
-
-    #     if rect.height < 2 or rect.width < 1:
-    #         return
-
-    #     # single frame, set up internal fill colour
-
-    #     if self._style.GetCaptionStyle() == CAPTIONBAR_RECTANGLE:
-    #         colour = self.GetParent().GetBackgroundColour()
-    #         br = wx.Brush(colour, wx.BRUSHSTYLE_SOLID)
-    #     else:
-    #         colour = self._style.GetFirstColour()
-    #         br = wx.Brush(colour, wx.BRUSHSTYLE_SOLID)
-
-    #     # setup the pen frame
-
-    #     pen = wx.Pen(self._style.GetSecondColour())
-    #     dc.SetPen(pen)
-    #     dc.SetBrush(br)
-    #     dc.DrawRoundedRectangle(rect.x, rect.y, rect.width, rect.height - 1, 4)
-
-    #     bgpen = wx.Pen(self.GetParent().GetBackgroundColour())
-    #     dc.SetPen(bgpen)
-    #     dc.DrawLine(rect.x, rect.y + rect.height - 1, rect.x + rect.width,
-    #                 rect.y + rect.height - 1)
-
-
-    def OnSize(self, event):
-        """
-        Handles the ``wx.EVT_SIZE`` event for :class:`CaptionBar`.
-
-        :param `event`: a :class:`wx.SizeEvent` event to be processed.
-        """
-
-        if not self._controlCreated:
-            event.Skip()
-            return
-
-        size = event.GetSize()
-
-        if self._foldIcons:
-
-            # What I am doing here is simply invalidating the part of the window
-            # exposed. So when I make a rect with as width the newly exposed part,
-            # and the x,y of the old window size origin, I don't need a bitmap
-            # calculation in it, or do I ? The bitmap needs redrawing anyway.
-            # Leave it like this until I figured it out.
-
-            # set rect to redraw as old bitmap area which is entitled to redraw
-
-            rect = wx.Rect(size.GetWidth() - self._iconWidth - self._rightIndent, 0,
-                           self._iconWidth + self._rightIndent,
-                           self._iconWidth + self._rightIndent)
-
-            # adjust rectangle when more is slided so we need to redraw all
-            # the old stuff but not all (ugly flickering)
-
-            diffX = size.GetWidth() - self._oldSize.GetWidth()
-
-            if diffX > 1:
-
-                # adjust the rect with all the crap to redraw
-
-                rect.SetWidth(rect.GetWidth() + diffX + 10)
-                rect.SetX(rect.GetX() - diffX - 10)
-
-            self.RefreshRect(rect)
-
-        else:
-
-            rect = self.GetRect()
-            self.RefreshRect(rect)
-
-        self._oldSize = size
-
-
-    def RedrawIconBitmap(self):
-        """ Redraws the icons (if they exists). """
-
-        if self._foldIcons:
-
-            # invalidate the bitmap area and force a redraw
-
-            rect = self.GetRect()
-
-            rect.SetX(rect.GetWidth() - self._iconWidth - self._rightIndent)
-            rect.SetWidth(self._iconWidth + self._rightIndent)
-            self.RefreshRect(rect)
-
-
-# ---------------------------------------------------------------------------------- #
-# class FoldPanelBar
-# ---------------------------------------------------------------------------------- #
-
-class FoldPanelBar(wx.Panel):
-    """
-    The :class:`FoldPanelBar` is a class which can maintain a list of
-    collapsible panels. Once a panel is collapsed, only it's caption
-    bar is visible to the user. This will provide more space for the
-    other panels, or allow the user to close panels which are not used
-    often to get the most out of the work area.
-
-    This control is easy to use. Simply create it as a child for a
-    panel or sash window, and populate panels with
-    :meth:`FoldPanelBar.AddFoldPanel() <FoldPanelBar.AddFoldPanel>`. Then use the
-    :meth:`FoldPanelBar.AddFoldPanelWindow() <FoldPanelBar.AddFoldPanelWindow>` to add
-    :class:`wx.Window` derived controls to the current fold panel. Use
-    :meth:`FoldPanelBar.AddFoldPanelSeparator() <FoldPanelBar.AddFoldPanelSeparator>` to put separators between the groups of
-    controls that need a visual separator to group them
-    together. After all is constructed, the user can fold the panels
-    by double clicking on the bar or single click on the arrow, which
-    will indicate the collapsed or expanded state.
-    """
-
-    def __init__(self, parent, id=-1, pos=wx.DefaultPosition, size=wx.DefaultSize,
-                 style=wx.TAB_TRAVERSAL|wx.NO_BORDER, agwStyle=0):
-        """
-        Default class constructor.
-
-        :param `parent`: the :class:`FoldPanelBar` parent window;
-        :param `id`: an identifier for the control: a value of -1 is taken to mean a default;
-        :param `pos`: the control position. A value of (-1, -1) indicates a default position,
-         chosen by either the windowing system or wxPython, depending on platform;
-        :param `size`: the control size. A value of (-1, -1) indicates a default size,
-         chosen by either the windowing system or wxPython, depending on platform;
-        :param `style`: the underlying :class:`Panel` window style;
-        :param `agwStyle`: the AGW-specific :class:`FoldPanelBar` window style. It can be one of the
-         following bits:
-
-         ========================== =========== ==================================================
-         Window Styles              Hex Value   Description
-         ========================== =========== ==================================================
-         ``FPB_SINGLE_FOLD``                0x1 Single fold forces other panels to close when they are open, and only opens the current panel. This will allow the open panel to gain the full size left in the client area.
-         ``FPB_COLLAPSE_TO_BOTTOM``         0x2 All panels are stacked to the bottom. When they are expanded again they show up at the top.
-         ``FPB_EXCLUSIVE_FOLD``             0x4 ``FPB_SINGLE_FOLD`` style plus the panels will be stacked at the bottom.
-         ``FPB_HORIZONTAL``                 0x4 :class:`FoldPanelBar` will be horizontal.
-         ``FPB_VERTICAL``                   0x8 :class:`FoldPanelBar` will be vertical.
-         ========================== =========== ==================================================
-        """
-
-        self._controlCreated = False
-
-        # make sure there is any orientation
-        if not agwStyle & (FPB_HORIZONTAL | FPB_VERTICAL):
-            agwStyle = agwStyle | FPB_VERTICAL
-
-        if agwStyle & FPB_HORIZONTAL:
-            self._isVertical = False
-        else:
-            self._isVertical = True
-
-        self._agwStyle = agwStyle
-
-        # create the panel (duh!). This causes a size event, which we are going
-        # to skip when we are not initialised
-
-        wx.Panel.__init__(self, parent, id, pos, size, style)
-
-        # the fold panel area
-
-        self._foldPanel = wx.Panel(self, wx.ID_ANY, pos, size,
-                                   wx.NO_BORDER | wx.TAB_TRAVERSAL)
-
-        self._controlCreated = True
-        self._panels = []
-
-        self.Bind(EVT_CAPTIONBAR, self.OnPressCaption)
-        self.Bind(wx.EVT_SIZE, self.OnSizePanel)
-
-
-    def AddFoldPanel(self, caption="", collapsed=False, foldIcons=None, cbstyle=None):
-        """
-        Adds a fold panel to the list of panels.
-
-        :param `caption`: the caption to be displayed in the associated :class:`CaptionBar`;
-        :param `collapsed`: if set to ``True``, the panel is collapsed initially;
-        :param `foldIcons`: an instance of :class:`wx.ImageList` containing the icons to display
-         next to the caption text;
-        :param `cbstyle`: an instance of :class:`CaptionBarStyle`.
-
-        :note: The FoldPanel item which is returned, can be used as a reference to perform
-         actions upon the fold panel like collapsing it, expanding it, or deleting it
-         from the list. Use this foldpanel to add windows to it.
-
-        :see: :meth:`~FoldPanelBar.AddFoldPanelWindow` and :meth:`~FoldPanelBar.AddFoldPanelSeparator` to see how to add
-         items derived from :class:`wx.Window` to the panels.
-        """
-
-        if cbstyle is None:
-            cbstyle = EmptyCaptionBarStyle
-
-        # create a fold panel item, which is first only the caption.
-        # the user can now add a panel area which will be folded in
-        # when pressed.
-
-        if foldIcons is None:
-            foldIcons = wx.ImageList(16, 16)
-
-            bmp = ExpandedIcon.GetBitmap()
-            foldIcons.Add(bmp)
-            bmp = CollapsedIcon.GetBitmap()
-            foldIcons.Add(bmp)
-
-        item = FoldPanelItem(self._foldPanel, -1, caption=caption,
-                             foldIcons=foldIcons,
-                             collapsed=collapsed, cbstyle=cbstyle)
-
-        pos = 0
-        if len(self._panels) > 0:
-            pos = self._panels[-1].GetItemPos() + self._panels[-1].GetPanelLength()
-
-        item.Reposition(pos)
-        self._panels.append(item)
-
-        return item
-
-
-    def AddFoldPanelWindow(self, panel, window, flags=FPB_ALIGN_WIDTH,
-                           spacing=FPB_DEFAULT_SPACING,
-                           leftSpacing=FPB_DEFAULT_LEFTLINESPACING,
-                           rightSpacing=FPB_DEFAULT_RIGHTLINESPACING):
-        """
-        Adds a :class:`wx.Window` derived instance to the referenced fold panel.
-
-        :param `panel`: an instance of :class:`FoldPanelItem`;
-        :param `window`: the window we wish to add to the fold panel, an instance
-         of :class:`wx.Window`;
-        :param `flags`: can be one of the following bits:
-
-         ====================== ======= ====================================
-         Align Flag              Value  Description
-         ====================== ======= ====================================
-         ``FPB_ALIGN_WIDTH``          1 The :class:`wx.Window` to be added will be aligned to fit the width of the FoldPanel when it is resized. Very handy for sizer items, buttons and text boxes.
-         ``FPB_ALIGN_LEFT``           0 Aligns left instead of fitting the width of the child window to be added. Use either this one or ``FPB_ALIGN_WIDTH``.
-         ====================== ======= ====================================
-
-        :param `spacing`: the :class:`wx.Window` to be added can be slightly indented from
-         left and right so it is more visibly placed in the fold panel. Use `spacing` > 0
-         to give the control an y offset from the previous :class:`wx.Window` added;
-        :param `leftSpacing`: give the :class:`wx.Window` added a slight indent from the left;
-        :param `rightSpacing`: give the :class:`wx.Window` added a slight indent from the right;
-
-        :note: Make the window be a child of the fold panel!
-
-         The following example adds a FoldPanel to the :class:`FoldPanelBar` and
-         adds two :class:`wx.Window` derived controls to the FoldPanel::
-
-               # Create the FoldPanelBar
-               m_pnl = FoldPanelBar(self, wx.ID_ANY, wx.DefaultPosition, wx.DefaultSize, agwStyle=0x2)
-
-               # Add a foldpanel to the control. "Test me" is the caption and it is
-               # initially not collapsed.
-               item = m_pnl.AddFoldPanel("Test me", False)
-
-               # Now add a button to the fold panel. Mind that the button should be
-               # made child of the FoldPanel and not of the main form.
-               m_pnl.AddFoldPanelWindow(item, wx.Button(item, ID_COLLAPSEME, "Collapse Me"))
-
-               # Add a separator between the two controls. This is purely a visual
-               # line that can have a certain colour and also the indents and width
-               # aligning like a control.
-               m_pnl.AddFoldPanelSeparator(item)
-
-               # Now add a text ctrl. Also very easy. Align this on width so that
-               # when the control gets wider the text control also sizes along.
-               m_pnl.AddFoldPanelWindow(item, wx.TextCtrl(item, wx.ID_ANY, "Comment"), FPB_ALIGN_WIDTH, FPB_DEFAULT_SPACING, 20)
-
-        """
-
-        try:
-            item = self._panels.index(panel)
-        except:
-            raise Exception("ERROR: Invalid Panel Passed To AddFoldPanelWindow: " + repr(panel))
-
-        panel.AddWindow(window, flags, spacing, leftSpacing, rightSpacing)
-
-        # TODO: Take old and new height, and if difference, reposition all the lower
-        # panels this is because the user can add new wxWindow controls somewhere in
-        # between when other panels are already present.
-
-        return 0
-
-
-    def AddFoldPanelSeparator(self, panel, colour=wx.BLACK,
-                              spacing=FPB_DEFAULT_SPACING,
-                              leftSpacing=FPB_DEFAULT_LEFTLINESPACING,
-                              rightSpacing=FPB_DEFAULT_RIGHTLINESPACING):
-        """
-        Adds a separator line to the current fold panel.
-
-        The separator is a simple line which is drawn and is no real
-        component. It can be used to separate groups of controls
-        which belong to each other.
-
-        :param `colour`: the separator colour, an instance of :class:`wx.Colour`;
-        :param `spacing`: the separator to be added can be slightly indented from
-         left and right so it is more visibly placed in the fold panel. Use `spacing` > 0
-         to give the control an y offset from the previous :class:`wx.Window` added;
-        :param `leftSpacing`: give the added separator a slight indent from the left;
-        :param `rightSpacing`: give the added separator a slight indent from the right.
-        """
-
-        try:
-            item = self._panels.index(panel)
-        except:
-            raise Exception("ERROR: Invalid Panel Passed To AddFoldPanelSeparator: " + repr(panel))
-
-        panel.AddSeparator(colour, spacing, leftSpacing, rightSpacing)
-        return 0
-
-
-    def OnSizePanel(self, event):
-        """
-        Handles the ``wx.EVT_SIZE`` event for :class:`FoldPanelBar`.
-
-        :param `event`: a :class:`wx.SizeEvent` event to be processed.
-        """
-
-        # skip all stuff when we are not initialised yet
-
-        if not self._controlCreated:
-            event.Skip()
-            return
-
-        foldrect = self.GetRect()
-
-        # fold panel itself. If too little space,
-        # don't show it
-
-        foldrect.SetX(0)
-        foldrect.SetY(0)
-
-        self._foldPanel.SetSize(foldrect[2:])
-
-        if self._agwStyle & FPB_COLLAPSE_TO_BOTTOM or self._agwStyle & FPB_EXCLUSIVE_FOLD:
-            rect = self.RepositionCollapsedToBottom()
-            vertical = self.IsVertical()
-            if vertical and rect.GetHeight() > 0 or not vertical and rect.GetWidth() > 0:
-                self.RefreshRect(rect)
-
-        # TODO: A smart way to check wether the old - new width of the
-        # panel changed, if so no need to resize the fold panel items
-
-        self.RedisplayFoldPanelItems()
-
-
-    def OnPressCaption(self, event):
-        """
-        Handles the ``wx.EVT_CAPTIONBAR`` event for :class:`CaptionBar`.
-
-        :param `event`: a :class:`CaptionBarEvent` event to be processed.
-        """
-
-        # act upon the folding or expanding status of the bar
-        # to expand or collapse the panel(s)
-
-        if event.GetFoldStatus():
-            self.Collapse(event.GetTag())
-        else:
-            self.Expand(event.GetTag())
-
-
-
-    def RefreshPanelsFrom(self, item):
-        """
-        Refreshes all the panels from given one down to last one.
-
-        :param `item`: the first :class:`FoldPanelItem` to be refreshed.
-        """
-
-        try:
-            i = self._panels.index(item)
-        except:
-            raise Exception("ERROR: Invalid Panel Passed To RefreshPanelsFrom: " + repr(item))
-
-        self.Freeze()
-
-        # if collapse to bottom is on, the panels that are not expanded
-        # should be drawn at the bottom. All panels that are expanded
-        # are drawn on top. The last expanded panel gets all the extra space
-
-        if self._agwStyle & FPB_COLLAPSE_TO_BOTTOM or self._agwStyle & FPB_EXCLUSIVE_FOLD:
-
-            offset = 0
-
-            for panels in self._panels:
-
-                if panels.IsExpanded():
-                    offset = offset + panels.Reposition(offset) + 6  # 6px of padding
-
-            # put all non collapsed panels at the bottom where there is space,
-            # else put them right behind the expanded ones
-
-            self.RepositionCollapsedToBottom()
-
-        else:
-
-            pos = self._panels[i].GetItemPos() + self._panels[i].GetPanelLength()
-            for j in range(i+1, len(self._panels)):
-                pos = pos + self._panels[j].Reposition(pos) + 6  # 6px of padding
-
-        self.Thaw()
-
-
-    def RedisplayFoldPanelItems(self):
-        """ Resizes the fold panels so they match the width. """
-
-        # resize them all. No need to reposition
-        for panels in self._panels:
-            panels.ResizePanel()
-            panels.Refresh()
-
-
-    def RepositionCollapsedToBottom(self):
-        """
-        Repositions all the collapsed panels to the bottom.
-
-        When it is not possible to align them to the bottom, stick them behind
-        the visible panels.
-        """
-
-        value = wx.Rect(0,0,0,0)
-        vertical = self.IsVertical()
-
-        # determine wether the number of panels left
-        # times the size of their captions is enough
-        # to be placed in the left over space
-
-        expanded = 0
-        collapsed = 0
-        collapsed, expanded, values = self.GetPanelsLength(collapsed, expanded)
-
-        # if no room stick them behind the normal ones, else
-        # at the bottom
-
-        if (vertical and [self.GetSize().GetHeight()] or \
-            [self.GetSize().GetWidth()])[0] - expanded - collapsed < 0:
-            offset = expanded
-        else:
-
-            # value is the region which is left unpainted
-            # I will send it back as 'slack' so it does not need to
-            # be recalculated.
-
-            value.SetHeight(self.GetSize().GetHeight())
-            value.SetWidth(self.GetSize().GetWidth())
-
-            if vertical:
-                value.SetY(expanded)
-                value.SetHeight(value.GetHeight() - expanded)
-            else:
-                value.SetX(expanded)
-                value.SetWidth(value.GetWidth() - expanded)
-
-            offset = (vertical and [self.GetSize().GetHeight()] or \
-                      [self.GetSize().GetWidth()])[0] - collapsed
-
-
-        # go reposition
-
-        for panels in self._panels:
-            if not panels.IsExpanded():
-                offset = offset + panels.Reposition(offset)
-
-        return value
-
-
-    def GetPanelsLength(self, collapsed, expanded):
-        """
-        Returns the length of the panels that are expanded and
-        collapsed.
-
-        :param `collapsed`: the current value of the collapsed panels;
-        :param `expanded`: the current value of the expanded panels.
-
-        :note: This is useful to determine quickly what size is used to display,
-         and what is left at the bottom (right) to align the collapsed panels.
-        """
-
-        value = 0
-
-        # assumed here that all the panels that are expanded
-        # are positioned after each other from 0,0 to end.
-
-        for j in range(0, len(self._panels)):
-            offset = self._panels[j].GetPanelLength()
-            value = value + offset
-            if self._panels[j].IsExpanded():
-                expanded = expanded + offset
-            else:
-                collapsed = collapsed + offset
-
-        return collapsed, expanded, value
-
-
-    def Collapse(self, foldpanel):
-        """
-        Collapses the given fold panel reference, and updates the foldpanel bar.
-
-        :param `foldpanel`: an instance of :class:`FoldPanelItem`.
-
-        :note: With the ``FPB_COLLAPSE_TO_BOTTOM`` style set, all collapsed captions
-         are put at the bottom of the control. In the normal mode, they stay where
-         they are.
-        """
-
-        try:
-            item = self._panels.index(foldpanel)
-        except:
-            raise Exception("ERROR: Invalid Panel Passed To Collapse: " + repr(foldpanel))
-
-        foldpanel.Collapse()
-        self.RefreshPanelsFrom(foldpanel)
-
-
-    def Expand(self, foldpanel):
-        """
-        Expands the given fold panel reference, and updates the foldpanel bar.
-
-        :param `foldpanel`: an instance of :class:`FoldPanelItem`.
-
-        :note: With the ``FPB_COLLAPSE_TO_BOTTOM`` style set, they will be removed
-         from the bottom and the order where the panel originally was placed is
-         restored.
-        """
-
-        fpbextrastyle = 0
-
-        if self._agwStyle & FPB_SINGLE_FOLD or self._agwStyle & FPB_EXCLUSIVE_FOLD:
-            fpbextrastyle = 1
-            for panel in self._panels:
-                panel.Collapse()
-
-        foldpanel.Expand()
-
-        if fpbextrastyle:
-            if self._agwStyle & FPB_EXCLUSIVE_FOLD:
-                self.RepositionCollapsedToBottom()
-            self.RefreshPanelsFrom(self._panels[0])
-        else:
-            self.RefreshPanelsFrom(foldpanel)
-
-
-    def ApplyCaptionStyle(self, foldpanel, cbstyle):
-        """
-        Sets the style of the caption bar (:class:`CaptionBar`) of the fold panel.
-
-        :param `foldpanel`: an instance of :class:`FoldPanelItem`;
-        :param `cbstyle`: an instance of :class:`CaptionBarStyle`.
-
-        :note:
-
-         The changes are applied immediately. All styles not set in the
-         :class:`CaptionBarStyle` class are not applied. Use the :class:`CaptionBar` reference
-         to indicate what captionbar you want to apply the style to. To apply one
-         style to all :class:`CaptionBar` items, use :meth:`~FoldPanelBar.ApplyCaptionStyleAll`.
-        """
-
-        foldpanel.ApplyCaptionStyle(cbstyle)
-
-
-    def ApplyCaptionStyleAll(self, cbstyle):
-        """
-        Sets the style of all the caption bars of the fold panel.
-        The changes are applied immediately.
-
-        :param `cbstyle`: an instance of :class:`CaptionBarStyle`.
-        """
-
-        for panels in self._panels:
-            self.ApplyCaptionStyle(panels, cbstyle)
-
-
-    def GetCaptionStyle(self, foldpanel):
-        """
-        Returns the currently used caption style for the fold panel.
-
-        It is returned as a :class:`CaptionBarStyle` class. After modifying it, it can
-        be set again.
-
-        :param `foldpanel`: an instance of :class:`FoldPanelItem`.
-        """
-
-        return foldpanel.GetCaptionStyle()
-
-
-    def IsVertical(self):
-        """
-        Returns whether the :class:`CaptionBar` has default orientation or not.
-        Default is vertical.
-        """
-
-        return self._isVertical
-
-
-    def GetFoldPanel(self, item):
-        """
-        Returns the panel associated with the index `item`.
-
-        :param `item`: an integer representing the :class:`FoldPanelItem` in the list of
-         panels in this :class:`FoldPanelBar`.
-        """
-
-        try:
-            ind = self._panels[item]
-            return self._panels[item]
-        except:
-            raise Exception("ERROR: List Index Out Of Range Or Bad Item Passed: " + repr(item) + \
-                            ". Item Should Be An Integer Between " + repr(0) + " And " + \
-                            repr(len(self._panels)))
-
-
-    def GetCount(self):
-        """ Returns the number of panels in the :class:`FoldPanelBar`. """
-
-        try:
-            return len(self._panels)
-        except:
-            raise Exception("ERROR: No Panels Have Been Added To FoldPanelBar")
-
-
-
-# --------------------------------------------------------------------------------- #
-# class FoldPanelItem
-# --------------------------------------------------------------------------------- #
-
-class FoldPanelItem(wx.Panel):
-    """
-    This class is a child sibling of the :class:`FoldPanelBar` class. It will
-    contain a :class:`CaptionBar` class for receiving of events, and a the
-    rest of the area can be populated by a :class:`Panel` derived class.
-    """
-
-    def __init__(self, parent, id=wx.ID_ANY, caption="", foldIcons=None,
-                 collapsed=False, cbstyle=None):
-        """
-        Default class constructor.
-
-        :param `parent`: the :class:`FoldPanelItem` parent window;
-        :param `id`: an identifier for the control: a value of -1 is taken to mean a default;
-        :param `caption`: the string to be displayed in :class:`CaptionBar`;
-        :param `foldIcons`: an instance of :class:`wx.ImageList` containing the icons to display
-         next to the caption text;
-        :param `collapsed`: ``True`` if the :class:`CaptionBar` should start in the collapsed state,
-         ``False`` otherwise;
-        :param `cbstyle`: the :class:`CaptionBar` window style. Must be an instance of
-         :class:`CaptionBarStyle`.
-        """
-
-        wx.Panel.__init__(self, parent, id, wx.Point(0,0), style=wx.CLIP_CHILDREN)
-        self._controlCreated = False
-        self._UserSize = 0
-        self._PanelSize = 0
-        self._LastInsertPos = 0
-        self._itemPos = 0
-        self._userSized = False
-
-        if foldIcons is None:
-            foldIcons = wx.ImageList(16, 16)
-
-            bmp = ExpandedIcon.GetBitmap()
-            foldIcons.Add(bmp)
-            bmp = CollapsedIcon.GetBitmap()
-            foldIcons.Add(bmp)
-
-        self._foldIcons = foldIcons
-        if cbstyle is None:
-            cbstyle = EmptyCaptionBarStyle
-
-        # create the caption bar, in collapsed or expanded state
-
-        self._captionBar = CaptionBar(self, wx.ID_ANY, wx.Point(0,0),
-                                      size=wx.DefaultSize, caption=caption,
-                                      foldIcons=foldIcons, cbstyle=cbstyle)
-
-        if collapsed:
-            self._captionBar.Collapse()
-
-        self._controlCreated = True
-
-        # make initial size for component, if collapsed, the
-        # size is determined on the panel height and won't change
-
-        size = self._captionBar.GetSize() + wx.Size(0, 6)
-
-        self._PanelSize = (self.IsVertical() and [size.GetHeight()] or \
-                           [size.GetWidth()])[0]
-
-        self._LastInsertPos = self._PanelSize
-        self._items = []
-
-        self.Bind(EVT_CAPTIONBAR, self.OnPressCaption)
-        self.Bind(wx.EVT_PAINT, self.OnPaint)
-
-
-    def AddWindow(self, window, flags=FPB_ALIGN_WIDTH, spacing=FPB_DEFAULT_SPACING,
-                  leftSpacing=FPB_DEFAULT_LEFTLINESPACING,
-                  rightSpacing=FPB_DEFAULT_RIGHTLINESPACING):
-        """
-        Adds a window item to the list of items on this panel.
-
-        :param `window`: an instance of :class:`wx.Window`;
-        :param `flags`: can be one of the following bits:
-
-         ====================== ======= ====================================
-         Align Flag              Value  Description
-         ====================== ======= ====================================
-         ``FPB_ALIGN_WIDTH``          1 The :class:`wx.Window` to be added will be aligned to fit the width of the FoldPanel when it is resized. Very handy for sizer items, buttons and text boxes.
-         ``FPB_ALIGN_LEFT``           0 Aligns left instead of fitting the width of the child window to be added. Use either this one or ``FPB_ALIGN_WIDTH``.
-         ====================== ======= ====================================
-
-        :param `spacing`: reserves a number of pixels before the window element;
-        :param `leftSpacing`: an indent, in pixels;
-        :param `rightSpacing`: a right spacing, only relevant when the style
-         ``FPB_ALIGN_WIDTH`` is chosen.
-        """
-
-        wi = FoldWindowItem(self, window, Type="WINDOW", flags=flags, spacing=spacing,
-                            leftSpacing=leftSpacing, rightSpacing=rightSpacing)
-
-        self._items.append(wi)
-
-        vertical = self.IsVertical()
-
-        self._spacing = spacing
-        self._leftSpacing = leftSpacing
-        self._rightSpacing = rightSpacing
-
-        xpos = (vertical and [leftSpacing] or [self._LastInsertPos + spacing])[0]
-        ypos = (vertical and [self._LastInsertPos + spacing] or [leftSpacing])[0]
-
-        window.SetSize(xpos, ypos, -1, -1, wx.SIZE_USE_EXISTING)
-
-        self._LastInsertPos = self._LastInsertPos + wi.GetWindowLength(vertical)
-        self.ResizePanel()
-
-
-    def AddSeparator(self, colour=wx.BLACK, spacing=FPB_DEFAULT_SPACING,
-                     leftSpacing=FPB_DEFAULT_LEFTSPACING,
-                     rightSpacing=FPB_DEFAULT_RIGHTSPACING):
-        """
-        Adds a separator item to the list of items on this panel.
-
-        :param `colour`: the separator colour, an instance of :class:`wx.Colour`;
-        :param `spacing`: the separator to be added can be slightly indented from
-         left and right so it is more visibly placed in the fold panel. Use `spacing` > 0
-         to give the control an y offset from the previous :class:`wx.Window` added;
-        :param `leftSpacing`: give the added separator a slight indent from the left;
-        :param `rightSpacing`: give the added separator a slight indent from the right.
-        """
-
-        wi = FoldWindowItem(self, window=None, Type="SEPARATOR",
-                            flags=FPB_ALIGN_WIDTH, y=self._LastInsertPos,
-                            colour=colour, spacing=spacing, leftSpacing=leftSpacing,
-                            rightSpacing=rightSpacing)
-
-        self._items.append(wi)
-        self._LastInsertPos = self._LastInsertPos + \
-                              wi.GetWindowLength(self.IsVertical())
-
-        self.ResizePanel()
-
-
-    def Reposition(self, pos):
-        """
-        Repositions this :class:`FoldPanelItem` and reports the length occupied
-        for the next :class:`FoldPanelItem` in the list.
-
-        :param `pos`: the new item position.
-        """
-
-        # NOTE: Call Resize before Reposition when an item is added, because the new
-        # size needed will be calculated by Resize. Of course the relative position
-        # of the controls have to be correct in respect to the caption bar
-
-        self.Freeze()
-
-        vertical = self.IsVertical()
-        xpos = (vertical and [-1] or [pos])[0]
-        ypos = (vertical and [pos] or [-1])[0]
-
-        self.SetSize(xpos, ypos, -1, -1, wx.SIZE_USE_EXISTING)
-        self._itemPos = pos + 6  # Add 6px of padding to bottom of each item
-
-        self.Thaw()
-
-        return self.GetPanelLength()
-
-
-    def OnPressCaption(self, event):
-        """
-        Handles the ``wx.EVT_CAPTIONBAR`` event for :class:`FoldPanelItem`.
-
-        :param `event`: a :class:`CaptionBarEvent` event to be processed.
-        """
-
-        # tell the upper container we are responsible
-        # for this event, so it can fold the panel item
-        # and do a refresh
-
-        event.SetTag(self)
-        event.Skip()
-
-
-    def ResizePanel(self):
-        """ Resizes the panel. """
-
-        # prevent unnecessary updates by blocking repaints for a sec
-
-        self.Freeze()
-
-        vertical = self.IsVertical()
-        # force this panel to take the width of the parent panel and the y of the
-        # user or calculated width (which will be recalculated by the contents here)
-
-
-        if self._captionBar.IsCollapsed():
-            size = self._captionBar.GetSize()
-            self._PanelSize = (vertical and [size.GetHeight()] or [size.GetWidth()])[0]
-        else:
-            size = self.GetBestSize()
-            self._PanelSize = (vertical and [size.GetHeight()] or [size.GetWidth()])[0]
-
-            if self._UserSize:
-                if vertical:
-                    size.SetHeight(self._UserSize)
-                else:
-                    size.SetWidth(self._UserSize)
-
-        pnlsize = self.GetParent().GetSize()
-
-        if vertical:
-            size.SetWidth(pnlsize.GetWidth())
-        else:
-            size.SetHeight(pnlsize.GetHeight())
-
-        # resize caption bar
-        xsize = (vertical and [size.GetWidth()] or [-1])[0]
-        ysize = (vertical and [-1] or [size.GetHeight()])[0]
-
-        self._captionBar.SetSize((xsize, ysize))
-
-        # resize the panel
-        self.SetSize(size)
-
-        # go by all the controls and call Layout
-
-        for items in self._items:
-            items.ResizeItem((vertical and [size.GetWidth()] or \
-                              [size.GetHeight()])[0], vertical)
-
-        self.Thaw()
-
-
-    def OnPaint(self, event):
-        """
-        Handles the ``wx.EVT_PAINT`` event for :class:`FoldPanelItem`.
-
-        :param `event`: a :class:`PaintEvent` event to be processed.
-        """
-
-        # draw all the items that are lines
-
-        dc = wx.PaintDC(self)
-        vertical = self.IsVertical()
-
-        for item in self._items:
-
-            if item.GetType() == "SEPARATOR":
-                pen = wx.Pen(item.GetLineColour(), 1, wx.PENSTYLE_SOLID)
-                dc.SetPen(pen)
-                a = item.GetLeftSpacing()
-                b = item.GetLineY() + item.GetSpacing()
-                c = item.GetLineLength()
-                d = a + c
-
-                if vertical:
-                    dc.DrawLine(a, b, d, b)
-                else:
-                    dc.DrawLine(b, a, b, d)
-
-        event.Skip()
-
-
-    def IsVertical(self):
-        """
-        Returns whether the :class:`CaptionBar` has default orientation or not.
-        Default is vertical.
-        """
-
-        # grandparent of FoldPanelItem is FoldPanelBar
-        # default is vertical
-
-        if isinstance(self.GetGrandParent(), FoldPanelBar):
-            return self.GetGrandParent().IsVertical()
-        else:
-            raise Exception("ERROR: Wrong Parent " + repr(self.GetGrandParent()))
-
-
-    def IsExpanded(self):
-        """
-        Returns expanded or collapsed status.  If the panel is
-        expanded, ``True`` is returned.
-        """
-
-        return not self._captionBar.IsCollapsed()
-
-
-    def GetItemPos(self):
-        """ Returns item's position. """
-
-        return self._itemPos
-
-
-    def Collapse(self):
-        """
-        Internal method.
-
-        This should not be called by the user, because it doesn't trigger the
-        parent  to tell it that we are collapsed or expanded, it only changes
-        visual state.
-        """
-
-        self._captionBar.Collapse()
-        self.ResizePanel()
-
-
-    def Expand(self):
-        """
-        Internal method.
-
-        This should not be called by the user, because it doesn't trigger the
-        parent to tell it that we are collapsed or expanded, it only changes
-        visual state.
-        """
-
-        self._captionBar.Expand()
-        self.ResizePanel()
-
-
-    def GetPanelLength(self):
-        """ Returns size of panel. """
-
-        if self._captionBar.IsCollapsed():
-            return self.GetCaptionLength()
-        elif self._userSized:
-            return self._UserSize
-
-        return self._PanelSize
-
-
-    def GetCaptionLength(self):
-        """ Returns height of caption only. This is for folding calculation purposes. """
-
-        size = self._captionBar.GetSize()
-        return (self.IsVertical() and [size.GetHeight()] or [size.GetWidth()])[0]
-
-
-    def ApplyCaptionStyle(self, cbstyle):
-        """ Applies the style defined in `cbstyle` to the :class:`CaptionBar`."""
-
-        self._captionBar.SetCaptionStyle(cbstyle)
-
-
-    def GetCaptionStyle(self):
-        """
-        Returns the current style of the captionbar in a :class:`CaptionBarStyle` class.
-
-        This can be used to change and set back the changes.
-        """
-
-        return self._captionBar.GetCaptionStyle()
-
-
-# ----------------------------------------------------------------------------------- #
-# class FoldWindowItem
-# ----------------------------------------------------------------------------------- #
-
-class FoldWindowItem(object):
-    """
-    This class is a child sibling of the :class:`FoldPanelItem` class. It
-    will contain :class:`wx.Window` that can be either a separator (a coloured
-    line simulated by a :class:`wx.Window`) or a wxPython controls (such as a
-    :class:`Button`, a :class:`ListCtrl` etc...).
-    """
-
-    def __init__(self, parent, window=None, **kw):
-        """
-        Default class constructor
-
-        :param `parent`: the :class:`FoldWindowItem` parent;
-        :param `window`: the window contained in this item.
-
-        :keyword `Type`: can be "WINDOW" or "SEPARATOR";
-        :keyword `lineColour`: the separator colour (meaningful for separators only);
-        :keyword `y`: the separator y position (meaningful for separators only);
-        :keyword `flags`: the alignment flags;
-        :keyword `spacing`: reserves a number of pixels before the window/separator element;
-        :keyword `leftSpacing`: an indent, in pixels;
-        :keyword `rightSpacing`: a right spacing, only relevant when the style
-         ``FPB_ALIGN_WIDTH`` is chosen.
-
-        :see: :meth:`FoldPanelBar.AddFoldPanelWindow() <FoldPanelBar.AddFoldPanelWindow>` for a list of valid alignment flags.
-        """
-
-        if "Type" not in kw:
-            raise Exception('ERROR: Missing Window Type Information. This Should Be "WINDOW" Or "SEPARATOR"')
-
-        if kw.get("Type") == "WINDOW":
-            # Window constructor. This initialises the class as a wx.Window Type
-
-            if "flags" in kw:
-                self._flags = kw.get("flags")
-            else:
-                self._flags = FPB_ALIGN_WIDTH
-            if "spacing" in kw:
-                self._spacing = kw.get("spacing")
-            else:
-                self._spacing = FPB_DEFAULT_SPACING
-            if "leftSpacing" in kw:
-                self._leftSpacing = kw.get("leftSpacing")
-            else:
-                self._leftSpacing = FPB_DEFAULT_LEFTSPACING
-            if "rightSpacing" in kw:
-                self._rightSpacing = kw.get("rightSpacing")
-            else:
-                self._rightSpacing = FPB_DEFAULT_RIGHTSPACING
-
-            self._lineY = 0
-            self._sepLineColour = None
-            self._wnd = window
-
-
-        elif kw.get("Type") == "SEPARATOR":
-            # separator constructor. This initialises the class as a separator type
-
-            if "y" in kw:
-                self._lineY = kw.get("y")
-            else:
-                raise Exception("ERROR: Undefined Y Position For The Separator")
-            if "lineColour" in kw:
-                self._sepLineColour = kw.get("lineColour")
-            else:
-                self._sepLineColour = wx.BLACK
-            if "flags" in kw:
-                self._flags = kw.get("flags")
-            else:
-                self._flags = FPB_ALIGN_WIDTH
-            if "spacing" in kw:
-                self._spacing = kw.get("spacing")
-            else:
-                self._spacing = FPB_DEFAULT_SPACING
-            if "leftSpacing" in kw:
-                self._leftSpacing = kw.get("leftSpacing")
-            else:
-                self._leftSpacing = FPB_DEFAULT_LEFTSPACING
-            if "rightSpacing" in kw:
-                self._rightSpacing = kw.get("rightSpacing")
-            else:
-                self._rightSpacing = FPB_DEFAULT_RIGHTSPACING
-
-            self._wnd = window
-
-        else:
-            raise Exception("ERROR: Undefined Window Type Selected: " + repr(kw.get("Type")))
-
-        self._type = kw.get("Type")
-        self._lineLength = 0
-
-
-    def GetType(self):
-        """ Returns the :class:`FoldWindowItem` type. """
-
-        return self._type
-
-
-    def GetLineY(self):
-        """ Returns the y position of the separator. """
-
-        return self._lineY
-
-
-    def GetLineLength(self):
-        """ Returns the separator line length. """
-
-        return self._lineLength
-
-
-    def GetLineColour(self):
-        """ Returns the separator line colour. """
-
-        return self._sepLineColour
-
-
-    def GetLeftSpacing(self):
-        """ Returns the left indent of :class:`FoldWindowItem`. """
-
-        return self._leftSpacing
-
-
-    def GetRightSpacing(self):
-        """ Returns the right indent of :class:`FoldWindowItem`. """
-
-        return self._rightSpacing
-
-
-    def GetSpacing(self):
-        """ Returns the spacing of :class:`FoldWindowItem`. """
-
-        return self._spacing
-
-
-    def GetWindowLength(self, vertical=True):
-        """
-        Returns space needed by the window if type is :class:`FoldWindowItem`
-        "WINDOW" and returns the total size plus the extra spacing.
-
-        :param `vertical`: ``True`` if the parent :class:`FoldPanelBar` is in vertical
-         mode.
-        """
-
-        value = 0
-        if self._type == "WINDOW":
-            size = self._wnd.GetSize()
-            value = (vertical and [size.GetHeight()] or [size.GetWidth()])[0] + \
-                    self._spacing
-
-        elif self._type == "SEPARATOR":
-            value = 1 + self._spacing
-
-        return value
-
-
-    def ResizeItem(self, size, vertical=True):
-        """
-        Resizes the element, whatever it is.
-
-        A separator or line will be always aligned by width or height
-        depending on orientation of the whole panel.
-
-        :param `size`: the maximum size available for the :class:`FoldWindowItem`;
-        :param `vertical`: ``True`` if the parent :class:`FoldPanelBar` is in vertical
-         mode.
-        """
-
-        if self._flags & FPB_ALIGN_WIDTH:
-            # align by taking full width
-            mySize = size - self._leftSpacing - self._rightSpacing
-
-            if mySize < 0:
-                mySize = 10  # can't have negative width
-
-            if self._type == "SEPARATOR":
-                self._lineLength = mySize
-            else:
-                xsize = (vertical and [mySize] or [-1])[0]
-                ysize = (vertical and [-1] or [mySize])[0]
-
-                self._wnd.SetSize((xsize, ysize))
-
-
-if __name__ == '__main__':
-
-    import wx
-
-    class MyFrame(wx.Frame):
-
-        def __init__(self, parent):
-
-            wx.Frame.__init__(self, parent, -1, "FoldPanelBar Demo")
-
-            text_ctrl = wx.TextCtrl(self, -1, size=(400, 100), style=wx.TE_MULTILINE)
-
-            panel_bar = FoldPanelBar(self, -1, agwStyle=FPB_VERTICAL)
-
-            fold_panel = panel_bar.AddFoldPanel("Thing")
-            thing = wx.TextCtrl(fold_panel, -1, size=(400, -1), style=wx.TE_MULTILINE)
-
-            panel_bar.AddFoldPanelWindow(fold_panel, thing)
-
-            main_sizer = wx.BoxSizer(wx.VERTICAL)
-            main_sizer.Add(text_ctrl, 1, wx.EXPAND)
-            main_sizer.Add(panel_bar, 1, wx.EXPAND)
-            self.SetSizer(main_sizer)
-
-
-    # our normal wxApp-derived class, as usual
-
-    app = wx.App(0)
-
-    frame = MyFrame(None)
-    app.SetTopWindow(frame)
-    frame.Show()
-
-    app.MainLoop()
+# --------------------------------------------------------------------------- #
+# FOLDPANELBAR wxPython IMPLEMENTATION
+# Ported From Jorgen Bodde & Julian Smart (Extended Demo) C++ Code By:
+#
+# Andrea Gavana, @ 23 Mar 2005
+# Latest Revision: 16 Jul 2012, 15.00 GMT
+# 
+# Edited version in gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
+#
+# TODO List
+#
+# All The C++ TODOs Are Still Alive. I Am Not Able to Read Jorges's Mind
+# So I Don't Really Know What Will Be The New Features/Additions He Will
+# Make On His Code. At The Moment They Are:
+#
+# 1. OnPaint Function In CaptionBar Class:
+# TODO: Maybe First A Memory Dc Should Draw All, And Then Paint It On The
+# Caption. This Way A Flickering Arrow During Resize Is Not Visible.
+#
+# 2. OnChar Function In CaptionBar Class:
+# TODO: This Is Easy To Do But I Don't Have Any Useful Idea On Which Kind
+# Of Features To Add. Does Anyone Have An Intelligent Idea?
+#
+# 3. AddFoldPanelWindow Function In FoldPanelBar Class:
+# TODO: Take Old And New Heights, And If Difference, Reposition All The
+# Lower Panels. This Is Because The User Can Add New wxWindow Controls
+# Somewhere In Between When Other Panels Are Already Present.
+# Don't Know What It Means. Probably Is My Poor English...
+#
+# 4. OnSizePanel Function In FoldPanelBar Class:
+# TODO: A Smart Way To Check Wether The Old - New Width Of The
+# Panel Changed, If So No Need To Resize The Fold Panel Items
+#
+#
+# DONE List:
+#
+# 1. Implemented Styles Like FPB_SINGLE_FOLD and FPB_EXCLUSIVE_FOLD
+# Thanks To E. A. Tacao For His Nice Suggestions.
+#
+# 2. Added Some Maquillage To FoldPanelBar: When The Mouse Enters The Icon
+# Region, It Is Changed To wx.CURSOR_HAND.
+#
+#
+# For The Original TODO List From Jorgen, Please Refer To:
+# http://www.solidsteel.nl/jorg/components/foldpanel/wxFoldPanelBar.php#todo_list
+#
+#
+#
+# For All Kind Of Problems, Requests Of Enhancements And Bug Reports, Please
+# Write To Me At:
+#
+# andrea.gavana@gmail.com
+# andrea.gavana@maerskoil.com
+#
+# Or, Obviously, To The wxPython Mailing List!!!
+#
+# Tags:        phoenix-port, unittest, documented, py3-port
+#
+# End Of Comments
+# --------------------------------------------------------------------------- #
+
+
+"""
+:class:`~wx.lib.agw.foldpanelbar.FoldPanelBar` is a control that contains multiple panels, which can be expanded
+or collapsed.
+
+
+Description
+===========
+
+The :class:`FoldPanelBar` is a control that contains multiple panels (of type
+:class:`FoldPanelItem`) that can be expanded or collapsed. The captionbar of
+the :class:`FoldPanelBar` can be customized by setting it to a horizontal gradient
+style, vertical gradient style, a single colour, a rectangle or filled
+rectangle. The `FoldPanel` items can be collapsed in place or to the
+bottom of the control. :class:`wx.Window` derived controls can be added
+dynamically, and separated by separator lines.
+
+
+How does it work
+----------------
+
+The internals of the :class:`FoldPanelBar` is a list of :class:`FoldPanelItem` objects. Through
+the reference of `FoldPanel` these panels can be controlled by adding new controls
+to a FoldPanel or adding new FoldPanels to the :class:`FoldPanelBar`.
+
+The :class:`CaptionBar` fires events to the parent (container of all panel items) when a
+sub-panel needs resizing (either folding or expanding). The fold or expand process
+is simply a resize of the panel so it looks like all controls on it are gone. All
+controls are still child of the `FoldPanel` they are located on. If they don't
+handle the event (and they won't) then the owner of the :class:`FoldPanelBar` gets the
+events.
+
+This is what you need to handle the controls. There isn't much to it just
+a lot of calculations to see what panel belongs where. There are no sizers
+involved in the panels, everything is purely x-y positioning.
+
+
+What can it do and what not?
+----------------------------
+
+a) What it can do:
+
+   * Run-time addition of panels (no deletion just yet);
+   * Run time addition of controls to the panel (it will be resized accordingly);
+   * Creating panels in collapsed mode or expanded mode;
+   * Various modes of caption behaviour and filling to make it more appealing;
+   * Panels can be folded and collapsed (or all of them) to allow more space.
+
+b) What it cannot do:
+
+   * Selection of a panel like in a listctrl;
+   * Dragging and dropping the panels;
+   * Re-ordering the panels (not yet).
+
+
+Usage
+=====
+
+Usage example::
+
+    import wx
+    import wx.lib.agw.foldpanelbar as fpb
+
+    class MyFrame(wx.Frame):
+
+        def __init__(self, parent):
+
+            wx.Frame.__init__(self, parent, -1, "FoldPanelBar Demo")
+
+            text_ctrl = wx.TextCtrl(self, -1, size=(400, 100), style=wx.TE_MULTILINE)
+
+            panel_bar = fpb.FoldPanelBar(self, -1, agwStyle=fpb.FPB_VERTICAL)
+
+            fold_panel = panel_bar.AddFoldPanel("Thing")
+            thing = wx.TextCtrl(fold_panel, -1, size=(400, -1), style=wx.TE_MULTILINE)
+
+            panel_bar.AddFoldPanelWindow(fold_panel, thing)
+
+            main_sizer = wx.BoxSizer(wx.VERTICAL)
+            main_sizer.Add(text_ctrl, 1, wx.EXPAND)
+            main_sizer.Add(panel_bar, 1, wx.EXPAND)
+            self.SetSizer(main_sizer)
+
+
+    # our normal wxApp-derived class, as usual
+
+    app = wx.App(0)
+
+    frame = MyFrame(None)
+    app.SetTopWindow(frame)
+    frame.Show()
+
+    app.MainLoop()
+
+
+
+Supported Platforms
+===================
+
+:class:`FoldPanelBar` is supported on the following platforms:
+  * Windows (Verified on Windows XP, 2000)
+  * Linux/Unix (GTK2) (Thanks to Toni Brkic and Robin Dunn)
+  * Mac OSX (Thanks to Robin Dunn for the :class:`CaptionBar` size patch)
+
+
+Window Styles
+=============
+
+This class supports the following window styles:
+
+========================== =========== ==================================================
+Window Styles              Hex Value   Description
+========================== =========== ==================================================
+``FPB_SINGLE_FOLD``                0x1 Single fold forces other panels to close when they are open, and only opens the current panel. This will allow the open panel to gain the full size left in the client area.
+``FPB_COLLAPSE_TO_BOTTOM``         0x2 All panels are stacked to the bottom. When they are expanded again they show up at the top.
+``FPB_EXCLUSIVE_FOLD``             0x4 ``FPB_SINGLE_FOLD`` style plus the panels will be stacked at the bottom.
+``FPB_HORIZONTAL``                 0x8 :class:`FoldPanelBar` will be horizontal.
+``FPB_VERTICAL``                  0x10 :class:`FoldPanelBar` will be vertical.
+========================== =========== ==================================================
+
+
+Events Processing
+=================
+
+This class processes the following events:
+
+================== ==================================================
+Event Name         Description
+================== ==================================================
+``EVT_CAPTIONBAR`` The user has pressed the caption bar: :class:`FoldPanelBar` will either expand or collapse the underlying panel.
+================== ==================================================
+
+
+License And Version
+===================
+
+:class:`FoldPanelBar` is distributed under the wxPython license.
+
+Latest Revision: Andrea Gavana @ 16 Jul 2012, 15.00 GMT
+
+Version 0.6
+
+"""
+
+import wx
+
+from .constants import FOLDPANEL_BG_COLOR
+    
+#----------------------------------------------------------------------
+# Collapsed And Expanded Bitmap Images
+# Created With img2py.py
+#----------------------------------------------------------------------
+from wx.lib.embeddedimage import PyEmbeddedImage
+
+CollapsedIcon = PyEmbeddedImage(
+    "iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABHNCSVQICAgIfAhkiAAAADdJ"
+    "REFUOI1jZGRiZqAEMFGke/Ab8P/f3/8D5wKY7YRcQRsXoNuKzxXUdwEu23CJU+wCxtG8wAAA"
+    "mvUb+vltJD8AAAAASUVORK5CYII=")
+
+ExpandedIcon = PyEmbeddedImage(
+    "iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABHNCSVQICAgIfAhkiAAAAEJJ"
+    "REFUOI1jZGRiZqAEMFGke1AYwIIu8P/f3/+4FDMyMTNS3QUYBmCzBZ84bQIR3TZcttPOBci2"
+    "4rOdKi5gHM0LDACevARXGc9htQAAAABJRU5ErkJggg==")
+
+#----------------------------------------------------------------------
+# FOLDPANELBAR Starts Here
+#----------------------------------------------------------------------
+
+# CAPTIONBAR STYLES
+#
+#- CAPTIONBAR_GRADIENT_V: Draws a vertical gradient from top to bottom
+#- CAPTIONBAR_GRADIENT_H: Draws a horizontal gradient from left to right
+#- CAPTIONBAR_SINGLE: Draws a single filled rectangle to draw the caption
+#- CAPTIONBAR_RECTANGLE: Draws a single colour with a rectangle around the caption
+#- CAPTIONBAR_FILLED_RECTANGLE: Draws a filled rectangle and a border around it
+
+CAPTIONBAR_NOSTYLE            = 0
+""" The :class:`CaptionBar` has no style bit set. """
+CAPTIONBAR_GRADIENT_V         = 1
+""" Draws a vertical gradient from top to bottom. """
+CAPTIONBAR_GRADIENT_H         = 2
+""" Draws a vertical gradient from left to right. """
+CAPTIONBAR_SINGLE             = 3
+""" Draws a single filled rectangle to draw the caption. """
+CAPTIONBAR_RECTANGLE          = 4
+""" Draws a single colour with a rectangle around the caption. """
+CAPTIONBAR_FILLED_RECTANGLE   = 5
+""" Draws a filled rectangle and a border around it. """
+
+FPB_EXTRA_X = 10
+""" Extra horizontal padding, in pixels. """
+FPB_EXTRA_Y = 8
+""" Extra vertical padding, in pixels. """
+
+# pixels of the bmp to be aligned from the right filled with space
+FPB_BMP_RIGHTSPACE = 2
+""" Pixels of the bmp to be aligned from the right filled with space. """
+
+# Now supported! Single fold forces
+# other panels to close when they are open, and only opens the current panel.
+# This will allow the open panel to gain the full size left in the client area
+FPB_SINGLE_FOLD = 0x0001
+""" Single fold forces other panels to close when they are open, and only opens the current panel. This will allow the open panel to gain the full size left in the client area."""
+
+# All panels are stacked to the bottom. When they are expanded again they
+# show up at the top
+FPB_COLLAPSE_TO_BOTTOM = 0x0002
+""" All panels are stacked to the bottom. When they are expanded again they show up at the top. """
+
+# Now supported! Single fold plus panels
+# will be stacked at the bottom
+FPB_EXCLUSIVE_FOLD = 0x0004
+""" ``FPB_SINGLE_FOLD`` style plus the panels will be stacked at the bottom. """
+
+# Orientation Flag
+FPB_HORIZONTAL = 0x0008
+""" :class:`FoldPanelBar` will be horizontal. """
+FPB_VERTICAL = 0x0010
+""" :class:`FoldPanelBar` will be vertical. """
+
+# FoldPanelItem default settings
+FPB_ALIGN_LEFT = 0
+""" Aligns left instead of fitting the width of the child window to be added. Use either this one or ``FPB_ALIGN_WIDTH``. """
+FPB_ALIGN_WIDTH = 1
+""" The :class:`wx.Window` to be added will be aligned to fit the width of the FoldPanel when it is resized. Very handy for sizer items, buttons and text boxes. """
+
+FPB_DEFAULT_LEFTSPACING = 10
+FPB_DEFAULT_RIGHTSPACING = 10
+FPB_DEFAULT_SPACING = 8
+
+FPB_DEFAULT_LEFTLINESPACING = 20
+FPB_DEFAULT_RIGHTLINESPACING = 20
+
+
+# ------------------------------------------------------------------------------ #
+# class CaptionBarStyle
+# ------------------------------------------------------------------------------ #
+
+class CaptionBarStyle(object):
+    """
+    This class encapsulates the styles you wish to set for the
+    :class:`CaptionBar` (this is the part of the `FoldPanel` where the caption
+    is displayed). It can either be applied at creation time be
+    reapplied when styles need to be changed.
+
+    At construction time, all styles are set to their default
+    transparency.  This means none of the styles will be applied to
+    the :class:`CaptionBar` in question, meaning it will be created using the
+    default internals. When setting i.e the colour, font or panel
+    style, these styles become active to be used.
+    """
+
+    def __init__(self):
+        """ Default constructor for this class. """
+
+        self.ResetDefaults()
+
+
+    def ResetDefaults(self):
+        """ Resets default :class:`CaptionBarStyle`. """
+        self._firstColourUsed = False
+        self._secondColourUsed = False
+        self._textColourUsed = False
+        self._captionFontUsed = False
+        self._captionStyleUsed = False
+        self._captionStyle = CAPTIONBAR_GRADIENT_V
+
+
+    # ------- CaptionBar Font -------
+
+    def SetCaptionFont(self, font):
+        """
+        Sets font for the caption bar.
+
+        :param `font`: a valid :class:`wx.Font` object.
+
+        :note: If this is not set, the font property is undefined and will not be used.
+         Use :meth:`~CaptionBarStyle.CaptionFontUsed` to check if this style is used.
+        """
+
+        self._captionFont = font
+        self._captionFontUsed = True
+
+
+    def CaptionFontUsed(self):
+        """ Checks if the caption bar font is set. """
+
+        return self._captionFontUsed
+
+
+    def GetCaptionFont(self):
+        """
+        Returns the font for the caption bar.
+
+        :note: Please be warned this will result in an assertion failure when
+         this property is not previously set.
+
+        :see: :meth:`~CaptionBarStyle.SetCaptionFont`, :meth:`~CaptionBarStyle.CaptionFontUsed`
+        """
+
+        return self._captionFont
+
+
+    # ------- First Colour -------
+
+    def SetFirstColour(self, colour):
+        """
+        Sets first colour for the caption bar.
+
+        :param `colour`: a valid :class:`wx.Colour` object.
+
+        :note: If this is not set, the colour property is undefined and will not be used.
+         Use :meth:`~CaptionBarStyle.FirstColourUsed` to check if this style is used.
+        """
+
+        self._firstColour = colour
+        self._firstColourUsed = True
+
+
+    def FirstColourUsed(self):
+        """ Checks if the first colour of the caption bar is set."""
+
+        return self._firstColourUsed
+
+
+    def GetFirstColour(self):
+        """
+        Returns the first colour for the caption bar.
+
+        :note: Please be warned this will result in an assertion failure when
+         this property is not previously set.
+
+        :see: :meth:`~CaptionBarStyle.SetFirstColour`, :meth:`~CaptionBarStyle.FirstColourUsed`
+        """
+
+        return self._firstColour
+
+
+    # ------- Second Colour -------
+
+    def SetSecondColour(self, colour):
+        """
+        Sets second colour for the caption bar.
+
+        :param `colour`: a valid :class:`wx.Colour` object.
+
+        :note: If this is not set, the colour property is undefined and will not be used.
+         Use :meth:`~CaptionBarStyle.SecondColourUsed` to check if this style is used.
+        """
+
+        self._secondColour = colour
+        self._secondColourUsed = True
+
+
+    def SecondColourUsed(self):
+        """ Checks if the second colour of the caption bar is set."""
+
+        return self._secondColourUsed
+
+
+    def GetSecondColour(self):
+        """
+        Returns the second colour for the caption bar.
+
+        :note: Please be warned this will result in an assertion failure when
+         this property is not previously set.
+
+        :see: :meth:`~CaptionBarStyle.SetSecondColour`, :meth:`~CaptionBarStyle.SecondColourUsed`
+        """
+
+        return self._secondColour
+
+
+    # ------- Caption Text Colour -------
+
+    def SetCaptionColour(self, colour):
+        """
+        Sets caption colour for the caption bar.
+
+        :param `colour`: a valid :class:`wx.Colour` object.
+
+        :note: If this is not set, the colour property is undefined and will not be used.
+         Use :meth:`~CaptionBarStyle.CaptionColourUsed` to check if this style is used.
+        """
+
+        self._textColour = colour
+        self._textColourUsed = True
+
+
+    def CaptionColourUsed(self):
+        """ Checks if the caption colour of the caption bar is set."""
+
+        return self._textColourUsed
+
+
+    def GetCaptionColour(self):
+        """
+        Returns the caption colour for the caption bar.
+
+        :note: Please be warned this will result in an assertion failure
+         when this property is not previously set.
+
+        :see: :meth:`~CaptionBarStyle.SetCaptionColour`, :meth:`~CaptionBarStyle.CaptionColourUsed`
+        """
+
+        return self._textColour
+
+
+    # ------- CaptionStyle  -------
+
+    def SetCaptionStyle(self, style):
+        """
+        Sets caption style for the caption bar.
+
+        :param `style`: can be one of the following bits:
+
+         =============================== ======= =============================
+         Caption Style                    Value  Description
+         =============================== ======= =============================
+         ``CAPTIONBAR_GRADIENT_V``             1 Draws a vertical gradient from top to bottom
+         ``CAPTIONBAR_GRADIENT_H``             2 Draws a horizontal gradient from left to right
+         ``CAPTIONBAR_SINGLE``                 3 Draws a single filled rectangle to draw the caption
+         ``CAPTIONBAR_RECTANGLE``              4 Draws a single colour with a rectangle around the caption
+         ``CAPTIONBAR_FILLED_RECTANGLE``       5 Draws a filled rectangle and a border around it
+         =============================== ======= =============================
+
+        :note: If this is not set, the property is undefined and will not be used.
+         Use :meth:`~CaptionBarStyle.CaptionStyleUsed` to check if this style is used.
+        """
+
+        self._captionStyle = style
+        self._captionStyleUsed = True
+
+
+    def CaptionStyleUsed(self):
+        """ Checks if the caption style of the caption bar is set."""
+
+        return self._captionStyleUsed
+
+
+    def GetCaptionStyle(self):
+        """
+        Returns the caption style for the caption bar.
+
+        :note: Please be warned this will result in an assertion failure
+         when this property is not previously set.
+
+        :see: :meth:`~CaptionBarStyle.SetCaptionStyle`, :meth:`~CaptionBarStyle.CaptionStyleUsed`
+        """
+
+        return self._captionStyle
+
+
+#-----------------------------------#
+#        CaptionBarEvent
+#-----------------------------------#
+wxEVT_CAPTIONBAR = wx.NewEventType()
+EVT_CAPTIONBAR = wx.PyEventBinder(wxEVT_CAPTIONBAR, 0)
+""" The user has pressed the caption bar: :class:`FoldPanelBar` will either expand or""" \
+""" collapse the underlying panel. """
+
+# Define Empty CaptionBar Style
+EmptyCaptionBarStyle = CaptionBarStyle()
+
+# ---------------------------------------------------------------------------- #
+# class CaptionBarEvent
+# ---------------------------------------------------------------------------- #
+
+class CaptionBarEvent(wx.CommandEvent):
+    """
+    This event will be sent when a ``EVT_CAPTIONBAR`` is mapped in the parent.
+    It is to notify the parent that the bar is now in collapsed or expanded
+    state. The parent should re-arrange the associated windows accordingly
+    """
+
+    def __init__(self, evtType):
+        """
+        Default class constructor.
+
+        :param `evtType`: the event type.
+        """
+
+        wx.CommandEvent.__init__(self, evtType)
+
+
+    def GetFoldStatus(self):
+        """
+        Returns whether the bar is expanded or collapsed. ``True`` means
+        expanded.
+        """
+
+        return not self._bar.IsCollapsed()
+
+
+    def GetBar(self):
+        """ Returns the selected :class:`CaptionBar`. """
+
+        return self._bar
+
+
+    def SetTag(self, tag):
+        """
+        Assigns a tag to the selected :class:`CaptionBar`.
+
+        :param `tag`: an instance of :class:`FoldPanelBar`.
+        """
+
+        self._tag = tag
+
+
+    def GetTag(self):
+        """ Returns the tag assigned to the selected :class:`CaptionBar`. """
+
+        return self._tag
+
+
+    def SetBar(self, bar):
+        """
+        Sets the bar associated with this event.
+
+        :param `bar`: an instance of :class:`CaptionBar`.
+
+        :note: Should not be used by any other than the originator of the event.
+        """
+
+        self._bar = bar
+
+
+# -------------------------------------------------------------------------------- #
+# class CaptionBar
+# -------------------------------------------------------------------------------- #
+
+class CaptionBar(wx.Window):
+    """
+    This class is a graphical caption component that consists of a
+    caption and a clickable arrow.
+
+    The :class:`CaptionBar` fires an event ``EVT_CAPTIONBAR`` which is a
+    :class:`CaptionBarEvent`. This event can be caught and the parent window
+    can act upon the collapsed or expanded state of the bar (which is
+    actually just the icon which changed). The parent panel can
+    reduce size or expand again.
+    """
+
+    def __init__(self, parent, id, pos, size, caption="",
+                 foldIcons=None, cbstyle=None,
+                 rightIndent=FPB_BMP_RIGHTSPACE,
+                 iconWidth=16, iconHeight=16, collapsed=False):
+        """
+        Default class constructor.
+
+        :param `parent`: the :class:`CaptionBar` parent window;
+        :param `id`: an identifier for the control: a value of -1 is taken to mean a default;
+        :param `pos`: the control position. A value of (-1, -1) indicates a default position,
+         chosen by either the windowing system or wxPython, depending on platform;
+        :param `size`: the control size. A value of (-1, -1) indicates a default size,
+         chosen by either the windowing system or wxPython, depending on platform;
+        :param `caption`: the string to be displayed in :class:`CaptionBar`;
+        :param `foldIcons`: an instance of :class:`wx.ImageList` containing the icons to display
+         next to the caption text;
+        :param `cbstyle`: the :class:`CaptionBar` window style. Must be an instance of
+         :class:`CaptionBarStyle`;
+        :param `rightIndent`: number of pixels of the bmp to be aligned from the right filled
+         with space;
+        :param `iconWidth`: the :class:`CaptionBar` icon width;
+        :param `iconHeight`: the :class:`CaptionBar` icon height;
+        :param `collapsed`: ``True`` if the :class:`CaptionBar` should start in the collapsed state,
+         ``False`` otherwise.
+        """
+
+        wx.Window.__init__(self, parent, wx.ID_ANY, pos=pos,
+                           size=(20,20), style=wx.NO_BORDER)
+
+        self._controlCreated = False
+        self._collapsed = collapsed
+        self.ApplyCaptionStyle(cbstyle, True)
+
+        if foldIcons is None:
+            foldIcons = wx.ImageList(16, 16)
+
+            bmp = ExpandedIcon.GetBitmap()
+            foldIcons.Add(bmp)
+            bmp = CollapsedIcon.GetBitmap()
+            foldIcons.Add(bmp)
+
+        # set initial size
+        if foldIcons:
+            assert foldIcons.GetImageCount() > 1
+            iconWidth, iconHeight = foldIcons.GetSize(0)
+
+        self._caption = caption
+        self._foldIcons = foldIcons
+        self._style = cbstyle
+        self._rightIndent = rightIndent
+        self._iconWidth = iconWidth
+        self._iconHeight = iconHeight
+        self._oldSize = wx.Size(20,20)
+
+        self._controlCreated = True
+        
+        self.SetBackgroundColour(FOLDPANEL_BG_COLOR)
+
+        self.Bind(wx.EVT_PAINT, self.OnPaint)
+        self.Bind(wx.EVT_SIZE, self.OnSize)
+        self.Bind(wx.EVT_MOUSE_EVENTS, self.OnMouseEvent)
+        self.Bind(wx.EVT_CHAR, self.OnChar)
+
+
+    def ApplyCaptionStyle(self, cbstyle=None, applyDefault=True):
+        """
+        Applies the style defined in `cbstyle` to the :class:`CaptionBar`.
+
+        :param `cbstyle`: an instance of :class:`CaptionBarStyle`;
+        :param `applyDefault`: if ``True``, the colours used in the :class:`CaptionBarStyle`
+         will be reset to their default values.
+        """
+
+        if cbstyle is None:
+            cbstyle = EmptyCaptionBarStyle
+
+        newstyle = cbstyle
+
+        if applyDefault:
+
+            # get first colour from style or make it default
+            if not newstyle.FirstColourUsed():
+                newstyle.SetFirstColour(wx.WHITE)
+
+            # get second colour from style or make it default
+            if not newstyle.SecondColourUsed():
+                # make the second colour slightly darker then the background
+                colour = self.GetParent().GetBackgroundColour()
+                r, g, b = int(colour.Red()), int(colour.Green()), int(colour.Blue())
+                colour = ((r >> 1) + 20, (g >> 1) + 20, (b >> 1) + 20)
+                newstyle.SetSecondColour(wx.Colour(colour[0], colour[1], colour[2]))
+
+            # get text colour
+            if not newstyle.CaptionColourUsed():
+                newstyle.SetCaptionColour(wx.BLACK)
+
+            # get font colour
+            if not newstyle.CaptionFontUsed():
+                newstyle.SetCaptionFont(self.GetParent().GetFont())
+
+            # apply caption style
+            if not newstyle.CaptionStyleUsed():
+                newstyle.SetCaptionStyle(CAPTIONBAR_GRADIENT_V)
+
+        self._style = newstyle
+
+
+    def SetCaptionStyle(self, cbstyle=None, applyDefault=True):
+        """
+        Sets :class:`CaptionBar` styles with :class:`CaptionBarStyle` class.
+
+        :param `cbstyle`: an instance of :class:`CaptionBarStyle`;
+        :param `applyDefault`: if ``True``, the colours used in the :class:`CaptionBarStyle`
+         will be reset to their default values.
+
+        :note: All styles that are actually set, are applied. If you set `applyDefault`
+         to ``True``, all other (not defined) styles will be set to default. If it is
+         ``False``, the styles which are not set in the :class:`CaptionBarStyle` will be ignored.
+        """
+
+        if cbstyle is None:
+            cbstyle = EmptyCaptionBarStyle
+
+        self.ApplyCaptionStyle(cbstyle, applyDefault)
+        self.Refresh()
+
+
+    def GetCaptionStyle(self):
+        """
+        Returns the current style of the captionbar in a :class:`CaptionBarStyle` class.
+
+        :note: This can be used to change and set back the changes.
+        """
+
+        return self._style
+
+
+    def IsCollapsed(self):
+        """ Returns wether the status of the bar is expanded or collapsed. """
+
+        return self._collapsed
+
+
+    def SetRightIndent(self, pixels):
+        """
+        Sets the amount of pixels on the right from which the bitmap
+        is trailing.
+
+        :param `pixels`: the number of pixels on the right from which the bitmap
+         is trailing. If this is 0, it will be drawn all the way to the right,
+         default is equal to ``FPB_BMP_RIGHTSPACE``. Assign this before
+         assigning an image list to prevent a redraw.
+        """
+
+        assert pixels >= 0
+        self._rightIndent = pixels
+        if self._foldIcons:
+            self.Refresh()
+
+
+    def Collapse(self):
+        """
+        This sets the internal state/representation to collapsed.
+
+        :note: This does not trigger a :class:`CaptionBarEvent` to be sent to the
+         parent.
+        """
+
+        self._collapsed = True
+        self.RedrawIconBitmap()
+
+
+    def Expand(self):
+        """
+        This sets the internal state/representation to expanded.
+
+        :note: This does not trigger a :class:`CaptionBarEvent` to be sent to the
+         parent.
+        """
+
+        self._collapsed = False
+        self.RedrawIconBitmap()
+
+
+    def SetBoldFont(self):
+        """ Sets the :class:`CaptionBar` font weight to bold."""
+
+        self.GetFont().SetWeight(wx.FONTWEIGHT_BOLD)
+
+
+    def SetNormalFont(self):
+        """ Sets the :class:`CaptionBar` font weight to normal."""
+
+        self.GetFont().SetWeight(wx.FONTWEIGHT_NORMAL)
+
+
+    def IsVertical(self):
+        """
+        Returns wether the :class:`CaptionBar` has a default orientation or not.
+        Default is vertical.
+        """
+
+        fld = self.GetParent().GetGrandParent()
+        if isinstance(fld, FoldPanelBar):
+            return self.GetParent().GetGrandParent().IsVertical()
+        else:
+            raise Exception("ERROR: Wrong Parent " + repr(fld))
+
+
+    def OnPaint(self, event):
+        """
+        Handles the ``wx.EVT_PAINT`` event for :class:`CaptionBar`.
+
+        :param `event`: a :class:`PaintEvent` event to be processed.
+        """
+
+        if not self._controlCreated:
+            event.Skip()
+            return
+
+        dc = wx.PaintDC(self)
+        wndRect = self.GetRect()
+        vertical = self.IsVertical()
+
+        # TODO: Maybe first a memory DC should draw all, and then paint it on
+        # the caption. This way a flickering arrow during resize is not visible
+
+        self.FillCaptionBackground(dc)
+        dc.SetFont(self._style.GetCaptionFont())
+        dc.SetTextForeground(self._style.GetCaptionColour())
+
+        # draw small icon, either collapsed or expanded
+        # based on the state of the bar. If we have any bmp's
+
+        if self._foldIcons:
+
+            index = self._collapsed
+
+            if vertical:
+                drw = self._iconWidth - self._rightIndent - 10
+                self._foldIcons.Draw(index, dc, drw,
+                                     (wndRect.GetHeight() - self._iconHeight)//2,
+                                     wx.IMAGELIST_DRAW_TRANSPARENT)
+            else:
+                self._foldIcons.Draw(index, dc,
+                                     (wndRect.GetWidth() - self._iconWidth)//2,
+                                     self._rightIndent, wx.IMAGELIST_DRAW_TRANSPARENT)
+
+        else:
+            pass
+
+        txt_w, txt_h = dc.GetTextExtent(self._caption)
+
+        if vertical:
+            dc.DrawText(self._caption,
+                        10 + self._rightIndent + self._iconWidth,
+                        FPB_EXTRA_Y//2)
+        else:
+            dc.DrawRotatedText(self._caption, FPB_EXTRA_Y//2,
+                               wndRect.GetBottom() - 4, 90)
+
+##        event.Skip()
+
+
+    def FillCaptionBackground(self, dc):
+        """
+        Fills the background of the caption with either a gradient or
+        a solid colour.
+
+        :param `dc`: an instance of :class:`wx.DC`.
+        """
+
+        style = self._style.GetCaptionStyle()
+
+        if style == CAPTIONBAR_GRADIENT_V:
+            if self.IsVertical():
+                self.DrawVerticalGradient(dc, self.GetRect())
+            else:
+                self.DrawHorizontalGradient(dc, self.GetRect())
+
+        elif style == CAPTIONBAR_GRADIENT_H:
+            if self.IsVertical():
+                self.DrawHorizontalGradient(dc, self.GetRect())
+            else:
+                self.DrawVerticalGradient(dc, self.GetRect())
+
+        elif style == CAPTIONBAR_SINGLE:
+            self.DrawSingleColour(dc, self.GetRect())
+        elif style == CAPTIONBAR_RECTANGLE or style == CAPTIONBAR_FILLED_RECTANGLE:
+            self.DrawSingleRectangle(dc, self.GetRect())
+        else:
+            raise Exception("STYLE Error: Undefined Style Selected: " + repr(style))
+
+
+    def OnMouseEvent(self, event):
+        """
+        Handles the ``wx.EVT_MOUSE_EVENTS`` event for :class:`CaptionBar`.
+
+        :param `event`: a :class:`MouseEvent` event to be processed.
+
+        :note: This method catches the mouse click-double click. If clicked on
+         the arrow (single) or double on the caption we change state and an event
+         must be fired to let this panel collapse or expand.
+        """
+
+        send_event = False
+        vertical = self.IsVertical()
+
+        if event.LeftDown() and self._foldIcons:
+
+            pt = event.GetPosition()
+            rect = self.GetRect()
+
+            drw = 0
+            if vertical and pt.x > 0 or not vertical and \
+               pt.y < (self._iconHeight + self._rightIndent):
+                send_event = True
+
+        elif event.LeftDClick():
+            # self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
+            send_event = True
+
+        # elif event.Entering() and self._foldIcons:
+        #     self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
+
+        #     pt = event.GetPosition()
+        #     rect = self.GetRect()
+
+        #     drw = 0
+        #     if vertical and pt.x > drw or not vertical and \
+        #        pt.y < (self._iconHeight + self._rightIndent):
+        #         self.SetCursor(wx.Cursor(wx.CURSOR_HAND))
+        #     else:
+        #         self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
+
+        # elif event.Leaving():
+        #     self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
+
+        # elif event.Moving():
+        #     pt = event.GetPosition()
+        #     rect = self.GetRect()
+
+        #     drw = 0
+        #     if vertical and pt.x > drw or not vertical and \
+        #        pt.y < (self._iconHeight + self._rightIndent):
+        #         self.SetCursor(wx.Cursor(wx.CURSOR_HAND))
+        #     else:
+        #         self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
+
+        # send the collapse, expand event to the parent
+
+        if send_event:
+            event = CaptionBarEvent(wxEVT_CAPTIONBAR)
+            event.SetId(self.GetId())
+            event.SetEventObject(self)
+            event.SetBar(self)
+            self.GetEventHandler().ProcessEvent(event)
+
+
+    def OnChar(self, event):
+        """
+        Handles the ``wx.EVT_CHAR`` event for :class:`CaptionBar`.
+
+        :param `event`: a :class:`KeyEvent` event to be processed.
+
+        :note: This method currently does nothing.
+        """
+
+        # TODO: Anything here?
+        event.Skip()
+
+
+    def DoGetBestSize(self):
+        """
+        Returns the best size for this panel, based upon the font
+        assigned to this window, and the caption string.
+
+        :note: Overridden from :class:`wx.Window`.
+        """
+
+        if self.IsVertical():
+            x, y = self.GetTextExtent(self._caption)
+        else:
+            y, x = self.GetTextExtent(self._caption)
+
+        if x < self._iconWidth:
+            x = self._iconWidth
+
+        if y < self._iconHeight:
+            y = self._iconHeight
+
+        # TODO: The extra FPB_EXTRA_X constants should be adjustable as well
+
+        return wx.Size(x + FPB_EXTRA_X, y + FPB_EXTRA_Y)
+
+
+    # def DrawVerticalGradient(self, dc, rect):
+    #     """
+    #     Gradient fill from colour 1 to colour 2 from top to bottom.
+
+    #     :param `dc`: an instance of :class:`wx.DC`;
+    #     :param `rect`: the :class:`CaptionBar` client rectangle.
+    #     """
+
+    #     if  rect.height < 1 or rect.width < 1:
+    #         return
+
+    #     dc.SetPen(wx.TRANSPARENT_PEN)
+
+    #     # calculate gradient coefficients
+    #     col2 = self._style.GetSecondColour()
+    #     col1 = self._style.GetFirstColour()
+
+    #     r1, g1, b1 = int(col1.Red()), int(col1.Green()), int(col1.Blue())
+    #     r2, g2, b2 = int(col2.Red()), int(col2.Green()), int(col2.Blue())
+
+    #     flrect = float(rect.height)
+
+    #     rstep = float((r2 - r1)) / flrect
+    #     gstep = float((g2 - g1)) / flrect
+    #     bstep = float((b2 - b1)) / flrect
+
+    #     rf, gf, bf = 0, 0, 0
+
+    #     for y in range(rect.y, rect.y + rect.height):
+    #         currCol = (r1 + rf, g1 + gf, b1 + bf)
+
+    #         dc.SetBrush(wx.Brush(currCol, wx.BRUSHSTYLE_SOLID))
+    #         dc.DrawRoundedRectangle(rect.x, rect.y + (y - rect.y), rect.width, rect.height, 4)
+    #         rf = rf + rstep
+    #         gf = gf + gstep
+    #         bf = bf + bstep
+
+
+    # def DrawHorizontalGradient(self, dc, rect):
+    #     """
+    #     Gradient fill from colour 1 to colour 2 from left to right.
+
+    #     :param `dc`: an instance of :class:`wx.DC`;
+    #     :param `rect`: the :class:`CaptionBar` client rectangle.
+    #     """
+
+    #     if rect.height < 1 or rect.width < 1:
+    #         return
+
+    #     dc.SetPen(wx.TRANSPARENT_PEN)
+
+    #     # calculate gradient coefficients
+    #     col2 = self._style.GetSecondColour()
+    #     col1 = self._style.GetFirstColour()
+
+    #     r1, g1, b1 = int(col1.Red()), int(col1.Green()), int(col1.Blue())
+    #     r2, g2, b2 = int(col2.Red()), int(col2.Green()), int(col2.Blue())
+
+    #     flrect = float(rect.width)
+
+    #     rstep = float((r2 - r1)) / flrect
+    #     gstep = float((g2 - g1)) / flrect
+    #     bstep = float((b2 - b1)) / flrect
+
+    #     rf, gf, bf = 0, 0, 0
+
+    #     for x in range(rect.x, rect.x + rect.width):
+    #         currCol = (r1 + rf, g1 + gf, b1 + bf)
+
+    #         dc.SetBrush(wx.Brush(currCol, wx.BRUSHSTYLE_SOLID))
+    #         dc.DrawRectangle(rect.x + (x - rect.x), rect.y, 1, rect.height)
+    #         rf = rf + rstep
+    #         gf = gf + gstep
+    #         bf = bf + bstep
+
+
+    def DrawSingleColour(self, dc, rect):
+        """
+        Single colour fill for :class:`CaptionBar`.
+
+        :param `dc`: an instance of :class:`wx.DC`;
+        :param `rect`: the :class:`CaptionBar` client rectangle.
+        """
+
+        if rect.height < 1 or rect.width < 1:
+            return
+
+        dc.SetPen(wx.TRANSPARENT_PEN)
+
+        # draw simple rectangle
+        dc.SetBrush(wx.Brush(self._style.GetFirstColour(), wx.BRUSHSTYLE_SOLID))
+        dc.DrawRoundedRectangle(rect.x, rect.y, rect.width, rect.height, 4)
+
+        if self.IsCollapsed() is not True:
+            dc.DrawRectangle(rect.x, rect.y+rect.height-2, rect.width, 4)
+
+
+    # def DrawSingleRectangle(self, dc, rect):
+    #     """
+    #     Single rectangle for :class:`CaptionBar`.
+
+    #     :param `dc`: an instance of :class:`wx.DC`;
+    #     :param `rect`: the :class:`CaptionBar` client rectangle.
+    #     """
+
+    #     if rect.height < 2 or rect.width < 1:
+    #         return
+
+    #     # single frame, set up internal fill colour
+
+    #     if self._style.GetCaptionStyle() == CAPTIONBAR_RECTANGLE:
+    #         colour = self.GetParent().GetBackgroundColour()
+    #         br = wx.Brush(colour, wx.BRUSHSTYLE_SOLID)
+    #     else:
+    #         colour = self._style.GetFirstColour()
+    #         br = wx.Brush(colour, wx.BRUSHSTYLE_SOLID)
+
+    #     # setup the pen frame
+
+    #     pen = wx.Pen(self._style.GetSecondColour())
+    #     dc.SetPen(pen)
+    #     dc.SetBrush(br)
+    #     dc.DrawRoundedRectangle(rect.x, rect.y, rect.width, rect.height - 1, 4)
+
+    #     bgpen = wx.Pen(self.GetParent().GetBackgroundColour())
+    #     dc.SetPen(bgpen)
+    #     dc.DrawLine(rect.x, rect.y + rect.height - 1, rect.x + rect.width,
+    #                 rect.y + rect.height - 1)
+
+
+    def OnSize(self, event):
+        """
+        Handles the ``wx.EVT_SIZE`` event for :class:`CaptionBar`.
+
+        :param `event`: a :class:`wx.SizeEvent` event to be processed.
+        """
+
+        if not self._controlCreated:
+            event.Skip()
+            return
+
+        size = event.GetSize()
+
+        if self._foldIcons:
+
+            # What I am doing here is simply invalidating the part of the window
+            # exposed. So when I make a rect with as width the newly exposed part,
+            # and the x,y of the old window size origin, I don't need a bitmap
+            # calculation in it, or do I ? The bitmap needs redrawing anyway.
+            # Leave it like this until I figured it out.
+
+            # set rect to redraw as old bitmap area which is entitled to redraw
+
+            rect = wx.Rect(size.GetWidth() - self._iconWidth - self._rightIndent, 0,
+                           self._iconWidth + self._rightIndent,
+                           self._iconWidth + self._rightIndent)
+
+            # adjust rectangle when more is slided so we need to redraw all
+            # the old stuff but not all (ugly flickering)
+
+            diffX = size.GetWidth() - self._oldSize.GetWidth()
+
+            if diffX > 1:
+
+                # adjust the rect with all the crap to redraw
+
+                rect.SetWidth(rect.GetWidth() + diffX + 10)
+                rect.SetX(rect.GetX() - diffX - 10)
+
+            self.RefreshRect(rect)
+
+        else:
+
+            rect = self.GetRect()
+            self.RefreshRect(rect)
+
+        self._oldSize = size
+
+
+    def RedrawIconBitmap(self):
+        """ Redraws the icons (if they exists). """
+
+        if self._foldIcons:
+
+            # invalidate the bitmap area and force a redraw
+
+            rect = self.GetRect()
+
+            rect.SetX(rect.GetWidth() - self._iconWidth - self._rightIndent)
+            rect.SetWidth(self._iconWidth + self._rightIndent)
+            self.RefreshRect(rect)
+
+
+# ---------------------------------------------------------------------------------- #
+# class FoldPanelBar
+# ---------------------------------------------------------------------------------- #
+
+class FoldPanelBar(wx.Panel):
+    """
+    The :class:`FoldPanelBar` is a class which can maintain a list of
+    collapsible panels. Once a panel is collapsed, only it's caption
+    bar is visible to the user. This will provide more space for the
+    other panels, or allow the user to close panels which are not used
+    often to get the most out of the work area.
+
+    This control is easy to use. Simply create it as a child for a
+    panel or sash window, and populate panels with
+    :meth:`FoldPanelBar.AddFoldPanel() <FoldPanelBar.AddFoldPanel>`. Then use the
+    :meth:`FoldPanelBar.AddFoldPanelWindow() <FoldPanelBar.AddFoldPanelWindow>` to add
+    :class:`wx.Window` derived controls to the current fold panel. Use
+    :meth:`FoldPanelBar.AddFoldPanelSeparator() <FoldPanelBar.AddFoldPanelSeparator>` to put separators between the groups of
+    controls that need a visual separator to group them
+    together. After all is constructed, the user can fold the panels
+    by double clicking on the bar or single click on the arrow, which
+    will indicate the collapsed or expanded state.
+    """
+
+    def __init__(self, parent, id=-1, pos=wx.DefaultPosition, size=wx.DefaultSize,
+                 style=wx.TAB_TRAVERSAL|wx.NO_BORDER, agwStyle=0):
+        """
+        Default class constructor.
+
+        :param `parent`: the :class:`FoldPanelBar` parent window;
+        :param `id`: an identifier for the control: a value of -1 is taken to mean a default;
+        :param `pos`: the control position. A value of (-1, -1) indicates a default position,
+         chosen by either the windowing system or wxPython, depending on platform;
+        :param `size`: the control size. A value of (-1, -1) indicates a default size,
+         chosen by either the windowing system or wxPython, depending on platform;
+        :param `style`: the underlying :class:`Panel` window style;
+        :param `agwStyle`: the AGW-specific :class:`FoldPanelBar` window style. It can be one of the
+         following bits:
+
+         ========================== =========== ==================================================
+         Window Styles              Hex Value   Description
+         ========================== =========== ==================================================
+         ``FPB_SINGLE_FOLD``                0x1 Single fold forces other panels to close when they are open, and only opens the current panel. This will allow the open panel to gain the full size left in the client area.
+         ``FPB_COLLAPSE_TO_BOTTOM``         0x2 All panels are stacked to the bottom. When they are expanded again they show up at the top.
+         ``FPB_EXCLUSIVE_FOLD``             0x4 ``FPB_SINGLE_FOLD`` style plus the panels will be stacked at the bottom.
+         ``FPB_HORIZONTAL``                 0x4 :class:`FoldPanelBar` will be horizontal.
+         ``FPB_VERTICAL``                   0x8 :class:`FoldPanelBar` will be vertical.
+         ========================== =========== ==================================================
+        """
+
+        self._controlCreated = False
+
+        # make sure there is any orientation
+        if not agwStyle & (FPB_HORIZONTAL | FPB_VERTICAL):
+            agwStyle = agwStyle | FPB_VERTICAL
+
+        if agwStyle & FPB_HORIZONTAL:
+            self._isVertical = False
+        else:
+            self._isVertical = True
+
+        self._agwStyle = agwStyle
+
+        # create the panel (duh!). This causes a size event, which we are going
+        # to skip when we are not initialised
+
+        wx.Panel.__init__(self, parent, id, pos, size, style)
+
+        # the fold panel area
+
+        self._foldPanel = wx.Panel(self, wx.ID_ANY, pos, size,
+                                   wx.NO_BORDER | wx.TAB_TRAVERSAL)
+
+        self._controlCreated = True
+        self._panels = []
+
+        self.Bind(EVT_CAPTIONBAR, self.OnPressCaption)
+        self.Bind(wx.EVT_SIZE, self.OnSizePanel)
+
+
+    def AddFoldPanel(self, caption="", collapsed=False, foldIcons=None, cbstyle=None):
+        """
+        Adds a fold panel to the list of panels.
+
+        :param `caption`: the caption to be displayed in the associated :class:`CaptionBar`;
+        :param `collapsed`: if set to ``True``, the panel is collapsed initially;
+        :param `foldIcons`: an instance of :class:`wx.ImageList` containing the icons to display
+         next to the caption text;
+        :param `cbstyle`: an instance of :class:`CaptionBarStyle`.
+
+        :note: The FoldPanel item which is returned, can be used as a reference to perform
+         actions upon the fold panel like collapsing it, expanding it, or deleting it
+         from the list. Use this foldpanel to add windows to it.
+
+        :see: :meth:`~FoldPanelBar.AddFoldPanelWindow` and :meth:`~FoldPanelBar.AddFoldPanelSeparator` to see how to add
+         items derived from :class:`wx.Window` to the panels.
+        """
+
+        if cbstyle is None:
+            cbstyle = EmptyCaptionBarStyle
+
+        # create a fold panel item, which is first only the caption.
+        # the user can now add a panel area which will be folded in
+        # when pressed.
+
+        if foldIcons is None:
+            foldIcons = wx.ImageList(16, 16)
+
+            bmp = ExpandedIcon.GetBitmap()
+            foldIcons.Add(bmp)
+            bmp = CollapsedIcon.GetBitmap()
+            foldIcons.Add(bmp)
+
+        item = FoldPanelItem(self._foldPanel, -1, caption=caption,
+                             foldIcons=foldIcons,
+                             collapsed=collapsed, cbstyle=cbstyle)
+
+        pos = 0
+        if len(self._panels) > 0:
+            pos = self._panels[-1].GetItemPos() + self._panels[-1].GetPanelLength()
+
+        item.Reposition(pos)
+        self._panels.append(item)
+
+        return item
+
+
+    def AddFoldPanelWindow(self, panel, window, flags=FPB_ALIGN_WIDTH,
+                           spacing=FPB_DEFAULT_SPACING,
+                           leftSpacing=FPB_DEFAULT_LEFTLINESPACING,
+                           rightSpacing=FPB_DEFAULT_RIGHTLINESPACING):
+        """
+        Adds a :class:`wx.Window` derived instance to the referenced fold panel.
+
+        :param `panel`: an instance of :class:`FoldPanelItem`;
+        :param `window`: the window we wish to add to the fold panel, an instance
+         of :class:`wx.Window`;
+        :param `flags`: can be one of the following bits:
+
+         ====================== ======= ====================================
+         Align Flag              Value  Description
+         ====================== ======= ====================================
+         ``FPB_ALIGN_WIDTH``          1 The :class:`wx.Window` to be added will be aligned to fit the width of the FoldPanel when it is resized. Very handy for sizer items, buttons and text boxes.
+         ``FPB_ALIGN_LEFT``           0 Aligns left instead of fitting the width of the child window to be added. Use either this one or ``FPB_ALIGN_WIDTH``.
+         ====================== ======= ====================================
+
+        :param `spacing`: the :class:`wx.Window` to be added can be slightly indented from
+         left and right so it is more visibly placed in the fold panel. Use `spacing` > 0
+         to give the control an y offset from the previous :class:`wx.Window` added;
+        :param `leftSpacing`: give the :class:`wx.Window` added a slight indent from the left;
+        :param `rightSpacing`: give the :class:`wx.Window` added a slight indent from the right;
+
+        :note: Make the window be a child of the fold panel!
+
+         The following example adds a FoldPanel to the :class:`FoldPanelBar` and
+         adds two :class:`wx.Window` derived controls to the FoldPanel::
+
+               # Create the FoldPanelBar
+               m_pnl = FoldPanelBar(self, wx.ID_ANY, wx.DefaultPosition, wx.DefaultSize, agwStyle=0x2)
+
+               # Add a foldpanel to the control. "Test me" is the caption and it is
+               # initially not collapsed.
+               item = m_pnl.AddFoldPanel("Test me", False)
+
+               # Now add a button to the fold panel. Mind that the button should be
+               # made child of the FoldPanel and not of the main form.
+               m_pnl.AddFoldPanelWindow(item, wx.Button(item, ID_COLLAPSEME, "Collapse Me"))
+
+               # Add a separator between the two controls. This is purely a visual
+               # line that can have a certain colour and also the indents and width
+               # aligning like a control.
+               m_pnl.AddFoldPanelSeparator(item)
+
+               # Now add a text ctrl. Also very easy. Align this on width so that
+               # when the control gets wider the text control also sizes along.
+               m_pnl.AddFoldPanelWindow(item, wx.TextCtrl(item, wx.ID_ANY, "Comment"), FPB_ALIGN_WIDTH, FPB_DEFAULT_SPACING, 20)
+
+        """
+
+        try:
+            item = self._panels.index(panel)
+        except:
+            raise Exception("ERROR: Invalid Panel Passed To AddFoldPanelWindow: " + repr(panel))
+
+        panel.AddWindow(window, flags, spacing, leftSpacing, rightSpacing)
+
+        # TODO: Take old and new height, and if difference, reposition all the lower
+        # panels this is because the user can add new wxWindow controls somewhere in
+        # between when other panels are already present.
+
+        return 0
+
+
+    def AddFoldPanelSeparator(self, panel, colour=wx.BLACK,
+                              spacing=FPB_DEFAULT_SPACING,
+                              leftSpacing=FPB_DEFAULT_LEFTLINESPACING,
+                              rightSpacing=FPB_DEFAULT_RIGHTLINESPACING):
+        """
+        Adds a separator line to the current fold panel.
+
+        The separator is a simple line which is drawn and is no real
+        component. It can be used to separate groups of controls
+        which belong to each other.
+
+        :param `colour`: the separator colour, an instance of :class:`wx.Colour`;
+        :param `spacing`: the separator to be added can be slightly indented from
+         left and right so it is more visibly placed in the fold panel. Use `spacing` > 0
+         to give the control an y offset from the previous :class:`wx.Window` added;
+        :param `leftSpacing`: give the added separator a slight indent from the left;
+        :param `rightSpacing`: give the added separator a slight indent from the right.
+        """
+
+        try:
+            item = self._panels.index(panel)
+        except:
+            raise Exception("ERROR: Invalid Panel Passed To AddFoldPanelSeparator: " + repr(panel))
+
+        panel.AddSeparator(colour, spacing, leftSpacing, rightSpacing)
+        return 0
+
+
+    def OnSizePanel(self, event):
+        """
+        Handles the ``wx.EVT_SIZE`` event for :class:`FoldPanelBar`.
+
+        :param `event`: a :class:`wx.SizeEvent` event to be processed.
+        """
+
+        # skip all stuff when we are not initialised yet
+
+        if not self._controlCreated:
+            event.Skip()
+            return
+
+        foldrect = self.GetRect()
+
+        # fold panel itself. If too little space,
+        # don't show it
+
+        foldrect.SetX(0)
+        foldrect.SetY(0)
+
+        self._foldPanel.SetSize(foldrect[2:])
+
+        if self._agwStyle & FPB_COLLAPSE_TO_BOTTOM or self._agwStyle & FPB_EXCLUSIVE_FOLD:
+            rect = self.RepositionCollapsedToBottom()
+            vertical = self.IsVertical()
+            if vertical and rect.GetHeight() > 0 or not vertical and rect.GetWidth() > 0:
+                self.RefreshRect(rect)
+
+        # TODO: A smart way to check wether the old - new width of the
+        # panel changed, if so no need to resize the fold panel items
+
+        self.RedisplayFoldPanelItems()
+
+
+    def OnPressCaption(self, event):
+        """
+        Handles the ``wx.EVT_CAPTIONBAR`` event for :class:`CaptionBar`.
+
+        :param `event`: a :class:`CaptionBarEvent` event to be processed.
+        """
+
+        # act upon the folding or expanding status of the bar
+        # to expand or collapse the panel(s)
+
+        if event.GetFoldStatus():
+            self.Collapse(event.GetTag())
+        else:
+            self.Expand(event.GetTag())
+
+
+
+    def RefreshPanelsFrom(self, item):
+        """
+        Refreshes all the panels from given one down to last one.
+
+        :param `item`: the first :class:`FoldPanelItem` to be refreshed.
+        """
+
+        try:
+            i = self._panels.index(item)
+        except:
+            raise Exception("ERROR: Invalid Panel Passed To RefreshPanelsFrom: " + repr(item))
+
+        self.Freeze()
+
+        # if collapse to bottom is on, the panels that are not expanded
+        # should be drawn at the bottom. All panels that are expanded
+        # are drawn on top. The last expanded panel gets all the extra space
+
+        if self._agwStyle & FPB_COLLAPSE_TO_BOTTOM or self._agwStyle & FPB_EXCLUSIVE_FOLD:
+
+            offset = 0
+
+            for panels in self._panels:
+
+                if panels.IsExpanded():
+                    offset = offset + panels.Reposition(offset) + 6  # 6px of padding
+
+            # put all non collapsed panels at the bottom where there is space,
+            # else put them right behind the expanded ones
+
+            self.RepositionCollapsedToBottom()
+
+        else:
+
+            pos = self._panels[i].GetItemPos() + self._panels[i].GetPanelLength()
+            for j in range(i+1, len(self._panels)):
+                pos = pos + self._panels[j].Reposition(pos) + 6  # 6px of padding
+
+        self.Thaw()
+
+
+    def RedisplayFoldPanelItems(self):
+        """ Resizes the fold panels so they match the width. """
+
+        # resize them all. No need to reposition
+        for panels in self._panels:
+            panels.ResizePanel()
+            panels.Refresh()
+
+
+    def RepositionCollapsedToBottom(self):
+        """
+        Repositions all the collapsed panels to the bottom.
+
+        When it is not possible to align them to the bottom, stick them behind
+        the visible panels.
+        """
+
+        value = wx.Rect(0,0,0,0)
+        vertical = self.IsVertical()
+
+        # determine wether the number of panels left
+        # times the size of their captions is enough
+        # to be placed in the left over space
+
+        expanded = 0
+        collapsed = 0
+        collapsed, expanded, values = self.GetPanelsLength(collapsed, expanded)
+
+        # if no room stick them behind the normal ones, else
+        # at the bottom
+
+        if (vertical and [self.GetSize().GetHeight()] or \
+            [self.GetSize().GetWidth()])[0] - expanded - collapsed < 0:
+            offset = expanded
+        else:
+
+            # value is the region which is left unpainted
+            # I will send it back as 'slack' so it does not need to
+            # be recalculated.
+
+            value.SetHeight(self.GetSize().GetHeight())
+            value.SetWidth(self.GetSize().GetWidth())
+
+            if vertical:
+                value.SetY(expanded)
+                value.SetHeight(value.GetHeight() - expanded)
+            else:
+                value.SetX(expanded)
+                value.SetWidth(value.GetWidth() - expanded)
+
+            offset = (vertical and [self.GetSize().GetHeight()] or \
+                      [self.GetSize().GetWidth()])[0] - collapsed
+
+
+        # go reposition
+
+        for panels in self._panels:
+            if not panels.IsExpanded():
+                offset = offset + panels.Reposition(offset)
+
+        return value
+
+
+    def GetPanelsLength(self, collapsed, expanded):
+        """
+        Returns the length of the panels that are expanded and
+        collapsed.
+
+        :param `collapsed`: the current value of the collapsed panels;
+        :param `expanded`: the current value of the expanded panels.
+
+        :note: This is useful to determine quickly what size is used to display,
+         and what is left at the bottom (right) to align the collapsed panels.
+        """
+
+        value = 0
+
+        # assumed here that all the panels that are expanded
+        # are positioned after each other from 0,0 to end.
+
+        for j in range(0, len(self._panels)):
+            offset = self._panels[j].GetPanelLength()
+            value = value + offset
+            if self._panels[j].IsExpanded():
+                expanded = expanded + offset
+            else:
+                collapsed = collapsed + offset
+
+        return collapsed, expanded, value
+
+
+    def Collapse(self, foldpanel):
+        """
+        Collapses the given fold panel reference, and updates the foldpanel bar.
+
+        :param `foldpanel`: an instance of :class:`FoldPanelItem`.
+
+        :note: With the ``FPB_COLLAPSE_TO_BOTTOM`` style set, all collapsed captions
+         are put at the bottom of the control. In the normal mode, they stay where
+         they are.
+        """
+
+        try:
+            item = self._panels.index(foldpanel)
+        except:
+            raise Exception("ERROR: Invalid Panel Passed To Collapse: " + repr(foldpanel))
+
+        foldpanel.Collapse()
+        self.RefreshPanelsFrom(foldpanel)
+
+
+    def Expand(self, foldpanel):
+        """
+        Expands the given fold panel reference, and updates the foldpanel bar.
+
+        :param `foldpanel`: an instance of :class:`FoldPanelItem`.
+
+        :note: With the ``FPB_COLLAPSE_TO_BOTTOM`` style set, they will be removed
+         from the bottom and the order where the panel originally was placed is
+         restored.
+        """
+
+        fpbextrastyle = 0
+
+        if self._agwStyle & FPB_SINGLE_FOLD or self._agwStyle & FPB_EXCLUSIVE_FOLD:
+            fpbextrastyle = 1
+            for panel in self._panels:
+                panel.Collapse()
+
+        foldpanel.Expand()
+
+        if fpbextrastyle:
+            if self._agwStyle & FPB_EXCLUSIVE_FOLD:
+                self.RepositionCollapsedToBottom()
+            self.RefreshPanelsFrom(self._panels[0])
+        else:
+            self.RefreshPanelsFrom(foldpanel)
+
+
+    def ApplyCaptionStyle(self, foldpanel, cbstyle):
+        """
+        Sets the style of the caption bar (:class:`CaptionBar`) of the fold panel.
+
+        :param `foldpanel`: an instance of :class:`FoldPanelItem`;
+        :param `cbstyle`: an instance of :class:`CaptionBarStyle`.
+
+        :note:
+
+         The changes are applied immediately. All styles not set in the
+         :class:`CaptionBarStyle` class are not applied. Use the :class:`CaptionBar` reference
+         to indicate what captionbar you want to apply the style to. To apply one
+         style to all :class:`CaptionBar` items, use :meth:`~FoldPanelBar.ApplyCaptionStyleAll`.
+        """
+
+        foldpanel.ApplyCaptionStyle(cbstyle)
+
+
+    def ApplyCaptionStyleAll(self, cbstyle):
+        """
+        Sets the style of all the caption bars of the fold panel.
+        The changes are applied immediately.
+
+        :param `cbstyle`: an instance of :class:`CaptionBarStyle`.
+        """
+
+        for panels in self._panels:
+            self.ApplyCaptionStyle(panels, cbstyle)
+
+
+    def GetCaptionStyle(self, foldpanel):
+        """
+        Returns the currently used caption style for the fold panel.
+
+        It is returned as a :class:`CaptionBarStyle` class. After modifying it, it can
+        be set again.
+
+        :param `foldpanel`: an instance of :class:`FoldPanelItem`.
+        """
+
+        return foldpanel.GetCaptionStyle()
+
+
+    def IsVertical(self):
+        """
+        Returns whether the :class:`CaptionBar` has default orientation or not.
+        Default is vertical.
+        """
+
+        return self._isVertical
+
+
+    def GetFoldPanel(self, item):
+        """
+        Returns the panel associated with the index `item`.
+
+        :param `item`: an integer representing the :class:`FoldPanelItem` in the list of
+         panels in this :class:`FoldPanelBar`.
+        """
+
+        try:
+            ind = self._panels[item]
+            return self._panels[item]
+        except:
+            raise Exception("ERROR: List Index Out Of Range Or Bad Item Passed: " + repr(item) + \
+                            ". Item Should Be An Integer Between " + repr(0) + " And " + \
+                            repr(len(self._panels)))
+
+
+    def GetCount(self):
+        """ Returns the number of panels in the :class:`FoldPanelBar`. """
+
+        try:
+            return len(self._panels)
+        except:
+            raise Exception("ERROR: No Panels Have Been Added To FoldPanelBar")
+
+
+
+# --------------------------------------------------------------------------------- #
+# class FoldPanelItem
+# --------------------------------------------------------------------------------- #
+
+class FoldPanelItem(wx.Panel):
+    """
+    This class is a child sibling of the :class:`FoldPanelBar` class. It will
+    contain a :class:`CaptionBar` class for receiving of events, and a the
+    rest of the area can be populated by a :class:`Panel` derived class.
+    """
+
+    def __init__(self, parent, id=wx.ID_ANY, caption="", foldIcons=None,
+                 collapsed=False, cbstyle=None):
+        """
+        Default class constructor.
+
+        :param `parent`: the :class:`FoldPanelItem` parent window;
+        :param `id`: an identifier for the control: a value of -1 is taken to mean a default;
+        :param `caption`: the string to be displayed in :class:`CaptionBar`;
+        :param `foldIcons`: an instance of :class:`wx.ImageList` containing the icons to display
+         next to the caption text;
+        :param `collapsed`: ``True`` if the :class:`CaptionBar` should start in the collapsed state,
+         ``False`` otherwise;
+        :param `cbstyle`: the :class:`CaptionBar` window style. Must be an instance of
+         :class:`CaptionBarStyle`.
+        """
+
+        wx.Panel.__init__(self, parent, id, wx.Point(0,0), style=wx.CLIP_CHILDREN)
+        self._controlCreated = False
+        self._UserSize = 0
+        self._PanelSize = 0
+        self._LastInsertPos = 0
+        self._itemPos = 0
+        self._userSized = False
+
+        if foldIcons is None:
+            foldIcons = wx.ImageList(16, 16)
+
+            bmp = ExpandedIcon.GetBitmap()
+            foldIcons.Add(bmp)
+            bmp = CollapsedIcon.GetBitmap()
+            foldIcons.Add(bmp)
+
+        self._foldIcons = foldIcons
+        if cbstyle is None:
+            cbstyle = EmptyCaptionBarStyle
+
+        # create the caption bar, in collapsed or expanded state
+
+        self._captionBar = CaptionBar(self, wx.ID_ANY, wx.Point(0,0),
+                                      size=wx.DefaultSize, caption=caption,
+                                      foldIcons=foldIcons, cbstyle=cbstyle)
+
+        if collapsed:
+            self._captionBar.Collapse()
+
+        self._controlCreated = True
+
+        # make initial size for component, if collapsed, the
+        # size is determined on the panel height and won't change
+
+        size = self._captionBar.GetSize() + wx.Size(0, 6)
+
+        self._PanelSize = (self.IsVertical() and [size.GetHeight()] or \
+                           [size.GetWidth()])[0]
+
+        self._LastInsertPos = self._PanelSize
+        self._items = []
+
+        self.Bind(EVT_CAPTIONBAR, self.OnPressCaption)
+        self.Bind(wx.EVT_PAINT, self.OnPaint)
+
+
+    def AddWindow(self, window, flags=FPB_ALIGN_WIDTH, spacing=FPB_DEFAULT_SPACING,
+                  leftSpacing=FPB_DEFAULT_LEFTLINESPACING,
+                  rightSpacing=FPB_DEFAULT_RIGHTLINESPACING):
+        """
+        Adds a window item to the list of items on this panel.
+
+        :param `window`: an instance of :class:`wx.Window`;
+        :param `flags`: can be one of the following bits:
+
+         ====================== ======= ====================================
+         Align Flag              Value  Description
+         ====================== ======= ====================================
+         ``FPB_ALIGN_WIDTH``          1 The :class:`wx.Window` to be added will be aligned to fit the width of the FoldPanel when it is resized. Very handy for sizer items, buttons and text boxes.
+         ``FPB_ALIGN_LEFT``           0 Aligns left instead of fitting the width of the child window to be added. Use either this one or ``FPB_ALIGN_WIDTH``.
+         ====================== ======= ====================================
+
+        :param `spacing`: reserves a number of pixels before the window element;
+        :param `leftSpacing`: an indent, in pixels;
+        :param `rightSpacing`: a right spacing, only relevant when the style
+         ``FPB_ALIGN_WIDTH`` is chosen.
+        """
+
+        wi = FoldWindowItem(self, window, Type="WINDOW", flags=flags, spacing=spacing,
+                            leftSpacing=leftSpacing, rightSpacing=rightSpacing)
+
+        self._items.append(wi)
+
+        vertical = self.IsVertical()
+
+        self._spacing = spacing
+        self._leftSpacing = leftSpacing
+        self._rightSpacing = rightSpacing
+
+        xpos = (vertical and [leftSpacing] or [self._LastInsertPos + spacing])[0]
+        ypos = (vertical and [self._LastInsertPos + spacing] or [leftSpacing])[0]
+
+        window.SetSize(xpos, ypos, -1, -1, wx.SIZE_USE_EXISTING)
+
+        self._LastInsertPos = self._LastInsertPos + wi.GetWindowLength(vertical)
+        self.ResizePanel()
+
+
+    def AddSeparator(self, colour=wx.BLACK, spacing=FPB_DEFAULT_SPACING,
+                     leftSpacing=FPB_DEFAULT_LEFTSPACING,
+                     rightSpacing=FPB_DEFAULT_RIGHTSPACING):
+        """
+        Adds a separator item to the list of items on this panel.
+
+        :param `colour`: the separator colour, an instance of :class:`wx.Colour`;
+        :param `spacing`: the separator to be added can be slightly indented from
+         left and right so it is more visibly placed in the fold panel. Use `spacing` > 0
+         to give the control an y offset from the previous :class:`wx.Window` added;
+        :param `leftSpacing`: give the added separator a slight indent from the left;
+        :param `rightSpacing`: give the added separator a slight indent from the right.
+        """
+
+        wi = FoldWindowItem(self, window=None, Type="SEPARATOR",
+                            flags=FPB_ALIGN_WIDTH, y=self._LastInsertPos,
+                            colour=colour, spacing=spacing, leftSpacing=leftSpacing,
+                            rightSpacing=rightSpacing)
+
+        self._items.append(wi)
+        self._LastInsertPos = self._LastInsertPos + \
+                              wi.GetWindowLength(self.IsVertical())
+
+        self.ResizePanel()
+
+
+    def Reposition(self, pos):
+        """
+        Repositions this :class:`FoldPanelItem` and reports the length occupied
+        for the next :class:`FoldPanelItem` in the list.
+
+        :param `pos`: the new item position.
+        """
+
+        # NOTE: Call Resize before Reposition when an item is added, because the new
+        # size needed will be calculated by Resize. Of course the relative position
+        # of the controls have to be correct in respect to the caption bar
+
+        self.Freeze()
+
+        vertical = self.IsVertical()
+        xpos = (vertical and [-1] or [pos])[0]
+        ypos = (vertical and [pos] or [-1])[0]
+
+        self.SetSize(xpos, ypos, -1, -1, wx.SIZE_USE_EXISTING)
+        self._itemPos = pos + 6  # Add 6px of padding to bottom of each item
+
+        self.Thaw()
+
+        return self.GetPanelLength()
+
+
+    def OnPressCaption(self, event):
+        """
+        Handles the ``wx.EVT_CAPTIONBAR`` event for :class:`FoldPanelItem`.
+
+        :param `event`: a :class:`CaptionBarEvent` event to be processed.
+        """
+
+        # tell the upper container we are responsible
+        # for this event, so it can fold the panel item
+        # and do a refresh
+
+        event.SetTag(self)
+        event.Skip()
+
+
+    def ResizePanel(self):
+        """ Resizes the panel. """
+
+        # prevent unnecessary updates by blocking repaints for a sec
+
+        self.Freeze()
+
+        vertical = self.IsVertical()
+        # force this panel to take the width of the parent panel and the y of the
+        # user or calculated width (which will be recalculated by the contents here)
+
+
+        if self._captionBar.IsCollapsed():
+            size = self._captionBar.GetSize()
+            self._PanelSize = (vertical and [size.GetHeight()] or [size.GetWidth()])[0]
+        else:
+            size = self.GetBestSize()
+            self._PanelSize = (vertical and [size.GetHeight()] or [size.GetWidth()])[0]
+
+            if self._UserSize:
+                if vertical:
+                    size.SetHeight(self._UserSize)
+                else:
+                    size.SetWidth(self._UserSize)
+
+        pnlsize = self.GetParent().GetSize()
+
+        if vertical:
+            size.SetWidth(pnlsize.GetWidth())
+        else:
+            size.SetHeight(pnlsize.GetHeight())
+
+        # resize caption bar
+        xsize = (vertical and [size.GetWidth()] or [-1])[0]
+        ysize = (vertical and [-1] or [size.GetHeight()])[0]
+
+        self._captionBar.SetSize((xsize, ysize))
+
+        # resize the panel
+        self.SetSize(size)
+
+        # go by all the controls and call Layout
+
+        for items in self._items:
+            items.ResizeItem((vertical and [size.GetWidth()] or \
+                              [size.GetHeight()])[0], vertical)
+
+        self.Thaw()
+
+
+    def OnPaint(self, event):
+        """
+        Handles the ``wx.EVT_PAINT`` event for :class:`FoldPanelItem`.
+
+        :param `event`: a :class:`PaintEvent` event to be processed.
+        """
+
+        # draw all the items that are lines
+
+        dc = wx.PaintDC(self)
+        vertical = self.IsVertical()
+
+        for item in self._items:
+
+            if item.GetType() == "SEPARATOR":
+                pen = wx.Pen(item.GetLineColour(), 1, wx.PENSTYLE_SOLID)
+                dc.SetPen(pen)
+                a = item.GetLeftSpacing()
+                b = item.GetLineY() + item.GetSpacing()
+                c = item.GetLineLength()
+                d = a + c
+
+                if vertical:
+                    dc.DrawLine(a, b, d, b)
+                else:
+                    dc.DrawLine(b, a, b, d)
+
+        event.Skip()
+
+
+    def IsVertical(self):
+        """
+        Returns whether the :class:`CaptionBar` has default orientation or not.
+        Default is vertical.
+        """
+
+        # grandparent of FoldPanelItem is FoldPanelBar
+        # default is vertical
+
+        if isinstance(self.GetGrandParent(), FoldPanelBar):
+            return self.GetGrandParent().IsVertical()
+        else:
+            raise Exception("ERROR: Wrong Parent " + repr(self.GetGrandParent()))
+
+
+    def IsExpanded(self):
+        """
+        Returns expanded or collapsed status.  If the panel is
+        expanded, ``True`` is returned.
+        """
+
+        return not self._captionBar.IsCollapsed()
+
+
+    def GetItemPos(self):
+        """ Returns item's position. """
+
+        return self._itemPos
+
+
+    def Collapse(self):
+        """
+        Internal method.
+
+        This should not be called by the user, because it doesn't trigger the
+        parent  to tell it that we are collapsed or expanded, it only changes
+        visual state.
+        """
+
+        self._captionBar.Collapse()
+        self.ResizePanel()
+
+
+    def Expand(self):
+        """
+        Internal method.
+
+        This should not be called by the user, because it doesn't trigger the
+        parent to tell it that we are collapsed or expanded, it only changes
+        visual state.
+        """
+
+        self._captionBar.Expand()
+        self.ResizePanel()
+
+
+    def GetPanelLength(self):
+        """ Returns size of panel. """
+
+        if self._captionBar.IsCollapsed():
+            return self.GetCaptionLength()
+        elif self._userSized:
+            return self._UserSize
+
+        return self._PanelSize
+
+
+    def GetCaptionLength(self):
+        """ Returns height of caption only. This is for folding calculation purposes. """
+
+        size = self._captionBar.GetSize()
+        return (self.IsVertical() and [size.GetHeight()] or [size.GetWidth()])[0]
+
+
+    def ApplyCaptionStyle(self, cbstyle):
+        """ Applies the style defined in `cbstyle` to the :class:`CaptionBar`."""
+
+        self._captionBar.SetCaptionStyle(cbstyle)
+
+
+    def GetCaptionStyle(self):
+        """
+        Returns the current style of the captionbar in a :class:`CaptionBarStyle` class.
+
+        This can be used to change and set back the changes.
+        """
+
+        return self._captionBar.GetCaptionStyle()
+
+
+# ----------------------------------------------------------------------------------- #
+# class FoldWindowItem
+# ----------------------------------------------------------------------------------- #
+
+class FoldWindowItem(object):
+    """
+    This class is a child sibling of the :class:`FoldPanelItem` class. It
+    will contain :class:`wx.Window` that can be either a separator (a coloured
+    line simulated by a :class:`wx.Window`) or a wxPython controls (such as a
+    :class:`Button`, a :class:`ListCtrl` etc...).
+    """
+
+    def __init__(self, parent, window=None, **kw):
+        """
+        Default class constructor
+
+        :param `parent`: the :class:`FoldWindowItem` parent;
+        :param `window`: the window contained in this item.
+
+        :keyword `Type`: can be "WINDOW" or "SEPARATOR";
+        :keyword `lineColour`: the separator colour (meaningful for separators only);
+        :keyword `y`: the separator y position (meaningful for separators only);
+        :keyword `flags`: the alignment flags;
+        :keyword `spacing`: reserves a number of pixels before the window/separator element;
+        :keyword `leftSpacing`: an indent, in pixels;
+        :keyword `rightSpacing`: a right spacing, only relevant when the style
+         ``FPB_ALIGN_WIDTH`` is chosen.
+
+        :see: :meth:`FoldPanelBar.AddFoldPanelWindow() <FoldPanelBar.AddFoldPanelWindow>` for a list of valid alignment flags.
+        """
+
+        if "Type" not in kw:
+            raise Exception('ERROR: Missing Window Type Information. This Should Be "WINDOW" Or "SEPARATOR"')
+
+        if kw.get("Type") == "WINDOW":
+            # Window constructor. This initialises the class as a wx.Window Type
+
+            if "flags" in kw:
+                self._flags = kw.get("flags")
+            else:
+                self._flags = FPB_ALIGN_WIDTH
+            if "spacing" in kw:
+                self._spacing = kw.get("spacing")
+            else:
+                self._spacing = FPB_DEFAULT_SPACING
+            if "leftSpacing" in kw:
+                self._leftSpacing = kw.get("leftSpacing")
+            else:
+                self._leftSpacing = FPB_DEFAULT_LEFTSPACING
+            if "rightSpacing" in kw:
+                self._rightSpacing = kw.get("rightSpacing")
+            else:
+                self._rightSpacing = FPB_DEFAULT_RIGHTSPACING
+
+            self._lineY = 0
+            self._sepLineColour = None
+            self._wnd = window
+
+
+        elif kw.get("Type") == "SEPARATOR":
+            # separator constructor. This initialises the class as a separator type
+
+            if "y" in kw:
+                self._lineY = kw.get("y")
+            else:
+                raise Exception("ERROR: Undefined Y Position For The Separator")
+            if "lineColour" in kw:
+                self._sepLineColour = kw.get("lineColour")
+            else:
+                self._sepLineColour = wx.BLACK
+            if "flags" in kw:
+                self._flags = kw.get("flags")
+            else:
+                self._flags = FPB_ALIGN_WIDTH
+            if "spacing" in kw:
+                self._spacing = kw.get("spacing")
+            else:
+                self._spacing = FPB_DEFAULT_SPACING
+            if "leftSpacing" in kw:
+                self._leftSpacing = kw.get("leftSpacing")
+            else:
+                self._leftSpacing = FPB_DEFAULT_LEFTSPACING
+            if "rightSpacing" in kw:
+                self._rightSpacing = kw.get("rightSpacing")
+            else:
+                self._rightSpacing = FPB_DEFAULT_RIGHTSPACING
+
+            self._wnd = window
+
+        else:
+            raise Exception("ERROR: Undefined Window Type Selected: " + repr(kw.get("Type")))
+
+        self._type = kw.get("Type")
+        self._lineLength = 0
+
+
+    def GetType(self):
+        """ Returns the :class:`FoldWindowItem` type. """
+
+        return self._type
+
+
+    def GetLineY(self):
+        """ Returns the y position of the separator. """
+
+        return self._lineY
+
+
+    def GetLineLength(self):
+        """ Returns the separator line length. """
+
+        return self._lineLength
+
+
+    def GetLineColour(self):
+        """ Returns the separator line colour. """
+
+        return self._sepLineColour
+
+
+    def GetLeftSpacing(self):
+        """ Returns the left indent of :class:`FoldWindowItem`. """
+
+        return self._leftSpacing
+
+
+    def GetRightSpacing(self):
+        """ Returns the right indent of :class:`FoldWindowItem`. """
+
+        return self._rightSpacing
+
+
+    def GetSpacing(self):
+        """ Returns the spacing of :class:`FoldWindowItem`. """
+
+        return self._spacing
+
+
+    def GetWindowLength(self, vertical=True):
+        """
+        Returns space needed by the window if type is :class:`FoldWindowItem`
+        "WINDOW" and returns the total size plus the extra spacing.
+
+        :param `vertical`: ``True`` if the parent :class:`FoldPanelBar` is in vertical
+         mode.
+        """
+
+        value = 0
+        if self._type == "WINDOW":
+            size = self._wnd.GetSize()
+            value = (vertical and [size.GetHeight()] or [size.GetWidth()])[0] + \
+                    self._spacing
+
+        elif self._type == "SEPARATOR":
+            value = 1 + self._spacing
+
+        return value
+
+
+    def ResizeItem(self, size, vertical=True):
+        """
+        Resizes the element, whatever it is.
+
+        A separator or line will be always aligned by width or height
+        depending on orientation of the whole panel.
+
+        :param `size`: the maximum size available for the :class:`FoldWindowItem`;
+        :param `vertical`: ``True`` if the parent :class:`FoldPanelBar` is in vertical
+         mode.
+        """
+
+        if self._flags & FPB_ALIGN_WIDTH:
+            # align by taking full width
+            mySize = size - self._leftSpacing - self._rightSpacing
+
+            if mySize < 0:
+                mySize = 10  # can't have negative width
+
+            if self._type == "SEPARATOR":
+                self._lineLength = mySize
+            else:
+                xsize = (vertical and [mySize] or [-1])[0]
+                ysize = (vertical and [-1] or [mySize])[0]
+
+                self._wnd.SetSize((xsize, ysize))
+
+
+if __name__ == '__main__':
+
+    import wx
+
+    class MyFrame(wx.Frame):
+
+        def __init__(self, parent):
+
+            wx.Frame.__init__(self, parent, -1, "FoldPanelBar Demo")
+
+            text_ctrl = wx.TextCtrl(self, -1, size=(400, 100), style=wx.TE_MULTILINE)
+
+            panel_bar = FoldPanelBar(self, -1, agwStyle=FPB_VERTICAL)
+
+            fold_panel = panel_bar.AddFoldPanel("Thing")
+            thing = wx.TextCtrl(fold_panel, -1, size=(400, -1), style=wx.TE_MULTILINE)
+
+            panel_bar.AddFoldPanelWindow(fold_panel, thing)
+
+            main_sizer = wx.BoxSizer(wx.VERTICAL)
+            main_sizer.Add(text_ctrl, 1, wx.EXPAND)
+            main_sizer.Add(panel_bar, 1, wx.EXPAND)
+            self.SetSizer(main_sizer)
+
+
+    # our normal wxApp-derived class, as usual
+
+    app = wx.App(0)
+
+    frame = MyFrame(None)
+    app.SetTopWindow(frame)
+    frame.Show()
+
+    app.MainLoop()
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/icons/icons.py` & `gswidgetkit-0.3.3/gswidgetkit/icons/icons.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-from wx.lib.embeddedimage import PyEmbeddedImage
-#--------------------
-ICON_BRUSH_CHECKERBOARD = PyEmbeddedImage(
-    b'iVBORw0KGgoAAAANSUhEUgAAAGQAAABkAQMAAABKLAcXAAAABlBMVEVfYWQnLjUoH6AuAAAA'
-    b'KElEQVQ4y2NgsP/A/B9GDDDv/wH+PzCCYWB5o+EyGi6j4TIaLrTiAQDYaoSnfkBkDwAAAABJ'
-    b'RU5ErkJggg==')
-
-#----------------------------------------------------------------------
-ICON_CHECKBOX_CHECKED = PyEmbeddedImage(
-    b'iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABHNCSVQICAgIfAhkiAAAAVJJ'
-    b'REFUOI2d0M8rg3EcwPH38x3b2hDRgyKmZn49y8pBmZLkJiQrSubiIJGd2fMc3Z3HUVHyD4jk'
-    b'DzA5uNly3IgpPGabw9Z4ahvb5/rp9f7+kOa1S78EKtBJeRMBtoQArQJM1mRUkYGOCnBupEFR'
-    b'CXM0vFNrTgFQdmDc08LuxiSBBU/5Aa8iszrlJPais3dyZwzYrVUl8ahbZn3WRTyho+6HeXr9'
-    b'/AksTjhQ/W5slsKR4b4m1qa7iSd0gqFrHhN6ficAkl9pOprt7CwrWM0mAx5yNbI518Pj6yfB'
-    b'0HX+ZEPg+CLK6dUDXa01bC8pWKpFHgd8vUUxgKl/bEUDuL1/RggJryLjbKvjQ09lcUJHO7gp'
-    b'iAEMjz46j2ISEjPedgYc9cRejB/2ZwDg8CwCwIgiF73275F82mWm0CKdfENU20piACFBtODi'
-    b'HxgIizRoxSKlJme0b6+FcOtiAVh9AAAAAElFTkSuQmCC')
-
-#----------------------------------------------------------------------
-ICON_CHECKBOX_FOCUSED = PyEmbeddedImage(
-    b'iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAADC3pUWHRSYXcgcHJvZmlsZSB0'
-    b'eXBlIGV4aWYAAHja7ZZbkuQoDEX/WUUvAUkIieXwMBGzg1l+X/yqyqyq7o6p/ppIEwZSxheh'
-    b'I3CG7d9/ZviBi4qlkNQ8l5wjrlRS4YqOx+Oqe00x7fX5I16dB3u4HzBMglaOn57P8Zed4oMS'
-    b'VfT0nZD380F7fFDSqe9PQnw0sjxa/XEKlVNI+HhAp0A9lhVzcXu/hLYd7bhW4scdVpX80e0P'
-    b'vw3RG4p5hHkTkoiahQ8HZN0UpOIBoY7ia6DI3j/qa6kIyGdxiu+8Cs9U7h59YX+CIvmwBxge'
-    b'g5nv9lM76ZP9FAx7iN/NLP2e+cFu6Z7iIcjrnnN4mHM7VldTRkjzuahrKXsPAxtCLvtrGcVw'
-    b'K/q2l4LiAdnbgXzEHhtKp0IMLJMSDao0advbTh0uJt7Y0DJ3gFo2F+PCXWIAsbQKTTYpMsRB'
-    b'rgOvwMq3L7TPW/bpOjkmHoSRTBCjlQphVX+jfCk050p5ouh3rOAXrySEG4vcqjEKQGheeaR7'
-    b'gK/yfC2uAoK6h9mxwBrbIdGUztxaeSQ7aMFARXvsNbJxCiBEmFvhDHZAophJlDJFYzYixNHB'
-    b'p0LIWRI3ICBVHvCSk0gGHOwYzI13jPaxrHyYcWYBhEoWA5oiFazWwYb8seTIoaqiSVWzmroW'
-    b'rVlyyppztrwOv2piydSymbkVqy6eXD27uQcvXgsXweGoJRcrXkqpFZNWKFe8XTGg1sZNWmra'
-    b'crPmrbTakT49de25W/fQS6+DhwycEyMPGz7KqBttSKUtbbrlzTbfylYnUm3KTFNnnjZ9lllv'
-    b'ahQOrB/Kn1OjixrvpNZAu6nhVbNLgtZxoosZiHEiELdFAAnNi1l0SonDQreYxbLONGV4qQvO'
-    b'oEUMBNNGrJNudm/kHriFlL7FjS9yYaH7G+TCQvcFuY/cPqE21temRwk7obUNV1CjYPt1+OJ1'
-    b'fc9aUkr4ACBgqxejft2G3w34ZVveZgrpW0pv7UvoJfQSegm9hF5C/x+htn9p16fy2y6F//Yi'
-    b'/qnPUcJPiaVBoB5++ksAAAGGaUNDUElDQyBwcm9maWxlAAB4nH2RO0jDUBSG/6YWXxUHO4g4'
-    b'ZKjiYEFUxFGqWAQLpa3QqoPJTV/QpCFJcXEUXAsOPharDi7Oujq4CoLgA8TNzUnRRUo8Nym0'
-    b'iPHA5X789/w/954LCPUyU82OCUDVLCMZi4qZ7KrY+YpedCMAH8YkZurx1GIanvV1T31UdxGe'
-    b'5d33Z/UpOZMBPpF4jumGRbxBPLNp6Zz3iUOsKCnE58TjBl2Q+JHrsstvnAsOCzwzZKST88Qh'
-    b'YrHQxnIbs6KhEk8ThxVVo3wh47LCeYuzWq6y5j35C4M5bSXFdVrDiGEJcSQgQkYVJZRhIUK7'
-    b'RoqJJJ1HPfxDjj9BLplcJTByLKACFZLjB/+D37M181OTblIwCgRebPtjBOjcBRo12/4+tu3G'
-    b'CeB/Bq60lr9SB2Y/Sa+1tPAR0L8NXFy3NHkPuNwBBp90yZAcyU9LyOeB9zP6piwwcAv0rLlz'
-    b'a57j9AFI06yWb4CDQ2C0QNnrHu/uap/bvz3N+f0AMZVyjczf1CsAAA+caVRYdFhNTDpjb20u'
-    b'YWRvYmUueG1wAAAAAAA8P3hwYWNrZXQgYmVnaW49Iu+7vyIgaWQ9Ilc1TTBNcENlaGlIenJl'
-    b'U3pOVGN6a2M5ZCI/Pgo8eDp4bXBtZXRhIHhtbG5zOng9ImFkb2JlOm5zOm1ldGEvIiB4Onht'
-    b'cHRrPSJYTVAgQ29yZSA0LjQuMC1FeGl2MiI+CiA8cmRmOlJERiB4bWxuczpyZGY9Imh0dHA6'
-    b'Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiPgogIDxyZGY6RGVzY3Jp'
-    b'cHRpb24gcmRmOmFib3V0PSIiCiAgICB4bWxuczppcHRjRXh0PSJodHRwOi8vaXB0Yy5vcmcv'
-    b'c3RkL0lwdGM0eG1wRXh0LzIwMDgtMDItMjkvIgogICAgeG1sbnM6eG1wTU09Imh0dHA6Ly9u'
-    b'cy5hZG9iZS5jb20veGFwLzEuMC9tbS8iCiAgICB4bWxuczpzdEV2dD0iaHR0cDovL25zLmFk'
-    b'b2JlLmNvbS94YXAvMS4wL3NUeXBlL1Jlc291cmNlRXZlbnQjIgogICAgeG1sbnM6cGx1cz0i'
-    b'aHR0cDovL25zLnVzZXBsdXMub3JnL2xkZi94bXAvMS4wLyIKICAgIHhtbG5zOkdJTVA9Imh0'
-    b'dHA6Ly93d3cuZ2ltcC5vcmcveG1wLyIKICAgIHhtbG5zOmRjPSJodHRwOi8vcHVybC5vcmcv'
-    b'ZGMvZWxlbWVudHMvMS4xLyIKICAgIHhtbG5zOnRpZmY9Imh0dHA6Ly9ucy5hZG9iZS5jb20v'
-    b'dGlmZi8xLjAvIgogICAgeG1sbnM6eG1wPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAv'
-    b'IgogICB4bXBNTTpEb2N1bWVudElEPSJnaW1wOmRvY2lkOmdpbXA6ZTg4MzMxNTYtMzZiYy00'
-    b'ZTczLWFiMGYtODJiM2E1MzI1NmFlIgogICB4bXBNTTpJbnN0YW5jZUlEPSJ4bXAuaWlkOmU5'
-    b'MmZmYWQ4LThhMzctNGQ0MC1hZTYyLWJjNjYwZTM1YWM2YSIKICAgeG1wTU06T3JpZ2luYWxE'
-    b'b2N1bWVudElEPSJ4bXAuZGlkOjYyYzNjYTYyLTE1YTYtNDhiYy1hNGY0LTY2OGRhMDczNzdm'
-    b'ZCIKICAgR0lNUDpBUEk9IjIuMCIKICAgR0lNUDpQbGF0Zm9ybT0iV2luZG93cyIKICAgR0lN'
-    b'UDpUaW1lU3RhbXA9IjE2MzY0MzQxODc5NTk3NzQiCiAgIEdJTVA6VmVyc2lvbj0iMi4xMC4y'
-    b'MiIKICAgZGM6Rm9ybWF0PSJpbWFnZS9wbmciCiAgIHRpZmY6T3JpZW50YXRpb249IjEiCiAg'
-    b'IHhtcDpDcmVhdG9yVG9vbD0iR0lNUCAyLjEwIj4KICAgPGlwdGNFeHQ6TG9jYXRpb25DcmVh'
-    b'dGVkPgogICAgPHJkZjpCYWcvPgogICA8L2lwdGNFeHQ6TG9jYXRpb25DcmVhdGVkPgogICA8'
-    b'aXB0Y0V4dDpMb2NhdGlvblNob3duPgogICAgPHJkZjpCYWcvPgogICA8L2lwdGNFeHQ6TG9j'
-    b'YXRpb25TaG93bj4KICAgPGlwdGNFeHQ6QXJ0d29ya09yT2JqZWN0PgogICAgPHJkZjpCYWcv'
-    b'PgogICA8L2lwdGNFeHQ6QXJ0d29ya09yT2JqZWN0PgogICA8aXB0Y0V4dDpSZWdpc3RyeUlk'
-    b'PgogICAgPHJkZjpCYWcvPgogICA8L2lwdGNFeHQ6UmVnaXN0cnlJZD4KICAgPHhtcE1NOkhp'
-    b'c3Rvcnk+CiAgICA8cmRmOlNlcT4KICAgICA8cmRmOmxpCiAgICAgIHN0RXZ0OmFjdGlvbj0i'
-    b'c2F2ZWQiCiAgICAgIHN0RXZ0OmNoYW5nZWQ9Ii8iCiAgICAgIHN0RXZ0Omluc3RhbmNlSUQ9'
-    b'InhtcC5paWQ6MDAyOWEyODItNTllYy00NWMzLThiNjMtMTE2MmUwOWVhMjA0IgogICAgICBz'
-    b'dEV2dDpzb2Z0d2FyZUFnZW50PSJHaW1wIDIuMTAgKFdpbmRvd3MpIgogICAgICBzdEV2dDp3'
-    b'aGVuPSIyMDIxLTExLTA4VDIzOjAzOjA3Ii8+CiAgICA8L3JkZjpTZXE+CiAgIDwveG1wTU06'
-    b'SGlzdG9yeT4KICAgPHBsdXM6SW1hZ2VTdXBwbGllcj4KICAgIDxyZGY6U2VxLz4KICAgPC9w'
-    b'bHVzOkltYWdlU3VwcGxpZXI+CiAgIDxwbHVzOkltYWdlQ3JlYXRvcj4KICAgIDxyZGY6U2Vx'
-    b'Lz4KICAgPC9wbHVzOkltYWdlQ3JlYXRvcj4KICAgPHBsdXM6Q29weXJpZ2h0T3duZXI+CiAg'
-    b'ICA8cmRmOlNlcS8+CiAgIDwvcGx1czpDb3B5cmlnaHRPd25lcj4KICAgPHBsdXM6TGljZW5z'
-    b'b3I+CiAgICA8cmRmOlNlcS8+CiAgIDwvcGx1czpMaWNlbnNvcj4KICA8L3JkZjpEZXNjcmlw'
-    b'dGlvbj4KIDwvcmRmOlJERj4KPC94OnhtcG1ldGE+CiAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAKICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgIAogICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgCiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAKICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIAogICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgCiAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAKICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgIAogICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgCiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAKICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgIAogICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'CiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAKICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIAogICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgCiAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAKICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgIAogICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgCiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAKICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIAog'
-    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAKPD94cGFja2V0IGVuZD0idyI/PsmlmdUAAAAG'
-    b'YktHRAD/AP8A/6C9p5MAAAAJcEhZcwAACxMAAAsTAQCanBgAAAAHdElNRQflCwkFAwczB1qB'
-    b'AAAAU0lEQVQ4y+3NsRWAIBAE0R2efWgJlkROZAVci3YgjdyZGJgiiQE/31lKKdndK7CpQ0Rc'
-    b'wLFEhAGrOj2HNUnqHr/sSYNmYAb+E2gD+zMB9jHSJNkNEGQSt/B1TqkAAAAASUVORK5CYII=')
-
-#----------------------------------------------------------------------
-ICON_CHECKBOX_UNCHECKED = PyEmbeddedImage(
-    b'iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABHNCSVQICAgIfAhkiAAAAFpJ'
-    b'REFUOI3tzDERgDAQBdH9wQAOoKS6wVBmsIACIgkrOCBGcrS0IQ1Ftn+rGONWSjkkzVTk7rek'
-    b'fTCzsxYDSBqBJQBTLX61hgYMQB/0wX8GucFfQVL6OMlAegBdmw/j71Be5wAAAABJRU5ErkJg'
-    b'gg==')
-
-#----------------------------------------------------------------------
-ICON_DROPDOWN_ARROW = PyEmbeddedImage(
-    b'iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAABHNCSVQICAgIfAhkiAAAAHJJ'
-    b'REFUSIntkEENg1AQBYc6+Q7AQaUgBSdIQAJIwMG0DuqgHNqE088C6anZOe5udl4eJEny56iT'
-    b'2gY3vTrU9rfA8QTmmkTtgRF4RGGjhO/vs3D+E4k6qq+oPoDmjIRPHQvQAfdSyno1dFWirkeS'
-    b'J0myswFVsUqvSX87GAAAAABJRU5ErkJggg==')
-
-#----------------------------------------------------------------------
-ICON_TEST = PyEmbeddedImage(
-    b'iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAABHNCSVQICAgIfAhkiAAAAQJJ'
-    b'REFUSIntlNFRw0AMRF+owCVkK4g7wB1gOnAJKYEOYiogHQAdmAriDpYOsDvg4y4zmQGfIPAF'
-    b'eT+euZO1llYyXPjzrKIA2xVwDdT56FnS+CsCtjtgB1TAS35ugAG4lTRFAldB8gfgXtJKUiOp'
-    b'BpQ/7JCr+z62K9tvtreFmNH2Psq1VEELzJL6wrt3wM25AmsgMnIAKtt1KWjRA5KhJY73r+cI'
-    b'jMAmMLEhtbE4SZ8KSHoCZlKfP5CFd0v3oUCmBTrbj6d9tt0CB1KLhkggWrQa6EmbfGTOZxOp'
-    b'gqa02eGvIgutSZM1nSbLy9hHIj/Cdmd7WhrXkgdfQtIe2JIqvPAfeQcbwWKpPHAccgAAAABJ'
-    b'RU5ErkJggg==')
-
+from wx.lib.embeddedimage import PyEmbeddedImage
+#--------------------
+ICON_BRUSH_CHECKERBOARD = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAAGQAAABkAQMAAABKLAcXAAAABlBMVEVfYWQnLjUoH6AuAAAA'
+    b'KElEQVQ4y2NgsP/A/B9GDDDv/wH+PzCCYWB5o+EyGi6j4TIaLrTiAQDYaoSnfkBkDwAAAABJ'
+    b'RU5ErkJggg==')
+
+#----------------------------------------------------------------------
+ICON_CHECKBOX_CHECKED = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABHNCSVQICAgIfAhkiAAAAVJJ'
+    b'REFUOI2d0M8rg3EcwPH38x3b2hDRgyKmZn49y8pBmZLkJiQrSubiIJGd2fMc3Z3HUVHyD4jk'
+    b'DzA5uNly3IgpPGabw9Z4ahvb5/rp9f7+kOa1S78EKtBJeRMBtoQArQJM1mRUkYGOCnBupEFR'
+    b'CXM0vFNrTgFQdmDc08LuxiSBBU/5Aa8iszrlJPais3dyZwzYrVUl8ahbZn3WRTyho+6HeXr9'
+    b'/AksTjhQ/W5slsKR4b4m1qa7iSd0gqFrHhN6ficAkl9pOprt7CwrWM0mAx5yNbI518Pj6yfB'
+    b'0HX+ZEPg+CLK6dUDXa01bC8pWKpFHgd8vUUxgKl/bEUDuL1/RggJryLjbKvjQ09lcUJHO7gp'
+    b'iAEMjz46j2ISEjPedgYc9cRejB/2ZwDg8CwCwIgiF73275F82mWm0CKdfENU20piACFBtODi'
+    b'HxgIizRoxSKlJme0b6+FcOtiAVh9AAAAAElFTkSuQmCC')
+
+#----------------------------------------------------------------------
+ICON_CHECKBOX_FOCUSED = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAADC3pUWHRSYXcgcHJvZmlsZSB0'
+    b'eXBlIGV4aWYAAHja7ZZbkuQoDEX/WUUvAUkIieXwMBGzg1l+X/yqyqyq7o6p/ppIEwZSxheh'
+    b'I3CG7d9/ZviBi4qlkNQ8l5wjrlRS4YqOx+Oqe00x7fX5I16dB3u4HzBMglaOn57P8Zed4oMS'
+    b'VfT0nZD380F7fFDSqe9PQnw0sjxa/XEKlVNI+HhAp0A9lhVzcXu/hLYd7bhW4scdVpX80e0P'
+    b'vw3RG4p5hHkTkoiahQ8HZN0UpOIBoY7ia6DI3j/qa6kIyGdxiu+8Cs9U7h59YX+CIvmwBxge'
+    b'g5nv9lM76ZP9FAx7iN/NLP2e+cFu6Z7iIcjrnnN4mHM7VldTRkjzuahrKXsPAxtCLvtrGcVw'
+    b'K/q2l4LiAdnbgXzEHhtKp0IMLJMSDao0advbTh0uJt7Y0DJ3gFo2F+PCXWIAsbQKTTYpMsRB'
+    b'rgOvwMq3L7TPW/bpOjkmHoSRTBCjlQphVX+jfCk050p5ouh3rOAXrySEG4vcqjEKQGheeaR7'
+    b'gK/yfC2uAoK6h9mxwBrbIdGUztxaeSQ7aMFARXvsNbJxCiBEmFvhDHZAophJlDJFYzYixNHB'
+    b'p0LIWRI3ICBVHvCSk0gGHOwYzI13jPaxrHyYcWYBhEoWA5oiFazWwYb8seTIoaqiSVWzmroW'
+    b'rVlyyppztrwOv2piydSymbkVqy6eXD27uQcvXgsXweGoJRcrXkqpFZNWKFe8XTGg1sZNWmra'
+    b'crPmrbTakT49de25W/fQS6+DhwycEyMPGz7KqBttSKUtbbrlzTbfylYnUm3KTFNnnjZ9lllv'
+    b'ahQOrB/Kn1OjixrvpNZAu6nhVbNLgtZxoosZiHEiELdFAAnNi1l0SonDQreYxbLONGV4qQvO'
+    b'oEUMBNNGrJNudm/kHriFlL7FjS9yYaH7G+TCQvcFuY/cPqE21temRwk7obUNV1CjYPt1+OJ1'
+    b'fc9aUkr4ACBgqxejft2G3w34ZVveZgrpW0pv7UvoJfQSegm9hF5C/x+htn9p16fy2y6F//Yi'
+    b'/qnPUcJPiaVBoB5++ksAAAGGaUNDUElDQyBwcm9maWxlAAB4nH2RO0jDUBSG/6YWXxUHO4g4'
+    b'ZKjiYEFUxFGqWAQLpa3QqoPJTV/QpCFJcXEUXAsOPharDi7Oujq4CoLgA8TNzUnRRUo8Nym0'
+    b'iPHA5X789/w/954LCPUyU82OCUDVLCMZi4qZ7KrY+YpedCMAH8YkZurx1GIanvV1T31UdxGe'
+    b'5d33Z/UpOZMBPpF4jumGRbxBPLNp6Zz3iUOsKCnE58TjBl2Q+JHrsstvnAsOCzwzZKST88Qh'
+    b'YrHQxnIbs6KhEk8ThxVVo3wh47LCeYuzWq6y5j35C4M5bSXFdVrDiGEJcSQgQkYVJZRhIUK7'
+    b'RoqJJJ1HPfxDjj9BLplcJTByLKACFZLjB/+D37M181OTblIwCgRebPtjBOjcBRo12/4+tu3G'
+    b'CeB/Bq60lr9SB2Y/Sa+1tPAR0L8NXFy3NHkPuNwBBp90yZAcyU9LyOeB9zP6piwwcAv0rLlz'
+    b'a57j9AFI06yWb4CDQ2C0QNnrHu/uap/bvz3N+f0AMZVyjczf1CsAAA+caVRYdFhNTDpjb20u'
+    b'YWRvYmUueG1wAAAAAAA8P3hwYWNrZXQgYmVnaW49Iu+7vyIgaWQ9Ilc1TTBNcENlaGlIenJl'
+    b'U3pOVGN6a2M5ZCI/Pgo8eDp4bXBtZXRhIHhtbG5zOng9ImFkb2JlOm5zOm1ldGEvIiB4Onht'
+    b'cHRrPSJYTVAgQ29yZSA0LjQuMC1FeGl2MiI+CiA8cmRmOlJERiB4bWxuczpyZGY9Imh0dHA6'
+    b'Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiPgogIDxyZGY6RGVzY3Jp'
+    b'cHRpb24gcmRmOmFib3V0PSIiCiAgICB4bWxuczppcHRjRXh0PSJodHRwOi8vaXB0Yy5vcmcv'
+    b'c3RkL0lwdGM0eG1wRXh0LzIwMDgtMDItMjkvIgogICAgeG1sbnM6eG1wTU09Imh0dHA6Ly9u'
+    b'cy5hZG9iZS5jb20veGFwLzEuMC9tbS8iCiAgICB4bWxuczpzdEV2dD0iaHR0cDovL25zLmFk'
+    b'b2JlLmNvbS94YXAvMS4wL3NUeXBlL1Jlc291cmNlRXZlbnQjIgogICAgeG1sbnM6cGx1cz0i'
+    b'aHR0cDovL25zLnVzZXBsdXMub3JnL2xkZi94bXAvMS4wLyIKICAgIHhtbG5zOkdJTVA9Imh0'
+    b'dHA6Ly93d3cuZ2ltcC5vcmcveG1wLyIKICAgIHhtbG5zOmRjPSJodHRwOi8vcHVybC5vcmcv'
+    b'ZGMvZWxlbWVudHMvMS4xLyIKICAgIHhtbG5zOnRpZmY9Imh0dHA6Ly9ucy5hZG9iZS5jb20v'
+    b'dGlmZi8xLjAvIgogICAgeG1sbnM6eG1wPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAv'
+    b'IgogICB4bXBNTTpEb2N1bWVudElEPSJnaW1wOmRvY2lkOmdpbXA6ZTg4MzMxNTYtMzZiYy00'
+    b'ZTczLWFiMGYtODJiM2E1MzI1NmFlIgogICB4bXBNTTpJbnN0YW5jZUlEPSJ4bXAuaWlkOmU5'
+    b'MmZmYWQ4LThhMzctNGQ0MC1hZTYyLWJjNjYwZTM1YWM2YSIKICAgeG1wTU06T3JpZ2luYWxE'
+    b'b2N1bWVudElEPSJ4bXAuZGlkOjYyYzNjYTYyLTE1YTYtNDhiYy1hNGY0LTY2OGRhMDczNzdm'
+    b'ZCIKICAgR0lNUDpBUEk9IjIuMCIKICAgR0lNUDpQbGF0Zm9ybT0iV2luZG93cyIKICAgR0lN'
+    b'UDpUaW1lU3RhbXA9IjE2MzY0MzQxODc5NTk3NzQiCiAgIEdJTVA6VmVyc2lvbj0iMi4xMC4y'
+    b'MiIKICAgZGM6Rm9ybWF0PSJpbWFnZS9wbmciCiAgIHRpZmY6T3JpZW50YXRpb249IjEiCiAg'
+    b'IHhtcDpDcmVhdG9yVG9vbD0iR0lNUCAyLjEwIj4KICAgPGlwdGNFeHQ6TG9jYXRpb25DcmVh'
+    b'dGVkPgogICAgPHJkZjpCYWcvPgogICA8L2lwdGNFeHQ6TG9jYXRpb25DcmVhdGVkPgogICA8'
+    b'aXB0Y0V4dDpMb2NhdGlvblNob3duPgogICAgPHJkZjpCYWcvPgogICA8L2lwdGNFeHQ6TG9j'
+    b'YXRpb25TaG93bj4KICAgPGlwdGNFeHQ6QXJ0d29ya09yT2JqZWN0PgogICAgPHJkZjpCYWcv'
+    b'PgogICA8L2lwdGNFeHQ6QXJ0d29ya09yT2JqZWN0PgogICA8aXB0Y0V4dDpSZWdpc3RyeUlk'
+    b'PgogICAgPHJkZjpCYWcvPgogICA8L2lwdGNFeHQ6UmVnaXN0cnlJZD4KICAgPHhtcE1NOkhp'
+    b'c3Rvcnk+CiAgICA8cmRmOlNlcT4KICAgICA8cmRmOmxpCiAgICAgIHN0RXZ0OmFjdGlvbj0i'
+    b'c2F2ZWQiCiAgICAgIHN0RXZ0OmNoYW5nZWQ9Ii8iCiAgICAgIHN0RXZ0Omluc3RhbmNlSUQ9'
+    b'InhtcC5paWQ6MDAyOWEyODItNTllYy00NWMzLThiNjMtMTE2MmUwOWVhMjA0IgogICAgICBz'
+    b'dEV2dDpzb2Z0d2FyZUFnZW50PSJHaW1wIDIuMTAgKFdpbmRvd3MpIgogICAgICBzdEV2dDp3'
+    b'aGVuPSIyMDIxLTExLTA4VDIzOjAzOjA3Ii8+CiAgICA8L3JkZjpTZXE+CiAgIDwveG1wTU06'
+    b'SGlzdG9yeT4KICAgPHBsdXM6SW1hZ2VTdXBwbGllcj4KICAgIDxyZGY6U2VxLz4KICAgPC9w'
+    b'bHVzOkltYWdlU3VwcGxpZXI+CiAgIDxwbHVzOkltYWdlQ3JlYXRvcj4KICAgIDxyZGY6U2Vx'
+    b'Lz4KICAgPC9wbHVzOkltYWdlQ3JlYXRvcj4KICAgPHBsdXM6Q29weXJpZ2h0T3duZXI+CiAg'
+    b'ICA8cmRmOlNlcS8+CiAgIDwvcGx1czpDb3B5cmlnaHRPd25lcj4KICAgPHBsdXM6TGljZW5z'
+    b'b3I+CiAgICA8cmRmOlNlcS8+CiAgIDwvcGx1czpMaWNlbnNvcj4KICA8L3JkZjpEZXNjcmlw'
+    b'dGlvbj4KIDwvcmRmOlJERj4KPC94OnhtcG1ldGE+CiAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAKICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgIAogICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgCiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAKICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIAogICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgCiAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAKICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgIAogICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgCiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAKICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgIAogICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'CiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAKICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIAogICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgCiAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAKICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgIAogICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgCiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAKICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIAog'
+    b'ICAgICAgICAgICAgICAgICAgICAgICAgICAKPD94cGFja2V0IGVuZD0idyI/PsmlmdUAAAAG'
+    b'YktHRAD/AP8A/6C9p5MAAAAJcEhZcwAACxMAAAsTAQCanBgAAAAHdElNRQflCwkFAwczB1qB'
+    b'AAAAU0lEQVQ4y+3NsRWAIBAE0R2efWgJlkROZAVci3YgjdyZGJgiiQE/31lKKdndK7CpQ0Rc'
+    b'wLFEhAGrOj2HNUnqHr/sSYNmYAb+E2gD+zMB9jHSJNkNEGQSt/B1TqkAAAAASUVORK5CYII=')
+
+#----------------------------------------------------------------------
+ICON_CHECKBOX_UNCHECKED = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABHNCSVQICAgIfAhkiAAAAFpJ'
+    b'REFUOI3tzDERgDAQBdH9wQAOoKS6wVBmsIACIgkrOCBGcrS0IQ1Ftn+rGONWSjkkzVTk7rek'
+    b'fTCzsxYDSBqBJQBTLX61hgYMQB/0wX8GucFfQVL6OMlAegBdmw/j71Be5wAAAABJRU5ErkJg'
+    b'gg==')
+
+#----------------------------------------------------------------------
+ICON_DROPDOWN_ARROW = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAABHNCSVQICAgIfAhkiAAAAHJJ'
+    b'REFUSIntkEENg1AQBYc6+Q7AQaUgBSdIQAJIwMG0DuqgHNqE088C6anZOe5udl4eJEny56iT'
+    b'2gY3vTrU9rfA8QTmmkTtgRF4RGGjhO/vs3D+E4k6qq+oPoDmjIRPHQvQAfdSyno1dFWirkeS'
+    b'J0myswFVsUqvSX87GAAAAABJRU5ErkJggg==')
+
+#----------------------------------------------------------------------
+ICON_TEST = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAABHNCSVQICAgIfAhkiAAAAQJJ'
+    b'REFUSIntlNFRw0AMRF+owCVkK4g7wB1gOnAJKYEOYiogHQAdmAriDpYOsDvg4y4zmQGfIPAF'
+    b'eT+euZO1llYyXPjzrKIA2xVwDdT56FnS+CsCtjtgB1TAS35ugAG4lTRFAldB8gfgXtJKUiOp'
+    b'BpQ/7JCr+z62K9tvtreFmNH2Psq1VEELzJL6wrt3wM25AmsgMnIAKtt1KWjRA5KhJY73r+cI'
+    b'jMAmMLEhtbE4SZ8KSHoCZlKfP5CFd0v3oUCmBTrbj6d9tt0CB1KLhkggWrQa6EmbfGTOZxOp'
+    b'gqa02eGvIgutSZM1nSbLy9hHIj/Cdmd7WhrXkgdfQtIe2JIqvPAfeQcbwWKpPHAccgAAAABJ'
+    b'RU5ErkJggg==')
+
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/label.py` & `gswidgetkit-0.3.3/gswidgetkit/label.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# ----------------------------------------------------------------------------
-# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
-
-class Label(wx.StaticText):
-    """ 
-    Label widget wrapper created to abstract away needing to have extra code for
-    changing the label's colors and font.
-
-    :param wx.Window `parent`: parent window. Must not be ``None``.
-    :param integer `id`: window identifier. A value of -1 indicates a default value.
-    :param string `label`: the label text.
-    :param `color`: the label text color.
-    :param `bg_color`: the label background color. 
-    :param bool `font_bold`: if true, the label text will be bolded.
-    """
-    def __init__(self, parent, id=wx.ID_ANY, label="", color="#fff",
-                 bg_color=None, font_bold=False, style=0):
-        wx.StaticText.__init__(self, parent, id=id, label=label, style=style)
-
-        if bg_color is None:
-            self.SetBackgroundColour(parent.GetBackgroundColour())
-        else:
-            self.SetBackgroundColour(bg_color)
-        if font_bold is True:
-            self.SetFont(self.GetFont().Bold())
-        self.SetForegroundColour(color)
+# ----------------------------------------------------------------------------
+# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
+
+class Label(wx.StaticText):
+    """ 
+    Label widget wrapper created to abstract away needing to have extra code for
+    changing the label's colors and font.
+
+    :param wx.Window `parent`: parent window. Must not be ``None``.
+    :param integer `id`: window identifier. A value of -1 indicates a default value.
+    :param string `label`: the label text.
+    :param `color`: the label text color.
+    :param `bg_color`: the label background color. 
+    :param bool `font_bold`: if true, the label text will be bolded.
+    """
+    def __init__(self, parent, id=wx.ID_ANY, label="", color="#fff",
+                 bg_color=None, font_bold=False, style=0):
+        wx.StaticText.__init__(self, parent, id=id, label=label, style=style)
+
+        if bg_color is None:
+            self.SetBackgroundColour(parent.GetBackgroundColour())
+        else:
+            self.SetBackgroundColour(bg_color)
+        if font_bold is True:
+            self.SetFont(self.GetFont().Bold())
+        self.SetForegroundColour(color)
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/number_field.py` & `gswidgetkit-0.3.3/gswidgetkit/number_field.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,387 +1,387 @@
-# ----------------------------------------------------------------------------
-# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
-from wx.lib.newevent import NewCommandEvent
-
-from .constants import ACCENT_COLOR, NUMBERFIELD_BG_COLOR, TEXT_COLOR
-from .textctrl import StyledTextCtrl
-from .utils import GetTextExtent
-
-numberfield_cmd_event, EVT_NUMBERFIELD = NewCommandEvent()
-numberfield_change_cmd_event, EVT_NUMBERFIELD_CHANGE = NewCommandEvent()
-
-
-class NumberField(wx.Control):
-    """ 
-    Number field widget to select an integer. Supports both precise and imprecise
-    editing (via dragging the cursor).
-
-    :param wx.Window `parent`: parent window. Must not be ``None``.
-    :param integer `id`: window identifier. A value of -1 indicates a default value.
-    :param string `label`: the displayed text on the Numberfield label.
-    :param string `type_`: the type of number field ("INTEGER" or "FLOAT")
-    :param integer/float `default_value`: the default value.
-    :param integer/float `min_value`: the minimum value the control can be set to.
-    :param integer/float `max_value`: the maximum value the control can be set to.
-    :param integer/float `step_size`: how much the value increments/decrements when mouse drags on this widget
-    :param string `suffix`: the label text shown directly after the value.
-    :param bool `show_p`: if True, show the progress in the background of the control.
-    :param bool `disable_precise`: if True, disable the ability to edit the value via typing in a precise value.
-    :param bool `scroll_horz`: if True, the user can scroll horizontally with the mouse.
-    """
-    def __init__(self, parent, id=wx.ID_ANY, label="", type_="INTEGER", default_value=0, min_value=0,
-                 max_value=100, step_size=1, suffix="px", show_p=True, disable_precise=False,
-                 scroll_horz=True, size=wx.DefaultSize):
-        wx.Control.__init__(self, parent, id, pos=wx.DefaultPosition,
-                            size=size, style=wx.NO_BORDER)
-
-        self.parent = parent
-        self.focused = False
-        self.mouse_in = False
-        self.control_size = wx.DefaultSize
-        self.show_p = show_p
-        self.disable_precise = disable_precise
-        self.buffer = None
-
-        if scroll_horz is True:
-            self.scroll_dir = 0
-        else:
-            self.scroll_dir = 1
-
-        self.type_ = type_
-        self.cur_value = default_value
-        self.min_value = min_value
-        self.max_value = max_value
-        self.change_rate = .5
-        self.change_value = 0
-        self.step_size = step_size
-        self.suffix = suffix
-
-        self.value_range = [min_value, max_value]
-
-        self.label = label
-
-        self.padding_x = 20
-        self.padding_y = 10
-
-        # Flag that is true if a drag is happening after a left click
-        self.changing_value = False
-
-        # Keep track of last sent event
-        self.last_sent_event = None
-
-        # The point in which the cursor gets anchored to during the drag event
-        self.anchor_point = (0, 0)
-
-        # Text ctrl
-        self.textctrl = StyledTextCtrl(self, value=str(self.cur_value),
-                                       bg_color=NUMBERFIELD_BG_COLOR,
-                                       style=wx.BORDER_NONE, pos=(0, 0),
-                                       size=(10, 24))
-        self.textctrl.Hide()
-        self.textctrl.Bind(wx.EVT_KILL_FOCUS, self.OnHideTextCtrl)
-
-        self.Bind(wx.EVT_PAINT, self.OnPaint)
-        self.Bind(wx.EVT_ERASE_BACKGROUND, lambda x: None)
-        self.Bind(wx.EVT_CHAR_HOOK, self.OnKey)
-        self.Bind(wx.EVT_MOTION, self.OnMouseMotion)
-        self.Bind(wx.EVT_LEFT_DOWN, self.OnLeftDown, self)
-        self.Bind(wx.EVT_LEFT_UP, self.OnLeftUp, self)
-        self.Bind(wx.EVT_SET_FOCUS, self.OnSetFocus)
-        self.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
-        self.Bind(wx.EVT_LEAVE_WINDOW, self.OnMouseLeave)
-        self.Bind(wx.EVT_ENTER_WINDOW, self.OnMouseEnter)
-        self.Bind(wx.EVT_LEFT_DCLICK, self.OnShowTextCtrl)
-        self.Bind(wx.EVT_SIZE, self.OnSize)
-
-    def OnPaint(self, event):
-        wx.BufferedPaintDC(self, self.buffer)
-
-    def OnSize(self, event):
-        size = self.GetClientSize()
-
-        # Make sure size is at least 1px to avoid
-        # strange "invalid bitmap size" errors.
-        if size[0] < 1:
-            size = (1, 1)
-        self.buffer = wx.Bitmap(*size)
-        self.UpdateDrawing()
-
-    def UpdateDrawing(self):
-        dc = wx.MemoryDC()
-        dc.SelectObject(self.buffer)
-        dc = wx.GCDC(dc)
-        self.OnDrawBackground(dc)
-        self.OnDrawWidget(dc)
-        del dc  # need to get rid of the MemoryDC before Update() is called.
-        self.Refresh()
-        self.Update()
-
-    def OnDrawBackground(self, dc):
-        dc.SetBackground(wx.Brush(self.parent.GetBackgroundColour()))
-        dc.Clear()
-
-    def OnDrawWidget(self, dc):
-        fnt = self.parent.GetFont()
-        dc.SetFont(fnt)
-        dc.SetPen(wx.TRANSPARENT_PEN)
-
-        full_val_lbl = str(self.cur_value)+self.suffix
-
-        width = self.Size[0]
-        height = self.Size[1]
-        one_val = (width) / (self.max_value + abs(self.min_value))
-        self.p_val = round(((self.cur_value + abs(self.min_value))*one_val))
-
-        if self.mouse_in:
-            p_color = wx.Colour(ACCENT_COLOR)
-            bg_color = wx.Colour(NUMBERFIELD_BG_COLOR)
-        else:
-            p_color = wx.Colour(ACCENT_COLOR).ChangeLightness(90)
-            bg_color = wx.Colour(NUMBERFIELD_BG_COLOR).ChangeLightness(85)
-        dc.SetTextForeground(wx.Colour(TEXT_COLOR))
-        dc.SetBrush(wx.Brush(bg_color))
-        dc.DrawRoundedRectangle(0, 0, width, height, 4)
-
-        if self.show_p is True:
-            dc.SetBrush(wx.Brush(p_color))
-            dc.DrawRoundedRectangle(0, 0, self.p_val, height, 4)
-
-            if self.p_val < width-4 and self.p_val > (self.min_value+4):
-                dc.DrawRectangle((self.p_val)-4, 0, 4, height)
-
-        lbl_w, lbl_h = GetTextExtent(self.label)
-        val_w, val_h = GetTextExtent(full_val_lbl)
-
-        dc.DrawText(self.label, self.padding_x, int((height/2) - (lbl_h/2)))
-        dc.DrawText(full_val_lbl, (width-self.padding_x) - (val_w), int((height/2) - (val_h/2)))
-
-        # Update position of textctrl
-        self.textctrl.SetPosition((5, (int(self.Size[1]/2) - 10)))
-        self.textctrl.SetSize((int(self.Size[0]-10), 24))
-
-    def OnKey(self, event):
-        key = event.GetKeyCode()
-        if key == wx.WXK_RETURN:
-            self.mouse_in = False
-            self.focused = False
-            self.OnHideTextCtrl(None)
-            self.UpdateDrawing()
-        else:
-            event.Skip()
-
-    def OnMouseMotion(self, event):
-        """
-        When the mouse moves, it check to see if it is a drag, or if left down had happened.
-        If neither of those cases are true then it will cancel the action.
-        If they are true then it calculates the change in position of the mouse, then changes
-        the position of the cursor back to where the left click event happened.
-        """
-        # Changes the cursor
-        if self.changing_value:
-            self.SetCursor(wx.Cursor(wx.CURSOR_BLANK))
-        else:
-            self.SetCursor(wx.Cursor(wx.CURSOR_SIZEWE))
-
-        # Calculate the change in mouse position
-        cur_point = event.GetPosition()
-        self.delta = cur_point[self.scroll_dir] - self.anchor_point[self.scroll_dir]
-
-        # If the cursor is being moved and dragged left or right
-        if self.delta != 0 and event.Dragging() and self.changing_value:
-            self.UpdateWidget()
-            self.UpdateDrawing()
-
-        if event.Dragging() and self.changing_value:
-            self.SetCursor(wx.Cursor(wx.CURSOR_BLANK))
-            # Set the cursor back to the original point so it doesn't run away
-            if "wxMac" not in wx.PlatformInfo:
-                self.WarpPointer(int(self.anchor_point[0]), int(self.anchor_point[1]))
-
-        # Case where the mouse is moving over the control, but has no
-        # intent to actually change the value
-        if self.changing_value and not event.Dragging():
-            self.changing_value = False
-            self.parent.SetDoubleBuffered(False)
-
-        event.Skip()
-
-    def OnHideTextCtrl(self, event):
-        value = self.textctrl.GetValue()
-        if value != " ":
-            if (self.type_ == "INTEGER"):
-                new_value = int(value)
-            elif (self.type_ == "FLOAT"):
-                new_value = float(value)
-            else:
-                new_value = int(value)
-
-            if new_value >= self.min_value and new_value <= self.max_value:
-                self.cur_value = new_value
-
-        self.textctrl.Hide()
-        self.SendChangeEvent()
-        self.SendSliderEvent()
-        self.UpdateDrawing()
-
-    def OnShowTextCtrl(self, event):
-        if self.show_p is False and self.disable_precise is False:
-            self.textctrl.SetValue(str(self.cur_value))
-            self.textctrl.Show()
-            self.textctrl.SetFocus()
-        event.Skip()
-        self.textctrl.SetCurrentPos(len(str(self.cur_value+1)))
-
-    def SendSliderEvent(self):
-        wx.PostEvent(self, numberfield_cmd_event(id=self.GetId(), value=self.cur_value))
-
-    def SendChangeEvent(self):
-        # Implement a debounce system where only one event is
-        # sent only if the value actually changed.
-        if self.cur_value != self.last_sent_event:
-            wx.PostEvent(self, numberfield_change_cmd_event(
-                                    id=self.GetId(), value=self.cur_value))
-            self.last_sent_event = self.cur_value
-
-    def Increasing(self):
-        if self.delta > 0:
-            return True
-        else:
-            return False
-
-    def Decreasing(self):
-        if self.delta < 0:
-            return True
-        else:
-            return False
-
-    def OnLeftUp(self, event):
-        """
-        Cancels the changing event, and turns off the optimization buffering
-        """
-        self.changing_value = False
-        self.parent.SetDoubleBuffered(False)
-        self.SetCursor(wx.Cursor(wx.CURSOR_SIZEWE))
-        self.SendSliderEvent()
-
-    def OnLeftDown(self, event):
-        """
-        Sets the anchor point that the cursor will go back to the original position.
-        Also turns on the doublebuffering which eliminates the flickering when rapidly changing values.
-        """
-        pos = event.GetPosition()
-        self.anchor_point = (pos[0], pos[1])
-        self.changing_value = True
-        self.parent.SetDoubleBuffered(True)
-        self.UpdateDrawing()
-
-    def OnSetFocus(self, event):
-        self.focused = True
-        self.Refresh()
-
-    def OnKillFocus(self, event):
-        self.focused = False
-        self.Refresh()
-
-    def OnMouseEnter(self, event):
-        self.mouse_in = True
-        self.Refresh()
-        self.UpdateDrawing()
-
-    def OnMouseLeave(self, event):
-        """
-        In the event that the mouse is moved fast enough to leave the bounds of the label, this
-        will be triggered, warping the cursor back to where the left click event originally
-        happened
-        """
-        if self.changing_value:
-            self.WarpPointer(self.anchor_point[0], self.anchor_point[1])
-        self.mouse_in = False
-        self.Refresh()
-        self.UpdateDrawing()
-
-    def AcceptsFocusFromKeyboard(self):
-        """Overridden base class virtual."""
-        return True
-
-    def AcceptsFocus(self):
-        """ Overridden base class virtual. """
-        return True
-
-    def HasFocus(self):
-        """ Returns whether or not we have the focus. """
-        return self.focused
-
-    def GetValue(self):
-        return self.cur_value
-
-    def SetValue(self, value):
-        self.cur_value = value
-
-    def SetLabel(self, label):
-        self.label = label
-
-    def UpdateWidget(self):
-        self.change_value += self.change_rate/2.0
-
-        if self.change_value >= 1:
-            if self.Increasing():
-                if self.cur_value < self.max_value:
-                    self.cur_value += self.step_size
-            else:
-                if (self.cur_value - 1) >= self.min_value:
-                    if self.cur_value > self.min_value:
-                        self.cur_value -= self.step_size
-
-            # Reset the change value since the value was just changed.
-            self.change_value = 0
-
-        self.SendChangeEvent()
-
-    def DoGetBestSize(self):
-        """
-        Overridden base class virtual.  Determines the best size of the control
-        based on the label size, the bitmap size and the current font.
-        """
-
-        normal_label = self.label
-        value_label = str(self.cur_value) + self.suffix
-
-        font = wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT)
-
-        dc = wx.ClientDC(self)
-        dc.SetFont(font)
-
-        # Measure our labels
-        lbl_text_w, lbl_text_h = dc.GetTextExtent(normal_label)
-        val_text_w, val_text_h = dc.GetTextExtent(value_label)
-
-        totalwidth = lbl_text_w + val_text_w + self.padding_x + 76
-
-        # To avoid issues with drawing the control properly, we
-        # always make sure the width is an even number.
-        if totalwidth % 2:
-            totalwidth -= 1
-        totalheight = lbl_text_h + self.padding_y
-
-        best = wx.Size(totalwidth, totalheight)
-
-        # Cache the best size so it doesn't need to be calculated again,
-        # at least until some properties of the window change
-        self.CacheBestSize(best)
-
-        return best
+# ----------------------------------------------------------------------------
+# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
+from wx.lib.newevent import NewCommandEvent
+
+from .constants import ACCENT_COLOR, NUMBERFIELD_BG_COLOR, TEXT_COLOR
+from .textctrl import StyledTextCtrl
+from .utils import GetTextExtent
+
+numberfield_cmd_event, EVT_NUMBERFIELD = NewCommandEvent()
+numberfield_change_cmd_event, EVT_NUMBERFIELD_CHANGE = NewCommandEvent()
+
+
+class NumberField(wx.Control):
+    """ 
+    Number field widget to select an integer. Supports both precise and imprecise
+    editing (via dragging the cursor).
+
+    :param wx.Window `parent`: parent window. Must not be ``None``.
+    :param integer `id`: window identifier. A value of -1 indicates a default value.
+    :param string `label`: the displayed text on the Numberfield label.
+    :param string `type_`: the type of number field ("INTEGER" or "FLOAT")
+    :param integer/float `default_value`: the default value.
+    :param integer/float `min_value`: the minimum value the control can be set to.
+    :param integer/float `max_value`: the maximum value the control can be set to.
+    :param integer/float `step_size`: how much the value increments/decrements when mouse drags on this widget
+    :param string `suffix`: the label text shown directly after the value.
+    :param bool `show_p`: if True, show the progress in the background of the control.
+    :param bool `disable_precise`: if True, disable the ability to edit the value via typing in a precise value.
+    :param bool `scroll_horz`: if True, the user can scroll horizontally with the mouse.
+    """
+    def __init__(self, parent, id=wx.ID_ANY, label="", type_="INTEGER", default_value=0, min_value=0,
+                 max_value=100, step_size=1, suffix="px", show_p=True, disable_precise=False,
+                 scroll_horz=True, size=wx.DefaultSize):
+        wx.Control.__init__(self, parent, id, pos=wx.DefaultPosition,
+                            size=size, style=wx.NO_BORDER)
+
+        self.parent = parent
+        self.focused = False
+        self.mouse_in = False
+        self.control_size = wx.DefaultSize
+        self.show_p = show_p
+        self.disable_precise = disable_precise
+        self.buffer = None
+
+        if scroll_horz is True:
+            self.scroll_dir = 0
+        else:
+            self.scroll_dir = 1
+
+        self.type_ = type_
+        self.cur_value = default_value
+        self.min_value = min_value
+        self.max_value = max_value
+        self.change_rate = .5
+        self.change_value = 0
+        self.step_size = step_size
+        self.suffix = suffix
+
+        self.value_range = [min_value, max_value]
+
+        self.label = label
+
+        self.padding_x = 20
+        self.padding_y = 10
+
+        # Flag that is true if a drag is happening after a left click
+        self.changing_value = False
+
+        # Keep track of last sent event
+        self.last_sent_event = None
+
+        # The point in which the cursor gets anchored to during the drag event
+        self.anchor_point = (0, 0)
+
+        # Text ctrl
+        self.textctrl = StyledTextCtrl(self, value=str(self.cur_value),
+                                       bg_color=NUMBERFIELD_BG_COLOR,
+                                       style=wx.BORDER_NONE, pos=(0, 0),
+                                       size=(10, 24))
+        self.textctrl.Hide()
+        self.textctrl.Bind(wx.EVT_KILL_FOCUS, self.OnHideTextCtrl)
+
+        self.Bind(wx.EVT_PAINT, self.OnPaint)
+        self.Bind(wx.EVT_ERASE_BACKGROUND, lambda x: None)
+        self.Bind(wx.EVT_CHAR_HOOK, self.OnKey)
+        self.Bind(wx.EVT_MOTION, self.OnMouseMotion)
+        self.Bind(wx.EVT_LEFT_DOWN, self.OnLeftDown, self)
+        self.Bind(wx.EVT_LEFT_UP, self.OnLeftUp, self)
+        self.Bind(wx.EVT_SET_FOCUS, self.OnSetFocus)
+        self.Bind(wx.EVT_KILL_FOCUS, self.OnKillFocus)
+        self.Bind(wx.EVT_LEAVE_WINDOW, self.OnMouseLeave)
+        self.Bind(wx.EVT_ENTER_WINDOW, self.OnMouseEnter)
+        self.Bind(wx.EVT_LEFT_DCLICK, self.OnShowTextCtrl)
+        self.Bind(wx.EVT_SIZE, self.OnSize)
+
+    def OnPaint(self, event):
+        wx.BufferedPaintDC(self, self.buffer)
+
+    def OnSize(self, event):
+        size = self.GetClientSize()
+
+        # Make sure size is at least 1px to avoid
+        # strange "invalid bitmap size" errors.
+        if size[0] < 1:
+            size = (1, 1)
+        self.buffer = wx.Bitmap(*size)
+        self.UpdateDrawing()
+
+    def UpdateDrawing(self):
+        dc = wx.MemoryDC()
+        dc.SelectObject(self.buffer)
+        dc = wx.GCDC(dc)
+        self.OnDrawBackground(dc)
+        self.OnDrawWidget(dc)
+        del dc  # need to get rid of the MemoryDC before Update() is called.
+        self.Refresh()
+        self.Update()
+
+    def OnDrawBackground(self, dc):
+        dc.SetBackground(wx.Brush(self.parent.GetBackgroundColour()))
+        dc.Clear()
+
+    def OnDrawWidget(self, dc):
+        fnt = self.parent.GetFont()
+        dc.SetFont(fnt)
+        dc.SetPen(wx.TRANSPARENT_PEN)
+
+        full_val_lbl = str(self.cur_value)+self.suffix
+
+        width = self.Size[0]
+        height = self.Size[1]
+        one_val = (width) / (self.max_value + abs(self.min_value))
+        self.p_val = round(((self.cur_value + abs(self.min_value))*one_val))
+
+        if self.mouse_in:
+            p_color = wx.Colour(ACCENT_COLOR)
+            bg_color = wx.Colour(NUMBERFIELD_BG_COLOR)
+        else:
+            p_color = wx.Colour(ACCENT_COLOR).ChangeLightness(90)
+            bg_color = wx.Colour(NUMBERFIELD_BG_COLOR).ChangeLightness(85)
+        dc.SetTextForeground(wx.Colour(TEXT_COLOR))
+        dc.SetBrush(wx.Brush(bg_color))
+        dc.DrawRoundedRectangle(0, 0, width, height, 4)
+
+        if self.show_p is True:
+            dc.SetBrush(wx.Brush(p_color))
+            dc.DrawRoundedRectangle(0, 0, self.p_val, height, 4)
+
+            if self.p_val < width-4 and self.p_val > (self.min_value+4):
+                dc.DrawRectangle((self.p_val)-4, 0, 4, height)
+
+        lbl_w, lbl_h = GetTextExtent(self.label)
+        val_w, val_h = GetTextExtent(full_val_lbl)
+
+        dc.DrawText(self.label, self.padding_x, int((height/2) - (lbl_h/2)))
+        dc.DrawText(full_val_lbl, (width-self.padding_x) - (val_w), int((height/2) - (val_h/2)))
+
+        # Update position of textctrl
+        self.textctrl.SetPosition((5, (int(self.Size[1]/2) - 10)))
+        self.textctrl.SetSize((int(self.Size[0]-10), 24))
+
+    def OnKey(self, event):
+        key = event.GetKeyCode()
+        if key == wx.WXK_RETURN:
+            self.mouse_in = False
+            self.focused = False
+            self.OnHideTextCtrl(None)
+            self.UpdateDrawing()
+        else:
+            event.Skip()
+
+    def OnMouseMotion(self, event):
+        """
+        When the mouse moves, it check to see if it is a drag, or if left down had happened.
+        If neither of those cases are true then it will cancel the action.
+        If they are true then it calculates the change in position of the mouse, then changes
+        the position of the cursor back to where the left click event happened.
+        """
+        # Changes the cursor
+        if self.changing_value:
+            self.SetCursor(wx.Cursor(wx.CURSOR_BLANK))
+        else:
+            self.SetCursor(wx.Cursor(wx.CURSOR_SIZEWE))
+
+        # Calculate the change in mouse position
+        cur_point = event.GetPosition()
+        self.delta = cur_point[self.scroll_dir] - self.anchor_point[self.scroll_dir]
+
+        # If the cursor is being moved and dragged left or right
+        if self.delta != 0 and event.Dragging() and self.changing_value:
+            self.UpdateWidget()
+            self.UpdateDrawing()
+
+        if event.Dragging() and self.changing_value:
+            self.SetCursor(wx.Cursor(wx.CURSOR_BLANK))
+            # Set the cursor back to the original point so it doesn't run away
+            if "wxMac" not in wx.PlatformInfo:
+                self.WarpPointer(int(self.anchor_point[0]), int(self.anchor_point[1]))
+
+        # Case where the mouse is moving over the control, but has no
+        # intent to actually change the value
+        if self.changing_value and not event.Dragging():
+            self.changing_value = False
+            self.parent.SetDoubleBuffered(False)
+
+        event.Skip()
+
+    def OnHideTextCtrl(self, event):
+        value = self.textctrl.GetValue()
+        if value != " ":
+            if (self.type_ == "INTEGER"):
+                new_value = int(value)
+            elif (self.type_ == "FLOAT"):
+                new_value = float(value)
+            else:
+                new_value = int(value)
+
+            if new_value >= self.min_value and new_value <= self.max_value:
+                self.cur_value = new_value
+
+        self.textctrl.Hide()
+        self.SendChangeEvent()
+        self.SendSliderEvent()
+        self.UpdateDrawing()
+
+    def OnShowTextCtrl(self, event):
+        if self.show_p is False and self.disable_precise is False:
+            self.textctrl.SetValue(str(self.cur_value))
+            self.textctrl.Show()
+            self.textctrl.SetFocus()
+        event.Skip()
+        self.textctrl.SetCurrentPos(len(str(self.cur_value+1)))
+
+    def SendSliderEvent(self):
+        wx.PostEvent(self, numberfield_cmd_event(id=self.GetId(), value=self.cur_value))
+
+    def SendChangeEvent(self):
+        # Implement a debounce system where only one event is
+        # sent only if the value actually changed.
+        if self.cur_value != self.last_sent_event:
+            wx.PostEvent(self, numberfield_change_cmd_event(
+                                    id=self.GetId(), value=self.cur_value))
+            self.last_sent_event = self.cur_value
+
+    def Increasing(self):
+        if self.delta > 0:
+            return True
+        else:
+            return False
+
+    def Decreasing(self):
+        if self.delta < 0:
+            return True
+        else:
+            return False
+
+    def OnLeftUp(self, event):
+        """
+        Cancels the changing event, and turns off the optimization buffering
+        """
+        self.changing_value = False
+        self.parent.SetDoubleBuffered(False)
+        self.SetCursor(wx.Cursor(wx.CURSOR_SIZEWE))
+        self.SendSliderEvent()
+
+    def OnLeftDown(self, event):
+        """
+        Sets the anchor point that the cursor will go back to the original position.
+        Also turns on the doublebuffering which eliminates the flickering when rapidly changing values.
+        """
+        pos = event.GetPosition()
+        self.anchor_point = (pos[0], pos[1])
+        self.changing_value = True
+        self.parent.SetDoubleBuffered(True)
+        self.UpdateDrawing()
+
+    def OnSetFocus(self, event):
+        self.focused = True
+        self.Refresh()
+
+    def OnKillFocus(self, event):
+        self.focused = False
+        self.Refresh()
+
+    def OnMouseEnter(self, event):
+        self.mouse_in = True
+        self.Refresh()
+        self.UpdateDrawing()
+
+    def OnMouseLeave(self, event):
+        """
+        In the event that the mouse is moved fast enough to leave the bounds of the label, this
+        will be triggered, warping the cursor back to where the left click event originally
+        happened
+        """
+        if self.changing_value:
+            self.WarpPointer(self.anchor_point[0], self.anchor_point[1])
+        self.mouse_in = False
+        self.Refresh()
+        self.UpdateDrawing()
+
+    def AcceptsFocusFromKeyboard(self):
+        """Overridden base class virtual."""
+        return True
+
+    def AcceptsFocus(self):
+        """ Overridden base class virtual. """
+        return True
+
+    def HasFocus(self):
+        """ Returns whether or not we have the focus. """
+        return self.focused
+
+    def GetValue(self):
+        return self.cur_value
+
+    def SetValue(self, value):
+        self.cur_value = value
+
+    def SetLabel(self, label):
+        self.label = label
+
+    def UpdateWidget(self):
+        self.change_value += self.change_rate/2.0
+
+        if self.change_value >= 1:
+            if self.Increasing():
+                if self.cur_value < self.max_value:
+                    self.cur_value += self.step_size
+            else:
+                if (self.cur_value - 1) >= self.min_value:
+                    if self.cur_value > self.min_value:
+                        self.cur_value -= self.step_size
+
+            # Reset the change value since the value was just changed.
+            self.change_value = 0
+
+        self.SendChangeEvent()
+
+    def DoGetBestSize(self):
+        """
+        Overridden base class virtual.  Determines the best size of the control
+        based on the label size, the bitmap size and the current font.
+        """
+
+        normal_label = self.label
+        value_label = str(self.cur_value) + self.suffix
+
+        font = wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT)
+
+        dc = wx.ClientDC(self)
+        dc.SetFont(font)
+
+        # Measure our labels
+        lbl_text_w, lbl_text_h = dc.GetTextExtent(normal_label)
+        val_text_w, val_text_h = dc.GetTextExtent(value_label)
+
+        totalwidth = lbl_text_w + val_text_w + self.padding_x + 76
+
+        # To avoid issues with drawing the control properly, we
+        # always make sure the width is an even number.
+        if totalwidth % 2:
+            totalwidth -= 1
+        totalheight = lbl_text_h + self.padding_y
+
+        best = wx.Size(totalwidth, totalheight)
+
+        # Cache the best size so it doesn't need to be calculated again,
+        # at least until some properties of the window change
+        self.CacheBestSize(best)
+
+        return best
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/popups.py` & `gswidgetkit-0.3.3/gswidgetkit/popups.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# ----------------------------------------------------------------------------
-# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
-from wx.lib.newevent import NewCommandEvent
-
-
-class Popup(wx.Control):
-    def __init__(self, parent, id=wx.ID_ANY, pos=wx.DefaultPosition, size=wx.DefaultSize, style=wx.NO_BORDER, *args, **kwargs):
-        wx.Control.__init__(self, parent, id, pos, size, style, *args, **kwargs)
-        
-        self.parent = parent
-
+# ----------------------------------------------------------------------------
+# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
+from wx.lib.newevent import NewCommandEvent
+
+
+class Popup(wx.Control):
+    def __init__(self, parent, id=wx.ID_ANY, pos=wx.DefaultPosition, size=wx.DefaultSize, style=wx.NO_BORDER, *args, **kwargs):
+        wx.Control.__init__(self, parent, id, pos, size, style, *args, **kwargs)
+        
+        self.parent = parent
+
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/scrollbar.py` & `gswidgetkit-0.3.3/gswidgetkit/scrollbar.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# ----------------------------------------------------------------------------
-# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
+# ----------------------------------------------------------------------------
+# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/textctrl.py` & `gswidgetkit-0.3.3/gswidgetkit/textctrl.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,232 +1,232 @@
-# ----------------------------------------------------------------------------
-# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
-from wx import stc
-
-from .constants import (ACCENT_COLOR, TEXT_COLOR, TEXTCTRL_BG_COLOR, 
-                        TEXTCTRL_BORDER_COLOR)
-
-
-class StyledTextCtrl(stc.StyledTextCtrl):
-    def __init__(self, parent, value="", placeholder="", scrollbar=False,
-                 style=0, bg_color=TEXTCTRL_BG_COLOR, sel_color=ACCENT_COLOR, 
-                 *args, **kwargs):
-        stc.StyledTextCtrl.__init__(self, parent, style=style | wx.TRANSPARENT_WINDOW, *args, **kwargs)
-
-        if scrollbar is False:
-            self.SetUseVerticalScrollBar(False)
-            self.SetUseHorizontalScrollBar(False)
-        self.SetCaretWidth(2)
-        self.SetCaretForeground(sel_color)
-        self.SetMarginLeft(8)
-        self.SetMarginRight(8)
-        self.SetMarginWidth(1, 0)
-        self.SetEOLMode(stc.STC_EOL_LF)
-        self.SetLexer(stc.STC_LEX_NULL)
-        self.SetIndent(4)
-        self.SetUseTabs(False)
-        self.SetTabWidth(4)
-        self.SetValue(value)
-        self.SetScrollWidth(self.GetSize()[0])
-        self.SetScrollWidthTracking(True)
-        self.SetSelBackground(True, sel_color)
-        self.StyleSetBackground(stc.STC_STYLE_DEFAULT, wx.Colour(bg_color))
-        self.StyleSetForeground(stc.STC_STYLE_DEFAULT, wx.Colour("#ffffff"))
-        self.StyleSetFont(stc.STC_STYLE_DEFAULT,
-                          wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT))
-        self.StyleClearAll()
-        self.SetValue(value)
-
-
-class NativeTextCtrl(wx.TextCtrl):
-    def __init__(self, parent, value="", style=wx.BORDER_SIMPLE, *args, **kwargs):
-        wx.TextCtrl.__init__(self, parent, value=value, style=style, *args, **kwargs)
-        self.SetBackgroundColour(wx.Colour(TEXTCTRL_BG_COLOR))
-        self.SetForegroundColour(wx.Colour("#fff"))
-
-
-class TextCtrl(wx.Control):
-    def __init__(self, parent, default="", icon=None, size=wx.DefaultSize):
-        wx.Control.__init__(self, parent, wx.ID_ANY, pos=wx.DefaultPosition,
-                            size=size, style=wx.NO_BORDER)
-
-        self.parent = parent
-        self.focused = False
-        self.mouse_in = False
-        self.control_size = wx.DefaultSize
-        self.buffer = None
-
-        self.value = default
-        self.icon = icon
-
-        self.padding_x = 20
-        self.padding_y = 30
-
-        # Inner text ctrl
-        self.textctrl = StyledTextCtrl(self, value=str(self.value),
-                                       style=wx.BORDER_NONE, 
-                                       bg_color=TEXTCTRL_BG_COLOR,
-                                       sel_color=ACCENT_COLOR, pos=(0, 0), 
-                                       size=(10, 24))
-
-        self.textctrl.Bind(wx.EVT_KILL_FOCUS, self.OnMouseLeave)
-        self.textctrl.Bind(wx.EVT_SET_FOCUS, self.OnFocused)
-        self.textctrl.Bind(wx.EVT_CHAR_HOOK, self.OnKey)
-
-        self.Bind(wx.EVT_PAINT, self.OnPaint)
-        self.Bind(wx.EVT_ERASE_BACKGROUND, lambda x: None)
-        self.Bind(wx.EVT_SIZE, self.OnSize)
-
-    def OnPaint(self, event):
-        wx.BufferedPaintDC(self, self.buffer)
-
-    def OnSize(self, event):
-        size = self.GetClientSize()
-
-        # Make sure size is at least 1px to avoid
-        # strange "invalid bitmap size" errors.
-        if size[0] < 1:
-            size = (1, 1)
-        self.buffer = wx.Bitmap(*size)
-        self.UpdateDrawing()
-
-    def UpdateDrawing(self):
-        dc = wx.MemoryDC()
-        dc.SelectObject(self.buffer)
-        dc = wx.GCDC(dc)
-        self.OnDrawBackground(dc)
-        self.OnDrawWidget(dc)
-        del dc  # need to get rid of the MemoryDC before Update() is called.
-        self.Refresh()
-        self.Update()
-
-    def OnDrawBackground(self, dc):
-        dc.SetBackground(wx.Brush(self.parent.GetBackgroundColour()))
-        dc.Clear()
-
-    def OnDrawWidget(self, dc):
-        fnt = self.parent.GetFont()
-        dc.SetFont(fnt)
-
-        width = self.Size[0]
-        height = self.Size[1]
-
-        if self.mouse_in:
-            text_color = wx.Colour(TEXT_COLOR)
-            border_color = wx.Colour(ACCENT_COLOR)
-            bg_color = wx.Colour(TEXTCTRL_BG_COLOR)
-        else:
-            text_color = wx.Colour(TEXT_COLOR)
-            border_color = wx.Colour(TEXTCTRL_BORDER_COLOR)
-            bg_color = wx.Colour(TEXTCTRL_BG_COLOR).ChangeLightness(85)
-
-        dc.SetTextForeground(text_color)
-        dc.SetPen(wx.Pen(border_color, 1))
-        dc.SetBrush(wx.Brush(bg_color))
-        dc.DrawRoundedRectangle(1, 1, width-1, height-1, 4)
-
-        self.textctrl.StyleSetBackground(stc.STC_STYLE_DEFAULT, bg_color)
-
-        if self.icon != None:
-            dc.DrawBitmap(self.icon, 8, int(self.Size[1]/2) - (self.icon.Height/2))
-
-        # Update position of textctrl
-        if self.icon == None:
-            self.textctrl.SetPosition((2, (int(self.Size[1]/2) - 10)))
-            self.textctrl.SetSize((int(self.Size[0]-4), 20))
-        else:
-            self.textctrl.SetPosition((self.icon.Width + 4, (int(self.Size[1]/2) - 10)))
-            self.textctrl.SetSize((int(self.Size[0]-(self.icon.Width + 4)-4), 20))
-        self.textctrl.SetCurrentPos(len(str(self.value)))
-        self.textctrl.SelectNone()
-
-    def OnKey(self, event):
-        key = event.GetKeyCode()
-        if key == wx.WXK_RETURN:
-            self.mouse_in = False
-            self.focused = False
-            self.textctrl.SetCurrentPos(len(str(self.value)))
-            self.UpdateDrawing()
-        else:
-            event.Skip()
-
-    def OnFocused(self, event):
-        self.mouse_in = True
-        event.Skip()
-        self.UpdateDrawing()
-
-    def OnSetFocus(self, event):
-        self.focused = True
-        self.textctrl.SetFocus()
-        event.Skip()
-        self.Refresh()
-
-    def OnKillFocus(self, event):
-        self.focused = False
-        event.Skip()
-        self.Refresh()
-
-    def OnMouseLeave(self, event):
-        self.mouse_in = False
-        event.Skip()
-        self.Refresh()
-        self.UpdateDrawing()
-
-    def AcceptsFocusFromKeyboard(self):
-        """Overridden base class virtual."""
-        return True
-
-    def AcceptsFocus(self):
-        """ Overridden base class virtual. """
-        return True
-
-    def HasFocus(self):
-        """ Returns whether or not we have the focus. """
-        return self.focused
-
-    def GetValue(self):
-        return self.value
-
-    def SetValue(self, value):
-        self.value = value
-        self.textctrl.SetValue(value)
-
-    def SetIcon(self, icon):
-        self.icon = icon
-
-    def SetFocus(self):
-        self.textctrl.SetFocus()
-
-    def DoGetBestSize(self):
-        """
-        Overridden base class virtual. Determines the best size of the control.
-        """
-        font = wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT)
-        dc = wx.ClientDC(self)
-        dc.SetFont(font)
-
-        # Calculate sizing
-        totalwidth = self.padding_x + self.textctrl.GetSize()[0] + 130
-        totalheight = self.textctrl.GetSize()[1] + self.padding_y
-
-        best = wx.Size(totalwidth, totalheight)
-
-        # Cache the best size so it doesn't need to be calculated again,
-        # at least until some properties of the window change
-        self.CacheBestSize(best)
-
-        return best
+# ----------------------------------------------------------------------------
+# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
+from wx import stc
+
+from .constants import (ACCENT_COLOR, TEXT_COLOR, TEXTCTRL_BG_COLOR, 
+                        TEXTCTRL_BORDER_COLOR)
+
+
+class StyledTextCtrl(stc.StyledTextCtrl):
+    def __init__(self, parent, value="", placeholder="", scrollbar=False,
+                 style=0, bg_color=TEXTCTRL_BG_COLOR, sel_color=ACCENT_COLOR, 
+                 *args, **kwargs):
+        stc.StyledTextCtrl.__init__(self, parent, style=style | wx.TRANSPARENT_WINDOW, *args, **kwargs)
+
+        if scrollbar is False:
+            self.SetUseVerticalScrollBar(False)
+            self.SetUseHorizontalScrollBar(False)
+        self.SetCaretWidth(2)
+        self.SetCaretForeground(sel_color)
+        self.SetMarginLeft(8)
+        self.SetMarginRight(8)
+        self.SetMarginWidth(1, 0)
+        self.SetEOLMode(stc.STC_EOL_LF)
+        self.SetLexer(stc.STC_LEX_NULL)
+        self.SetIndent(4)
+        self.SetUseTabs(False)
+        self.SetTabWidth(4)
+        self.SetValue(value)
+        self.SetScrollWidth(self.GetSize()[0])
+        self.SetScrollWidthTracking(True)
+        self.SetSelBackground(True, sel_color)
+        self.StyleSetBackground(stc.STC_STYLE_DEFAULT, wx.Colour(bg_color))
+        self.StyleSetForeground(stc.STC_STYLE_DEFAULT, wx.Colour("#ffffff"))
+        self.StyleSetFont(stc.STC_STYLE_DEFAULT,
+                          wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT))
+        self.StyleClearAll()
+        self.SetValue(value)
+
+
+class NativeTextCtrl(wx.TextCtrl):
+    def __init__(self, parent, value="", style=wx.BORDER_SIMPLE, *args, **kwargs):
+        wx.TextCtrl.__init__(self, parent, value=value, style=style, *args, **kwargs)
+        self.SetBackgroundColour(wx.Colour(TEXTCTRL_BG_COLOR))
+        self.SetForegroundColour(wx.Colour("#fff"))
+
+
+class TextCtrl(wx.Control):
+    def __init__(self, parent, default="", icon=None, size=wx.DefaultSize):
+        wx.Control.__init__(self, parent, wx.ID_ANY, pos=wx.DefaultPosition,
+                            size=size, style=wx.NO_BORDER)
+
+        self.parent = parent
+        self.focused = False
+        self.mouse_in = False
+        self.control_size = wx.DefaultSize
+        self.buffer = None
+
+        self.value = default
+        self.icon = icon
+
+        self.padding_x = 20
+        self.padding_y = 30
+
+        # Inner text ctrl
+        self.textctrl = StyledTextCtrl(self, value=str(self.value),
+                                       style=wx.BORDER_NONE, 
+                                       bg_color=TEXTCTRL_BG_COLOR,
+                                       sel_color=ACCENT_COLOR, pos=(0, 0), 
+                                       size=(10, 24))
+
+        self.textctrl.Bind(wx.EVT_KILL_FOCUS, self.OnMouseLeave)
+        self.textctrl.Bind(wx.EVT_SET_FOCUS, self.OnFocused)
+        self.textctrl.Bind(wx.EVT_CHAR_HOOK, self.OnKey)
+
+        self.Bind(wx.EVT_PAINT, self.OnPaint)
+        self.Bind(wx.EVT_ERASE_BACKGROUND, lambda x: None)
+        self.Bind(wx.EVT_SIZE, self.OnSize)
+
+    def OnPaint(self, event):
+        wx.BufferedPaintDC(self, self.buffer)
+
+    def OnSize(self, event):
+        size = self.GetClientSize()
+
+        # Make sure size is at least 1px to avoid
+        # strange "invalid bitmap size" errors.
+        if size[0] < 1:
+            size = (1, 1)
+        self.buffer = wx.Bitmap(*size)
+        self.UpdateDrawing()
+
+    def UpdateDrawing(self):
+        dc = wx.MemoryDC()
+        dc.SelectObject(self.buffer)
+        dc = wx.GCDC(dc)
+        self.OnDrawBackground(dc)
+        self.OnDrawWidget(dc)
+        del dc  # need to get rid of the MemoryDC before Update() is called.
+        self.Refresh()
+        self.Update()
+
+    def OnDrawBackground(self, dc):
+        dc.SetBackground(wx.Brush(self.parent.GetBackgroundColour()))
+        dc.Clear()
+
+    def OnDrawWidget(self, dc):
+        fnt = self.parent.GetFont()
+        dc.SetFont(fnt)
+
+        width = self.Size[0]
+        height = self.Size[1]
+
+        if self.mouse_in:
+            text_color = wx.Colour(TEXT_COLOR)
+            border_color = wx.Colour(ACCENT_COLOR)
+            bg_color = wx.Colour(TEXTCTRL_BG_COLOR)
+        else:
+            text_color = wx.Colour(TEXT_COLOR)
+            border_color = wx.Colour(TEXTCTRL_BORDER_COLOR)
+            bg_color = wx.Colour(TEXTCTRL_BG_COLOR).ChangeLightness(85)
+
+        dc.SetTextForeground(text_color)
+        dc.SetPen(wx.Pen(border_color, 1))
+        dc.SetBrush(wx.Brush(bg_color))
+        dc.DrawRoundedRectangle(1, 1, width-1, height-1, 4)
+
+        self.textctrl.StyleSetBackground(stc.STC_STYLE_DEFAULT, bg_color)
+
+        if self.icon != None:
+            dc.DrawBitmap(self.icon, 8, int(self.Size[1]/2) - (self.icon.Height/2))
+
+        # Update position of textctrl
+        if self.icon == None:
+            self.textctrl.SetPosition((2, (int(self.Size[1]/2) - 10)))
+            self.textctrl.SetSize((int(self.Size[0]-4), 20))
+        else:
+            self.textctrl.SetPosition((self.icon.Width + 4, (int(self.Size[1]/2) - 10)))
+            self.textctrl.SetSize((int(self.Size[0]-(self.icon.Width + 4)-4), 20))
+        self.textctrl.SetCurrentPos(len(str(self.value)))
+        self.textctrl.SelectNone()
+
+    def OnKey(self, event):
+        key = event.GetKeyCode()
+        if key == wx.WXK_RETURN:
+            self.mouse_in = False
+            self.focused = False
+            self.textctrl.SetCurrentPos(len(str(self.value)))
+            self.UpdateDrawing()
+        else:
+            event.Skip()
+
+    def OnFocused(self, event):
+        self.mouse_in = True
+        event.Skip()
+        self.UpdateDrawing()
+
+    def OnSetFocus(self, event):
+        self.focused = True
+        self.textctrl.SetFocus()
+        event.Skip()
+        self.Refresh()
+
+    def OnKillFocus(self, event):
+        self.focused = False
+        event.Skip()
+        self.Refresh()
+
+    def OnMouseLeave(self, event):
+        self.mouse_in = False
+        event.Skip()
+        self.Refresh()
+        self.UpdateDrawing()
+
+    def AcceptsFocusFromKeyboard(self):
+        """Overridden base class virtual."""
+        return True
+
+    def AcceptsFocus(self):
+        """ Overridden base class virtual. """
+        return True
+
+    def HasFocus(self):
+        """ Returns whether or not we have the focus. """
+        return self.focused
+
+    def GetValue(self):
+        return self.value
+
+    def SetValue(self, value):
+        self.value = value
+        self.textctrl.SetValue(value)
+
+    def SetIcon(self, icon):
+        self.icon = icon
+
+    def SetFocus(self):
+        self.textctrl.SetFocus()
+
+    def DoGetBestSize(self):
+        """
+        Overridden base class virtual. Determines the best size of the control.
+        """
+        font = wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT)
+        dc = wx.ClientDC(self)
+        dc.SetFont(font)
+
+        # Calculate sizing
+        totalwidth = self.padding_x + self.textctrl.GetSize()[0] + 130
+        totalheight = self.textctrl.GetSize()[1] + self.padding_y
+
+        best = wx.Size(totalwidth, totalheight)
+
+        # Cache the best size so it doesn't need to be calculated again,
+        # at least until some properties of the window change
+        self.CacheBestSize(best)
+
+        return best
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/tooltip.py` & `gswidgetkit-0.3.3/gswidgetkit/tooltip.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,478 +1,478 @@
-# ----------------------------------------------------------------------------
-# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
-#
-# This file includes modified code from wx.lib.agw.supertooltip
-#
-# ----------------------------------------------------------------------------
-
-import wx
-import wx.lib.agw.supertooltip as STT
-
-
-def MakeBold(font):
-    """
-    Makes a font bold. Utility method.
-
-    :param `font`: the font to be made bold.
-    """
-
-    newFont = wx.Font(font.GetPointSize(), font.GetFamily(), font.GetStyle(),
-                      wx.FONTWEIGHT_BOLD, font.GetUnderlined(), font.GetFaceName())
-
-    return newFont
-
-
-def ExtractLink(line):
-    """
-    Extract the link from an hyperlink line.
-
-    :param `line`: the line of text to be processed.
-    """
-
-    line = line[4:]
-    indxStart = line.find("{")
-    indxEnd = line.find("}")
-    hl = line[indxStart+1:indxEnd].strip()
-    line = line[0:indxStart].strip()
-
-    return line, hl
-
-
-class ToolTipWindowBase(object):
-    """ Base class for the different Windows and Mac implementation. """
-
-    def __init__(self, parent, classParent):
-        """
-        Default class constructor.
-
-        :param `parent`: the :class:`SuperToolTip` parent widget;
-        :param `classParent`: the :class:`SuperToolTip` class object.
-        """
-
-        self._spacing = 18
-        self._wasOnLink = False
-        self._hyperlinkRect, self._hyperlinkWeb = [], []
-
-        self._classParent = classParent
-
-        # Bind the events
-        self.Bind(wx.EVT_PAINT, self.OnPaint)
-        self.Bind(wx.EVT_SIZE, self.OnSize)
-        self.Bind(wx.EVT_ERASE_BACKGROUND, self.OnEraseBackground)
-        self.Bind(wx.EVT_MOTION, self.OnMouseMotion)
-        parent.Bind(wx.EVT_KILL_FOCUS, self.OnDestroy)
-        self.Bind(wx.EVT_LEFT_DOWN, self.OnDestroy)
-        self.Bind(wx.EVT_LEFT_DCLICK, self.OnDestroy)
-
-
-    def OnPaint(self, event):
-        """
-        Handles the ``wx.EVT_PAINT`` event for :class:`SuperToolTip`.
-
-        If the `event` parameter is ``None``, calculates best size and returns it.
-
-        :param `event`: a :class:`PaintEvent` event to be processed or ``None``.
-        """
-
-        maxWidth = 0
-        if event is None:
-            dc = wx.ClientDC(self)
-        else:
-            # Go with double buffering...
-            dc = wx.BufferedPaintDC(self)
-
-        frameRect = self.GetClientRect()
-        x, y, width, _height = frameRect
-        # Store the rects for the hyperlink lines
-        self._hyperlinkRect, self._hyperlinkWeb = [], []
-        classParent = self._classParent
-
-        # Retrieve the colours for the blended triple-gradient background
-        topColour, middleColour, bottomColour = classParent.GetTopGradientColour(), \
-                                                classParent.GetMiddleGradientColour(), \
-                                                classParent.GetBottomGradientColour()
-
-        # Get the user options for header, bitmaps etc...
-        drawHeader, drawFooter = classParent.GetDrawHeaderLine(), classParent.GetDrawFooterLine()
-        topRect = wx.Rect(frameRect.x, frameRect.y, frameRect.width, frameRect.height/2)
-        bottomRect = wx.Rect(frameRect.x, frameRect.y+frameRect.height/2, frameRect.width, frameRect.height/2+1)
-        # Fill the triple-gradient
-        dc.GradientFillLinear(topRect, topColour, middleColour, wx.SOUTH)
-        dc.GradientFillLinear(bottomRect, middleColour, bottomColour, wx.SOUTH)
-
-        header, headerBmp = classParent.GetHeader(), classParent.GetHeaderBitmap()
-        headerFont, messageFont, footerFont, hyperlinkFont = classParent.GetHeaderFont(), classParent.GetMessageFont(), \
-                                                             classParent.GetFooterFont(), classParent.GetHyperlinkFont()
-
-        yPos = 0
-        bmpXPos = 0
-        bmpHeight = textHeight = bmpWidth = 0
-
-        if headerBmp and headerBmp.IsOk():
-            # We got the header bitmap
-            bmpHeight, bmpWidth = headerBmp.GetHeight(), headerBmp.GetWidth()
-            bmpXPos = self._spacing
-
-        if header:
-            # We got the header text
-            dc.SetFont(headerFont)
-            textWidth, textHeight = dc.GetTextExtent(header)
-            maxWidth = max(bmpWidth+(textWidth+self._spacing*2), maxWidth)
-        # Calculate the header height
-        height = max(textHeight, bmpHeight)
-        normalText = classParent.GetTextColour()
-        if header:
-            dc.SetTextForeground(normalText)
-            dc.DrawText(header, bmpXPos+bmpWidth+self._spacing, (height-textHeight+self._spacing)/2)
-        if headerBmp and headerBmp.IsOk():
-            dc.DrawBitmap(headerBmp, bmpXPos, (height-bmpHeight+self._spacing)/2, True)
-
-        if header or (headerBmp and headerBmp.IsOk()):
-            yPos += height
-            if drawHeader:
-                # Draw the separator line after the header
-                dc.SetPen(wx.GREY_PEN)
-                dc.DrawLine(self._spacing, yPos+self._spacing, width-self._spacing, yPos+self._spacing)
-                yPos += self._spacing
-
-        maxWidth = max(bmpXPos + bmpWidth + self._spacing, maxWidth)
-        # Get the big body image (if any)
-        embeddedImage = classParent.GetBodyImage()
-        bmpWidth = bmpHeight = -1
-        if embeddedImage and embeddedImage.IsOk():
-            bmpWidth, bmpHeight = embeddedImage.GetWidth(), embeddedImage.GetHeight()
-
-        # A bunch of calculations to draw the main body message
-        messageHeight = 0
-        lines = classParent.GetMessage().split("\n")
-        yText = yPos
-        embImgPos = yPos
-        hyperLinkText = wx.BLUE
-        messagePos = self._getTextExtent(dc, lines[0] if lines else "")[1] // 2 + self._spacing
-        for line in lines:
-            # Loop over all the lines in the message
-            if line.startswith("<hr>"):     # draw a line
-                yText += self._spacing * 2
-                dc.DrawLine(self._spacing, yText+self._spacing, width-self._spacing, yText+self._spacing)
-            else:
-                isLink = False
-                dc.SetTextForeground(normalText)
-                if line.startswith("</b>"):      # is a bold line
-                    line = line[4:]
-                    font = MakeBold(messageFont)
-                    dc.SetFont(font)
-                elif line.startswith("</l>"):    # is a link
-                    dc.SetFont(hyperlinkFont)
-                    isLink = True
-                    line, hl = ExtractLink(line)
-                    dc.SetTextForeground(hyperLinkText)
-                else:
-                    # Is a normal line
-                    dc.SetFont(messageFont)
-
-                textWidth, textHeight = self._getTextExtent(dc, line)
-
-                messageHeight += textHeight
-
-                xText = (bmpWidth + 2 * (self._spacing/2)) if bmpWidth > 0 else self._spacing
-                yText += textHeight/2+(self._spacing/2)
-                maxWidth = max(xText + textWidth + self._spacing, maxWidth)
-                dc.DrawText(line, xText, yText)
-                if isLink:
-                    self._storeHyperLinkInfo(xText, yText, textWidth, textHeight, hl)
-
-        toAdd = 0
-        if bmpHeight > messageHeight:
-            yPos += 2*self._spacing + bmpHeight
-            toAdd = self._spacing
-        else:
-            yPos += messageHeight + 2*self._spacing
-
-        yText = max(messageHeight, bmpHeight+2*self._spacing)
-        if embeddedImage and embeddedImage.IsOk():
-            # Draw the main body image
-            dc.DrawBitmap(embeddedImage, self._spacing, embImgPos + (self._spacing * 2), True)
-
-        footer, footerBmp = classParent.GetFooter(), classParent.GetFooterBitmap()
-        bmpHeight = bmpWidth = textHeight = textWidth = 0
-        bmpXPos = 0
-
-        if footerBmp and footerBmp.IsOk():
-            # Got the footer bitmap
-            bmpHeight, bmpWidth = footerBmp.GetHeight(), footerBmp.GetWidth()
-            bmpXPos = self._spacing
-
-        if footer:
-            # Got the footer text
-            footerFont.SetWeight(wx.FONTWEIGHT_NORMAL)
-            dc.SetFont(footerFont.Italic())
-            textWidth, textHeight = dc.GetTextExtent(footer)
-
-        if textHeight or bmpHeight:
-            if drawFooter:
-                # Draw the separator line before the footer
-                dc.SetPen(wx.GREY_PEN)
-                dc.DrawLine(self._spacing, yPos-self._spacing/2+toAdd,
-                            width-self._spacing, yPos-self._spacing/2+toAdd)
-        # Draw the footer and footer bitmap (if any)
-        dc.SetTextForeground(wx.Colour("#96B0DA"))
-        height = max(textHeight, bmpHeight)
-        yPos += toAdd
-        if footer:
-            toAdd = (height - textHeight + (self._spacing/2)) // 2
-            dc.DrawText(footer, bmpXPos + bmpWidth + self._spacing, yPos + toAdd)
-            maxWidth = max(bmpXPos + bmpWidth + (self._spacing/2) + textWidth, maxWidth)
-        if footerBmp and footerBmp.IsOk():
-            toAdd = (height - bmpHeight + (self._spacing/2)) / 2
-            dc.DrawBitmap(footerBmp, bmpXPos, yPos + toAdd, True)
-            maxWidth = max(footerBmp.GetSize().GetWidth() + bmpXPos, maxWidth)
-
-        maxHeight = yPos + height + toAdd + 8
-        if event is None:
-            return maxWidth, maxHeight
-
-
-    @staticmethod
-    def _getTextExtent(dc, line):
-        textWidth, textHeight = dc.GetTextExtent(line)
-        if textHeight == 0:
-            _, textHeight = dc.GetTextExtent("a")
-        return textWidth, textHeight
-
-    def _storeHyperLinkInfo(self, hTextPos, vTextPos, textWidth, textHeight, linkTarget):
-        # Store the hyperlink rectangle and link
-        self._hyperlinkRect.append(wx.Rect(hTextPos, vTextPos, textWidth, textHeight))
-        self._hyperlinkWeb.append(linkTarget)
-
-
-    def OnEraseBackground(self, event):
-        """
-        Handles the ``wx.EVT_ERASE_BACKGROUND`` event for :class:`SuperToolTip`.
-
-        :param `event`: a :class:`EraseEvent` event to be processed.
-
-        :note: This method is intentionally empty to reduce flicker.
-        """
-
-        # This is intentionally empty to reduce flicker
-        pass
-
-
-    def OnSize(self, event):
-        """
-        Handles the ``wx.EVT_SIZE`` event for :class:`SuperToolTip`.
-
-        :param `event`: a :class:`wx.SizeEvent` event to be processed.
-        """
-
-        self.Refresh()
-        event.Skip()
-
-
-    def OnMouseMotion(self, event):
-        """
-        Handles the ``wx.EVT_MOTION`` event for :class:`SuperToolTip`.
-
-        :param `event`: a :class:`MouseEvent` event to be processed.
-        """
-
-        x, y = event.GetPosition()
-        for rect in self._hyperlinkRect:
-            if rect.Contains((x, y)):
-                # We are over one hyperlink...
-                self.SetCursor(wx.Cursor(wx.CURSOR_HAND))
-                self._wasOnLink = True
-                return
-
-        if self._wasOnLink:
-            # Restore the normal cursor
-            self._wasOnLink = False
-            self.SetCursor(wx.NullCursor)
-
-
-    def OnDestroy(self, event):
-        """
-        Handles the ``wx.EVT_LEFT_DOWN``, ``wx.EVT_LEFT_DCLICK`` and ``wx.EVT_KILL_FOCUS``
-        events for :class:`SuperToolTip`. All these events destroy the :class:`SuperToolTip`,
-        unless the user clicked on one hyperlink.
-
-        :param `event`: a :class:`MouseEvent` or a :class:`FocusEvent` event to be processed.
-        """
-
-        if not isinstance(event, wx.MouseEvent):
-            # We haven't clicked a link
-            if self:  # Check if window still exists, Destroy might have been called manually (more than once)
-                self.Destroy()
-            return
-
-        x, y = event.GetPosition()
-        for indx, rect in enumerate(self._hyperlinkRect):
-            if rect.Contains((x, y)):
-                # Run the webbrowser with the clicked link
-                webbrowser.open_new_tab(self._hyperlinkWeb[indx])
-                return
-
-        self.Destroy()
-
-
-    def SetFont(self, font):
-        """
-        Sets the :class:`SuperToolTip` font globally.
-
-        :param `font`: the font to set.
-        """
-
-        wx.PopupWindow.SetFont(self, font)
-        self._classParent.InitFont()
-        self.Invalidate()
-
-
-    def Invalidate(self):
-        """ Invalidate :class:`SuperToolTip` size and repaint it. """
-
-        if not self._classParent.GetMessage():
-            # No message yet...
-            return
-
-        self.CalculateBestSize()
-        self.Refresh()
-
-    def CalculateBestSize(self):
-        """ Calculates the :class:`SuperToolTip` window best size. """
-
-        maxWidth, maxHeight = self.OnPaint(None)
-        self.SetSize((maxWidth, maxHeight))
-
-    def CalculateBestPosition(self, widget):
-        x, y = wx.GetMousePosition()
-        screen = wx.ClientDisplayRect()[2:]
-        left, top = widget.ClientToScreen((0, 0))
-        right, bottom = widget.ClientToScreen(widget.GetClientRect()[2:])
-        size = self.GetSize()
-
-        if x+size[0]>screen[0]:
-            xpos = x-size[0]
-        else:
-            xpos = x
-
-        if bottom+size[1]>screen[1]:
-            ypos = top-size[1] + 6
-        else:
-            ypos = bottom + 6
-
-        self.SetPosition((xpos,ypos))
-
-
-# Handle Mac and Windows/GTK differences...
-
-if wx.Platform == "__WXMAC__":
-
-    class ToolTipWindow(wx.Frame, ToolTipWindowBase):
-        """ Popup window that works on wxMac. """
-
-        def __init__(self, parent, classParent):
-            """
-            Default class constructor.
-
-            :param `parent`: the :class:`SuperToolTip` parent widget;
-            :param `classParent`: the :class:`SuperToolTip` class object.
-            """
-
-            wx.Frame.__init__(self, parent, style=wx.NO_BORDER|wx.FRAME_FLOAT_ON_PARENT|wx.FRAME_NO_TASKBAR|wx.POPUP_WINDOW)
-            # Call the base class
-            ToolTipWindowBase.__init__(self, parent, classParent)
-
-else:
-
-    class ToolTipWindow(ToolTipWindowBase, wx.PopupWindow):
-        """
-        A simple :class:`PopupWindow` that holds fancy tooltips.
-        Not available on Mac as :class:`PopupWindow` is not implemented there.
-        """
-
-        def __init__(self, parent, classParent):
-            """
-            Default class constructor.
-
-            :param `parent`: the :class:`SuperToolTip` parent widget;
-            :param `classParent`: the :class:`SuperToolTip` class object.
-            """
-
-            wx.PopupWindow.__init__(self, parent)
-            # Call the base class
-            ToolTipWindowBase.__init__(self, parent, classParent)
-
-
-
-class ToolTip(STT.SuperToolTip):
-    def __init__(self, header, message, target, bodyImage=wx.NullBitmap, headerBmp=wx.NullBitmap, footer="", footerBmp=wx.NullBitmap):
-        STT.SuperToolTip.__init__(self, message, bodyImage, header, headerBmp, footer, footerBmp)
-
-        self.SetHeader(header)
-        self.SetTarget(target)
-        self.SetStartDelay(.5)
-        self.SetTopGradientColour(wx.Colour("#272727"))
-        self.SetMiddleGradientColour(wx.Colour("#272727"))
-        self.SetBottomGradientColour(wx.Colour("#272727"))
-        self.SetTextColour(wx.Colour("#ccc"))
-
-    def OnStartTimer(self):
-        """ The creation time has expired, create the :class:`SuperToolTip`. """
-
-        # target widget might already be destroyed
-        if not self._widget:
-            self._startTimer.Stop()
-            return
-
-        tip = ToolTipWindow(self._widget, self)
-        self._superToolTip = tip
-        self._superToolTip.CalculateBestSize()
-        self._superToolTip.CalculateBestPosition(self._widget)
-
-        self._superToolTip.Show()
-
-        self._startTimer.Stop()
-        self._endTimer.Start(self._endDelayTime*1000)
-
-
-    def OnEndTimer(self):
-        """ The show time for :class:`SuperToolTip` has expired, destroy the :class:`SuperToolTip`. """
-
-        if self._superToolTip:
-            self._superToolTip.Destroy()
-
-        self._endTimer.Stop()
-
-
-    def DoShowNow(self):
-        """ Create the :class:`SuperToolTip` immediately. """
-
-        if self._superToolTip:
-            # need to destroy it if already exists,
-            # otherwise we might end up with many of them
-            self._superToolTip.Destroy()
-
-        tip = ToolTipWindow(self._widget, self)
-        self._superToolTip = tip
-        self._superToolTip.CalculateBestSize()
-        self._superToolTip.CalculateBestPosition(self._widget)
-
-        # need to stop this, otherwise we get into trouble when leaving the window
-        self._startTimer.Stop()
-
-        self._superToolTip.Show()
-
-        self._endTimer.Start(self._endDelayTime*1000)
-
+# ----------------------------------------------------------------------------
+# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
+#
+# This file includes modified code from wx.lib.agw.supertooltip
+#
+# ----------------------------------------------------------------------------
+
+import wx
+import wx.lib.agw.supertooltip as STT
+
+
+def MakeBold(font):
+    """
+    Makes a font bold. Utility method.
+
+    :param `font`: the font to be made bold.
+    """
+
+    newFont = wx.Font(font.GetPointSize(), font.GetFamily(), font.GetStyle(),
+                      wx.FONTWEIGHT_BOLD, font.GetUnderlined(), font.GetFaceName())
+
+    return newFont
+
+
+def ExtractLink(line):
+    """
+    Extract the link from an hyperlink line.
+
+    :param `line`: the line of text to be processed.
+    """
+
+    line = line[4:]
+    indxStart = line.find("{")
+    indxEnd = line.find("}")
+    hl = line[indxStart+1:indxEnd].strip()
+    line = line[0:indxStart].strip()
+
+    return line, hl
+
+
+class ToolTipWindowBase(object):
+    """ Base class for the different Windows and Mac implementation. """
+
+    def __init__(self, parent, classParent):
+        """
+        Default class constructor.
+
+        :param `parent`: the :class:`SuperToolTip` parent widget;
+        :param `classParent`: the :class:`SuperToolTip` class object.
+        """
+
+        self._spacing = 18
+        self._wasOnLink = False
+        self._hyperlinkRect, self._hyperlinkWeb = [], []
+
+        self._classParent = classParent
+
+        # Bind the events
+        self.Bind(wx.EVT_PAINT, self.OnPaint)
+        self.Bind(wx.EVT_SIZE, self.OnSize)
+        self.Bind(wx.EVT_ERASE_BACKGROUND, self.OnEraseBackground)
+        self.Bind(wx.EVT_MOTION, self.OnMouseMotion)
+        parent.Bind(wx.EVT_KILL_FOCUS, self.OnDestroy)
+        self.Bind(wx.EVT_LEFT_DOWN, self.OnDestroy)
+        self.Bind(wx.EVT_LEFT_DCLICK, self.OnDestroy)
+
+
+    def OnPaint(self, event):
+        """
+        Handles the ``wx.EVT_PAINT`` event for :class:`SuperToolTip`.
+
+        If the `event` parameter is ``None``, calculates best size and returns it.
+
+        :param `event`: a :class:`PaintEvent` event to be processed or ``None``.
+        """
+
+        maxWidth = 0
+        if event is None:
+            dc = wx.ClientDC(self)
+        else:
+            # Go with double buffering...
+            dc = wx.BufferedPaintDC(self)
+
+        frameRect = self.GetClientRect()
+        x, y, width, _height = frameRect
+        # Store the rects for the hyperlink lines
+        self._hyperlinkRect, self._hyperlinkWeb = [], []
+        classParent = self._classParent
+
+        # Retrieve the colours for the blended triple-gradient background
+        topColour, middleColour, bottomColour = classParent.GetTopGradientColour(), \
+                                                classParent.GetMiddleGradientColour(), \
+                                                classParent.GetBottomGradientColour()
+
+        # Get the user options for header, bitmaps etc...
+        drawHeader, drawFooter = classParent.GetDrawHeaderLine(), classParent.GetDrawFooterLine()
+        topRect = wx.Rect(frameRect.x, frameRect.y, frameRect.width, frameRect.height/2)
+        bottomRect = wx.Rect(frameRect.x, frameRect.y+frameRect.height/2, frameRect.width, frameRect.height/2+1)
+        # Fill the triple-gradient
+        dc.GradientFillLinear(topRect, topColour, middleColour, wx.SOUTH)
+        dc.GradientFillLinear(bottomRect, middleColour, bottomColour, wx.SOUTH)
+
+        header, headerBmp = classParent.GetHeader(), classParent.GetHeaderBitmap()
+        headerFont, messageFont, footerFont, hyperlinkFont = classParent.GetHeaderFont(), classParent.GetMessageFont(), \
+                                                             classParent.GetFooterFont(), classParent.GetHyperlinkFont()
+
+        yPos = 0
+        bmpXPos = 0
+        bmpHeight = textHeight = bmpWidth = 0
+
+        if headerBmp and headerBmp.IsOk():
+            # We got the header bitmap
+            bmpHeight, bmpWidth = headerBmp.GetHeight(), headerBmp.GetWidth()
+            bmpXPos = self._spacing
+
+        if header:
+            # We got the header text
+            dc.SetFont(headerFont)
+            textWidth, textHeight = dc.GetTextExtent(header)
+            maxWidth = max(bmpWidth+(textWidth+self._spacing*2), maxWidth)
+        # Calculate the header height
+        height = max(textHeight, bmpHeight)
+        normalText = classParent.GetTextColour()
+        if header:
+            dc.SetTextForeground(normalText)
+            dc.DrawText(header, bmpXPos+bmpWidth+self._spacing, (height-textHeight+self._spacing)/2)
+        if headerBmp and headerBmp.IsOk():
+            dc.DrawBitmap(headerBmp, bmpXPos, (height-bmpHeight+self._spacing)/2, True)
+
+        if header or (headerBmp and headerBmp.IsOk()):
+            yPos += height
+            if drawHeader:
+                # Draw the separator line after the header
+                dc.SetPen(wx.GREY_PEN)
+                dc.DrawLine(self._spacing, yPos+self._spacing, width-self._spacing, yPos+self._spacing)
+                yPos += self._spacing
+
+        maxWidth = max(bmpXPos + bmpWidth + self._spacing, maxWidth)
+        # Get the big body image (if any)
+        embeddedImage = classParent.GetBodyImage()
+        bmpWidth = bmpHeight = -1
+        if embeddedImage and embeddedImage.IsOk():
+            bmpWidth, bmpHeight = embeddedImage.GetWidth(), embeddedImage.GetHeight()
+
+        # A bunch of calculations to draw the main body message
+        messageHeight = 0
+        lines = classParent.GetMessage().split("\n")
+        yText = yPos
+        embImgPos = yPos
+        hyperLinkText = wx.BLUE
+        messagePos = self._getTextExtent(dc, lines[0] if lines else "")[1] // 2 + self._spacing
+        for line in lines:
+            # Loop over all the lines in the message
+            if line.startswith("<hr>"):     # draw a line
+                yText += self._spacing * 2
+                dc.DrawLine(self._spacing, yText+self._spacing, width-self._spacing, yText+self._spacing)
+            else:
+                isLink = False
+                dc.SetTextForeground(normalText)
+                if line.startswith("</b>"):      # is a bold line
+                    line = line[4:]
+                    font = MakeBold(messageFont)
+                    dc.SetFont(font)
+                elif line.startswith("</l>"):    # is a link
+                    dc.SetFont(hyperlinkFont)
+                    isLink = True
+                    line, hl = ExtractLink(line)
+                    dc.SetTextForeground(hyperLinkText)
+                else:
+                    # Is a normal line
+                    dc.SetFont(messageFont)
+
+                textWidth, textHeight = self._getTextExtent(dc, line)
+
+                messageHeight += textHeight
+
+                xText = (bmpWidth + 2 * (self._spacing/2)) if bmpWidth > 0 else self._spacing
+                yText += textHeight/2+(self._spacing/2)
+                maxWidth = max(xText + textWidth + self._spacing, maxWidth)
+                dc.DrawText(line, xText, yText)
+                if isLink:
+                    self._storeHyperLinkInfo(xText, yText, textWidth, textHeight, hl)
+
+        toAdd = 0
+        if bmpHeight > messageHeight:
+            yPos += 2*self._spacing + bmpHeight
+            toAdd = self._spacing
+        else:
+            yPos += messageHeight + 2*self._spacing
+
+        yText = max(messageHeight, bmpHeight+2*self._spacing)
+        if embeddedImage and embeddedImage.IsOk():
+            # Draw the main body image
+            dc.DrawBitmap(embeddedImage, self._spacing, embImgPos + (self._spacing * 2), True)
+
+        footer, footerBmp = classParent.GetFooter(), classParent.GetFooterBitmap()
+        bmpHeight = bmpWidth = textHeight = textWidth = 0
+        bmpXPos = 0
+
+        if footerBmp and footerBmp.IsOk():
+            # Got the footer bitmap
+            bmpHeight, bmpWidth = footerBmp.GetHeight(), footerBmp.GetWidth()
+            bmpXPos = self._spacing
+
+        if footer:
+            # Got the footer text
+            footerFont.SetWeight(wx.FONTWEIGHT_NORMAL)
+            dc.SetFont(footerFont.Italic())
+            textWidth, textHeight = dc.GetTextExtent(footer)
+
+        if textHeight or bmpHeight:
+            if drawFooter:
+                # Draw the separator line before the footer
+                dc.SetPen(wx.GREY_PEN)
+                dc.DrawLine(self._spacing, yPos-self._spacing/2+toAdd,
+                            width-self._spacing, yPos-self._spacing/2+toAdd)
+        # Draw the footer and footer bitmap (if any)
+        dc.SetTextForeground(wx.Colour("#96B0DA"))
+        height = max(textHeight, bmpHeight)
+        yPos += toAdd
+        if footer:
+            toAdd = (height - textHeight + (self._spacing/2)) // 2
+            dc.DrawText(footer, bmpXPos + bmpWidth + self._spacing, yPos + toAdd)
+            maxWidth = max(bmpXPos + bmpWidth + (self._spacing/2) + textWidth, maxWidth)
+        if footerBmp and footerBmp.IsOk():
+            toAdd = (height - bmpHeight + (self._spacing/2)) / 2
+            dc.DrawBitmap(footerBmp, bmpXPos, yPos + toAdd, True)
+            maxWidth = max(footerBmp.GetSize().GetWidth() + bmpXPos, maxWidth)
+
+        maxHeight = yPos + height + toAdd + 8
+        if event is None:
+            return maxWidth, maxHeight
+
+
+    @staticmethod
+    def _getTextExtent(dc, line):
+        textWidth, textHeight = dc.GetTextExtent(line)
+        if textHeight == 0:
+            _, textHeight = dc.GetTextExtent("a")
+        return textWidth, textHeight
+
+    def _storeHyperLinkInfo(self, hTextPos, vTextPos, textWidth, textHeight, linkTarget):
+        # Store the hyperlink rectangle and link
+        self._hyperlinkRect.append(wx.Rect(hTextPos, vTextPos, textWidth, textHeight))
+        self._hyperlinkWeb.append(linkTarget)
+
+
+    def OnEraseBackground(self, event):
+        """
+        Handles the ``wx.EVT_ERASE_BACKGROUND`` event for :class:`SuperToolTip`.
+
+        :param `event`: a :class:`EraseEvent` event to be processed.
+
+        :note: This method is intentionally empty to reduce flicker.
+        """
+
+        # This is intentionally empty to reduce flicker
+        pass
+
+
+    def OnSize(self, event):
+        """
+        Handles the ``wx.EVT_SIZE`` event for :class:`SuperToolTip`.
+
+        :param `event`: a :class:`wx.SizeEvent` event to be processed.
+        """
+
+        self.Refresh()
+        event.Skip()
+
+
+    def OnMouseMotion(self, event):
+        """
+        Handles the ``wx.EVT_MOTION`` event for :class:`SuperToolTip`.
+
+        :param `event`: a :class:`MouseEvent` event to be processed.
+        """
+
+        x, y = event.GetPosition()
+        for rect in self._hyperlinkRect:
+            if rect.Contains((x, y)):
+                # We are over one hyperlink...
+                self.SetCursor(wx.Cursor(wx.CURSOR_HAND))
+                self._wasOnLink = True
+                return
+
+        if self._wasOnLink:
+            # Restore the normal cursor
+            self._wasOnLink = False
+            self.SetCursor(wx.NullCursor)
+
+
+    def OnDestroy(self, event):
+        """
+        Handles the ``wx.EVT_LEFT_DOWN``, ``wx.EVT_LEFT_DCLICK`` and ``wx.EVT_KILL_FOCUS``
+        events for :class:`SuperToolTip`. All these events destroy the :class:`SuperToolTip`,
+        unless the user clicked on one hyperlink.
+
+        :param `event`: a :class:`MouseEvent` or a :class:`FocusEvent` event to be processed.
+        """
+
+        if not isinstance(event, wx.MouseEvent):
+            # We haven't clicked a link
+            if self:  # Check if window still exists, Destroy might have been called manually (more than once)
+                self.Destroy()
+            return
+
+        x, y = event.GetPosition()
+        for indx, rect in enumerate(self._hyperlinkRect):
+            if rect.Contains((x, y)):
+                # Run the webbrowser with the clicked link
+                webbrowser.open_new_tab(self._hyperlinkWeb[indx])
+                return
+
+        self.Destroy()
+
+
+    def SetFont(self, font):
+        """
+        Sets the :class:`SuperToolTip` font globally.
+
+        :param `font`: the font to set.
+        """
+
+        wx.PopupWindow.SetFont(self, font)
+        self._classParent.InitFont()
+        self.Invalidate()
+
+
+    def Invalidate(self):
+        """ Invalidate :class:`SuperToolTip` size and repaint it. """
+
+        if not self._classParent.GetMessage():
+            # No message yet...
+            return
+
+        self.CalculateBestSize()
+        self.Refresh()
+
+    def CalculateBestSize(self):
+        """ Calculates the :class:`SuperToolTip` window best size. """
+
+        maxWidth, maxHeight = self.OnPaint(None)
+        self.SetSize((maxWidth, maxHeight))
+
+    def CalculateBestPosition(self, widget):
+        x, y = wx.GetMousePosition()
+        screen = wx.ClientDisplayRect()[2:]
+        left, top = widget.ClientToScreen((0, 0))
+        right, bottom = widget.ClientToScreen(widget.GetClientRect()[2:])
+        size = self.GetSize()
+
+        if x+size[0]>screen[0]:
+            xpos = x-size[0]
+        else:
+            xpos = x
+
+        if bottom+size[1]>screen[1]:
+            ypos = top-size[1] + 6
+        else:
+            ypos = bottom + 6
+
+        self.SetPosition((xpos,ypos))
+
+
+# Handle Mac and Windows/GTK differences...
+
+if wx.Platform == "__WXMAC__":
+
+    class ToolTipWindow(wx.Frame, ToolTipWindowBase):
+        """ Popup window that works on wxMac. """
+
+        def __init__(self, parent, classParent):
+            """
+            Default class constructor.
+
+            :param `parent`: the :class:`SuperToolTip` parent widget;
+            :param `classParent`: the :class:`SuperToolTip` class object.
+            """
+
+            wx.Frame.__init__(self, parent, style=wx.NO_BORDER|wx.FRAME_FLOAT_ON_PARENT|wx.FRAME_NO_TASKBAR|wx.POPUP_WINDOW)
+            # Call the base class
+            ToolTipWindowBase.__init__(self, parent, classParent)
+
+else:
+
+    class ToolTipWindow(ToolTipWindowBase, wx.PopupWindow):
+        """
+        A simple :class:`PopupWindow` that holds fancy tooltips.
+        Not available on Mac as :class:`PopupWindow` is not implemented there.
+        """
+
+        def __init__(self, parent, classParent):
+            """
+            Default class constructor.
+
+            :param `parent`: the :class:`SuperToolTip` parent widget;
+            :param `classParent`: the :class:`SuperToolTip` class object.
+            """
+
+            wx.PopupWindow.__init__(self, parent)
+            # Call the base class
+            ToolTipWindowBase.__init__(self, parent, classParent)
+
+
+
+class ToolTip(STT.SuperToolTip):
+    def __init__(self, header, message, target, bodyImage=wx.NullBitmap, headerBmp=wx.NullBitmap, footer="", footerBmp=wx.NullBitmap):
+        STT.SuperToolTip.__init__(self, message, bodyImage, header, headerBmp, footer, footerBmp)
+
+        self.SetHeader(header)
+        self.SetTarget(target)
+        self.SetStartDelay(.5)
+        self.SetTopGradientColour(wx.Colour("#272727"))
+        self.SetMiddleGradientColour(wx.Colour("#272727"))
+        self.SetBottomGradientColour(wx.Colour("#272727"))
+        self.SetTextColour(wx.Colour("#ccc"))
+
+    def OnStartTimer(self):
+        """ The creation time has expired, create the :class:`SuperToolTip`. """
+
+        # target widget might already be destroyed
+        if not self._widget:
+            self._startTimer.Stop()
+            return
+
+        tip = ToolTipWindow(self._widget, self)
+        self._superToolTip = tip
+        self._superToolTip.CalculateBestSize()
+        self._superToolTip.CalculateBestPosition(self._widget)
+
+        self._superToolTip.Show()
+
+        self._startTimer.Stop()
+        self._endTimer.Start(self._endDelayTime*1000)
+
+
+    def OnEndTimer(self):
+        """ The show time for :class:`SuperToolTip` has expired, destroy the :class:`SuperToolTip`. """
+
+        if self._superToolTip:
+            self._superToolTip.Destroy()
+
+        self._endTimer.Stop()
+
+
+    def DoShowNow(self):
+        """ Create the :class:`SuperToolTip` immediately. """
+
+        if self._superToolTip:
+            # need to destroy it if already exists,
+            # otherwise we might end up with many of them
+            self._superToolTip.Destroy()
+
+        tip = ToolTipWindow(self._widget, self)
+        self._superToolTip = tip
+        self._superToolTip.CalculateBestSize()
+        self._superToolTip.CalculateBestPosition(self._widget)
+
+        # need to stop this, otherwise we get into trouble when leaving the window
+        self._startTimer.Stop()
+
+        self._superToolTip.Show()
+
+        self._endTimer.Start(self._endDelayTime*1000)
+
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/utils.py` & `gswidgetkit-0.3.3/gswidgetkit/utils.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ----------------------------------------------------------------------------
-# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
-
-def GetTextExtent(text):
-    tdc = wx.WindowDC(wx.GetApp().GetTopWindow())
-    w, h = tdc.GetTextExtent(text)
-    return w, h
+# ----------------------------------------------------------------------------
+# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
+
+def GetTextExtent(text):
+    tdc = wx.WindowDC(wx.GetApp().GetTopWindow())
+    w, h = tdc.GetTextExtent(text)
+    return w, h
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit/z_matrix.py` & `gswidgetkit-0.3.3/gswidgetkit/z_matrix.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-# ----------------------------------------------------------------------------
-# Gimel Studio Copyright 2021-2022 by Noah Rahm and contributors
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
-#
-# This file is code originally from EmbroidePy
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
+# Gimel Studio Copyright 2021-2022 by Noah Rahm and contributors
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
+#
+# This file is code originally from EmbroidePy
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

### Comparing `gswidgetkit-0.3.2/gswidgetkit/zoom_panel.py` & `gswidgetkit-0.3.3/gswidgetkit/zoom_panel.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-# ----------------------------------------------------------------------------
-# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
-from .z_matrix import ZMatrix
-
-
-class ZoomPanel(wx.Panel):
-    def __init__(self, *args, **kwds):
-        self.matrix = ZMatrix()
-        self.identity = ZMatrix()
-        self.matrix.Reset()
-        self.identity.Reset()
-        self.previous_position = None
-        self._Buffer = None
-
-        kwds["style"] = kwds.get("style", 0) | wx.DEFAULT_FRAME_STYLE
-        wx.Panel.__init__(self, *args, **kwds)
-
-        self.Bind(wx.EVT_PAINT, self.OnPaint)
-        self.Bind(wx.EVT_ERASE_BACKGROUND, lambda x: None)
-        self.Bind(wx.EVT_MOTION, self.OnMouseMove)
-        self.Bind(wx.EVT_MOUSEWHEEL, self.OnMousewheel)
-        self.Bind(wx.EVT_MIDDLE_DOWN, self.OnMouseMiddleDown)
-        self.Bind(wx.EVT_MIDDLE_UP, self.OnMouseMiddleUp)
-        self.Bind(wx.EVT_SIZE, self.OnSize)
-
-    def OnPaint(self, event):
-        dc = wx.BufferedPaintDC(self, self._Buffer)
-
-    def OnSize(self, event):
-        size = self.GetClientSize()
-
-        # Make sure size is at least 1px to avoid
-        # strange "invalid bitmap size" errors.
-        if size[0] < 1:
-            size = (10, 10)
-        self._Buffer = wx.Bitmap(*size)
-        self.UpdateDrawing()
-
-    def UpdateDrawing(self):
-        dc = wx.MemoryDC()
-        dc.SelectObject(self._Buffer)
-        self.OnDrawBackground(dc)
-        dc.SetTransformMatrix(self.matrix)
-        self.OnDrawScene(dc)
-        dc.SetTransformMatrix(self.identity)
-        self.OnDrawInterface(dc)
-        del dc  # need to get rid of the MemoryDC before Update() is called.
-        self.Refresh()
-        self.Update()
-
-    def OnDrawBackground(self, dc):
-        pass
-
-    def OnDrawScene(self, dc):
-        pass
-
-    def OnDrawInterface(self, dc):
-        pass
-
-    def SceneMatrixReset(self):
-        self.matrix.Reset()
-
-    def ScenePostScale(self, sx, sy=None, ax=0, ay=0):
-        self.matrix.PostScale(sx, sy, ax, ay)
-
-    def ScenePostPan(self, px, py):
-        self.matrix.PostTranslate(px, py)
-
-    def ScenePostRotate(self, angle, rx=0, ry=0):
-        self.matrix.PostRotate(angle, rx, ry)
-
-    def ScenePreScale(self, sx, sy=None, ax=0, ay=0):
-        self.matrix.PreScale(sx, sy, ax, ay)
-
-    def ScenePrePan(self, px, py):
-        self.matrix.PreTranslate(px, py)
-
-    def ScenePreRotate(self, angle, rx=0, ry=0):
-        self.matrix.PreRotate(angle, rx, ry)
-
-    def GetScaleX(self):
-        return self.matrix.GetScaleX()
-
-    def GetScaleY(self):
-        return self.matrix.GetScaleY()
-
-    def GetSkewX(self):
-        return self.matrix.GetSkewX()
-
-    def GetSkewY(self):
-        return self.matrix.GetSkewY()
-
-    def GetTranslateX(self):
-        return self.matrix.GetTranslateX()
-
-    def GetTranslateY(self):
-        return self.matrix.GetTranslateY()
-
-    def OnMousewheel(self, event):
-        rotation = event.GetWheelRotation()
-        mouse = event.GetPosition()
-        if rotation > 1:
-            self.ScenePostScale(1.1, 1.1, mouse[0], mouse[1])
-        elif rotation < -1:
-            self.ScenePostScale(0.9, 0.9, mouse[0], mouse[1])
-        self.UpdateDrawing()
-
-    def OnMouseMiddleDown(self, event):
-        self.previous_position = event.GetPosition()
-        self.SetCursor(wx.Cursor(wx.CURSOR_SIZING))
-
-    def OnMouseMiddleUp(self, event):
-        self.previous_position = None
-        self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
-
-    def OnMouseMove(self, event):
-        if self.previous_position is None:
-            return
-        scene_position = event.GetPosition()
-        previous_scene_position = self.previous_position
-        dx = (scene_position[0] - previous_scene_position[0])
-        dy = (scene_position[1] - previous_scene_position[1])
-        self.ScenePostPan(dx, dy)
-        self.UpdateDrawing()
-        self.previous_position = scene_position
-
-    def FocusPositionScene(self, scene_point):
-        window_width, window_height = self.ClientSize
-        scale_x = self.GetScaleX()
-        scale_y = self.GetScaleY()
-        self.SceneMatrixReset()
-        self.ScenePostPan(-scene_point[0], -scene_point[1])
-        self.ScenePostScale(scale_x, scale_y)
-        self.ScenePostPan(window_width / 2.0, window_height / 2.0)
-
-    def FocusViewportScene(self, new_scene_viewport, buffer=0, lock=True):
-        window_width, window_height = self.ClientSize
-        left = new_scene_viewport[0]
-        top = new_scene_viewport[1]
-        right = new_scene_viewport[2]
-        bottom = new_scene_viewport[3]
-        viewport_width = right - left
-        viewport_height = bottom - top
-
-        left -= viewport_width * buffer
-        right += viewport_width * buffer
-        top -= viewport_height * buffer
-        bottom += viewport_height * buffer
-
-        if right == left:
-            scale_x = 100
-        else:
-            scale_x = window_width / float(right - left)
-        if bottom == top:
-            scale_y = 100
-        else:
-            scale_y = window_height / float(bottom - top)
-
-        cx = ((right + left) / 2)
-        cy = ((top + bottom) / 2)
-        self.matrix.Reset()
-        self.matrix.PostTranslate(-cx, -cy)
-        if lock:
-            scale = min(scale_x, scale_y)
-            if scale != 0:
-                self.matrix.PostScale(scale)
-        else:
-            if scale_x != 0 and scale_y != 0:
-                self.matrix.PostScale(scale_x, scale_y)
-        self.matrix.PostTranslate(window_width / 2.0, window_height / 2.0)
-
-    def ConvertSceneToWindow(self, position):
-        return self.matrix.TransformPoint([position[0], position[1]])
-
-    def ConvertWindowToScene(self, position):
-        return self.matrix.InverseTransformPoint([position[0], position[1]])
+# ----------------------------------------------------------------------------
+# gswidgetkit Copyright 2021-2022 by Noah Rahm and contributors
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
+from .z_matrix import ZMatrix
+
+
+class ZoomPanel(wx.Panel):
+    def __init__(self, *args, **kwds):
+        self.matrix = ZMatrix()
+        self.identity = ZMatrix()
+        self.matrix.Reset()
+        self.identity.Reset()
+        self.previous_position = None
+        self._Buffer = None
+
+        kwds["style"] = kwds.get("style", 0) | wx.DEFAULT_FRAME_STYLE
+        wx.Panel.__init__(self, *args, **kwds)
+
+        self.Bind(wx.EVT_PAINT, self.OnPaint)
+        self.Bind(wx.EVT_ERASE_BACKGROUND, lambda x: None)
+        self.Bind(wx.EVT_MOTION, self.OnMouseMove)
+        self.Bind(wx.EVT_MOUSEWHEEL, self.OnMousewheel)
+        self.Bind(wx.EVT_MIDDLE_DOWN, self.OnMouseMiddleDown)
+        self.Bind(wx.EVT_MIDDLE_UP, self.OnMouseMiddleUp)
+        self.Bind(wx.EVT_SIZE, self.OnSize)
+
+    def OnPaint(self, event):
+        dc = wx.BufferedPaintDC(self, self._Buffer)
+
+    def OnSize(self, event):
+        size = self.GetClientSize()
+
+        # Make sure size is at least 1px to avoid
+        # strange "invalid bitmap size" errors.
+        if size[0] < 1:
+            size = (10, 10)
+        self._Buffer = wx.Bitmap(*size)
+        self.UpdateDrawing()
+
+    def UpdateDrawing(self):
+        dc = wx.MemoryDC()
+        dc.SelectObject(self._Buffer)
+        self.OnDrawBackground(dc)
+        dc.SetTransformMatrix(self.matrix)
+        self.OnDrawScene(dc)
+        dc.SetTransformMatrix(self.identity)
+        self.OnDrawInterface(dc)
+        del dc  # need to get rid of the MemoryDC before Update() is called.
+        self.Refresh()
+        self.Update()
+
+    def OnDrawBackground(self, dc):
+        pass
+
+    def OnDrawScene(self, dc):
+        pass
+
+    def OnDrawInterface(self, dc):
+        pass
+
+    def SceneMatrixReset(self):
+        self.matrix.Reset()
+
+    def ScenePostScale(self, sx, sy=None, ax=0, ay=0):
+        self.matrix.PostScale(sx, sy, ax, ay)
+
+    def ScenePostPan(self, px, py):
+        self.matrix.PostTranslate(px, py)
+
+    def ScenePostRotate(self, angle, rx=0, ry=0):
+        self.matrix.PostRotate(angle, rx, ry)
+
+    def ScenePreScale(self, sx, sy=None, ax=0, ay=0):
+        self.matrix.PreScale(sx, sy, ax, ay)
+
+    def ScenePrePan(self, px, py):
+        self.matrix.PreTranslate(px, py)
+
+    def ScenePreRotate(self, angle, rx=0, ry=0):
+        self.matrix.PreRotate(angle, rx, ry)
+
+    def GetScaleX(self):
+        return self.matrix.GetScaleX()
+
+    def GetScaleY(self):
+        return self.matrix.GetScaleY()
+
+    def GetSkewX(self):
+        return self.matrix.GetSkewX()
+
+    def GetSkewY(self):
+        return self.matrix.GetSkewY()
+
+    def GetTranslateX(self):
+        return self.matrix.GetTranslateX()
+
+    def GetTranslateY(self):
+        return self.matrix.GetTranslateY()
+
+    def OnMousewheel(self, event):
+        rotation = event.GetWheelRotation()
+        mouse = event.GetPosition()
+        if rotation > 1:
+            self.ScenePostScale(1.1, 1.1, mouse[0], mouse[1])
+        elif rotation < -1:
+            self.ScenePostScale(0.9, 0.9, mouse[0], mouse[1])
+        self.UpdateDrawing()
+
+    def OnMouseMiddleDown(self, event):
+        self.previous_position = event.GetPosition()
+        self.SetCursor(wx.Cursor(wx.CURSOR_SIZING))
+
+    def OnMouseMiddleUp(self, event):
+        self.previous_position = None
+        self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
+
+    def OnMouseMove(self, event):
+        if self.previous_position is None:
+            return
+        scene_position = event.GetPosition()
+        previous_scene_position = self.previous_position
+        dx = (scene_position[0] - previous_scene_position[0])
+        dy = (scene_position[1] - previous_scene_position[1])
+        self.ScenePostPan(dx, dy)
+        self.UpdateDrawing()
+        self.previous_position = scene_position
+
+    def FocusPositionScene(self, scene_point):
+        window_width, window_height = self.ClientSize
+        scale_x = self.GetScaleX()
+        scale_y = self.GetScaleY()
+        self.SceneMatrixReset()
+        self.ScenePostPan(-scene_point[0], -scene_point[1])
+        self.ScenePostScale(scale_x, scale_y)
+        self.ScenePostPan(window_width / 2.0, window_height / 2.0)
+
+    def FocusViewportScene(self, new_scene_viewport, buffer=0, lock=True):
+        window_width, window_height = self.ClientSize
+        left = new_scene_viewport[0]
+        top = new_scene_viewport[1]
+        right = new_scene_viewport[2]
+        bottom = new_scene_viewport[3]
+        viewport_width = right - left
+        viewport_height = bottom - top
+
+        left -= viewport_width * buffer
+        right += viewport_width * buffer
+        top -= viewport_height * buffer
+        bottom += viewport_height * buffer
+
+        if right == left:
+            scale_x = 100
+        else:
+            scale_x = window_width / float(right - left)
+        if bottom == top:
+            scale_y = 100
+        else:
+            scale_y = window_height / float(bottom - top)
+
+        cx = ((right + left) / 2)
+        cy = ((top + bottom) / 2)
+        self.matrix.Reset()
+        self.matrix.PostTranslate(-cx, -cy)
+        if lock:
+            scale = min(scale_x, scale_y)
+            if scale != 0:
+                self.matrix.PostScale(scale)
+        else:
+            if scale_x != 0 and scale_y != 0:
+                self.matrix.PostScale(scale_x, scale_y)
+        self.matrix.PostTranslate(window_width / 2.0, window_height / 2.0)
+
+    def ConvertSceneToWindow(self, position):
+        return self.matrix.TransformPoint([position[0], position[1]])
+
+    def ConvertWindowToScene(self, position):
+        return self.matrix.InverseTransformPoint([position[0], position[1]])
```

### Comparing `gswidgetkit-0.3.2/gswidgetkit.egg-info/SOURCES.txt` & `gswidgetkit-0.3.3/gswidgetkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*


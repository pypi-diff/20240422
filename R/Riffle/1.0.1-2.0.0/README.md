# Comparing `tmp/Riffle-1.0.1.tar.gz` & `tmp/Riffle-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Riffle-1.0.1.tar", last modified: Tue Mar 30 10:24:55 2021, max compression
+gzip compressed data, was "Riffle-2.0.0.tar", last modified: Mon Apr 22 08:52:28 2024, max compression
```

## Comparing `Riffle-1.0.1.tar` & `Riffle-2.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)        0 2021-03-30 10:24:44.000000 Riffle-1.0.1/
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)    10173 2020-10-13 08:15:12.000000 Riffle-1.0.1/LICENSE.txt
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)       78 2020-10-13 08:15:12.000000 Riffle-1.0.1/MANIFEST.in
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)     1839 2021-03-30 10:24:44.000000 Riffle-1.0.1/PKG-INFO
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      983 2020-10-13 08:15:12.000000 Riffle-1.0.1/README.rst
-drwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)        0 2021-03-30 10:24:43.000000 Riffle-1.0.1/resource/
-drwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)        0 2021-03-30 10:24:43.000000 Riffle-1.0.1/resource/icon/
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      504 2020-10-13 08:15:12.000000 Riffle-1.0.1/resource/icon/arrow_left.png
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      497 2020-10-13 08:15:12.000000 Riffle-1.0.1/resource/icon/arrow_right.png
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      492 2020-10-13 08:15:12.000000 Riffle-1.0.1/resource/icon/arrow_up.png
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      400 2020-10-13 08:15:12.000000 Riffle-1.0.1/resource/icon/collection.png
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      193 2020-10-13 08:15:12.000000 Riffle-1.0.1/resource/icon/document.png
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      308 2020-10-13 08:15:12.000000 Riffle-1.0.1/resource/icon/drive.png
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      262 2020-10-13 08:15:12.000000 Riffle-1.0.1/resource/icon/folder.png
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      241 2020-10-13 08:15:12.000000 Riffle-1.0.1/resource/icon/screen.png
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      527 2020-10-13 08:15:12.000000 Riffle-1.0.1/resource/resource.qrc
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)       38 2021-03-30 10:24:44.000000 Riffle-1.0.1/setup.cfg
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)     6339 2021-03-30 10:23:26.000000 Riffle-1.0.1/setup.py
-drwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)        0 2021-03-30 10:24:43.000000 Riffle-1.0.1/source/
-drwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)        0 2021-03-30 10:24:44.000000 Riffle-1.0.1/source/Riffle.egg-info/
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)     1839 2021-03-30 10:24:43.000000 Riffle-1.0.1/source/Riffle.egg-info/PKG-INFO
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      621 2021-03-30 10:24:43.000000 Riffle-1.0.1/source/Riffle.egg-info/SOURCES.txt
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)        1 2021-03-30 10:24:43.000000 Riffle-1.0.1/source/Riffle.egg-info/dependency_links.txt
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      256 2021-03-30 10:24:43.000000 Riffle-1.0.1/source/Riffle.egg-info/requires.txt
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)        7 2021-03-30 10:24:43.000000 Riffle-1.0.1/source/Riffle.egg-info/top_level.txt
-drwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)        0 2021-03-30 10:24:44.000000 Riffle-1.0.1/source/riffle/
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)      139 2020-10-13 08:15:12.000000 Riffle-1.0.1/source/riffle/__init__.py
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)       23 2021-03-30 10:23:58.000000 Riffle-1.0.1/source/riffle/_version.py
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)     9487 2021-03-25 14:23:06.000000 Riffle-1.0.1/source/riffle/browser.py
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)     1982 2020-10-13 08:15:12.000000 Riffle-1.0.1/source/riffle/icon_factory.py
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)    15192 2021-03-25 14:23:06.000000 Riffle-1.0.1/source/riffle/model.py
--rwxrwxrwx   0 ftrackwork  (1001) ftrackwork  (1001)    11070 2021-03-25 14:30:17.000000 Riffle-1.0.1/source/riffle/resource.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:52:28.855152 Riffle-2.0.0/
+-rw-rw-rw-   0        0        0    10349 2024-04-22 07:25:17.000000 Riffle-2.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       81 2024-04-22 07:25:17.000000 Riffle-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1617 2024-04-22 08:52:28.854155 Riffle-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1020 2024-04-22 07:25:17.000000 Riffle-2.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-22 08:52:28.818649 Riffle-2.0.0/resource/
+drwxrwxrwx   0        0        0        0 2024-04-22 08:52:28.826763 Riffle-2.0.0/resource/icon/
+-rw-rw-rw-   0        0        0      504 2024-04-22 07:25:17.000000 Riffle-2.0.0/resource/icon/arrow_left.png
+-rw-rw-rw-   0        0        0      497 2024-04-22 07:25:17.000000 Riffle-2.0.0/resource/icon/arrow_right.png
+-rw-rw-rw-   0        0        0      492 2024-04-22 07:25:17.000000 Riffle-2.0.0/resource/icon/arrow_up.png
+-rw-rw-rw-   0        0        0      400 2024-04-22 07:25:17.000000 Riffle-2.0.0/resource/icon/collection.png
+-rw-rw-rw-   0        0        0      193 2024-04-22 07:25:17.000000 Riffle-2.0.0/resource/icon/document.png
+-rw-rw-rw-   0        0        0      308 2024-04-22 07:25:17.000000 Riffle-2.0.0/resource/icon/drive.png
+-rw-rw-rw-   0        0        0      262 2024-04-22 07:25:17.000000 Riffle-2.0.0/resource/icon/folder.png
+-rw-rw-rw-   0        0        0      241 2024-04-22 07:25:17.000000 Riffle-2.0.0/resource/icon/screen.png
+-rw-rw-rw-   0        0        0      539 2024-04-22 07:25:17.000000 Riffle-2.0.0/resource/resource.qrc
+-rw-rw-rw-   0        0        0       42 2024-04-22 08:52:28.855152 Riffle-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     6602 2024-04-22 08:50:02.000000 Riffle-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:52:28.811471 Riffle-2.0.0/source/
+drwxrwxrwx   0        0        0        0 2024-04-22 08:52:28.846835 Riffle-2.0.0/source/Riffle.egg-info/
+-rw-rw-rw-   0        0        0     1617 2024-04-22 08:52:28.000000 Riffle-2.0.0/source/Riffle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2024-04-22 08:52:28.000000 Riffle-2.0.0/source/Riffle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 08:52:28.000000 Riffle-2.0.0/source/Riffle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      254 2024-04-22 08:52:28.000000 Riffle-2.0.0/source/Riffle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-22 08:52:28.000000 Riffle-2.0.0/source/Riffle.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 08:52:28.853154 Riffle-2.0.0/source/riffle/
+-rw-rw-rw-   0        0        0      144 2024-04-22 07:25:17.000000 Riffle-2.0.0/source/riffle/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-04-22 08:35:56.000000 Riffle-2.0.0/source/riffle/_version.py
+-rw-rw-rw-   0        0        0     9881 2024-04-22 08:34:11.000000 Riffle-2.0.0/source/riffle/browser.py
+-rw-rw-rw-   0        0        0     2038 2024-04-22 08:34:11.000000 Riffle-2.0.0/source/riffle/icon_factory.py
+-rw-rw-rw-   0        0        0    15939 2024-04-22 08:34:11.000000 Riffle-2.0.0/source/riffle/model.py
+-rw-rw-rw-   0        0        0    11437 2024-04-22 08:51:57.000000 Riffle-2.0.0/source/riffle/resource.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Riffle-1.0.1/LICENSE.txt` & `Riffle-2.0.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,176 +1,176 @@
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
```

### Comparing `Riffle-1.0.1/PKG-INFO` & `Riffle-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,58 @@
-Metadata-Version: 2.1
-Name: Riffle
-Version: 1.0.1
-Summary: Filesystem browser for PySide.
-Home-page: https://gitlab.com/4degrees/riffle
-Author: Martin Pengelly-Phillips
-Author-email: martin@4degrees.ltd.uk
-License: Apache License (2.0)
-Description: ######
-        Riffle
-        ######
-        
-        A filesystem browser for PySide.
-        
-        *************
-        Documentation
-        *************
-        
-        Full documentation can be found at http://riffle.readthedocs.org
-        
-        *************
-        Issue tracker
-        *************
-        
-        Found a bug? Have an idea on how to make the tool better?
-        
-        Post it at https://gitlab.com/4degrees/riffle/issues
-        
-        *********************
-        Copyright and license
-        *********************
-        
-        Copyright (c) 2014 Martin Pengelly-Phillips
-        
-        Licensed under the Apache License, Version 2.0 (the "License"); you may not use
-        this work except in compliance with the License. You may obtain a copy of the
-        License in the LICENSE.txt file, or at:
-        
-        http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software distributed
-        under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
-        CONDITIONS OF ANY KIND, either express or implied. See the License for the
-        specific language governing permissions and limitations under the License.
-        
-        
-Keywords: filesystem,browser,pyside,qt,pyqt
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.0, <4.0
-Provides-Extra: setup
-Provides-Extra: tests
-Provides-Extra: dev
+Metadata-Version: 2.1
+Name: Riffle
+Version: 2.0.0
+Summary: Filesystem browser for PySide.
+Home-page: https://gitlab.com/4degrees/riffle
+Author: Martin Pengelly-Phillips
+Author-email: martin@4degrees.ltd.uk
+License: Apache License (2.0)
+Keywords: filesystem,browser,pyside,qt,pyqt
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8, <3.13
+Provides-Extra: setup
+Provides-Extra: tests
+Provides-Extra: dev
+License-File: LICENSE.txt
+
+######
+Riffle
+######
+
+A filesystem browser for PySide.
+
+*************
+Documentation
+*************
+
+Full documentation can be found at http://riffle.readthedocs.org
+
+*************
+Issue tracker
+*************
+
+Found a bug? Have an idea on how to make the tool better?
+
+Post it at https://gitlab.com/4degrees/riffle/issues
+
+*********************
+Copyright and license
+*********************
+
+Copyright (c) 2014 Martin Pengelly-Phillips
+
+Licensed under the Apache License, Version 2.0 (the "License"); you may not use
+this work except in compliance with the License. You may obtain a copy of the
+License in the LICENSE.txt file, or at:
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software distributed
+under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
+CONDITIONS OF ANY KIND, either express or implied. See the License for the
+specific language governing permissions and limitations under the License.
+
+
+
```

### Comparing `Riffle-1.0.1/source/Riffle.egg-info/PKG-INFO` & `Riffle-2.0.0/source/Riffle.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,58 @@
-Metadata-Version: 2.1
-Name: Riffle
-Version: 1.0.1
-Summary: Filesystem browser for PySide.
-Home-page: https://gitlab.com/4degrees/riffle
-Author: Martin Pengelly-Phillips
-Author-email: martin@4degrees.ltd.uk
-License: Apache License (2.0)
-Description: ######
-        Riffle
-        ######
-        
-        A filesystem browser for PySide.
-        
-        *************
-        Documentation
-        *************
-        
-        Full documentation can be found at http://riffle.readthedocs.org
-        
-        *************
-        Issue tracker
-        *************
-        
-        Found a bug? Have an idea on how to make the tool better?
-        
-        Post it at https://gitlab.com/4degrees/riffle/issues
-        
-        *********************
-        Copyright and license
-        *********************
-        
-        Copyright (c) 2014 Martin Pengelly-Phillips
-        
-        Licensed under the Apache License, Version 2.0 (the "License"); you may not use
-        this work except in compliance with the License. You may obtain a copy of the
-        License in the LICENSE.txt file, or at:
-        
-        http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software distributed
-        under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
-        CONDITIONS OF ANY KIND, either express or implied. See the License for the
-        specific language governing permissions and limitations under the License.
-        
-        
-Keywords: filesystem,browser,pyside,qt,pyqt
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.0, <4.0
-Provides-Extra: setup
-Provides-Extra: tests
-Provides-Extra: dev
+Metadata-Version: 2.1
+Name: Riffle
+Version: 2.0.0
+Summary: Filesystem browser for PySide.
+Home-page: https://gitlab.com/4degrees/riffle
+Author: Martin Pengelly-Phillips
+Author-email: martin@4degrees.ltd.uk
+License: Apache License (2.0)
+Keywords: filesystem,browser,pyside,qt,pyqt
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8, <3.13
+Provides-Extra: setup
+Provides-Extra: tests
+Provides-Extra: dev
+License-File: LICENSE.txt
+
+######
+Riffle
+######
+
+A filesystem browser for PySide.
+
+*************
+Documentation
+*************
+
+Full documentation can be found at http://riffle.readthedocs.org
+
+*************
+Issue tracker
+*************
+
+Found a bug? Have an idea on how to make the tool better?
+
+Post it at https://gitlab.com/4degrees/riffle/issues
+
+*********************
+Copyright and license
+*********************
+
+Copyright (c) 2014 Martin Pengelly-Phillips
+
+Licensed under the Apache License, Version 2.0 (the "License"); you may not use
+this work except in compliance with the License. You may obtain a copy of the
+License in the LICENSE.txt file, or at:
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software distributed
+under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
+CONDITIONS OF ANY KIND, either express or implied. See the License for the
+specific language governing permissions and limitations under the License.
+
+
+
```

### Comparing `Riffle-1.0.1/source/Riffle.egg-info/SOURCES.txt` & `Riffle-2.0.0/source/Riffle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Riffle-1.0.1/source/riffle/browser.py` & `Riffle-2.0.0/source/riffle/browser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,283 +1,284 @@
-# :coding: utf-8
-# :copyright: Copyright (c) 2014 Martin Pengelly-Phillips
-# :license: See LICENSE.txt.
-
-from datetime import datetime
-import os
-
-from PySide2 import QtWidgets, QtGui, QtCore
-
-import riffle.resource
-import riffle.model
-import riffle.icon_factory
-
-
-class FilesystemBrowser(QtWidgets.QDialog):
-    '''FilesystemBrowser dialog.'''
-
-    def __init__(self, root='', parent=None, iconFactory=None):
-        '''Initialise browser with *root* path.
-
-        Use an empty *root* path to specify the computer.
-
-        *parent* is the optional owner of this UI element.
-
-        *iconFactory* specifies the optional factory to pass to the model for
-        customising icons.
-
-        '''
-        super(FilesystemBrowser, self).__init__(parent=parent)
-        self._root = root
-        self._iconFactory = iconFactory
-        self._selected = []
-        self._construct()
-        self._postConstruction()
-
-    def _construct(self):
-        '''Construct widget.'''
-        self.setLayout(QtWidgets.QVBoxLayout())
-
-        self._headerLayout = QtWidgets.QHBoxLayout()
-
-        self._locationWidget = QtWidgets.QComboBox()
-        self._headerLayout.addWidget(self._locationWidget, stretch=1)
-
-        self._upButton = QtWidgets.QToolButton()
-        self._upButton.setIcon(QtGui.QIcon(':riffle/icon/up'))
-        self._headerLayout.addWidget(self._upButton)
-
-        self.layout().addLayout(self._headerLayout)
-
-        self._contentSplitter = QtWidgets.QSplitter()
-
-        self._bookmarksWidget = QtWidgets.QListView()
-        self._contentSplitter.addWidget(self._bookmarksWidget)
-
-        self._filesystemWidget = QtWidgets.QTableView()
-        self._filesystemWidget.setSelectionBehavior(
-            self._filesystemWidget.SelectRows
-        )
-        self._filesystemWidget.setSelectionMode(
-            self._filesystemWidget.SingleSelection
-        )
-        self._filesystemWidget.verticalHeader().hide()
-
-        self._contentSplitter.addWidget(self._filesystemWidget)
-
-        proxy = riffle.model.FilesystemSortProxy(self)
-        model = riffle.model.Filesystem(
-            path=self._root, parent=self, iconFactory=self._iconFactory
-        )
-        proxy.setSourceModel(model)
-        proxy.setDynamicSortFilter(True)
-
-        self._filesystemWidget.setModel(proxy)
-        self._filesystemWidget.setSortingEnabled(True)
-        # Apply delegate to "Date Modified" column
-        delegate = DateDelegate(self._filesystemWidget)
-        self._filesystemWidget.setItemDelegateForColumn(3, delegate)
-
-        self._contentSplitter.setStretchFactor(1, 1)
-        self.layout().addWidget(self._contentSplitter)
-
-        self._footerLayout = QtWidgets.QHBoxLayout()
-        self._footerLayout.addStretch(1)
-
-        self._cancelButton = QtWidgets.QPushButton('Cancel')
-        self._footerLayout.addWidget(self._cancelButton)
-
-        self._acceptButton = QtWidgets.QPushButton('Choose')
-        self._footerLayout.addWidget(self._acceptButton)
-
-        self.layout().addLayout(self._footerLayout)
-
-    def _postConstruction(self):
-        '''Perform post-construction operations.'''
-        self.setWindowTitle('Filesystem Browser')
-        self._filesystemWidget.sortByColumn(0, QtCore.Qt.AscendingOrder)
-
-        # TODO: Remove once bookmarks widget implemented.
-        self._bookmarksWidget.hide()
-
-        self._acceptButton.setDefault(True)
-        self._acceptButton.setDisabled(True)
-
-        self._acceptButton.clicked.connect(self.accept)
-        self._cancelButton.clicked.connect(self.reject)
-
-        self._configureShortcuts()
-
-        self.setLocation(self._root)
-
-        self._filesystemWidget.horizontalHeader().setSectionResizeMode(
-            0,
-            QtWidgets.QHeaderView.ResizeToContents
-        )
-        self._filesystemWidget.horizontalHeader().setSectionResizeMode(
-            0,
-            QtWidgets.QHeaderView.Stretch
-        )
-
-        self._upButton.clicked.connect(self._onNavigateUpButtonClicked)
-        self._locationWidget.currentIndexChanged.connect(
-            self._onNavigate
-        )
-
-        self._filesystemWidget.activated.connect(self._onActivateItem)
-        selectionModel = self._filesystemWidget.selectionModel()
-        selectionModel.currentRowChanged.connect(self._onSelectItem)
-
-    def _configureShortcuts(self):
-        '''Add keyboard shortcuts to navigate the filesystem.'''
-        self._upShortcut = QtWidgets.QShortcut(
-            QtGui.QKeySequence('Backspace'), self
-        )
-        self._upShortcut.setAutoRepeat(False)
-        self._upShortcut.activated.connect(self._onNavigateUpButtonClicked)
-
-    def _onActivateItem(self, index):
-        '''Handle activation of item in listing.'''
-        item = self._filesystemWidget.model().item(index)
-        if not isinstance(item, riffle.model.File):
-            self._acceptButton.setDisabled(True)
-            self.setLocation(item.path, interactive=True)
-
-    def _onSelectItem(self, selection, previousSelection):
-        '''Handle selection of item in listing.'''
-        self._acceptButton.setEnabled(True)
-        del self._selected[:]
-        item = self._filesystemWidget.model().item(selection)
-        self._selected.append(item.path)
-
-    def _onNavigate(self, index):
-        '''Handle selection of path segment.'''
-        if index > 0:
-            self.setLocation(
-                self._locationWidget.itemData(index), interactive=True
-            )
-
-    def _onNavigateUpButtonClicked(self):
-        '''Navigate up a directory on button click.'''
-        index = self._locationWidget.currentIndex()
-        self._onNavigate(index + 1)
-
-    def _segmentPath(self, path):
-        '''Return list of valid *path* segments.'''
-        parts = []
-        model = self._filesystemWidget.model()
-
-        # Separate root path from remainder.
-        remainder = path
-
-        while True:
-            if remainder == model.root.path:
-                break
-
-            if remainder:
-                parts.append(remainder)
-
-            head, tail = os.path.split(remainder)
-            if head == remainder:
-                break
-
-            remainder = head
-
-        parts.append(model.root.path)
-        return parts
-
-    def setLocation(self, path, interactive=False):
-        '''Set current location to *path*.
-
-        *path* must be the same as root or under the root.
-
-        .. note::
-
-            Comparisons are case-sensitive. If you set the root as 'D:/' then
-            location can be set as 'D:/folder' *not* 'd:/folder'.
-
-        If *interactive* is True, catch any exception occurring and display an
-        appropriate warning dialog to the user. Otherwise allow exceptions to
-        bubble up as normal.
-
-        '''
-        try:
-            self._setLocation(path)
-        except Exception as error:
-            if not interactive:
-                raise
-            else:
-                warning_dialog = QtWidgets.QMessageBox(
-                    QtWidgets.QMessageBox.Warning,
-                    'Location is not available',
-                    '{0} is not accessible.'.format(path),
-                    QtWidgets.QMessageBox.Ok,
-                    self
-                )
-                warning_dialog.setDetailedText(str(error))
-                warning_dialog.exec_()
-
-    def _setLocation(self, path):
-        '''Set current location to *path*.
-
-        *path* must be the same as root or under the root.
-
-        .. note::
-
-            Comparisons are case-sensitive. If you set the root as 'D:/' then
-            location can be set as 'D:/folder' *not* 'd:/folder'.
-
-        '''
-        model = self._filesystemWidget.model()
-
-        if not path.startswith(model.root.path):
-            raise ValueError('Location must be root or under root.')
-
-        # Ensure children for each segment in path are loaded.
-        segments = self._segmentPath(path)
-        for segment in reversed(segments):
-            pathIndex = model.pathIndex(segment)
-            model.fetchMore(pathIndex)
-
-        self._filesystemWidget.setRootIndex(model.pathIndex(path))
-        self._locationWidget.clear()
-
-        # Add history entry for each segment.
-        for segment in segments:
-            index = model.pathIndex(segment)
-            if not index.isValid():
-                # Root item.
-                icon = model.iconFactory.icon(
-                    riffle.icon_factory.IconType.Computer
-                )
-                self._locationWidget.addItem(
-                    icon, model.root.path or model.root.name, model.root.path
-                )
-            else:
-                icon = model.icon(index)
-                self._locationWidget.addItem(icon, segment, segment)
-
-        if self._locationWidget.count() > 1:
-            self._upButton.setEnabled(True)
-            self._upShortcut.setEnabled(True)
-        else:
-            self._upButton.setEnabled(False)
-            self._upShortcut.setEnabled(False)
-
-    def selected(self):
-        '''Return selected paths.'''
-        return self._selected[:]
-
-
-class DateDelegate(QtWidgets.QStyledItemDelegate):
-    '''Simple QStyledItemDelegate to format timestamps.'''
-
-    def displayText(self, value, locale):
-        '''Converts float timestamp *value* to a string representation.
-
-        All other datatypes will pass through unmodified.
-        '''
-
-        # Some items (e.g. collections) will be set to None, so skip those
-        if isinstance(value, float):
-            return datetime.fromtimestamp(value).strftime('%c')
-        return value
+# :coding: utf-8
+# :copyright: Copyright (c) 2014 Martin Pengelly-Phillips
+# :license: See LICENSE.txt.
+
+from datetime import datetime
+import os
+
+from PySide6 import QtWidgets, QtCore, QtGui
+from PySide6.QtGui import QShortcut
+
+import riffle.resource
+import riffle.model
+import riffle.icon_factory
+
+
+class FilesystemBrowser(QtWidgets.QDialog):
+    '''FilesystemBrowser dialog.'''
+
+    def __init__(self, root='', parent=None, iconFactory=None):
+        '''Initialise browser with *root* path.
+
+        Use an empty *root* path to specify the computer.
+
+        *parent* is the optional owner of this UI element.
+
+        *iconFactory* specifies the optional factory to pass to the model for
+        customising icons.
+
+        '''
+        super(FilesystemBrowser, self).__init__(parent=parent)
+        self._root = root
+        self._iconFactory = iconFactory
+        self._selected = []
+        self._construct()
+        self._postConstruction()
+
+    def _construct(self):
+        '''Construct widget.'''
+        self.setLayout(QtWidgets.QVBoxLayout())
+
+        self._headerLayout = QtWidgets.QHBoxLayout()
+
+        self._locationWidget = QtWidgets.QComboBox()
+        self._headerLayout.addWidget(self._locationWidget, stretch=1)
+
+        self._upButton = QtWidgets.QToolButton()
+        self._upButton.setIcon(QtGui.QIcon(':riffle/icon/up'))
+        self._headerLayout.addWidget(self._upButton)
+
+        self.layout().addLayout(self._headerLayout)
+
+        self._contentSplitter = QtWidgets.QSplitter()
+
+        self._bookmarksWidget = QtWidgets.QListView()
+        self._contentSplitter.addWidget(self._bookmarksWidget)
+
+        self._filesystemWidget = QtWidgets.QTableView()
+        self._filesystemWidget.setSelectionBehavior(
+            self._filesystemWidget.SelectionBehavior.SelectRows
+        )
+        self._filesystemWidget.setSelectionMode(
+            self._filesystemWidget.SelectionMode.SingleSelection
+        )
+        self._filesystemWidget.verticalHeader().hide()
+
+        self._contentSplitter.addWidget(self._filesystemWidget)
+
+        proxy = riffle.model.FilesystemSortProxy(self)
+        model = riffle.model.Filesystem(
+            path=self._root, parent=self, iconFactory=self._iconFactory
+        )
+        proxy.setSourceModel(model)
+        proxy.setDynamicSortFilter(True)
+
+        self._filesystemWidget.setModel(proxy)
+        self._filesystemWidget.setSortingEnabled(True)
+        # Apply delegate to "Date Modified" column
+        delegate = DateDelegate(self._filesystemWidget)
+        self._filesystemWidget.setItemDelegateForColumn(3, delegate)
+
+        self._contentSplitter.setStretchFactor(1, 1)
+        self.layout().addWidget(self._contentSplitter)
+
+        self._footerLayout = QtWidgets.QHBoxLayout()
+        self._footerLayout.addStretch(1)
+
+        self._cancelButton = QtWidgets.QPushButton('Cancel')
+        self._footerLayout.addWidget(self._cancelButton)
+
+        self._acceptButton = QtWidgets.QPushButton('Choose')
+        self._footerLayout.addWidget(self._acceptButton)
+
+        self.layout().addLayout(self._footerLayout)
+
+    def _postConstruction(self):
+        '''Perform post-construction operations.'''
+        self.setWindowTitle('Filesystem Browser')
+        self._filesystemWidget.sortByColumn(0, QtCore.Qt.SortOrder.AscendingOrder)
+
+        # TODO: Remove once bookmarks widget implemented.
+        self._bookmarksWidget.hide()
+
+        self._acceptButton.setDefault(True)
+        self._acceptButton.setDisabled(True)
+
+        self._acceptButton.clicked.connect(self.accept)
+        self._cancelButton.clicked.connect(self.reject)
+
+        self._configureShortcuts()
+
+        self.setLocation(self._root)
+
+        self._filesystemWidget.horizontalHeader().setSectionResizeMode(
+            0,
+            QtWidgets.QHeaderView.ResizeMode.ResizeToContents
+        )
+        self._filesystemWidget.horizontalHeader().setSectionResizeMode(
+            0,
+            QtWidgets.QHeaderView.ResizeMode.Stretch
+        )
+
+        self._upButton.clicked.connect(self._onNavigateUpButtonClicked)
+        self._locationWidget.currentIndexChanged.connect(
+            self._onNavigate
+        )
+
+        self._filesystemWidget.activated.connect(self._onActivateItem)
+        selectionModel = self._filesystemWidget.selectionModel()
+        selectionModel.currentRowChanged.connect(self._onSelectItem)
+
+    def _configureShortcuts(self):
+        '''Add keyboard shortcuts to navigate the filesystem.'''
+        self._upShortcut = QShortcut(
+            QtGui.QKeySequence('Backspace'), self
+        )
+        self._upShortcut.setAutoRepeat(False)
+        self._upShortcut.activated.connect(self._onNavigateUpButtonClicked)
+
+    def _onActivateItem(self, index):
+        '''Handle activation of item in listing.'''
+        item = self._filesystemWidget.model().item(index)
+        if not isinstance(item, riffle.model.File):
+            self._acceptButton.setDisabled(True)
+            self.setLocation(item.path, interactive=True)
+
+    def _onSelectItem(self, selection, previousSelection):
+        '''Handle selection of item in listing.'''
+        self._acceptButton.setEnabled(True)
+        del self._selected[:]
+        item = self._filesystemWidget.model().item(selection)
+        self._selected.append(item.path)
+
+    def _onNavigate(self, index):
+        '''Handle selection of path segment.'''
+        if index > 0:
+            self.setLocation(
+                self._locationWidget.itemData(index), interactive=True
+            )
+
+    def _onNavigateUpButtonClicked(self):
+        '''Navigate up a directory on button click.'''
+        index = self._locationWidget.currentIndex()
+        self._onNavigate(index + 1)
+
+    def _segmentPath(self, path):
+        '''Return list of valid *path* segments.'''
+        parts = []
+        model = self._filesystemWidget.model()
+
+        # Separate root path from remainder.
+        remainder = path
+
+        while True:
+            if remainder == model.root.path:
+                break
+
+            if remainder:
+                parts.append(remainder)
+
+            head, tail = os.path.split(remainder)
+            if head == remainder:
+                break
+
+            remainder = head
+
+        parts.append(model.root.path)
+        return parts
+
+    def setLocation(self, path, interactive=False):
+        '''Set current location to *path*.
+
+        *path* must be the same as root or under the root.
+
+        .. note::
+
+            Comparisons are case-sensitive. If you set the root as 'D:/' then
+            location can be set as 'D:/folder' *not* 'd:/folder'.
+
+        If *interactive* is True, catch any exception occurring and display an
+        appropriate warning dialog to the user. Otherwise allow exceptions to
+        bubble up as normal.
+
+        '''
+        try:
+            self._setLocation(path)
+        except Exception as error:
+            if not interactive:
+                raise
+            else:
+                warning_dialog = QtWidgets.QMessageBox(
+                    QtWidgets.QMessageBox.Icon.Warning,
+                    'Location is not available',
+                    '{0} is not accessible.'.format(path),
+                    QtWidgets.QMessageBox.StandardButton.Ok,
+                    self
+                )
+                warning_dialog.setDetailedText(str(error))
+                warning_dialog.exec_()
+
+    def _setLocation(self, path):
+        '''Set current location to *path*.
+
+        *path* must be the same as root or under the root.
+
+        .. note::
+
+            Comparisons are case-sensitive. If you set the root as 'D:/' then
+            location can be set as 'D:/folder' *not* 'd:/folder'.
+
+        '''
+        model = self._filesystemWidget.model()
+
+        if not path.startswith(model.root.path):
+            raise ValueError('Location must be root or under root.')
+
+        # Ensure children for each segment in path are loaded.
+        segments = self._segmentPath(path)
+        for segment in reversed(segments):
+            pathIndex = model.pathIndex(segment)
+            model.fetchMore(pathIndex)
+
+        self._filesystemWidget.setRootIndex(model.pathIndex(path))
+        self._locationWidget.clear()
+
+        # Add history entry for each segment.
+        for segment in segments:
+            index = model.pathIndex(segment)
+            if not index.isValid():
+                # Root item.
+                icon = model.iconFactory.icon(
+                    riffle.icon_factory.IconType.Computer
+                )
+                self._locationWidget.addItem(
+                    icon, model.root.path or model.root.name, model.root.path
+                )
+            else:
+                icon = model.icon(index)
+                self._locationWidget.addItem(icon, segment, segment)
+
+        if self._locationWidget.count() > 1:
+            self._upButton.setEnabled(True)
+            self._upShortcut.setEnabled(True)
+        else:
+            self._upButton.setEnabled(False)
+            self._upShortcut.setEnabled(False)
+
+    def selected(self):
+        '''Return selected paths.'''
+        return self._selected[:]
+
+
+class DateDelegate(QtWidgets.QStyledItemDelegate):
+    '''Simple QStyledItemDelegate to format timestamps.'''
+
+    def displayText(self, value, locale):
+        '''Converts float timestamp *value* to a string representation.
+
+        All other datatypes will pass through unmodified.
+        '''
+
+        # Some items (e.g. collections) will be set to None, so skip those
+        if isinstance(value, float):
+            return datetime.fromtimestamp(value).strftime('%c')
+        return value
```

### Comparing `Riffle-1.0.1/source/riffle/icon_factory.py` & `Riffle-2.0.0/source/riffle/icon_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-# :coding: utf-8
-# :copyright: Copyright (c) 2014 Martin Pengelly-Phillips
-# :license: See LICENSE.txt.
-
-
-from PySide2 import QtWidgets, QtGui, QtCore
-
-import riffle.model
-
-
-class IconType(object):
-    '''Icon types.'''
-
-    Computer = 'Computer',
-    File = 'File',
-    Directory = 'Directory',
-    Mount = 'Mount',
-    Collection = 'Collection'
-    Unknown = 'Unknown'
-
-
-class IconFactory(object):
-    '''Icon provider.'''
-
-    def icon(self, specification):
-        '''Return appropriate icon for *specification*.
-
-        *specification* should be either:
-
-            * An instance of :py:class:`riffle.model.Item`
-            * One of the defined icon types (:py:class:`IconType`)
-
-        '''
-        if isinstance(specification, riffle.model.Item):
-            specification = self.type(specification)
-
-        icon = None
-
-        if specification == IconType.Computer:
-            icon = QtGui.QIcon(':riffle/icon/computer')
-
-        elif specification == IconType.Mount:
-            icon = QtGui.QIcon(':riffle/icon/drive')
-
-        elif specification == IconType.Directory:
-            icon = QtGui.QIcon(':riffle/icon/folder')
-
-        elif specification == IconType.File:
-            icon = QtGui.QIcon(':riffle/icon/file')
-
-        elif specification == IconType.Collection:
-            icon = QtGui.QIcon(':riffle/icon/collection')
-
-        return icon
-
-    def type(self, item):
-        '''Return appropriate icon type for *item*.'''
-        iconType = IconType.Unknown
-
-        if isinstance(item, riffle.model.Computer):
-            iconType = IconType.Computer
-
-        elif isinstance(item, riffle.model.Mount):
-            iconType = IconType.Mount
-
-        elif isinstance(item, riffle.model.Directory):
-            iconType = IconType.Directory
-
-        elif isinstance(item, riffle.model.File):
-            iconType = IconType.File
-
-        elif isinstance(item, riffle.model.Collection):
-            iconType = IconType.Collection
-
-        return iconType
+# :coding: utf-8
+# :copyright: Copyright (c) 2014 Martin Pengelly-Phillips
+# :license: See LICENSE.txt.
+
+
+from PySide6 import QtGui
+
+import riffle.model
+
+
+class IconType(object):
+    '''Icon types.'''
+
+    Computer = 'Computer',
+    File = 'File',
+    Directory = 'Directory',
+    Mount = 'Mount',
+    Collection = 'Collection'
+    Unknown = 'Unknown'
+
+
+class IconFactory(object):
+    '''Icon provider.'''
+
+    def icon(self, specification):
+        '''Return appropriate icon for *specification*.
+
+        *specification* should be either:
+
+            * An instance of :py:class:`riffle.model.Item`
+            * One of the defined icon types (:py:class:`IconType`)
+
+        '''
+        if isinstance(specification, riffle.model.Item):
+            specification = self.type(specification)
+
+        icon = None
+
+        if specification == IconType.Computer:
+            icon = QtGui.QIcon(':riffle/icon/computer')
+
+        elif specification == IconType.Mount:
+            icon = QtGui.QIcon(':riffle/icon/drive')
+
+        elif specification == IconType.Directory:
+            icon = QtGui.QIcon(':riffle/icon/folder')
+
+        elif specification == IconType.File:
+            icon = QtGui.QIcon(':riffle/icon/file')
+
+        elif specification == IconType.Collection:
+            icon = QtGui.QIcon(':riffle/icon/collection')
+
+        return icon
+
+    def type(self, item):
+        '''Return appropriate icon type for *item*.'''
+        iconType = IconType.Unknown
+
+        if isinstance(item, riffle.model.Computer):
+            iconType = IconType.Computer
+
+        elif isinstance(item, riffle.model.Mount):
+            iconType = IconType.Mount
+
+        elif isinstance(item, riffle.model.Directory):
+            iconType = IconType.Directory
+
+        elif isinstance(item, riffle.model.File):
+            iconType = IconType.File
+
+        elif isinstance(item, riffle.model.Collection):
+            iconType = IconType.Collection
+
+        return iconType
```

### Comparing `Riffle-1.0.1/source/riffle/resource.py` & `Riffle-2.0.0/source/riffle/resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,287 +1,287 @@
-# Resource object code (Python 3)
-# Created by: object code
-# Created by: The Resource Compiler for Qt version 5.14.1
-# WARNING! All changes made in this file will be lost!
-
-from PySide2 import QtCore
-
-qt_resource_data = b"\
-\x00\x00\x014\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
-\x00\x00\x00\xfbIDATX\x85\xed\x96Q\x11\x830\
-\x10DW\x02\x12\x22\x01\x09\x95\x10\x09\x91\x80\x04\x1cT\
-B$ \x01\x09H\x88\x04$\xd0\x8f\x90!\xa5\x5cH\
-\xd2\xbb|\xb13\xfb\xc5\x0c\xfb\x80\xbd\x0b\xc0\xa3Gy\
-\xea+\xac\xb8\x82\x17\x00[\xa5\xdd~\x8f*u\x7f\x86\
-\x07\xaf\xb5\x00\x9a!<\xd8\xd4\x00\xcc\x8c\x00\xae4\xbc\
-g\x0c\x0f.\xea\x82\x15\x00\xb0\xb9\xe1\x1d|q\xb8\x01\
-6d\x8e\xe6(\x14\xbe\x01\x18r\x008F\x8f\xf2\xed\
-Hr\x8e\x1ee\x93\x02\x98\x1a\x00,T\xb8j\x10\x9e\
-,\xe3\xd8\x10\xc0^\x01\xb8\x86\x00?e\x94\xd8|w\
-~\xc5\x00\xe7\xf6;\xf8\xb2p\xfa\xbc\xdc\x0c\x05`\xe1\
-\xb7\xa1\x84\xe2)\xd3\xf1\x85\x8e\x22cV\xfc\xa0\xea|\
-1\xbc\xa2\xacuY\xa9\x01D\x09\x81\xe3\xfc\x9f\x04\x01\
-,\x12\xcb\xe8\x8d\x83N\x09\x84\xc7\xa7\xec\xe5\x1e\x88\xbf\
-\x8f\xdb\x81\x06&\x8f\xf8>\xe4\x0cE\xd8j\x09\x91\x7f\
-G\x1a\xbe\x0b\xdc; x\x86l\xc9\x1f\x95\xeb\x03w\
-\x86\xc7l\xd1\x8c;C\x00\x00\x00\x00IEND\xae\
-B`\x82\
-\x00\x00\x01\xf8\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
-\x00\x00\x01\xbfIDATX\x85\xd5\x97]\x91\xc30\
-\x0c\x84?\x08\x86\x10\x08\x81`\x08\x85P\x08\x85`\x06\
-\x81\x10\x08\x81P\x08\x85p\x10\x0c\xe1\xee!\xce\x8cb\
-K\x89\x9c\xf6\xe6\xe64\xe3'\xcb\xda\xd5J\xfe\x83\x7f\
-f\x01\x88\xc0\x03\x98\x80\xb9\x8cTF\xfc-\xe0\xb1\x00\
-~\x01\xdf\x8e1\x01\xc3'\x80C\x09\x96\x9d\xc0\x1a\x91\
-p\x15|\xc4\xce\xf8\x05,\x05 \xb1\x96\xe1i\xf8\xe6\
-\x12\xab\xcb\x22m\xd6\xb9\x80\x1d\x05\x0b\xac\xfd\xa1)\x16\
-\xbd\xe0\xa3\x12\xe0\x8a\x94I!q\xaaD`\x95Wf\
-}\xef\x04\x96\x16iU<L$U\x0b\xde\x01\xb7H\
-\xcc\x96\xe3\xc0^\xfa\xc9\x11\xdc[\x96\xa9\x221\x9c9\
-\x9dJ\xc5\xaa\x8e\x87$%\x96\xdcQ\xaa\x0a\xd2!\x9d\
-\x04\xdc\x1a\xd5\x94S\xb1;\xfb\x04\x9b\x80\xa7\x12U\xe0\
-\x87\xf5T,T\x18QN>\xc4\xc4\xcb\x09\xbe\x8d/\
-chI\xc8\xc3*\xc9\x89\xc4y\x97\x0e\xf8\xef\x02k\
-\xcf\xcb>\xdb\xe1\xccbBk\xac^p\x8b\x80Lt\
-\xb1\x08$ea\xa0\xffB\xd2\x08\xc8R?\xe5\x84\x94\
-fi\xd7\x01\xed9q\x85\x80\xa9t\x12\x13\xcd\x16\x11\
-V\xef\x96\x8c\xdd\x84\x1a\x81\xc5\x22\x10\xab\xc0\xc3\x01\x09\
-\xe9\xdb\xbb\x0d\xa5\x82\xb7\xdaA6\xd9\xe3$\xd8F\xa2\
-\x87\xc0\x8d\xbdr\xcdI;\xe3+\x83$\xe1%P\xdf\
-\xb2j\x9f\x0d\xec\xcb\x90\x9c\x81=\x96\xaa\xd8\xd1r\x9c\
-+\xc7\xa6N\x17\xec\xce\xbe\xf6\xd6.\x03\xda[\xeb]\
-\x12\xb1\x02\xcf8^\xcb\xf5V\xb3N\xc7#\xd3^\xd3\
-\x99\x8ed\xa2B\xc2\xf3<\x0b\x05\xa4V\xf1\xd2\xd3N\
-\xbb\xf9d\x1dg\xd6\xe6\xda~I/\xc3\xbf+s-\
-\xa3\xba1{\xc6\x93\x0f\xfd\x90\xc6\x0e\x22\xb9\x00w\x7f\
-F\xbcvc\xff\x1b\xda~H\x13k\xef\x5c\xfe\x8a\xfd\
-\x89\xfd\x00\x5c\x8fR,\xed\xd1\x07\x01\x00\x00\x00\x00I\
-END\xaeB`\x82\
-\x00\x00\x01\x06\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
-\x00\x00\x00\xcdIDATX\x85\xed\x95Q\x0d\xc3 \
-\x14E\x8f\x84I@\xc2$TB%T\xc2$\xe0\x00\
-\x09\x95P\x09H@B%TB\xf7\x01iH\xd3m\
-\xa4\x09\xdc&\xebM\x0e\xbf\x9c<\xf2.p\xe7b1\
-\x80\x03\xfc\x01\x13`k\x0b\x8c\xc0\xfa\x83\x00<k\x09\
-\xcc\x05\x02+\xb0\x00C\x0d\x81\x92\xcbs<qj\xae\
-\x10\xcb\x97\xe9\x99\x13\x02g\xe9\x8f\x04\xba\x86\x02\xd3\xa7\
-)\xfcg^\x1c\xef}m\xb6^)]\xbd\x1a,\xa4\
-C%\xb0Bl6\xd5\xe5\x81\xf4\x1e*\x01\x0f\xb1\xa1\
-T\x02\xa3Z\xc0A\x5cC\x95\x80\x85\xd8\xcb*\x81\x01\
-\xda\xfe\x01{zh\xfb\x0b\xee\xe9\x00\x1eB\x01C\x8a\
-\xaa\x0d\xb7(\x04\xe6\x5c@Q\xc7!\x17\xf0\x02\x01\x9f\
-\x0b(\xda\xd0\xe5\x02&\x19\x85Fx\xd2\x0a\xde\x91\xe7\
-\x0dk\x8ey`\x16\x09pi\x00\x00\x00\x00IEN\
-D\xaeB`\x82\
-\x00\x00\x00\xf1\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
-\x00\x00\x00\xb8IDATX\x85\xed\x97Q\x0d\x830\
-\x14E\x8f\x04$ a\x12&\xa1\x12&\x01\x09u\x80\
-\x04$L\x02\x12*\xa1\x12*a\xfb(M\xba\x97.\
-K\x0a<\xf6\xf1nr?\xe8\xcf9\xf4A\xd2\xc2\x9f\
-ePh33\x90\x80\x97R\x13\xe0\x0b|R\x04\xcb\
-N\x00\xb1Z\x08\x0a\xady\x09at\xff6\xa3\x03s\
-\x13L\x130\x01\x130\x01\x130\x01\x130\x81\x8f\x87\
-\x85|L:\xb3^\x0aD\xb1\xa0\xd9\x08\xd7\x1eJ}\
-\x99\xcb\xf3\x02\xf8\x8a\xb8'8\xf2\xfd \x9c\x08\x0d\xdb\
-\xcb:\x09o\xc5\x91\xc7\xb3tJ\x15\x98'\x7f\xf9?\
-\x81\xad\x0c\xe4_\xb3G`\x05\x1e=\xd0\x1a~\xc48\
-\x020\xee\x11\x19w\xb6k\xeb\xd5\xf2\x06\xc9:~b\
-*a\x8b\xe0\x00\x00\x00\x00IEND\xaeB`\x82\
-\
-\x00\x00\x01\xf1\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
-\x00\x00\x01\xb8IDATX\x85\xd5Wm\x91\xc5 \
-\x0c\x5c\x09H@B% \xe1I\xa8\x84J\xc0A%\
- \xa1\x12*\xa1\x12NB%\xbc\xfb\x01\xdc\x844@\
-\xe8\xeb\xcd\xcde\x86_\x84\xecf\x13\xbe\x80\x7ff\x06\
-\x80\x03\xb0\x00X\x01\x844|\x1a\xee\xb7\x80\xa7\x04\xf8\
-\x05\xe0\xad\x18+\x00\xfb\x04\xb0I\xc1N%\xb0D\xc4\
-\xdc\x05\x9fP\xcf\xf8\x00\xb0%\x00\x8fX\x86\xbd\xe2{\
-\xa6XC\xe6p\xcd\xfaL`\xad`\x06\xb1?$\xc5\
-\x9c\x16|\x12\x02\xdc\x91\xd2\x0b$\xbaJ\x18Dyi\
-\xd6\xf3 05\x87\xab\x8a\xcdD<[\xf0\x09x\x8d\
-D\xa89Z\x94\xd2\xafJ\x00MiVF\xc2\xf6\x9c\
-\xbaR\xb1u/\x05I\xba\xa3D\x15\xa8\x83W\x82g\
-\x02\x9a.\x9fQ&X\xd8\x04\x85D\x1d\x02=\x12\x86\
-a\x14\xbe\x0b\x998\x84\xc5\x16Q!i\xd0\xbe\xe9\x1d\
-:\xf4\xb0\xf2t\xc2\xa3]\x1f\xcb\xd8\xb7F\x8b\x04U\
-\xab\xc0\x09dB\xea\xfe\x11\x02\x99\x84\x15\xe2\xd0D\xb7\
-\x1a\x01\xff\x10\x01I\x05Z\xea\x9dNPi\xb6\xeb\xba\
-\xe1\x128!\x06O\xb4P\xda\xb3\x00\xdc\xf2>\xd64\
-a\xebL\xd8j\x04\x1c\xcb\xc26\x82p\xcb\xea\xf5\xc0\
-\x0d#{\xf1\xa5\x07\xd12H\xa0\x07\x8e4\xdf<i\
-\x03\xdaeh\x11\x98;>\xfc\x96\x95\xfa\xec\xd2h^\
-I\xc0*|<\x8b\xedj\x8e\x819\xf6d\xd5\xd8\x8c\
-\xb2\xf6b\xf6\xd9\xf8\xad\xf5)\x09\x87\xeb.\xb1\xbdE\
-\xfcb\xaa\x9d\x8e-\x93^\xd3\x9aF\xfd1'\x90\xd0\
-<\xcfL\x02\xe1*\xdez\xdaI\x8fSZ\xc7\x80\xd8\
-\x5c\xf9\x97tT\xfc\x872\x972\xe2\x8d92v<\
-\xf4C\x9a\x06\x88\x9c\x09x\xf83\xa2\xb5\x17\xca\xdfP\
-\xfe!\xad\x88\xbds\xfb+\xf6'\xf6\x0d\xaeFRL\
-\x5c\x1b\x18x\x00\x00\x00\x00IEND\xaeB`\x82\
-\
-\x00\x00\x00\xc1\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
-\x00\x00\x00\x88IDATX\x85\xed\xd0A\x0d\xc0 \
-\x10D\xd1/\xa1\x12\x90\x80\x04$ \xa1\x12\xea\xb0\x12\
-\x90\x80\x04$\xb4\x87\xa6\x09\xe1\x04]\xd2\xb4\xc9L2\
-\xc7\xdd}Y\xf8p\x16 \x00\xab\xb1\xe1\xc9q\x0fd\
-\xe0\x98\xd42\x0aI\x13\x8f\xd7\x88\xae\xb8f0\x19[\
-\xefr=\x00\xdf\x0cYS\xef\x0a\x02\x08 \x80\x00\x02\
-\x08 \x80\x00\x02\x08\xf0\x0b\xc0\xd2\x0c\xed\xc6\xd6\xbb\x5c\
-\xaf:7\x833\x9a{\x8f\xc3\xf5\xaa2\xf1x\x01\xe2\
-\x08\xe0N\x046c#\x03\xaf\x7f='\x7fv\x14\x9c\
-N\x18\xe9\xb6\x00\x00\x00\x00IEND\xaeB`\x82\
-\
-\x00\x00\x01\x90\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
-\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
-\xa7\x93\x00\x00\x00\x09pHYs\x00\x00\x0b\x13\x00\x00\
-\x0b\x13\x01\x00\x9a\x9c\x18\x00\x00\x00\x07tIME\x07\
-\xde\x06\x12\x07)\x0f@\x06)\xb4\x00\x00\x01\x1dID\
-ATX\xc3\xed\xd7=J\xc4P\x10\xc0\xf1\x9f\xdf\x82\
-\x16\x82`!*+(\x1669\xc2z\x02=\x80\xe0\
-\x1d\x16\x0f\x22\xd8\xdax\x01\xaf\xa0\xa5\x8d\xb8\x16v\xc2\
-\xae\x88X\xa9\xd8\x0a\xa2\xcd[xD\x5c7\xe4i\x9a\
-70\x90L\xded\xfeo&\x99\xc7\xd0\xb0\x8c\x0dy\
-\xb6\x80\x02\xad\x9a1\xfa\xb8\xa8\xeaT\xa0\x87\xcfD\xfa\
-\x8av\x15\x80\xeb\x84\xc1c\x88\x91J\xd0\x0a\xbb\x1fH\
-\xb7f\x09\x8a\xe8z=\x94\xe4W\x87\x98\xbc\xae\xc4\xef\
-\xfaV\x86\xf1\xa6\xff\x82\x0c\x90\x012@\x15\x80\xd9\xa0\
-q\x13\x9b\xc7Td\x9b\xc0\xdc_\x00\xac\xe2\x08\xc7X\
-\x0e\xb6]\x9c\xe2\x103!x'\xd8v\xea\xb6\xcer\
-'\xdc\x8f\xee\x0f0\x8d3|\xe0\x01[X\xc1sX\
-s\x92\xba\x13\xde\x86\x03\xea\x1ewx\xc7%\x1eq\x83\
-\x17\xbc\x05\xdb\x13\xaeRg\x00\xd6\xb0Q\xfa&\xb6\xb1\
-\x14\xd9\x16\xb1Y\xda\xd8\xd0\x0c\xe4\xc3(\x03d\x80\x0c\
-\xd08\xc0\xe4\x0f\x93L,\xe7\x09\xe3\xf5G]\x98r\
-*\x1ah\xaf\x0ai;L2)\xa7\xa2\xbd\xaa\xc3\xa9\
-\xe0\x94b8\xedVI\xff\xbf\xca\x17s\x0c\x90\x8c\x16\
-$\xacm\x00\x00\x00\x00IEND\xaeB`\x82\
-\x00\x00\x01\xec\
-\x89\
-PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
-\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
-\x00\x00\x01\xb3IDATX\x85\xd5WQ\x91\xc4 \
-\x0c}\x12\x90\x80\x84J@B%\xac\x84J\xc0A%\
-TB%TB%\xac\x04$\xec}\x94\xce\x85\x90\xb4\
-\xa1\xdb\xce\xcde&_\x84\xbc\x97\x90\x10\x00\xfe\x998\
-\x00\x01\xc0\x00`\x040e\x8dY\xc3S\xc0]\x06|\
-\x03\xf8\x18t\x04\xe0\xef\x00v\xd9Y2\x02KD\xdc\
-U\xf0\x0ez\xc4+\x809\x03Dl\xc7\xb0(\xb6)\
-\xfbj\x92\x80:\xea\x94\xc1\x8e\x9c9l\xf5!e,\
-X\xc1;\xc1\xc1\x95TF\x81\xc4i&\x1c\xb6\xf4\xd2\
-\xa8_\x8d\xc0T\x02\xea,\x1e\x06\x12\xd9\x86o\xc05\
-\x12\x93f\xe8Q\xa6~48w\xb0\xb5\xdb\xc8H\x88\
-{\xa8\xd1i\xaa\xf0\xdb%\x96*w(;J\xcc\x02\
-5\x88F\xf0\x96V{1\xfb\xca\xe1i\x8a\x88\xad\xd4\
-fg$\x1c\xb3\x0ftq \x0b\xeb\x81\x93\xa0\x80[\
-\xfb\x9d^V\x91.D\x9c\x9c\x8f\x11|\xd7^\xf1A\
-\xeb\xac\xc0\x99\xc8\x82T\xfd\x1e\xe5\xf4\xd3\xae\xdc\x89\xa8\
-\x17\xfc\xd0@g\x8d@T\xd8S\x91f\xc4\xdb\xb0\x8f\
-\x1e\xf5B\x17hj\xe6z\xdfm\x04\xd4LG\x94\xa9\
-|\x8a\xc0\xac\x11\x08\xcc\x99\x7f\x80\x80CY\xc4U\xa1\
-R\xa7\xc3\x03\x04z\x94Y\xaen\xda\x09\xf6ch%\
-\xc0\xa7\xacXg\x9e9\x8c\x07\x0e=\xb6[\x8f\xab&\
-\x91\xf9\x0e\x9a!\xefq\xedBi\x91\x17\xca\xb3?\xec\
-2>\xb5\xbe%\x11\x18x\x82a|\xf3\xc1\xa4\xdd\x8e\
-G\x22\xbd\xa6\x13\x1a\x82\x09\x02\x09\xcb\xf3\xcce\x10\x9e\
-\xc5KO;m\xec\xee\xe78a+\xae\xfd\x97\xb4*\
-\xf6M\x91K\x11i\xc3\xc7\xa2\x0bn\xfa!u\x0dD\
-R\x06n\xfe\x8cX\xa5G\xf9\x1b\xda\x7fH#\xb6\xda\
-\xb9\xfc\x15\xfb\x13\xf9\x01\xafRRL\xcb)\xf0z\x00\
-\x00\x00\x00IEND\xaeB`\x82\
-"
-
-qt_resource_name = b"\
-\x00\x06\
-\x07\x8f\xcd%\
-\x00r\
-\x00i\x00f\x00f\x00l\x00e\
-\x00\x04\
-\x00\x06\xfa^\
-\x00i\
-\x00c\x00o\x00n\
-\x00\x05\
-\x00k\x90\xc5\
-\x00d\
-\x00r\x00i\x00v\x00e\
-\x00\x08\
-\x08\xcd\x08#\
-\x00p\
-\x00r\x00e\x00v\x00i\x00o\x00u\x00s\
-\x00\x06\
-\x06\xd6*\xc2\
-\x00f\
-\x00o\x00l\x00d\x00e\x00r\
-\x00\x08\
-\x06G\xc7\x82\
-\x00c\
-\x00o\x00m\x00p\x00u\x00t\x00e\x00r\
-\x00\x04\
-\x00\x07L\xf4\
-\x00n\
-\x00e\x00x\x00t\
-\x00\x04\
-\x00\x06\xd0%\
-\x00f\
-\x00i\x00l\x00e\
-\x00\x0a\
-\x02\xb7\xe4>\
-\x00c\
-\x00o\x00l\x00l\x00e\x00c\x00t\x00i\x00o\x00n\
-\x00\x02\
-\x00\x00\x07\xc0\
-\x00u\
-\x00p\
-"
-
-qt_resource_struct = b"\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
-\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
-\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x12\x00\x02\x00\x00\x00\x08\x00\x00\x00\x03\
-\x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x09\x81\
-\x00\x00\x01u!\x07\x10\x5c\
-\x00\x00\x00|\x00\x00\x00\x00\x00\x01\x00\x00\x07(\
-\x00\x00\x01u!\x07\x10f\
-\x00\x00\x00n\x00\x00\x00\x00\x00\x01\x00\x00\x053\
-\x00\x00\x01u!\x07\x10W\
-\x00\x00\x00 \x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01u!\x07\x10k\
-\x00\x00\x00\x8a\x00\x00\x00\x00\x00\x01\x00\x00\x07\xed\
-\x00\x00\x01u!\x07\x10a\
-\x00\x00\x00X\x00\x00\x00\x00\x00\x01\x00\x00\x04>\
-\x00\x00\x01u!\x07\x10u\
-\x00\x00\x00F\x00\x00\x00\x00\x00\x01\x00\x00\x034\
-\x00\x00\x01u!\x07\x10p\
-\x00\x00\x000\x00\x00\x00\x00\x00\x01\x00\x00\x018\
-\x00\x00\x01u!\x07\x10Q\
-"
-
-def qInitResources():
-    QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
-
-def qCleanupResources():
-    QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
-
-qInitResources()
+# Resource object code (Python 3)
+# Created by: object code
+# Created by: The Resource Compiler for Qt version 6.7.0
+# WARNING! All changes made in this file will be lost!
+
+from PySide6 import QtCore
+
+qt_resource_data = b"\
+\x00\x00\x01\xf8\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
+\x00\x00\x01\xbfIDATX\x85\xd5\x97]\x91\xc30\
+\x0c\x84?\x08\x86\x10\x08\x81`\x08\x85P\x08\x85`\x06\
+\x81\x10\x08\x81P\x08\x85p\x10\x0c\xe1\xee!\xce\x8cb\
+K\x89\x9c\xf6\xe6\xe64\xe3'\xcb\xda\xd5J\xfe\x83\x7f\
+f\x01\x88\xc0\x03\x98\x80\xb9\x8cTF\xfc-\xe0\xb1\x00\
+~\x01\xdf\x8e1\x01\xc3'\x80C\x09\x96\x9d\xc0\x1a\x91\
+p\x15|\xc4\xce\xf8\x05,\x05 \xb1\x96\xe1i\xf8\xe6\
+\x12\xab\xcb\x22m\xd6\xb9\x80\x1d\x05\x0b\xac\xfd\xa1)\x16\
+\xbd\xe0\xa3\x12\xe0\x8a\x94I!q\xaaD`\x95Wf\
+}\xef\x04\x96\x16iU<L$U\x0b\xde\x01\xb7H\
+\xcc\x96\xe3\xc0^\xfa\xc9\x11\xdc[\x96\xa9\x221\x9c9\
+\x9dJ\xc5\xaa\x8e\x87$%\x96\xdcQ\xaa\x0a\xd2!\x9d\
+\x04\xdc\x1a\xd5\x94S\xb1;\xfb\x04\x9b\x80\xa7\x12U\xe0\
+\x87\xf5T,T\x18QN>\xc4\xc4\xcb\x09\xbe\x8d/\
+chI\xc8\xc3*\xc9\x89\xc4y\x97\x0e\xf8\xef\x02k\
+\xcf\xcb>\xdb\xe1\xccbBk\xac^p\x8b\x80Lt\
+\xb1\x08$ea\xa0\xffB\xd2\x08\xc8R?\xe5\x84\x94\
+fi\xd7\x01\xed9q\x85\x80\xa9t\x12\x13\xcd\x16\x11\
+V\xef\x96\x8c\xdd\x84\x1a\x81\xc5\x22\x10\xab\xc0\xc3\x01\x09\
+\xe9\xdb\xbb\x0d\xa5\x82\xb7\xdaA6\xd9\xe3$\xd8F\xa2\
+\x87\xc0\x8d\xbdr\xcdI;\xe3+\x83$\xe1%P\xdf\
+\xb2j\x9f\x0d\xec\xcb\x90\x9c\x81=\x96\xaa\xd8\xd1r\x9c\
++\xc7\xa6N\x17\xec\xce\xbe\xf6\xd6.\x03\xda[\xeb]\
+\x12\xb1\x02\xcf8^\xcb\xf5V\xb3N\xc7#\xd3^\xd3\
+\x99\x8ed\xa2B\xc2\xf3<\x0b\x05\xa4V\xf1\xd2\xd3N\
+\xbb\xf9d\x1dg\xd6\xe6\xda~I/\xc3\xbf+s-\
+\xa3\xba1{\xc6\x93\x0f\xfd\x90\xc6\x0e\x22\xb9\x00w\x7f\
+F\xbcvc\xff\x1b\xda~H\x13k\xef\x5c\xfe\x8a\xfd\
+\x89\xfd\x00\x5c\x8fR,\xed\xd1\x07\x01\x00\x00\x00\x00I\
+END\xaeB`\x82\
+\x00\x00\x01\xec\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
+\x00\x00\x01\xb3IDATX\x85\xd5WQ\x91\xc4 \
+\x0c}\x12\x90\x80\x84J@B%\xac\x84J\xc0A%\
+TB%TB%\xac\x04$\xec}\x94\xce\x85\x90\xb4\
+\xa1\xdb\xce\xcde&_\x84\xbc\x97\x90\x10\x00\xfe\x998\
+\x00\x01\xc0\x00`\x040e\x8dY\xc3S\xc0]\x06|\
+\x03\xf8\x18t\x04\xe0\xef\x00v\xd9Y2\x02KD\xdc\
+U\xf0\x0ez\xc4+\x809\x03Dl\xc7\xb0(\xb6)\
+\xfbj\x92\x80:\xea\x94\xc1\x8e\x9c9l\xf5!e,\
+X\xc1;\xc1\xc1\x95TF\x81\xc4i&\x1c\xb6\xf4\xd2\
+\xa8_\x8d\xc0T\x02\xea,\x1e\x06\x12\xd9\x86o\xc05\
+\x12\x93f\xe8Q\xa6~48w\xb0\xb5\xdb\xc8H\x88\
+{\xa8\xd1i\xaa\xf0\xdb%\x96*w(;J\xcc\x02\
+5\x88F\xf0\x96V{1\xfb\xca\xe1i\x8a\x88\xad\xd4\
+fg$\x1c\xb3\x0ftq \x0b\xeb\x81\x93\xa0\x80[\
+\xfb\x9d^V\x91.D\x9c\x9c\x8f\x11|\xd7^\xf1A\
+\xeb\xac\xc0\x99\xc8\x82T\xfd\x1e\xe5\xf4\xd3\xae\xdc\x89\xa8\
+\x17\xfc\xd0@g\x8d@T\xd8S\x91f\xc4\xdb\xb0\x8f\
+\x1e\xf5B\x17hj\xe6z\xdfm\x04\xd4LG\x94\xa9\
+|\x8a\xc0\xac\x11\x08\xcc\x99\x7f\x80\x80CY\xc4U\xa1\
+R\xa7\xc3\x03\x04z\x94Y\xaen\xda\x09\xf6ch%\
+\xc0\xa7\xacXg\x9e9\x8c\x07\x0e=\xb6[\x8f\xab&\
+\x91\xf9\x0e\x9a!\xefq\xedBi\x91\x17\xca\xb3?\xec\
+2>\xb5\xbe%\x11\x18x\x82a|\xf3\xc1\xa4\xdd\x8e\
+G\x22\xbd\xa6\x13\x1a\x82\x09\x02\x09\xcb\xf3\xcce\x10\x9e\
+\xc5KO;m\xec\xee\xe78a+\xae\xfd\x97\xb4*\
+\xf6M\x91K\x11i\xc3\xc7\xa2\x0bn\xfa!u\x0dD\
+R\x06n\xfe\x8cX\xa5G\xf9\x1b\xda\x7fH#\xb6\xda\
+\xb9\xfc\x15\xfb\x13\xf9\x01\xafRRL\xcb)\xf0z\x00\
+\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x00\xc1\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
+\x00\x00\x00\x88IDATX\x85\xed\xd0A\x0d\xc0 \
+\x10D\xd1/\xa1\x12\x90\x80\x04$ \xa1\x12\xea\xb0\x12\
+\x90\x80\x04$\xb4\x87\xa6\x09\xe1\x04]\xd2\xb4\xc9L2\
+\xc7\xdd}Y\xf8p\x16 \x00\xab\xb1\xe1\xc9q\x0fd\
+\xe0\x98\xd42\x0aI\x13\x8f\xd7\x88\xae\xb8f0\x19[\
+\xefr=\x00\xdf\x0cYS\xef\x0a\x02\x08 \x80\x00\x02\
+\x08 \x80\x00\x02\x08\xf0\x0b\xc0\xd2\x0c\xed\xc6\xd6\xbb\x5c\
+\xaf:7\x833\x9a{\x8f\xc3\xf5\xaa2\xf1x\x01\xe2\
+\x08\xe0N\x046c#\x03\xaf\x7f='\x7fv\x14\x9c\
+N\x18\xe9\xb6\x00\x00\x00\x00IEND\xaeB`\x82\
+\
+\x00\x00\x01\x06\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
+\x00\x00\x00\xcdIDATX\x85\xed\x95Q\x0d\xc3 \
+\x14E\x8f\x84I@\xc2$TB%T\xc2$\xe0\x00\
+\x09\x95P\x09H@B%TB\xf7\x01iH\xd3m\
+\xa4\x09\xdc&\xebM\x0e\xbf\x9c<\xf2.p\xe7b1\
+\x80\x03\xfc\x01\x13`k\x0b\x8c\xc0\xfa\x83\x00<k\x09\
+\xcc\x05\x02+\xb0\x00C\x0d\x81\x92\xcbs<qj\xae\
+\x10\xcb\x97\xe9\x99\x13\x02g\xe9\x8f\x04\xba\x86\x02\xd3\xa7\
+)\xfcg^\x1c\xef}m\xb6^)]\xbd\x1a,\xa4\
+C%\xb0Bl6\xd5\xe5\x81\xf4\x1e*\x01\x0f\xb1\xa1\
+T\x02\xa3Z\xc0A\x5cC\x95\x80\x85\xd8\xcb*\x81\x01\
+\xda\xfe\x01{zh\xfb\x0b\xee\xe9\x00\x1eB\x01C\x8a\
+\xaa\x0d\xb7(\x04\xe6\x5c@Q\xc7!\x17\xf0\x02\x01\x9f\
+\x0b(\xda\xd0\xe5\x02&\x19\x85Fx\xd2\x0a\xde\x91\xe7\
+\x0dk\x8ey`\x16\x09pi\x00\x00\x00\x00IEN\
+D\xaeB`\x82\
+\x00\x00\x00\xf1\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
+\x00\x00\x00\xb8IDATX\x85\xed\x97Q\x0d\x830\
+\x14E\x8f\x04$ a\x12&\xa1\x12&\x01\x09u\x80\
+\x04$L\x02\x12*\xa1\x12*a\xfb(M\xba\x97.\
+K\x0a<\xf6\xf1nr?\xe8\xcf9\xf4A\xd2\xc2\x9f\
+ePh33\x90\x80\x97R\x13\xe0\x0b|R\x04\xcb\
+N\x00\xb1Z\x08\x0a\xady\x09at\xff6\xa3\x03s\
+\x13L\x130\x01\x130\x01\x130\x01\x130\x81\x8f\x87\
+\x85|L:\xb3^\x0aD\xb1\xa0\xd9\x08\xd7\x1eJ}\
+\x99\xcb\xf3\x02\xf8\x8a\xb8'8\xf2\xfd \x9c\x08\x0d\xdb\
+\xcb:\x09o\xc5\x91\xc7\xb3tJ\x15\x98'\x7f\xf9?\
+\x81\xad\x0c\xe4_\xb3G`\x05\x1e=\xd0\x1a~\xc48\
+\x020\xee\x11\x19w\xb6k\xeb\xd5\xf2\x06\xc9:~b\
+*a\x8b\xe0\x00\x00\x00\x00IEND\xaeB`\x82\
+\
+\x00\x00\x014\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
+\x00\x00\x00\xfbIDATX\x85\xed\x96Q\x11\x830\
+\x10DW\x02\x12\x22\x01\x09\x95\x10\x09\x91\x80\x04\x1cT\
+B$ \x01\x09H\x88\x04$\xd0\x8f\x90!\xa5\x5cH\
+\xd2\xbb|\xb13\xfb\xc5\x0c\xfb\x80\xbd\x0b\xc0\xa3Gy\
+\xea+\xac\xb8\x82\x17\x00[\xa5\xdd~\x8f*u\x7f\x86\
+\x07\xaf\xb5\x00\x9a!<\xd8\xd4\x00\xcc\x8c\x00\xae4\xbc\
+g\x0c\x0f.\xea\x82\x15\x00\xb0\xb9\xe1\x1d|q\xb8\x01\
+6d\x8e\xe6(\x14\xbe\x01\x18r\x008F\x8f\xf2\xed\
+Hr\x8e\x1ee\x93\x02\x98\x1a\x00,T\xb8j\x10\x9e\
+,\xe3\xd8\x10\xc0^\x01\xb8\x86\x00?e\x94\xd8|w\
+~\xc5\x00\xe7\xf6;\xf8\xb2p\xfa\xbc\xdc\x0c\x05`\xe1\
+\xb7\xa1\x84\xe2)\xd3\xf1\x85\x8e\x22cV\xfc\xa0\xea|\
+1\xbc\xa2\xacuY\xa9\x01D\x09\x81\xe3\xfc\x9f\x04\x01\
+,\x12\xcb\xe8\x8d\x83N\x09\x84\xc7\xa7\xec\xe5\x1e\x88\xbf\
+\x8f\xdb\x81\x06&\x8f\xf8>\xe4\x0cE\xd8j\x09\x91\x7f\
+G\x1a\xbe\x0b\xdc; x\x86l\xc9\x1f\x95\xeb\x03w\
+\x86\xc7l\xd1\x8c;C\x00\x00\x00\x00IEND\xae\
+B`\x82\
+\x00\x00\x01\x90\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
+\x00\x00\x00\x06bKGD\x00\xff\x00\xff\x00\xff\xa0\xbd\
+\xa7\x93\x00\x00\x00\x09pHYs\x00\x00\x0b\x13\x00\x00\
+\x0b\x13\x01\x00\x9a\x9c\x18\x00\x00\x00\x07tIME\x07\
+\xde\x06\x12\x07)\x0f@\x06)\xb4\x00\x00\x01\x1dID\
+ATX\xc3\xed\xd7=J\xc4P\x10\xc0\xf1\x9f\xdf\x82\
+\x16\x82`!*+(\x1669\xc2z\x02=\x80\xe0\
+\x1d\x16\x0f\x22\xd8\xdax\x01\xaf\xa0\xa5\x8d\xb8\x16v\xc2\
+\xae\x88X\xa9\xd8\x0a\xa2\xcd[xD\x5c7\xe4i\x9a\
+70\x90L\xded\xfeo&\x99\xc7\xd0\xb0\x8c\x0dy\
+\xb6\x80\x02\xad\x9a1\xfa\xb8\xa8\xeaT\xa0\x87\xcfD\xfa\
+\x8av\x15\x80\xeb\x84\xc1c\x88\x91J\xd0\x0a\xbb\x1fH\
+\xb7f\x09\x8a\xe8z=\x94\xe4W\x87\x98\xbc\xae\xc4\xef\
+\xfaV\x86\xf1\xa6\xff\x82\x0c\x90\x012@\x15\x80\xd9\xa0\
+q\x13\x9b\xc7Td\x9b\xc0\xdc_\x00\xac\xe2\x08\xc7X\
+\x0e\xb6]\x9c\xe2\x103!x'\xd8v\xea\xb6\xcer\
+'\xdc\x8f\xee\x0f0\x8d3|\xe0\x01[X\xc1sX\
+s\x92\xba\x13\xde\x86\x03\xea\x1ewx\xc7%\x1eq\x83\
+\x17\xbc\x05\xdb\x13\xaeRg\x00\xd6\xb0Q\xfa&\xb6\xb1\
+\x14\xd9\x16\xb1Y\xda\xd8\xd0\x0c\xe4\xc3(\x03d\x80\x0c\
+\xd08\xc0\xe4\x0f\x93L,\xe7\x09\xe3\xf5G]\x98r\
+*\x1ah\xaf\x0ai;L2)\xa7\xa2\xbd\xaa\xc3\xa9\
+\xe0\x94b8\xedVI\xff\xbf\xca\x17s\x0c\x90\x8c\x16\
+$\xacm\x00\x00\x00\x00IEND\xaeB`\x82\
+\x00\x00\x01\xf1\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00 \x00\x00\x00 \x08\x06\x00\x00\x00szz\xf4\
+\x00\x00\x01\xb8IDATX\x85\xd5Wm\x91\xc5 \
+\x0c\x5c\x09H@B% \xe1I\xa8\x84J\xc0A%\
+ \xa1\x12*\xa1\x12NB%\xbc\xfb\x01\xdc\x844@\
+\xe8\xeb\xcd\xcde\x86_\x84\xecf\x13\xbe\x80\x7ff\x06\
+\x80\x03\xb0\x00X\x01\x844|\x1a\xee\xb7\x80\xa7\x04\xf8\
+\x05\xe0\xad\x18+\x00\xfb\x04\xb0I\xc1N%\xb0D\xc4\
+\xdc\x05\x9fP\xcf\xf8\x00\xb0%\x00\x8fX\x86\xbd\xe2{\
+\xa6XC\xe6p\xcd\xfaL`\xad`\x06\xb1?$\xc5\
+\x9c\x16|\x12\x02\xdc\x91\xd2\x0b$\xbaJ\x18Dyi\
+\xd6\xf3 05\x87\xab\x8a\xcdD<[\xf0\x09x\x8d\
+D\xa89Z\x94\xd2\xafJ\x00MiVF\xc2\xf6\x9c\
+\xbaR\xb1u/\x05I\xba\xa3D\x15\xa8\x83W\x82g\
+\x02\x9a.\x9fQ&X\xd8\x04\x85D\x1d\x02=\x12\x86\
+a\x14\xbe\x0b\x998\x84\xc5\x16Q!i\xd0\xbe\xe9\x1d\
+:\xf4\xb0\xf2t\xc2\xa3]\x1f\xcb\xd8\xb7F\x8b\x04U\
+\xab\xc0\x09dB\xea\xfe\x11\x02\x99\x84\x15\xe2\xd0D\xb7\
+\x1a\x01\xff\x10\x01I\x05Z\xea\x9dNPi\xb6\xeb\xba\
+\xe1\x128!\x06O\xb4P\xda\xb3\x00\xdc\xf2>\xd64\
+a\xebL\xd8j\x04\x1c\xcb\xc26\x82p\xcb\xea\xf5\xc0\
+\x0d#{\xf1\xa5\x07\xd12H\xa0\x07\x8e4\xdf<i\
+\x03\xdaeh\x11\x98;>\xfc\x96\x95\xfa\xec\xd2h^\
+I\xc0*|<\x8b\xedj\x8e\x819\xf6d\xd5\xd8\x8c\
+\xb2\xf6b\xf6\xd9\xf8\xad\xf5)\x09\x87\xeb.\xb1\xbdE\
+\xfcb\xaa\x9d\x8e-\x93^\xd3\x9aF\xfd1'\x90\xd0\
+<\xcfL\x02\xe1*\xdez\xdaI\x8fSZ\xc7\x80\xd8\
+\x5c\xf9\x97tT\xfc\x872\x972\xe2\x8d92v<\
+\xf4C\x9a\x06\x88\x9c\x09x\xf83\xa2\xb5\x17\xca\xdfP\
+\xfe!\xad\x88\xbds\xfb+\xf6'\xf6\x0d\xaeFRL\
+\x5c\x1b\x18x\x00\x00\x00\x00IEND\xaeB`\x82\
+\
+"
+
+qt_resource_name = b"\
+\x00\x06\
+\x07\x8f\xcd%\
+\x00r\
+\x00i\x00f\x00f\x00l\x00e\
+\x00\x04\
+\x00\x06\xfa^\
+\x00i\
+\x00c\x00o\x00n\
+\x00\x08\
+\x08\xcd\x08#\
+\x00p\
+\x00r\x00e\x00v\x00i\x00o\x00u\x00s\
+\x00\x02\
+\x00\x00\x07\xc0\
+\x00u\
+\x00p\
+\x00\x04\
+\x00\x06\xd0%\
+\x00f\
+\x00i\x00l\x00e\
+\x00\x06\
+\x06\xd6*\xc2\
+\x00f\
+\x00o\x00l\x00d\x00e\x00r\
+\x00\x08\
+\x06G\xc7\x82\
+\x00c\
+\x00o\x00m\x00p\x00u\x00t\x00e\x00r\
+\x00\x05\
+\x00k\x90\xc5\
+\x00d\
+\x00r\x00i\x00v\x00e\
+\x00\x0a\
+\x02\xb7\xe4>\
+\x00c\
+\x00o\x00l\x00l\x00e\x00c\x00t\x00i\x00o\x00n\
+\x00\x04\
+\x00\x07L\xf4\
+\x00n\
+\x00e\x00x\x00t\
+"
+
+qt_resource_struct = b"\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00\x12\x00\x02\x00\x00\x00\x08\x00\x00\x00\x03\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x006\x00\x00\x00\x00\x00\x01\x00\x00\x01\xfc\
+\x00\x00\x01\x8f\x04\xb1\xe3\x04\
+\x00\x00\x00@\x00\x00\x00\x00\x00\x01\x00\x00\x03\xec\
+\x00\x00\x01\x8f\x04\xb1\xe3\x05\
+\x00\x00\x00\xa0\x00\x00\x00\x00\x00\x01\x00\x00\x09|\
+\x00\x00\x01\x8f\x04\xb1\xe3\x04\
+\x00\x00\x00v\x00\x00\x00\x00\x00\x01\x00\x00\x06\xb0\
+\x00\x00\x01\x8f\x04\xb1\xe3\x05\
+\x00\x00\x00\x86\x00\x00\x00\x00\x00\x01\x00\x00\x07\xe8\
+\x00\x00\x01\x8f\x04\xb1\xe3\x05\
+\x00\x00\x00`\x00\x00\x00\x00\x00\x01\x00\x00\x05\xbb\
+\x00\x00\x01\x8f\x04\xb1\xe3\x06\
+\x00\x00\x00N\x00\x00\x00\x00\x00\x01\x00\x00\x04\xb1\
+\x00\x00\x01\x8f\x04\xb1\xe3\x06\
+\x00\x00\x00 \x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x01\x8f\x04\xb1\xe3\x04\
+"
+
+def qInitResources():
+    QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
+
+def qCleanupResources():
+    QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
+
+qInitResources()
```


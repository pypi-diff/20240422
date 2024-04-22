# Comparing `tmp/pih-plb_db-0.16.tar.gz` & `tmp/pih-plb_db-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_db-0.16.tar", last modified: Mon Apr 15 00:55:24 2024, max compression
+gzip compressed data, was "pih-plb_db-0.18.tar", last modified: Mon Apr 22 04:03:54 2024, max compression
```

## Comparing `pih-plb_db-0.16.tar` & `pih-plb_db-0.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 00:55:25.027242 pih-plb_db-0.16/
--rw-rw-rw-   0        0        0      280 2024-04-15 00:55:24.994954 pih-plb_db-0.16/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 00:55:24.551223 pih-plb_db-0.16/PolibaseDatabaseService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.16/PolibaseDatabaseService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.16/PolibaseDatabaseService/__main__.py
--rw-rw-rw-   0        0        0     6528 2024-03-30 01:06:51.000000 pih-plb_db-0.16/PolibaseDatabaseService/api.py
--rw-rw-rw-   0        0        0      568 2024-04-15 00:44:28.000000 pih-plb_db-0.16/PolibaseDatabaseService/const.py
--rw-rw-rw-   0        0        0     1146 2024-04-10 00:35:00.000000 pih-plb_db-0.16/PolibaseDatabaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-15 00:55:24.948083 pih-plb_db-0.16/pih_plb_db.egg-info/
--rw-rw-rw-   0        0        0      280 2024-04-15 00:55:23.000000 pih-plb_db-0.16/pih_plb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-04-15 00:55:24.000000 pih-plb_db-0.16/pih_plb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 00:55:24.000000 pih-plb_db-0.16/pih_plb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-15 00:55:24.000000 pih-plb_db-0.16/pih_plb_db.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-15 00:55:24.000000 pih-plb_db-0.16/pih_plb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-15 00:55:24.000000 pih-plb_db-0.16/pih_plb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 00:55:25.027242 pih-plb_db-0.16/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-22 04:03:54.723813 pih-plb_db-0.18/
+-rw-rw-rw-   0        0        0      280 2024-04-22 04:03:54.692557 pih-plb_db-0.18/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-22 04:03:54.367854 pih-plb_db-0.18/PolibaseDatabaseService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.18/PolibaseDatabaseService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.18/PolibaseDatabaseService/__main__.py
+-rw-rw-rw-   0        0        0     9811 2024-04-22 03:57:57.000000 pih-plb_db-0.18/PolibaseDatabaseService/api.py
+-rw-rw-rw-   0        0        0     1074 2024-04-22 04:02:19.000000 pih-plb_db-0.18/PolibaseDatabaseService/const.py
+-rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.18/PolibaseDatabaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-22 04:03:54.661314 pih-plb_db-0.18/pih_plb_db.egg-info/
+-rw-rw-rw-   0        0        0      280 2024-04-22 04:03:53.000000 pih-plb_db-0.18/pih_plb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-04-22 04:03:54.000000 pih-plb_db-0.18/pih_plb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 04:03:53.000000 pih-plb_db-0.18/pih_plb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-22 04:03:53.000000 pih-plb_db-0.18/pih_plb_db.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-22 04:03:53.000000 pih-plb_db-0.18/pih_plb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-22 04:03:53.000000 pih-plb_db-0.18/pih_plb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 04:03:54.739437 pih-plb_db-0.18/setup.cfg
```

### Comparing `pih-plb_db-0.16/PolibaseDatabaseService/api.py` & `pih-plb_db-0.18/PolibaseDatabaseService/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,16 @@
 import ipih
 
 import os
 from pih import A
-from pih.tools import j, js, n
+from pih.tools import j, n, js, esc
+from PolibaseDatabaseService.const import *
 
 TEST: bool = False
 #
-TEST_NAME: str = "test"
-STUB_DIRECTORY_NAME: str = "stub"
-#
-POLIBASE_NAME: str = "Polibase"
-ARCHIVE_TYPE: str = A.CT_F_E.ARCHIVE
-
-
-class MOUNT_POINT:
-    POLIBASE: str = "C:"
-    NAS: str = "K:"
-    POLIBASE2: str = "L:"
-
-
-class DATABASE_DUMP:
-    FILE_NAME: str = "DatabaseDump"
-    FILE_EXTENSION: str = "DMP"
 
 
 class PolibaseDBApi:
 
     @staticmethod
     def create_dump(file_name: str | None = None, test: bool | None = None) -> None:
         test = TEST if n(test) else test
@@ -33,25 +18,27 @@
         local_polibase_database_dump_folder_name: str = j(
             (POLIBASE_NAME, DATABASE_DUMP.FILE_NAME)
         )
         nas_polibase_database_dump_folder_name: str = A.PTH.join(
             POLIBASE_NAME, DATABASE_DUMP.FILE_NAME
         )
         polibase_folder_path: str = A.PTH.join(
-            MOUNT_POINT.POLIBASE, "\\", local_polibase_database_dump_folder_name
+            j((MOUNT_POINT.POLIBASE, A.CT.SPLITTER)),
+            "\\",
+            local_polibase_database_dump_folder_name,
         )
 
-        dump_file_name_result: str = "IN"
-
         if test:
             file_name = TEST_NAME
         else:
             if n(file_name):
                 file_name = A.D.now_to_string(A.CT_P.DB_DATETIME_FORMAT)
 
+        dump_file_name_result: str = DATABASE_DUMP.RESULT_FILE_NAME
+
         dump_file_name_result = A.PTH.add_extension(
             dump_file_name_result, DATABASE_DUMP.FILE_EXTENSION
         )
         file_database_dump_name_out: str = A.PTH.add_extension(
             file_name, DATABASE_DUMP.FILE_EXTENSION
         )
         if test:
@@ -69,50 +56,50 @@
                     )
                 )
             )
         polibase2_folder_path: str = A.PTH.for_windows(
             A.PTH.join(A.CT_H.POLIBASE2.NAME, local_polibase_database_dump_folder_name)
         )
 
-        nas_folder_path: str = A.PTH.for_windows(
-            A.PTH.join(
-                A.CT_H.NAS.NAME, "backups", nas_polibase_database_dump_folder_name
-            )
-        )
-
         archiver_program_path: str = 'C:/"Program Files"/7-Zip/7z'
 
         file_out_name = A.PTH.add_extension(file_name, ARCHIVE_TYPE)
 
-        nas_create_connection_command = js(
-            (
-                "net",
-                "use",
-                MOUNT_POINT.NAS,
-                nas_folder_path,
-                j(("/user:", A.D_V_E.value("NAS_USER_LOGIN"))),
-                A.D_V_E.value("NAS_USER_PASSWORD"),
-            )
-        )
-        polibase2_create_connection_command = js(
+        nas_copy_command = js(
             (
-                "net",
-                "use",
-                MOUNT_POINT.POLIBASE2,
-                polibase2_folder_path,
+                "robocopy",
+                polibase_folder_path,
+                j(
+                    (
+                        (
+                            PRECONNECTED_MOUNT_POINT.NAS
+                            if USE_PRECONNECTED_DISKS
+                            else MOUNT_POINT.NAS
+                        ),
+                        A.CT.SPLITTER,
+                    )
+                ),
+                file_out_name,
+                "/J",
             )
         )
-        nas_copy_command = js(
-            ("robocopy", polibase_folder_path, MOUNT_POINT.NAS, file_out_name, "/J")
-        )
         polibase2_copy_command = js(
             (
                 "robocopy",
                 polibase_folder_path,
-                MOUNT_POINT.POLIBASE2,
+                j(
+                    (
+                        (
+                            PRECONNECTED_MOUNT_POINT.POLIBASE2
+                            if USE_PRECONNECTED_DISKS
+                            else MOUNT_POINT.POLIBASE2
+                        ),
+                        A.CT.SPLITTER,
+                    )
+                ),
                 file_database_dump_name_out,
                 "/J",
             )
         )
         os.chdir(polibase_folder_path)
         # step 1
         A.E.backup_notify_about_polibase_creation_db_dumb_start(not test)
@@ -131,26 +118,61 @@
             os.path.getsize(
                 A.PTH.join(polibase_folder_path, file_database_dump_name_out)
             ),
             not test,
         )
 
         # step 2: connect net location with credentials
-        os.system(nas_create_connection_command)
-        os.system(polibase2_create_connection_command)
+        if not USE_PRECONNECTED_DISKS:
+            nas_folder_path: str = A.PTH.for_windows(
+                A.PTH.join(
+                    A.CT_H.NAS.NAME, "backups", nas_polibase_database_dump_folder_name
+                )
+            )
+            nas_create_connection_command = js(
+                (
+                    "net",
+                    "use",
+                    j((MOUNT_POINT.NAS, A.CT.SPLITTER)),
+                    nas_folder_path,
+                    j(("/user:", A.D_V_E.value("NAS_USER_LOGIN"))),
+                    A.D_V_E.value("NAS_USER_PASSWORD"),
+                )
+            )
+            polibase2_create_connection_command = js(
+                (
+                    "net",
+                    "use",
+                    j((MOUNT_POINT.POLIBASE2, A.CT.SPLITTER)),
+                    polibase2_folder_path,
+                )
+            )
+            os.system(nas_create_connection_command)
+            os.system(polibase2_create_connection_command)
 
         # step 3
         A.E.backup_notify_about_polibase_creation_archived_db_dumb_start()
-        os.system(
-            js(
-                (
-                    archiver_program_path,
-                    j(("a -t", ARCHIVE_TYPE)),
-                    file_out_name,
-                    file_database_dump_name_out,
+        print(
+            os.system(
+                js(
+                    (
+                        archiver_program_path,
+                        j(("a -t", ARCHIVE_TYPE)),
+                        j(("-mx", COMPRESSION_RATIO)),
+                        j(
+                            (
+                                "-p",
+                                esc(
+                                    A.D_V_E.value("POLIBASE_DATABASE_ARCHIVE_PASSWORD")
+                                ),
+                            )
+                        ),
+                        file_out_name,
+                        file_database_dump_name_out,
+                    )
                 )
             )
         )
 
         A.E.backup_notify_about_polibase_creation_archived_db_dumb_complete(
             os.path.getsize(A.PTH.join(polibase_folder_path, file_out_name)), not test
         )
@@ -174,31 +196,92 @@
         )
 
         # step 6
         polibase2_previous_file_delete_command: str = js(
             (
                 "del",
                 A.PTH.for_windows(
-                    A.PTH.join(MOUNT_POINT.POLIBASE2, "\\", dump_file_name_result)
+                    A.PTH.join(
+                        j(
+                            (
+                                (
+                                    PRECONNECTED_MOUNT_POINT.POLIBASE2
+                                    if USE_PRECONNECTED_DISKS
+                                    else MOUNT_POINT.POLIBASE2
+                                ),
+                                A.CT.SPLITTER,
+                            )
+                        ),
+                        "\\",
+                        dump_file_name_result,
+                    )
                 ),
             )
         )
         polibase_file_rename_command: str = js(
             (
                 "ren",
                 A.PTH.for_windows(
-                    A.PTH.join(MOUNT_POINT.POLIBASE2, "\\", file_database_dump_name_out)
+                    A.PTH.join(
+                        j(
+                            (
+                                (
+                                    PRECONNECTED_MOUNT_POINT.POLIBASE2
+                                    if USE_PRECONNECTED_DISKS
+                                    else MOUNT_POINT.POLIBASE2
+                                ),
+                                A.CT.SPLITTER,
+                            )
+                        ),
+                        "\\",
+                        file_database_dump_name_out,
+                    )
                 ),
                 dump_file_name_result,
             )
         )
 
         os.system(polibase2_previous_file_delete_command)
         os.system(polibase_file_rename_command)
 
         # step 7: disconnect net location with credentials
-        os.system(js(("net use", MOUNT_POINT.NAS, "/delete /y")))
-        os.system(js(("net use", MOUNT_POINT.POLIBASE2, "/delete /y")))
+        if not USE_PRECONNECTED_DISKS:
+            os.system(
+                js(
+                    (
+                        "net use",
+                        j(
+                            (
+                                (
+                                    PRECONNECTED_MOUNT_POINT.NAS
+                                    if USE_PRECONNECTED_DISKS
+                                    else MOUNT_POINT.POLIBASE2
+                                ),
+                                A.CT.SPLITTER,
+                            )
+                        ),
+                        "/delete /y",
+                    )
+                )
+            )
+            os.system(
+                js(
+                    (
+                        "net use",
+                        j(
+                            (
+                                (
+                                    PRECONNECTED_MOUNT_POINT.POLIBASE2
+                                    if USE_PRECONNECTED_DISKS
+                                    else MOUNT_POINT.POLIBASE2
+                                ),
+                                A.CT.SPLITTER,
+                            )
+                        ),
+                        "/delete /y",
+                    )
+                )
+            )
 
         # step 8
         os.system(js(("del", file_database_dump_name_out)))
         os.system(js(("del", file_out_name)))
```

### Comparing `pih-plb_db-0.16/PolibaseDatabaseService/service.py` & `pih-plb_db-0.18/PolibaseDatabaseService/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import ipih
 
-from pih import A, PIHThread
+from pih import A
 from PolibaseDatabaseService.const import SD
 
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
 def start(as_standalone: bool = False) -> None:
```


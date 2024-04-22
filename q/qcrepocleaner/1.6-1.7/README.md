# Comparing `tmp/qcrepocleaner-1.6.tar.gz` & `tmp/qcrepocleaner-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcrepocleaner-1.6.tar", last modified: Thu Aug 24 08:22:46 2023, max compression
+gzip compressed data, was "qcrepocleaner-1.7.tar", last modified: Mon Apr 22 08:32:27 2024, max compression
```

## Comparing `qcrepocleaner-1.6.tar` & `qcrepocleaner-1.7.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-08-24 08:22:46.145812 qcrepocleaner-1.6/
--rw-r--r--   0 bvonhall   (502) staff       (20)     3807 2023-08-24 08:22:46.145330 qcrepocleaner-1.6/PKG-INFO
--rw-r--r--   0 bvonhall   (502) staff       (20)     3182 2023-08-10 07:21:55.000000 qcrepocleaner-1.6/README.md
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-08-24 08:22:46.050830 qcrepocleaner-1.6/qcrepocleaner/
--rw-r--r--   0 bvonhall   (502) staff       (20)    10303 2023-06-26 09:12:45.000000 qcrepocleaner-1.6/qcrepocleaner/Ccdb.py
--rw-r--r--   0 bvonhall   (502) staff       (20)        0 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/qcrepocleaner/__init__.py
--rw-r--r--   0 bvonhall   (502) staff       (20)      688 2023-05-15 08:10:36.000000 qcrepocleaner-1.6/qcrepocleaner/binUtils.py
--rwxr-xr-x   0 bvonhall   (502) staff       (20)    15668 2023-06-26 09:12:45.000000 qcrepocleaner-1.6/qcrepocleaner/o2-qc-repo-cleaner
--rwxr-xr-x   0 bvonhall   (502) staff       (20)     3571 2023-07-12 06:15:02.000000 qcrepocleaner-1.6/qcrepocleaner/o2-qc-repo-delete-not-in-runs
--rwxr-xr-x   0 bvonhall   (502) staff       (20)     4436 2023-03-22 10:52:32.000000 qcrepocleaner-1.6/qcrepocleaner/o2-qc-repo-delete-objects-in-runs
--rwxr-xr-x   0 bvonhall   (502) staff       (20)     3234 2023-03-22 10:52:32.000000 qcrepocleaner-1.6/qcrepocleaner/o2-qc-repo-delete-time-interval
--rwxr-xr-x   0 bvonhall   (502) staff       (20)     3080 2023-03-17 13:45:20.000000 qcrepocleaner-1.6/qcrepocleaner/o2-qc-repo-find-objects-not-updated
--rwxr-xr-x   0 bvonhall   (502) staff       (20)     3368 2023-03-22 10:52:32.000000 qcrepocleaner-1.6/qcrepocleaner/o2-qc-repo-move-objects
--rw-r--r--   0 bvonhall   (502) staff       (20)     1249 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/qcrepocleaner/pidfile.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     1138 2023-08-22 13:15:34.000000 qcrepocleaner-1.6/qcrepocleaner/policies_utils.py
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-08-24 08:22:46.120524 qcrepocleaner-1.6/qcrepocleaner/rules/
--rw-r--r--   0 bvonhall   (502) staff       (20)     2927 2023-07-11 11:49:30.000000 qcrepocleaner-1.6/qcrepocleaner/rules/1_per_hour.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     5494 2023-03-17 13:45:20.000000 qcrepocleaner-1.6/qcrepocleaner/rules/1_per_run.py
--rw-r--r--   0 bvonhall   (502) staff       (20)        0 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/qcrepocleaner/rules/__init__.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     2739 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/qcrepocleaner/rules/last_only.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     5967 2023-08-22 13:15:34.000000 qcrepocleaner-1.6/qcrepocleaner/rules/multiple_per_run.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     2282 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/qcrepocleaner/rules/none_kept.py
--rw-r--r--   0 bvonhall   (502) staff       (20)      987 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/qcrepocleaner/rules/plugin_template.py
--rw-r--r--   0 bvonhall   (502) staff       (20)    12266 2023-07-11 11:49:30.000000 qcrepocleaner-1.6/qcrepocleaner/rules/production.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     1408 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/qcrepocleaner/rules/skip.py
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-08-24 08:22:46.072677 qcrepocleaner-1.6/qcrepocleaner.egg-info/
--rw-r--r--   0 bvonhall   (502) staff       (20)     3807 2023-08-24 08:22:45.000000 qcrepocleaner-1.6/qcrepocleaner.egg-info/PKG-INFO
--rw-r--r--   0 bvonhall   (502) staff       (20)     1088 2023-08-24 08:22:45.000000 qcrepocleaner-1.6/qcrepocleaner.egg-info/SOURCES.txt
--rw-r--r--   0 bvonhall   (502) staff       (20)        1 2023-08-24 08:22:45.000000 qcrepocleaner-1.6/qcrepocleaner.egg-info/dependency_links.txt
--rw-r--r--   0 bvonhall   (502) staff       (20)       55 2023-08-24 08:22:45.000000 qcrepocleaner-1.6/qcrepocleaner.egg-info/requires.txt
--rw-r--r--   0 bvonhall   (502) staff       (20)       20 2023-08-24 08:22:45.000000 qcrepocleaner-1.6/qcrepocleaner.egg-info/top_level.txt
--rw-r--r--   0 bvonhall   (502) staff       (20)       38 2023-08-24 08:22:46.145963 qcrepocleaner-1.6/setup.cfg
--rw-r--r--   0 bvonhall   (502) staff       (20)     1416 2023-08-24 08:20:18.000000 qcrepocleaner-1.6/setup.py
-drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2023-08-24 08:22:46.144554 qcrepocleaner-1.6/tests/
--rw-r--r--   0 bvonhall   (502) staff       (20)        0 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/tests/__init__.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     4318 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/tests/test_1_per_hour.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     4173 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/tests/test_1_per_run.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     1772 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/tests/test_Ccdb.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     8735 2023-08-22 13:15:34.000000 qcrepocleaner-1.6/tests/test_MultiplePerRun.py
--rw-r--r--   0 bvonhall   (502) staff       (20)    12389 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/tests/test_Production.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     3154 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/tests/test_last_only.py
--rw-r--r--   0 bvonhall   (502) staff       (20)     2641 2023-03-17 13:01:58.000000 qcrepocleaner-1.6/tests/test_repoCleaner.py
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2024-04-22 08:32:27.359142 qcrepocleaner-1.7/
+-rw-r--r--   0 bvonhall   (502) staff       (20)     3807 2024-04-22 08:32:27.358860 qcrepocleaner-1.7/PKG-INFO
+-rw-r--r--   0 bvonhall   (502) staff       (20)     3182 2023-10-11 06:52:06.000000 qcrepocleaner-1.7/README.md
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2024-04-22 08:32:27.343492 qcrepocleaner-1.7/qcrepocleaner/
+-rw-r--r--   0 bvonhall   (502) staff       (20)    11187 2024-04-16 06:47:56.000000 qcrepocleaner-1.7/qcrepocleaner/Ccdb.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)        0 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/qcrepocleaner/__init__.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)      688 2023-10-11 06:52:06.000000 qcrepocleaner-1.7/qcrepocleaner/binUtils.py
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)    15668 2024-03-25 07:29:45.000000 qcrepocleaner-1.7/qcrepocleaner/o2-qc-repo-cleaner
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)     3571 2024-01-24 15:40:48.000000 qcrepocleaner-1.7/qcrepocleaner/o2-qc-repo-delete-not-in-runs
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)     4436 2024-03-15 07:28:37.000000 qcrepocleaner-1.7/qcrepocleaner/o2-qc-repo-delete-objects-in-runs
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)     3234 2024-02-09 07:29:33.000000 qcrepocleaner-1.7/qcrepocleaner/o2-qc-repo-delete-time-interval
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)     3080 2023-10-11 06:52:06.000000 qcrepocleaner-1.7/qcrepocleaner/o2-qc-repo-find-objects-not-updated
+-rwxr-xr-x   0 bvonhall   (502) staff       (20)     3368 2023-10-11 06:52:06.000000 qcrepocleaner-1.7/qcrepocleaner/o2-qc-repo-move-objects
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1249 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/qcrepocleaner/pidfile.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1206 2024-01-24 15:41:08.000000 qcrepocleaner-1.7/qcrepocleaner/policies_utils.py
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2024-04-22 08:32:27.351457 qcrepocleaner-1.7/qcrepocleaner/rules/
+-rw-r--r--   0 bvonhall   (502) staff       (20)     2927 2024-01-24 15:40:47.000000 qcrepocleaner-1.7/qcrepocleaner/rules/1_per_hour.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     5613 2024-04-18 08:51:30.000000 qcrepocleaner-1.7/qcrepocleaner/rules/1_per_run.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)        0 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/qcrepocleaner/rules/__init__.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     2739 2024-01-10 09:32:30.000000 qcrepocleaner-1.7/qcrepocleaner/rules/last_only.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     7730 2024-01-24 15:41:08.000000 qcrepocleaner-1.7/qcrepocleaner/rules/multiple_per_run.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     2282 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/qcrepocleaner/rules/none_kept.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)      987 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/qcrepocleaner/rules/plugin_template.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)    12266 2024-01-24 15:40:47.000000 qcrepocleaner-1.7/qcrepocleaner/rules/production.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1408 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/qcrepocleaner/rules/skip.py
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2024-04-22 08:32:27.345289 qcrepocleaner-1.7/qcrepocleaner.egg-info/
+-rw-r--r--   0 bvonhall   (502) staff       (20)     3807 2024-04-22 08:32:27.000000 qcrepocleaner-1.7/qcrepocleaner.egg-info/PKG-INFO
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1133 2024-04-22 08:32:27.000000 qcrepocleaner-1.7/qcrepocleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 bvonhall   (502) staff       (20)        1 2024-04-22 08:32:27.000000 qcrepocleaner-1.7/qcrepocleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 bvonhall   (502) staff       (20)       55 2024-04-22 08:32:27.000000 qcrepocleaner-1.7/qcrepocleaner.egg-info/requires.txt
+-rw-r--r--   0 bvonhall   (502) staff       (20)       20 2024-04-22 08:32:27.000000 qcrepocleaner-1.7/qcrepocleaner.egg-info/top_level.txt
+-rw-r--r--   0 bvonhall   (502) staff       (20)       38 2024-04-22 08:32:27.359238 qcrepocleaner-1.7/setup.cfg
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1416 2024-04-22 08:31:53.000000 qcrepocleaner-1.7/setup.py
+drwxr-xr-x   0 bvonhall   (502) staff       (20)        0 2024-04-22 08:32:27.358090 qcrepocleaner-1.7/tests/
+-rw-r--r--   0 bvonhall   (502) staff       (20)        0 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/tests/__init__.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     4318 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/tests/test_1_per_hour.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     4173 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/tests/test_1_per_run.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     1772 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/tests/test_Ccdb.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     8776 2024-01-24 15:41:08.000000 qcrepocleaner-1.7/tests/test_MultiplePerRun.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     9086 2024-01-24 15:41:08.000000 qcrepocleaner-1.7/tests/test_MultiplePerRun_deleteFirstLast.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)    12389 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/tests/test_Production.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     3154 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/tests/test_last_only.py
+-rw-r--r--   0 bvonhall   (502) staff       (20)     2641 2023-03-17 13:01:58.000000 qcrepocleaner-1.7/tests/test_repoCleaner.py
```

### Comparing `qcrepocleaner-1.6/PKG-INFO` & `qcrepocleaner-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcrepocleaner
-Version: 1.6
+Version: 1.7
 Summary: Set of tools to clean up the QCDB repository.
 Home-page: https://gitlab.cern.ch/AliceO2Group/QualityControl/Framework/script/RepoCleaner
 Author: Barthelemy von Haller
 Author-email: bvonhall@cern.ch
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qcrepocleaner-1.6/README.md` & `qcrepocleaner-1.7/README.md`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/Ccdb.py` & `qcrepocleaner-1.7/qcrepocleaner/Ccdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self.createdAt = createdAt
         # precomputed Datetime ("Dt") of the timestamp `createdAt`
         self.createdAtDt = datetime.datetime.fromtimestamp(int(createdAt) / 1000)  # /1000 because we get ms
 
     def __repr__(self):
         if "Run" in self.metadata or "RunNumber" in self.metadata:
             run_number = self.metadata["Run"] if "Run" in self.metadata else self.metadata["RunNumber"]
-            return f"Version of object {self.path} valid from {self.validFromAsDt}, run {run_number}"
+            return f"Version of object {self.path} valid from {self.validFromAsDt}, run {run_number} (uuid {self.uuid})"
         else:
             return f"Version of object {self.path} valid from {self.validFromAsDt} (uuid {self.uuid}, " \
                    f"ts {self.validFrom})"
 
 
 class Ccdb:
     '''
@@ -196,15 +196,32 @@
             headers = {'Connection': 'close'}
             r = requests.put(full_path, headers=headers)
             r.raise_for_status()
             self.counter_validity_updated += 1
         except requests.exceptions.RequestException as e:  
             logging.error(f"Exception in updateValidity: {traceback.format_exc()}")
 
+    @dryable.Dryable()
+    def updateMetadata(self, version: ObjectVersion, metadata):
+        logger.debug(f"update metadata : {metadata}")
+        full_path = self.url + '/' + version.path + '/' + str(version.validFrom) + '/' + str(version.uuid) + '?'
+        if metadata is not None:
+            for key in metadata:
+                full_path += key + "=" + metadata[key] + "&"
+        if self.set_adjustable_eov:
+            logger.debug(f"As the parameter force is set, we add metadata adjustableEOV")
+            full_path += "adjustableEOV=1&"
+        try:
+            headers = {'Connection': 'close'}
+            r = requests.put(full_path, headers=headers)
+            r.raise_for_status()
+        except requests.exceptions.RequestException as e:
+            logging.error(f"Exception in updateMetadata: {traceback.format_exc()}")
 
+    @dryable.Dryable()
     def putVersion(self, version: ObjectVersion, data):
         '''
         :param version: An ObjectVersion that describes the data to be uploaded.
         :param data: the actual data to send. E.g.:{'somekey': 'somevalue'}
         :return A list of ObjectVersion.
         '''
         full_path=self.url + "/" + version.path + "/" + str(version.validFrom) + "/" + str(version.validTo) + "/"
```

### Comparing `qcrepocleaner-1.6/qcrepocleaner/binUtils.py` & `qcrepocleaner-1.7/qcrepocleaner/binUtils.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/o2-qc-repo-cleaner` & `qcrepocleaner-1.7/qcrepocleaner/o2-qc-repo-cleaner`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/o2-qc-repo-delete-not-in-runs` & `qcrepocleaner-1.7/qcrepocleaner/o2-qc-repo-delete-not-in-runs`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/o2-qc-repo-delete-objects-in-runs` & `qcrepocleaner-1.7/qcrepocleaner/o2-qc-repo-delete-objects-in-runs`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/o2-qc-repo-delete-time-interval` & `qcrepocleaner-1.7/qcrepocleaner/o2-qc-repo-delete-time-interval`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/o2-qc-repo-find-objects-not-updated` & `qcrepocleaner-1.7/qcrepocleaner/o2-qc-repo-find-objects-not-updated`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/o2-qc-repo-move-objects` & `qcrepocleaner-1.7/qcrepocleaner/o2-qc-repo-move-objects`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/pidfile.py` & `qcrepocleaner-1.7/qcrepocleaner/pidfile.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/policies_utils.py` & `qcrepocleaner-1.7/qcrepocleaner/policies_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         run = str(v.metadata['RunNumber'])
     return run
 
 
 def group_versions(ccdb, object_path, period_pass, versions_buckets_dict: DefaultDict[str, List[ObjectVersion]]):
     # Find all the runs and group the versions (by run or by a combination of multiple attributes)
     versions = ccdb.getVersionsList(object_path)
+    logger.debug(f"group_versions: found {len(versions)} versions")
     for v in versions:
         logger.debug(f"Assigning {v} to a bucket")
         run = get_run(v)
         period_name = v.metadata.get("PeriodName") or ""
         pass_name = v.metadata.get("PassName") or ""
         key = run + period_name + pass_name if period_pass else run
         versions_buckets_dict[key].append(v)
```

### Comparing `qcrepocleaner-1.6/qcrepocleaner/rules/1_per_hour.py` & `qcrepocleaner-1.7/qcrepocleaner/rules/1_per_hour.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/rules/1_per_run.py` & `qcrepocleaner-1.7/qcrepocleaner/rules/1_per_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,118 +7,120 @@
 from typing import Dict, List, DefaultDict
 from qcrepocleaner.policies_utils import in_grace_period, group_versions
 from qcrepocleaner import policies_utils
 
 logger = logging  # default logger
 
 
-def process(ccdb: Ccdb, object_path: str, delay: int,  from_timestamp: int, to_timestamp: int, extra_params: Dict[str, str]):
-    '''
+def process(ccdb: Ccdb, object_path: str, delay: int, from_timestamp: int, to_timestamp: int,
+            extra_params: Dict[str, str]):
+    """
     Process this deletion rule on the object. We use the CCDB passed by argument.
     Objects which have been created recently are spared (delay is expressed in minutes).
-    This specific policy, 1_per_run, keeps only the most recent version for a given run based on the validity_from.
+    This specific policy, 1_per_run, keeps only the most recent version for a given run based on the createdAt.
 
     Config Parameters:
     - period_pass: Keep 1 version for a combination of run+pass+period if true.
     - delete_when_no_run: Versions without runs are preserved if delete_when_no_run is set to false (default).
-      Otherwise only the last one is preserved.
+      Otherwise, only the last one is preserved.
     THEY CANNOT BE BOTH TRUE AT THE SAME TIME
 
     It is implemented like this :
     Map of buckets: run[+pass+period] -> list of versions
     Go through all objects: Add the object to the corresponding key (run[+pass+period])
-    If delete_when_no_run is false, remove the versions without run from the map
+    If delete_when_no_run is false, remove from the map the versions without run or with run==0
     Go through the map: for each run (resp. run+pass+period) keep the most recent object and delete the rest.
 
     :param ccdb: the ccdb in which objects are cleaned up.
     :param object_path: path to the object, or pattern, to which a rule will apply.
     :param delay: the grace period during which a new object is never deleted.
     :param from_timestamp: only objects created after this timestamp are considered.
     :param to_timestamp: only objects created before this timestamp are considered.
     :param extra_params: a dictionary containing extra parameters for this rule.
     :return a dictionary with the number of deleted, preserved and updated versions. Total = deleted+preserved.
-    '''
-    
+    """
+
     logger.debug(f"Plugin 1_per_run processing {object_path}")
 
     preservation_list: List[ObjectVersion] = []
     deletion_list: List[ObjectVersion] = []
     update_list: List[ObjectVersion] = []
     versions_buckets_dict: DefaultDict[str, List[ObjectVersion]] = defaultdict(list)
 
     # config parameters
-    delete_when_no_run = (extra_params.get("delete_when_no_run", False) == True)
+    delete_when_no_run = (extra_params.get("delete_when_no_run", False) is True)
     logger.debug(f"delete_when_no_run : {delete_when_no_run}")
-    period_pass = (extra_params.get("period_pass", False) == True)
+    period_pass = (extra_params.get("period_pass", False) is True)
     logger.debug(f"period_pass : {period_pass}")
-    if delete_when_no_run == True and period_pass == True:
+    if delete_when_no_run is True and period_pass is True:
         logger.error(f"1_per_run does not allow both delete_when_no_run and period_pass to be on at the same time")
         return {"deleted": 0, "preserved": 0, "updated": 0}
 
     # Find all the runs and group the versions (by run or by a combination of multiple attributes)
     policies_utils.group_versions(ccdb, object_path, period_pass, versions_buckets_dict)
 
     logger.debug(f"Number of buckets : {len(versions_buckets_dict)}")
     if not period_pass:
         logger.debug(f"Number of versions without runs : {len(versions_buckets_dict['none'])}")
 
     # if we should not touch the files with no runs, let's just remove them from the map
     if not delete_when_no_run:
         del versions_buckets_dict['none']
+        del versions_buckets_dict['0']
 
     # Dispatch the versions to deletion and preservation lists
     for bucket, run_versions in versions_buckets_dict.items():
         # logger.debug(f"- bucket {bucket}")
+        sorted_run_versions = sorted(run_versions, key=lambda x: (x.createdAt))
 
         freshest: ObjectVersion = None
-        for v in run_versions:
-            if freshest is None or freshest.validFromAsDt < v.validFromAsDt:
-                if freshest is not None:
-                    if policies_utils.in_grace_period(freshest, delay):
-                        preservation_list.append(freshest)
-                    else:
-                        deletion_list.append(freshest)
+        for v in sorted_run_versions:
+            if freshest is None:
+                freshest = v
+            elif freshest.createdAtDt < v.createdAtDt:
+                if policies_utils.in_grace_period(freshest, delay):
+                    preservation_list.append(freshest)
+                else:
+                    deletion_list.append(freshest)
                 freshest = v
             else:
                 if policies_utils.in_grace_period(freshest, delay):
                     preservation_list.append(v)
                 else:
                     deletion_list.append(v)
         preservation_list.append(freshest)
 
     # Actual deletion
     logger.debug(f"Delete but preserve versions that are not in the period passed to the policy")
     temp_deletion_list: List[ObjectVersion] = []
     for v in deletion_list:
         if from_timestamp < v.validFrom < to_timestamp:  # in the allowed period
-            temp_deletion_list.append(v)   # we will delete any ways
+            temp_deletion_list.append(v)  # we will delete any ways
             ccdb.deleteVersion(v)
         else:
-            preservation_list.append(v)    # we preserve
+            preservation_list.append(v)  # we preserve
     deletion_list = temp_deletion_list
 
     logger.debug(f"deleted ({len(deletion_list)}) : ")
     for v in deletion_list:
         logger.debug(f"   {v}")
 
     logger.debug(f"preserved ({len(preservation_list)}) : ")
     for v in preservation_list:
         logger.debug(f"   {v}")
 
     logger.debug(f"updated ({len(update_list)}) : ")
     for v in update_list:
         logger.debug(f"   {v}")
 
-    return {"deleted" : len(deletion_list), "preserved": len(preservation_list), "updated" : len(update_list)}
-
-
+    return {"deleted": len(deletion_list), "preserved": len(preservation_list), "updated": len(update_list)}
 
 
 def main():
     logger.getLogger().setLevel(int(10))
-    dryable.set( True )
+    dryable.set(True)
     ccdb = Ccdb('http://ccdb-test.cern.ch:8080')
     process(ccdb, "qc/testRunCleanup", 0)
 
 
 if __name__ == "__main__":  # to be able to run the test code above when not imported.
     main()
```

### Comparing `qcrepocleaner-1.6/qcrepocleaner/rules/last_only.py` & `qcrepocleaner-1.7/qcrepocleaner/rules/last_only.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/rules/multiple_per_run.py` & `qcrepocleaner-1.7/qcrepocleaner/rules/multiple_per_run.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,33 +7,44 @@
 from qcrepocleaner.Ccdb import Ccdb, ObjectVersion
 from qcrepocleaner.policies_utils import in_grace_period, group_versions
 
 from qcrepocleaner import policies_utils
 
 logger = logging  # default logger
 
+
 def process(ccdb: Ccdb, object_path: str, delay: int,  from_timestamp: int, to_timestamp: int,
             extra_params: Dict[str, str]):
     '''
     Process this deletion rule on the object. We use the CCDB passed by argument.
     Objects who have been created recently are spared (delay is expressed in minutes).
 
     This specific policy, multiple_per_run, operates like this : Keep the first and the last version of a run plus
     1 version every X minutes.
 
     Extra parameters:
       - migrate_to_EOS: Migrate the object to EOS. (default: false)
       - interval_between_versions: Period in minutes between the versions we will keep. (default: 90)
       - period_pass: Keep 1 version for a combination of run+pass+period if true. (default: false)
+      - delete_first_last: delete the first and last of the run[+pass+period] before actually applying the rule.
 
     It is implemented like this :
         Map of buckets: run[+pass+period] -> list of versions
         Go through all objects: Add the object to the corresponding key (run[+pass+period])
+        Sort the versions in the bucket
         Remove the empty run from the map (we ignore objects without a run)
         Go through the map: for each run (resp. run+pass+period)
+
+            if delete_first_last
+                Get flag cleaner_2nd from first object (if there)
+                if cleaner_2nd
+                    continue   # we do not want to reprocess the same run twice
+                flag second with `cleaner_2nd`
+                delete first and last versions in the bucket
+
             Get SOR (validity of first object)
             if SOR < now - delay
                 do
                     keep first
                     delete everything for the next interval_between_versions
                 until no more
                 move the last one, from delete to preserve
@@ -58,14 +69,16 @@
     # config parameters
     period_pass = (extra_params.get("period_pass", False) is True)
     logger.debug(f"period_pass : {period_pass}")
     interval_between_versions = int(extra_params.get("interval_between_versions", 90))
     logger.debug(f"interval_between_versions : {interval_between_versions}")
     migrate_to_EOS = (extra_params.get("migrate_to_EOS", False) is True)
     logger.debug(f"migrate_to_EOS : {migrate_to_EOS}")
+    delete_first_last = (extra_params.get("delete_first_last", False) is True)
+    logger.debug(f"delete_first_last : {delete_first_last}")
 
     # Find all the runs and group the versions (by run or by a combination of multiple attributes)
     policies_utils.group_versions(ccdb, object_path, period_pass, versions_buckets_dict)
 
     # Remove the empty run from the map (we ignore objects without a run)
     logger.debug(f"Number of buckets : {len(versions_buckets_dict)}")
     if not period_pass:
@@ -81,28 +94,49 @@
         if policies_utils.in_grace_period(first_object, delay):
             logger.debug(f"     in grace period, skip this bucket")
             preservation_list.extend(run_versions)
         elif not (from_timestamp < first_object.createdAt < to_timestamp):  # in the allowed period
             logger.debug(f"     not in the allowed period, skip this bucket")
             preservation_list.extend(run_versions)
         else:
-            logger.debug(f"     not in the grace period")
+            logger.debug(f"    not in the grace period")
+
+            if delete_first_last:
+                logger.debug(f"    delete_first_last is set")
+                run_versions.sort(key=lambda x: x.createdAt)
+                # Get flag cleaner_2nd from first object (if there)
+                cleaner_2nd = "cleaner_2nd" in run_versions[0].metadata
+                if cleaner_2nd or len(run_versions) < 4:
+                    logger.debug(f"        first version has flag cleaner_2nd or there are less than 4 version, "
+                                 f"we continue to next bucket")
+                    preservation_list.extend(run_versions)
+                    continue
+                # flag second with `cleaner_2nd`
+                ccdb.updateMetadata(run_versions[1], {'cleaner_2nd': 'true'})
+                # delete first and last versions in the bucket
+                logger.debug(f"        delete the first and last versions")
+                deletion_list.append(run_versions[-1])
+                ccdb.deleteVersion(run_versions[-1])
+                del run_versions[-1]
+                deletion_list.append(run_versions[0])
+                ccdb.deleteVersion(run_versions[0])
+                del run_versions[0]
 
             last_preserved: ObjectVersion = None
             for v in run_versions:
                 logger.debug(f"process {v}")
 
                 # first or next after the period, or last one --> preserve
                 if last_preserved is None or \
                         last_preserved.createdAtDt < v.createdAtDt - timedelta(minutes=interval_between_versions) or \
                         v == run_versions[-1]:
                     logger.debug(f" --> preserve")
                     last_preserved = v
                     if migrate_to_EOS:
-                        ccdb.updateValidity(v, v.validFrom, v.validTo, metadata_for_preservation)
+                        ccdb.updateMetadata(v, metadata_for_preservation)
                     preservation_list.append(last_preserved)
                 else:  # in between period --> delete
                     logger.debug(f" --> delete")
                     deletion_list.append(v)
                     ccdb.deleteVersion(v)
 
     logger.debug(f"deleted ({len(deletion_list)}) : ")
```

### Comparing `qcrepocleaner-1.6/qcrepocleaner/rules/none_kept.py` & `qcrepocleaner-1.7/qcrepocleaner/rules/none_kept.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/rules/plugin_template.py` & `qcrepocleaner-1.7/qcrepocleaner/rules/plugin_template.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/rules/production.py` & `qcrepocleaner-1.7/qcrepocleaner/rules/production.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner/rules/skip.py` & `qcrepocleaner-1.7/qcrepocleaner/rules/skip.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/qcrepocleaner.egg-info/PKG-INFO` & `qcrepocleaner-1.7/qcrepocleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcrepocleaner
-Version: 1.6
+Version: 1.7
 Summary: Set of tools to clean up the QCDB repository.
 Home-page: https://gitlab.cern.ch/AliceO2Group/QualityControl/Framework/script/RepoCleaner
 Author: Barthelemy von Haller
 Author-email: bvonhall@cern.ch
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qcrepocleaner-1.6/qcrepocleaner.egg-info/SOURCES.txt` & `qcrepocleaner-1.7/qcrepocleaner.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,10 +26,11 @@
 qcrepocleaner/rules/production.py
 qcrepocleaner/rules/skip.py
 tests/__init__.py
 tests/test_1_per_hour.py
 tests/test_1_per_run.py
 tests/test_Ccdb.py
 tests/test_MultiplePerRun.py
+tests/test_MultiplePerRun_deleteFirstLast.py
 tests/test_Production.py
 tests/test_last_only.py
 tests/test_repoCleaner.py
```

### Comparing `qcrepocleaner-1.6/setup.py` & `qcrepocleaner-1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='qcrepocleaner',
-    version='1.6',
+    version='1.7',
     author='Barthelemy von Haller',
     author_email='bvonhall@cern.ch',
     url='https://gitlab.cern.ch/AliceO2Group/QualityControl/Framework/script/RepoCleaner',
     license='GPLv3',
     description='Set of tools to clean up the QCDB repository.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `qcrepocleaner-1.6/tests/test_1_per_hour.py` & `qcrepocleaner-1.7/tests/test_1_per_hour.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/tests/test_1_per_run.py` & `qcrepocleaner-1.7/tests/test_1_per_run.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/tests/test_Ccdb.py` & `qcrepocleaner-1.7/tests/test_Ccdb.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/tests/test_MultiplePerRun.py` & `qcrepocleaner-1.7/tests/test_MultiplePerRun.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     thirty_minutes = 1800000
     one_hour = 3600000
     in_ten_years = 1975323342000
     one_minute = 60000
 
     def setUp(self):
-        self.ccdb = Ccdb('http://ccdb-test.cern.ch:8080')
+        self.ccdb = Ccdb('http://137.138.47.222:8080')
         self.extra = {"interval_between_versions": "90", "migrate_to_EOS": False}
         self.path = "qc/TST/MO/repo/test"
 
     def test_1_finished_run(self):
         """
         1 run of 2.5 hours finished 22 hours ago.
         Expected output: SOR, EOR, 1 in the middle
@@ -73,15 +73,16 @@
         """
         logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s',
                             datefmt='%d-%b-%y %H:%M:%S')
         logging.getLogger().setLevel(int(10))
 
         # Prepare data
         test_path = self.path + "/test_5_runs"
-        self.prepare_data(test_path, [3, 3, 3, 3, 3], [60, 120, 190, 240, 24*60], 123)
+        self.prepare_data(test_path, [1*60, 2*60, 3*60+10, 4*60, 5*60],
+                          [60, 120, 190, 240, 24*60], 123)
 
         stats = multiple_per_run.process(self.ccdb, test_path, delay=60*24, from_timestamp=1,
                                        to_timestamp=self.in_ten_years, extra_params=self.extra)
         self.assertEqual(stats["deleted"], 60+120+190+240+300-18)
         self.assertEqual(stats["preserved"], 18)
         self.assertEqual(stats["updated"], 0)
```

### Comparing `qcrepocleaner-1.6/tests/test_Production.py` & `qcrepocleaner-1.7/tests/test_Production.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/tests/test_last_only.py` & `qcrepocleaner-1.7/tests/test_last_only.py`

 * *Files identical despite different names*

### Comparing `qcrepocleaner-1.6/tests/test_repoCleaner.py` & `qcrepocleaner-1.7/tests/test_repoCleaner.py`

 * *Files identical despite different names*


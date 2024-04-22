# Comparing `tmp/pygmtsar-2024.3.15.post8.tar.gz` & `tmp/pygmtsar-2024.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtsar-2024.3.15.post8.tar", last modified: Thu Apr 11 18:25:57 2024, max compression
+gzip compressed data, was "pygmtsar-2024.4.17.tar", last modified: Mon Apr 22 06:47:48 2024, max compression
```

## Comparing `pygmtsar-2024.3.15.post8.tar` & `pygmtsar-2024.4.17.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-11 18:25:57.762517 pygmtsar-2024.3.15.post8/
--rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.3.15.post8/LICENSE.txt
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-11 18:25:57.762271 pygmtsar-2024.3.15.post8/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.3.15.post8/README.md
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-11 18:25:57.760670 pygmtsar-2024.3.15.post8/pygmtsar/
--rw-r--r--   0 mbg        (501) staff       (20)    20813 2024-03-28 13:09:48.000000 pygmtsar-2024.3.15.post8/pygmtsar/ASF.py
--rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.3.15.post8/pygmtsar/AWS.py
--rw-r--r--   0 mbg        (501) staff       (20)     7454 2024-03-15 10:56:24.000000 pygmtsar-2024.3.15.post8/pygmtsar/ESA.py
--rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.3.15.post8/pygmtsar/GMT.py
--rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.3.15.post8/pygmtsar/IO.py
--rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.3.15.post8/pygmtsar/NCubeVTK.py
--rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.3.15.post8/pygmtsar/PRM.py
--rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.3.15.post8/pygmtsar/PRM_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    18986 2024-04-05 07:42:45.000000 pygmtsar-2024.3.15.post8/pygmtsar/S1.py
--rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack.py
--rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_align.py
--rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_base.py
--rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_dem.py
--rw-r--r--   0 mbg        (501) staff       (20)    44173 2024-02-08 18:53:49.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_detrend.py
--rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_export.py
--rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_geocode.py
--rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_incidence.py
--rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_landmask.py
--rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_multilooking.py
--rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_orbits.py
--rw-r--r--   0 mbg        (501) staff       (20)    47295 2024-03-29 07:29:11.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_phasediff.py
--rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_prm.py
--rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_ps.py
--rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_reframe.py
--rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_reframe_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    46640 2024-04-11 04:05:10.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_sbas.py
--rw-r--r--   0 mbg        (501) staff       (20)     8884 2024-01-01 15:32:51.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_stl.py
--rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_tidal.py
--rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_topo.py
--rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_trans.py
--rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_trans_inv.py
--rw-r--r--   0 mbg        (501) staff       (20)    26654 2024-04-11 05:08:11.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_unwrap.py
--rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_unwrap_snaphu.py
--rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.3.15.post8/pygmtsar/Tiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.3.15.post8/pygmtsar/XYZTiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.3.15.post8/pygmtsar/_Stack_merge.py
--rw-r--r--   0 mbg        (501) staff       (20)     1061 2024-04-11 02:26:04.000000 pygmtsar-2024.3.15.post8/pygmtsar/__init__.py
--rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.3.15.post8/pygmtsar/datagrid.py
--rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.3.15.post8/pygmtsar/tqdm_dask.py
--rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.3.15.post8/pygmtsar/tqdm_joblib.py
--rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.3.15.post8/pygmtsar/utils.py
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-11 18:25:57.761817 pygmtsar-2024.3.15.post8/pygmtsar.egg-info/
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-11 18:25:57.000000 pygmtsar-2024.3.15.post8/pygmtsar.egg-info/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)     1132 2024-04-11 18:25:57.000000 pygmtsar-2024.3.15.post8/pygmtsar.egg-info/SOURCES.txt
--rw-r--r--   0 mbg        (501) staff       (20)        1 2024-04-11 18:25:57.000000 pygmtsar-2024.3.15.post8/pygmtsar.egg-info/dependency_links.txt
--rw-r--r--   0 mbg        (501) staff       (20)      330 2024-04-11 18:25:57.000000 pygmtsar-2024.3.15.post8/pygmtsar.egg-info/requires.txt
--rw-r--r--   0 mbg        (501) staff       (20)        9 2024-04-11 18:25:57.000000 pygmtsar-2024.3.15.post8/pygmtsar.egg-info/top_level.txt
--rw-r--r--   0 mbg        (501) staff       (20)       38 2024-04-11 18:25:57.762575 pygmtsar-2024.3.15.post8/setup.cfg
--rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-04-11 03:27:25.000000 pygmtsar-2024.3.15.post8/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-22 06:47:48.348651 pygmtsar-2024.4.17/
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17/LICENSE.txt
+-rw-r--r--   0 mbg        (501) staff       (20)    13457 2024-04-22 06:47:48.348389 pygmtsar-2024.4.17/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17/README.md
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-22 06:47:48.346999 pygmtsar-2024.4.17/pygmtsar/
+-rw-r--r--   0 mbg        (501) staff       (20)    16155 2024-04-17 06:55:44.000000 pygmtsar-2024.4.17/pygmtsar/ASF.py
+-rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17/pygmtsar/AWS.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17/pygmtsar/GMT.py
+-rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17/pygmtsar/IO.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17/pygmtsar/NCubeVTK.py
+-rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17/pygmtsar/PRM.py
+-rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17/pygmtsar/PRM_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17/pygmtsar/S1.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.4.17/pygmtsar/Stack.py
+-rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17/pygmtsar/Stack_align.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17/pygmtsar/Stack_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17/pygmtsar/Stack_dem.py
+-rw-r--r--   0 mbg        (501) staff       (20)    44173 2024-02-08 18:53:49.000000 pygmtsar-2024.4.17/pygmtsar/Stack_detrend.py
+-rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17/pygmtsar/Stack_export.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17/pygmtsar/Stack_geocode.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17/pygmtsar/Stack_incidence.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17/pygmtsar/Stack_landmask.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17/pygmtsar/Stack_multilooking.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17/pygmtsar/Stack_orbits.py
+-rw-r--r--   0 mbg        (501) staff       (20)    47295 2024-03-29 07:29:11.000000 pygmtsar-2024.4.17/pygmtsar/Stack_phasediff.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17/pygmtsar/Stack_prm.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17/pygmtsar/Stack_ps.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.4.17/pygmtsar/Stack_reframe.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17/pygmtsar/Stack_reframe_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    46640 2024-04-11 04:05:10.000000 pygmtsar-2024.4.17/pygmtsar/Stack_sbas.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8884 2024-01-01 15:32:51.000000 pygmtsar-2024.4.17/pygmtsar/Stack_stl.py
+-rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17/pygmtsar/Stack_tidal.py
+-rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17/pygmtsar/Stack_topo.py
+-rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17/pygmtsar/Stack_trans.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17/pygmtsar/Stack_trans_inv.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26654 2024-04-11 05:08:11.000000 pygmtsar-2024.4.17/pygmtsar/Stack_unwrap.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17/pygmtsar/Stack_unwrap_snaphu.py
+-rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17/pygmtsar/Tiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.4.17/pygmtsar/XYZTiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17/pygmtsar/_Stack_merge.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1034 2024-04-17 08:18:17.000000 pygmtsar-2024.4.17/pygmtsar/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17/pygmtsar/datagrid.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17/pygmtsar/tqdm_dask.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17/pygmtsar/tqdm_joblib.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17/pygmtsar/utils.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-22 06:47:48.348097 pygmtsar-2024.4.17/pygmtsar.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)    13457 2024-04-22 06:47:48.000000 pygmtsar-2024.4.17/pygmtsar.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-04-22 06:47:48.000000 pygmtsar-2024.4.17/pygmtsar.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2024-04-22 06:47:48.000000 pygmtsar-2024.4.17/pygmtsar.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      330 2024-04-22 06:47:48.000000 pygmtsar-2024.4.17/pygmtsar.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2024-04-22 06:47:48.000000 pygmtsar-2024.4.17/pygmtsar.egg-info/top_level.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       38 2024-04-22 06:47:48.348704 pygmtsar-2024.4.17/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-04-11 03:27:25.000000 pygmtsar-2024.4.17/setup.py
```

### Comparing `pygmtsar-2024.3.15.post8/LICENSE.txt` & `pygmtsar-2024.4.17/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/PKG-INFO` & `pygmtsar-2024.4.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.3.15.post8
+Version: 2024.4.17
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.3.15.post8/README.md` & `pygmtsar-2024.4.17/README.md`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/ASF.py` & `pygmtsar-2024.4.17/pygmtsar/ASF.py`

 * *Files 14% similar despite different names*

```diff
@@ -134,114 +134,14 @@
         #print ('scenes', len(scenes))
         scenes_downloaded = pd.DataFrame(scenes_missed, columns=['scene'])
         # return the results in a user-friendly dataframe
         #scenes_downloaded['scene'] = scenes_downloaded.scene\
         #                             .apply(lambda name: self.template_url.format(satellite=name[2:3], scene=name))
         return scenes_downloaded
 
-    """
-    find . -type f -name '*.tiff' -exec basename {} .tiff \; \
-        | awk -F'-' -v OFS='_' '{print toupper($1), "IW_SLC__1SDV", toupper($5), toupper($6), $7, toupper($8), $9"X.SAFE"}' \
-        | xargs -I {} mkdir -p {}
-    """
-    def download_orbits(self, basedir: str, session=None, n_jobs: int = 8, skip_exist: bool = True):
-        import pandas as pd
-        import requests
-        import os
-        import re
-        import glob
-        from datetime import datetime
-        import asf_search
-        import joblib
-        from tqdm.auto import tqdm
-
-        # create the directory if needed
-        os.makedirs(basedir, exist_ok=True)
-
-        if not skip_exist:
-            orbits = glob.glob('*.EOF', root_dir=basedir)
-            #print ('orbits', orbits)
-            for orbit in orbits:
-                os.remove(os.path.join(basedir, orbit))
-
-        scenes = S1.scan_slc(basedir)
-        scenes = scenes[scenes.orbitpath.isnull()]\
-            .reset_index()\
-            .groupby(['date', 'mission'])\
-            .first()\
-            .reset_index()[['mission', 'datetime']]
-        #print ('scenes', scenes)
-        if len(scenes) == 0:
-            return
-
-        # prepare authorized connection
-        if session is None:
-            session = self._get_asf_session()
-
-        # download orbits
-        orbits_found = []
-        for product_type in ['POEORB', 'RESORB']:
-            # nothing to do
-            if scenes is None or len(scenes) == 0:
-                continue
-
-            url = self.resorb_url if product_type == 'RESORB' else self.poeorb_url
-
-            # get orbits HTML list
-            with tqdm(desc=f'ASF Downloading {product_type} Catalog:', total=1) as pbar:
-                response = session.get(url)
-                pbar.update(1)
-            response.raise_for_status()
-            lines = response.text.splitlines()
-            orbits = [re.search(self.pattern_orbit, line).group(0) if re.search(self.pattern_orbit, line) else None for line in lines]
-            orbits = pd.DataFrame(orbits, columns=['orbit']).dropna()
-            orbits['mission']    = orbits['orbit'].apply(lambda name: name[:3])
-            orbits['time']       = orbits['orbit'].apply(lambda name: datetime.strptime(name.split('_')[5], '%Y%m%dT%H%M%S'))
-            if product_type == 'RESORB':
-                orbits['time_start'] = orbits['orbit'].apply(lambda name: datetime.strptime(name.split('_')[6][1:],  '%Y%m%dT%H%M%S')) + self.offset_start
-                orbits['time_end']   = orbits['orbit'].apply(lambda name: datetime.strptime(name[:-4].split('_')[7], '%Y%m%dT%H%M%S')) - self.offset_end
-            elif product_type == 'POEORB':
-                # use daily orbits
-                orbits['time_start'] = orbits['orbit'].apply(lambda name: datetime.strptime(name.split('_')[6][1:][:9]  + '235959', '%Y%m%dT%H%M%S'))
-                orbits['time_end']   = orbits['orbit'].apply(lambda name: datetime.strptime(name[:-4].split('_')[7][:9] + '000001', '%Y%m%dT%H%M%S'))
-            #print ('orbits', orbits.head(3))
-
-            urls = []
-            scenes_missed = []
-            for scene in scenes.itertuples():
-                #print ('scene', scene)
-                # look for the orbit file
-                orbit = orbits[(orbits.mission == scene.mission)&\
-                               (orbits.time_start <= scene.datetime)&\
-                               (orbits.time_end   >= scene.datetime)].sort_values('time')
-                #print ('orbit', orbit)
-                # add the recent orbit
-                orbit = orbit.tail(1).orbit.item() if len(orbit) >= 1 else None
-                if orbit is None:
-                    scenes_missed.append(scene)
-                else:
-                    urls.append(url + orbit)
-                    orbits_found.append(orbit)
-
-            # this routine can use multiple threads but it does not provide a progress indicator
-            with self.tqdm_joblib(tqdm(desc=f'ASF Downloading {product_type} Orbits:', total=len(orbits_found))) as progress_bar:
-                joblib.Parallel(n_jobs=n_jobs)(joblib.delayed(asf_search.download_urls)(urls=[url], path=basedir, session=session) \
-                                               for url in urls)
-
-            # remove processed scenes
-            if len(scenes_missed) > 0:
-                scenes = pd.DataFrame(scenes_missed)[['mission', 'datetime']]
-            else:
-                scenes = None
-
-        # check for scenes without orbits
-        if scenes is not None and len(scenes) > 0:
-            raise Exception(f'ERROR: missed {len(scenes)} orbits')
-        return pd.Series(orbits_found)
-
     def download(self, *args, **kwarg):
         print ('NOTE: Function is deprecated. Use ASF.download_scenes() and ASF.download_orbits().')
 
     # https://asf.alaska.edu/datasets/data-sets/derived-data-sets/sentinel-1-bursts/
     def download_bursts(self, basedir, bursts, session=None, n_jobs=4, skip_exist=True):
         import rioxarray as rio
         import xmltodict
```

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/AWS.py` & `pygmtsar-2024.4.17/pygmtsar/AWS.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/GMT.py` & `pygmtsar-2024.4.17/pygmtsar/GMT.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/IO.py` & `pygmtsar-2024.4.17/pygmtsar/IO.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/NCubeVTK.py` & `pygmtsar-2024.4.17/pygmtsar/NCubeVTK.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/PRM.py` & `pygmtsar-2024.4.17/pygmtsar/PRM.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/PRM_gmtsar.py` & `pygmtsar-2024.4.17/pygmtsar/PRM_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/S1.py` & `pygmtsar-2024.4.17/pygmtsar/S1.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,19 @@
     orbits_url = 'https://s1orbits.pechnikov.workers.dev/{mission}/{year}/{month:02}/{day:02}/'
     # see _select_orbit.py in sentineleof package
     #Orbital period of Sentinel-1 in seconds
     #T_ORBIT = (12 * 86400.0) / 175.0
     orbit_offset_start = timedelta(seconds=(12 * 86400.0) // 175.0 + 60)
     orbit_offset_end = timedelta(seconds=300)
 
+    """
+    find . -type f -name '*.tiff' -exec basename {} .tiff \; \
+        | awk -F'-' -v OFS='_' '{print toupper($1), "IW_SLC__1SDV", toupper($5), toupper($6), $7, toupper($8), $9"X.SAFE"}' \
+        | xargs -I {} mkdir -p {}
+    """
     @staticmethod
     def download_orbits(basedir: str, scenes: list | pd.DataFrame,
                         n_jobs: int = 8, joblib_backend='loky', skip_exist: bool = True):
         import pandas as pd
         import requests
         import os
         import re
```

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack.py` & `pygmtsar-2024.4.17/pygmtsar/Stack.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_align.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_align.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_base.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_base.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_dem.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_dem.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_detrend.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_detrend.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_export.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_export.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_geocode.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_geocode.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_incidence.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_incidence.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_landmask.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_landmask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_multilooking.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_multilooking.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_orbits.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_orbits.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_phasediff.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_phasediff.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_prm.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_prm.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_ps.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_ps.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_reframe.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_reframe.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_reframe_gmtsar.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_reframe_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_sbas.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_sbas.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_stl.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_stl.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_tidal.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_tidal.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_topo.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_topo.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_trans.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_trans.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_trans_inv.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_trans_inv.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_unwrap.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_unwrap.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Stack_unwrap_snaphu.py` & `pygmtsar-2024.4.17/pygmtsar/Stack_unwrap_snaphu.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/Tiles.py` & `pygmtsar-2024.4.17/pygmtsar/Tiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/XYZTiles.py` & `pygmtsar-2024.4.17/pygmtsar/XYZTiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/_Stack_merge.py` & `pygmtsar-2024.4.17/pygmtsar/_Stack_merge.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/__init__.py` & `pygmtsar-2024.4.17/pygmtsar/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 
 # This file is part of the PyGMTSAR project: https://github.com/mobigroup/gmtsar
 # 
 # Copyright (c) 2023, Alexey Pechnikov
 # 
 # Licensed under the BSD 3-Clause License (see LICENSE for details)
 # ----------------------------------------------------------------------------
-__version__ = '2024.3.15.post8'
+__version__ = '2024.4.17'
 
 # unified progress indicators
 from .tqdm_joblib import tqdm_joblib
 from .tqdm_dask import tqdm_dask
 # base NetCDF operations and parameters on NetCDF grid
 from .datagrid import datagrid
 # top level module classes
@@ -20,15 +20,14 @@
 # Sentinel-1 processing functions
 from .S1 import S1
 # export to VTK format
 from .NCubeVTK import NCubeVTK
 # ASF, AWS, ESA, GMT downloading functions
 from .ASF import ASF
 from .AWS import AWS
-from .ESA import ESA
 from .GMT import GMT
 # tiles downloading
 from .Tiles import Tiles
 # XYZ map tiles downloading
 from .XYZTiles import XYZTiles
 # morphology and other helper functions
 from .utils import utils
```

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/datagrid.py` & `pygmtsar-2024.4.17/pygmtsar/datagrid.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/tqdm_dask.py` & `pygmtsar-2024.4.17/pygmtsar/tqdm_dask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/tqdm_joblib.py` & `pygmtsar-2024.4.17/pygmtsar/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar/utils.py` & `pygmtsar-2024.4.17/pygmtsar/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar.egg-info/PKG-INFO` & `pygmtsar-2024.4.17/pygmtsar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.3.15.post8
+Version: 2024.4.17
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.3.15.post8/pygmtsar.egg-info/SOURCES.txt` & `pygmtsar-2024.4.17/pygmtsar.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE.txt
 README.md
 setup.py
 ../README.md
 pygmtsar/ASF.py
 pygmtsar/AWS.py
-pygmtsar/ESA.py
 pygmtsar/GMT.py
 pygmtsar/IO.py
 pygmtsar/NCubeVTK.py
 pygmtsar/PRM.py
 pygmtsar/PRM_gmtsar.py
 pygmtsar/S1.py
 pygmtsar/Stack.py
```

### Comparing `pygmtsar-2024.3.15.post8/setup.py` & `pygmtsar-2024.4.17/setup.py`

 * *Files identical despite different names*


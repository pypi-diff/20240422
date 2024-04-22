# Comparing `tmp/ocp_vscode-2.3.0.tar.gz` & `tmp/ocp_vscode-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_vscode-2.3.0.tar", last modified: Wed Apr 17 18:24:07 2024, max compression
+gzip compressed data, was "ocp_vscode-2.3.1.tar", last modified: Mon Apr 22 06:43:09 2024, max compression
```

## Comparing `ocp_vscode-2.3.0.tar` & `ocp_vscode-2.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-17 18:24:07.921338 ocp_vscode-2.3.0/
--rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-2.3.0/LICENSE
--rw-r--r--   0 bernhard   (501) staff       (20)      959 2024-04-17 18:24:07.921165 ocp_vscode-2.3.0/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)    12859 2024-04-17 06:53:57.000000 ocp_vscode-2.3.0/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-17 18:24:07.919664 ocp_vscode-2.3.0/ocp_vscode/
--rw-r--r--   0 bernhard   (501) staff       (20)     1281 2024-04-16 19:20:47.000000 ocp_vscode-2.3.0/ocp_vscode/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4972 2024-01-16 17:49:02.000000 ocp_vscode-2.3.0/ocp_vscode/animation.py
--rw-r--r--   0 bernhard   (501) staff       (20)    14216 2024-01-16 17:49:02.000000 ocp_vscode-2.3.0/ocp_vscode/backend.py
--rw-r--r--   0 bernhard   (501) staff       (20)    19453 2024-01-16 17:49:02.000000 ocp_vscode-2.3.0/ocp_vscode/build123d.py
--rw-r--r--   0 bernhard   (501) staff       (20)    19488 2024-01-16 17:49:02.000000 ocp_vscode-2.3.0/ocp_vscode/colors.py
--rw-r--r--   0 bernhard   (501) staff       (20)     8166 2024-04-16 20:13:02.000000 ocp_vscode-2.3.0/ocp_vscode/comms.py
--rw-r--r--   0 bernhard   (501) staff       (20)    16326 2024-04-16 20:13:23.000000 ocp_vscode-2.3.0/ocp_vscode/config.py
--rw-r--r--   0 bernhard   (501) staff       (20)    33098 2024-04-17 06:24:29.000000 ocp_vscode-2.3.0/ocp_vscode/show.py
--rw-r--r--   0 bernhard   (501) staff       (20)     5024 2024-01-16 17:49:02.000000 ocp_vscode-2.3.0/ocp_vscode/state.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-17 18:24:07.920954 ocp_vscode-2.3.0/ocp_vscode.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      959 2024-04-17 18:24:07.000000 ocp_vscode-2.3.0/ocp_vscode.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      479 2024-04-17 18:24:07.000000 ocp_vscode-2.3.0/ocp_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-17 18:24:07.000000 ocp_vscode-2.3.0/ocp_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-17 18:24:07.000000 ocp_vscode-2.3.0/ocp_vscode.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)       78 2024-04-17 18:24:07.000000 ocp_vscode-2.3.0/ocp_vscode.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       11 2024-04-17 18:24:07.000000 ocp_vscode-2.3.0/ocp_vscode.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)     1038 2024-04-17 18:24:07.921631 ocp_vscode-2.3.0/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1227 2024-04-14 16:40:03.000000 ocp_vscode-2.3.0/setup.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-17 18:24:07.920771 ocp_vscode-2.3.0/test/
--rw-r--r--   0 bernhard   (501) staff       (20)      401 2023-11-24 07:13:36.000000 ocp_vscode-2.3.0/test/test_for_backend.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1890 2023-11-24 07:13:36.000000 ocp_vscode-2.3.0/test/testextension.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:43:09.263153 ocp_vscode-2.3.1/
+-rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-2.3.1/LICENSE
+-rw-r--r--   0 bernhard   (501) staff       (20)      959 2024-04-22 06:43:09.263078 ocp_vscode-2.3.1/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)    12982 2024-04-20 11:59:28.000000 ocp_vscode-2.3.1/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:43:09.261775 ocp_vscode-2.3.1/ocp_vscode/
+-rw-r--r--   0 bernhard   (501) staff       (20)     1332 2024-04-20 15:35:45.000000 ocp_vscode-2.3.1/ocp_vscode/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4972 2024-01-16 17:49:02.000000 ocp_vscode-2.3.1/ocp_vscode/animation.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    14216 2024-01-16 17:49:02.000000 ocp_vscode-2.3.1/ocp_vscode/backend.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    19453 2024-01-16 17:49:02.000000 ocp_vscode-2.3.1/ocp_vscode/build123d.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    19488 2024-01-16 17:49:02.000000 ocp_vscode-2.3.1/ocp_vscode/colors.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     8166 2024-04-20 15:33:55.000000 ocp_vscode-2.3.1/ocp_vscode/comms.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    16326 2024-04-16 20:13:23.000000 ocp_vscode-2.3.1/ocp_vscode/config.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    32313 2024-04-20 17:15:29.000000 ocp_vscode-2.3.1/ocp_vscode/show.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     5024 2024-01-16 17:49:02.000000 ocp_vscode-2.3.1/ocp_vscode/state.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:43:09.262883 ocp_vscode-2.3.1/ocp_vscode.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      959 2024-04-22 06:43:09.000000 ocp_vscode-2.3.1/ocp_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      479 2024-04-22 06:43:09.000000 ocp_vscode-2.3.1/ocp_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-22 06:43:09.000000 ocp_vscode-2.3.1/ocp_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-22 06:43:09.000000 ocp_vscode-2.3.1/ocp_vscode.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)       78 2024-04-22 06:43:09.000000 ocp_vscode-2.3.1/ocp_vscode.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       11 2024-04-22 06:43:09.000000 ocp_vscode-2.3.1/ocp_vscode.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)     1038 2024-04-22 06:43:09.263406 ocp_vscode-2.3.1/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1227 2024-04-20 12:06:41.000000 ocp_vscode-2.3.1/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:43:09.262722 ocp_vscode-2.3.1/test/
+-rw-r--r--   0 bernhard   (501) staff       (20)      401 2023-11-24 07:13:36.000000 ocp_vscode-2.3.1/test/test_for_backend.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1890 2023-11-24 07:13:36.000000 ocp_vscode-2.3.1/test/testextension.py
```

### Comparing `ocp_vscode-2.3.0/LICENSE` & `ocp_vscode-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.0/PKG-INFO` & `ocp_vscode-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 2.3.0
+Version: 2.3.1
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -13,14 +13,14 @@
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: ocp-tessellate<2.4.0,>=2.3.0
+Requires-Dist: ocp-tessellate<2.4.0,>=2.3.2
 Requires-Dist: requests
 Requires-Dist: ipykernel
 Requires-Dist: orjson
 Requires-Dist: websockets<11.1,>=11.0
 
 An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via threejs
```

### Comparing `ocp_vscode-2.3.0/README.md` & `ocp_vscode-2.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,18 @@
 ```bash
 NATIVE_TESSELLATOR=0 OCP_VSCODE_PYTEST=1 pytest -v -s pytests/
 NATIVE_TESSELLATOR=1 OCP_VSCODE_PYTEST=1 pytest -v -s pytests/
 ```
 
 ## Changes
 
+v2.3.1
+- Add latest ocp-tessellate to fixed regression with handling instances
+- Make native default if ocp-addons exists
+
 v2.3.0
 - Add newest ocp-tessellate to allow using native tessellator from ocp_addons
 - Fine tune communication to ensure the memory view of buffers will be passed through to javascript for performance
 - Use of the new protocol v3 of three-cad-viewer
 
 v2.2.2
 - Fix regression in measure tools
```

### Comparing `ocp_vscode-2.3.0/ocp_vscode/__init__.py` & `ocp_vscode-2.3.1/ocp_vscode/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.3.0"
+__version__ = "2.3.1"
+
+import os
 
 from .show import *
 from .config import *
 from .comms import *
 
 from .colors import *
 from .animation import Animation
@@ -28,17 +30,19 @@
 try:
     from ocp_tessellate.tessellator import (
         enable_native_tessellator,
         disable_native_tessellator,
         is_native_tessellator_enabled,
     )
 
-    if is_native_tessellator_enabled():
-        print(
-            "Enabled native tessellator, to disable, call `disable_native_tessellator()`\n"
-        )
+    if os.environ.get("NATIVE_TESSELLATOR") == "0":
+        disable_native_tessellator()
     else:
-        print(
-            "Found native tessellator, to ansable, call `enable_native_tessellator()`\n"
-        )
+        enable_native_tessellator()
+
+    print(
+        "Found and enabled native tessellator.\n"
+        "To disable, call `disable_native_tessellator()`\n"
+        "To enable, call `enable_native_tessellator()`\n"
+    )
 except:
     pass
```

### Comparing `ocp_vscode-2.3.0/ocp_vscode/animation.py` & `ocp_vscode-2.3.1/ocp_vscode/animation.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.0/ocp_vscode/backend.py` & `ocp_vscode-2.3.1/ocp_vscode/backend.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.0/ocp_vscode/build123d.py` & `ocp_vscode-2.3.1/ocp_vscode/build123d.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.0/ocp_vscode/colors.py` & `ocp_vscode-2.3.1/ocp_vscode/colors.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.0/ocp_vscode/comms.py` & `ocp_vscode-2.3.1/ocp_vscode/comms.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.0/ocp_vscode/config.py` & `ocp_vscode-2.3.1/ocp_vscode/config.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.0/ocp_vscode/show.py` & `ocp_vscode-2.3.1/ocp_vscode/show.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 from ocp_tessellate import PartGroup
 from ocp_tessellate.convert import (
     tessellate_group,
     get_normal_len,
     combined_bb,
     to_assembly,
-    mp_get_results,
     conv,
 )
 from ocp_tessellate.utils import numpy_to_buffer_json, Timer, Color
 from ocp_tessellate.ocp_utils import (
     is_vector,
     is_topods_shape,
     is_topods_compound,
@@ -38,15 +37,14 @@
     is_cadquery_assembly,
     is_cadquery_sketch,
     is_build123d,
     is_toploc_location,
     is_wrapped,
 )
 
-from ocp_tessellate.mp_tessellator import init_pool, keymap, close_pool
 from ocp_tessellate.cad_objects import (
     OCP_PartGroup,
     OCP_Edges,
     OCP_Faces,
     OCP_Part,
     OCP_Vertices,
 )
@@ -197,38 +195,22 @@
             print(f"Setting {k} can only be set in VSCode config")
 
         elif v is not None:
             if k == "reset_camera" and params.get("_splash") is True:
                 continue
             params[k] = v
 
-    parallel = preset("parallel", params.get("parallel"))
-    if parallel and not any(
-        [isinstance(obj, OCP_PartGroup) for obj in part_group.objects]
-    ):
-        print("parallel only works for assemblies, setting it to False")
-        parallel = False
-        params["parallel"] = False
-
     if kwargs.get("debug") is not None and kwargs["debug"]:
         print("\ntessellation parameters:\n", params)
 
     with Timer(timeit, "", "tessellate", 1):
-        if parallel:
-            init_pool()
-            keymap.reset()
-
         instances, shapes, states, mapping = tessellate_group(
             part_group, instances, params, progress, params.get("timeit")
         )
 
-        if parallel:
-            instances, shapes = mp_get_results(instances, shapes, progress)
-            close_pool()
-
     params["normal_len"] = get_normal_len(
         preset("render_normals", params.get("render_normals")),
         shapes,
         preset("deviation", params.get("deviation")),
     )
 
     with Timer(timeit, "", "bb", 1):
@@ -379,15 +361,14 @@
     roughness=None,
     render_edges=None,
     render_normals=None,
     render_mates=None,
     render_joints=None,
     show_parent=None,
     show_sketch_local=None,
-    parallel=None,
     helper_scale=None,
     mate_scale=None,  # DEPRECATED
     debug=None,
     timeit=None,
     _force_in_debug=False,
 ):
     # pylint: disable=line-too-long
@@ -470,15 +451,14 @@
         metalness:               Metalness property of the default material (default=0.30)
         roughness:               Roughness property of the default material (default=0.65)
 
         render_edges:            Render edges  (default=True)
         render_normals:          Render normals (default=False)
         render_mates:            Render mates for MAssemblies (default=False)
         render_joints:           Render build123d joints (default=False)
-        parallel:                Tessellate objects in parallel (default=False)
         show_parent:             Render parent of faces, edges or vertices as wireframe (default=False)
         show_sketch_local:       In build123d show local sketch in addition to relocate sketch (default=True)
         helper_scale:            Scale of rendered helpers (locations, axis, mates for MAssemblies) (default=1)
 
     - Debug
         debug:                   Show debug statements to the VS Code browser console (default=False)
         timeit:                  Show timing information from level 0-3 (default=False)
@@ -638,15 +618,14 @@
     metalness=None,
     roughness=None,
     direct_intensity=None,
     render_edges=None,
     render_normals=None,
     render_mates=None,
     render_joints=None,
-    parallel=None,
     show_parent=None,
     show_sketch_local=None,
     helper_scale=None,
     mate_scale=None,  # DEPRECATED
     debug=None,
     timeit=None,
 ):
@@ -735,15 +714,14 @@
         roughness:               Roughness property of the default material (default=0.65)
 
 
         render_edges:            Render edges  (default=True)
         render_normals:          Render normals (default=False)
         render_mates:            Render mates for MAssemblies (default=False)
         render_joints:           Render build123d joints (default=False)
-        parallel:                Tessellate objects in parallel (default=False)
         show_parent:             Render parent of faces, edges or vertices as wireframe (default=False)
         show_sketch_local:       In build123d show local sketch in addition to relocate sketch (default=True)
         helper_scale:            Scale of rendered helpers (locations, axis, mates for MAssemblies) (default=1)
 
     - Debug
         debug:                   Show debug statements to the VS Code browser console (default=False)
         imeit:                   Show timing information from level 0-3 (default=False)
```

### Comparing `ocp_vscode-2.3.0/ocp_vscode/state.py` & `ocp_vscode-2.3.1/ocp_vscode/state.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.0/ocp_vscode.egg-info/PKG-INFO` & `ocp_vscode-2.3.1/ocp_vscode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 2.3.0
+Version: 2.3.1
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -13,14 +13,14 @@
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: ocp-tessellate<2.4.0,>=2.3.0
+Requires-Dist: ocp-tessellate<2.4.0,>=2.3.2
 Requires-Dist: requests
 Requires-Dist: ipykernel
 Requires-Dist: orjson
 Requires-Dist: websockets<11.1,>=11.0
 
 An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via threejs
```

### Comparing `ocp_vscode-2.3.0/setup.cfg` & `ocp_vscode-2.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.3.0
+current_version = 2.3.1
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_vscode-2.3.0/setup.py` & `ocp_vscode-2.3.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup_args = {
     "name": "ocp_vscode",
-    "version": "2.3.0",
+    "version": "2.3.1",
     "description": "OCP CAD Viewer for VSCode",
     "long_description": "An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via threejs",
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
-        "ocp-tessellate>=2.3.0,<2.4.0",
+        "ocp-tessellate>=2.3.2,<2.4.0",
         "requests",
         "ipykernel",
         "orjson",
         "websockets>=11.0,<11.1",
     ],
     "packages": find_packages(),
     "zip_safe": False,
```

### Comparing `ocp_vscode-2.3.0/test/testextension.py` & `ocp_vscode-2.3.1/test/testextension.py`

 * *Files identical despite different names*


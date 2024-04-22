# Comparing `tmp/ehdg_pupil_detector-3.3.0.tar.gz` & `tmp/ehdg_pupil_detector-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_pupil_detector-3.3.0.tar", last modified: Thu Apr 18 02:08:38 2024, max compression
+gzip compressed data, was "ehdg_pupil_detector-3.4.0.tar", last modified: Mon Apr 22 05:51:17 2024, max compression
```

## Comparing `ehdg_pupil_detector-3.3.0.tar` & `ehdg_pupil_detector-3.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 02:08:38.038578 ehdg_pupil_detector-3.3.0/
--rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.3.0/LICENSE
--rw-rw-rw-   0        0        0     4075 2024-04-18 02:08:38.037582 ehdg_pupil_detector-3.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.3.0/README.md
--rw-rw-rw-   0        0        0     1162 2024-04-18 02:07:06.000000 ehdg_pupil_detector-3.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 02:08:38.038578 ehdg_pupil_detector-3.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 02:08:38.004427 ehdg_pupil_detector-3.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:08:38.013403 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector/__init__.py
--rw-rw-rw-   0        0        0    23108 2024-04-18 01:34:44.000000 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py
--rw-rw-rw-   0        0        0      260 2024-04-15 01:15:20.000000 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector/opm_detector_config.json
--rw-rw-rw-   0        0        0    19156 2024-04-18 02:03:29.000000 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector/opmtrack.py
--rw-rw-rw-   0        0        0      200 2024-04-17 02:41:31.000000 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector/opmtrack_plot.json
-drwxrwxrwx   0        0        0        0 2024-04-18 02:08:38.036584 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector.egg-info/
--rw-rw-rw-   0        0        0     4075 2024-04-18 02:08:37.000000 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2024-04-18 02:08:38.000000 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 02:08:37.000000 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-18 02:08:37.000000 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2024-04-18 02:08:37.000000 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-18 02:08:37.000000 ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 05:51:17.286776 ehdg_pupil_detector-3.4.0/
+-rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.4.0/LICENSE
+-rw-rw-rw-   0        0        0     4075 2024-04-22 05:51:17.285779 ehdg_pupil_detector-3.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.4.0/README.md
+-rw-rw-rw-   0        0        0     1162 2024-04-22 04:39:44.000000 ehdg_pupil_detector-3.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-22 05:51:17.286776 ehdg_pupil_detector-3.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-22 05:51:17.254814 ehdg_pupil_detector-3.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 05:51:17.261795 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector/__init__.py
+-rw-rw-rw-   0        0        0    23108 2024-04-18 01:34:44.000000 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py
+-rw-rw-rw-   0        0        0      312 2024-04-22 05:49:11.000000 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector/opm_detector_config.json
+-rw-rw-rw-   0        0        0    23473 2024-04-22 05:36:58.000000 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector/opmtrack.py
+-rw-rw-rw-   0        0        0      200 2024-04-17 02:41:31.000000 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector/opmtrack_plot.json
+drwxrwxrwx   0        0        0        0 2024-04-22 05:51:17.283784 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector.egg-info/
+-rw-rw-rw-   0        0        0     4075 2024-04-22 05:51:17.000000 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2024-04-22 05:51:17.000000 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 05:51:17.000000 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-22 05:51:17.000000 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      105 2024-04-22 05:51:17.000000 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-22 05:51:17.000000 ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector.egg-info/top_level.txt
```

### Comparing `ehdg_pupil_detector-3.3.0/LICENSE` & `ehdg_pupil_detector-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.3.0/PKG-INFO` & `ehdg_pupil_detector-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.3.0
+Version: 3.4.0
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0
 Requires-Dist: opencv-python>=4.8.1.78
 Requires-Dist: scipy>=1.11.3
 Requires-Dist: numpy>=1.26.1
 Requires-Dist: commentjson
-Requires-Dist: ehdg_tools>=4.2.1
+Requires-Dist: ehdg_tools>=4.2.2
 Requires-Dist: numpy
 
 # EYE HEALTH DIAGNOSTIC GROUP'S PUPIL DETECTOR (ehdg_pupil_detector)
 This is the python package libray pupil detector created by eye health diagnostic group.
 
 ## Installtion
 ```
```

### Comparing `ehdg_pupil_detector-3.3.0/README.md` & `ehdg_pupil_detector-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.3.0/pyproject.toml` & `ehdg_pupil_detector-3.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "ehdg_pupil_detector"
-version = "3.3.0"
+version = "3.4.0"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for Pupil Detector of Eye Health Diagnostic Group"
 readme = "README.md"
-dependencies = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools>=4.2.1", "numpy"]
+dependencies = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools>=4.2.2", "numpy"]
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
@@ -18,15 +18,15 @@
 opmtrack = "ehdg_pupil_detector.opmtrack:main"
 
 [project.urls]
 "Homepage" = "https://github.com/jtur044/ehdg_pupil_detector"
 "Bug Tracker" = "https://github.com/jtur044/ehdg_pupil_detector/issues"
 
 [build-system]
-requires = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools>=4.2.1", "numpy"]
+requires = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools>=4.2.2", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py` & `ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector/opmtrack.py` & `ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector/opmtrack.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import importlib.metadata
 from importlib.resources import files
 import cv2
 import commentjson
 from ehdg_pupil_detector import ehdg_pupil_detector
 from ehdg_tools.ehdg_buffers import TinyFillBuffer
 from ehdg_tools.ehdg_plotter import raw_plot
+from ehdg_tools.ehdg_functions import string_to_bgr_tuple
 import numpy as np
 
 
 # This function is to get built-in config location with new library (from importlib.resources import files)
 def get_config_location(module_name, config_file_name):
     config_dir = files(module_name).joinpath(config_file_name)
     return str(config_dir)
@@ -53,21 +54,26 @@
     return temp_dict
 
 
 # This function is to redetect with pupil detector by given detector and tiny fill buffer
 # rrt = reflection removal threshold
 def opm_detect(trial_video, out_folder, config_dict, plot_dict,
                buffer_length_input, reflection_removal=True,
-               rrt_lower_limit=0,
-               rrt_upper_limit=255,
+               rrt_lower_limit=0, rrt_upper_limit=255,
                gaussian_blur=True, binary_fill=True,
-               direction_input=None):
-
+               direction_input=None, min_max_circle=True,
+               min_circle_color="green", max_circle_color="orange",
+               pupil_circle_color="red"):
     out_csv_dir = os.path.join(out_folder, "result.csv")
     out_video_dir = os.path.join(out_folder, "result.mp4")
+    min_pupil_size = config_dict["min_pupil_size"]
+    max_pupil_size = config_dict["max_pupil_size"]
+    pupil_circle_color_tuple = string_to_bgr_tuple(pupil_circle_color)
+    min_circle_color_tuple = string_to_bgr_tuple(min_circle_color)
+    max_circle_color_tuple = string_to_bgr_tuple(max_circle_color)
 
     detector = ehdg_pupil_detector.Detector(reflection_removal=reflection_removal,
                                             reflection_removal_lower_limit=rrt_lower_limit,
                                             reflection_removal_upper_limit=rrt_upper_limit,
                                             gaussian_blur=gaussian_blur,
                                             binary_fill_hole=binary_fill)
 
@@ -144,16 +150,55 @@
                 if center_of_pupil != (0, 0):
                     cv2.ellipse(
                         detected_frame,
                         center_of_pupil,
                         (int(major_axis), int(minor_axis)),
                         int(angle_of_pupil),
                         0, 360,  # start/end angle for drawing
-                        (0, 0, 255)  # color (BGR): red
+                        pupil_circle_color_tuple
                     )
+                    if min_max_circle:
+                        cv2.ellipse(
+                            detected_frame,
+                            center_of_pupil,
+                            (int(min_pupil_size), int(min_pupil_size)),
+                            int(angle_of_pupil),
+                            0, 360,  # start/end angle for drawing
+                            min_circle_color_tuple
+                        )
+                        cv2.ellipse(
+                            detected_frame,
+                            center_of_pupil,
+                            (int(max_pupil_size), int(max_pupil_size)),
+                            int(angle_of_pupil),
+                            0, 360,  # start/end angle for drawing
+                            max_circle_color_tuple
+                        )
+                else:
+                    middle_of_width = int(frame_width / 2)
+                    middle_of_height = int(frame_height / 2)
+                    min_max_area = (middle_of_width, middle_of_height)
+                    if min_max_circle:
+                        cv2.ellipse(
+                            detected_frame,
+                            min_max_area,
+                            (int(min_pupil_size), int(min_pupil_size)),
+                            90,
+                            0, 360,  # start/end angle for drawing
+                            min_circle_color_tuple
+                        )
+                        cv2.ellipse(
+                            detected_frame,
+                            min_max_area,
+                            (int(max_pupil_size), int(max_pupil_size)),
+                            90,
+                            0, 360,  # start/end angle for drawing
+                            max_circle_color_tuple
+                        )
+
                 v_writer.write(detected_frame)
 
                 pupil_data = {}
                 pupil_data["x_value"] = x_value
                 pupil_data["y_value"] = y_value
                 pupil_data["major_axis"] = major_axis
                 pupil_data["minor_axis"] = minor_axis
@@ -211,14 +256,21 @@
     parser.add_argument("-rbf", dest="remove_binary_fill_hole", required=False,
                         help="remove binary fill hole", action="store_false")
 
     parser.add_argument("-rrt", dest="reflection_removal_threshold",
                         required=False, default=None, metavar="",
                         help="reflection removal threshold")
 
+    parser.add_argument("-hmmc", dest="hide_min_max_circle", required=False,
+                        help="hide min max circle", action="store_true")
+
+    parser.add_argument("-pmmcc", dest="pupil_min_max_circles_color",
+                        required=False, default=None, metavar="",
+                        help="pupil min max circles color")
+
     args = parser.parse_args()
     input_video = args.input_video
     if input_video is None:
         print("opmtrack needs -i argument to accept input video directory.")
         return
     output_folder = args.output_folder
     if output_folder is None:
@@ -381,15 +433,48 @@
             print(f"There is buffer length input but it is invalid: {buffer_length}.")
             print(f"OPM detector will be using Tiny Fill Buffer with default length:{buffer_length_to_be_used}.")
     else:
         buffer_length_to_be_used = default_buffer_length
         print("There is no buffer length input.")
         print(f"OPM detector will be using Tiny Fill Buffer with default length:{buffer_length_to_be_used}.")
 
+    hide_min_max_circle = args.hide_min_max_circle
+    pupil_min_max_circles_color = args.pupil_min_max_circles_color
+
+    pupil_color_string = "red"
+    min_color_string = "green"
+    max_color_string = "orange"
+    if pupil_min_max_circles_color is not None:
+        if "," in pupil_min_max_circles_color:
+            color_string_array = str(pupil_min_max_circles_color).split(",")
+            if len(color_string_array) == 3:
+                pupil_color_string = color_string_array[0]
+                min_color_string = color_string_array[1]
+                max_color_string = color_string_array[2]
+                print(f"Pupil circle color will be {pupil_color_string}.")
+                print(f"Min circle color will be {min_color_string}.")
+                print(f"Max circle color will be {max_color_string}.")
+            else:
+                print("Invalid pupil_min_max_circles_color input.")
+                print(f"The pupil_min_max_circles_color input : {pupil_min_max_circles_color}.")
+                print("Example input:")
+                print("-pmmcc red,green,orange")
+                return
+        else:
+            print("Invalid pupil_min_max_circles_color input.")
+            print(f"The pupil_min_max_circles_color input : {pupil_min_max_circles_color}.")
+            print("Example input:")
+            print("-pmmcc red,green,orange")
+            return
+
     opm_detect(input_video, output_directory, opm_config_dict, plot_info_dict,
                buffer_length_to_be_used,
                reflection_removal=remove_reflection_removal,
                rrt_lower_limit=lower_limit,
                rrt_upper_limit=upper_limit,
                gaussian_blur=remove_gaussian_blur,
                binary_fill=remove_binary_fill,
-               direction_input=direction_to_be_used)
+               direction_input=direction_to_be_used,
+               min_max_circle=not hide_min_max_circle,
+               min_circle_color=min_color_string,
+               max_circle_color=max_color_string,
+               pupil_circle_color=pupil_color_string)
```

### Comparing `ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector.egg-info/PKG-INFO` & `ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.3.0
+Version: 3.4.0
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0
 Requires-Dist: opencv-python>=4.8.1.78
 Requires-Dist: scipy>=1.11.3
 Requires-Dist: numpy>=1.26.1
 Requires-Dist: commentjson
-Requires-Dist: ehdg_tools>=4.2.1
+Requires-Dist: ehdg_tools>=4.2.2
 Requires-Dist: numpy
 
 # EYE HEALTH DIAGNOSTIC GROUP'S PUPIL DETECTOR (ehdg_pupil_detector)
 This is the python package libray pupil detector created by eye health diagnostic group.
 
 ## Installtion
 ```
```

### Comparing `ehdg_pupil_detector-3.3.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt` & `ehdg_pupil_detector-3.4.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt`

 * *Files identical despite different names*


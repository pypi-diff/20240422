# Comparing `tmp/opencv_wrap-0.1.1.tar.gz` & `tmp/opencv_wrap-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencv_wrap-0.1.1.tar", last modified: Tue Apr 16 04:14:28 2024, max compression
+gzip compressed data, was "opencv_wrap-0.1.2.tar", last modified: Mon Apr 22 02:25:11 2024, max compression
```

## Comparing `opencv_wrap-0.1.1.tar` & `opencv_wrap-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-16 04:14:28.444821 opencv_wrap-0.1.1/
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1069 2024-02-15 08:26:11.000000 opencv_wrap-0.1.1/LICENSE
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)    11136 2024-04-16 04:14:28.444302 opencv_wrap-0.1.1/PKG-INFO
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)    10223 2024-04-16 04:14:27.000000 opencv_wrap-0.1.1/README.rst
-drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-16 04:14:28.420920 opencv_wrap-0.1.1/opencv_wrap/
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)       69 2024-04-15 16:15:05.000000 opencv_wrap-0.1.1/opencv_wrap/__init__.py
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)    13904 2024-04-16 01:51:50.000000 opencv_wrap-0.1.1/opencv_wrap/cv2Decorator.py
-drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-16 04:14:28.436732 opencv_wrap-0.1.1/opencv_wrap/detectors/
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     6262 2024-04-15 22:50:35.000000 opencv_wrap-0.1.1/opencv_wrap/detectors/Face.py
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     4221 2024-04-15 22:50:13.000000 opencv_wrap-0.1.1/opencv_wrap/detectors/Hand.py
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     4198 2024-04-15 22:50:13.000000 opencv_wrap-0.1.1/opencv_wrap/detectors/Pose.py
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)      117 2024-04-15 22:30:48.000000 opencv_wrap-0.1.1/opencv_wrap/detectors/__init__.py
-drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-16 04:14:28.442231 opencv_wrap-0.1.1/opencv_wrap/utils/
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)       19 2024-04-15 16:13:38.000000 opencv_wrap-0.1.1/opencv_wrap/utils/__init__.py
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2217 2024-04-15 22:51:11.000000 opencv_wrap-0.1.1/opencv_wrap/utils/base.py
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)    13236 2024-04-15 20:19:38.000000 opencv_wrap-0.1.1/opencv_wrap/utils/helper.py
-drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-16 04:14:28.429422 opencv_wrap-0.1.1/opencv_wrap.egg-info/
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)    11136 2024-04-16 04:14:28.000000 opencv_wrap-0.1.1/opencv_wrap.egg-info/PKG-INFO
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)      495 2024-04-16 04:14:28.000000 opencv_wrap-0.1.1/opencv_wrap.egg-info/SOURCES.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-04-16 04:14:28.000000 opencv_wrap-0.1.1/opencv_wrap.egg-info/dependency_links.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-04-16 04:07:21.000000 opencv_wrap-0.1.1/opencv_wrap.egg-info/not-zip-safe
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)      982 2024-04-16 04:14:28.000000 opencv_wrap-0.1.1/opencv_wrap.egg-info/requires.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)       12 2024-04-16 04:14:28.000000 opencv_wrap-0.1.1/opencv_wrap.egg-info/top_level.txt
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)       38 2024-04-16 04:14:28.445117 opencv_wrap-0.1.1/setup.cfg
--rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2304 2024-04-16 04:14:27.000000 opencv_wrap-0.1.1/setup.py
+drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-22 02:25:11.822887 opencv_wrap-0.1.2/
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     1069 2024-02-15 08:26:11.000000 opencv_wrap-0.1.2/LICENSE
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)    11395 2024-04-22 02:25:11.822610 opencv_wrap-0.1.2/PKG-INFO
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)    10482 2024-04-22 02:25:10.000000 opencv_wrap-0.1.2/README.rst
+drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-22 02:25:11.802640 opencv_wrap-0.1.2/opencv_wrap/
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)       69 2024-04-15 16:15:05.000000 opencv_wrap-0.1.2/opencv_wrap/__init__.py
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)    13904 2024-04-16 01:51:50.000000 opencv_wrap-0.1.2/opencv_wrap/cv2Decorator.py
+drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-22 02:25:11.815191 opencv_wrap-0.1.2/opencv_wrap/detectors/
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     6262 2024-04-15 22:50:35.000000 opencv_wrap-0.1.2/opencv_wrap/detectors/Face.py
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     4182 2024-04-22 02:16:09.000000 opencv_wrap-0.1.2/opencv_wrap/detectors/Hand.py
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     4336 2024-04-16 06:33:14.000000 opencv_wrap-0.1.2/opencv_wrap/detectors/Pose.py
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)      117 2024-04-15 22:30:48.000000 opencv_wrap-0.1.2/opencv_wrap/detectors/__init__.py
+drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-22 02:25:11.821775 opencv_wrap-0.1.2/opencv_wrap/utils/
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)       19 2024-04-15 16:13:38.000000 opencv_wrap-0.1.2/opencv_wrap/utils/__init__.py
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2217 2024-04-15 22:51:11.000000 opencv_wrap-0.1.2/opencv_wrap/utils/base.py
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)    13236 2024-04-15 20:19:38.000000 opencv_wrap-0.1.2/opencv_wrap/utils/helper.py
+drwxrwxrwx   0 rishi     (1000) rishi     (1000)        0 2024-04-22 02:25:11.808053 opencv_wrap-0.1.2/opencv_wrap.egg-info/
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)    11395 2024-04-22 02:25:11.000000 opencv_wrap-0.1.2/opencv_wrap.egg-info/PKG-INFO
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)      495 2024-04-22 02:25:11.000000 opencv_wrap-0.1.2/opencv_wrap.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-04-22 02:25:11.000000 opencv_wrap-0.1.2/opencv_wrap.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)        1 2024-04-16 04:07:21.000000 opencv_wrap-0.1.2/opencv_wrap.egg-info/not-zip-safe
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)      982 2024-04-22 02:25:11.000000 opencv_wrap-0.1.2/opencv_wrap.egg-info/requires.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)       12 2024-04-22 02:25:11.000000 opencv_wrap-0.1.2/opencv_wrap.egg-info/top_level.txt
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)       38 2024-04-22 02:25:11.822997 opencv_wrap-0.1.2/setup.cfg
+-rwxrwxrwx   0 rishi     (1000) rishi     (1000)     2304 2024-04-22 02:25:10.000000 opencv_wrap-0.1.2/setup.py
```

### Comparing `opencv_wrap-0.1.1/LICENSE` & `opencv_wrap-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.1.1/PKG-INFO` & `opencv_wrap-0.1.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: opencv_wrap
-Version: 0.1.1
-Summary: Working with opencv can be quite a hussel, a lot of boiler code, nested functions for specific use cases, this package is designed to make it easier to work with opencv, while focusing on the main task in hand. best for prototyping and quick testing. second part is speed and performance, this package is designed to be fast and efficient.
-Home-page: https://github.com/rishi23root/opencv_wrap
-Author: rishi23root
-Author-email: rishi23root@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-License-File: LICENSE
-
 opencv_wrap
 ===========
 
 A collection of decorators for opencv and helper functions for multiple
 opencv tasks.
 
 Working with opencv can be quite a hussel, a lot of boiler code, nested
@@ -262,14 +244,19 @@
        kwargs["detected"] = [clipImage(mainFrameCopy, i) for i in face_coordinate]
        show_all_frames(kwargs, keysToShow=["frame", "detected"])
        return kwargs
 
 
    kwargs = all_actions()
 
+.. figure:: https://rishi23root.github.io/opencv_wrap/static/Screenshot-20240422075128-1152x666.png
+   :alt: image
+
+   image
+
 ..
 
    **Example 3** : Reading video and detecting Pose in each frame
 
 .. code:: python
 
    @cv2Decorator.DetectInEachFrame(
@@ -293,14 +280,19 @@
        kwargs["detected"] = [clipImage(mainFrameCopy, i) for i in face_coordinate]
        show_all_frames(kwargs, keysToShow=["frame", "detected"])
        return kwargs
 
 
    all_actions()
 
+.. figure:: https://rishi23root.github.io/opencv_wrap/static/Screenshot%20from%202024-04-22%2007-42-13.png
+   :alt: image
+
+   image
+
 ..
 
    **Example 4** : Reading video and saving each frame in a folder
 
 .. code:: python
 
    from opencv_wrap import cv2Decorator
@@ -354,9 +346,7 @@
    :target: https://pypi.org/project/opencv_wrap/
 .. |GitHub| image:: https://img.shields.io/github/license/rishi23root/opencv_wrap.svg
    :target: https://github.com/rishi23root/opencv_wrap/blob/master/LICENSE
 .. |PyPI - Python Version| image:: https://img.shields.io/pypi/pyversions/Django.svg
 .. |Say Thanks!| image:: https://img.shields.io/badge/Say%20Thanks-:D-1EAEDB.svg
    :target: https://saythanks.io/to/rishi23root
 .. |image| image:: https://rishi23root.github.io/opencv_wrap/static/Screenshot-20240416071956-1175x661.png
-
-
```

### Comparing `opencv_wrap-0.1.1/README.rst` & `opencv_wrap-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: opencv_wrap
+Version: 0.1.2
+Summary: Working with opencv can be quite a hussel, a lot of boiler code, nested functions for specific use cases, this package is designed to make it easier to work with opencv, while focusing on the main task in hand. best for prototyping and quick testing. second part is speed and performance, this package is designed to be fast and efficient.
+Home-page: https://github.com/rishi23root/opencv_wrap
+Author: rishi23root
+Author-email: rishi23root@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+
 opencv_wrap
 ===========
 
 A collection of decorators for opencv and helper functions for multiple
 opencv tasks.
 
 Working with opencv can be quite a hussel, a lot of boiler code, nested
@@ -244,14 +262,19 @@
        kwargs["detected"] = [clipImage(mainFrameCopy, i) for i in face_coordinate]
        show_all_frames(kwargs, keysToShow=["frame", "detected"])
        return kwargs
 
 
    kwargs = all_actions()
 
+.. figure:: https://rishi23root.github.io/opencv_wrap/static/Screenshot-20240422075128-1152x666.png
+   :alt: image
+
+   image
+
 ..
 
    **Example 3** : Reading video and detecting Pose in each frame
 
 .. code:: python
 
    @cv2Decorator.DetectInEachFrame(
@@ -275,14 +298,19 @@
        kwargs["detected"] = [clipImage(mainFrameCopy, i) for i in face_coordinate]
        show_all_frames(kwargs, keysToShow=["frame", "detected"])
        return kwargs
 
 
    all_actions()
 
+.. figure:: https://rishi23root.github.io/opencv_wrap/static/Screenshot%20from%202024-04-22%2007-42-13.png
+   :alt: image
+
+   image
+
 ..
 
    **Example 4** : Reading video and saving each frame in a folder
 
 .. code:: python
 
    from opencv_wrap import cv2Decorator
@@ -336,7 +364,9 @@
    :target: https://pypi.org/project/opencv_wrap/
 .. |GitHub| image:: https://img.shields.io/github/license/rishi23root/opencv_wrap.svg
    :target: https://github.com/rishi23root/opencv_wrap/blob/master/LICENSE
 .. |PyPI - Python Version| image:: https://img.shields.io/pypi/pyversions/Django.svg
 .. |Say Thanks!| image:: https://img.shields.io/badge/Say%20Thanks-:D-1EAEDB.svg
    :target: https://saythanks.io/to/rishi23root
 .. |image| image:: https://rishi23root.github.io/opencv_wrap/static/Screenshot-20240416071956-1175x661.png
+
+
```

### Comparing `opencv_wrap-0.1.1/opencv_wrap/cv2Decorator.py` & `opencv_wrap-0.1.2/opencv_wrap/cv2Decorator.py`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.1.1/opencv_wrap/detectors/Face.py` & `opencv_wrap-0.1.2/opencv_wrap/detectors/Face.py`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.1.1/opencv_wrap/detectors/Hand.py` & `opencv_wrap-0.1.2/opencv_wrap/detectors/Hand.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+# flake8: noqa: E501
 import mediapipe as mp
 from opencv_wrap.utils import DetectorClass
 from opencv_wrap.utils.helper import detectionBox
 
 
 mp_hands = mp.solutions.hands
 mp_drawing = mp.solutions.drawing_utils
 
 
 class HandDetector(DetectorClass):
 
     def __init__(
         self,
-        max_num_hands=2,
+        max_num_hands=10,
         min_detection_confidence=0.5,
         min_tracking_confidence=0.5,
         verbose=False,
     ):
         if self._detector is None:
             self.hands = mp_hands.Hands(
                 max_num_hands=max_num_hands,
@@ -34,22 +35,21 @@
 
         Returns
         -------
         landmarks
             output of hands.process function
         """
         return self.hands.process(frame)
-    
 
     def getDetectionBox(self, processedFrame, frame, padding_ratio=0.2, draw=False):
         """return the detected box from the processed frame, here face
 
         Parameters
         ----------
-        processedFrame : 
+        processedFrame :
             output of processFrame function
         frame : np.array
             frame to draw the box on
         padding_ratio : float, optional
             padding ratio for the box, by default 0.2
         draw : bool, optional
             draw the box on the frame, by default False
@@ -88,45 +88,44 @@
                 cy_max += padding_y
 
                 # check if the box is within the frame from the given coordinates
                 cx_min = max(0, cx_min)
                 cy_min = max(0, cy_min)
                 cx_max = min(w, cx_max)
                 cy_max = min(h, cy_max)
-                
 
                 hand_boxes.append((cx_min, cy_min, cx_max - cx_min, cy_max - cy_min))
 
         if draw:
             detectionBox(detectedArr=hand_boxes, frame=frame)
 
         return hand_boxes
 
     def getLandmarks(self, processedFrame, frame, draw=False):
         """return the detected landmarks from the processed frame, here face
 
         Parameters
         ----------
-        processedFrame : 
+        processedFrame :
             output of processFrame function
         frame : np.array
             frame to draw the landmarks on
         draw : bool, optional
             draw the landmarks on the frame, by default False
 
         Returns
         -------
         list
             list of landmarks
         """
         if processedFrame.multi_hand_landmarks and draw:
             for hand_landmarks in processedFrame.multi_hand_landmarks:
-                    mp_drawing.draw_landmarks(
-                        frame,
-                        hand_landmarks,
-                        mp_hands.HAND_CONNECTIONS)
+                mp_drawing.draw_landmarks(
+                    frame, hand_landmarks, mp_hands.HAND_CONNECTIONS
+                )
 
         return processedFrame.multi_hand_landmarks
 
+
 if __name__ == "__main__":
     HandDetector()
-    pass
+    pass
```

### Comparing `opencv_wrap-0.1.1/opencv_wrap/detectors/Pose.py` & `opencv_wrap-0.1.2/opencv_wrap/detectors/Pose.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+# flake8: noqa: E501
+
 import mediapipe as mp
 from opencv_wrap.utils import DetectorClass
 from opencv_wrap.utils.helper import detectionBox
 
 mp_drawing = mp.solutions.drawing_utils
 mp_drawing_styles = mp.solutions.drawing_styles
 mp_pose = mp.solutions.pose
 
 
-# have to test with multiple people in the frame
+# tested with multiple people in the frame, not working
+# 1. use yolo to detect the person in the frame
+# 2. crop the person from the frame
+# 3. use pose detection on the cropped frame
+
 
 class PoseDetector(DetectorClass):
 
     def __init__(
         self,
         min_detection_confidence=0.5,
         min_tracking_confidence=0.5,
@@ -34,21 +40,21 @@
 
         Returns
         -------
         landmarks
             output of pose.process function
         """
         return self.pose.process(frame)
-    
+
     def getDetectionBox(self, processedFrame, frame, padding_ratio=0.2, draw=False):
         """return the detected box from the processed frame, here pose
 
         Parameters
         ----------
-        processedFrame : 
+        processedFrame :
             output of processFrame function
         frame : np.array
             frame to draw the box on
         padding_ratio : float, optional
             padding ratio for the box, by default 0.2
         draw : bool, optional
             draw the box on the frame, by default False
@@ -91,27 +97,25 @@
             cx_min = max(0, cx_min)
             cy_min = max(0, cy_min)
             cx_max = min(w, cx_max)
             cy_max = min(h, cy_max)
 
             pose_box.append((cx_min, cy_min, cx_max - cx_min, cy_max - cy_min))
 
-
-            
         if draw:
             detectionBox(detectedArr=pose_box, frame=frame)
-        
+
         return pose_box
 
     def getLandmarks(self, processedFrame, frame, draw=False):
         """return the detected landmarks from the processed frame, here pose
 
         Parameters
         ----------
-        processedFrame : 
+        processedFrame :
             output of processFrame function
         frame : np.array
             frame to draw the landmarks on
         draw : bool, optional
             draw the landmarks on the frame, by default False
 
         Returns
@@ -120,15 +124,16 @@
             list of landmarks
         """
         # Implementation for landmark extraction for body pose detection
         mp_drawing.draw_landmarks(
             frame,
             processedFrame.pose_landmarks,
             mp_pose.POSE_CONNECTIONS,
-            landmark_drawing_spec=mp_drawing_styles.get_default_pose_landmarks_style()
+            landmark_drawing_spec=mp_drawing_styles.get_default_pose_landmarks_style(),
         )
 
         return processedFrame.pose_landmarks
 
+
 if __name__ == "__main__":
     PoseDetector()
     pass
```

### Comparing `opencv_wrap-0.1.1/opencv_wrap/utils/base.py` & `opencv_wrap-0.1.2/opencv_wrap/utils/base.py`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.1.1/opencv_wrap/utils/helper.py` & `opencv_wrap-0.1.2/opencv_wrap/utils/helper.py`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.1.1/opencv_wrap.egg-info/PKG-INFO` & `opencv_wrap-0.1.2/opencv_wrap.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencv-wrap
-Version: 0.1.1
+Version: 0.1.2
 Summary: Working with opencv can be quite a hussel, a lot of boiler code, nested functions for specific use cases, this package is designed to make it easier to work with opencv, while focusing on the main task in hand. best for prototyping and quick testing. second part is speed and performance, this package is designed to be fast and efficient.
 Home-page: https://github.com/rishi23root/opencv_wrap
 Author: rishi23root
 Author-email: rishi23root@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -262,14 +262,19 @@
        kwargs["detected"] = [clipImage(mainFrameCopy, i) for i in face_coordinate]
        show_all_frames(kwargs, keysToShow=["frame", "detected"])
        return kwargs
 
 
    kwargs = all_actions()
 
+.. figure:: https://rishi23root.github.io/opencv_wrap/static/Screenshot-20240422075128-1152x666.png
+   :alt: image
+
+   image
+
 ..
 
    **Example 3** : Reading video and detecting Pose in each frame
 
 .. code:: python
 
    @cv2Decorator.DetectInEachFrame(
@@ -293,14 +298,19 @@
        kwargs["detected"] = [clipImage(mainFrameCopy, i) for i in face_coordinate]
        show_all_frames(kwargs, keysToShow=["frame", "detected"])
        return kwargs
 
 
    all_actions()
 
+.. figure:: https://rishi23root.github.io/opencv_wrap/static/Screenshot%20from%202024-04-22%2007-42-13.png
+   :alt: image
+
+   image
+
 ..
 
    **Example 4** : Reading video and saving each frame in a folder
 
 .. code:: python
 
    from opencv_wrap import cv2Decorator
```

### Comparing `opencv_wrap-0.1.1/opencv_wrap.egg-info/requires.txt` & `opencv_wrap-0.1.2/opencv_wrap.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `opencv_wrap-0.1.1/setup.py` & `opencv_wrap-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # flake8: noqa: E501
 from setuptools import setup, find_packages
 
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 DESCRIPTION = "Working with opencv can be quite a hussel, a lot of boiler code, nested functions for specific use cases, this package is designed to make it easier to work with opencv, while focusing on the main task in hand. best for prototyping and quick testing. second part is speed and performance, this package is designed to be fast and efficient."
 
 setup(
     name="opencv_wrap",
     version=VERSION,
     description=DESCRIPTION,
     long_description=open("README.rst").read(),
```


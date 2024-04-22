# Comparing `tmp/dem_roughness_calculator-1.0.5.tar.gz` & `tmp/dem_roughness_calculator-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dem_roughness_calculator-1.0.5.tar", last modified: Sun Apr 21 21:30:48 2024, max compression
+gzip compressed data, was "dem_roughness_calculator-1.0.7.tar", last modified: Mon Apr 22 09:22:56 2024, max compression
```

## Comparing `dem_roughness_calculator-1.0.5.tar` & `dem_roughness_calculator-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:48.629492 dem_roughness_calculator-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 21:30:40.000000 dem_roughness_calculator-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-21 21:30:48.629492 dem_roughness_calculator-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-21 21:30:40.000000 dem_roughness_calculator-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:48.629492 dem_roughness_calculator-1.0.5/dem_roughness_calculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-21 21:30:48.000000 dem_roughness_calculator-1.0.5/dem_roughness_calculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-21 21:30:48.000000 dem_roughness_calculator-1.0.5/dem_roughness_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 21:30:48.000000 dem_roughness_calculator-1.0.5/dem_roughness_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-21 21:30:48.000000 dem_roughness_calculator-1.0.5/dem_roughness_calculator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-21 21:30:48.000000 dem_roughness_calculator-1.0.5/dem_roughness_calculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 21:30:48.000000 dem_roughness_calculator-1.0.5/dem_roughness_calculator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:48.629492 dem_roughness_calculator-1.0.5/roughness_calculator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:40.000000 dem_roughness_calculator-1.0.5/roughness_calculator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:48.629492 dem_roughness_calculator-1.0.5/roughness_calculator/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:40.000000 dem_roughness_calculator-1.0.5/roughness_calculator/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13925 2024-04-21 21:30:40.000000 dem_roughness_calculator-1.0.5/roughness_calculator/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    24761 2024-04-21 21:30:41.000000 dem_roughness_calculator-1.0.5/roughness_calculator/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-21 21:30:41.000000 dem_roughness_calculator-1.0.5/roughness_calculator/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    19897 2024-04-21 21:30:41.000000 dem_roughness_calculator-1.0.5/roughness_calculator/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-21 21:30:41.000000 dem_roughness_calculator-1.0.5/roughness_calculator/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 21:30:48.629492 dem_roughness_calculator-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-21 21:30:41.000000 dem_roughness_calculator-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:48.629492 dem_roughness_calculator-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 21:30:41.000000 dem_roughness_calculator-1.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-21 21:30:41.000000 dem_roughness_calculator-1.0.5/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:22:56.271421 dem_roughness_calculator-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 09:22:48.000000 dem_roughness_calculator-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-22 09:22:56.271421 dem_roughness_calculator-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-22 09:22:48.000000 dem_roughness_calculator-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:22:56.271421 dem_roughness_calculator-1.0.7/dem_roughness_calculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-22 09:22:56.000000 dem_roughness_calculator-1.0.7/dem_roughness_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 09:22:56.000000 dem_roughness_calculator-1.0.7/dem_roughness_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:22:56.000000 dem_roughness_calculator-1.0.7/dem_roughness_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-22 09:22:56.000000 dem_roughness_calculator-1.0.7/dem_roughness_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-22 09:22:56.000000 dem_roughness_calculator-1.0.7/dem_roughness_calculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 09:22:56.000000 dem_roughness_calculator-1.0.7/dem_roughness_calculator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:22:56.271421 dem_roughness_calculator-1.0.7/roughness_calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:22:48.000000 dem_roughness_calculator-1.0.7/roughness_calculator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:22:56.271421 dem_roughness_calculator-1.0.7/roughness_calculator/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:22:48.000000 dem_roughness_calculator-1.0.7/roughness_calculator/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13925 2024-04-22 09:22:48.000000 dem_roughness_calculator-1.0.7/roughness_calculator/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24761 2024-04-22 09:22:48.000000 dem_roughness_calculator-1.0.7/roughness_calculator/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-22 09:22:48.000000 dem_roughness_calculator-1.0.7/roughness_calculator/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21807 2024-04-22 09:22:48.000000 dem_roughness_calculator-1.0.7/roughness_calculator/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-22 09:22:48.000000 dem_roughness_calculator-1.0.7/roughness_calculator/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:22:56.271421 dem_roughness_calculator-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-22 09:22:48.000000 dem_roughness_calculator-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:22:56.271421 dem_roughness_calculator-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:22:48.000000 dem_roughness_calculator-1.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-22 09:22:48.000000 dem_roughness_calculator-1.0.7/tests/test_application_driver.py
```

### Comparing `dem_roughness_calculator-1.0.5/LICENSE` & `dem_roughness_calculator-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.0.5/PKG-INFO` & `dem_roughness_calculator-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dem-roughness-calculator
-Version: 1.0.5
+Version: 1.0.7
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/dem-roughness-calculator
 Author: lbatschelet
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dem_roughness_calculator-1.0.5/dem_roughness_calculator.egg-info/PKG-INFO` & `dem_roughness_calculator-1.0.7/dem_roughness_calculator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dem-roughness-calculator
-Version: 1.0.5
+Version: 1.0.7
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/dem-roughness-calculator
 Author: lbatschelet
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dem_roughness_calculator-1.0.5/dem_roughness_calculator.egg-info/SOURCES.txt` & `dem_roughness_calculator-1.0.7/dem_roughness_calculator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.0.5/roughness_calculator/classes/application_driver.py` & `dem_roughness_calculator-1.0.7/roughness_calculator/classes/application_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 application_driver.py
 ---------------------
-Version: 1.0.5
+Version: 1.0.7
 Author: Lukas Batschelet
-Date: 21.04.2024
+Date: 22.04.2024
 ---------------------
 This module contains the ApplicationDriver class which is responsible for running the application.
 It acts as a sort of interface between the calling User Interface (UI) and the GeoTIFFProcessor class.
 This enables the separation of concerns and allows for easier testing and maintenance of the code.
 (i.e. the UI does not need to know how the processing is done, it just needs to know how to call the processing.)
 """
 from typing import List, Optional, Union
```

### Comparing `dem_roughness_calculator-1.0.5/roughness_calculator/classes/geo_tiff_processor.py` & `dem_roughness_calculator-1.0.7/roughness_calculator/classes/geo_tiff_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 geo_tiff_processor.py
 ---------------------
-Version: 1.0.5
+Version: 1.0.7
 Author: Lukas Batschelet
-Date: 21.04.2024
+Date: 22.04.2024
 ---------------------
 This module contains the GeoTIFFProcessor class which is responsible for processing GeoTIFF files.
 It provides methods for loading, processing, and saving GeoTIFF files.
 Until now, only a method to calculate the roughness of a GeoTIFF file has been implemented.
 """
 import numpy as np
 import rasterio
```

### Comparing `dem_roughness_calculator-1.0.5/roughness_calculator/gui_main.py` & `dem_roughness_calculator-1.0.7/roughness_calculator/gui_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 gui_main.py
 -----------
-Version: 1.0.5
+Version: 1.0.7
 Author: Lukas Batschelet
-Date: 21.04.2024
+Date: 22.04.2024
 -----------
 This module contains the ApplicationGUI class which is
 responsible for creating the graphical user interface (GUI) of the application.
 """
 from PIL import Image, ImageTk
 
 from roughness_calculator.classes.application_driver import ApplicationDriver
@@ -152,17 +152,29 @@
             Label(self.image_frame, text="Processed Image (Pseudo-colored for Visualization):",
                   font=("Helvetica", 10)).grid(
                 row=0, column=0, sticky="w")
             self.image_label = Label(self.image_frame, borderwidth=2, relief="groove")
             self.image_label.grid(row=1, column=0, sticky="nsew", padx=5, pady=5)
             self.image_frame.grid_columnconfigure(0, weight=1)  # Ensure the image frame takes up full width
 
-            self.save_button = Button(self.master, text="Save Processed Image", command=self.save_image,
+            # Create a frame for the buttons
+            button_frame = Frame(self.master)
+            button_frame.grid(row=5, column=0, pady=20, sticky="ew")
+
+            # Now place buttons inside this frame
+            self.help_button = Button(button_frame, text="Help", command=self.show_help)
+            self.help_button.grid(row=0, column=0, padx=5, sticky="ew")
+
+            self.save_button = Button(button_frame, text="Save Processed Image", command=self.save_image,
                                       state='disabled')
-            self.save_button.grid(row=5, column=0, pady=20, sticky="ew")
+            self.save_button.grid(row=0, column=1, padx=5, sticky="ew")
+
+            # Configure the button frame column weights if necessary
+            button_frame.grid_columnconfigure(0, weight=1)
+            button_frame.grid_columnconfigure(1, weight=1)
         except Exception as e:
             # Log the error and raise the original exception
             logging.error("Error setting up the GUI: " + str(e))
             raise RuntimeError("Error setting up the GUI: " + str(e))
 
     def load_input(self) -> None:
         """
@@ -423,14 +435,52 @@
             # Configure the row of the image label to use the calculated height
             self.image_frame.grid_rowconfigure(1, minsize=new_height)
         except Exception as e:
             # Log the error and raise the original exception
             logging.error("Error adjusting image label height: " + str(e))
             raise RuntimeError("Error adjusting image label height: " + str(e))
 
+    def show_help(self):
+        help_text = """
+        DEM Roughness Calculator Help:
+
+
+        Input TIFF Path:
+        Path to the input GeoTIFF file.
+        
+        
+        Output Directory:
+        Directory where the output files will be saved.
+        (Optional, if not set you can choose to save the processed image after previewing it.)
+
+        Window Size (m):
+        Defines the size of the square window in meters to calculate roughness. 
+        (Optional, default is 1.0)
+        
+        
+        Band Number:
+        Specifies the band of the GeoTIFF to be processed.
+        (Optional, default is 1, only different in rare cases where the GeoTIFF has multiple bands including a DEM)
+        
+        
+        High Value Threshold:
+        Sets the threshold above which values are considered as noise and set to nodata.
+        (Optional, default is 1.0, should often be lower, rarely higher)
+        
+        
+        Categorical Thresholds:
+        Comma-separated thresholds for categorizing the roughness values.
+        (Optional, default is None. Grouping roughness values into categories can help in visualizing the data.)
+
+
+        For more detailed information, visit the GitHub wiki at:
+        https://github.com/lbatschelet/dem-roughness-calculator/wiki
+        """
+        messagebox.showinfo("Help", help_text)
+
 
 def main():
     root = tk.Tk()
     app = ApplicationGUI(root)
     root.mainloop()
```

### Comparing `dem_roughness_calculator-1.0.5/roughness_calculator/log_config.py` & `dem_roughness_calculator-1.0.7/roughness_calculator/log_config.py`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.0.5/setup.py` & `dem_roughness_calculator-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='dem-roughness-calculator',
-    version='1.0.5',
+    version='1.0.7',
     packages=find_packages(),  # Automatically find all packages in the directory
     url='https://github.com/lbatschelet/dem-roughness-calculator',
     license='GPL-3.0',
     author='lbatschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     install_requires=requirements,  # Install dependencies from requirements.txt
     python_requires='>=3.12',  # Specify Python version requirement
```


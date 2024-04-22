# Comparing `tmp/phope-0.0.7.tar.gz` & `tmp/phope-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phope-0.0.7.tar", last modified: Mon Aug 28 08:15:42 2023, max compression
+gzip compressed data, was "phope-0.0.8.tar", last modified: Mon Apr 22 07:41:01 2024, max compression
```

## Comparing `phope-0.0.7.tar` & `phope-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-28 08:15:42.127435 phope-0.0.7/
--rw-r--r--   0 yt        (1000) yt        (1000)     3147 2023-08-28 08:15:42.127435 phope-0.0.7/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     2637 2023-02-28 00:29:29.000000 phope-0.0.7/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-08-28 08:15:42.128434 phope-0.0.7/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      921 2023-08-28 08:14:56.000000 phope-0.0.7/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-28 08:15:42.123414 phope-0.0.7/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-28 08:15:42.126433 phope-0.0.7/src/phope.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     3147 2023-08-28 08:15:41.000000 phope-0.0.7/src/phope.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      199 2023-08-28 08:15:41.000000 phope-0.0.7/src/phope.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-08-28 08:15:41.000000 phope-0.0.7/src/phope.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-08-28 08:15:41.000000 phope-0.0.7/src/phope.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        6 2023-08-28 08:15:41.000000 phope-0.0.7/src/phope.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     2414 2023-08-28 08:14:08.000000 phope-0.0.7/src/phope.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:41:01.269370 phope-0.0.8/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4139 2024-04-22 07:41:01.269370 phope-0.0.8/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     3627 2024-04-22 07:37:54.000000 phope-0.0.8/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 07:41:01.269370 phope-0.0.8/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      923 2024-04-22 07:39:56.000000 phope-0.0.8/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:41:01.269370 phope-0.0.8/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-04-22 07:41:01.269370 phope-0.0.8/src/phope.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4139 2024-04-22 07:41:01.000000 phope-0.0.8/src/phope.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      199 2024-04-22 07:41:01.000000 phope-0.0.8/src/phope.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-04-22 07:41:01.000000 phope-0.0.8/src/phope.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-04-22 07:41:01.000000 phope-0.0.8/src/phope.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        6 2024-04-22 07:41:01.000000 phope-0.0.8/src/phope.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2414 2023-08-28 08:14:08.000000 phope-0.0.8/src/phope.py
```

### Comparing `phope-0.0.7/PKG-INFO` & `phope-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,86 @@
 Metadata-Version: 2.1
 Name: phope
-Version: 0.0.7
+Version: 0.0.8
 Summary: universal biomarker prediction tool
-Home-page: https://github.com/ytakefuji/patient
+Home-page: https://github.com/y-takefuji/patient
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/patient
+Project-URL: Bug Tracker, https://github.com/y-takefuji/patient
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # patient
 This is under review.
 
 Patients need to know effects of medication and exercise for alleviating diseases. 
 Biomarkers are used to monitor the status of individual diseases.
 
 phope.py (Patient for Hospital Observation and Predicting Effects of medication and exercise)
-with five determinants such as "day" (tested date), "hgb" of hbA1c value (biomarker for diabetes), "ntbnp" of NT-proBNP value (biomarker for heart failure), "degree1" (polynomial regression for hbA1c), and "degree2" (polynomial regression for NT-proBNP) is a universal biomarker prediction tool that can be used for evaluating the performance and predicting values of biomarkers in the next hospital visit.
+with five determinants such as "day" (tested date), "hgb" of hbA1c value (biomarker for diabetes), "ntbnp" of NT-proBNP value (biomarker for heart failure), "degree1" (polynomial regression for hbA1c), and "degree2" (polynomial regression for NT-proBNP) is a universal biomarker prediction tool that can be used for evaluating the performance and predicting values of biomarkers for the next hospital visit.
 
 To run phope.py after creating a data.csv, type python phope.py in the terminal.
+The following table is an example of data.csv. 
+2023/4/10 is the date of the next hospital visit.
 
-In phope.py, you can change it for your use.
+# An example of data.csv for phope.py
+<img src="https://github.com/y-takefuji/patient/raw/main/datacsv.png" height=120 width=480>
 
-phope is a PyPI application. phope allows users to run on Windows, MacOS, and Linux operating systems as long as Python is installed on the system. phope can set left vertical axis and right vertical axis of two biomakers with data.csv.
+In phope.py, you can change Python codes for your use.
 
-data.csv is a data file composed of seven determinants such as "day" (tested date), "hgb" of hbA1c value (biomarker for diabetes), "ntbnp" of NT-proBNP value (biomarker for heart failure), "degree1" (polynomial regression for hbA1c), "degree2" (polynomial regression for NT-proBNP), the first vertical-axis range on left side (low and high), and the second vertical-axis range on right side (low and high).
+phope was developed based on phope.py 
+which is a PyPI universal biomarker prediction tool with data.csv. 
+PyPI allows phope to run on Windows, MacOS, and Linux operating systems 
+as long as Python is installed on the system. 
+phope can set left vertical axis and right vertical axis of two biomakers with data.csv.
 
-The data.csv file must be created by the patient or physician before running the program.
+data.csv for phope is a data file composed of seven determinants such as "day" (tested date), "hbA1c" value (biomarker for diabetes), "NT-proBNP" value (biomarker for heart failure), "degree1" (polynomial regression for hbA1c), "degree2" (polynomial regression for NT-proBNP), the left vertical-axis range (low and high), and the right vertical-axis range (low and high).
 
-<img src="https://github.com/ytakefuji/patient/raw/main/fig.png" height=90 width=400>
+The data.csv file must be created by the patient or physician before running the program as shown in the following table.
+
+# An example of data.csv for phope
+<img src="https://github.com/y-takefuji/patient/raw/main/fig.png" height=120 width=480>
 
 phope allows users to modify two biomarker's names such as hbA1c and NT-proBNP in data.csv.
 
-Five determinant names such as "day", degree1, degree2, y1 and y2 in data.csv should not be changed.
+The next hospital visit date is automatically recognized by phope with the end of "day" 
+in data.csv.
+
+Five determinant names such as "day", "degree1", "degree2", 
+"y1" and "y2" should not be changed in data.csv.
+
+This example shows two biomarkers such as hbA1c and NT-proBNP. 
 
-phope is a universal biomarker prediction tool with the past data. This example shows two biomarkers such as hbA1c and NT-proBNP. 
+phope can predict any two biomakers simultaneously with the second and third columns in data.csv.
 
-phope can predict any two biomakers simultaneously using the data in the second and third columns.
+Columns 4 (degree1) and 5 (degree2) show the degree of polynomial regression for the first and second biomarkers, respectively.
 
-Columns 4 and 5 show the degree of polynomial regression for the first and second biomarkers, respectively.
+Columns 6 (y1) and 7 (y2) set the range of vertical axis for the first and second biomarkers, respectively. The range of y1 is from 5 to 9 and that of y2 is from 0 to 450.
 
-Columns 6 and 7 set the range of vertical axis for the first and second biomarkers, respectively.
+Based on data.csv with state-of-the-art technology using linear polynomial regressions, phope or phope.py can calculate and predict values of biomarkers for the next hospital visit.
 
-Based on data.csv with state-of-the-art technology, phope or phope.py can calculate and predict values of biomarkers for the next visit.
+R2-squared value can identify the best polynomial regression model. The higher the R2-squared, the better the prediction accuracy.
 
 Predicting biomarker values allows patients to know the progress and trends of improvement in their diseases. 
 
 Predictive values are hopes of patients.
 
+An image png file will be automatically generated by phope or phope.py
+
 # How to install phope
+If you receive an error message in installation, Python may not be installed properly.
+
 $ pip install phope
 
 # How to run phope
+Make sure that data.csv file is the same directory for running phope.
+
 $ phope
 
+The result will be displayed on your screen and the png image file will be also generated.
```

### Comparing `phope-0.0.7/README.md` & `phope-0.0.8/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,68 @@
 # patient
 This is under review.
 
 Patients need to know effects of medication and exercise for alleviating diseases. 
 Biomarkers are used to monitor the status of individual diseases.
 
 phope.py (Patient for Hospital Observation and Predicting Effects of medication and exercise)
-with five determinants such as "day" (tested date), "hgb" of hbA1c value (biomarker for diabetes), "ntbnp" of NT-proBNP value (biomarker for heart failure), "degree1" (polynomial regression for hbA1c), and "degree2" (polynomial regression for NT-proBNP) is a universal biomarker prediction tool that can be used for evaluating the performance and predicting values of biomarkers in the next hospital visit.
+with five determinants such as "day" (tested date), "hgb" of hbA1c value (biomarker for diabetes), "ntbnp" of NT-proBNP value (biomarker for heart failure), "degree1" (polynomial regression for hbA1c), and "degree2" (polynomial regression for NT-proBNP) is a universal biomarker prediction tool that can be used for evaluating the performance and predicting values of biomarkers for the next hospital visit.
 
 To run phope.py after creating a data.csv, type python phope.py in the terminal.
+The following table is an example of data.csv. 
+2023/4/10 is the date of the next hospital visit.
 
-In phope.py, you can change it for your use.
+# An example of data.csv for phope.py
+<img src="https://github.com/y-takefuji/patient/raw/main/datacsv.png" height=120 width=480>
 
-phope is a PyPI application. phope allows users to run on Windows, MacOS, and Linux operating systems as long as Python is installed on the system. phope can set left vertical axis and right vertical axis of two biomakers with data.csv.
+In phope.py, you can change Python codes for your use.
 
-data.csv is a data file composed of seven determinants such as "day" (tested date), "hgb" of hbA1c value (biomarker for diabetes), "ntbnp" of NT-proBNP value (biomarker for heart failure), "degree1" (polynomial regression for hbA1c), "degree2" (polynomial regression for NT-proBNP), the first vertical-axis range on left side (low and high), and the second vertical-axis range on right side (low and high).
+phope was developed based on phope.py 
+which is a PyPI universal biomarker prediction tool with data.csv. 
+PyPI allows phope to run on Windows, MacOS, and Linux operating systems 
+as long as Python is installed on the system. 
+phope can set left vertical axis and right vertical axis of two biomakers with data.csv.
 
-The data.csv file must be created by the patient or physician before running the program.
+data.csv for phope is a data file composed of seven determinants such as "day" (tested date), "hbA1c" value (biomarker for diabetes), "NT-proBNP" value (biomarker for heart failure), "degree1" (polynomial regression for hbA1c), "degree2" (polynomial regression for NT-proBNP), the left vertical-axis range (low and high), and the right vertical-axis range (low and high).
 
-<img src="https://github.com/ytakefuji/patient/raw/main/fig.png" height=90 width=400>
+The data.csv file must be created by the patient or physician before running the program as shown in the following table.
+
+# An example of data.csv for phope
+<img src="https://github.com/y-takefuji/patient/raw/main/fig.png" height=120 width=480>
 
 phope allows users to modify two biomarker's names such as hbA1c and NT-proBNP in data.csv.
 
-Five determinant names such as "day", degree1, degree2, y1 and y2 in data.csv should not be changed.
+The next hospital visit date is automatically recognized by phope with the end of "day" 
+in data.csv.
+
+Five determinant names such as "day", "degree1", "degree2", 
+"y1" and "y2" should not be changed in data.csv.
+
+This example shows two biomarkers such as hbA1c and NT-proBNP. 
 
-phope is a universal biomarker prediction tool with the past data. This example shows two biomarkers such as hbA1c and NT-proBNP. 
+phope can predict any two biomakers simultaneously with the second and third columns in data.csv.
 
-phope can predict any two biomakers simultaneously using the data in the second and third columns.
+Columns 4 (degree1) and 5 (degree2) show the degree of polynomial regression for the first and second biomarkers, respectively.
 
-Columns 4 and 5 show the degree of polynomial regression for the first and second biomarkers, respectively.
+Columns 6 (y1) and 7 (y2) set the range of vertical axis for the first and second biomarkers, respectively. The range of y1 is from 5 to 9 and that of y2 is from 0 to 450.
 
-Columns 6 and 7 set the range of vertical axis for the first and second biomarkers, respectively.
+Based on data.csv with state-of-the-art technology using linear polynomial regressions, phope or phope.py can calculate and predict values of biomarkers for the next hospital visit.
 
-Based on data.csv with state-of-the-art technology, phope or phope.py can calculate and predict values of biomarkers for the next visit.
+R2-squared value can identify the best polynomial regression model. The higher the R2-squared, the better the prediction accuracy.
 
 Predicting biomarker values allows patients to know the progress and trends of improvement in their diseases. 
 
 Predictive values are hopes of patients.
 
+An image png file will be automatically generated by phope or phope.py
+
 # How to install phope
+If you receive an error message in installation, Python may not be installed properly.
+
 $ pip install phope
 
 # How to run phope
+Make sure that data.csv file is the same directory for running phope.
+
 $ phope
 
+The result will be displayed on your screen and the png image file will be also generated.
```

### Comparing `phope-0.0.7/setup.py` & `phope-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phope",
-    version="0.0.7",
+    version="0.0.8",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="universal biomarker prediction tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/patient",
+    url="https://github.com/y-takefuji/patient",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/patient",
+        "Bug Tracker": "https://github.com/y-takefuji/patient",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
```

### Comparing `phope-0.0.7/src/phope.egg-info/PKG-INFO` & `phope-0.0.8/src/phope.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,86 @@
 Metadata-Version: 2.1
 Name: phope
-Version: 0.0.7
+Version: 0.0.8
 Summary: universal biomarker prediction tool
-Home-page: https://github.com/ytakefuji/patient
+Home-page: https://github.com/y-takefuji/patient
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/patient
+Project-URL: Bug Tracker, https://github.com/y-takefuji/patient
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # patient
 This is under review.
 
 Patients need to know effects of medication and exercise for alleviating diseases. 
 Biomarkers are used to monitor the status of individual diseases.
 
 phope.py (Patient for Hospital Observation and Predicting Effects of medication and exercise)
-with five determinants such as "day" (tested date), "hgb" of hbA1c value (biomarker for diabetes), "ntbnp" of NT-proBNP value (biomarker for heart failure), "degree1" (polynomial regression for hbA1c), and "degree2" (polynomial regression for NT-proBNP) is a universal biomarker prediction tool that can be used for evaluating the performance and predicting values of biomarkers in the next hospital visit.
+with five determinants such as "day" (tested date), "hgb" of hbA1c value (biomarker for diabetes), "ntbnp" of NT-proBNP value (biomarker for heart failure), "degree1" (polynomial regression for hbA1c), and "degree2" (polynomial regression for NT-proBNP) is a universal biomarker prediction tool that can be used for evaluating the performance and predicting values of biomarkers for the next hospital visit.
 
 To run phope.py after creating a data.csv, type python phope.py in the terminal.
+The following table is an example of data.csv. 
+2023/4/10 is the date of the next hospital visit.
 
-In phope.py, you can change it for your use.
+# An example of data.csv for phope.py
+<img src="https://github.com/y-takefuji/patient/raw/main/datacsv.png" height=120 width=480>
 
-phope is a PyPI application. phope allows users to run on Windows, MacOS, and Linux operating systems as long as Python is installed on the system. phope can set left vertical axis and right vertical axis of two biomakers with data.csv.
+In phope.py, you can change Python codes for your use.
 
-data.csv is a data file composed of seven determinants such as "day" (tested date), "hgb" of hbA1c value (biomarker for diabetes), "ntbnp" of NT-proBNP value (biomarker for heart failure), "degree1" (polynomial regression for hbA1c), "degree2" (polynomial regression for NT-proBNP), the first vertical-axis range on left side (low and high), and the second vertical-axis range on right side (low and high).
+phope was developed based on phope.py 
+which is a PyPI universal biomarker prediction tool with data.csv. 
+PyPI allows phope to run on Windows, MacOS, and Linux operating systems 
+as long as Python is installed on the system. 
+phope can set left vertical axis and right vertical axis of two biomakers with data.csv.
 
-The data.csv file must be created by the patient or physician before running the program.
+data.csv for phope is a data file composed of seven determinants such as "day" (tested date), "hbA1c" value (biomarker for diabetes), "NT-proBNP" value (biomarker for heart failure), "degree1" (polynomial regression for hbA1c), "degree2" (polynomial regression for NT-proBNP), the left vertical-axis range (low and high), and the right vertical-axis range (low and high).
 
-<img src="https://github.com/ytakefuji/patient/raw/main/fig.png" height=90 width=400>
+The data.csv file must be created by the patient or physician before running the program as shown in the following table.
+
+# An example of data.csv for phope
+<img src="https://github.com/y-takefuji/patient/raw/main/fig.png" height=120 width=480>
 
 phope allows users to modify two biomarker's names such as hbA1c and NT-proBNP in data.csv.
 
-Five determinant names such as "day", degree1, degree2, y1 and y2 in data.csv should not be changed.
+The next hospital visit date is automatically recognized by phope with the end of "day" 
+in data.csv.
+
+Five determinant names such as "day", "degree1", "degree2", 
+"y1" and "y2" should not be changed in data.csv.
+
+This example shows two biomarkers such as hbA1c and NT-proBNP. 
 
-phope is a universal biomarker prediction tool with the past data. This example shows two biomarkers such as hbA1c and NT-proBNP. 
+phope can predict any two biomakers simultaneously with the second and third columns in data.csv.
 
-phope can predict any two biomakers simultaneously using the data in the second and third columns.
+Columns 4 (degree1) and 5 (degree2) show the degree of polynomial regression for the first and second biomarkers, respectively.
 
-Columns 4 and 5 show the degree of polynomial regression for the first and second biomarkers, respectively.
+Columns 6 (y1) and 7 (y2) set the range of vertical axis for the first and second biomarkers, respectively. The range of y1 is from 5 to 9 and that of y2 is from 0 to 450.
 
-Columns 6 and 7 set the range of vertical axis for the first and second biomarkers, respectively.
+Based on data.csv with state-of-the-art technology using linear polynomial regressions, phope or phope.py can calculate and predict values of biomarkers for the next hospital visit.
 
-Based on data.csv with state-of-the-art technology, phope or phope.py can calculate and predict values of biomarkers for the next visit.
+R2-squared value can identify the best polynomial regression model. The higher the R2-squared, the better the prediction accuracy.
 
 Predicting biomarker values allows patients to know the progress and trends of improvement in their diseases. 
 
 Predictive values are hopes of patients.
 
+An image png file will be automatically generated by phope or phope.py
+
 # How to install phope
+If you receive an error message in installation, Python may not be installed properly.
+
 $ pip install phope
 
 # How to run phope
+Make sure that data.csv file is the same directory for running phope.
+
 $ phope
 
+The result will be displayed on your screen and the png image file will be also generated.
```

### Comparing `phope-0.0.7/src/phope.py` & `phope-0.0.8/src/phope.py`

 * *Files identical despite different names*


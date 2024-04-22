# Comparing `tmp/clidoro-0.1.3.tar.gz` & `tmp/clidoro-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clidoro-0.1.3.tar", last modified: Thu Apr 18 08:26:50 2024, max compression
+gzip compressed data, was "clidoro-0.1.4.tar", last modified: Mon Apr 22 05:37:52 2024, max compression
```

## Comparing `clidoro-0.1.3.tar` & `clidoro-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:26:50.350615 clidoro-0.1.3/
--rw-rw-r--   0 juno      (1000) juno      (1000)     1065 2024-04-18 03:48:24.000000 clidoro-0.1.3/LICENSE.MD
--rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-18 08:26:50.350615 clidoro-0.1.3/PKG-INFO
--rw-rw-r--   0 juno      (1000) juno      (1000)     1343 2024-04-18 08:13:36.000000 clidoro-0.1.3/README.md
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:26:50.346615 clidoro-0.1.3/clidoro/
--rw-rw-r--   0 juno      (1000) juno      (1000)        0 2024-04-18 05:42:39.000000 clidoro-0.1.3/clidoro/__init__.py
--rw-rw-r--   0 juno      (1000) juno      (1000)     2870 2024-04-18 08:05:45.000000 clidoro-0.1.3/clidoro/_utils.py
--rw-rw-r--   0 juno      (1000) juno      (1000)     2923 2024-04-18 06:32:17.000000 clidoro-0.1.3/clidoro/chart.py
--rw-rw-r--   0 juno      (1000) juno      (1000)    57042 2024-04-18 07:45:05.000000 clidoro-0.1.3/clidoro/clidoro.png
--rw-------   0 juno      (1000) juno      (1000)     3717 2024-04-18 08:25:45.000000 clidoro-0.1.3/clidoro/clidoro.py
--rw-rw-r--   0 juno      (1000) juno      (1000)      642 2024-04-18 08:11:45.000000 clidoro-0.1.3/clidoro/data.py
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:26:50.350615 clidoro-0.1.3/clidoro/termgraph/
--rw-rw-r--   0 juno      (1000) juno      (1000)      205 2024-04-17 14:24:17.000000 clidoro-0.1.3/clidoro/termgraph/__init__.py
--rw-rw-r--   0 juno      (1000) juno      (1000)    24073 2024-04-17 14:20:38.000000 clidoro-0.1.3/clidoro/termgraph/_termgraph.py
--rw-rw-r--   0 juno      (1000) juno      (1000)    12733 2024-04-17 14:42:37.000000 clidoro-0.1.3/clidoro/termgraph/module.py
--rw-rw-r--   0 juno      (1000) juno      (1000)      546 2024-04-17 14:26:13.000000 clidoro-0.1.3/clidoro/termgraph/utils.py
-drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-18 08:26:50.350615 clidoro-0.1.3/clidoro.egg-info/
--rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-18 08:26:50.000000 clidoro-0.1.3/clidoro.egg-info/PKG-INFO
--rw-rw-r--   0 juno      (1000) juno      (1000)      484 2024-04-18 08:26:50.000000 clidoro-0.1.3/clidoro.egg-info/SOURCES.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 08:26:50.000000 clidoro-0.1.3/clidoro.egg-info/dependency_links.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)       49 2024-04-18 08:26:50.000000 clidoro-0.1.3/clidoro.egg-info/entry_points.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 04:35:24.000000 clidoro-0.1.3/clidoro.egg-info/not-zip-safe
--rw-rw-r--   0 juno      (1000) juno      (1000)       70 2024-04-18 08:26:50.000000 clidoro-0.1.3/clidoro.egg-info/requires.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)        8 2024-04-18 08:26:50.000000 clidoro-0.1.3/clidoro.egg-info/top_level.txt
--rw-rw-r--   0 juno      (1000) juno      (1000)      102 2024-04-18 08:26:50.350615 clidoro-0.1.3/setup.cfg
--rw-rw-r--   0 juno      (1000) juno      (1000)     1887 2024-04-18 08:26:30.000000 clidoro-0.1.3/setup.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-22 05:37:52.098888 clidoro-0.1.4/
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1065 2024-04-18 03:48:24.000000 clidoro-0.1.4/LICENSE.MD
+-rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-22 05:37:52.098888 clidoro-0.1.4/PKG-INFO
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1343 2024-04-18 08:13:36.000000 clidoro-0.1.4/README.md
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-22 05:37:52.094888 clidoro-0.1.4/clidoro/
+-rw-rw-r--   0 juno      (1000) juno      (1000)        0 2024-04-18 05:42:39.000000 clidoro-0.1.4/clidoro/__init__.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)     2870 2024-04-18 08:05:45.000000 clidoro-0.1.4/clidoro/_utils.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)     3903 2024-04-22 05:36:24.000000 clidoro-0.1.4/clidoro/chart.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)    57042 2024-04-18 07:45:05.000000 clidoro-0.1.4/clidoro/clidoro.png
+-rw-------   0 juno      (1000) juno      (1000)     3717 2024-04-22 05:25:54.000000 clidoro-0.1.4/clidoro/clidoro.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)      642 2024-04-18 08:11:45.000000 clidoro-0.1.4/clidoro/data.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-22 05:37:52.098888 clidoro-0.1.4/clidoro/termgraph/
+-rw-rw-r--   0 juno      (1000) juno      (1000)      205 2024-04-17 14:24:17.000000 clidoro-0.1.4/clidoro/termgraph/__init__.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)    24073 2024-04-17 14:20:38.000000 clidoro-0.1.4/clidoro/termgraph/_termgraph.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)    12733 2024-04-17 14:42:37.000000 clidoro-0.1.4/clidoro/termgraph/module.py
+-rw-rw-r--   0 juno      (1000) juno      (1000)      546 2024-04-17 14:26:13.000000 clidoro-0.1.4/clidoro/termgraph/utils.py
+drwxrwxr-x   0 juno      (1000) juno      (1000)        0 2024-04-22 05:37:52.098888 clidoro-0.1.4/clidoro.egg-info/
+-rw-r--r--   0 juno      (1000) juno      (1000)     2579 2024-04-22 05:37:52.000000 clidoro-0.1.4/clidoro.egg-info/PKG-INFO
+-rw-rw-r--   0 juno      (1000) juno      (1000)      484 2024-04-22 05:37:52.000000 clidoro-0.1.4/clidoro.egg-info/SOURCES.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-22 05:37:52.000000 clidoro-0.1.4/clidoro.egg-info/dependency_links.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)       49 2024-04-22 05:37:52.000000 clidoro-0.1.4/clidoro.egg-info/entry_points.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        1 2024-04-18 04:35:24.000000 clidoro-0.1.4/clidoro.egg-info/not-zip-safe
+-rw-rw-r--   0 juno      (1000) juno      (1000)       70 2024-04-22 05:37:52.000000 clidoro-0.1.4/clidoro.egg-info/requires.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)        8 2024-04-22 05:37:52.000000 clidoro-0.1.4/clidoro.egg-info/top_level.txt
+-rw-rw-r--   0 juno      (1000) juno      (1000)      102 2024-04-22 05:37:52.098888 clidoro-0.1.4/setup.cfg
+-rw-rw-r--   0 juno      (1000) juno      (1000)     1887 2024-04-22 05:36:48.000000 clidoro-0.1.4/setup.py
```

### Comparing `clidoro-0.1.3/LICENSE.MD` & `clidoro-0.1.4/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.3/PKG-INFO` & `clidoro-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clidoro
-Version: 0.1.3
+Version: 0.1.4
 Summary: clidoro: pomodoro in your cli
 Home-page: https://github.com/kingjuno/clidoro
 License: MIT
 Keywords: Productivity,Pomodoro
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
```

### Comparing `clidoro-0.1.3/README.md` & `clidoro-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.3/clidoro/_utils.py` & `clidoro-0.1.4/clidoro/_utils.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.3/clidoro/chart.py` & `clidoro-0.1.4/clidoro/chart.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
 import sqlite3
 from contextlib import redirect_stdout
-from datetime import date, datetime
+from datetime import date, datetime, timedelta
 
 from clidoro._utils import date_str_to_datetime
 from clidoro.termgraph.module import Args, BarChart, Colors, Data
 
 GREEN_COLOR = "\033[92m"
 RED_COLOR = "\033[91m"
 RESET_COLOR = "\033[0m"
@@ -15,49 +15,80 @@
     try:
         conn = sqlite3.connect(f"{cache_dir}/clidoro.sqlite")
         cursor = conn.cursor()
         cursor.execute("SELECT date, amount FROM random_data")
         rows = cursor.fetchall()
         conn.close()
         dates = [list(row) for row in rows]
-        if len(dates) == 0: raise
+        if len(dates) == 0:
+            raise
     except:
         return f"{RED_COLOR}No data found.{RESET_COLOR}\n"
 
     todays_date = date.today()
     todays_times = [
         row[1]
         for row in dates
         if datetime.strptime(row[0], "%Y-%m-%d %H:%M:%S.%f").date() == todays_date
     ]
     times = [time[1] for time in dates]
+
+    # Calculate this week's statistics starting from Sunday
+    today_weekday = todays_date.weekday()  # 0 for Monday, 6 for Sunday
+    start_of_week = todays_date - timedelta(days=today_weekday)
+    this_week = [
+        time[1]
+        for time in dates
+        if start_of_week
+        <= datetime.strptime(time[0], "%Y-%m-%d %H:%M:%S.%f").date()
+        <= todays_date
+    ]
+    week_stats = (
+        f"\n{GREEN_COLOR}Pomodoros This Week: {RED_COLOR}{len(this_week)}{RESET_COLOR}\n"
+        + f"{GREEN_COLOR}Hours This Week: {RED_COLOR}{sum(this_week)/60:.2f}{RESET_COLOR}\n"
+    )
+
+    first_day = min(
+        datetime.strptime(row[0], "%Y-%m-%d %H:%M:%S.%f").date() for row in dates
+    )
+
+    days_since_start = (todays_date - first_day).days
+    if days_since_start > 0:
+        daily_avg = sum(times) / days_since_start
+        avg_stats = f"\n{GREEN_COLOR}Daily Average: {RED_COLOR}{daily_avg/60:.2f}{RESET_COLOR} hours\n"
+    else:
+        avg_stats = ""
+
     stats = (
         f"{GREEN_COLOR}Pomodoros Today: {RED_COLOR}{len(todays_times)}{RESET_COLOR}\n"
         + f"{GREEN_COLOR}Hours Today: {RED_COLOR}{sum(todays_times)/60:.2f}{RESET_COLOR}\n"
     )
 
     stats += (
         f"\n{GREEN_COLOR}Pomodoros Total: {RED_COLOR}{len(times)}{RESET_COLOR}\n"
         f"{GREEN_COLOR}Hours Total: {RED_COLOR}{sum(times)/60:.2f}{RESET_COLOR}\n"
     )
+
+    stats += week_stats + avg_stats
     return stats
 
 
 def history(cache_dir):
     try:
         conn = sqlite3.connect(f"{cache_dir}/clidoro.sqlite")
         cursor = conn.cursor()
         cursor.execute("SELECT date, amount FROM random_data")
         rows = cursor.fetchall()
         conn.close()
         dates = [list(row) for row in rows]
-        if len(dates) == 0: raise
+        if len(dates) == 0:
+            raise
     except:
         return f"{RED_COLOR}No data found.{RESET_COLOR}\n"
-    
+
     timers = set([timer[-1] for timer in dates])
     if len(dates) == 0:
         return f"{RED_COLOR}No data found.{RESET_COLOR}\n"
     current_week = datetime.now().isocalendar()[1]
     weekly_stats = {
         "Monday": {timer: 0 for timer in timers},
         "Tuesday": {timer: 0 for timer in timers},
@@ -65,17 +96,16 @@
         "Thursday": {timer: 0 for timer in timers},
         "Friday": {timer: 0 for timer in timers},
         "Saturday": {timer: 0 for timer in timers},
         "Sunday": {timer: 0 for timer in timers},
     }
     for date, timer in dates:
         date = date_str_to_datetime(date)
-        if date.isocalendar()[1] == current_week:
-            weekday = date.strftime("%A")
-            weekly_stats[weekday][timer] += 1
+        weekday = date.strftime("%A")
+        weekly_stats[weekday][timer] += 1
 
     week_data = [[sum([i[j] for j in i])] for i in weekly_stats.values()]
     data = Data(week_data, list(weekly_stats.keys()), ["Pomodoros by Week Day"])
     chart = BarChart(
         data,
         Args(
             title=None,
```

### Comparing `clidoro-0.1.3/clidoro/clidoro.png` & `clidoro-0.1.4/clidoro/clidoro.png`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.3/clidoro/clidoro.py` & `clidoro-0.1.4/clidoro/clidoro.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.3/clidoro/data.py` & `clidoro-0.1.4/clidoro/data.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.3/clidoro/termgraph/_termgraph.py` & `clidoro-0.1.4/clidoro/termgraph/_termgraph.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.3/clidoro/termgraph/module.py` & `clidoro-0.1.4/clidoro/termgraph/module.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.3/clidoro/termgraph/utils.py` & `clidoro-0.1.4/clidoro/termgraph/utils.py`

 * *Files identical despite different names*

### Comparing `clidoro-0.1.3/clidoro.egg-info/PKG-INFO` & `clidoro-0.1.4/clidoro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clidoro
-Version: 0.1.3
+Version: 0.1.4
 Summary: clidoro: pomodoro in your cli
 Home-page: https://github.com/kingjuno/clidoro
 License: MIT
 Keywords: Productivity,Pomodoro
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
```

### Comparing `clidoro-0.1.3/setup.py` & `clidoro-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
 MAJOR_VERSION = "0"
 MINOR_VERSION = "1"
-MICRO_VERSION = "3"
+MICRO_VERSION = "4"
 VERSION = "{}.{}.{}".format(MAJOR_VERSION, MINOR_VERSION, MICRO_VERSION)
 
 
 setup(
     name="clidoro",
     packages=find_packages(exclude=["docs", "tests*", "examples"]),
     version=VERSION,
```


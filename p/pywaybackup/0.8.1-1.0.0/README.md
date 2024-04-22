# Comparing `tmp/pywaybackup-0.8.1.tar.gz` & `tmp/pywaybackup-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywaybackup-0.8.1.tar", last modified: Fri Apr 12 12:41:33 2024, max compression
+gzip compressed data, was "pywaybackup-1.0.0.tar", last modified: Mon Apr 22 06:58:06 2024, max compression
```

## Comparing `pywaybackup-0.8.1.tar` & `pywaybackup-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-04-12 12:41:33.239507 pywaybackup-0.8.1/
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1065 2024-02-25 19:19:33.000000 pywaybackup-0.8.1/LICENSE
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4925 2024-04-12 12:41:33.239507 pywaybackup-0.8.1/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4572 2024-04-12 12:30:31.000000 pywaybackup-0.8.1/README.md
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-04-12 12:41:33.239507 pywaybackup-0.8.1/pywaybackup/
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4606 2024-04-12 12:30:05.000000 pywaybackup-0.8.1/pywaybackup/SnapshotCollection.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1644 2024-04-12 12:30:31.000000 pywaybackup-0.8.1/pywaybackup/Verbosity.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)        0 2024-02-25 19:19:33.000000 pywaybackup-0.8.1/pywaybackup/__init__.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       21 2024-04-12 12:40:47.000000 pywaybackup-0.8.1/pywaybackup/__version__.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)    11879 2024-04-12 12:40:16.000000 pywaybackup-0.8.1/pywaybackup/archive.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     2329 2024-04-12 12:40:16.000000 pywaybackup-0.8.1/pywaybackup/arguments.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)      868 2024-04-12 12:40:16.000000 pywaybackup-0.8.1/pywaybackup/main.py
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-04-12 12:41:33.239507 pywaybackup-0.8.1/pywaybackup.egg-info/
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4925 2024-04-12 12:41:33.000000 pywaybackup-0.8.1/pywaybackup.egg-info/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)      416 2024-04-12 12:41:33.000000 pywaybackup-0.8.1/pywaybackup.egg-info/SOURCES.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)        1 2024-04-12 12:41:33.000000 pywaybackup-0.8.1/pywaybackup.egg-info/dependency_links.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       52 2024-04-12 12:41:33.000000 pywaybackup-0.8.1/pywaybackup.egg-info/entry_points.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       30 2024-04-12 12:41:33.000000 pywaybackup-0.8.1/pywaybackup.egg-info/requires.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       12 2024-04-12 12:41:33.000000 pywaybackup-0.8.1/pywaybackup.egg-info/top_level.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       38 2024-04-12 12:41:33.239507 pywaybackup-0.8.1/setup.cfg
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1091 2024-02-26 09:18:12.000000 pywaybackup-0.8.1/setup.py
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-04-22 06:58:06.836944 pywaybackup-1.0.0/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1065 2024-02-25 19:19:33.000000 pywaybackup-1.0.0/LICENSE
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     5403 2024-04-22 06:58:06.826944 pywaybackup-1.0.0/PKG-INFO
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     5050 2024-04-22 06:58:04.000000 pywaybackup-1.0.0/README.md
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-04-22 06:58:06.826944 pywaybackup-1.0.0/pywaybackup/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4606 2024-04-12 12:30:05.000000 pywaybackup-1.0.0/pywaybackup/SnapshotCollection.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1644 2024-04-12 12:30:31.000000 pywaybackup-1.0.0/pywaybackup/Verbosity.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)        0 2024-02-25 19:19:33.000000 pywaybackup-1.0.0/pywaybackup/__init__.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)       21 2024-04-22 06:58:04.000000 pywaybackup-1.0.0/pywaybackup/__version__.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)    12030 2024-04-22 06:58:04.000000 pywaybackup-1.0.0/pywaybackup/archive.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     2461 2024-04-22 06:58:04.000000 pywaybackup-1.0.0/pywaybackup/arguments.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)      877 2024-04-22 06:58:04.000000 pywaybackup-1.0.0/pywaybackup/main.py
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-04-22 06:58:06.826944 pywaybackup-1.0.0/pywaybackup.egg-info/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     5403 2024-04-22 06:58:06.000000 pywaybackup-1.0.0/pywaybackup.egg-info/PKG-INFO
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)      416 2024-04-22 06:58:06.000000 pywaybackup-1.0.0/pywaybackup.egg-info/SOURCES.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)        1 2024-04-22 06:58:06.000000 pywaybackup-1.0.0/pywaybackup.egg-info/dependency_links.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)       52 2024-04-22 06:58:06.000000 pywaybackup-1.0.0/pywaybackup.egg-info/entry_points.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)       30 2024-04-22 06:58:06.000000 pywaybackup-1.0.0/pywaybackup.egg-info/requires.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)       12 2024-04-22 06:58:06.000000 pywaybackup-1.0.0/pywaybackup.egg-info/top_level.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)       38 2024-04-22 06:58:06.836944 pywaybackup-1.0.0/setup.cfg
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1091 2024-02-26 09:18:12.000000 pywaybackup-1.0.0/setup.py
```

### Comparing `pywaybackup-0.8.1/LICENSE` & `pywaybackup-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywaybackup-0.8.1/PKG-INFO` & `pywaybackup-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pywaybackup
-Version: 0.8.1
+Version: 1.0.0
 Summary: Download snapshots from the Wayback Machine
 Home-page: https://github.com/bitdruid/python-wayback-machine-downloader
 Author: bitdruid
 Author-email: bitdruid@outlook.com
 License: MIT
 Keywords: wayback machine internet archive
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # archive wayback downloader
 
 [![PyPI](https://img.shields.io/pypi/v/pywaybackup)](https://pypi.org/project/pywaybackup/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pywaybackup)](https://pypi.org/project/pywaybackup/)
-![Release](https://img.shields.io/badge/Release-beta-orange)
 ![Python Version](https://img.shields.io/badge/Python-3.6-blue)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 Downloading archived web pages from the [Wayback Machine](https://archive.org/web/).
 
 Internet-archive is a nice source for several OSINT-information. This script is a work in progress to query and fetch archived web pages.
 
@@ -39,66 +38,70 @@
    ```pip install .```
    - in a virtual env or use `--break-system-package`
 
 ## Usage
 
 This script allows you to download content from the Wayback Machine (archive.org). You can use it to download either the latest version or all versions of web page snapshots within a specified range.
 
-<!-- ## Info -->
-
 ### Arguments
 
 - `-h`, `--help`: Show the help message and exit.
 - `-a`, `--about`: Show information about the script and exit.
 
 #### Required Arguments
 
-- `-u URL`, `--url URL`: The URL of the web page to download. This argument is required.
+- `-u`, `--url`: The URL of the web page to download. This argument is required.
 
 #### Mode Selection (Choose One)
 
-- `-c`, `--current`: Download the latest version of each file snapshot. You will get a rebuild of the current website with all available files.
+- `-c`, `--current`: Download the latest version of each file snapshot. You will get a rebuild of the current website with all available files (but not any original state because new and old versions are mixed).
 - `-f`, `--full`: Download snapshots of all timestamps. You will get a folder per timestamp with the files available at that time.
 - `-s`, `--save`: Save a page to the Wayback Machine. (beta)
 
 #### Optional Arguments
 
 - `-l`, `--list`: Only print the snapshots available within the specified range. Does not download the snapshots.
 - `-e`, `--explicit`: Only download the explicit given url. No wildcard subdomains or paths.
-- `-o OUTPUT`, `--output OUTPUT`: The folder where downloaded files will be saved.
+- `-o`, `--output`: The folder where downloaded files will be saved.
 
 - **Range Selection:**<br>
 Specify the range in years or a specific timestamp either start, end or both. If you specify the `range` argument, the `start` and `end` arguments will be ignored. Format for timestamps: YYYYMMDDhhmmss. You can only give a year or increase specificity by going through the timestamp starting on the left.<br>
 (year 2019, year+month 201901, year+month+day 20190101, year+month+day+hour 2019010112)
-   - `-r RANGE`, `--range RANGE`: Specify the range in years for which to search and download snapshots.
+   - `-r`, `--range`: Specify the range in years for which to search and download snapshots.
    - `--start`: Timestamp to start searching.
    - `--end`: Timestamp to end searching.
 
 #### Additional
 
-- `--csv`: Save a csv file with the list of snapshots inside the output folder.
+- `--csv`: Save a csv file with the list of snapshots inside the output folder or a specified folder. If you set `--list` the csv will contain the cdx list of snapshots. If you set either `--current` or `--full` the csv will contain the downloaded files.
 - `--no-redirect`: Do not follow redirects of snapshots. Archive.org sometimes redirects to a different snapshot for several reasons. Downloading redirects may lead to timestamp-folders which contain some files with a different timestamp. This does not matter if you only want to download the latest version (`-c`).
-- `--verbosity [LEVEL]`: Set the verbosity: json (print json response), progress (show progress bar) or standard (default).
-- `--retry [RETRY_FAILED]`: Retry failed downloads. You can specify the number of retry attempts as an integer.
-- `--worker [AMOUNT]`: The number of worker to use for downloading (simultaneous downloads). Default is 1. A safe spot is about 10 workers. Beware: Using too many worker will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
+- `--verbosity`: Set the verbosity: json (print json response), progress (show progress bar).
+- `--retry`: Retry failed downloads. You can specify the number of retry attempts as an integer.
+- `--workers`: The number of workers to use for downloading (simultaneous downloads). Default is 1. A safe spot is about 10 workers. Beware: Using too many workers will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
 
 ### Examples
 
 Download latest snapshot of all files:<br>
 `waybackup -u http://example.com -c`
 
 Download latest snapshot of all files with retries:<br>
 `waybackup -u http://example.com -c --retry 3`
 
-Download all snapshots sorted per timestamp with a specified range and follow redirects:<br>
-`waybackup -u http://example.com -f -r 5 --redirect`
+Download all snapshots sorted per timestamp with a specified range and do not follow redirects:<br>
+`waybackup -u http://example.com -f -r 5 --no-redirect`
+
+Download all snapshots sorted per timestamp with a specified range and save to a specified folder with 3 workers:<br>
+`waybackup -u http://example.com -f -r 5 -o /home/user/Downloads/snapshots --workers 3`
+
+Download all snapshots from 2020 to 12th of December 2022 with 4 workers, save a csv and show a progress bar:
+`waybackup -u http://example.com -f --start 2020 --end 20221212 --workers 4 --csv --verbosity progress`
 
-Download all snapshots sorted per timestamp with a specified range and save to a specified folder with 3 worker:<br>
-`waybackup -u http://example.com -f -r 5 -o /home/user/Downloads/snapshots --worker 3`
+Download all snapshots and output a json response:<br>
+`waybackup -u http://example.com -f --verbosity json`
 
-List available snapshots per timestamp without downloading:<br>
-`waybackup -u http://example.com -f -l`
+List available snapshots per timestamp without downloading and save a csv file to home folder:<br>
+`waybackup -u http://example.com -f -l --csv /home/user/Downloads`
 
 ## Contributing
 
 I'm always happy for some feature requests to improve the usability of this script.
 Feel free to give suggestions and report issues. Project is still far from being perfect.
```

### Comparing `pywaybackup-0.8.1/README.md` & `pywaybackup-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # archive wayback downloader
 
 [![PyPI](https://img.shields.io/pypi/v/pywaybackup)](https://pypi.org/project/pywaybackup/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pywaybackup)](https://pypi.org/project/pywaybackup/)
-![Release](https://img.shields.io/badge/Release-beta-orange)
 ![Python Version](https://img.shields.io/badge/Python-3.6-blue)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 Downloading archived web pages from the [Wayback Machine](https://archive.org/web/).
 
 Internet-archive is a nice source for several OSINT-information. This script is a work in progress to query and fetch archived web pages.
 
@@ -27,66 +26,70 @@
    ```pip install .```
    - in a virtual env or use `--break-system-package`
 
 ## Usage
 
 This script allows you to download content from the Wayback Machine (archive.org). You can use it to download either the latest version or all versions of web page snapshots within a specified range.
 
-<!-- ## Info -->
-
 ### Arguments
 
 - `-h`, `--help`: Show the help message and exit.
 - `-a`, `--about`: Show information about the script and exit.
 
 #### Required Arguments
 
-- `-u URL`, `--url URL`: The URL of the web page to download. This argument is required.
+- `-u`, `--url`: The URL of the web page to download. This argument is required.
 
 #### Mode Selection (Choose One)
 
-- `-c`, `--current`: Download the latest version of each file snapshot. You will get a rebuild of the current website with all available files.
+- `-c`, `--current`: Download the latest version of each file snapshot. You will get a rebuild of the current website with all available files (but not any original state because new and old versions are mixed).
 - `-f`, `--full`: Download snapshots of all timestamps. You will get a folder per timestamp with the files available at that time.
 - `-s`, `--save`: Save a page to the Wayback Machine. (beta)
 
 #### Optional Arguments
 
 - `-l`, `--list`: Only print the snapshots available within the specified range. Does not download the snapshots.
 - `-e`, `--explicit`: Only download the explicit given url. No wildcard subdomains or paths.
-- `-o OUTPUT`, `--output OUTPUT`: The folder where downloaded files will be saved.
+- `-o`, `--output`: The folder where downloaded files will be saved.
 
 - **Range Selection:**<br>
 Specify the range in years or a specific timestamp either start, end or both. If you specify the `range` argument, the `start` and `end` arguments will be ignored. Format for timestamps: YYYYMMDDhhmmss. You can only give a year or increase specificity by going through the timestamp starting on the left.<br>
 (year 2019, year+month 201901, year+month+day 20190101, year+month+day+hour 2019010112)
-   - `-r RANGE`, `--range RANGE`: Specify the range in years for which to search and download snapshots.
+   - `-r`, `--range`: Specify the range in years for which to search and download snapshots.
    - `--start`: Timestamp to start searching.
    - `--end`: Timestamp to end searching.
 
 #### Additional
 
-- `--csv`: Save a csv file with the list of snapshots inside the output folder.
+- `--csv`: Save a csv file with the list of snapshots inside the output folder or a specified folder. If you set `--list` the csv will contain the cdx list of snapshots. If you set either `--current` or `--full` the csv will contain the downloaded files.
 - `--no-redirect`: Do not follow redirects of snapshots. Archive.org sometimes redirects to a different snapshot for several reasons. Downloading redirects may lead to timestamp-folders which contain some files with a different timestamp. This does not matter if you only want to download the latest version (`-c`).
-- `--verbosity [LEVEL]`: Set the verbosity: json (print json response), progress (show progress bar) or standard (default).
-- `--retry [RETRY_FAILED]`: Retry failed downloads. You can specify the number of retry attempts as an integer.
-- `--worker [AMOUNT]`: The number of worker to use for downloading (simultaneous downloads). Default is 1. A safe spot is about 10 workers. Beware: Using too many worker will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
+- `--verbosity`: Set the verbosity: json (print json response), progress (show progress bar).
+- `--retry`: Retry failed downloads. You can specify the number of retry attempts as an integer.
+- `--workers`: The number of workers to use for downloading (simultaneous downloads). Default is 1. A safe spot is about 10 workers. Beware: Using too many workers will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
 
 ### Examples
 
 Download latest snapshot of all files:<br>
 `waybackup -u http://example.com -c`
 
 Download latest snapshot of all files with retries:<br>
 `waybackup -u http://example.com -c --retry 3`
 
-Download all snapshots sorted per timestamp with a specified range and follow redirects:<br>
-`waybackup -u http://example.com -f -r 5 --redirect`
+Download all snapshots sorted per timestamp with a specified range and do not follow redirects:<br>
+`waybackup -u http://example.com -f -r 5 --no-redirect`
+
+Download all snapshots sorted per timestamp with a specified range and save to a specified folder with 3 workers:<br>
+`waybackup -u http://example.com -f -r 5 -o /home/user/Downloads/snapshots --workers 3`
+
+Download all snapshots from 2020 to 12th of December 2022 with 4 workers, save a csv and show a progress bar:
+`waybackup -u http://example.com -f --start 2020 --end 20221212 --workers 4 --csv --verbosity progress`
 
-Download all snapshots sorted per timestamp with a specified range and save to a specified folder with 3 worker:<br>
-`waybackup -u http://example.com -f -r 5 -o /home/user/Downloads/snapshots --worker 3`
+Download all snapshots and output a json response:<br>
+`waybackup -u http://example.com -f --verbosity json`
 
-List available snapshots per timestamp without downloading:<br>
-`waybackup -u http://example.com -f -l`
+List available snapshots per timestamp without downloading and save a csv file to home folder:<br>
+`waybackup -u http://example.com -f -l --csv /home/user/Downloads`
 
 ## Contributing
 
 I'm always happy for some feature requests to improve the usability of this script.
 Feel free to give suggestions and report issues. Project is still far from being perfect.
```

### Comparing `pywaybackup-0.8.1/pywaybackup/SnapshotCollection.py` & `pywaybackup-1.0.0/pywaybackup/SnapshotCollection.py`

 * *Files identical despite different names*

### Comparing `pywaybackup-0.8.1/pywaybackup/Verbosity.py` & `pywaybackup-1.0.0/pywaybackup/Verbosity.py`

 * *Files identical despite different names*

### Comparing `pywaybackup-0.8.1/pywaybackup/archive.py` & `pywaybackup-1.0.0/pywaybackup/archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,34 +103,34 @@
         v.write(f"\n-----> ERROR: could not query snapshots:\n{e}"); exit()
 
 
 
 
 
 # example download: http://web.archive.org/web/20190815104545id_/https://www.google.com/
-def download_list(output, retry, no_redirect, worker):
+def download_list(output, retry, no_redirect, workers):
     """
     Download a list of urls in format: [{"timestamp": "20190815104545", "url": "https://www.google.com/"}]
     """
     if sc.count_list() == 0: 
         v.write("\nNothing to download");
         return
     v.write("\nDownloading snapshots...", progress=0)
-    if worker > 1:
-        v.write(f"\n-----> Simultaneous downloads: {worker}")
-        batch_size = sc.count_list() // worker + 1
+    if workers > 1:
+        v.write(f"\n-----> Simultaneous downloads: {workers}")
+        batch_size = sc.count_list() // workers + 1
     else:
         batch_size = sc.count_list()
     sc.create_collection()
     batch_list = [sc.SNAPSHOT_COLLECTION[i:i + batch_size] for i in range(0, len(sc.SNAPSHOT_COLLECTION), batch_size)]    
     threads = []
     worker = 0
     for batch in batch_list:
         worker += 1
-        thread = threading.Thread(target=download_loop, args=(batch, output, worker, retry, no_redirect))
+        thread = threading.Thread(target=download_loop, args=(batch, output, workers, retry, no_redirect))
         threads.append(thread)
         thread.start()
     for thread in threads:
         thread.join()
 
 def download_loop(snapshot_batch, output, worker, retry, no_redirect, attempt=1, connection=None):
     """
@@ -252,20 +252,23 @@
     """
     Parse the response code of the Wayback Machine and return a human-readable message.
     """
     if response_code in RESPONSE_CODE_DICT:
         return RESPONSE_CODE_DICT[response_code]
     return "Unknown response code"
 
-def save_csv(csv_path: str):
+def save_csv(csv_path: str, url: str):
     """
     Write a CSV file with the list of snapshots.
     """
     import csv
+    disallowed = ['<', '>', ':', '"', '/', '\\', '|', '?', '*']
+    for char in disallowed:
+        url = url.replace(char, '.')
     if sc.count_list() > 0:
         v.write("\nSaving CSV file...")
         os.makedirs(os.path.abspath(csv_path), exist_ok=True)
-        with open(os.path.join(csv_path, "waybackup.csv"), mode='w') as file:
+        with open(os.path.join(csv_path, f"waybackup_{url}.csv"), mode='w') as file:
             row = csv.DictWriter(file, sc.SNAPSHOT_COLLECTION[0].keys())
             row.writeheader()
             for snapshot in sc.SNAPSHOT_COLLECTION:
                 row.writerow(snapshot)
```

### Comparing `pywaybackup-0.8.1/pywaybackup/arguments.py` & `pywaybackup-1.0.0/pywaybackup/arguments.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,34 @@
+import sys
 import argparse
 from pywaybackup.__version__ import __version__
 
 def parse():
 
     parser = argparse.ArgumentParser(description='Download from wayback machine (archive.org)')
     parser.add_argument('-a', '--about', action='version', version='%(prog)s ' + __version__ + ' by @bitdruid -> https://github.com/bitdruid')
 
     required = parser.add_argument_group('required')
-    required.add_argument('-u', '--url', type=str, help='URL to use')
+    required.add_argument('-u', '--url', type=str, metavar="", help='URL to use')
     exclusive_required = required.add_mutually_exclusive_group(required=True)
     exclusive_required.add_argument('-c', '--current', action='store_true', help='Download the latest version of each file snapshot (opt range in y)')
     exclusive_required.add_argument('-f', '--full', action='store_true', help='Download snapshots of all timestamps (opt range in y)')
     exclusive_required.add_argument('-s', '--save', action='store_true', help='Save a page to the wayback machine')
 
     optional = parser.add_argument_group('optional')
     optional.add_argument('-l', '--list', action='store_true', help='Only print snapshots (opt range in y)')
     optional.add_argument('-e', '--explicit', action='store_true', help='Search only for the explicit given url')
-    optional.add_argument('-o', '--output', type=str, help='Output folder defaults to current directory')
-    optional.add_argument('-r', '--range', type=int, help='Range in years to search')
-    optional.add_argument('--start', type=int, help='Start timestamp format: YYYYMMDDhhmmss')
-    optional.add_argument('--end', type=int, help='End timestamp format: YYYYMMDDhhmmss')
+    optional.add_argument('-o', '--output', type=str, metavar="", help='Output folder defaults to current directory')
+    optional.add_argument('-r', '--range', type=int, metavar="", help='Range in years to search')
+    optional.add_argument('--start', type=int, metavar="", help='Start timestamp format: YYYYMMDDhhmmss')
+    optional.add_argument('--end', type=int, metavar="", help='End timestamp format: YYYYMMDDhhmmss')
 
     special = parser.add_argument_group('special')
-    special.add_argument('--csv', type=str, nargs='?', const=True, help='Save a csv file on a given path or defaults to the output folder')
+    special.add_argument('--csv', type=str, nargs='?', metavar='', help='Save a csv file on a given path or defaults to the output folder')
     special.add_argument('--no-redirect', action='store_true', help='Do not follow redirects by archive.org')
-    special.add_argument('--verbosity', type=str, default="standard", choices=["standard", "progress", "json"], help='Verbosity level')
-    special.add_argument('--retry', type=int, default=0, metavar="X-TIMES", help='Retry failed downloads (opt tries as int, else infinite)')
-    special.add_argument('--worker', type=int, default=1, metavar="AMOUNT", help='Number of worker (simultaneous downloads)')
+    special.add_argument('--verbosity', type=str, default="standard", metavar="", help='["progress", "json"] Verbosity level')
+    special.add_argument('--retry', type=int, default=0, metavar="", help='Retry failed downloads (opt tries as int, else infinite)')
+    special.add_argument('--workers', type=int, default=1, metavar="", help='Number of workers (simultaneous downloads)')
 
-    args = parser.parse_args()
+    args = parser.parse_args(args=None if sys.argv[1:] else ['--help']) # if no arguments are given, print help
 
     return args
```

### Comparing `pywaybackup-0.8.1/pywaybackup/main.py` & `pywaybackup-1.0.0/pywaybackup/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,24 @@
     if args.full:
         mode = "full"
     if args.current:
         mode = "current"
 
     if args.output is None:
         args.output = os.path.join(os.getcwd(), "waybackup_snapshots")
-    if args.csv is True:
+    if args.csv == "":
         args.csv = args.output
 
     if args.save:
         archive.save_page(args.url)
     else:
         archive.query_list(args.url, args.range, args.start, args.end, args.explicit, mode)
         if args.list:
             archive.print_list()
         else:
-            archive.download_list(args.output, args.retry, args.no_redirect, args.worker)
+            archive.download_list(args.output, args.retry, args.no_redirect, args.workers)
         if args.csv:
-            archive.save_csv(args.csv)
+            archive.save_csv(args.csv, args.url)
     v.close()
 
 if __name__ == "__main__":
     main()
```

### Comparing `pywaybackup-0.8.1/pywaybackup.egg-info/PKG-INFO` & `pywaybackup-1.0.0/pywaybackup.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pywaybackup
-Version: 0.8.1
+Version: 1.0.0
 Summary: Download snapshots from the Wayback Machine
 Home-page: https://github.com/bitdruid/python-wayback-machine-downloader
 Author: bitdruid
 Author-email: bitdruid@outlook.com
 License: MIT
 Keywords: wayback machine internet archive
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # archive wayback downloader
 
 [![PyPI](https://img.shields.io/pypi/v/pywaybackup)](https://pypi.org/project/pywaybackup/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pywaybackup)](https://pypi.org/project/pywaybackup/)
-![Release](https://img.shields.io/badge/Release-beta-orange)
 ![Python Version](https://img.shields.io/badge/Python-3.6-blue)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 Downloading archived web pages from the [Wayback Machine](https://archive.org/web/).
 
 Internet-archive is a nice source for several OSINT-information. This script is a work in progress to query and fetch archived web pages.
 
@@ -39,66 +38,70 @@
    ```pip install .```
    - in a virtual env or use `--break-system-package`
 
 ## Usage
 
 This script allows you to download content from the Wayback Machine (archive.org). You can use it to download either the latest version or all versions of web page snapshots within a specified range.
 
-<!-- ## Info -->
-
 ### Arguments
 
 - `-h`, `--help`: Show the help message and exit.
 - `-a`, `--about`: Show information about the script and exit.
 
 #### Required Arguments
 
-- `-u URL`, `--url URL`: The URL of the web page to download. This argument is required.
+- `-u`, `--url`: The URL of the web page to download. This argument is required.
 
 #### Mode Selection (Choose One)
 
-- `-c`, `--current`: Download the latest version of each file snapshot. You will get a rebuild of the current website with all available files.
+- `-c`, `--current`: Download the latest version of each file snapshot. You will get a rebuild of the current website with all available files (but not any original state because new and old versions are mixed).
 - `-f`, `--full`: Download snapshots of all timestamps. You will get a folder per timestamp with the files available at that time.
 - `-s`, `--save`: Save a page to the Wayback Machine. (beta)
 
 #### Optional Arguments
 
 - `-l`, `--list`: Only print the snapshots available within the specified range. Does not download the snapshots.
 - `-e`, `--explicit`: Only download the explicit given url. No wildcard subdomains or paths.
-- `-o OUTPUT`, `--output OUTPUT`: The folder where downloaded files will be saved.
+- `-o`, `--output`: The folder where downloaded files will be saved.
 
 - **Range Selection:**<br>
 Specify the range in years or a specific timestamp either start, end or both. If you specify the `range` argument, the `start` and `end` arguments will be ignored. Format for timestamps: YYYYMMDDhhmmss. You can only give a year or increase specificity by going through the timestamp starting on the left.<br>
 (year 2019, year+month 201901, year+month+day 20190101, year+month+day+hour 2019010112)
-   - `-r RANGE`, `--range RANGE`: Specify the range in years for which to search and download snapshots.
+   - `-r`, `--range`: Specify the range in years for which to search and download snapshots.
    - `--start`: Timestamp to start searching.
    - `--end`: Timestamp to end searching.
 
 #### Additional
 
-- `--csv`: Save a csv file with the list of snapshots inside the output folder.
+- `--csv`: Save a csv file with the list of snapshots inside the output folder or a specified folder. If you set `--list` the csv will contain the cdx list of snapshots. If you set either `--current` or `--full` the csv will contain the downloaded files.
 - `--no-redirect`: Do not follow redirects of snapshots. Archive.org sometimes redirects to a different snapshot for several reasons. Downloading redirects may lead to timestamp-folders which contain some files with a different timestamp. This does not matter if you only want to download the latest version (`-c`).
-- `--verbosity [LEVEL]`: Set the verbosity: json (print json response), progress (show progress bar) or standard (default).
-- `--retry [RETRY_FAILED]`: Retry failed downloads. You can specify the number of retry attempts as an integer.
-- `--worker [AMOUNT]`: The number of worker to use for downloading (simultaneous downloads). Default is 1. A safe spot is about 10 workers. Beware: Using too many worker will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
+- `--verbosity`: Set the verbosity: json (print json response), progress (show progress bar).
+- `--retry`: Retry failed downloads. You can specify the number of retry attempts as an integer.
+- `--workers`: The number of workers to use for downloading (simultaneous downloads). Default is 1. A safe spot is about 10 workers. Beware: Using too many workers will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
 
 ### Examples
 
 Download latest snapshot of all files:<br>
 `waybackup -u http://example.com -c`
 
 Download latest snapshot of all files with retries:<br>
 `waybackup -u http://example.com -c --retry 3`
 
-Download all snapshots sorted per timestamp with a specified range and follow redirects:<br>
-`waybackup -u http://example.com -f -r 5 --redirect`
+Download all snapshots sorted per timestamp with a specified range and do not follow redirects:<br>
+`waybackup -u http://example.com -f -r 5 --no-redirect`
+
+Download all snapshots sorted per timestamp with a specified range and save to a specified folder with 3 workers:<br>
+`waybackup -u http://example.com -f -r 5 -o /home/user/Downloads/snapshots --workers 3`
+
+Download all snapshots from 2020 to 12th of December 2022 with 4 workers, save a csv and show a progress bar:
+`waybackup -u http://example.com -f --start 2020 --end 20221212 --workers 4 --csv --verbosity progress`
 
-Download all snapshots sorted per timestamp with a specified range and save to a specified folder with 3 worker:<br>
-`waybackup -u http://example.com -f -r 5 -o /home/user/Downloads/snapshots --worker 3`
+Download all snapshots and output a json response:<br>
+`waybackup -u http://example.com -f --verbosity json`
 
-List available snapshots per timestamp without downloading:<br>
-`waybackup -u http://example.com -f -l`
+List available snapshots per timestamp without downloading and save a csv file to home folder:<br>
+`waybackup -u http://example.com -f -l --csv /home/user/Downloads`
 
 ## Contributing
 
 I'm always happy for some feature requests to improve the usability of this script.
 Feel free to give suggestions and report issues. Project is still far from being perfect.
```

### Comparing `pywaybackup-0.8.1/setup.py` & `pywaybackup-1.0.0/setup.py`

 * *Files identical despite different names*


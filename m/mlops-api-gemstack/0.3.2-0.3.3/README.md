# Comparing `tmp/mlops_api_gemstack-0.3.2.tar.gz` & `tmp/mlops_api_gemstack-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_api_gemstack-0.3.2.tar", last modified: Sat Apr 20 20:24:04 2024, max compression
+gzip compressed data, was "mlops_api_gemstack-0.3.3.tar", last modified: Mon Apr 22 05:04:59 2024, max compression
```

## Comparing `mlops_api_gemstack-0.3.2.tar` & `mlops_api_gemstack-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 20:24:04.179696 mlops_api_gemstack-0.3.2/
--rw-r--r--   0 ricardosun   (501) staff       (20)      344 2024-04-20 20:24:04.177610 mlops_api_gemstack-0.3.2/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)        0 2024-04-09 22:49:12.000000 mlops_api_gemstack-0.3.2/README.md
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 20:24:04.109075 mlops_api_gemstack-0.3.2/mlops_api_gemstack/
--rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3.2/mlops_api_gemstack/__init__.py
--rw-r--r--   0 ricardosun   (501) staff       (20)    12677 2024-04-20 20:22:49.000000 mlops_api_gemstack-0.3.2/mlops_api_gemstack/api.py
-drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-20 20:24:04.172913 mlops_api_gemstack-0.3.2/mlops_api_gemstack.egg-info/
--rw-r--r--   0 ricardosun   (501) staff       (20)      344 2024-04-20 20:24:03.000000 mlops_api_gemstack-0.3.2/mlops_api_gemstack.egg-info/PKG-INFO
--rw-r--r--   0 ricardosun   (501) staff       (20)      329 2024-04-20 20:24:03.000000 mlops_api_gemstack-0.3.2/mlops_api_gemstack.egg-info/SOURCES.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-20 20:24:03.000000 mlops_api_gemstack-0.3.2/mlops_api_gemstack.egg-info/dependency_links.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-20 20:24:03.000000 mlops_api_gemstack-0.3.2/mlops_api_gemstack.egg-info/entry_points.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-20 20:24:03.000000 mlops_api_gemstack-0.3.2/mlops_api_gemstack.egg-info/requires.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-20 20:24:03.000000 mlops_api_gemstack-0.3.2/mlops_api_gemstack.egg-info/top_level.txt
--rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-20 20:24:04.179869 mlops_api_gemstack-0.3.2/setup.cfg
--rw-r--r--   0 ricardosun   (501) staff       (20)      622 2024-04-20 20:22:55.000000 mlops_api_gemstack-0.3.2/setup.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-22 05:04:59.362135 mlops_api_gemstack-0.3.3/
+-rw-r--r--   0 ricardosun   (501) staff       (20)      344 2024-04-22 05:04:59.361573 mlops_api_gemstack-0.3.3/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)        0 2024-04-09 22:49:12.000000 mlops_api_gemstack-0.3.3/README.md
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-22 05:04:59.355685 mlops_api_gemstack-0.3.3/mlops_api_gemstack/
+-rw-r--r--   0 ricardosun   (501) staff       (20)       18 2024-04-20 05:10:06.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack/__init__.py
+-rw-r--r--   0 ricardosun   (501) staff       (20)    11792 2024-04-22 03:59:28.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack/api.py
+drwxr-xr-x   0 ricardosun   (501) staff       (20)        0 2024-04-22 05:04:59.360362 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/
+-rw-r--r--   0 ricardosun   (501) staff       (20)      344 2024-04-22 05:04:59.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/PKG-INFO
+-rw-r--r--   0 ricardosun   (501) staff       (20)      329 2024-04-22 05:04:59.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/SOURCES.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)        1 2024-04-22 05:04:59.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/dependency_links.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       50 2024-04-22 05:04:59.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/entry_points.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       37 2024-04-22 05:04:59.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/requires.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       19 2024-04-22 05:04:59.000000 mlops_api_gemstack-0.3.3/mlops_api_gemstack.egg-info/top_level.txt
+-rw-r--r--   0 ricardosun   (501) staff       (20)       38 2024-04-22 05:04:59.362357 mlops_api_gemstack-0.3.3/setup.cfg
+-rw-r--r--   0 ricardosun   (501) staff       (20)      622 2024-04-22 05:04:50.000000 mlops_api_gemstack-0.3.3/setup.py
```

### Comparing `mlops_api_gemstack-0.3.2/mlops_api_gemstack/api.py` & `mlops_api_gemstack-0.3.3/mlops_api_gemstack/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -281,34 +281,16 @@
 
     def stop_recording(sig, frame):
         print("Stopping rosbag recording")
         process.terminate()
         print("Recording stopped")
 
         # send rosbag file through api
-        with open(rosbag_file_name, 'rb') as f:
-            files = {'file': f}
-            response = requests.post(f"{base_url}/datasets/uploadBag", files=files)
-            if response.status_code == 200:
-                response_data = response.json()
-                click.echo(f"Message: {response_data['message']}.")
-
-                for inserted in response_data['inserted_objects']:
-                    response = requests.put(
-                        f"{base_url}/datasets/{inserted[1]}", 
-                        json={"Source": source}
-                    )
-                    if response.status_code == 200:
-                        click.echo("Dataset updated successfully")
-                        
-            elif response.status_code == 400:
-                click.echo(f"Error: {response.json()['error']}")
-            else:
-                click.echo(f"Failed to upload the file. Status code: {response.status_code}")
-
+        upload_bag(rosbag_file_name, source)
+       
         if delete_rosbag:
             print("Removing rosbag file")
             subprocess.run(f"rm {rosbag_file_name}", shell=True)
         exit(0)
 
     signal.signal(signal.SIGINT, stop_recording)
```

### Comparing `mlops_api_gemstack-0.3.2/setup.py` & `mlops_api_gemstack-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mlops_api_gemstack',
-    version='0.3.2',
+    version='0.3.3',
     description='An API package connect to a MLops server relating to the GEMstack project.',
     author='Haoming Sun',
     author_email='ricardosun990122@gmail.com',
     url='https://github.com/krishauser/GEMstack/tree/s2024_MLops/MLops/mlops_api_gemstack',
     packages=find_packages(),
     install_requires=[
         'requests',
```


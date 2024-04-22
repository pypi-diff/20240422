# Comparing `tmp/desktop_env-0.1.5.tar.gz` & `tmp/desktop_env-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop_env-0.1.5.tar", last modified: Sat Apr 13 15:46:58 2024, max compression
+gzip compressed data, was "desktop_env-0.1.6.tar", last modified: Mon Apr 22 08:40:02 2024, max compression
```

## Comparing `desktop_env-0.1.5.tar` & `desktop_env-0.1.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 15:46:58.598522 desktop_env-0.1.5/
--rw-rw-rw-   0        0        0    11358 2024-02-24 15:43:05.000000 desktop_env-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     8512 2024-04-13 15:46:58.598017 desktop_env-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6631 2024-04-13 14:15:25.000000 desktop_env-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 15:46:58.572721 desktop_env-0.1.5/desktop_env/
--rw-rw-rw-   0        0        0        2 2023-12-24 03:12:41.000000 desktop_env-0.1.5/desktop_env/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:46:58.582008 desktop_env-0.1.5/desktop_env/controllers/
--rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.5/desktop_env/controllers/__init__.py
--rw-rw-rw-   0        0        0    15393 2024-03-21 03:16:56.000000 desktop_env-0.1.5/desktop_env/controllers/python.py
--rw-rw-rw-   0        0        0    29975 2024-04-13 14:40:47.000000 desktop_env-0.1.5/desktop_env/controllers/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:46:58.584079 desktop_env-0.1.5/desktop_env/envs/
--rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.5/desktop_env/envs/__init__.py
--rw-rw-rw-   0        0        0     7377 2024-01-14 13:22:15.000000 desktop_env-0.1.5/desktop_env/envs/actions.py
--rw-rw-rw-   0        0        0    14755 2024-04-13 14:40:47.000000 desktop_env-0.1.5/desktop_env/envs/desktop_env.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:46:58.584079 desktop_env-0.1.5/desktop_env/evaluators/
--rw-rw-rw-   0        0        0      113 2023-12-24 05:57:07.000000 desktop_env-0.1.5/desktop_env/evaluators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:46:58.589480 desktop_env-0.1.5/desktop_env/evaluators/getters/
--rw-rw-rw-   0        0        0     1504 2024-04-13 14:50:54.000000 desktop_env-0.1.5/desktop_env/evaluators/getters/__init__.py
--rw-rw-rw-   0        0        0      537 2024-04-13 14:50:54.000000 desktop_env-0.1.5/desktop_env/evaluators/getters/calc.py
--rw-rw-rw-   0        0        0    62483 2024-04-01 11:46:38.000000 desktop_env-0.1.5/desktop_env/evaluators/getters/chrome.py
--rw-rw-rw-   0        0        0     4746 2024-03-10 07:16:40.000000 desktop_env-0.1.5/desktop_env/evaluators/getters/file.py
--rw-rw-rw-   0        0        0     1269 2024-03-08 12:39:20.000000 desktop_env-0.1.5/desktop_env/evaluators/getters/general.py
--rw-rw-rw-   0        0        0     1144 2024-01-30 18:56:45.000000 desktop_env-0.1.5/desktop_env/evaluators/getters/gimp.py
--rw-rw-rw-   0        0        0     7156 2024-03-08 11:36:11.000000 desktop_env-0.1.5/desktop_env/evaluators/getters/impress.py
--rw-rw-rw-   0        0        0      660 2024-01-26 05:22:46.000000 desktop_env-0.1.5/desktop_env/evaluators/getters/info.py
--rw-rw-rw-   0        0        0     7985 2024-03-08 12:47:17.000000 desktop_env-0.1.5/desktop_env/evaluators/getters/misc.py
--rw-rw-rw-   0        0        0      729 2024-01-13 16:57:53.000000 desktop_env-0.1.5/desktop_env/evaluators/getters/replay.py
--rw-rw-rw-   0        0        0     3768 2024-01-30 07:42:11.000000 desktop_env-0.1.5/desktop_env/evaluators/getters/vlc.py
--rw-rw-rw-   0        0        0     1113 2024-01-30 07:42:11.000000 desktop_env-0.1.5/desktop_env/evaluators/getters/vscode.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:46:58.597014 desktop_env-0.1.5/desktop_env/evaluators/metrics/
--rw-rw-rw-   0        0        0     4083 2024-04-13 14:50:54.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/__init__.py
--rw-rw-rw-   0        0        0     1877 2024-03-14 04:54:10.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/basic_os.py
--rw-rw-rw-   0        0        0    13473 2024-03-10 16:02:05.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/chrome.py
--rw-rw-rw-   0        0        0    28929 2024-04-02 06:37:07.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/docs.py
--rw-rw-rw-   0        0        0    17228 2024-04-01 06:53:32.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/general.py
--rw-rw-rw-   0        0        0    20366 2024-03-19 10:44:27.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/gimp.py
--rw-rw-rw-   0        0        0     1242 2024-03-14 04:54:10.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/libreoffice.py
--rw-rw-rw-   0        0        0     3316 2024-03-14 04:54:10.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/others.py
--rw-rw-rw-   0        0        0      832 2024-03-14 04:54:10.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/pdf.py
--rw-rw-rw-   0        0        0    22385 2024-03-21 14:05:41.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/slides.py
--rw-rw-rw-   0        0        0    23931 2024-03-14 04:54:10.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/table.py
--rw-rw-rw-   0        0        0     6801 2024-03-14 04:54:10.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/thunderbird.py
--rw-rw-rw-   0        0        0    29419 2024-03-08 12:47:17.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/utils.py
--rw-rw-rw-   0        0        0    14582 2024-01-25 04:36:46.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/vlc.py
--rw-rw-rw-   0        0        0     8034 2024-03-18 12:33:10.000000 desktop_env-0.1.5/desktop_env/evaluators/metrics/vscode.py
-drwxrwxrwx   0        0        0        0 2024-04-13 15:46:58.597014 desktop_env-0.1.5/desktop_env.egg-info/
--rw-rw-rw-   0        0        0     8512 2024-04-13 15:46:58.000000 desktop_env-0.1.5/desktop_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1552 2024-04-13 15:46:58.000000 desktop_env-0.1.5/desktop_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 15:46:58.000000 desktop_env-0.1.5/desktop_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      567 2024-04-13 15:46:58.000000 desktop_env-0.1.5/desktop_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-13 15:46:58.000000 desktop_env-0.1.5/desktop_env.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 15:46:58.598522 desktop_env-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2752 2024-04-13 15:46:56.000000 desktop_env-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:02.345753 desktop_env-0.1.6/
+-rw-rw-rw-   0        0        0    11358 2024-02-24 15:43:05.000000 desktop_env-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     9260 2024-04-22 08:40:02.345250 desktop_env-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7324 2024-04-21 11:49:28.000000 desktop_env-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:02.316320 desktop_env-0.1.6/desktop_env/
+-rw-rw-rw-   0        0        0        2 2023-12-24 03:12:41.000000 desktop_env-0.1.6/desktop_env/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:02.327461 desktop_env-0.1.6/desktop_env/controllers/
+-rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.6/desktop_env/controllers/__init__.py
+-rw-rw-rw-   0        0        0    15393 2024-03-21 03:16:56.000000 desktop_env-0.1.6/desktop_env/controllers/python.py
+-rw-rw-rw-   0        0        0    29975 2024-04-13 14:40:47.000000 desktop_env-0.1.6/desktop_env/controllers/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:02.329167 desktop_env-0.1.6/desktop_env/envs/
+-rw-rw-rw-   0        0        0    14132 2024-04-21 11:33:26.000000 desktop_env-0.1.6/desktop_env/envs/__init__.py
+-rw-rw-rw-   0        0        0     7377 2024-01-14 13:22:15.000000 desktop_env-0.1.6/desktop_env/envs/actions.py
+-rw-rw-rw-   0        0        0    14634 2024-04-21 11:31:18.000000 desktop_env-0.1.6/desktop_env/envs/desktop_env.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:02.329167 desktop_env-0.1.6/desktop_env/evaluators/
+-rw-rw-rw-   0        0        0      113 2023-12-24 05:57:07.000000 desktop_env-0.1.6/desktop_env/evaluators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:02.335199 desktop_env-0.1.6/desktop_env/evaluators/getters/
+-rw-rw-rw-   0        0        0     1504 2024-04-13 14:50:54.000000 desktop_env-0.1.6/desktop_env/evaluators/getters/__init__.py
+-rw-rw-rw-   0        0        0      537 2024-04-13 14:50:54.000000 desktop_env-0.1.6/desktop_env/evaluators/getters/calc.py
+-rw-rw-rw-   0        0        0    62483 2024-04-01 11:46:38.000000 desktop_env-0.1.6/desktop_env/evaluators/getters/chrome.py
+-rw-rw-rw-   0        0        0     4746 2024-03-10 07:16:40.000000 desktop_env-0.1.6/desktop_env/evaluators/getters/file.py
+-rw-rw-rw-   0        0        0     1269 2024-03-08 12:39:20.000000 desktop_env-0.1.6/desktop_env/evaluators/getters/general.py
+-rw-rw-rw-   0        0        0     1144 2024-01-30 18:56:45.000000 desktop_env-0.1.6/desktop_env/evaluators/getters/gimp.py
+-rw-rw-rw-   0        0        0     7156 2024-03-08 11:36:11.000000 desktop_env-0.1.6/desktop_env/evaluators/getters/impress.py
+-rw-rw-rw-   0        0        0      660 2024-01-26 05:22:46.000000 desktop_env-0.1.6/desktop_env/evaluators/getters/info.py
+-rw-rw-rw-   0        0        0     7985 2024-03-08 12:47:17.000000 desktop_env-0.1.6/desktop_env/evaluators/getters/misc.py
+-rw-rw-rw-   0        0        0      729 2024-01-13 16:57:53.000000 desktop_env-0.1.6/desktop_env/evaluators/getters/replay.py
+-rw-rw-rw-   0        0        0     3768 2024-01-30 07:42:11.000000 desktop_env-0.1.6/desktop_env/evaluators/getters/vlc.py
+-rw-rw-rw-   0        0        0     1113 2024-01-30 07:42:11.000000 desktop_env-0.1.6/desktop_env/evaluators/getters/vscode.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:02.344245 desktop_env-0.1.6/desktop_env/evaluators/metrics/
+-rw-rw-rw-   0        0        0     4083 2024-04-13 14:50:54.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1877 2024-03-14 04:54:10.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/basic_os.py
+-rw-rw-rw-   0        0        0    13473 2024-03-10 16:02:05.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/chrome.py
+-rw-rw-rw-   0        0        0    28929 2024-04-02 06:37:07.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/docs.py
+-rw-rw-rw-   0        0        0    17228 2024-04-01 06:53:32.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/general.py
+-rw-rw-rw-   0        0        0    20366 2024-03-19 10:44:27.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/gimp.py
+-rw-rw-rw-   0        0        0     1242 2024-03-14 04:54:10.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/libreoffice.py
+-rw-rw-rw-   0        0        0     3316 2024-03-14 04:54:10.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/others.py
+-rw-rw-rw-   0        0        0      832 2024-03-14 04:54:10.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/pdf.py
+-rw-rw-rw-   0        0        0    22385 2024-03-21 14:05:41.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/slides.py
+-rw-rw-rw-   0        0        0    23931 2024-03-14 04:54:10.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/table.py
+-rw-rw-rw-   0        0        0     6801 2024-03-14 04:54:10.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/thunderbird.py
+-rw-rw-rw-   0        0        0    29419 2024-03-08 12:47:17.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/utils.py
+-rw-rw-rw-   0        0        0    14582 2024-01-25 04:36:46.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/vlc.py
+-rw-rw-rw-   0        0        0     8034 2024-03-18 12:33:10.000000 desktop_env-0.1.6/desktop_env/evaluators/metrics/vscode.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:40:02.344245 desktop_env-0.1.6/desktop_env.egg-info/
+-rw-rw-rw-   0        0        0     9260 2024-04-22 08:40:02.000000 desktop_env-0.1.6/desktop_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1552 2024-04-22 08:40:02.000000 desktop_env-0.1.6/desktop_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 08:40:02.000000 desktop_env-0.1.6/desktop_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      567 2024-04-22 08:40:02.000000 desktop_env-0.1.6/desktop_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-22 08:40:02.000000 desktop_env-0.1.6/desktop_env.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 08:40:02.345753 desktop_env-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     2805 2024-04-22 08:39:59.000000 desktop_env-0.1.6/setup.py
```

### Comparing `desktop_env-0.1.5/LICENSE` & `desktop_env-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/PKG-INFO` & `desktop_env-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: desktop_env
-Version: 0.1.5
+Version: 0.1.6
 Summary: The package provides a desktop environment for setting and evaluating desktop automation tasks.
 Home-page: https://github.com/xlang-ai/desktop_env
-Author: Tianbao Xie, Danyang Zhang, Toh Jing Hua, etc.
+Author: Tianbao Xie, Danyang Zhang,  Jixuan Chen, Xiaochuan Li, Siheng Zhao, Ruisheng Cao, Toh Jing Hua, etc.
 Author-email: tianbaoxiexxx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -67,14 +67,34 @@
   <a href="https://os-world.github.io/">Website</a> •
   <a href="https://arxiv.org/abs/2404.07972">Paper</a> •
   <a href="https://github.com/xlang-ai/OSWorld/tree/main/evaluation_examples">Data</a> •
   <a href="https://os-world.github.io/explorer.html">Data Viewer</a> •
   <a href="https://discord.gg/4Gnw7eTEZR">Discord</a>
 </p>
 
+<p align="center">
+    <a href="https://img.shields.io/badge/PRs-Welcome-red">
+        <img src="https://img.shields.io/badge/PRs-Welcome-red">
+    </a>
+    <a href="https://img.shields.io/github/last-commit/xlang-ai/OSWorld?color=green">
+        <img src="https://img.shields.io/github/last-commit/xlang-ai/OSWorld?color=green">
+    </a>
+    <a href="https://opensource.org/licenses/Apache-2.0">
+        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg">
+    </a>
+    <a href="https://badge.fury.io/py/desktop-env">
+        <img src="https://badge.fury.io/py/desktop-env.svg">
+    </a>
+    <a href="https://pepy.tech/project/desktop-env">
+        <img src="https://static.pepy.tech/badge/desktop-env">
+    </a>
+    <br/>
+</p>
+
+
 ## 📢 Updates
 - 2024-04-11: We released our [paper](https://arxiv.org/abs/2404.07972), [environment and benchmark](https://github.com/xlang-ai/OSWorld), and [project page](https://os-world.github.io/). Check it out!
 
 ## 💾 Installation
 ### On Your Desktop or Server (Non-Virtualized Platform)
 Suppose you are operating on a system that has not been virtualized, meaning you are not utilizing a virtualized environment like AWS, Azure, or k8s. If this is the case, proceed with the instructions below. However, if you are on a virtualized platform, please refer to the [virtualized platform](https://github.com/xlang-ai/OSWorld?tab=readme-ov-file#virtualized-platform) section.
 
@@ -101,18 +121,15 @@
 
 2. Install [VMware Workstation Pro](https://www.vmware.com/products/workstation-pro/workstation-pro-evaluation.html) (for systems with Apple Chips, you should install [VMware Fusion](https://www.vmware.com/go/getfusion)) and configure the `vmrun` command. Verify the successful installation by running the following:
 ```bash
 vmrun -T ws list
 ```
 If the installation along with the environment variable set is successful, you will see the message showing the current running virtual machines.
 
-3. Run our setup script to download the necessary virtual machines and set up the environment☕:
-```bash
-python setup_vm.py
-```
+All set! Our setup script will automatically download the necessary virtual machines and configure the environment for you.
 
 ### On AWS or Azure (Virtualized platform)
 We are working on supporting it 👷. Please hold tight!
 
 ## 🚀 Quick Start
 Run the following minimal example to interact with the environment:
 ```python
@@ -145,18 +162,15 @@
                 "include": ["spotify"],
                 "exclude": ["not found"]
             }
         }
     }
 }
 
-env = DesktopEnv(
-    path_to_vm=r"Ubuntu/DesktopEnv-Ubuntu 64-bit Arm.vmx",
-    action_space="pyautogui"
-)
+env = DesktopEnv(action_space="pyautogui")
 
 obs = env.reset(task_config=example)
 obs, reward, done, info = env.step("pyautogui.rightClick()")
 ```
 You will see all the logs of the system running normally, including the successful creation of the environment, completion of setup, and successful execution of actions. In the end, you will observe a successful right-click on the screen, which means you are ready to go.
 
 ## 🧪 Experiments
```

#### html2text {}

```diff
@@ -1,34 +1,38 @@
-Metadata-Version: 2.1 Name: desktop_env Version: 0.1.5 Summary: The package
+Metadata-Version: 2.1 Name: desktop_env Version: 0.1.6 Summary: The package
 provides a desktop environment for setting and evaluating desktop automation
 tasks. Home-page: https://github.com/xlang-ai/desktop_env Author: Tianbao Xie,
-Danyang Zhang, Toh Jing Hua, etc. Author-email: tianbaoxiexxx@gmail.com
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: numpy~=1.24.3 Requires-Dist:
-Pillow~=10.1.0 Requires-Dist: fabric Requires-Dist: gymnasium~=0.28.1 Requires-
-Dist: requests~=2.31.0 Requires-Dist: transformers~=4.35.2 Requires-Dist:
-torch~=2.1.1 Requires-Dist: accelerate Requires-Dist: opencv-python~=4.8.1.78
-Requires-Dist: matplotlib~=3.7.4 Requires-Dist: pynput~=1.7.6 Requires-Dist:
-pyautogui~=0.9.54 Requires-Dist: psutil~=5.9.6 Requires-Dist: tqdm~=4.65.0
-Requires-Dist: pandas~=2.0.3 Requires-Dist: flask~=3.0.0 Requires-Dist:
-requests-toolbelt~=1.0.0 Requires-Dist: lxml Requires-Dist: cssselect Requires-
-Dist: xmltodict Requires-Dist: openpyxl Requires-Dist: python-docx Requires-
-Dist: python-pptx Requires-Dist: pypdf Requires-Dist: PyGetWindow Requires-
-Dist: rapidfuzz Requires-Dist: pyacoustid Requires-Dist: opencv-python
-Requires-Dist: ImageHash Requires-Dist: scikit-image Requires-Dist: librosa
-Requires-Dist: pymupdf Requires-Dist: chardet Requires-Dist: playwright
-Requires-Dist: formulas Requires-Dist: pydrive Requires-Dist: fastdtw Requires-
-Dist: odfpy Requires-Dist: func-timeout Requires-Dist: beautifulsoup4 Requires-
-Dist: PyYaml Requires-Dist: mutagen Requires-Dist: easyocr Requires-Dist: borb
-Requires-Dist: pypdf2 Requires-Dist: pdfplumber Requires-Dist:
-wrapt_timeout_decorator
+Danyang Zhang, Jixuan Chen, Xiaochuan Li, Siheng Zhao, Ruisheng Cao, Toh Jing
+Hua, etc. Author-email: tianbaoxiexxx@gmail.com Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.9
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+numpy~=1.24.3 Requires-Dist: Pillow~=10.1.0 Requires-Dist: fabric Requires-
+Dist: gymnasium~=0.28.1 Requires-Dist: requests~=2.31.0 Requires-Dist:
+transformers~=4.35.2 Requires-Dist: torch~=2.1.1 Requires-Dist: accelerate
+Requires-Dist: opencv-python~=4.8.1.78 Requires-Dist: matplotlib~=3.7.4
+Requires-Dist: pynput~=1.7.6 Requires-Dist: pyautogui~=0.9.54 Requires-Dist:
+psutil~=5.9.6 Requires-Dist: tqdm~=4.65.0 Requires-Dist: pandas~=2.0.3
+Requires-Dist: flask~=3.0.0 Requires-Dist: requests-toolbelt~=1.0.0 Requires-
+Dist: lxml Requires-Dist: cssselect Requires-Dist: xmltodict Requires-Dist:
+openpyxl Requires-Dist: python-docx Requires-Dist: python-pptx Requires-Dist:
+pypdf Requires-Dist: PyGetWindow Requires-Dist: rapidfuzz Requires-Dist:
+pyacoustid Requires-Dist: opencv-python Requires-Dist: ImageHash Requires-Dist:
+scikit-image Requires-Dist: librosa Requires-Dist: pymupdf Requires-Dist:
+chardet Requires-Dist: playwright Requires-Dist: formulas Requires-Dist:
+pydrive Requires-Dist: fastdtw Requires-Dist: odfpy Requires-Dist: func-timeout
+Requires-Dist: beautifulsoup4 Requires-Dist: PyYaml Requires-Dist: mutagen
+Requires-Dist: easyocr Requires-Dist: borb Requires-Dist: pypdf2 Requires-Dist:
+pdfplumber Requires-Dist: wrapt_timeout_decorator
                                    [Banner]
             _W_e_b_s_i_t_e â¢ _P_a_p_e_r â¢ _D_a_t_a â¢ _D_a_t_a_ _V_i_e_w_e_r â¢ _D_i_s_c_o_r_d
+ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_R_s_-_W_e_l_c_o_m_e_-_r_e_d_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
+_l_a_s_t_-_c_o_m_m_i_t_/_x_l_a_n_g_-_a_i_/_O_S_W_o_r_l_d_?_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-
+   _A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_d_e_s_k_t_o_p_-_e_n_v_._s_v_g_]_[_h_t_t_p_s_:_/_/
+                      _s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_d_e_s_k_t_o_p_-_e_n_v_]
 ## ð¢ Updates - 2024-04-11: We released our [paper](https://arxiv.org/abs/
 2404.07972), [environment and benchmark](https://github.com/xlang-ai/OSWorld),
 and [project page](https://os-world.github.io/). Check it out! ## ð¾
 Installation ### On Your Desktop or Server (Non-Virtualized Platform) Suppose
 you are operating on a system that has not been virtualized, meaning you are
 not utilizing a virtualized environment like AWS, Azure, or k8s. If this is the
 case, proceed with the instructions below. However, if you are on a virtualized
@@ -46,35 +50,34 @@
 any benchmark tasks: ```bash pip install desktop-env ``` 2. Install [VMware
 Workstation Pro](https://www.vmware.com/products/workstation-pro/workstation-
 pro-evaluation.html) (for systems with Apple Chips, you should install [VMware
 Fusion](https://www.vmware.com/go/getfusion)) and configure the `vmrun`
 command. Verify the successful installation by running the following: ```bash
 vmrun -T ws list ``` If the installation along with the environment variable
 set is successful, you will see the message showing the current running virtual
-machines. 3. Run our setup script to download the necessary virtual machines
-and set up the environmentâ: ```bash python setup_vm.py ``` ### On AWS or
-Azure (Virtualized platform) We are working on supporting it ð·. Please hold
-tight! ## ð Quick Start Run the following minimal example to interact with
-the environment: ```python from desktop_env.envs.desktop_env import DesktopEnv
+machines. All set! Our setup script will automatically download the necessary
+virtual machines and configure the environment for you. ### On AWS or Azure
+(Virtualized platform) We are working on supporting it ð·. Please hold tight!
+## ð Quick Start Run the following minimal example to interact with the
+environment: ```python from desktop_env.envs.desktop_env import DesktopEnv
 example = { "id": "94d95f96-9699-4208-98ba-3c3119edf9c2", "instruction": "I
 want to install Spotify on my current system. Could you please help me?",
 "config": [ { "type": "execute", "parameters": { "command": [ "python", "-c",
 "import pyautogui; import time; pyautogui.click(960, 540); time.sleep(0.5);" ]
 } } ], "evaluator": { "func": "check_include_exclude", "result": { "type":
 "vm_command_line", "command": "which spotify" }, "expected": { "type": "rule",
 "rules": { "include": ["spotify"], "exclude": ["not found"] } } } } env =
-DesktopEnv( path_to_vm=r"Ubuntu/DesktopEnv-Ubuntu 64-bit Arm.vmx",
-action_space="pyautogui" ) obs = env.reset(task_config=example) obs, reward,
-done, info = env.step("pyautogui.rightClick()") ``` You will see all the logs
-of the system running normally, including the successful creation of the
-environment, completion of setup, and successful execution of actions. In the
-end, you will observe a successful right-click on the screen, which means you
-are ready to go. ## ð§ª Experiments ### Agent Baselines If you wish to run the
-baseline agent used in our paper, you can execute the following command as an
-example under the GPT-4V pure-screenshot setting: ```bash python run.py --
+DesktopEnv(action_space="pyautogui") obs = env.reset(task_config=example) obs,
+reward, done, info = env.step("pyautogui.rightClick()") ``` You will see all
+the logs of the system running normally, including the successful creation of
+the environment, completion of setup, and successful execution of actions. In
+the end, you will observe a successful right-click on the screen, which means
+you are ready to go. ## ð§ª Experiments ### Agent Baselines If you wish to run
+the baseline agent used in our paper, you can execute the following command as
+an example under the GPT-4V pure-screenshot setting: ```bash python run.py --
 path_to_vm Ubuntu/Ubuntu.vmx --headless --observation_type screenshot --model
 gpt-4-vision-preview --result_dir ./results ``` The results, which include
 screenshots, actions, and video recordings of the agent's task completion, will
 be saved in the `./results` directory in this case. You can then run the
 following command to obtain the result: ```bash python show_result.py ``` ###
 Evaluation Please start by reading through the [agent interface](https://
 github.com/xlang-ai/OSWorld/blob/main/mm_agents/README.md) and the [environment
```

### Comparing `desktop_env-0.1.5/README.md` & `desktop_env-0.1.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,34 @@
   <a href="https://os-world.github.io/">Website</a> •
   <a href="https://arxiv.org/abs/2404.07972">Paper</a> •
   <a href="https://github.com/xlang-ai/OSWorld/tree/main/evaluation_examples">Data</a> •
   <a href="https://os-world.github.io/explorer.html">Data Viewer</a> •
   <a href="https://discord.gg/4Gnw7eTEZR">Discord</a>
 </p>
 
+<p align="center">
+    <a href="https://img.shields.io/badge/PRs-Welcome-red">
+        <img src="https://img.shields.io/badge/PRs-Welcome-red">
+    </a>
+    <a href="https://img.shields.io/github/last-commit/xlang-ai/OSWorld?color=green">
+        <img src="https://img.shields.io/github/last-commit/xlang-ai/OSWorld?color=green">
+    </a>
+    <a href="https://opensource.org/licenses/Apache-2.0">
+        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg">
+    </a>
+    <a href="https://badge.fury.io/py/desktop-env">
+        <img src="https://badge.fury.io/py/desktop-env.svg">
+    </a>
+    <a href="https://pepy.tech/project/desktop-env">
+        <img src="https://static.pepy.tech/badge/desktop-env">
+    </a>
+    <br/>
+</p>
+
+
 ## 📢 Updates
 - 2024-04-11: We released our [paper](https://arxiv.org/abs/2404.07972), [environment and benchmark](https://github.com/xlang-ai/OSWorld), and [project page](https://os-world.github.io/). Check it out!
 
 ## 💾 Installation
 ### On Your Desktop or Server (Non-Virtualized Platform)
 Suppose you are operating on a system that has not been virtualized, meaning you are not utilizing a virtualized environment like AWS, Azure, or k8s. If this is the case, proceed with the instructions below. However, if you are on a virtualized platform, please refer to the [virtualized platform](https://github.com/xlang-ai/OSWorld?tab=readme-ov-file#virtualized-platform) section.
 
@@ -40,18 +60,15 @@
 
 2. Install [VMware Workstation Pro](https://www.vmware.com/products/workstation-pro/workstation-pro-evaluation.html) (for systems with Apple Chips, you should install [VMware Fusion](https://www.vmware.com/go/getfusion)) and configure the `vmrun` command. Verify the successful installation by running the following:
 ```bash
 vmrun -T ws list
 ```
 If the installation along with the environment variable set is successful, you will see the message showing the current running virtual machines.
 
-3. Run our setup script to download the necessary virtual machines and set up the environment☕:
-```bash
-python setup_vm.py
-```
+All set! Our setup script will automatically download the necessary virtual machines and configure the environment for you.
 
 ### On AWS or Azure (Virtualized platform)
 We are working on supporting it 👷. Please hold tight!
 
 ## 🚀 Quick Start
 Run the following minimal example to interact with the environment:
 ```python
@@ -84,18 +101,15 @@
                 "include": ["spotify"],
                 "exclude": ["not found"]
             }
         }
     }
 }
 
-env = DesktopEnv(
-    path_to_vm=r"Ubuntu/DesktopEnv-Ubuntu 64-bit Arm.vmx",
-    action_space="pyautogui"
-)
+env = DesktopEnv(action_space="pyautogui")
 
 obs = env.reset(task_config=example)
 obs, reward, done, info = env.step("pyautogui.rightClick()")
 ```
 You will see all the logs of the system running normally, including the successful creation of the environment, completion of setup, and successful execution of actions. In the end, you will observe a successful right-click on the screen, which means you are ready to go.
 
 ## 🧪 Experiments
```

#### html2text {}

```diff
@@ -1,9 +1,13 @@
                                    [Banner]
             _W_e_b_s_i_t_e â¢ _P_a_p_e_r â¢ _D_a_t_a â¢ _D_a_t_a_ _V_i_e_w_e_r â¢ _D_i_s_c_o_r_d
+ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_R_s_-_W_e_l_c_o_m_e_-_r_e_d_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
+_l_a_s_t_-_c_o_m_m_i_t_/_x_l_a_n_g_-_a_i_/_O_S_W_o_r_l_d_?_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-
+   _A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_d_e_s_k_t_o_p_-_e_n_v_._s_v_g_]_[_h_t_t_p_s_:_/_/
+                      _s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_d_e_s_k_t_o_p_-_e_n_v_]
 ## ð¢ Updates - 2024-04-11: We released our [paper](https://arxiv.org/abs/
 2404.07972), [environment and benchmark](https://github.com/xlang-ai/OSWorld),
 and [project page](https://os-world.github.io/). Check it out! ## ð¾
 Installation ### On Your Desktop or Server (Non-Virtualized Platform) Suppose
 you are operating on a system that has not been virtualized, meaning you are
 not utilizing a virtualized environment like AWS, Azure, or k8s. If this is the
 case, proceed with the instructions below. However, if you are on a virtualized
@@ -21,35 +25,34 @@
 any benchmark tasks: ```bash pip install desktop-env ``` 2. Install [VMware
 Workstation Pro](https://www.vmware.com/products/workstation-pro/workstation-
 pro-evaluation.html) (for systems with Apple Chips, you should install [VMware
 Fusion](https://www.vmware.com/go/getfusion)) and configure the `vmrun`
 command. Verify the successful installation by running the following: ```bash
 vmrun -T ws list ``` If the installation along with the environment variable
 set is successful, you will see the message showing the current running virtual
-machines. 3. Run our setup script to download the necessary virtual machines
-and set up the environmentâ: ```bash python setup_vm.py ``` ### On AWS or
-Azure (Virtualized platform) We are working on supporting it ð·. Please hold
-tight! ## ð Quick Start Run the following minimal example to interact with
-the environment: ```python from desktop_env.envs.desktop_env import DesktopEnv
+machines. All set! Our setup script will automatically download the necessary
+virtual machines and configure the environment for you. ### On AWS or Azure
+(Virtualized platform) We are working on supporting it ð·. Please hold tight!
+## ð Quick Start Run the following minimal example to interact with the
+environment: ```python from desktop_env.envs.desktop_env import DesktopEnv
 example = { "id": "94d95f96-9699-4208-98ba-3c3119edf9c2", "instruction": "I
 want to install Spotify on my current system. Could you please help me?",
 "config": [ { "type": "execute", "parameters": { "command": [ "python", "-c",
 "import pyautogui; import time; pyautogui.click(960, 540); time.sleep(0.5);" ]
 } } ], "evaluator": { "func": "check_include_exclude", "result": { "type":
 "vm_command_line", "command": "which spotify" }, "expected": { "type": "rule",
 "rules": { "include": ["spotify"], "exclude": ["not found"] } } } } env =
-DesktopEnv( path_to_vm=r"Ubuntu/DesktopEnv-Ubuntu 64-bit Arm.vmx",
-action_space="pyautogui" ) obs = env.reset(task_config=example) obs, reward,
-done, info = env.step("pyautogui.rightClick()") ``` You will see all the logs
-of the system running normally, including the successful creation of the
-environment, completion of setup, and successful execution of actions. In the
-end, you will observe a successful right-click on the screen, which means you
-are ready to go. ## ð§ª Experiments ### Agent Baselines If you wish to run the
-baseline agent used in our paper, you can execute the following command as an
-example under the GPT-4V pure-screenshot setting: ```bash python run.py --
+DesktopEnv(action_space="pyautogui") obs = env.reset(task_config=example) obs,
+reward, done, info = env.step("pyautogui.rightClick()") ``` You will see all
+the logs of the system running normally, including the successful creation of
+the environment, completion of setup, and successful execution of actions. In
+the end, you will observe a successful right-click on the screen, which means
+you are ready to go. ## ð§ª Experiments ### Agent Baselines If you wish to run
+the baseline agent used in our paper, you can execute the following command as
+an example under the GPT-4V pure-screenshot setting: ```bash python run.py --
 path_to_vm Ubuntu/Ubuntu.vmx --headless --observation_type screenshot --model
 gpt-4-vision-preview --result_dir ./results ``` The results, which include
 screenshots, actions, and video recordings of the agent's task completion, will
 be saved in the `./results` directory in this case. You can then run the
 following command to obtain the result: ```bash python show_result.py ``` ###
 Evaluation Please start by reading through the [agent interface](https://
 github.com/xlang-ai/OSWorld/blob/main/mm_agents/README.md) and the [environment
```

### Comparing `desktop_env-0.1.5/desktop_env/controllers/python.py` & `desktop_env-0.1.6/desktop_env/controllers/python.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/controllers/setup.py` & `desktop_env-0.1.6/desktop_env/controllers/setup.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/envs/actions.py` & `desktop_env-0.1.6/desktop_env/envs/actions.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/envs/desktop_env.py` & `desktop_env-0.1.6/desktop_env/envs/desktop_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import List, Dict, Union
 
 import gymnasium as gym
 
 from desktop_env.controllers.python import PythonController
 from desktop_env.controllers.setup import SetupController
 from desktop_env.evaluators import metrics, getters
+from . import _get_vm_path
 
 logger = logging.getLogger("desktopenv.env")
 
 Metric = Callable[[Any, Any], float]
 Getter = Callable[[gym.Env, Dict[str, Any]], Any]
 
 
@@ -41,15 +42,15 @@
 class DesktopEnv(gym.Env):
     """
     DesktopEnv with OpenAI Gym interface. It provides a desktop environment for setting and evaluating desktop automation tasks.
     """
 
     def __init__(
             self,
-            path_to_vm: str,
+            path_to_vm: str = None,
             snapshot_name: str = "init_state",
             action_space: str = "computer_13",
             cache_dir: str = "cache",
             screen_size: Tuple[int] = (1920, 1080),
             headless: bool = False,
             require_a11y_tree: bool = True,
             require_terminal: bool = False,
@@ -64,44 +65,48 @@
             screen_size (Tuple[int]): screen size of the VM
             headless (bool): whether to run the VM in headless mode
             require_a11y_tree (bool): whether to require accessibility tree
             require_terminal (bool): whether to require terminal output
         """
 
         # Initialize environment variables
-        self.path_to_vm = os.path.abspath(os.path.expandvars(os.path.expanduser(path_to_vm)))
+        self.path_to_vm = os.path.abspath(os.path.expandvars(os.path.expanduser(path_to_vm if path_to_vm else _get_vm_path())))
         self.snapshot_name = snapshot_name
         self.cache_dir_base: str = cache_dir
-        self.vm_screen_size = screen_size  # todo: add the logic to get the screen size from the VM
+        # todo: add the logic to get the screen size from the VM
         self.headless = headless
         self.require_a11y_tree = require_a11y_tree
         self.require_terminal = require_terminal
 
         # Initialize emulator and controller
         logger.info("Initializing...")
         self._start_emulator()
         self.vm_ip = self._get_vm_ip()
         self.controller = PythonController(vm_ip=self.vm_ip)
         self.setup_controller = SetupController(vm_ip=self.vm_ip, cache_dir=self.cache_dir_base)
 
-        # Meta info of the VM
-        self.vm_platform: str = self.controller.get_vm_platform()
-        self.vm_screen_size = self.controller.get_vm_screen_size()
-
         # mode: human or machine
         self.instruction = None
         assert action_space in ["computer_13", "pyautogui"]
         self.action_space = action_space
 
         # episodic stuffs, like counters, will be updated or reset
         # when calling self.reset()
         self._traj_no: int = -1
         self._step_no: int = 0
         self.action_history: List[Dict[str, any]] = []
 
+    @property
+    def vm_platform(self):
+        return self.controller.get_vm_platform()
+
+    @property
+    def vm_screen_size(self):
+        return self.controller.get_vm_screen_size()
+
     def _start_emulator(self):
         while True:
             try:
                 output = subprocess.check_output("vmrun -T ws list", shell=True, stderr=subprocess.STDOUT)
                 output = output.decode()
                 output: List[str] = output.splitlines()
                 # if self.path_to_vm.lstrip("~/") in output:
@@ -225,18 +230,14 @@
         _execute_command(["vmrun", "-T", "ws", "revertToSnapshot", self.path_to_vm, self.snapshot_name])
         time.sleep(5)
 
         logger.info("Starting emulator...")
         self._start_emulator()
         logger.info("Emulator started.")
 
-        logger.info("Get meta info of the VM...")
-        self.vm_platform = self.controller.get_vm_platform()
-        self.vm_screen_size = self.controller.get_vm_screen_size()
-
         logger.info("Setting up environment...")
         self.setup_controller.setup(self.config)
 
         time.sleep(5)
         logger.info("Environment setup complete.")
 
         observation = self._get_obs()
```

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/getters/__init__.py` & `desktop_env-0.1.6/desktop_env/evaluators/getters/__init__.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/getters/calc.py` & `desktop_env-0.1.6/desktop_env/evaluators/getters/calc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/getters/chrome.py` & `desktop_env-0.1.6/desktop_env/evaluators/getters/chrome.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/getters/file.py` & `desktop_env-0.1.6/desktop_env/evaluators/getters/file.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/getters/general.py` & `desktop_env-0.1.6/desktop_env/evaluators/getters/general.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/getters/gimp.py` & `desktop_env-0.1.6/desktop_env/evaluators/getters/gimp.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/getters/impress.py` & `desktop_env-0.1.6/desktop_env/evaluators/getters/impress.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/getters/info.py` & `desktop_env-0.1.6/desktop_env/evaluators/getters/info.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/getters/misc.py` & `desktop_env-0.1.6/desktop_env/evaluators/getters/misc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/getters/replay.py` & `desktop_env-0.1.6/desktop_env/evaluators/getters/replay.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/getters/vlc.py` & `desktop_env-0.1.6/desktop_env/evaluators/getters/vlc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/getters/vscode.py` & `desktop_env-0.1.6/desktop_env/evaluators/getters/vscode.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/__init__.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/basic_os.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/basic_os.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/chrome.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/chrome.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/docs.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/docs.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/general.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/general.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/gimp.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/gimp.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/libreoffice.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/libreoffice.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/others.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/others.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/pdf.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/pdf.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/slides.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/slides.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/table.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/table.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/thunderbird.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/thunderbird.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/utils.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/vlc.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/vlc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env/evaluators/metrics/vscode.py` & `desktop_env-0.1.6/desktop_env/evaluators/metrics/vscode.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env.egg-info/PKG-INFO` & `desktop_env-0.1.6/desktop_env.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: desktop_env
-Version: 0.1.5
+Version: 0.1.6
 Summary: The package provides a desktop environment for setting and evaluating desktop automation tasks.
 Home-page: https://github.com/xlang-ai/desktop_env
-Author: Tianbao Xie, Danyang Zhang, Toh Jing Hua, etc.
+Author: Tianbao Xie, Danyang Zhang,  Jixuan Chen, Xiaochuan Li, Siheng Zhao, Ruisheng Cao, Toh Jing Hua, etc.
 Author-email: tianbaoxiexxx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -67,14 +67,34 @@
   <a href="https://os-world.github.io/">Website</a> •
   <a href="https://arxiv.org/abs/2404.07972">Paper</a> •
   <a href="https://github.com/xlang-ai/OSWorld/tree/main/evaluation_examples">Data</a> •
   <a href="https://os-world.github.io/explorer.html">Data Viewer</a> •
   <a href="https://discord.gg/4Gnw7eTEZR">Discord</a>
 </p>
 
+<p align="center">
+    <a href="https://img.shields.io/badge/PRs-Welcome-red">
+        <img src="https://img.shields.io/badge/PRs-Welcome-red">
+    </a>
+    <a href="https://img.shields.io/github/last-commit/xlang-ai/OSWorld?color=green">
+        <img src="https://img.shields.io/github/last-commit/xlang-ai/OSWorld?color=green">
+    </a>
+    <a href="https://opensource.org/licenses/Apache-2.0">
+        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg">
+    </a>
+    <a href="https://badge.fury.io/py/desktop-env">
+        <img src="https://badge.fury.io/py/desktop-env.svg">
+    </a>
+    <a href="https://pepy.tech/project/desktop-env">
+        <img src="https://static.pepy.tech/badge/desktop-env">
+    </a>
+    <br/>
+</p>
+
+
 ## 📢 Updates
 - 2024-04-11: We released our [paper](https://arxiv.org/abs/2404.07972), [environment and benchmark](https://github.com/xlang-ai/OSWorld), and [project page](https://os-world.github.io/). Check it out!
 
 ## 💾 Installation
 ### On Your Desktop or Server (Non-Virtualized Platform)
 Suppose you are operating on a system that has not been virtualized, meaning you are not utilizing a virtualized environment like AWS, Azure, or k8s. If this is the case, proceed with the instructions below. However, if you are on a virtualized platform, please refer to the [virtualized platform](https://github.com/xlang-ai/OSWorld?tab=readme-ov-file#virtualized-platform) section.
 
@@ -101,18 +121,15 @@
 
 2. Install [VMware Workstation Pro](https://www.vmware.com/products/workstation-pro/workstation-pro-evaluation.html) (for systems with Apple Chips, you should install [VMware Fusion](https://www.vmware.com/go/getfusion)) and configure the `vmrun` command. Verify the successful installation by running the following:
 ```bash
 vmrun -T ws list
 ```
 If the installation along with the environment variable set is successful, you will see the message showing the current running virtual machines.
 
-3. Run our setup script to download the necessary virtual machines and set up the environment☕:
-```bash
-python setup_vm.py
-```
+All set! Our setup script will automatically download the necessary virtual machines and configure the environment for you.
 
 ### On AWS or Azure (Virtualized platform)
 We are working on supporting it 👷. Please hold tight!
 
 ## 🚀 Quick Start
 Run the following minimal example to interact with the environment:
 ```python
@@ -145,18 +162,15 @@
                 "include": ["spotify"],
                 "exclude": ["not found"]
             }
         }
     }
 }
 
-env = DesktopEnv(
-    path_to_vm=r"Ubuntu/DesktopEnv-Ubuntu 64-bit Arm.vmx",
-    action_space="pyautogui"
-)
+env = DesktopEnv(action_space="pyautogui")
 
 obs = env.reset(task_config=example)
 obs, reward, done, info = env.step("pyautogui.rightClick()")
 ```
 You will see all the logs of the system running normally, including the successful creation of the environment, completion of setup, and successful execution of actions. In the end, you will observe a successful right-click on the screen, which means you are ready to go.
 
 ## 🧪 Experiments
```

#### html2text {}

```diff
@@ -1,34 +1,38 @@
-Metadata-Version: 2.1 Name: desktop_env Version: 0.1.5 Summary: The package
+Metadata-Version: 2.1 Name: desktop_env Version: 0.1.6 Summary: The package
 provides a desktop environment for setting and evaluating desktop automation
 tasks. Home-page: https://github.com/xlang-ai/desktop_env Author: Tianbao Xie,
-Danyang Zhang, Toh Jing Hua, etc. Author-email: tianbaoxiexxx@gmail.com
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: numpy~=1.24.3 Requires-Dist:
-Pillow~=10.1.0 Requires-Dist: fabric Requires-Dist: gymnasium~=0.28.1 Requires-
-Dist: requests~=2.31.0 Requires-Dist: transformers~=4.35.2 Requires-Dist:
-torch~=2.1.1 Requires-Dist: accelerate Requires-Dist: opencv-python~=4.8.1.78
-Requires-Dist: matplotlib~=3.7.4 Requires-Dist: pynput~=1.7.6 Requires-Dist:
-pyautogui~=0.9.54 Requires-Dist: psutil~=5.9.6 Requires-Dist: tqdm~=4.65.0
-Requires-Dist: pandas~=2.0.3 Requires-Dist: flask~=3.0.0 Requires-Dist:
-requests-toolbelt~=1.0.0 Requires-Dist: lxml Requires-Dist: cssselect Requires-
-Dist: xmltodict Requires-Dist: openpyxl Requires-Dist: python-docx Requires-
-Dist: python-pptx Requires-Dist: pypdf Requires-Dist: PyGetWindow Requires-
-Dist: rapidfuzz Requires-Dist: pyacoustid Requires-Dist: opencv-python
-Requires-Dist: ImageHash Requires-Dist: scikit-image Requires-Dist: librosa
-Requires-Dist: pymupdf Requires-Dist: chardet Requires-Dist: playwright
-Requires-Dist: formulas Requires-Dist: pydrive Requires-Dist: fastdtw Requires-
-Dist: odfpy Requires-Dist: func-timeout Requires-Dist: beautifulsoup4 Requires-
-Dist: PyYaml Requires-Dist: mutagen Requires-Dist: easyocr Requires-Dist: borb
-Requires-Dist: pypdf2 Requires-Dist: pdfplumber Requires-Dist:
-wrapt_timeout_decorator
+Danyang Zhang, Jixuan Chen, Xiaochuan Li, Siheng Zhao, Ruisheng Cao, Toh Jing
+Hua, etc. Author-email: tianbaoxiexxx@gmail.com Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.9
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+numpy~=1.24.3 Requires-Dist: Pillow~=10.1.0 Requires-Dist: fabric Requires-
+Dist: gymnasium~=0.28.1 Requires-Dist: requests~=2.31.0 Requires-Dist:
+transformers~=4.35.2 Requires-Dist: torch~=2.1.1 Requires-Dist: accelerate
+Requires-Dist: opencv-python~=4.8.1.78 Requires-Dist: matplotlib~=3.7.4
+Requires-Dist: pynput~=1.7.6 Requires-Dist: pyautogui~=0.9.54 Requires-Dist:
+psutil~=5.9.6 Requires-Dist: tqdm~=4.65.0 Requires-Dist: pandas~=2.0.3
+Requires-Dist: flask~=3.0.0 Requires-Dist: requests-toolbelt~=1.0.0 Requires-
+Dist: lxml Requires-Dist: cssselect Requires-Dist: xmltodict Requires-Dist:
+openpyxl Requires-Dist: python-docx Requires-Dist: python-pptx Requires-Dist:
+pypdf Requires-Dist: PyGetWindow Requires-Dist: rapidfuzz Requires-Dist:
+pyacoustid Requires-Dist: opencv-python Requires-Dist: ImageHash Requires-Dist:
+scikit-image Requires-Dist: librosa Requires-Dist: pymupdf Requires-Dist:
+chardet Requires-Dist: playwright Requires-Dist: formulas Requires-Dist:
+pydrive Requires-Dist: fastdtw Requires-Dist: odfpy Requires-Dist: func-timeout
+Requires-Dist: beautifulsoup4 Requires-Dist: PyYaml Requires-Dist: mutagen
+Requires-Dist: easyocr Requires-Dist: borb Requires-Dist: pypdf2 Requires-Dist:
+pdfplumber Requires-Dist: wrapt_timeout_decorator
                                    [Banner]
             _W_e_b_s_i_t_e â¢ _P_a_p_e_r â¢ _D_a_t_a â¢ _D_a_t_a_ _V_i_e_w_e_r â¢ _D_i_s_c_o_r_d
+ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_P_R_s_-_W_e_l_c_o_m_e_-_r_e_d_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
+_l_a_s_t_-_c_o_m_m_i_t_/_x_l_a_n_g_-_a_i_/_O_S_W_o_r_l_d_?_c_o_l_o_r_=_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-
+   _A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_d_e_s_k_t_o_p_-_e_n_v_._s_v_g_]_[_h_t_t_p_s_:_/_/
+                      _s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_d_e_s_k_t_o_p_-_e_n_v_]
 ## ð¢ Updates - 2024-04-11: We released our [paper](https://arxiv.org/abs/
 2404.07972), [environment and benchmark](https://github.com/xlang-ai/OSWorld),
 and [project page](https://os-world.github.io/). Check it out! ## ð¾
 Installation ### On Your Desktop or Server (Non-Virtualized Platform) Suppose
 you are operating on a system that has not been virtualized, meaning you are
 not utilizing a virtualized environment like AWS, Azure, or k8s. If this is the
 case, proceed with the instructions below. However, if you are on a virtualized
@@ -46,35 +50,34 @@
 any benchmark tasks: ```bash pip install desktop-env ``` 2. Install [VMware
 Workstation Pro](https://www.vmware.com/products/workstation-pro/workstation-
 pro-evaluation.html) (for systems with Apple Chips, you should install [VMware
 Fusion](https://www.vmware.com/go/getfusion)) and configure the `vmrun`
 command. Verify the successful installation by running the following: ```bash
 vmrun -T ws list ``` If the installation along with the environment variable
 set is successful, you will see the message showing the current running virtual
-machines. 3. Run our setup script to download the necessary virtual machines
-and set up the environmentâ: ```bash python setup_vm.py ``` ### On AWS or
-Azure (Virtualized platform) We are working on supporting it ð·. Please hold
-tight! ## ð Quick Start Run the following minimal example to interact with
-the environment: ```python from desktop_env.envs.desktop_env import DesktopEnv
+machines. All set! Our setup script will automatically download the necessary
+virtual machines and configure the environment for you. ### On AWS or Azure
+(Virtualized platform) We are working on supporting it ð·. Please hold tight!
+## ð Quick Start Run the following minimal example to interact with the
+environment: ```python from desktop_env.envs.desktop_env import DesktopEnv
 example = { "id": "94d95f96-9699-4208-98ba-3c3119edf9c2", "instruction": "I
 want to install Spotify on my current system. Could you please help me?",
 "config": [ { "type": "execute", "parameters": { "command": [ "python", "-c",
 "import pyautogui; import time; pyautogui.click(960, 540); time.sleep(0.5);" ]
 } } ], "evaluator": { "func": "check_include_exclude", "result": { "type":
 "vm_command_line", "command": "which spotify" }, "expected": { "type": "rule",
 "rules": { "include": ["spotify"], "exclude": ["not found"] } } } } env =
-DesktopEnv( path_to_vm=r"Ubuntu/DesktopEnv-Ubuntu 64-bit Arm.vmx",
-action_space="pyautogui" ) obs = env.reset(task_config=example) obs, reward,
-done, info = env.step("pyautogui.rightClick()") ``` You will see all the logs
-of the system running normally, including the successful creation of the
-environment, completion of setup, and successful execution of actions. In the
-end, you will observe a successful right-click on the screen, which means you
-are ready to go. ## ð§ª Experiments ### Agent Baselines If you wish to run the
-baseline agent used in our paper, you can execute the following command as an
-example under the GPT-4V pure-screenshot setting: ```bash python run.py --
+DesktopEnv(action_space="pyautogui") obs = env.reset(task_config=example) obs,
+reward, done, info = env.step("pyautogui.rightClick()") ``` You will see all
+the logs of the system running normally, including the successful creation of
+the environment, completion of setup, and successful execution of actions. In
+the end, you will observe a successful right-click on the screen, which means
+you are ready to go. ## ð§ª Experiments ### Agent Baselines If you wish to run
+the baseline agent used in our paper, you can execute the following command as
+an example under the GPT-4V pure-screenshot setting: ```bash python run.py --
 path_to_vm Ubuntu/Ubuntu.vmx --headless --observation_type screenshot --model
 gpt-4-vision-preview --result_dir ./results ``` The results, which include
 screenshots, actions, and video recordings of the agent's task completion, will
 be saved in the `./results` directory in this case. You can then run the
 following command to obtain the result: ```bash python show_result.py ``` ###
 Evaluation Please start by reading through the [agent interface](https://
 github.com/xlang-ai/OSWorld/blob/main/mm_agents/README.md) and the [environment
```

### Comparing `desktop_env-0.1.5/desktop_env.egg-info/SOURCES.txt` & `desktop_env-0.1.6/desktop_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/desktop_env.egg-info/requires.txt` & `desktop_env-0.1.6/desktop_env.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.5/setup.py` & `desktop_env-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
         except subprocess.CalledProcessError as e:
             print("Failed to run 'playwright install'. Please run 'playwright install' manually.")
             print(e)
 
 
 setup(
     name="desktop_env",
-    version="0.1.5",
-    author="Tianbao Xie, Danyang Zhang, Toh Jing Hua, etc.",
+    version="0.1.6",
+    author="Tianbao Xie, Danyang Zhang,  Jixuan Chen, Xiaochuan Li, Siheng Zhao, Ruisheng Cao, Toh Jing Hua, etc.",
     author_email="tianbaoxiexxx@gmail.com",
     description="The package provides a desktop environment for setting and evaluating desktop automation tasks.",
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/xlang-ai/desktop_env",
     packages=find_packages(),
     classifiers=[
@@ -85,8 +85,8 @@
         "pypdf2",
         "pdfplumber",
         "wrapt_timeout_decorator"
     ],
     cmdclass={
         'install': InstallPlaywrightCommand,  # Use the custom install command
     },
-)
+)
```


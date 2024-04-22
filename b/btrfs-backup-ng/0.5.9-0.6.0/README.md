# Comparing `tmp/btrfs-backup-ng-0.5.9.tar.gz` & `tmp/btrfs_backup_ng-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrfs-backup-ng-0.5.9.tar", last modified: Sun Feb 18 19:09:37 2024, max compression
+gzip compressed data, was "btrfs_backup_ng-0.6.0.tar", last modified: Mon Apr 22 00:59:20 2024, max compression
```

## Comparing `btrfs-backup-ng-0.5.9.tar` & `btrfs_backup_ng-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-18 19:09:37.406484 btrfs-backup-ng-0.5.9/
--rw-r--r--   0 berrym    (1000) berrym    (1000)     1227 2024-01-25 04:44:42.000000 btrfs-backup-ng-0.5.9/LICENSE
--rw-r--r--   0 berrym    (1000) berrym    (1000)    15576 2024-02-18 19:09:37.406484 btrfs-backup-ng-0.5.9/PKG-INFO
--rw-r--r--   0 berrym    (1000) berrym    (1000)    15081 2024-02-18 19:09:22.000000 btrfs-backup-ng-0.5.9/README.md
--rw-r--r--   0 berrym    (1000) berrym    (1000)      704 2024-02-18 19:09:22.000000 btrfs-backup-ng-0.5.9/pyproject.toml
--rw-r--r--   0 berrym    (1000) berrym    (1000)       38 2024-02-18 19:09:37.406484 btrfs-backup-ng-0.5.9/setup.cfg
--rw-r--r--   0 berrym    (1000) berrym    (1000)       38 2024-01-25 04:44:42.000000 btrfs-backup-ng-0.5.9/setup.py
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-18 19:09:37.404484 btrfs-backup-ng-0.5.9/src/
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-18 19:09:37.404484 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/
--rw-r--r--   0 berrym    (1000) berrym    (1000)       74 2024-02-18 19:09:22.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/__init__.py
--rw-r--r--   0 berrym    (1000) berrym    (1000)    25836 2024-02-18 19:09:22.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/__main__.py
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-18 19:09:37.406484 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/
--rw-r--r--   0 berrym    (1000) berrym    (1000)     2414 2024-01-25 04:44:42.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/__init__.py
--rw-r--r--   0 berrym    (1000) berrym    (1000)    13830 2024-02-16 17:47:20.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/common.py
--rw-r--r--   0 berrym    (1000) berrym    (1000)     1695 2024-02-16 17:47:20.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/local.py
--rw-r--r--   0 berrym    (1000) berrym    (1000)      599 2024-01-25 04:44:42.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/shell.py
--rw-r--r--   0 berrym    (1000) berrym    (1000)     5780 2024-02-16 17:47:20.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/ssh.py
--rw-r--r--   0 berrym    (1000) berrym    (1000)     9709 2024-02-16 17:47:20.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/util.py
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-18 19:09:37.406484 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/
--rw-r--r--   0 berrym    (1000) berrym    (1000)    15576 2024-02-18 19:09:37.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/PKG-INFO
--rw-r--r--   0 berrym    (1000) berrym    (1000)      585 2024-02-18 19:09:37.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/SOURCES.txt
--rw-r--r--   0 berrym    (1000) berrym    (1000)        1 2024-02-18 19:09:37.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/dependency_links.txt
--rw-r--r--   0 berrym    (1000) berrym    (1000)       66 2024-02-18 19:09:37.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/entry_points.txt
--rw-r--r--   0 berrym    (1000) berrym    (1000)        5 2024-02-18 19:09:37.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/requires.txt
--rw-r--r--   0 berrym    (1000) berrym    (1000)       16 2024-02-18 19:09:37.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/top_level.txt
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-04-22 00:59:20.410830 btrfs_backup_ng-0.6.0/
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     1227 2024-02-29 00:21:05.000000 btrfs_backup_ng-0.6.0/LICENSE
+-rw-r--r--   0 berrym    (1000) berrym    (1000)    15582 2024-04-22 00:59:20.410830 btrfs_backup_ng-0.6.0/PKG-INFO
+-rw-r--r--   0 berrym    (1000) berrym    (1000)    15087 2024-04-22 00:56:40.000000 btrfs_backup_ng-0.6.0/README.md
+-rw-r--r--   0 berrym    (1000) berrym    (1000)      704 2024-04-22 00:55:20.000000 btrfs_backup_ng-0.6.0/pyproject.toml
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       38 2024-04-22 00:59:20.410830 btrfs_backup_ng-0.6.0/setup.cfg
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       38 2024-02-29 00:21:05.000000 btrfs_backup_ng-0.6.0/setup.py
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-04-22 00:59:20.407830 btrfs_backup_ng-0.6.0/src/
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-04-22 00:59:20.408830 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       74 2024-04-22 00:32:58.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/__init__.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)    25980 2024-04-22 00:43:25.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/__main__.py
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-04-22 00:59:20.409830 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/endpoint/
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     2417 2024-04-22 00:32:42.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/endpoint/__init__.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)    13788 2024-04-22 00:51:32.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/endpoint/common.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     1661 2024-04-22 00:51:32.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/endpoint/local.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)      611 2024-04-22 00:31:52.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/endpoint/shell.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     5714 2024-04-22 00:51:32.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/endpoint/ssh.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     1205 2024-04-22 00:47:26.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/rich_logger.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     9583 2024-04-22 00:51:27.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/util.py
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-04-22 00:59:20.409830 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng.egg-info/
+-rw-r--r--   0 berrym    (1000) berrym    (1000)    15582 2024-04-22 00:59:20.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng.egg-info/PKG-INFO
+-rw-r--r--   0 berrym    (1000) berrym    (1000)      620 2024-04-22 00:59:20.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 berrym    (1000) berrym    (1000)        1 2024-04-22 00:59:20.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       66 2024-04-22 00:59:20.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng.egg-info/entry_points.txt
+-rw-r--r--   0 berrym    (1000) berrym    (1000)        5 2024-04-22 00:59:20.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng.egg-info/requires.txt
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       16 2024-04-22 00:59:20.000000 btrfs_backup_ng-0.6.0/src/btrfs_backup_ng.egg-info/top_level.txt
```

### Comparing `btrfs-backup-ng-0.5.9/LICENSE` & `btrfs_backup_ng-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `btrfs-backup-ng-0.5.9/PKG-INFO` & `btrfs_backup_ng-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrfs-backup-ng
-Version: 0.5.9
+Version: 0.6.0
 Summary: Intelligent, feature-rich backups for btrfs
 Author-email: Michael Berry <trismegustis@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/berrym/btrfs-backup-ng
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -40,15 +40,15 @@
 written by Chris Lawrence. Since then, most of the code has been
 refactored and many new features were added before this repository has
 been transferred to Robert Schindler. Many thanks to Chris for his work. The old code
 base has been tagged with `legacy`. If, for any reason, you want to
 continue using it and miss the new features, you can check that out.
 
 Latest release  
-v0.5.9
+v0.6.0
 
 Downloads  
 <http://pypi.python.org/pypi/btrfs_backup_ng>
 
 Source  
 <https://github.com/berrym/btrfs-backup-ng>
 
@@ -96,21 +96,21 @@
 via PIP. If `pip3` is missing on your system, and you run a Debian-based
 distribution, simply install it via:
 
     $ sudo apt-get install python3-pip python3-wheel
 
 Then, you can fetch the latest version of btrfs-backup-ng:
 
-    $ sudo pip3 install btrfs-backup-ng
+    $ pip3 install btrfs-backup-ng
 
 ### Pre-built packages
 
 There are currently pre-built packages available for Fedora and OpenSUSE Tumbleweed:
 
-Fedora 38, Fedora 39, Fedora Rawhide
+Fedora 38, Fedora 39, Fedora 40, Fedora Rawhide
 
     $ dnf copr enable mberry/btrfs-backup-ng
     $ dnf install btrfs-backup-ng --refresh
 
 OpenSUSE Tumbleweed
 
     $ sudo zypper addrepo https://download.opensuse.org/repositories/home:berrym/openSUSE_Tumbleweed/home:berrym.repo
@@ -122,15 +122,15 @@
 Note: This package now uses a pyproject.toml based build as outlined in
 PEP 517 and PEP 621.
 
 Clone this git repository
 
     $ git clone https://github.com/berrym/btrfs-backup-ng.git
     $ cd btrfs-backup-ng
-    $ git checkout tags/v0.5.9  # optionally checkout a specific version
+    $ git checkout tags/v0.6.0  # optionally checkout a specific version
     $ python3 -m venv /path/to/btrfs-backup-ng/venv # optionally use venv
     $ sh /path/to/btrfs-backup-ng/venv/bin/activate # using venv
     $ python3 -m build
     # using venv
     $ python3 -m pip install .
     # or 
     $ sudo python3 -m pip install .
```

### Comparing `btrfs-backup-ng-0.5.9/README.md` & `btrfs_backup_ng-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 written by Chris Lawrence. Since then, most of the code has been
 refactored and many new features were added before this repository has
 been transferred to Robert Schindler. Many thanks to Chris for his work. The old code
 base has been tagged with `legacy`. If, for any reason, you want to
 continue using it and miss the new features, you can check that out.
 
 Latest release  
-v0.5.9
+v0.6.0
 
 Downloads  
 <http://pypi.python.org/pypi/btrfs_backup_ng>
 
 Source  
 <https://github.com/berrym/btrfs-backup-ng>
 
@@ -81,21 +81,21 @@
 via PIP. If `pip3` is missing on your system, and you run a Debian-based
 distribution, simply install it via:
 
     $ sudo apt-get install python3-pip python3-wheel
 
 Then, you can fetch the latest version of btrfs-backup-ng:
 
-    $ sudo pip3 install btrfs-backup-ng
+    $ pip3 install btrfs-backup-ng
 
 ### Pre-built packages
 
 There are currently pre-built packages available for Fedora and OpenSUSE Tumbleweed:
 
-Fedora 38, Fedora 39, Fedora Rawhide
+Fedora 38, Fedora 39, Fedora 40, Fedora Rawhide
 
     $ dnf copr enable mberry/btrfs-backup-ng
     $ dnf install btrfs-backup-ng --refresh
 
 OpenSUSE Tumbleweed
 
     $ sudo zypper addrepo https://download.opensuse.org/repositories/home:berrym/openSUSE_Tumbleweed/home:berrym.repo
@@ -107,15 +107,15 @@
 Note: This package now uses a pyproject.toml based build as outlined in
 PEP 517 and PEP 621.
 
 Clone this git repository
 
     $ git clone https://github.com/berrym/btrfs-backup-ng.git
     $ cd btrfs-backup-ng
-    $ git checkout tags/v0.5.9  # optionally checkout a specific version
+    $ git checkout tags/v0.6.0  # optionally checkout a specific version
     $ python3 -m venv /path/to/btrfs-backup-ng/venv # optionally use venv
     $ sh /path/to/btrfs-backup-ng/venv/bin/activate # using venv
     $ python3 -m build
     # using venv
     $ python3 -m pip install .
     # or 
     $ sudo python3 -m pip install .
```

### Comparing `btrfs-backup-ng-0.5.9/pyproject.toml` & `btrfs_backup_ng-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "btrfs-backup-ng"
-version = "0.5.9"
+version = "0.6.0"
 description = "Intelligent, feature-rich backups for btrfs"
 authors = [{ name = "Michael Berry", email = "trismegustis@gmail.com" }]
 license = { text = "MIT" }
 dependencies = ["rich"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/__main__.py` & `btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,61 +25,59 @@
 BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import concurrent.futures
-import logging
-
 import os
 import sys
 import time
+
 from math import inf
 
-from rich.console import Console, Group
+from rich.align import Align
+from rich.layout import Layout
 from rich.live import Live
-from rich.logging import RichHandler
 from rich.panel import Panel
 from rich.progress import BarColumn, Progress, SpinnerColumn, TimeElapsedColumn
+from rich.text import Text
 
 from . import endpoint
+from .rich_logger import RichLogger, logger
 from . import util
 
 
-console = Console()
-
-
 def send_snapshot(snapshot, destination_endpoint, parent=None, clones=None):
     """
     Sends snapshot to destination endpoint, using given parent and clones.
     It connects the pipes of source and destination together.
     """
 
     # Now we need to send the snapshot (incrementally, if possible)
-    logging.info("Sending %s ...", snapshot)
+    logger.info("Sending %s ...", snapshot)
     if parent:
-        logging.info("  Using parent: %s", parent)
+        logger.info("  Using parent: %s", parent)
     else:
-        logging.info("  No parent snapshot available, sending in full mode.")
+        logger.info("  No parent snapshot available, sending in full mode.")
     if clones:
-        logging.info("  Using clones: %r", clones)
+        logger.info("  Using clones: %r", clones)
 
     pipes = [snapshot.endpoint.send(snapshot, parent=parent, clones=clones)]
 
     pipes.append(destination_endpoint.receive(pipes[-1].stdout))
 
     pids = [pipe.pid for pipe in pipes]
     while pids:
         pid, return_code = os.wait()
         if pid in pids:
-            logging.debug("  -> PID %d exited with return code %d", pid, return_code)
+            logger.debug("  -> PID %d exited with return code %d", pid, return_code)
             pids.remove(pid)
         if return_code != 0:
-            logging.error("Error during btrfs send / receive")
+            logger.error("Error during btrfs send / receive")
             raise util.SnapshotTransferError()
 
 
 def sync_snapshots(
     source_endpoint,
     destination_endpoint,
     keep_num_backups=0,
@@ -91,30 +89,30 @@
     about locking and deletion of corrupt snapshots from failed transfers.
     It never transfers snapshots that would anyway be deleted afterward
     due to retention policy.
     """
 
     # global snapshot
     snapshot = None
-    logging.info(util.log_heading(f"  To {destination_endpoint} ..."))
+    logger.info(util.log_heading(f"  To {destination_endpoint} ..."))
 
     source_snapshots = source_endpoint.list_snapshots()
     destination_snapshots = destination_endpoint.list_snapshots()
     destination_id = destination_endpoint.get_id()
 
     # delete corrupt snapshots from destination
     to_remove = []
     for snapshot in source_snapshots:
         if snapshot in destination_snapshots and destination_id in snapshot.locks:
             # seems to have failed previously and is present at
             # destination; delete corrupt snapshot there
             destination_snapshot = destination_snapshots[
                 destination_snapshots.index(snapshot)
             ]
-            logging.info(
+            logger.info(
                 "Potentially corrupt snapshot %s found at %s",
                 destination_snapshot,
                 destination_endpoint,
             )
             to_remove.append(destination_snapshot)
     if to_remove:
         destination_endpoint.delete_snapshots(to_remove)
@@ -124,31 +122,31 @@
     # now that deletion worked, remove all locks for this destination
     for snapshot in source_snapshots:
         if destination_id in snapshot.locks:
             source_endpoint.set_lock(snapshot, destination_id, False)
         if destination_id in snapshot.parent_locks:
             source_endpoint.set_lock(snapshot, destination_id, False, parent=True)
 
-    logging.debug("Planning transmissions ...")
+    logger.debug("Planning transmissions ...")
     to_consider = source_snapshots
     if keep_num_backups > 0:
         # it wouldn't make sense to transfer snapshots that would be deleted
         # afterward anyway
         to_consider = to_consider[-keep_num_backups:]
     to_transfer = [
         snapshot for snapshot in to_consider if snapshot not in destination_snapshots
     ]
 
     if not to_transfer:
-        logging.info("No snapshots need to be transferred.")
+        logger.info("No snapshots need to be transferred.")
         return
 
-    logging.info("Going to transfer %d snapshot(s):", len(to_transfer))
+    logger.info("Going to transfer %d snapshot(s):", len(to_transfer))
     for _ in to_transfer:
-        logging.info("  %s", snapshot)
+        logger.info("  %s", snapshot)
 
     while to_transfer:
         if no_incremental:
             # simply choose the last one
             best_snapshot = to_transfer[-1]
             parent = None
             clones = []
@@ -184,27 +182,27 @@
                 best_snapshot,
                 destination_endpoint,
                 parent=parent,
                 clones=clones,
                 **kwargs,
             )
         except util.SnapshotTransferError:
-            logging.info(
+            logger.info(
                 "Keeping %s locked to prevent it from getting removed.",
                 best_snapshot,
             )
         else:
             source_endpoint.set_lock(best_snapshot, destination_id, False)
             if parent:
                 source_endpoint.set_lock(parent, destination_id, False, parent=True)
             destination_endpoint.add_snapshot(best_snapshot)
             destination_snapshots = destination_endpoint.list_snapshots()
         to_transfer.remove(best_snapshot)
 
-    logging.info(util.log_heading(f"Transfers to {destination_endpoint} complete!"))
+    logger.info(util.log_heading(f"Transfers to {destination_endpoint} complete!"))
 
 
 def parse_options(argv):
     """Run the program. Items in ``argv`` are treated as command line
     arguments."""
 
     description = """\
@@ -424,177 +422,172 @@
 
     return options
 
 
 def run_task(options):
     """Create a list of tasks to run."""
 
-    logging.basicConfig(
-        format="%(message)s",
-        datefmt="%H:%M:%S",
-        level=options["verbosity"].upper(),
-        handlers=[RichHandler(console=console)],
-    )
+    logger.setLevel(options["verbosity"].upper())
 
     # applying shortcuts
     if "quiet" in options:
         options["verbosity"] = "warning"
     if "latest_only" in options:
         options["num_snapshots"] = 1
 
-    logging.info(util.log_heading(f"Started at {time.ctime()}"))
+    logger.info(util.log_heading(f"Started at {time.ctime()}"))
 
-    logging.debug(util.log_heading("Settings"))
+    logger.debug(util.log_heading("Settings"))
     if "snapshot_folder" in options:
         snapshot_directory = options["snapshot_folder"]
     else:
-        snapshot_directory = ".snapshots"
+        snapshot_directory = ".btrfs-backup-ng/snapshots"
 
     if "snapshot_prefix" in options:
         snapshot_prefix = options["snapshot_prefix"]
     else:
-        snapshot_prefix = ""
+        snapshot_prefix = f"{os.uname()[1]}-"
 
-    logging.debug("Enable btrfs debugging: %r", options["btrfs_debug"])
-    logging.debug("Don't take a new snapshot: %r", options["no_snapshot"])
-    logging.debug("Number of snapshots to keep: %d", options["num_snapshots"])
-    logging.debug(
+    logger.debug("Enable btrfs debugging: %r", options["btrfs_debug"])
+    logger.debug("Don't take a new snapshot: %r", options["no_snapshot"])
+    logger.debug("Number of snapshots to keep: %d", options["num_snapshots"])
+    logger.debug(
         "Number of backups to keep: %s",
         (str(options["num_backups"]) if options["num_backups"] > 0 else "Any"),
     )
-    logging.debug("Snapshot folder: %s", snapshot_directory)
-    logging.debug("Snapshot prefix: %s", snapshot_prefix if snapshot_prefix else None)
-    logging.debug("Don't transfer snapshots: %r", options["no_transfer"])
-    logging.debug("Don't send incrementally: %r", options["no_incremental"])
-    logging.debug("Extra SSH config options: %s", options["ssh_opt"])
-    logging.debug("Use sudo at SSH remote host: %r", options["ssh_sudo"])
-    logging.debug("Run 'btrfs subvolume sync' afterwards: %r", options["sync"])
-    logging.debug(
+    logger.debug("Snapshot folder: %s", snapshot_directory)
+    logger.debug("Snapshot prefix: %s", snapshot_prefix if snapshot_prefix else None)
+    logger.debug("Don't transfer snapshots: %r", options["no_transfer"])
+    logger.debug("Don't send incrementally: %r", options["no_incremental"])
+    logger.debug("Extra SSH config options: %s", options["ssh_opt"])
+    logger.debug("Use sudo at SSH remote host: %r", options["ssh_sudo"])
+    logger.debug("Run 'btrfs subvolume sync' afterwards: %r", options["sync"])
+    logger.debug(
         "Convert subvolumes to read-write before deletion: %r",
         options["convert_rw"],
     )
-    logging.debug("Remove locks for given destinations: %r", options["remove_locks"])
-    logging.debug("Skip filesystem checks: %r", options["skip_fs_checks"])
-    logging.debug("Auto add locked destinations: %r", options["locked_destinations"])
+    logger.debug("Remove locks for given destinations: %r", options["remove_locks"])
+    logger.debug("Skip filesystem checks: %r", options["skip_fs_checks"])
+    logger.debug("Auto add locked destinations: %r", options["locked_destinations"])
 
     # kwargs that are common between all endpoints
     endpoint_kwargs = {
         "snap_prefix": snapshot_prefix,
         "convert_rw": options["convert_rw"],
         "subvolume_sync": options["sync"],
         "btrfs_debug": options["btrfs_debug"],
         "fs_checks": not options["skip_fs_checks"],
         "ssh_opts": options["ssh_opt"],
         "ssh_sudo": options["ssh_sudo"],
     }
 
-    logging.debug("Source: %s", options["source"])
+    logger.debug("Source: %s", options["source"])
     source_endpoint_kwargs = dict(endpoint_kwargs)
     source_endpoint_kwargs["path"] = snapshot_directory
     try:
         source_endpoint = endpoint.choose_endpoint(
             options["source"], source_endpoint_kwargs, source=True
         )
     except ValueError as e:
-        logging.error("Couldn't parse source specification: %s", e)
+        logger.error("Couldn't parse source specification: %s", e)
         raise util.AbortError()
-    logging.debug("Source endpoint: %s", source_endpoint)
+    logger.debug("Source endpoint: %s", source_endpoint)
     source_endpoint.prepare()
 
     # add endpoint creation strings for locked destinations, if desired
     if options["locked_destinations"]:
         for snap in source_endpoint.list_snapshots():
             for lock in snap.locks:
                 if lock not in options["destinations"]:
                     options["destinations"].append(lock)
 
     if "remove_locks" in options.keys():
-        logging.info("Removing locks (--remove-locks) ...")
+        logger.info("Removing locks (--remove-locks) ...")
         for snap in source_endpoint.list_snapshots():
             for destination in options["destinations"]:
                 if destination in snap.locks:
-                    logging.info("  %s (%s)", snap, destination)
+                    logger.info("  %s (%s)", snap, destination)
                     source_endpoint.set_lock(snap, destination, False)
                 if destination in snap.parent_locks:
-                    logging.info("  %s (%s) [parent]", snap, destination)
+                    logger.info("  %s (%s) [parent]", snap, destination)
                     source_endpoint.set_lock(snap, destination, False, parent=True)
 
     destination_endpoints = []
     # only create destination endpoints if they are needed
     if options["no_transfer"] and options["num_backups"] <= 0:
-        logging.debug(
+        logger.debug(
             "Don't create destination endpoints because they won't be needed "
             "(--no-transfer and no --num-backups)."
         )
     else:
         for destination in options["destinations"]:
-            logging.debug("Destination: %s", destination)
+            logger.debug("Destination: %s", destination)
             try:
                 destination_endpoint = endpoint.choose_endpoint(
                     destination, endpoint_kwargs, source=False
                 )
             except ValueError as e:
-                logging.error("Couldn't parse destination specification: %s", e)
+                logger.error("Couldn't parse destination specification: %s", e)
                 raise util.AbortError()
             destination_endpoints.append(destination_endpoint)
-            logging.debug("Destination endpoint: %s", destination_endpoint)
+            logger.debug("Destination endpoint: %s", destination_endpoint)
             destination_endpoint.prepare()
 
     if options["no_snapshot"]:
-        logging.info("Taking no snapshot (--no-snapshot).")
+        logger.info("Taking no snapshot (--no-snapshot).")
     else:
         # First we need to create a new snapshot on the source disk
-        logging.info(util.log_heading("Snapshotting ..."))
+        logger.info(util.log_heading("Snapshotting ..."))
         source_endpoint.snapshot()
 
     if options["no_transfer"]:
-        logging.info(util.log_heading("Not transferring (--no-transfer)."))
+        logger.info(util.log_heading("Not transferring (--no-transfer)."))
     else:
-        logging.info(util.log_heading("Transferring ..."))
+        logger.info(util.log_heading("Transferring ..."))
         for destination_endpoint in destination_endpoints:
             try:
                 sync_snapshots(
                     source_endpoint,
                     destination_endpoint,
                     keep_num_backups=options["num_backups"],
                     no_incremental=options["no_incremental"],
                 )
             except util.AbortError as e:
-                logging.error(
+                logger.error(
                     "Aborting snapshot transfer to %s due to exception.",
                     destination_endpoint,
                 )
-                logging.debug("Exception was: %s", e)
+                logger.debug("Exception was: %s", e)
         if not destination_endpoints:
-            logging.info("No destination configured, don't sending anything.")
+            logger.info("No destination configured, don't sending anything.")
 
-    logging.info(util.log_heading("Cleaning up..."))
+    logger.info(util.log_heading("Cleaning up..."))
     # cleanup snapshots > num_snapshots in snap_dir
     if options["num_snapshots"] > 0:
         try:
             source_endpoint.delete_old_snapshots(options["num_snapshots"])
         except util.AbortError as e:
-            logging.debug(
+            logger.debug(
                 "Got AbortError while deleting source snapshots at %s\n" "Caught: %s",
                 source_endpoint,
                 e,
             )
     # cleanup backups > num_backups in backup target
     if options["num_backups"] > 0:
         for destination_endpoint in destination_endpoints:
             try:
                 destination_endpoint.delete_old_snapshots(options["num_backups"])
             except util.AbortError as e:
-                logging.debug(
+                logger.debug(
                     "Got AbortError while deleting backups at %s\n" "Caught: %s",
                     destination_endpoint,
                     e,
                 )
 
-    logging.info(util.log_heading(f"Finished at {time.ctime()}"))
+    logger.info(util.log_heading(f"Finished at {time.ctime()}"))
 
     return "Success"
 
 
 def elevate_privileges():
     """Re-run the program using sudo if privileges are needed."""
     if os.getuid() != 0:
@@ -624,75 +617,90 @@
 
     overall_progress = Progress(
         "[progress.description]{task.description}",
         BarColumn(),
         "[progress.percentage]{task.percentage:>3.0f}%",
         SpinnerColumn(),
         TimeElapsedColumn(),
-        refresh_per_second=4,
     )
 
     tasks_progress = Progress(
         "{task.description}",
         BarColumn(),
         SpinnerColumn(),
         TimeElapsedColumn(),
-        refresh_per_second=4,
     )
 
-    progress_group = Group(Panel(tasks_progress), Panel(overall_progress))
+    layout = Layout(name="root")
+
+    layout.split(
+        Layout(name="header", size=5),
+        Layout(name="main"),
+        Layout(name="footer", size=3),
+    )
+
+    layout["main"].split_row(
+        Layout(name="tasks"), Layout(name="logs", ratio=2, minimum_size=80)
+    )
+
+    layout["header"].update(
+        Panel(
+            Align.center(
+                Text(
+                    """btrfs-backup-ng\n\nIncremental backups for the btrfs filesystem.""",
+                    justify="center",
+                ),
+                vertical="middle",
+            )
+        ),
+    )
+
+    total_tasks = len(tasks)
+    overall_task_id = overall_progress.add_task(
+        "[green]All jobs progress:",
+        total=total_tasks,
+    )
+
+    layout["tasks"].update(Panel(tasks_progress))
+
+    log = RichLogger()
+    layout["logs"].update(Panel(Text("\n".join(log.messages))))
+
+    layout["footer"].update(Panel(overall_progress))
+
+    futures = []  # keep track of the concurrent futures
+    futures_id_map = {}  # associate a task_id with futures
 
     try:
-        with Live(progress_group, console=console, refresh_per_second=4):
-            futures = []  # keep track of the concurrent futures
-            task_numbers = []
-            futures_id_map = {}
-
-            with concurrent.futures.ProcessPoolExecutor(max_workers=8) as executor:
-                for n, _ in enumerate(tasks):
-                    futures.append(executor.submit(run_task, task_options[n]))
-
-                    task_id = tasks_progress.add_task(
-                        f"[red]task {n}: [cyan]{task_options[n]['source']} -> {task_options[n]['destinations']}",
-                        total=None,
-                        visible=True,
-                    )
-                    task_numbers.append(task_id)
-                    futures_id_map[futures[n]] = task_id
-
-                # Total count of completed tasks
-                total_tasks = len(task_numbers)
-                # tasks_completed = 0
-
-                overall_task_id = overall_progress.add_task(
-                    "[green]All jobs progress:",
-                    total=total_tasks,
-                    visible=True,
+        with concurrent.futures.ThreadPoolExecutor(max_workers=8) as executor:
+            for n in range(len(tasks)):
+                futures.append(executor.submit(run_task, task_options[n]))
+                task_id = tasks_progress.add_task(
+                    f"[red]task: [cyan]{task_options[n]['source']}",
+                    total=None,
                 )
+                futures_id_map[futures[n]] = task_id
+                layout["logs"].update(Panel(Text("\n".join(log.messages))))
 
-                # monitor the progress
-                for future in concurrent.futures.as_completed(futures):
-                    result = future.result()
-                    task_id = futures_id_map[future]
-                    logging.info(
-                        "Task %d has completed, result: %s",
-                        task_id,
-                        result,
-                    )
-                    tasks_progress.update(
-                        task_id,
-                        description=f"[red]Task {task_id}: [bold yellow]Completed!",
-                        total=1,
-                        completed=1,
-                    )
-                    overall_progress.update(
-                        overall_task_id,
-                        advance=1,
-                    )
-
-            overall_progress.update(
-                overall_task_id,
-                description="[bold yellow]All tasks have finished!",
-                completed=total_tasks,
-            )
+            with Live(layout, refresh_per_second=10):
+                while not overall_progress.finished:
+                    layout["logs"].update(Panel(Text("\n".join(log.messages))))
+                    done, _ = concurrent.futures.wait(futures, timeout=1)
+                    for future in done:
+                        layout["logs"].update(Panel(Text("\n".join(log.messages))))
+                        task_id = futures_id_map[future]
+                        tasks_progress.update(
+                            task_id,
+                            total=1,
+                            completed=1,
+                        )
+                        overall_progress.update(
+                            overall_task_id,
+                            advance=1,
+                        )
+                        futures.remove(future)
+                overall_progress.update(
+                    overall_task_id,
+                    completed=total_tasks,
+                )
     except (util.AbortError, KeyboardInterrupt):
         sys.exit(1)
```

### Comparing `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/__init__.py` & `btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/endpoint/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""btrfs-backup-ng: btrfs-backup/endpoint/__init__.py"""
+"""btrfs-backup-ng: btrfs_backup_ng/endpoint/__init__.py"""
 
 import os
 import urllib.parse
 
 from .local import LocalEndpoint
 from .shell import ShellEndpoint
 from .ssh import SSHEndpoint
```

### Comparing `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/common.py` & `btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/endpoint/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-"""btrfs-backup-ng: btrfs-backup/endpoint/common.py
+"""btrfs-backup-ng: btrfs_backup_ng/endpoint/common.py
 Common functionality among modules.
 """
 
 import logging
 import os
 import subprocess
 
+from ..rich_logger import logger
 from .. import util
 
 
 def require_source(method):
     """Decorator that ensures source is set on the object the called method belongs to."""
 
     def wrapped(self, *args, **kwargs):
@@ -45,29 +46,27 @@
         self.source = source
         self.fs_checks = fs_checks
         self.lock_file_name = ".outstanding_transfers"
         self.__cached_snapshots = None
 
     def prepare(self):
         """Public access to _prepare, which is called after creating an endpoint.XS"""
-        logging.info("Preparing endpoint %r ...", self)
+        logger.info("Preparing endpoint %r ...", self)
         return self._prepare()
 
     @require_source
     def snapshot(self, readonly=True, sync=True):
         """Takes a snapshot and returns the created object."""
 
         snapshot = util.Snapshot(self.path, self.snap_prefix, self)
         snapshot_path = snapshot.get_path()
-        logging.info("%s -> %s", self.source, snapshot_path)
+        logger.info("%s -> %s", self.source, snapshot_path)
 
         commands = [
-            self._build_snapshot_cmd(
-                self.source, snapshot_path, readonly=readonly
-            )
+            self._build_snapshot_cmd(self.source, snapshot_path, readonly=readonly)
         ]
 
         # sync disks
         if sync:
             commands.append(self._build_sync_command())
 
         for cmd in self._collapse_commands(commands, abort_on_failure=True):
@@ -88,32 +87,30 @@
         """Calls 'btrfs receive', setting the given pipe as its stdin.
         The receiving process's Popen object is returned."""
 
         cmd = self._build_receive_command(self.path)
         # from WARNING level onwards, hide stdout
         loglevel = logging.getLogger().getEffectiveLevel()
         stdout = subprocess.DEVNULL if loglevel >= logging.WARNING else None
-        return self._exec_command(
-            cmd, method="Popen", stdin=stdin, stdout=stdout
-        )
+        return self._exec_command(cmd, method="Popen", stdin=stdin, stdout=stdout)
 
     def list_snapshots(self, flush_cache=False):
         """Returns a list with all snapshots found at ``self.path``.
         If ``flush_cache`` is not set, cached results will be used
         if available."""
 
         if self.__cached_snapshots is not None and not flush_cache:
-            logging.debug(
+            logger.debug(
                 "Returning %d cached snapshots for %r.",
                 len(self.__cached_snapshots),
                 self,
             )
             return list(self.__cached_snapshots)
 
-        logging.debug("Building snapshot cache of %r ...", self)
+        logger.debug("Building snapshot cache of %r ...", self)
         snapshots = []
         listdir = self._listdir(self.path)
         for item in listdir:
             if item.startswith(self.snap_prefix):
                 time_str = item[len(self.snap_prefix) :]
                 try:
                     time_obj = util.str_to_date(time_str)
@@ -135,15 +132,15 @@
                     getattr(snapshot, lock_type).update(locks)
 
         # sort by date, then time;
         snapshots.sort()
 
         # populate cache
         self.__cached_snapshots = snapshots
-        logging.debug(
+        logger.debug(
             "Populated snapshot cache of %r with %d items.",
             self,
             len(snapshots),
         )
 
         return list(snapshots)
 
@@ -167,15 +164,15 @@
             if _snapshot.locks:
                 snap_entry["locks"] = list(_snapshot.locks)
             if _snapshot.parent_locks:
                 snap_entry["parent_locks"] = list(_snapshot.parent_locks)
             if snap_entry:
                 lock_dict[_snapshot.get_name()] = snap_entry
         self._write_locks(lock_dict)
-        logging.debug(
+        logger.debug(
             "Lock state for %s and lock_id %s changed to %s (parent = %s)",
             snapshot,
             lock_id,
             lock_state,
             parent,
         )
 
@@ -205,20 +202,20 @@
 
         # only remove snapshots that have no lock remaining
         to_remove = []
         for snapshot in snapshots:
             if not snapshot.locks and not snapshot.parent_locks:
                 to_remove.append(snapshot)
 
-        logging.info("Removing %d snapshot(s) from %r:", len(to_remove), self)
+        logger.info("Removing %d snapshot(s) from %r:", len(to_remove), self)
         for snapshot in snapshots:
             if snapshot in to_remove:
-                logging.info("  %s", snapshot)
+                logger.info("  %s", snapshot)
             else:
-                logging.info("  %s - is locked, keeping it", snapshot)
+                logger.info("  %s - is locked, keeping it", snapshot)
 
         if to_remove:
             # finally delete them
             cmds = self._build_deletion_commands(to_remove, **kwargs)
             cmds = self._collapse_commands(cmds, abort_on_failure=True)
             for cmd in cmds:
                 self._exec_command(cmd)
@@ -291,17 +288,15 @@
         return cmd
 
     def _build_receive_command(self, destination):
         """Should return a command to receive a snapshot to ``dest``.
         The stream is piped into stdin when the command is running."""
         return ["btrfs", "receive"] + self.btrfs_flags + [destination]
 
-    def _build_deletion_commands(
-        self, snapshots, convert_rw=None, subvolume_sync=None
-    ):
+    def _build_deletion_commands(self, snapshots, convert_rw=None, subvolume_sync=None):
         """Should return a list of commands that, when executed in order,
         delete the given ``snapshots``. ``convert_rw`` and
         ``subvolume_sync`` should be regarded as well."""
 
         if convert_rw is None:
             convert_rw = self.convert_rw
         if subvolume_sync is None:
@@ -368,22 +363,22 @@
         path = self._get_lock_file_path()
         try:
             if not os.path.isfile(path):
                 return {}
             with open(path, "r", encoding="utf-8") as f:
                 return util.read_locks(f.read())
         except (OSError, ValueError) as e:
-            logging.error("Error on reading lock file %s: %s", path, e)
+            logger.error("Error on reading lock file %s: %s", path, e)
             raise util.AbortError()
 
     @require_source
     def _write_locks(self, lock_dict):
         """Should write the locks given as ``lock_dict`` like
         ``util.read_locks`` returns it."""
         path = self._get_lock_file_path()
         try:
-            logging.debug("Writing lock file: %s", path)
+            logger.debug("Writing lock file: %s", path)
             with open(path, "w", encoding="utf-8") as f:
                 f.write(util.write_locks(lock_dict))
         except OSError as e:
-            logging.error("Error on writing lock file %s: %s", path, e)
+            logger.error("Error on writing lock file %s: %s", path, e)
             raise util.AbortError()
```

### Comparing `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/local.py` & `btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/endpoint/local.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""btrfs-backup-ng: btrfs-backup/local.py
+"""btrfs-backup-ng: btrfs_backup_ng/endpoint/local.py
 Create commands with local endpoints.
 """
 
-import logging
 import os
 
 from .common import Endpoint
+from ..rich_logger import logger
 from .. import util
 
 
 class LocalEndpoint(Endpoint):
     """Create a local command endpoint."""
 
     def __init__(self, **kwargs):
@@ -28,28 +28,24 @@
         # create directories, if needed
         dirs = []
         if self.source is not None:
             dirs.append(self.source)
         dirs.append(self.path)
         for d in dirs:
             if not os.path.isdir(d):
-                logging.info("Creating directory: %s", d)
+                logger.info("Creating directory: %s", d)
                 try:
                     os.makedirs(d)
                 except OSError as e:
-                    logging.error("Error creating new location %s: %s", d, e)
+                    logger.error("Error creating new location %s: %s", d, e)
                     raise util.AbortError()
 
         if (
             self.source is not None
             and self.fs_checks
             and not util.is_subvolume(self.source)
         ):
-            logging.error(
-                "%s does not seem to be a btrfs subvolume", self.source
-            )
+            logger.error("%s does not seem to be a btrfs subvolume", self.source)
             raise util.AbortError()
         if self.fs_checks and not util.is_btrfs(self.path):
-            logging.error(
-                "%s does not seem to be on a btrfs filesystem", self.path
-            )
+            logger.error("%s does not seem to be on a btrfs filesystem", self.path)
             raise util.AbortError()
```

### Comparing `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/shell.py` & `btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/endpoint/shell.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""btrfs-backup-ng: btrfs-backup/shell.py
+"""btrfs-backup-ng: btrfs_backup_ng/endpoint/shell.py
 Create destinations with shell command endpoints.
 """
 
 from .common import Endpoint
 
 
 class ShellEndpoint(Endpoint):
```

### Comparing `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/ssh.py` & `btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/endpoint/ssh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""btrfs-backup-ng: btrfs-backup/ssh.py
+"""btrfs-backup-ng: btrfs_backup_ng/endpoint/ssh.py
 Create commands with ssh endpoints.
 """
 
 import copy
-import logging
 import os
 import subprocess
 import tempfile
 
 from .common import Endpoint
+from ..rich_logger import logger
 from .. import util
 
 
 class SSHEndpoint(Endpoint):
     """Commands for creating an ssh endpoint."""
 
     def __init__(
@@ -48,76 +48,72 @@
             s = f"{self.username}@{s}"
         if self.port:
             s = f"{s}:{self.port}"
         return f"ssh://{s}{self.path}"
 
     def _prepare(self):
         # check whether ssh is available
-        logging.debug("Checking for ssh ...")
+        logger.debug("Checking for ssh ...")
         cmd = ["ssh"]
         try:
             util.exec_subprocess(
                 cmd,
                 method="call",
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
             )
         except FileNotFoundError as e:
-            logging.debug("  -> got exception: %s", e)
-            logging.info("ssh command is not available")
+            logger.debug("  -> got exception: %s", e)
+            logger.info("ssh command is not available")
             raise util.AbortError()
 
-        logging.debug("  -> ssh is available")
+        logger.debug("  -> ssh is available")
 
         # sshfs is useful for listing directories and reading/writing locks
         tempdir = tempfile.mkdtemp()
-        logging.debug("Created tempdir: %s", tempdir)
+        logger.debug("Created tempdir: %s", tempdir)
         mount_point = os.path.join(tempdir, "mnt")
         os.makedirs(mount_point)
-        logging.debug("Created directory: %s", mount_point)
-        logging.debug("Mounting sshfs ...")
+        logger.debug("Created directory: %s", mount_point)
+        logger.debug("Mounting sshfs ...")
 
         cmd = ["sshfs"]
         if self.port:
             cmd += ["-p", str(self.port)]
         for opt in self.sshfs_opts:
             cmd += ["-o", opt]
         cmd += [f"{self._build_connect_string()}:/", mount_point]
         try:
-            util.exec_subprocess(
-                cmd, method="check_call", stdout=subprocess.DEVNULL
-            )
+            util.exec_subprocess(cmd, method="check_call", stdout=subprocess.DEVNULL)
         except FileNotFoundError as e:
-            logging.debug("  -> got exception: %s", e)
+            logger.debug("  -> got exception: %s", e)
             if self.source:
                 # we need that for the locks
-                logging.info(
+                logger.info(
                     "  The sshfs command is not available but it is "
                     "mandatory for sourcing from SSH."
                 )
                 raise util.AbortError()
         else:
             self.sshfs = mount_point
-            logging.debug("  -> sshfs is available")
+            logger.debug("  -> sshfs is available")
 
         # create directories, if needed
         dirs = []
         if self.source is not None:
             dirs.append(self.source)
         dirs.append(self.path)
         if self.sshfs:
             for d in dirs:
                 if not os.path.isdir(self._path_to_sshfs(d)):
-                    logging.info("Creating directory: %s", d)
+                    logger.info("Creating directory: %s", d)
                     try:
                         os.makedirs(self._path_to_sshfs(d))
                     except OSError as e:
-                        logging.error(
-                            "Error creating new location %s: %s", d, e
-                        )
+                        logger.error("Error creating new location %s: %s", d, e)
                         raise util.AbortError()
         else:
             cmd = ["mkdir", "-p"] + dirs
             self._exec_command(cmd)
 
     def _collapse_commands(self, commands, abort_on_failure=True):
         """Concatenates all given commands, ';' is inserted as separator."""
```

### Comparing `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/util.py` & `btrfs_backup_ng-0.6.0/src/btrfs_backup_ng/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-"""btrfs-backup-ng: btrfs-backup/util.py
+"""btrfs-backup-ng: btrfs_backup_ng/util.py
 Common utility code shared between modules.
 """
 
 import argparse
 import functools
 import json
-import logging
 import os
 import subprocess
 import sys
 import time
 
+from .rich_logger import logger
+
+
 DATE_FORMAT = "%Y%m%d-%H%M%S"
 MOUNTS_FILE = "/proc/mounts"
 
 
 class AbortError(Exception):
     """Exception where btrfs-backup-ng should abort."""
 
@@ -76,20 +78,20 @@
         return None
 
 
 def exec_subprocess(command, method="check_output", **kwargs):
     """Executes ``getattr(subprocess, method)(cmd, **kwargs)`` and takes
     care of proper logging and error handling. ``AbortError`` is raised
     in case of a ``subprocess.CalledProcessError``."""
-    logging.debug("Executing: %s", command)
+    logger.debug("Executing: %s", command)
     m = getattr(subprocess, method)
     try:
         return m(command, **kwargs)
     except subprocess.CalledProcessError as e:
-        logging.error("Error on command: %s\nCaught: %s", command, e)
+        logger.error("Error on command: %s\nCaught: %s", command, e)
         raise AbortError() from e
 
 
 def log_heading(caption):
     """Formatted heading for logging output sections."""
     return f"{f'--[ {caption} ]':-<50}"
 
@@ -113,57 +115,55 @@
         fmt = DATE_FORMAT
     return time.strptime(time_string, fmt)
 
 
 def is_btrfs(path):
     """Checks whether path is inside a btrfs file system"""
     path = os.path.normpath(os.path.abspath(path))
-    logging.debug("Checking for btrfs filesystem: %s", path)
+    logger.debug("Checking for btrfs filesystem: %s", path)
     best_match = ""
     best_match_fs_type = ""
-    logging.debug("  Reading mounts file: %s", MOUNTS_FILE)
+    logger.debug("  Reading mounts file: %s", MOUNTS_FILE)
     for line in open(MOUNTS_FILE, encoding="utf-8"):
         try:
             mount_point, fs_type = line.split(" ")[1:3]
         except ValueError as e:
-            logging.debug(
-                "  Couldn't split line, skipping: %s\nCaught: %s", line, e
-            )
+            logger.debug("  Couldn't split line, skipping: %s\nCaught: %s", line, e)
             continue
         mount_point_prefix = mount_point
         if not mount_point_prefix.endswith(os.sep):
             mount_point_prefix += os.sep
-        if (
-            path == mount_point or path.startswith(mount_point_prefix)
-        ) and len(mount_point) > len(best_match):
+        if (path == mount_point or path.startswith(mount_point_prefix)) and len(
+            mount_point
+        ) > len(best_match):
             best_match = mount_point
             best_match_fs_type = fs_type
-            logging.debug(
+            logger.debug(
                 "  New best_match with filesystem type %s: %s",
                 best_match_fs_type,
                 best_match,
             )
     result = best_match_fs_type == "btrfs"
-    logging.debug(
+    logger.debug(
         "  -> best_match_fs_type is %s, result is %r",
         best_match_fs_type,
         result,
     )
     return result
 
 
 def is_subvolume(path):
     """Checks whether the given path is a btrfs subvolume."""
     if not is_btrfs(path):
         return False
-    logging.debug("Checking for btrfs subvolume: %s", path)
+    logger.debug("Checking for btrfs subvolume: %s", path)
     # subvolumes always have inode 256
     st = os.stat(path)
     result = st.st_ino == 256
-    logging.debug("  -> Inode is %d, result is %r", st.st_ino, result)
+    logger.debug("  -> Inode is %d, result is %r", st.st_ino, result)
     return result
 
 
 def read_locks(s):
     """Reads locks from lock file content given as string.
     Returns ``{'snap_name': {'locks': ['lock', ...], ...}, 'parent_locks': ['lock', ...]}``.
     If format is invalid, ``ValueError`` is raised."""
@@ -181,15 +181,15 @@
                 assert lock_type in ("locks", "parent_locks")
                 assert isinstance(locks, list)
                 for lock in locks:
                     assert isinstance(lock, str)
                 # eliminate multiple occurrences of locks
                 snapshot_entry[lock_type] = list(set(locks))
     except (AssertionError, json.JSONDecodeError) as e:
-        logging.error("Lock file couldn't be parsed: %s", e)
+        logger.error("Lock file couldn't be parsed: %s", e)
         raise ValueError("invalid lock file format") from e
 
     return content
 
 
 def write_locks(lock_dict):
     """Converts ``lock_dict`` back to the string readable by ``read_locks``."""
@@ -220,17 +220,15 @@
                 try:
                     with open(arg_string[1:], encoding="utf-8") as args_file:
                         for arg_line in args_file.read().splitlines():
                             for arg in self.convert_arg_line_to_args(arg_line):
                                 # make nested includes relative to their parent
                                 if (
                                     self.fromfile_prefix_chars is not None
-                                    and arg.startswith(
-                                        self.fromfile_prefix_chars
-                                    )
+                                    and arg.startswith(self.fromfile_prefix_chars)
                                 ):
                                     dir_name = os.path.dirname(arg_string[1:])
                                     path = os.path.join(dir_name, arg[1:])
                                     # eliminate ../foo/../foo constructs
                                     path = os.path.normpath(path)
                                     arg = arg[0] + path
                                 arg_strings.append(arg)
@@ -264,11 +262,9 @@
         if text.startswith("N|"):
             _lines = text[2:].splitlines()
         else:
             _lines = [text]
         lines = []
         for line in _lines:
             # this is the RawTextHelpFormatter._split_lines
-            lines.extend(
-                argparse.HelpFormatter._split_lines(self, line, width)
-            )
+            lines.extend(argparse.HelpFormatter._split_lines(self, line, width))
         return lines
```

### Comparing `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/PKG-INFO` & `btrfs_backup_ng-0.6.0/src/btrfs_backup_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrfs-backup-ng
-Version: 0.5.9
+Version: 0.6.0
 Summary: Intelligent, feature-rich backups for btrfs
 Author-email: Michael Berry <trismegustis@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/berrym/btrfs-backup-ng
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -40,15 +40,15 @@
 written by Chris Lawrence. Since then, most of the code has been
 refactored and many new features were added before this repository has
 been transferred to Robert Schindler. Many thanks to Chris for his work. The old code
 base has been tagged with `legacy`. If, for any reason, you want to
 continue using it and miss the new features, you can check that out.
 
 Latest release  
-v0.5.9
+v0.6.0
 
 Downloads  
 <http://pypi.python.org/pypi/btrfs_backup_ng>
 
 Source  
 <https://github.com/berrym/btrfs-backup-ng>
 
@@ -96,21 +96,21 @@
 via PIP. If `pip3` is missing on your system, and you run a Debian-based
 distribution, simply install it via:
 
     $ sudo apt-get install python3-pip python3-wheel
 
 Then, you can fetch the latest version of btrfs-backup-ng:
 
-    $ sudo pip3 install btrfs-backup-ng
+    $ pip3 install btrfs-backup-ng
 
 ### Pre-built packages
 
 There are currently pre-built packages available for Fedora and OpenSUSE Tumbleweed:
 
-Fedora 38, Fedora 39, Fedora Rawhide
+Fedora 38, Fedora 39, Fedora 40, Fedora Rawhide
 
     $ dnf copr enable mberry/btrfs-backup-ng
     $ dnf install btrfs-backup-ng --refresh
 
 OpenSUSE Tumbleweed
 
     $ sudo zypper addrepo https://download.opensuse.org/repositories/home:berrym/openSUSE_Tumbleweed/home:berrym.repo
@@ -122,15 +122,15 @@
 Note: This package now uses a pyproject.toml based build as outlined in
 PEP 517 and PEP 621.
 
 Clone this git repository
 
     $ git clone https://github.com/berrym/btrfs-backup-ng.git
     $ cd btrfs-backup-ng
-    $ git checkout tags/v0.5.9  # optionally checkout a specific version
+    $ git checkout tags/v0.6.0  # optionally checkout a specific version
     $ python3 -m venv /path/to/btrfs-backup-ng/venv # optionally use venv
     $ sh /path/to/btrfs-backup-ng/venv/bin/activate # using venv
     $ python3 -m build
     # using venv
     $ python3 -m pip install .
     # or 
     $ sudo python3 -m pip install .
```

### Comparing `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/SOURCES.txt` & `btrfs_backup_ng-0.6.0/src/btrfs_backup_ng.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/btrfs_backup_ng/__init__.py
 src/btrfs_backup_ng/__main__.py
+src/btrfs_backup_ng/rich_logger.py
 src/btrfs_backup_ng/util.py
 src/btrfs_backup_ng.egg-info/PKG-INFO
 src/btrfs_backup_ng.egg-info/SOURCES.txt
 src/btrfs_backup_ng.egg-info/dependency_links.txt
 src/btrfs_backup_ng.egg-info/entry_points.txt
 src/btrfs_backup_ng.egg-info/requires.txt
 src/btrfs_backup_ng.egg-info/top_level.txt
```


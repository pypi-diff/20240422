# Comparing `tmp/Akatosh-2.3.3.tar.gz` & `tmp/akatosh-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-2.3.3.tar", last modified: Wed Jan 10 04:17:45 2024, max compression
+gzip compressed data, was "akatosh-3.0.0.tar", max compression
```

## Comparing `Akatosh-2.3.3.tar` & `akatosh-3.0.0.tar`

### file list

```diff
@@ -1,18 +1,8 @@
-drwxrwxrwx   0        0        0        0 2024-01-10 04:17:45.911916 Akatosh-2.3.3/
-drwxrwxrwx   0        0        0        0 2024-01-10 04:17:45.805479 Akatosh-2.3.3/Akatosh/
--rw-rw-rw-   0        0        0      242 2023-12-12 03:57:46.000000 Akatosh-2.3.3/Akatosh/__init__.py
--rw-rw-rw-   0        0        0    22619 2023-12-12 08:24:11.000000 Akatosh-2.3.3/Akatosh/entity.py
--rw-rw-rw-   0        0        0    15530 2023-12-12 03:57:46.000000 Akatosh-2.3.3/Akatosh/event.py
--rw-rw-rw-   0        0        0      384 2023-12-12 03:57:46.000000 Akatosh-2.3.3/Akatosh/logger.py
--rw-rw-rw-   0        0        0     9397 2024-01-10 04:16:14.000000 Akatosh-2.3.3/Akatosh/resource.py
--rw-rw-rw-   0        0        0      230 2023-12-12 04:08:04.000000 Akatosh-2.3.3/Akatosh/states.py
--rw-rw-rw-   0        0        0     6343 2023-12-12 03:57:46.000000 Akatosh-2.3.3/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2024-01-10 04:17:45.861941 Akatosh-2.3.3/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2830 2024-01-10 04:17:45.000000 Akatosh-2.3.3/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-01-10 04:17:45.000000 Akatosh-2.3.3/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-10 04:17:45.000000 Akatosh-2.3.3/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-01-10 04:17:45.000000 Akatosh-2.3.3/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2830 2024-01-10 04:17:45.903921 Akatosh-2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-12-12 03:57:46.000000 Akatosh-2.3.3/README.md
--rw-rw-rw-   0        0        0      635 2024-01-10 04:16:43.000000 Akatosh-2.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-10 04:17:45.911916 Akatosh-2.3.3/setup.cfg
+-rw-r--r--   0        0        0      546 2024-04-10 03:45:43.677095 akatosh-3.0.0/Akatosh/__init__.py
+-rw-r--r--   0        0        0     4911 2024-04-22 03:58:25.918223 akatosh-3.0.0/Akatosh/entity.py
+-rw-r--r--   0        0        0     5591 2024-04-22 03:58:25.996779 akatosh-3.0.0/Akatosh/event.py
+-rw-r--r--   0        0        0     5230 2024-04-22 03:53:18.056982 akatosh-3.0.0/Akatosh/resource.py
+-rw-r--r--   0        0        0     5576 2024-04-22 03:58:25.939267 akatosh-3.0.0/Akatosh/universe.py
+-rw-r--r--   0        0        0      340 2024-04-22 02:03:33.682580 akatosh-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2324 2024-04-19 03:36:27.289023 akatosh-3.0.0/README.md
+-rw-r--r--   0        0        0     2666 1970-01-01 00:00:00.000000 akatosh-3.0.0/PKG-INFO
```

### Comparing `Akatosh-2.3.3/Akatosh.egg-info/PKG-INFO` & `akatosh-3.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,43 @@
-Metadata-Version: 2.1
-Name: Akatosh
-Version: 2.3.3
-Summary: A simple implement for discrete events simulation.
-Author-email: Yifei Ren <ryf0510@live.com>
-Project-URL: Homepage, https://github.com/ulfaric/Akatosh
-Project-URL: Documentation, https://ulfaric.github.io/Akatosh
-Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-#Akatosh
-
-<p style="text-align: justify;">
-<code>Akatosh</code> is a light-weighted disceret event simulation library. Unlike popular library <code>Simpy</code> which is progress-oriented and you have to write generator function for simulated events or events interaction, `Akatosh` is fully object-oriented that events are encapsulated as `InstantEvent`/`ContinousEvent` with states, priority and a life-cycle. The actual impact of events are simply regular python functions. You could create events all at once, or create event within event. In addition, `Akatosh` is async which means event that are happening at the same simulated time will be executed simultaneously for real, unless they have different priority.
-</p>
-
-<p style="text-align: justify;">
-<code>Akatosh</code> also support <code>Resource</code>, provide all functionalities as it is in <code>Simpy</code> with extra utilities for telemetries collection and interaction with <code>Entity</code>. The <code>Entity</code> is unique to <code>Akatosh</code> which represents a abstract entity with a life-cycle, for example a follower. The <code>Entity</code> supports utility functions to interact with `Resource` and automatically releases all its occupied resources upon termination.
-</p>
-
-<p style="text-align: justify;">
-You probably already noticed that <code>Akatosh</code> is the name of "Dragon God of Time" in elder scroll serie, therefore the singleton class <code>Mundus</code> is the core of the simulation. The <code>Mundus</code> will schedule the events, move forward time and engage async execution.
-</p>
+# Akatosh
+
+`Akatosh` is a light-weighted disceret event simulation library. Unlike popular library `Simpy` which is progress-oriented and you have to write generator function for simulated events or events interaction, `Akatosh` is fully object-oriented that events are encapsulated as `InstantEvent`/`ContinousEvent` with states, priority and a life-cycle. The actual impact of events are simply regular python functions. You could create events all at once, or create event within event. In addition, `Akatosh` is async which means event that are happening at the same simulated time will be executed simultaneously for real, unless they have different priority.
+
+`Akatosh` also support `Resource`, provide all functionalities as it is in `Simpy` with extra utilities for telemetries collection and interaction with `Entity`. The `Entity` is unique to `Akatosh` which represents a abstract entity with a life-cycle, for example a follower. The `Entity` supports utility functions to interact with `Resource` and automatically releases all its occupied resources upon termination.
+
+You probably already noticed that `Akatosh` is the name of "Dragon God of Time" in elder scroll serie, therefore the singleton class `Mundus` is the core of the simulation. The `Mundus` will schedule the events, move forward time and engage async execution.
 
 To use `Akatosh`:
-```
+
+```bash
 pip install -U Akatosh
 ```
 
 A basic example is showing below, for more information please look at *Examples* and *API Reference*, full documentation is available at https://ulfaric.github.io/Akatosh/.
 
 ```py
-import logging
-
-from Akatosh import event, Mundus
-
-# create two instant event at simulation time 1.0 and 5.0
-@event(at=5)
-def hellow_world_again():
-    print(f"{Mundus.now}:\tHello World! Again!")
-
-
-@event(at=1)
-def hellow_world():
-    print(f"{Mundus.now}:\tHello World!")
+from Akatosh.universe import universe
+from Akatosh.resource import Resource
+from Akatosh.entity import Entity
+from Akatosh.event import Event
+
+# create a resource with capacity of 100 and current level 50
+res = Resource(100.0, 50.0)
+
+# create a instance event happens at 0.9s
+lock = Event(0.9,0.9, lambda: print("Unlocked!"))
+
+# indicate a user entity should be created after lock event ended, wait till 1.1s.
+user = Entity(lock, 1.1, "User")
+
+# indicate user entity engage a event at 1.2s
+@user.event(1.2,1.2, "Use Resource")
+def user_event():
+    if res.distribute(user, 1):
+        print(res.level)
+    else:
+        print("Not enough resource")
 
-# enable debug message
-Mundus.set_logger(logging.DEBUG)
 
-# run simulation for 6s
-Mundus.simulate(6)
+# run simulation for 1.2s
+universe.simulate(1.2)
 ```
```


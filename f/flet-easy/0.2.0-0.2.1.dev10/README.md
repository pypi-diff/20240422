# Comparing `tmp/flet_easy-0.2.0.tar.gz` & `tmp/flet_easy-0.2.1.dev10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_easy-0.2.0.tar", last modified: Sat Apr 20 17:16:35 2024, max compression
+gzip compressed data, was "flet_easy-0.2.1.dev10.tar", last modified: Mon Apr 22 03:26:28 2024, max compression
```

## Comparing `flet_easy-0.2.0.tar` & `flet_easy-0.2.1.dev10.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11541 2024-04-12 03:06:37.458807 flet_easy-0.2.0/LICENSE
--rw-r--r--   0        0        0    11541 2024-04-12 03:06:37.458807 flet_easy-0.2.0/LICENSE
--rw-r--r--   0        0        0     5912 2024-04-20 16:33:47.462133 flet_easy-0.2.0/README.md
--rw-r--r--   0        0        0     5912 2024-04-20 16:33:47.462133 flet_easy-0.2.0/README.md
--rw-r--r--   0        0        0     1727 2024-04-20 17:16:35.137954 flet_easy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      432 2024-04-12 03:14:22.077045 flet_easy-0.2.0/src/flet_easy/__init__.py
--rw-r--r--   0        0        0     1282 2024-04-19 00:12:26.486653 flet_easy-0.2.0/src/flet_easy/auto_route.py
--rw-r--r--   0        0        0     2356 2024-04-12 03:14:22.079042 flet_easy-0.2.0/src/flet_easy/cli/copy.py
--rw-r--r--   0        0        0     2099 2024-04-18 16:58:31.614890 flet_easy-0.2.0/src/flet_easy/cli/main.py
--rw-r--r--   0        0        0     3266 2024-04-12 03:14:22.080559 flet_easy-0.2.0/src/flet_easy/cli/templates/.gitignore
--rw-r--r--   0        0        0      213 2024-04-12 03:14:22.081589 flet_easy-0.2.0/src/flet_easy/cli/templates/README.md
--rw-r--r--   0        0        0     1020 2024-04-12 03:14:22.081589 flet_easy-0.2.0/src/flet_easy/cli/templates/assets/favicon.png
--rw-r--r--   0        0        0    30189 2024-04-12 03:14:22.082609 flet_easy-0.2.0/src/flet_easy/cli/templates/assets/icon.png
--rw-r--r--   0        0        0     7610 2024-04-12 03:14:22.083607 flet_easy-0.2.0/src/flet_easy/cli/templates/assets/icons/icon-192.png
--rw-r--r--   0        0        0    33055 2024-04-12 03:14:22.084612 flet_easy-0.2.0/src/flet_easy/cli/templates/assets/icons/icon-512.png
--rw-r--r--   0        0        0     7610 2024-04-12 03:14:22.085610 flet_easy-0.2.0/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    33055 2024-04-12 03:14:22.086618 flet_easy-0.2.0/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    56474 2024-04-12 03:14:22.087607 flet_easy-0.2.0/src/flet_easy/cli/templates/assets/icons/loading-animation.png
--rw-r--r--   0        0        0     3626 2024-04-12 03:14:22.088615 flet_easy-0.2.0/src/flet_easy/cli/templates/assets/index.html
--rw-r--r--   0        0        0      932 2024-04-12 03:14:22.088615 flet_easy-0.2.0/src/flet_easy/cli/templates/assets/manifest.json
--rw-r--r--   0        0        0       84 2024-04-12 03:14:22.090138 flet_easy-0.2.0/src/flet_easy/cli/templates/components/__init__.py
--rw-r--r--   0        0        0     2422 2024-04-12 03:14:22.090138 flet_easy-0.2.0/src/flet_easy/cli/templates/components/counter.py
--rw-r--r--   0        0        0      543 2024-04-12 03:14:22.091176 flet_easy-0.2.0/src/flet_easy/cli/templates/components/swoDrawer.py
--rw-r--r--   0        0        0       45 2024-04-12 03:14:22.091176 flet_easy-0.2.0/src/flet_easy/cli/templates/controllers/__init__.py
--rw-r--r--   0        0        0     1258 2024-04-12 03:14:22.091176 flet_easy-0.2.0/src/flet_easy/cli/templates/controllers/counter.py
--rw-r--r--   0        0        0        0 2024-04-12 03:14:22.092763 flet_easy-0.2.0/src/flet_easy/cli/templates/core/__init__.py
--rw-r--r--   0        0        0     1662 2024-04-12 03:14:22.093720 flet_easy-0.2.0/src/flet_easy/cli/templates/core/config.py
--rw-r--r--   0        0        0      246 2024-04-19 16:50:45.518416 flet_easy-0.2.0/src/flet_easy/cli/templates/main.py
--rw-r--r--   0        0        0        0 2024-04-12 03:14:22.094724 flet_easy-0.2.0/src/flet_easy/cli/templates/models/__init__.py
--rw-r--r--   0        0        0      588 2024-04-12 03:14:22.096720 flet_easy-0.2.0/src/flet_easy/cli/templates/views/counter.py
--rw-r--r--   0        0        0      615 2024-04-16 23:25:58.330304 flet_easy-0.2.0/src/flet_easy/cli/templates/views/index.py
--rw-r--r--   0        0        0    12208 2024-04-16 21:36:20.961519 flet_easy-0.2.0/src/flet_easy/datasy.py
--rw-r--r--   0        0        0      187 2024-04-12 03:14:22.098727 flet_easy-0.2.0/src/flet_easy/extra.py
--rw-r--r--   0        0        0     2483 2024-04-12 03:14:22.098727 flet_easy-0.2.0/src/flet_easy/extrasJwt.py
--rw-r--r--   0        0        0    18351 2024-04-18 15:59:12.014794 flet_easy-0.2.0/src/flet_easy/fletEasy.py
--rw-r--r--   0        0        0     9856 2024-04-16 17:27:34.348744 flet_easy-0.2.0/src/flet_easy/inheritance.py
--rw-r--r--   0        0        0     1191 2024-04-16 21:14:26.280232 flet_easy-0.2.0/src/flet_easy/job.py
--rw-r--r--   0        0        0     4024 2024-04-16 21:27:52.940346 flet_easy-0.2.0/src/flet_easy/jwt.py
--rw-r--r--   0        0        0     7512 2024-04-16 17:27:54.461988 flet_easy-0.2.0/src/flet_easy/pagesy.py
--rw-r--r--   0        0        0    11272 2024-04-19 16:32:26.352407 flet_easy-0.2.0/src/flet_easy/route.py
--rw-r--r--   0        0        0     1540 2024-04-12 03:14:22.105829 flet_easy-0.2.0/src/flet_easy/view_404.py
--rw-r--r--   0        0        0     6942 1970-01-01 00:00:00.000000 flet_easy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11541 2024-04-22 02:46:04.968016 flet_easy-0.2.1.dev10/LICENSE
+-rw-r--r--   0        0        0    11541 2024-04-22 02:46:04.968016 flet_easy-0.2.1.dev10/LICENSE
+-rw-r--r--   0        0        0     5794 2024-04-22 02:46:04.968016 flet_easy-0.2.1.dev10/README.md
+-rw-r--r--   0        0        0     5794 2024-04-22 02:46:04.968016 flet_easy-0.2.1.dev10/README.md
+-rw-r--r--   0        0        0     1889 2024-04-22 03:26:28.417297 flet_easy-0.2.1.dev10/pyproject.toml
+-rw-r--r--   0        0        0      432 2024-04-22 02:46:05.087392 flet_easy-0.2.1.dev10/src/flet_easy/__init__.py
+-rw-r--r--   0        0        0     1282 2024-04-22 02:46:05.088420 flet_easy-0.2.1.dev10/src/flet_easy/auto_route.py
+-rw-r--r--   0        0        0     2356 2024-04-22 02:46:05.088943 flet_easy-0.2.1.dev10/src/flet_easy/cli/copy.py
+-rw-r--r--   0        0        0     2099 2024-04-22 02:46:05.089968 flet_easy-0.2.1.dev10/src/flet_easy/cli/main.py
+-rw-r--r--   0        0        0     3266 2024-04-22 02:46:05.090972 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/.gitignore
+-rw-r--r--   0        0        0      213 2024-04-22 02:46:05.090972 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/README.md
+-rw-r--r--   0        0        0     1020 2024-04-22 02:46:05.091969 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/favicon.png
+-rw-r--r--   0        0        0    30189 2024-04-22 02:46:05.092969 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icon.png
+-rw-r--r--   0        0        0     7610 2024-04-22 02:46:05.093972 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-192.png
+-rw-r--r--   0        0        0    33055 2024-04-22 02:46:05.093972 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-512.png
+-rw-r--r--   0        0        0     7610 2024-04-22 02:46:05.094968 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    33055 2024-04-22 02:46:05.096024 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    56474 2024-04-22 02:46:05.097486 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/loading-animation.png
+-rw-r--r--   0        0        0     3626 2024-04-22 02:46:05.097486 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/index.html
+-rw-r--r--   0        0        0      932 2024-04-22 02:46:05.098514 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/manifest.json
+-rw-r--r--   0        0        0       84 2024-04-22 02:46:05.099510 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/components/__init__.py
+-rw-r--r--   0        0        0     2422 2024-04-22 02:46:05.100031 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/components/counter.py
+-rw-r--r--   0        0        0      543 2024-04-22 02:46:05.100031 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/components/swoDrawer.py
+-rw-r--r--   0        0        0       45 2024-04-22 02:46:05.101050 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/controllers/__init__.py
+-rw-r--r--   0        0        0     1258 2024-04-22 02:46:05.102079 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/controllers/counter.py
+-rw-r--r--   0        0        0        0 2024-04-22 02:46:05.102079 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/core/__init__.py
+-rw-r--r--   0        0        0     1662 2024-04-22 02:46:05.103083 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/core/config.py
+-rw-r--r--   0        0        0      246 2024-04-22 02:46:05.103083 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/main.py
+-rw-r--r--   0        0        0        0 2024-04-22 02:46:05.104076 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/models/__init__.py
+-rw-r--r--   0        0        0      588 2024-04-22 02:46:05.105080 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/views/counter.py
+-rw-r--r--   0        0        0      615 2024-04-22 02:46:05.105080 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/views/index.py
+-rw-r--r--   0        0        0    12208 2024-04-22 02:46:05.106146 flet_easy-0.2.1.dev10/src/flet_easy/datasy.py
+-rw-r--r--   0        0        0      187 2024-04-22 02:46:05.107076 flet_easy-0.2.1.dev10/src/flet_easy/extra.py
+-rw-r--r--   0        0        0     2483 2024-04-22 02:46:05.107593 flet_easy-0.2.1.dev10/src/flet_easy/extrasJwt.py
+-rw-r--r--   0        0        0    18351 2024-04-22 02:46:05.107593 flet_easy-0.2.1.dev10/src/flet_easy/fletEasy.py
+-rw-r--r--   0        0        0     9856 2024-04-22 02:46:05.108619 flet_easy-0.2.1.dev10/src/flet_easy/inheritance.py
+-rw-r--r--   0        0        0     1191 2024-04-22 02:46:05.110135 flet_easy-0.2.1.dev10/src/flet_easy/job.py
+-rw-r--r--   0        0        0     4024 2024-04-22 02:46:05.110135 flet_easy-0.2.1.dev10/src/flet_easy/jwt.py
+-rw-r--r--   0        0        0     7512 2024-04-22 02:46:05.111160 flet_easy-0.2.1.dev10/src/flet_easy/pagesy.py
+-rw-r--r--   0        0        0    11143 2024-04-22 02:59:13.549820 flet_easy-0.2.1.dev10/src/flet_easy/route.py
+-rw-r--r--   0        0        0     1540 2024-04-22 02:46:05.112163 flet_easy-0.2.1.dev10/src/flet_easy/view_404.py
+-rw-r--r--   0        0        0     6937 1970-01-01 00:00:00.000000 flet_easy-0.2.1.dev10/PKG-INFO
```

### Comparing `flet_easy-0.2.0/LICENSE` & `flet_easy-0.2.1.dev10/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/README.md` & `flet_easy-0.2.1.dev10/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 
 # 🔥Flet-Easy
 `Flet-Easy` is a package built as an add-on for [`Flet`](https://github.com/flet-dev/flet), designed for beginners what it does is to make `Flet` easier when building your apps, with a tidier and simpler code.
 
 ## Features
 * Easy to use (**hence the name**).
 * Facilitates `flet` event handling.
-* Simple page routing (There are three ways) for whichever one suits you best. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/dynamic-routes/))
+* Simple page routing (There are three ways) for whichever one suits you best. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/dynamic-routes/))
 * App construction with numerous pages and custom flet configurations for desktop, mobile and web sites.
 * Provides a better construction of your code, which can be scalable and easy to read (it adapts to your preferences, there are no limitations).
-* Dynamic routing, customization in the routes for greater accuracy in sending data. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/dynamic-routes/#custom-validation))
-* Routing protection ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Customized-app/Route-protection/))
-* Custom Page 404 ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Customized-app/Page-404/))
-* Controlled data sharing between pages. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Data-sharing-between-pages/))
+* Dynamic routing, customization in the routes for greater accuracy in sending data. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/dynamic-routes/#custom-validation))
+* Routing protection ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Customized-app/Route-protection/))
+* Custom Page 404 ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Customized-app/Page-404/))
+* Controlled data sharing between pages. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Data-sharing-between-pages/))
 * Asynchronous support.
-* Middleware Support (in the app in general and in each of the pages). ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Midleware/))
-* JWT support for authentication sessions in the data parameter. (useful to control the time of sessions) ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Basic-JWT/))
-* Working with other applications. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Data-sharing-between-pages/))
-* CLI to create app structure `FletEasy` (`fs init`) ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/CLI-to-create-app/))
-* Easy integration of `on_keyboard_event` in each of the pages. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Events/keyboard-event/))
-* Use the percentage of the page width and height of the page with `on_resize`. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Events/On-resize/))
-* `ResponsiveControlsy` control to make the app responsive, useful for desktop applications. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/ResponsiveControlsy/))
-* Soporta Application Packaging para su distribución. [view](https://flet.dev/docs/publish)
+* Middleware Support (in the app in general and in each of the pages). ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Midleware/))
+* JWT support for authentication sessions in the data parameter. (useful to control the time of sessions) ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Basic-JWT/))
+* Working with other applications. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Data-sharing-between-pages/))
+* CLI to create app structure `FletEasy` (`fs init`) ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/CLI-to-create-app/))
+* Easy integration of `on_keyboard_event` in each of the pages. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Events/keyboard-event/))
+* Use the percentage of the page width and height of the page with `on_resize`. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Events/On-resize/))
+* `ResponsiveControlsy` control to make the app responsive, useful for desktop applications. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/ResponsiveControlsy/))
+* Soporta Application Packaging para su distribución. ([view](https://flet.dev/docs/publish))
 
 ## 📌Flet events it handles
 
 - `on_route_change` :  Dynamic routing
 - `on_view_pop`
 - `on_keyboard_event`
 - `on_resize`
```

### Comparing `flet_easy-0.2.0/pyproject.toml` & `flet_easy-0.2.1.dev10/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flet-easy"
-version = "0.2.0"
+version = "0.2.1.dev10"
 description = "Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features."
 authors = [
     { name = "Daxexs", email = "Daxexsdev@gmail.com" },
 ]
 dependencies = [
     "parse>=1.20.1",
     "pyJWT>=2.8.0",
@@ -14,15 +14,22 @@
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "flet easy",
     "flet",
     "python",
-    "flet router",
+    "flet easy route",
+    "python web template",
+    "app python",
+    "flet mvc",
+    "flet easy mvc",
+    "flet easy fastapi",
+    "flutter python",
+    "web application",
 ]
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `flet_easy-0.2.0/src/flet_easy/auto_route.py` & `flet_easy-0.2.1.dev10/src/flet_easy/auto_route.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/copy.py` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/copy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/main.py` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/main.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/.gitignore` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/assets/favicon.png` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/assets/icon.png` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icon.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/assets/icons/icon-192.png` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/assets/icons/icon-512.png` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/assets/icons/loading-animation.png` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/assets/index.html` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/index.html`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/assets/manifest.json` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/manifest.json`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/components/counter.py` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/components/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/components/swoDrawer.py` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/components/swoDrawer.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/controllers/counter.py` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/controllers/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/core/config.py` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/core/config.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/views/counter.py` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/views/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/cli/templates/views/index.py` & `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/views/index.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/datasy.py` & `flet_easy-0.2.1.dev10/src/flet_easy/datasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/extrasJwt.py` & `flet_easy-0.2.1.dev10/src/flet_easy/extrasJwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/fletEasy.py` & `flet_easy-0.2.1.dev10/src/flet_easy/fletEasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/inheritance.py` & `flet_easy-0.2.1.dev10/src/flet_easy/inheritance.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/job.py` & `flet_easy-0.2.1.dev10/src/flet_easy/job.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/jwt.py` & `flet_easy-0.2.1.dev10/src/flet_easy/jwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/pagesy.py` & `flet_easy-0.2.1.dev10/src/flet_easy/pagesy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/src/flet_easy/route.py` & `flet_easy-0.2.1.dev10/src/flet_easy/route.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,23 +147,22 @@
         if iscoroutinefunction(self.__view_data):
             return await self.__view_data(self.__data)
         else:
             return self.__view_data(self.__data)
 
     async def _view_append(self, route: str):
         """Add a new page and update it."""
-        if iscoroutinefunction(self.__pagesy.view):
-            view = await self.__pagesy.view(self.__data, **self.__data.url_params)
-            view.route = route
-            self.__page.views.append(view)
-        else:
-            view = self.__pagesy.view(self.__data, **self.__data.url_params)
-            view.route = route
-            self.__page.views.append(self.__pagesy.view(self.__data, **self.__data.url_params))
+        view = (
+            await self.__pagesy.view(self.__data, **self.__data.url_params)
+            if iscoroutinefunction(self.__pagesy.view)
+            else self.__pagesy.view(self.__data, **self.__data.url_params)
+        )
 
+        view.route = route
+        self.__page.views.append(view)
         self.__page.route = route
         self.__page.query()
         self.__page.update()
 
     def __reload_datasy(self, url_params: Dict[str, Any] = None):
         """Update `datasy` values when switching between pages."""
         self.__page.title = self.__pagesy.title
```

### Comparing `flet_easy-0.2.0/src/flet_easy/view_404.py` & `flet_easy-0.2.1.dev10/src/flet_easy/view_404.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.0/PKG-INFO` & `flet_easy-0.2.1.dev10/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: flet-easy
-Version: 0.2.0
+Version: 0.2.1.dev10
 Summary: Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features.
-Keywords: flet easy,flet,python,flet router
+Keywords: flet easy,flet,python,flet easy route,python web template,app python,flet mvc,flet easy mvc,flet easy fastapi,flutter python,web application
 Author-Email: Daxexs <Daxexsdev@gmail.com>
 License: apache-2.0
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -37,30 +37,30 @@
 
 # 🔥Flet-Easy
 `Flet-Easy` is a package built as an add-on for [`Flet`](https://github.com/flet-dev/flet), designed for beginners what it does is to make `Flet` easier when building your apps, with a tidier and simpler code.
 
 ## Features
 * Easy to use (**hence the name**).
 * Facilitates `flet` event handling.
-* Simple page routing (There are three ways) for whichever one suits you best. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/dynamic-routes/))
+* Simple page routing (There are three ways) for whichever one suits you best. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/dynamic-routes/))
 * App construction with numerous pages and custom flet configurations for desktop, mobile and web sites.
 * Provides a better construction of your code, which can be scalable and easy to read (it adapts to your preferences, there are no limitations).
-* Dynamic routing, customization in the routes for greater accuracy in sending data. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/dynamic-routes/#custom-validation))
-* Routing protection ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Customized-app/Route-protection/))
-* Custom Page 404 ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Customized-app/Page-404/))
-* Controlled data sharing between pages. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Data-sharing-between-pages/))
+* Dynamic routing, customization in the routes for greater accuracy in sending data. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/dynamic-routes/#custom-validation))
+* Routing protection ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Customized-app/Route-protection/))
+* Custom Page 404 ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Customized-app/Page-404/))
+* Controlled data sharing between pages. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Data-sharing-between-pages/))
 * Asynchronous support.
-* Middleware Support (in the app in general and in each of the pages). ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Midleware/))
-* JWT support for authentication sessions in the data parameter. (useful to control the time of sessions) ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Basic-JWT/))
-* Working with other applications. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Data-sharing-between-pages/))
-* CLI to create app structure `FletEasy` (`fs init`) ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/CLI-to-create-app/))
-* Easy integration of `on_keyboard_event` in each of the pages. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Events/keyboard-event/))
-* Use the percentage of the page width and height of the page with `on_resize`. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/Events/On-resize/))
-* `ResponsiveControlsy` control to make the app responsive, useful for desktop applications. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/flet-easy/ResponsiveControlsy/))
-* Soporta Application Packaging para su distribución. [view](https://flet.dev/docs/publish)
+* Middleware Support (in the app in general and in each of the pages). ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Midleware/))
+* JWT support for authentication sessions in the data parameter. (useful to control the time of sessions) ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Basic-JWT/))
+* Working with other applications. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Data-sharing-between-pages/))
+* CLI to create app structure `FletEasy` (`fs init`) ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/CLI-to-create-app/))
+* Easy integration of `on_keyboard_event` in each of the pages. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Events/keyboard-event/))
+* Use the percentage of the page width and height of the page with `on_resize`. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/Events/On-resize/))
+* `ResponsiveControlsy` control to make the app responsive, useful for desktop applications. ([**`Docs`**](https://daxexs.github.io/flet-easy/latest/ResponsiveControlsy/))
+* Soporta Application Packaging para su distribución. ([view](https://flet.dev/docs/publish))
 
 ## 📌Flet events it handles
 
 - `on_route_change` :  Dynamic routing
 - `on_view_pop`
 - `on_keyboard_event`
 - `on_resize`
```


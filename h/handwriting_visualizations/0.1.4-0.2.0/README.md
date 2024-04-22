# Comparing `tmp/handwriting_visualizations-0.1.4.tar.gz` & `tmp/handwriting_visualizations-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handwriting_visualizations-0.1.4.tar", max compression
+gzip compressed data, was "handwriting_visualizations-0.2.0.tar", max compression
```

## Comparing `handwriting_visualizations-0.1.4.tar` & `handwriting_visualizations-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0       59 2023-12-12 10:10:11.514312 handwriting_visualizations-0.1.4/README.md
--rwxr-xr-x   0        0        0      156 2023-12-05 17:23:32.604793 handwriting_visualizations-0.1.4/handwriting_visualizations/AdvancedPlots.py
--rwxr-xr-x   0        0        0     4971 2023-12-12 10:08:53.519189 handwriting_visualizations-0.1.4/handwriting_visualizations/Configs.py
--rwxr-xr-x   0        0        0      725 2023-12-11 18:21:52.046814 handwriting_visualizations-0.1.4/handwriting_visualizations/SimplePlots.py
--rwxr-xr-x   0        0        0        0 2023-12-05 17:52:26.822664 handwriting_visualizations-0.1.4/handwriting_visualizations/__init__.py
--rwxr-xr-x   0        0        0      479 2023-12-11 18:21:52.570811 handwriting_visualizations-0.1.4/handwriting_visualizations/handwriting_visualisations.py
--rwxr-xr-x   0        0        0     2151 2023-12-11 18:23:55.687405 handwriting_visualizations-0.1.4/handwriting_visualizations/visualization_tools.py
--rwxr-xr-x   0        0        0      331 2023-12-12 10:10:05.502847 handwriting_visualizations-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 handwriting_visualizations-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0      373 2024-04-22 06:46:22.392357 handwriting_visualizations-0.2.0/README.md
+-rwxr-xr-x   0        0        0      156 2024-04-22 06:13:02.432650 handwriting_visualizations-0.2.0/handwriting_visualizations/AdvancedPlots.py
+-rwxr-xr-x   0        0        0     5276 2024-04-22 06:13:02.433651 handwriting_visualizations-0.2.0/handwriting_visualizations/Configs.py
+-rwxr-xr-x   0        0        0     1588 2024-04-22 06:13:02.434650 handwriting_visualizations-0.2.0/handwriting_visualizations/SimplePlots.py
+-rwxr-xr-x   0        0        0        0 2024-04-22 06:13:02.454652 handwriting_visualizations-0.2.0/handwriting_visualizations/__init__.py
+-rwxr-xr-x   0        0        0      479 2024-04-22 06:13:02.472649 handwriting_visualizations-0.2.0/handwriting_visualizations/handwriting_visualisations.py
+-rwxr-xr-x   0        0        0     2151 2024-04-22 06:13:02.503651 handwriting_visualizations-0.2.0/handwriting_visualizations/visualization_tools.py
+-rwxr-xr-x   0        0        0      348 2024-04-22 06:13:02.504649 handwriting_visualizations-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 handwriting_visualizations-0.2.0/PKG-INFO
```

### Comparing `handwriting_visualizations-0.1.4/handwriting_visualizations/Configs.py` & `handwriting_visualizations-0.2.0/handwriting_visualizations/Configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,29 +15,31 @@
         if "output" not in custom_config:
             self.custom_config["output"] = "fig"
         if "show_legend" not in custom_config:
             self.custom_config["show_legend"] = True
         if "include_js" not in custom_config:
             self.custom_config["include_js"] = False
         if "margin" not in custom_config:
-            self.custom_config["margin"] = {"t":100, "r":80, "b":80, "l":80}
+            self.custom_config["margin"] = {"t":10, "r":10, "b":10, "l":10}
+        if "height" not in custom_config:
+            self.custom_config["height"] = 500
 
     def get_config(self):
         config = {}
         config["body"] = \
             [
                 [
                     {
                         "name": "X",
                         "x": self.x,
                         "y": self.y,
                         "mode": "lines",
                         "line": {
-                            "color": "blue",
-                            "width": 3
+                            "color": "black",
+                            "width": 2
                         },
                         "opacity": 0.65,
                     },
                     {
                         "_config": {  # https://plotly.com/python/axes/
                             "update_xaxes": {
                                 "title_text": self.custom_config["x_title_text"],
@@ -87,28 +89,31 @@
                 "rows": 1,
                 "cols": 1,
                 # "column_widths": [0.5, 0.5],
                 "vertical_spacing": 0.14,
                 "subplot_titles": ["1"]},
             "layout": {  # https://plotly.com/python/reference/layout/
                 "showlegend": self.custom_config['show_legend'],
-                # "title": "Časové řady",
                 "autosize": True,
+                "height": self.custom_config["height"],
+                # "title": "Časové řady",
                 "margin": self.custom_config["margin"],
                 "font": {
                     "family": "Georgia",
                     "size": 22,
                     "color": "black"
                 },
                 "legend": {
                     "orientation": "h",
                     "yanchor": "top",
                     "xanchor": "center",
                     "y": -0.1,
-                    "x": 0.5}
+                    "x": 0.5},
+                "paper_bgcolor": "rgb(255, 255, 255)",  # Background color for the entire plot area
+                "plot_bgcolor": "rgb(245, 245, 220)",
             },
             "display": self.custom_config["display"],
             "output": self.custom_config["output"],
             "picture": {},
             "include_js": self.custom_config["include_js"],
         }
         return config
```

### Comparing `handwriting_visualizations-0.1.4/handwriting_visualizations/visualization_tools.py` & `handwriting_visualizations-0.2.0/handwriting_visualizations/visualization_tools.py`

 * *Files identical despite different names*


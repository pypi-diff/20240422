# Comparing `tmp/pygubu_designer-0.39.tar.gz` & `tmp/pygubu_designer-0.39.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygubu_designer-0.39.tar", last modified: Wed Apr 17 00:46:57 2024, max compression
+gzip compressed data, was "pygubu_designer-0.39.1.tar", last modified: Mon Apr 22 01:14:39 2024, max compression
```

## Comparing `pygubu_designer-0.39.tar` & `pygubu_designer-0.39.1.tar`

### file list

```diff
@@ -1,759 +1,759 @@
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.911082 pygubu_designer-0.39/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       67 2023-09-09 20:40:32.000000 pygubu_designer-0.39/AUTHORS
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5128 2023-09-09 20:40:32.000000 pygubu_designer-0.39/LEEME.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    35064 2023-09-09 20:40:32.000000 pygubu_designer-0.39/LICENSE.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6509 2023-09-09 20:40:32.000000 pygubu_designer-0.39/LISEZMOI.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      248 2023-09-09 20:40:32.000000 pygubu_designer-0.39/MANIFEST.in
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7697 2024-04-17 00:46:57.911082 pygubu_designer-0.39/PKG-INFO
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5007 2023-09-09 20:40:32.000000 pygubu_designer-0.39/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.787082 pygubu_designer-0.39/development/
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     6434 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/create-imgs.py
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     6817 2024-03-17 20:08:13.000000 pygubu_designer-0.39/development/dev-notes.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2186 2024-04-08 04:51:29.000000 pygubu_designer-0.39/development/devtool.py
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     3885 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/devtool.sh
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.787082 pygubu_designer-0.39/development/gettext/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1037 2024-04-09 23:44:02.000000 pygubu_designer-0.39/development/gettext/pygubu.its
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2024-04-09 23:44:02.000000 pygubu_designer-0.39/development/gettext/pygubu.loc
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.791082 pygubu_designer-0.39/development/new-designer-icons/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2780 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/main.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.799082 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2129 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/button.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7010 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/button.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3744 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/canvas.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4072 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/canvas.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2101 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/combobox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9271 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/combobox.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1252 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/default.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4185 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/default.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      665 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/entry.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3834 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/entry.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1552 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/frame.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6047 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/frame.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1142 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/label.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5074 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/label.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1666 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/labelframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6735 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/labelframe.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2133 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/menubutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8598 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/menubutton.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      962 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook-tab.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3043 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook-tab.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1060 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3693 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      797 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3257 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      782 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3238 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1077 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/progressbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5356 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/progressbar.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/rect848.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1786 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/spinbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8481 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/spinbutton.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1126 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/textview.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6381 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/textview.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      867 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/toplevel.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3229 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/toplevel.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1068 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview-col.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5481 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview-col.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      935 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4893 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2489 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/viewport.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7036 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/viewport.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4315 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/template.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7552 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/testnewicons.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      854 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/new-designer-icons/testnewiconsapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.799082 pygubu_designer-0.39/development/pygubuLogo/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5501 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/Python-logo-notext.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)   174121 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/logo_pygubu .ico
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)   101863 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/logo_pygubu.icns
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)   174121 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/logo_pygubu.ico
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)   175900 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/logo_pygubu.xcf
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)   124131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/pyGubu_newLogo.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       92 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/rootOfSVGs.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10232 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubuLogo/tcl-tk.svg
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/pygubudesigner_.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       11 2023-09-09 20:40:32.000000 pygubu_designer-0.39/development/requirements.txt
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.803082 pygubu_designer-0.39/examples/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.803082 pygubu_designer-0.39/examples/7guis/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.803082 pygubu_designer-0.39/examples/7guis/01_counter/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1256 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/01_counter/counter.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      798 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/01_counter/counterapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.803082 pygubu_designer-0.39/examples/7guis/02_temperature_converter/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2687 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/02_temperature_converter/tempconv.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1648 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/02_temperature_converter/tempconvapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.803082 pygubu_designer-0.39/examples/7guis/03_flight_Booker/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2648 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/03_flight_Booker/flight_booker.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3212 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/03_flight_Booker/flightbookerapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.803082 pygubu_designer-0.39/examples/7guis/04_timer/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4089 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/04_timer/timer.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1777 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/04_timer/timerapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       81 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/7guis/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      347 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      546 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/binding.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      960 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/button_cb.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2053 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/button_cb.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.775082 pygubu_designer-0.39/examples/canvas/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/canvas/canvas-scrollregion/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      106 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/canvas/canvas-scrollregion/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5196 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/canvas/canvas-scrollregion/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5211 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/canvas/canvas-scrollregion/myapp.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      842 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/canvas_example.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/command_properties/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1221 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/command_properties/command_properties.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2641 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/command_properties/command_properties.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1256 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/command_properties/command_properties2.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3116 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/commands.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    18575 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/commands.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/control_variables/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      584 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/control_variables/controlvariables.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3634 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/control_variables/controlvariables.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/custom_widget/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      436 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/custom_widget/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1311 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/custom_widget/timer_main.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      515 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/custom_widget/timerapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      287 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/custom_widget/timerappwidgets.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2363 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/custom_widget/timewidget.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/customtkinter/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      174 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/customtkinter/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/customtkinter/complex/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    22578 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/customtkinter/complex/complex_demo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2365 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/customtkinter/complex/complexdemoapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/customtkinter/simple/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6284 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/customtkinter/simple/simple_demo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1269 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/customtkinter/simple/simpledemoapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/dialogs/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       51 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/dialogs/demo1/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       73 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo1/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1178 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo1/demo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5699 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo1/demo.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.807082 pygubu_designer-0.39/examples/dialogs/demo2/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       95 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo2/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1319 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo2/demo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4523 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo2/demo.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.811082 pygubu_designer-0.39/examples/dialogs/demo3/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       98 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo3/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4883 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo3/demo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9704 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo3/demo.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.811082 pygubu_designer-0.39/examples/dialogs/demo4/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      314 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo4/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.811082 pygubu_designer-0.39/examples/dialogs/demo4/__pycache__/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3373 2023-09-30 23:40:25.000000 pygubu_designer-0.39/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-311.pyc
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6987 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo4/settingsdemo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1002 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo4/settingsdemoapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1319 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/dialogs/demo4/settingsdialog.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1471 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/example_grid_rc.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1631 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/example_grid_rc_2.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.811082 pygubu_designer-0.39/examples/forms/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.811082 pygubu_designer-0.39/examples/forms/__pycache__/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1939 2024-04-13 02:37:32.000000 pygubu_designer-0.39/examples/forms/__pycache__/formsdemo1appui.cpython-311.pyc
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2087 2024-02-04 03:08:22.000000 pygubu_designer-0.39/examples/forms/__pycache__/formsdemo1base.cpython-311.pyc
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1156 2024-02-14 15:19:49.000000 pygubu_designer-0.39/examples/forms/__pycache__/project_styles.cpython-311.pyc
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12310 2024-04-13 02:36:09.000000 pygubu_designer-0.39/examples/forms/demo1.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1635 2024-04-13 02:37:16.000000 pygubu_designer-0.39/examples/forms/formsdemo1app.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      796 2024-04-14 01:37:57.000000 pygubu_designer-0.39/examples/forms/formsdemo1appui.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      635 2024-02-25 22:14:08.000000 pygubu_designer-0.39/examples/forms/project_styles.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      723 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/framepad.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.811082 pygubu_designer-0.39/examples/helloworld/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       82 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/helloworld/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      740 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/helloworld/helloworld.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1178 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/helloworld/helloworld.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/helloworld/holamundo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1176 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/helloworld/holamundo.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/i18n_gettext_demo/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2303 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/i18n_gettext_demo/__pycache__/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1237 2024-02-13 03:45:58.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/__pycache__/i18n.cpython-311.pyc
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11576 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/demo-i18n.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/demoapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1251 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/i18n.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/i18n_gettext_demo/locale/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1433 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/locale/demoapp.pot
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.775082 pygubu_designer-0.39/examples/i18n_gettext_demo/locale/es/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1048 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/demoapp.mo
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/image_property/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/image_property/green.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      710 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/image_property/image_property.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1682 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/image_property/image_property.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3270 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/image_property/red.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3572 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/image_property/yellow.gif
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/integration_with_cxFreeze/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      337 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.815082 pygubu_designer-0.39/examples/integration_with_cxFreeze/imgs/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/imgs/MenuIcon4.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/imgs/ps_circle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/imgs/ps_cross.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/imgs/ps_square.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/imgs/ps_triangle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6612 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/myapp.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2529 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_cxFreeze/setup.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.819082 pygubu_designer-0.39/examples/integration_with_nuitka/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      366 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.819082 pygubu_designer-0.39/examples/integration_with_nuitka/imgs/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/imgs/MenuIcon4.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/imgs/ps_circle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/imgs/ps_cross.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/imgs/ps_square.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/imgs/ps_triangle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6510 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_nuitka/myapp.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.819082 pygubu_designer-0.39/examples/integration_with_py2exe/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      258 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.819082 pygubu_designer-0.39/examples/integration_with_py2exe/imgs/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/imgs/MenuIcon4.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/imgs/ps_circle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/imgs/ps_cross.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/imgs/ps_square.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/imgs/ps_triangle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6602 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/myapp.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2731 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_py2exe/setup.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_pyinstaller/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      291 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_pyinstaller/imgs/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/imgs/MenuIcon4.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/imgs/ps_circle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/imgs/ps_cross.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/imgs/ps_square.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/imgs/ps_triangle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6602 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2513 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/myapp.spec
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_pyinstaller/myapp.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_tkcalendar/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      582 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1141 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/main.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      526 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/requirements.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      317 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/tkcalendarwidgets.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1750 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/main.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      547 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/requirements.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      644 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2190 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/main.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/requirements.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1975 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.823082 pygubu_designer-0.39/examples/integration_with_zipapp/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      365 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.779082 pygubu_designer-0.39/examples/integration_with_zipapp/src/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/__init__.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3445 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/extradata/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/extradata/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      320 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/extradata/notes.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/green.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      556 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/info.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3270 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/red.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3572 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/yellow.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1013 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/main.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/jpg_image_on_canvas/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      825 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/jpg_image_on_canvas/demoapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1244 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/jpg_image_on_canvas/demoapp.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       14 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/jpg_image_on_canvas/requirements.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    38211 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/jpg_image_on_canvas/seaside400.jpg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3187 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/menubutton.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1347 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/menuexample.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/notebook/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5153 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/notebook/demo1.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1379 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/notebook/demo1app.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1835 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/panedwindow.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/panes_and_notebooks.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/pathchooserdemo/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       32 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/pathchooserdemo/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/pathchooserdemo/demo1/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1897 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/pathchooserdemo/demo1/pathchooserdemo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3220 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/pathchooserdemo/demo1/pathchooserdemo.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.827082 pygubu_designer-0.39/examples/pathchooserdemo/demo2/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2644 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/pathchooserdemo/demo2/pathchooserdemo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/pathchooserdemo/demo2/pathchooserdemo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1840 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/scrollbarhelper.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.831082 pygubu_designer-0.39/examples/scrolledframe/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/scrolledframe/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      646 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/scrolledframe/demoapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12412 2024-02-14 15:17:08.000000 pygubu_designer-0.39/examples/scrolledframe/scrolledframe_demo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10765 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/scrolledframe-layouts.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9388 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/scrolledframe.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.831082 pygubu_designer-0.39/examples/scrolledtext/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4030 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/scrolledtext/scrolledtext_demo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      977 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/scrolledtext/scrolledtextdemoapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.831082 pygubu_designer-0.39/examples/static_image/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      539 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/static_image/demoapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1676 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/static_image/demoapp.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    23336 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/static_image/logo_253.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/static_image/requirements.txt
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.779082 pygubu_designer-0.39/examples/text/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.831082 pygubu_designer-0.39/examples/text/logwindowdemo/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3075 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/text/logwindowdemo/demo1.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1714 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/text/logwindowdemo/demo1app.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.831082 pygubu_designer-0.39/examples/tk_window/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      144 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/tk_window/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/tk_window/green.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1354 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/tk_window/tkdemo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      600 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/tk_window/tkdemoapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.831082 pygubu_designer-0.39/examples/toplevel_centered/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      154 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_centered/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1216 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_centered/centered_demo1.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1317 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_centered/centered_demo2.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1020 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_centered/demo.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/toplevel_menu/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       64 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_menu/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1291 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_menu/menu.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2470 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/toplevel_menu/menu.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview/demo1/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       43 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/demo1/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1496 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/demo1/treeview.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3473 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/demo1/treeview.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview/demo2/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       64 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/demo2/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    23736 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/demo2/columns_stretching.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2712 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview/demo2/columnsstretchingdemo.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview_editable/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       28 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_editable/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview_editable/demo1/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5044 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_editable/demo1/demoapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7875 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_editable/demo1/demoapp.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview_editable/demo2/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5944 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_editable/demo2/demo2.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3432 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_editable/demo2/demo2app.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/treeview_filterable/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       30 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_filterable/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5404 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_filterable/demo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2886 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/treeview_filterable/demoapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/user_input/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/user_input/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/user_input/requirements.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    28967 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/user_input/userinput.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3730 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/user_input/userinputapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      883 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/variables.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4346 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/vscrolledframe.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.835082 pygubu_designer-0.39/examples/windowdeleteevent/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      887 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/windowdeleteevent/demo1.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1122 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/windowdeleteevent/demo1.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      847 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/windowdeleteevent/demo2.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1271 2023-09-09 20:40:32.000000 pygubu_designer-0.39/examples/windowdeleteevent/demo2.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    88292 2024-04-10 03:51:03.000000 pygubu_designer-0.39/pygubu-designer.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2434 2024-04-11 02:30:33.000000 pygubu_designer-0.39/pyproject.toml
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       38 2024-04-17 00:46:57.911082 pygubu_designer-0.39/setup.cfg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       61 2023-09-09 20:40:32.000000 pygubu_designer-0.39/setup.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.779082 pygubu_designer-0.39/src/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.907082 pygubu_designer-0.39/src/pygubu_designer.egg-info/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7697 2024-04-17 00:46:57.000000 pygubu_designer-0.39/src/pygubu_designer.egg-info/PKG-INFO
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    36901 2024-04-17 00:46:57.000000 pygubu_designer-0.39/src/pygubu_designer.egg-info/SOURCES.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        1 2024-04-17 00:46:57.000000 pygubu_designer-0.39/src/pygubu_designer.egg-info/dependency_links.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       65 2024-04-17 00:46:57.000000 pygubu_designer-0.39/src/pygubu_designer.egg-info/entry_points.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      443 2024-04-17 00:46:57.000000 pygubu_designer-0.39/src/pygubu_designer.egg-info/requires.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       15 2024-04-17 00:46:57.000000 pygubu_designer-0.39/src/pygubu_designer.egg-info/top_level.txt
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.839082 pygubu_designer-0.39/src/pygubudesigner/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      198 2024-04-11 02:29:26.000000 pygubu_designer-0.39/src/pygubudesigner/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      122 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/__main__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1049 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/actions.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6373 2024-03-12 19:01:57.000000 pygubu_designer-0.39/src/pygubudesigner/bindingseditor.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.839082 pygubu_designer-0.39/src/pygubudesigner/codegen/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       76 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/codegen/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    19333 2024-04-08 01:37:06.000000 pygubu_designer-0.39/src/pygubudesigner/codegen/codebuilder.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12276 2024-04-08 02:05:57.000000 pygubu_designer-0.39/src/pygubudesigner/codegen/scriptgenerator.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11044 2024-03-12 19:01:57.000000 pygubu_designer-0.39/src/pygubudesigner/containerlayouteditor.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.843082 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2992 2024-03-13 03:14:18.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/app.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2024-03-13 03:28:33.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/appuser.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      453 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/base.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1620 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/customstyles.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2116 2024-04-08 02:11:56.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/script.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      474 2024-04-12 03:50:58.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/scriptuser.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      771 2024-04-08 02:22:55.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/widget.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      542 2024-03-06 04:13:52.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/widgetbo.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      655 2024-04-12 03:59:49.000000 pygubu_designer-0.39/src/pygubudesigner/data/code_templates/widgetuser.py.mako
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/images/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.843082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       70 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/arrow-left2.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       71 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/arrow-right2.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       81 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/bin-16.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       85 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/cancel-circle-16.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       61 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/close.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       73 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/download3-16.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/download3-32.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      230 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/mglass.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      377 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/property_invalid.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      875 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/pygubu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4897 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/pygubu200.gif
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.859082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      107 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.Labelwidget.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      352 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.calendarframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      128 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.pathchooserinput.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      224 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      231 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.toplevelmenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.LabelFrame.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       75 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Message.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      327 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.OptionMenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1120 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      126 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Labelframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      100 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.Tab.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      327 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.OptionMenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Sizegrip.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      109 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.Column.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.871082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      132 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.Labelwidget.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.calendarframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.combobox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.dialog.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.editabletreeview.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.pathchooserinput.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      197 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrolledframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      197 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.toplevelmenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Button.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Calendar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      599 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Checkbutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Entry.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Frame.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Label.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      129 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.LabelFrame.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Listbox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menubutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      156 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Checkbutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Command.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      195 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Radiobutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Separator.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Submenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Message.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.OptionMenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.Pane.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Radiobutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scale.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scrollbar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      133 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Spinbox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      114 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Text.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Toplevel.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.default.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Button.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Checkbutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Combobox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Entry.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Frame.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Label.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.LabeledScale.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      129 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Labelframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Menubutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      142 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.Tab.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.OptionMenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.Pane.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Progressbar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Radiobutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scale.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scrollbar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Separator.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Sizegrip.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      133 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Spinbox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      156 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.Column.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.gif
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.871082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      592 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      567 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      357 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-strikethrough.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      572 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.871082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      194 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/arrow-left2.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      184 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/arrow-right2.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      162 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/bin-16.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      353 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/cancel-circle-16.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      334 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/circle-left.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      333 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/circle-right.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      170 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/download3-16.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      214 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/download3-32.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      316 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/mglass.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      603 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/property_invalid.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4777 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/pygubu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    15896 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/pygubu200.png
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.883082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      488 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.calendarframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      613 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      389 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.dialog.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.editabletreeview.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.pathchooserinput.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      480 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      509 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrolledframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      426 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      480 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      509 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      638 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      488 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Calendar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1088 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      524 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Entry.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      356 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Frame.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      706 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Listbox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menubutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      527 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      334 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Command.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      433 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Radiobutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      325 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Separator.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.OptionMenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.Pane.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      508 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Radiobutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scale.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      431 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scrollbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      426 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Text.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      389 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Toplevel.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      291 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.default.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      638 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      524 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      613 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Entry.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      356 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Frame.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      706 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.LabeledScale.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Menubutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      435 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Notebook.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.OptionMenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.Pane.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      545 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      508 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Radiobutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scale.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      431 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scrollbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      293 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Separator.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Treeview.png
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.891082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      161 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.calendarframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      263 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.combobox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      169 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.dialog.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.editabletreeview.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.pathchooserinput.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      186 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      339 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrolledframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      148 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      186 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      339 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.toplevelmenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      181 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Button.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      161 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Calendar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      689 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Checkbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Entry.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      143 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Frame.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      205 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Label.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Listbox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menubutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      202 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Checkbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Command.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      323 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Radiobutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Separator.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Submenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.OptionMenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.Pane.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Radiobutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scale.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scrollbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      206 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Spinbox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      148 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Text.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      169 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Toplevel.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      116 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.default.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      181 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Button.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Checkbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      263 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Combobox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Entry.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      143 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Frame.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      205 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Label.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.LabeledScale.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Menubutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      175 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Notebook.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.OptionMenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.Pane.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Progressbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Radiobutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scale.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scrollbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      107 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Separator.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      206 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Spinbox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Treeview.png
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      705 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      619 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      611 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      673 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/locale/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/locale/de/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/locale/de/LC_MESSAGES/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3172 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      425 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu.mo
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/locale/es/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/locale/es/LC_MESSAGES/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13114 2024-04-14 23:23:45.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      854 2024-04-14 23:23:45.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    58684 2024-04-14 23:23:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/pygubu-designer.pot
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    20171 2024-04-14 23:23:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/pygubu.pot
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/locale/tr/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/locale/tr/LC_MESSAGES/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4815 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      393 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu.mo
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_CN/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    53166 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10936 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.783082 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_Hans/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.895082 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    52658 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10937 2024-04-14 23:07:29.000000 pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.899082 pygubu_designer-0.39/src/pygubudesigner/data/ui/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13872 2024-04-09 23:44:02.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/about_dialog.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6320 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10318 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/container_layout_editor_base.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    16121 2024-04-09 23:44:02.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/designer_settings.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4093 2024-04-09 23:44:02.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/messagebox.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    45719 2024-04-12 04:11:16.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/project_settings.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    49126 2024-04-12 03:11:36.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/pygubu-ui.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6509 2024-04-09 23:44:02.000000 pygubu_designer-0.39/src/pygubudesigner/data/ui/treecomponent_palette.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4326 2024-04-15 03:30:30.000000 pygubu_designer-0.39/src/pygubudesigner/designerstyles.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2525 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/dialogs.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2122 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/i18n.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8476 2024-03-19 19:06:18.000000 pygubu_designer-0.39/src/pygubudesigner/layouteditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2688 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/logpanel.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    33479 2024-04-13 01:47:41.000000 pygubu_designer-0.39/src/pygubudesigner/main.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4418 2024-04-06 02:39:05.000000 pygubu_designer-0.39/src/pygubudesigner/preferences.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.899082 pygubu_designer-0.39/src/pygubudesigner/preview/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       63 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/preview/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2664 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/preview/builder.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13624 2024-04-02 02:28:06.000000 pygubu_designer-0.39/src/pygubudesigner/preview/helper.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    17119 2024-04-01 04:38:44.000000 pygubu_designer-0.39/src/pygubudesigner/preview/preview.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.899082 pygubu_designer-0.39/src/pygubudesigner/properties/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      373 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/properties/__init__.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.899082 pygubu_designer-0.39/src/pygubudesigner/properties/editors/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/properties/editors/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1027 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/properties/editors/forms.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1866 2024-02-17 03:46:34.000000 pygubu_designer-0.39/src/pygubudesigner/properties/manager.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    50538 2024-04-11 03:47:20.000000 pygubu_designer-0.39/src/pygubudesigner/properties/predefined.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    31209 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/properties/propertieshelp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5528 2024-04-14 01:38:41.000000 pygubu_designer-0.39/src/pygubudesigner/propertieseditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1915 2024-04-07 01:08:23.000000 pygubu_designer-0.39/src/pygubudesigner/rfilemanager.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.903082 pygubu_designer-0.39/src/pygubudesigner/services/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1854 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/aboutdialog.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      982 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/aboutdialogui.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.903082 pygubu_designer-0.39/src/pygubudesigner/services/builders/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/builders/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3356 2024-03-31 01:41:21.000000 pygubu_designer-0.39/src/pygubudesigner/services/designersettings.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      931 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/designersettingsui.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2733 2024-04-14 22:42:58.000000 pygubu_designer-0.39/src/pygubudesigner/services/fieldvalidator.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1945 2024-03-07 01:08:46.000000 pygubu_designer-0.39/src/pygubudesigner/services/messagebox.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      843 2024-03-07 01:11:22.000000 pygubu_designer-0.39/src/pygubudesigner/services/messageboxui.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4224 2024-04-13 02:03:46.000000 pygubu_designer-0.39/src/pygubudesigner/services/project.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12314 2024-04-14 23:23:05.000000 pygubu_designer-0.39/src/pygubudesigner/services/projectsettings.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1821 2024-04-12 04:13:44.000000 pygubu_designer-0.39/src/pygubudesigner/services/projectsettingsui.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6301 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/stylehandler.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4220 2024-03-31 23:43:45.000000 pygubu_designer-0.39/src/pygubudesigner/services/theming.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.903082 pygubu_designer-0.39/src/pygubudesigner/services/widgets/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/widgets/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5799 2024-04-08 02:37:37.000000 pygubu_designer-0.39/src/pygubudesigner/services/widgets/treecomponentpalette.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      450 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/services/widgets/treecomponentpalettebo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3465 2024-04-08 03:06:36.000000 pygubu_designer-0.39/src/pygubudesigner/services/widgets/treecomponentpaletteui.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    59265 2024-04-14 01:49:08.000000 pygubu_designer-0.39/src/pygubudesigner/uitreeeditor.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.903082 pygubu_designer-0.39/src/pygubudesigner/util/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2823 2024-04-01 01:31:03.000000 pygubu_designer-0.39/src/pygubudesigner/util/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4297 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/util/gridcalculator.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1964 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/util/keyboard.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1175 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/util/observable.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1289 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/util/screens.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2798 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/util/selecttool.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8344 2024-04-14 01:38:14.000000 pygubu_designer-0.39/src/pygubudesigner/widgetdescr.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.907082 pygubu_designer-0.39/src/pygubudesigner/widgets/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1048 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3063 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/bindingeditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3502 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/colorentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5327 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/commandentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3943 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/componentpalette.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5088 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/containerlayouteditorbase.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1640 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/cursorentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2681 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/dimensionentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2282 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/dynamicpropeditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5164 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/entryvalidatecommandeditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8250 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/fontentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10193 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/gridselector.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2491 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/imageentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3046 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/namedideditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2102 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/pixelcoordinateentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11940 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/propertyeditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3059 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/relativeentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5174 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/stickyentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3255 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/tkvarentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5936 2024-02-25 22:14:08.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/toolbarframe.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2650 2024-04-02 02:52:39.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/ttkstyleentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2536 2023-09-09 20:40:32.000000 pygubu_designer-0.39/src/pygubudesigner/widgets/whentry.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-17 00:46:57.907082 pygubu_designer-0.39/tests/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      562 2023-09-09 20:40:32.000000 pygubu_designer-0.39/tests/test_plugin_init.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.073326 pygubu_designer-0.39.1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       67 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/AUTHORS
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5128 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/LEEME.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    35064 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/LICENSE.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6509 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/LISEZMOI.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      248 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/MANIFEST.in
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7699 2024-04-22 01:14:39.069326 pygubu_designer-0.39.1/PKG-INFO
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5007 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.949327 pygubu_designer-0.39.1/development/
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     6434 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/create-imgs.py
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     6817 2024-03-17 20:08:13.000000 pygubu_designer-0.39.1/development/dev-notes.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2186 2024-04-08 04:51:29.000000 pygubu_designer-0.39.1/development/devtool.py
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     3885 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/devtool.sh
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.949327 pygubu_designer-0.39.1/development/gettext/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1037 2024-04-09 23:44:02.000000 pygubu_designer-0.39.1/development/gettext/pygubu.its
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2024-04-09 23:44:02.000000 pygubu_designer-0.39.1/development/gettext/pygubu.loc
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.949327 pygubu_designer-0.39.1/development/new-designer-icons/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2780 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/main.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.957327 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2129 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7010 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/button.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3744 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/canvas.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4072 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/canvas.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2101 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9271 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/combobox.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1252 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/default.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/default.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      665 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3834 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/entry.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1552 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6047 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/frame.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1142 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5074 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/label.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1666 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/labelframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6735 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/labelframe.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2133 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8598 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/menubutton.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      962 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/notebook-tab.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3043 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/notebook-tab.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1060 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/notebook.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3693 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/notebook.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      797 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3257 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      782 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/pannedwindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3238 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/pannedwindow.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1077 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/progressbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5356 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/progressbar.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/rect848.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1786 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/spinbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8481 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/spinbutton.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1126 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/textview.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6381 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/textview.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      867 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/toplevel.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3229 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/toplevel.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1068 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/treeview-col.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5481 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/treeview-col.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      935 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/treeview.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4893 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/treeview.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2489 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/viewport.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7036 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/viewport.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4315 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/template.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7552 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/testnewicons.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      854 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/new-designer-icons/testnewiconsapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.961326 pygubu_designer-0.39.1/development/pygubuLogo/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5501 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/pygubuLogo/Python-logo-notext.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   174121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/pygubuLogo/logo_pygubu .ico
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   101863 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/pygubuLogo/logo_pygubu.icns
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   174121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/pygubuLogo/logo_pygubu.ico
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   175900 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/pygubuLogo/logo_pygubu.xcf
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   124131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/pygubuLogo/pyGubu_newLogo.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       92 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/pygubuLogo/rootOfSVGs.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10232 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/pygubuLogo/tcl-tk.svg
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/pygubudesigner_.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       11 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/development/requirements.txt
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.965327 pygubu_designer-0.39.1/examples/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.965327 pygubu_designer-0.39.1/examples/7guis/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.965327 pygubu_designer-0.39.1/examples/7guis/01_counter/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1256 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/7guis/01_counter/counter.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      798 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/7guis/01_counter/counterapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.969327 pygubu_designer-0.39.1/examples/7guis/02_temperature_converter/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2687 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/7guis/02_temperature_converter/tempconv.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1648 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/7guis/02_temperature_converter/tempconvapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.969327 pygubu_designer-0.39.1/examples/7guis/03_flight_Booker/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2648 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/7guis/03_flight_Booker/flight_booker.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3212 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/7guis/03_flight_Booker/flightbookerapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.969327 pygubu_designer-0.39.1/examples/7guis/04_timer/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4089 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/7guis/04_timer/timer.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1777 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/7guis/04_timer/timerapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       81 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/7guis/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      347 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      546 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/binding.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      960 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/button_cb.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2053 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/button_cb.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.937327 pygubu_designer-0.39.1/examples/canvas/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.969327 pygubu_designer-0.39.1/examples/canvas/canvas-scrollregion/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      106 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/canvas/canvas-scrollregion/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5196 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/canvas/canvas-scrollregion/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5211 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/canvas/canvas-scrollregion/myapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      842 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/canvas_example.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.969327 pygubu_designer-0.39.1/examples/command_properties/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1221 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/command_properties/command_properties.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2641 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/command_properties/command_properties.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1256 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/command_properties/command_properties2.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3116 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/commands.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    18575 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/commands.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.969327 pygubu_designer-0.39.1/examples/control_variables/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      584 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/control_variables/controlvariables.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3634 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/control_variables/controlvariables.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.969327 pygubu_designer-0.39.1/examples/custom_widget/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      436 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/custom_widget/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1311 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/custom_widget/timer_main.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      515 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/custom_widget/timerapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      287 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/custom_widget/timerappwidgets.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2363 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/custom_widget/timewidget.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.973327 pygubu_designer-0.39.1/examples/customtkinter/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      174 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/customtkinter/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.973327 pygubu_designer-0.39.1/examples/customtkinter/complex/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    22578 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/customtkinter/complex/complex_demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2365 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/customtkinter/complex/complexdemoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.973327 pygubu_designer-0.39.1/examples/customtkinter/simple/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6284 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/customtkinter/simple/simple_demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1269 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/customtkinter/simple/simpledemoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.973327 pygubu_designer-0.39.1/examples/dialogs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       51 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.973327 pygubu_designer-0.39.1/examples/dialogs/demo1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       73 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo1/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1178 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo1/demo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5699 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo1/demo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.973327 pygubu_designer-0.39.1/examples/dialogs/demo2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       95 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo2/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1319 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo2/demo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4523 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo2/demo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.973327 pygubu_designer-0.39.1/examples/dialogs/demo3/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       98 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo3/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4883 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo3/demo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9704 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo3/demo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.973327 pygubu_designer-0.39.1/examples/dialogs/demo4/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      314 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo4/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.973327 pygubu_designer-0.39.1/examples/dialogs/demo4/__pycache__/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3373 2023-09-30 23:40:25.000000 pygubu_designer-0.39.1/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6987 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo4/settingsdemo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1002 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo4/settingsdemoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1319 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/dialogs/demo4/settingsdialog.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1471 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/example_grid_rc.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1631 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/example_grid_rc_2.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.973327 pygubu_designer-0.39.1/examples/forms/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.977326 pygubu_designer-0.39.1/examples/forms/__pycache__/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1939 2024-04-13 02:37:32.000000 pygubu_designer-0.39.1/examples/forms/__pycache__/formsdemo1appui.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2087 2024-02-04 03:08:22.000000 pygubu_designer-0.39.1/examples/forms/__pycache__/formsdemo1base.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1156 2024-02-14 15:19:49.000000 pygubu_designer-0.39.1/examples/forms/__pycache__/project_styles.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12310 2024-04-13 02:36:09.000000 pygubu_designer-0.39.1/examples/forms/demo1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1635 2024-04-13 02:37:16.000000 pygubu_designer-0.39.1/examples/forms/formsdemo1app.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      796 2024-04-14 01:37:57.000000 pygubu_designer-0.39.1/examples/forms/formsdemo1appui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      635 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/examples/forms/project_styles.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      723 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/framepad.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.977326 pygubu_designer-0.39.1/examples/helloworld/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       82 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/helloworld/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      740 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/helloworld/helloworld.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1178 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/helloworld/helloworld.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/helloworld/holamundo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1176 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/helloworld/holamundo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.977326 pygubu_designer-0.39.1/examples/i18n_gettext_demo/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2303 2024-02-14 15:17:08.000000 pygubu_designer-0.39.1/examples/i18n_gettext_demo/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.977326 pygubu_designer-0.39.1/examples/i18n_gettext_demo/__pycache__/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1237 2024-02-13 03:45:58.000000 pygubu_designer-0.39.1/examples/i18n_gettext_demo/__pycache__/i18n.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11576 2024-02-14 15:17:08.000000 pygubu_designer-0.39.1/examples/i18n_gettext_demo/demo-i18n.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2024-02-14 15:17:08.000000 pygubu_designer-0.39.1/examples/i18n_gettext_demo/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1251 2024-02-14 15:17:08.000000 pygubu_designer-0.39.1/examples/i18n_gettext_demo/i18n.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.977326 pygubu_designer-0.39.1/examples/i18n_gettext_demo/locale/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1433 2024-02-14 15:17:08.000000 pygubu_designer-0.39.1/examples/i18n_gettext_demo/locale/demoapp.pot
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.937327 pygubu_designer-0.39.1/examples/i18n_gettext_demo/locale/es/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.977326 pygubu_designer-0.39.1/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1048 2024-02-14 15:17:08.000000 pygubu_designer-0.39.1/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/demoapp.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.977326 pygubu_designer-0.39.1/examples/image_property/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/image_property/green.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      710 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/image_property/image_property.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1682 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/image_property/image_property.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3270 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/image_property/red.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3572 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/image_property/yellow.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.981326 pygubu_designer-0.39.1/examples/integration_with_cxFreeze/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      337 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_cxFreeze/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.981326 pygubu_designer-0.39.1/examples/integration_with_cxFreeze/imgs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_cxFreeze/imgs/MenuIcon4.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_cxFreeze/imgs/ps_circle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_cxFreeze/imgs/ps_cross.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_cxFreeze/imgs/ps_square.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_cxFreeze/imgs/ps_triangle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6612 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_cxFreeze/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_cxFreeze/myapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2529 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_cxFreeze/setup.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.981326 pygubu_designer-0.39.1/examples/integration_with_nuitka/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      366 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_nuitka/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.981326 pygubu_designer-0.39.1/examples/integration_with_nuitka/imgs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_nuitka/imgs/MenuIcon4.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_nuitka/imgs/ps_circle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_nuitka/imgs/ps_cross.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_nuitka/imgs/ps_square.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_nuitka/imgs/ps_triangle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6510 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_nuitka/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_nuitka/myapp.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.981326 pygubu_designer-0.39.1/examples/integration_with_py2exe/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      258 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_py2exe/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.985326 pygubu_designer-0.39.1/examples/integration_with_py2exe/imgs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_py2exe/imgs/MenuIcon4.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_py2exe/imgs/ps_circle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_py2exe/imgs/ps_cross.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_py2exe/imgs/ps_square.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_py2exe/imgs/ps_triangle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6602 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_py2exe/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_py2exe/myapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2731 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_py2exe/setup.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.985326 pygubu_designer-0.39.1/examples/integration_with_pyinstaller/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      291 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_pyinstaller/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.985326 pygubu_designer-0.39.1/examples/integration_with_pyinstaller/imgs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_pyinstaller/imgs/MenuIcon4.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_pyinstaller/imgs/ps_circle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_pyinstaller/imgs/ps_cross.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_pyinstaller/imgs/ps_square.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_pyinstaller/imgs/ps_triangle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6602 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_pyinstaller/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2513 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_pyinstaller/myapp.spec
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_pyinstaller/myapp.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.985326 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      582 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.985326 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1141 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp1/main.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      526 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp1/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp1/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      317 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp1/tkcalendarwidgets.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.985326 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1750 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp2/main.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      547 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp2/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp2/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      644 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.989327 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp3/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2190 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp3/main.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp3/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp3/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1975 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.989327 pygubu_designer-0.39.1/examples/integration_with_zipapp/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      365 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_zipapp/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.937327 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.989327 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/__init__.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.989327 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3445 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.989327 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/extradata/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/extradata/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      320 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/extradata/notes.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/green.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      556 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/info.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3270 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/red.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3572 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/yellow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1013 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/main.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.989327 pygubu_designer-0.39.1/examples/jpg_image_on_canvas/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      825 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/jpg_image_on_canvas/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1244 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/jpg_image_on_canvas/demoapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       14 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/jpg_image_on_canvas/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    38211 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/jpg_image_on_canvas/seaside400.jpg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3187 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/menubutton.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1347 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/menuexample.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.989327 pygubu_designer-0.39.1/examples/notebook/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5153 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/notebook/demo1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1379 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/notebook/demo1app.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1835 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/panedwindow.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/panes_and_notebooks.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.989327 pygubu_designer-0.39.1/examples/pathchooserdemo/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       32 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/pathchooserdemo/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.989327 pygubu_designer-0.39.1/examples/pathchooserdemo/demo1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1897 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/pathchooserdemo/demo1/pathchooserdemo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3220 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/pathchooserdemo/demo1/pathchooserdemo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.989327 pygubu_designer-0.39.1/examples/pathchooserdemo/demo2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2644 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/pathchooserdemo/demo2/pathchooserdemo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/pathchooserdemo/demo2/pathchooserdemo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1840 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/scrollbarhelper.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.993327 pygubu_designer-0.39.1/examples/scrolledframe/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2024-02-14 15:17:08.000000 pygubu_designer-0.39.1/examples/scrolledframe/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      646 2024-02-14 15:17:08.000000 pygubu_designer-0.39.1/examples/scrolledframe/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12412 2024-02-14 15:17:08.000000 pygubu_designer-0.39.1/examples/scrolledframe/scrolledframe_demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10765 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/scrolledframe-layouts.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9388 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/scrolledframe.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.993327 pygubu_designer-0.39.1/examples/scrolledtext/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4030 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/scrolledtext/scrolledtext_demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      977 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/scrolledtext/scrolledtextdemoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.993327 pygubu_designer-0.39.1/examples/static_image/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      539 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/static_image/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1676 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/static_image/demoapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    23336 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/static_image/logo_253.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/static_image/requirements.txt
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.941327 pygubu_designer-0.39.1/examples/text/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.993327 pygubu_designer-0.39.1/examples/text/logwindowdemo/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3075 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/text/logwindowdemo/demo1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1714 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/text/logwindowdemo/demo1app.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.993327 pygubu_designer-0.39.1/examples/tk_window/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      144 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/tk_window/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/tk_window/green.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1354 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/tk_window/tkdemo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      600 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/tk_window/tkdemoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.993327 pygubu_designer-0.39.1/examples/toplevel_centered/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      154 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/toplevel_centered/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1216 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/toplevel_centered/centered_demo1.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1317 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/toplevel_centered/centered_demo2.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1020 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/toplevel_centered/demo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.993327 pygubu_designer-0.39.1/examples/toplevel_menu/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       64 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/toplevel_menu/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1291 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/toplevel_menu/menu.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2470 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/toplevel_menu/menu.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.993327 pygubu_designer-0.39.1/examples/treeview/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.997326 pygubu_designer-0.39.1/examples/treeview/demo1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       43 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview/demo1/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1496 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview/demo1/treeview.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3473 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview/demo1/treeview.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.997326 pygubu_designer-0.39.1/examples/treeview/demo2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       64 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview/demo2/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    23736 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview/demo2/columns_stretching.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2712 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview/demo2/columnsstretchingdemo.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.997326 pygubu_designer-0.39.1/examples/treeview_editable/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       28 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview_editable/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.997326 pygubu_designer-0.39.1/examples/treeview_editable/demo1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5044 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview_editable/demo1/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7875 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview_editable/demo1/demoapp.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.997326 pygubu_designer-0.39.1/examples/treeview_editable/demo2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5944 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview_editable/demo2/demo2.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3432 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview_editable/demo2/demo2app.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.997326 pygubu_designer-0.39.1/examples/treeview_filterable/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       30 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview_filterable/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5404 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview_filterable/demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2886 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/treeview_filterable/demoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.997326 pygubu_designer-0.39.1/examples/user_input/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/user_input/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/user_input/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    28967 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/user_input/userinput.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3730 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/user_input/userinputapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      883 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/variables.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4346 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/vscrolledframe.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.997326 pygubu_designer-0.39.1/examples/windowdeleteevent/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      887 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/windowdeleteevent/demo1.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1122 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/windowdeleteevent/demo1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      847 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/windowdeleteevent/demo2.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1271 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/examples/windowdeleteevent/demo2.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    88292 2024-04-10 03:51:03.000000 pygubu_designer-0.39.1/pygubu-designer.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2434 2024-04-11 02:30:33.000000 pygubu_designer-0.39.1/pyproject.toml
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       38 2024-04-22 01:14:39.073326 pygubu_designer-0.39.1/setup.cfg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       61 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/setup.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.941327 pygubu_designer-0.39.1/src/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.069326 pygubu_designer-0.39.1/src/pygubu_designer.egg-info/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7699 2024-04-22 01:14:38.000000 pygubu_designer-0.39.1/src/pygubu_designer.egg-info/PKG-INFO
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    36901 2024-04-22 01:14:38.000000 pygubu_designer-0.39.1/src/pygubu_designer.egg-info/SOURCES.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        1 2024-04-22 01:14:38.000000 pygubu_designer-0.39.1/src/pygubu_designer.egg-info/dependency_links.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       65 2024-04-22 01:14:38.000000 pygubu_designer-0.39.1/src/pygubu_designer.egg-info/entry_points.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      443 2024-04-22 01:14:38.000000 pygubu_designer-0.39.1/src/pygubu_designer.egg-info/requires.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       15 2024-04-22 01:14:38.000000 pygubu_designer-0.39.1/src/pygubu_designer.egg-info/top_level.txt
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.001326 pygubu_designer-0.39.1/src/pygubudesigner/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      200 2024-04-22 01:11:40.000000 pygubu_designer-0.39.1/src/pygubudesigner/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      122 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/__main__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1049 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/actions.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6373 2024-03-12 19:01:57.000000 pygubu_designer-0.39.1/src/pygubudesigner/bindingseditor.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.005326 pygubu_designer-0.39.1/src/pygubudesigner/codegen/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       76 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/codegen/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    19333 2024-04-08 01:37:06.000000 pygubu_designer-0.39.1/src/pygubudesigner/codegen/codebuilder.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12276 2024-04-08 02:05:57.000000 pygubu_designer-0.39.1/src/pygubudesigner/codegen/scriptgenerator.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11044 2024-03-12 19:01:57.000000 pygubu_designer-0.39.1/src/pygubudesigner/containerlayouteditor.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.945327 pygubu_designer-0.39.1/src/pygubudesigner/data/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.005326 pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2992 2024-03-13 03:14:18.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/app.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2024-03-13 03:28:33.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/appuser.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      453 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/base.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1620 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/customstyles.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2116 2024-04-08 02:11:56.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/script.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      474 2024-04-12 03:50:58.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/scriptuser.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      771 2024-04-08 02:22:55.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/widget.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      542 2024-03-06 04:13:52.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/widgetbo.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      655 2024-04-12 03:59:49.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/widgetuser.py.mako
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.941327 pygubu_designer-0.39.1/src/pygubudesigner/data/images/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.005326 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       70 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/arrow-left2.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       71 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/arrow-right2.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       81 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/bin-16.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       85 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/cancel-circle-16.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       61 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/close.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       73 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/download3-16.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/download3-32.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      230 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/mglass.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/property_invalid.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      875 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/pygubu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4897 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/pygubu200.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.941327 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.017326 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      107 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.Labelwidget.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      352 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.calendarframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      128 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.pathchooserinput.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      224 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      231 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.toplevelmenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.LabelFrame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       75 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Message.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      327 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.OptionMenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1120 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      126 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Labelframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      100 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.Tab.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      327 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.OptionMenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Sizegrip.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      109 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.Column.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.029326 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      132 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.Labelwidget.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.calendarframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.combobox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.dialog.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.editabletreeview.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.pathchooserinput.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      197 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrolledframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      197 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.toplevelmenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Button.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Calendar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      599 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Entry.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Frame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Label.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      129 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.LabelFrame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Listbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menubutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      156 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Command.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      195 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Separator.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Submenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Message.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.OptionMenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.Pane.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scrollbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      133 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Spinbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      114 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Text.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Toplevel.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.default.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Button.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Combobox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Entry.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Frame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Label.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.LabeledScale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      129 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Labelframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Menubutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      142 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.Tab.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.OptionMenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.Pane.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Progressbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scrollbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Separator.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Sizegrip.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      133 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Spinbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      156 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.Column.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.029326 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/fontentry/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      592 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      567 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      357 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-strikethrough.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      572 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.029326 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      194 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/arrow-left2.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      184 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/arrow-right2.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      162 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/bin-16.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      353 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/cancel-circle-16.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      334 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/circle-left.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      333 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/circle-right.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      170 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/download3-16.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      214 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/download3-32.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      316 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/mglass.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      603 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/property_invalid.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4777 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/pygubu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    15896 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/pygubu200.png
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.941327 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.041326 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      488 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.calendarframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      613 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      389 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.dialog.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.editabletreeview.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.pathchooserinput.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      480 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      509 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrolledframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      426 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      480 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      509 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      638 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      488 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Calendar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1088 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      524 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      356 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      706 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Listbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      527 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      334 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Command.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      433 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      325 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Separator.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.OptionMenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.Pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      508 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      431 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scrollbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      426 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Text.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      389 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Toplevel.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      291 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.default.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      638 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      524 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      613 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      356 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      706 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.LabeledScale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      435 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Notebook.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.OptionMenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.Pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      545 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      508 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      431 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scrollbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      293 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Separator.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Treeview.png
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.053326 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      161 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.calendarframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      263 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      169 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.dialog.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.editabletreeview.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.pathchooserinput.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      186 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      339 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrolledframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      148 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      186 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      339 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.toplevelmenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      181 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      161 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Calendar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      689 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      143 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      205 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Listbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      202 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Command.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      323 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Separator.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Submenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.OptionMenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.Pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scrollbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      206 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Spinbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      148 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Text.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      169 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Toplevel.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      116 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.default.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      181 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      263 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      143 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      205 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.LabeledScale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      175 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Notebook.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.OptionMenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.Pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Progressbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scrollbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      107 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Separator.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      206 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Spinbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Treeview.png
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.053326 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/fontentry/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      705 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      619 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      611 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      673 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.053326 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.941327 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/de/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.053326 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/de/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3172 2024-04-22 01:08:18.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      425 2024-04-22 01:08:18.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.941327 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/es/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.057326 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/es/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13309 2024-04-22 01:09:43.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      854 2024-04-22 01:08:18.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    58879 2024-04-22 00:44:13.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/pygubu-designer.pot
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    20171 2024-04-22 00:44:13.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/pygubu.pot
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.945327 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/tr/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.057326 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4815 2024-04-22 01:08:18.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      393 2024-04-22 01:08:18.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.945327 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/zh_CN/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.057326 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    53166 2024-04-22 01:08:18.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10936 2024-04-22 01:08:18.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:38.945327 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/zh_Hans/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.057326 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    52658 2024-04-22 01:08:18.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10937 2024-04-22 01:08:18.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.057326 pygubu_designer-0.39.1/src/pygubudesigner/data/ui/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13872 2024-04-09 23:44:02.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/ui/about_dialog.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6320 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10318 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/ui/container_layout_editor_base.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    16121 2024-04-09 23:44:02.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/ui/designer_settings.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4093 2024-04-09 23:44:02.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/ui/messagebox.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    45719 2024-04-12 04:11:16.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/ui/project_settings.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    49541 2024-04-20 01:39:30.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/ui/pygubu-ui.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6509 2024-04-09 23:44:02.000000 pygubu_designer-0.39.1/src/pygubudesigner/data/ui/treecomponent_palette.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4326 2024-04-15 03:30:30.000000 pygubu_designer-0.39.1/src/pygubudesigner/designerstyles.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2525 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/dialogs.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2122 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/i18n.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8476 2024-03-19 19:06:18.000000 pygubu_designer-0.39.1/src/pygubudesigner/layouteditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2688 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/logpanel.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    34307 2024-04-20 01:39:30.000000 pygubu_designer-0.39.1/src/pygubudesigner/main.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4418 2024-04-06 02:39:05.000000 pygubu_designer-0.39.1/src/pygubudesigner/preferences.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.057326 pygubu_designer-0.39.1/src/pygubudesigner/preview/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       63 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/preview/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2664 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/preview/builder.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13624 2024-04-02 02:28:06.000000 pygubu_designer-0.39.1/src/pygubudesigner/preview/helper.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    17119 2024-04-01 04:38:44.000000 pygubu_designer-0.39.1/src/pygubudesigner/preview/preview.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.061326 pygubu_designer-0.39.1/src/pygubudesigner/properties/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      373 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/properties/__init__.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.061326 pygubu_designer-0.39.1/src/pygubudesigner/properties/editors/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/properties/editors/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1027 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/properties/editors/forms.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1866 2024-02-17 03:46:34.000000 pygubu_designer-0.39.1/src/pygubudesigner/properties/manager.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    50538 2024-04-11 03:47:20.000000 pygubu_designer-0.39.1/src/pygubudesigner/properties/predefined.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    31209 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/properties/propertieshelp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5528 2024-04-14 01:38:41.000000 pygubu_designer-0.39.1/src/pygubudesigner/propertieseditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1915 2024-04-07 01:08:23.000000 pygubu_designer-0.39.1/src/pygubudesigner/rfilemanager.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.061326 pygubu_designer-0.39.1/src/pygubudesigner/services/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1854 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/aboutdialog.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      982 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/aboutdialogui.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.061326 pygubu_designer-0.39.1/src/pygubudesigner/services/builders/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/builders/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3356 2024-03-31 01:41:21.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/designersettings.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      931 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/designersettingsui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2733 2024-04-14 22:42:58.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/fieldvalidator.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1945 2024-03-07 01:08:46.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/messagebox.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      843 2024-03-07 01:11:22.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/messageboxui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4224 2024-04-13 02:03:46.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/project.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12314 2024-04-14 23:23:05.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/projectsettings.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1821 2024-04-12 04:13:44.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/projectsettingsui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6301 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/stylehandler.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4220 2024-03-31 23:43:45.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/theming.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.065326 pygubu_designer-0.39.1/src/pygubudesigner/services/widgets/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/widgets/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5799 2024-04-08 02:37:37.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/widgets/treecomponentpalette.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      450 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/widgets/treecomponentpalettebo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3465 2024-04-08 03:06:36.000000 pygubu_designer-0.39.1/src/pygubudesigner/services/widgets/treecomponentpaletteui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    59265 2024-04-14 01:49:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/uitreeeditor.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.065326 pygubu_designer-0.39.1/src/pygubudesigner/util/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2823 2024-04-01 01:31:03.000000 pygubu_designer-0.39.1/src/pygubudesigner/util/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4297 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/util/gridcalculator.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1964 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/util/keyboard.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1175 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/util/observable.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1289 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/util/screens.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2798 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/util/selecttool.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8344 2024-04-14 01:38:14.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgetdescr.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.069326 pygubu_designer-0.39.1/src/pygubudesigner/widgets/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1048 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3063 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/bindingeditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3502 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/colorentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5327 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/commandentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3943 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/componentpalette.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5088 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/containerlayouteditorbase.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1640 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/cursorentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2681 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/dimensionentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2282 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/dynamicpropeditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5164 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/entryvalidatecommandeditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8250 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/fontentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10193 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/gridselector.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2491 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/imageentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3046 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/namedideditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2102 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/pixelcoordinateentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11940 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/propertyeditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3059 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/relativeentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5174 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/stickyentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3255 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/tkvarentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5936 2024-02-25 22:14:08.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/toolbarframe.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2650 2024-04-02 02:52:39.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/ttkstyleentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2536 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/src/pygubudesigner/widgets/whentry.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-04-22 01:14:39.069326 pygubu_designer-0.39.1/tests/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      562 2023-09-09 20:40:32.000000 pygubu_designer-0.39.1/tests/test_plugin_init.py
```

### Comparing `pygubu_designer-0.39/LEEME.md` & `pygubu_designer-0.39.1/LEEME.md`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/LICENSE.md` & `pygubu_designer-0.39.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/LISEZMOI.md` & `pygubu_designer-0.39.1/LISEZMOI.md`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/PKG-INFO` & `pygubu_designer-0.39.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygubu-designer
-Version: 0.39
+Version: 0.39.1
 Summary: A simple GUI designer for the python tkinter module
 Author-email: Alejandro Autalan <alejandroautalan@gmail.com>
 License: GPL-3
 Project-URL: Documentation, https://github.com/alejandroautalan/pygubu-designer#readme
 Project-URL: Issues, https://github.com/alejandroautalan/pygubu-designer/issues
 Project-URL: Source, https://github.com/alejandroautalan/pygubu-designer
 Keywords: gui,tkinter,designer
```

### Comparing `pygubu_designer-0.39/README.md` & `pygubu_designer-0.39.1/README.md`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/create-imgs.py` & `pygubu_designer-0.39.1/development/create-imgs.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/dev-notes.txt` & `pygubu_designer-0.39.1/development/dev-notes.txt`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/devtool.py` & `pygubu_designer-0.39.1/development/devtool.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/devtool.sh` & `pygubu_designer-0.39.1/development/devtool.sh`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/gettext/pygubu.its` & `pygubu_designer-0.39.1/development/gettext/pygubu.its`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/main.py` & `pygubu_designer-0.39.1/development/new-designer-icons/main.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/button.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/button.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/button.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/button.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/canvas.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/canvas.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/canvas.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/canvas.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/combobox.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/combobox.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/combobox.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/combobox.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/default.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/default.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/default.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/default.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/entry.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/entry.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/entry.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/entry.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/frame.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/frame.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/frame.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/frame.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/label.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/label.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/label.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/label.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/labelframe.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/labelframe.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/labelframe.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/labelframe.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/menubutton.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/menubutton.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/menubutton.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/menubutton.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook-tab.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/notebook-tab.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook-tab.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/notebook-tab.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/notebook.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/notebook.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/notebook.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/pannedwindow.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/pannedwindow.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/pannedwindow.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/progressbar.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/progressbar.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/progressbar.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/progressbar.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/spinbutton.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/spinbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/spinbutton.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/spinbutton.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/textview.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/textview.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/textview.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/textview.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/toplevel.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/toplevel.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/toplevel.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/toplevel.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview-col.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/treeview-col.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview-col.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/treeview-col.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/treeview.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/treeview.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/treeview.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/viewport.png` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/viewport.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/pygubu-icons/viewport.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/pygubu-icons/viewport.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/template.svg` & `pygubu_designer-0.39.1/development/new-designer-icons/template.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/testnewicons.ui` & `pygubu_designer-0.39.1/development/new-designer-icons/testnewicons.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/new-designer-icons/testnewiconsapp.py` & `pygubu_designer-0.39.1/development/new-designer-icons/testnewiconsapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/pygubuLogo/Python-logo-notext.svg` & `pygubu_designer-0.39.1/development/pygubuLogo/Python-logo-notext.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/pygubuLogo/logo_pygubu .ico` & `pygubu_designer-0.39.1/development/pygubuLogo/logo_pygubu .ico`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/pygubuLogo/logo_pygubu.icns` & `pygubu_designer-0.39.1/development/pygubuLogo/logo_pygubu.icns`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/pygubuLogo/logo_pygubu.ico` & `pygubu_designer-0.39.1/development/pygubuLogo/logo_pygubu.ico`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/pygubuLogo/logo_pygubu.xcf` & `pygubu_designer-0.39.1/development/pygubuLogo/logo_pygubu.xcf`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/pygubuLogo/pyGubu_newLogo.svg` & `pygubu_designer-0.39.1/development/pygubuLogo/pyGubu_newLogo.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/pygubuLogo/tcl-tk.svg` & `pygubu_designer-0.39.1/development/pygubuLogo/tcl-tk.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/development/pygubudesigner_.py` & `pygubu_designer-0.39.1/development/pygubudesigner_.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/7guis/01_counter/counter.ui` & `pygubu_designer-0.39.1/examples/7guis/01_counter/counter.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/7guis/01_counter/counterapp.py` & `pygubu_designer-0.39.1/examples/7guis/01_counter/counterapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/7guis/02_temperature_converter/tempconv.ui` & `pygubu_designer-0.39.1/examples/7guis/02_temperature_converter/tempconv.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/7guis/02_temperature_converter/tempconvapp.py` & `pygubu_designer-0.39.1/examples/7guis/02_temperature_converter/tempconvapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/7guis/03_flight_Booker/flight_booker.ui` & `pygubu_designer-0.39.1/examples/7guis/03_flight_Booker/flight_booker.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/7guis/03_flight_Booker/flightbookerapp.py` & `pygubu_designer-0.39.1/examples/7guis/03_flight_Booker/flightbookerapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/7guis/04_timer/timer.ui` & `pygubu_designer-0.39.1/examples/7guis/04_timer/timer.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/7guis/04_timer/timerapp.py` & `pygubu_designer-0.39.1/examples/7guis/04_timer/timerapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/binding.ui` & `pygubu_designer-0.39.1/examples/binding.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/button_cb.py` & `pygubu_designer-0.39.1/examples/button_cb.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/button_cb.ui` & `pygubu_designer-0.39.1/examples/button_cb.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/canvas/canvas-scrollregion/myapp.py` & `pygubu_designer-0.39.1/examples/canvas/canvas-scrollregion/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/canvas/canvas-scrollregion/myapp.ui` & `pygubu_designer-0.39.1/examples/canvas/canvas-scrollregion/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/canvas_example.ui` & `pygubu_designer-0.39.1/examples/canvas_example.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/command_properties/command_properties.py` & `pygubu_designer-0.39.1/examples/command_properties/command_properties.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/command_properties/command_properties.ui` & `pygubu_designer-0.39.1/examples/command_properties/command_properties.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/command_properties/command_properties2.py` & `pygubu_designer-0.39.1/examples/command_properties/command_properties2.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/commands.py` & `pygubu_designer-0.39.1/examples/commands.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/commands.ui` & `pygubu_designer-0.39.1/examples/commands.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/control_variables/controlvariables.py` & `pygubu_designer-0.39.1/examples/control_variables/controlvariables.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/control_variables/controlvariables.ui` & `pygubu_designer-0.39.1/examples/control_variables/controlvariables.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/custom_widget/timer_main.ui` & `pygubu_designer-0.39.1/examples/custom_widget/timer_main.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/custom_widget/timerapp.py` & `pygubu_designer-0.39.1/examples/custom_widget/timerapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/custom_widget/timewidget.py` & `pygubu_designer-0.39.1/examples/custom_widget/timewidget.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/customtkinter/complex/complex_demo.ui` & `pygubu_designer-0.39.1/examples/customtkinter/complex/complex_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/customtkinter/complex/complexdemoapp.py` & `pygubu_designer-0.39.1/examples/customtkinter/complex/complexdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/customtkinter/simple/simple_demo.ui` & `pygubu_designer-0.39.1/examples/customtkinter/simple/simple_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/customtkinter/simple/simpledemoapp.py` & `pygubu_designer-0.39.1/examples/customtkinter/simple/simpledemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/dialogs/demo1/demo.py` & `pygubu_designer-0.39.1/examples/dialogs/demo1/demo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/dialogs/demo1/demo.ui` & `pygubu_designer-0.39.1/examples/dialogs/demo1/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/dialogs/demo2/demo.py` & `pygubu_designer-0.39.1/examples/dialogs/demo2/demo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/dialogs/demo2/demo.ui` & `pygubu_designer-0.39.1/examples/dialogs/demo2/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/dialogs/demo3/demo.py` & `pygubu_designer-0.39.1/examples/dialogs/demo3/demo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/dialogs/demo3/demo.ui` & `pygubu_designer-0.39.1/examples/dialogs/demo3/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-311.pyc` & `pygubu_designer-0.39.1/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/dialogs/demo4/settingsdemo.ui` & `pygubu_designer-0.39.1/examples/dialogs/demo4/settingsdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/dialogs/demo4/settingsdemoapp.py` & `pygubu_designer-0.39.1/examples/dialogs/demo4/settingsdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/dialogs/demo4/settingsdialog.py` & `pygubu_designer-0.39.1/examples/dialogs/demo4/settingsdialog.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/example_grid_rc.ui` & `pygubu_designer-0.39.1/examples/example_grid_rc.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/example_grid_rc_2.ui` & `pygubu_designer-0.39.1/examples/example_grid_rc_2.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/forms/__pycache__/formsdemo1appui.cpython-311.pyc` & `pygubu_designer-0.39.1/examples/forms/__pycache__/formsdemo1appui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/forms/__pycache__/formsdemo1base.cpython-311.pyc` & `pygubu_designer-0.39.1/examples/forms/__pycache__/formsdemo1base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/forms/__pycache__/project_styles.cpython-311.pyc` & `pygubu_designer-0.39.1/examples/forms/__pycache__/project_styles.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/forms/demo1.ui` & `pygubu_designer-0.39.1/examples/forms/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/forms/formsdemo1app.py` & `pygubu_designer-0.39.1/examples/forms/formsdemo1app.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/forms/formsdemo1appui.py` & `pygubu_designer-0.39.1/examples/forms/formsdemo1appui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/forms/project_styles.py` & `pygubu_designer-0.39.1/examples/forms/project_styles.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/framepad.ui` & `pygubu_designer-0.39.1/examples/framepad.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/helloworld/helloworld.py` & `pygubu_designer-0.39.1/examples/helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/helloworld/helloworld.ui` & `pygubu_designer-0.39.1/examples/helloworld/helloworld.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/helloworld/holamundo.py` & `pygubu_designer-0.39.1/examples/helloworld/holamundo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/helloworld/holamundo.ui` & `pygubu_designer-0.39.1/examples/helloworld/holamundo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/i18n_gettext_demo/README.md` & `pygubu_designer-0.39.1/examples/i18n_gettext_demo/README.md`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/i18n_gettext_demo/__pycache__/i18n.cpython-311.pyc` & `pygubu_designer-0.39.1/examples/i18n_gettext_demo/__pycache__/i18n.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/i18n_gettext_demo/demo-i18n.ui` & `pygubu_designer-0.39.1/examples/i18n_gettext_demo/demo-i18n.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/i18n_gettext_demo/demoapp.py` & `pygubu_designer-0.39.1/examples/i18n_gettext_demo/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/i18n_gettext_demo/i18n.py` & `pygubu_designer-0.39.1/examples/i18n_gettext_demo/i18n.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/i18n_gettext_demo/locale/demoapp.pot` & `pygubu_designer-0.39.1/examples/i18n_gettext_demo/locale/demoapp.pot`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/demoapp.mo` & `pygubu_designer-0.39.1/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/demoapp.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/image_property/green.gif` & `pygubu_designer-0.39.1/examples/image_property/green.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/image_property/image_property.py` & `pygubu_designer-0.39.1/examples/image_property/image_property.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/image_property/image_property.ui` & `pygubu_designer-0.39.1/examples/image_property/image_property.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/image_property/red.gif` & `pygubu_designer-0.39.1/examples/image_property/red.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/image_property/yellow.gif` & `pygubu_designer-0.39.1/examples/image_property/yellow.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_cxFreeze/myapp.py` & `pygubu_designer-0.39.1/examples/integration_with_cxFreeze/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_cxFreeze/myapp.ui` & `pygubu_designer-0.39.1/examples/integration_with_cxFreeze/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_cxFreeze/setup.py` & `pygubu_designer-0.39.1/examples/integration_with_cxFreeze/setup.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_nuitka/myapp.py` & `pygubu_designer-0.39.1/examples/integration_with_nuitka/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_nuitka/myapp.ui` & `pygubu_designer-0.39.1/examples/integration_with_nuitka/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_py2exe/myapp.py` & `pygubu_designer-0.39.1/examples/integration_with_py2exe/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_py2exe/myapp.ui` & `pygubu_designer-0.39.1/examples/integration_with_py2exe/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_py2exe/setup.py` & `pygubu_designer-0.39.1/examples/integration_with_py2exe/setup.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_pyinstaller/myapp.py` & `pygubu_designer-0.39.1/examples/integration_with_pyinstaller/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_pyinstaller/myapp.spec` & `pygubu_designer-0.39.1/examples/integration_with_pyinstaller/myapp.spec`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_pyinstaller/myapp.ui` & `pygubu_designer-0.39.1/examples/integration_with_pyinstaller/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_tkcalendar/README.md` & `pygubu_designer-0.39.1/examples/integration_with_tkcalendar/README.md`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/main.ui` & `pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp1/main.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp1/myapp.py` & `pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp1/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/main.ui` & `pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp2/main.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/myapp.py` & `pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp2/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py` & `pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/main.ui` & `pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp3/main.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/myapp.py` & `pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp3/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py` & `pygubu_designer-0.39.1/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui` & `pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/green.gif` & `pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/green.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/info.txt` & `pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/info.txt`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/red.gif` & `pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/red.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/data/yellow.gif` & `pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/data/yellow.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/integration_with_zipapp/src/demoapp/main.py` & `pygubu_designer-0.39.1/examples/integration_with_zipapp/src/demoapp/main.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/jpg_image_on_canvas/demoapp.py` & `pygubu_designer-0.39.1/examples/jpg_image_on_canvas/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/jpg_image_on_canvas/demoapp.ui` & `pygubu_designer-0.39.1/examples/jpg_image_on_canvas/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/jpg_image_on_canvas/seaside400.jpg` & `pygubu_designer-0.39.1/examples/jpg_image_on_canvas/seaside400.jpg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/menubutton.ui` & `pygubu_designer-0.39.1/examples/menubutton.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/menuexample.ui` & `pygubu_designer-0.39.1/examples/menuexample.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/notebook/demo1.ui` & `pygubu_designer-0.39.1/examples/notebook/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/notebook/demo1app.py` & `pygubu_designer-0.39.1/examples/notebook/demo1app.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/panedwindow.ui` & `pygubu_designer-0.39.1/examples/panedwindow.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/panes_and_notebooks.ui` & `pygubu_designer-0.39.1/examples/panes_and_notebooks.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/pathchooserdemo/demo1/pathchooserdemo.py` & `pygubu_designer-0.39.1/examples/pathchooserdemo/demo1/pathchooserdemo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/pathchooserdemo/demo1/pathchooserdemo.ui` & `pygubu_designer-0.39.1/examples/pathchooserdemo/demo1/pathchooserdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/pathchooserdemo/demo2/pathchooserdemo.py` & `pygubu_designer-0.39.1/examples/pathchooserdemo/demo2/pathchooserdemo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/pathchooserdemo/demo2/pathchooserdemo.ui` & `pygubu_designer-0.39.1/examples/pathchooserdemo/demo2/pathchooserdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/scrollbarhelper.ui` & `pygubu_designer-0.39.1/examples/scrollbarhelper.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/scrolledframe/demoapp.py` & `pygubu_designer-0.39.1/examples/scrolledframe/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/scrolledframe/scrolledframe_demo.ui` & `pygubu_designer-0.39.1/examples/scrolledframe/scrolledframe_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/scrolledframe-layouts.ui` & `pygubu_designer-0.39.1/examples/scrolledframe-layouts.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/scrolledframe.ui` & `pygubu_designer-0.39.1/examples/scrolledframe.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/scrolledtext/scrolledtext_demo.ui` & `pygubu_designer-0.39.1/examples/scrolledtext/scrolledtext_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/scrolledtext/scrolledtextdemoapp.py` & `pygubu_designer-0.39.1/examples/scrolledtext/scrolledtextdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/static_image/demoapp.py` & `pygubu_designer-0.39.1/examples/static_image/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/static_image/demoapp.ui` & `pygubu_designer-0.39.1/examples/static_image/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/static_image/logo_253.png` & `pygubu_designer-0.39.1/examples/static_image/logo_253.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/text/logwindowdemo/demo1.ui` & `pygubu_designer-0.39.1/examples/text/logwindowdemo/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/text/logwindowdemo/demo1app.py` & `pygubu_designer-0.39.1/examples/text/logwindowdemo/demo1app.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/tk_window/green.gif` & `pygubu_designer-0.39.1/examples/tk_window/green.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/tk_window/tkdemo.ui` & `pygubu_designer-0.39.1/examples/tk_window/tkdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/tk_window/tkdemoapp.py` & `pygubu_designer-0.39.1/examples/tk_window/tkdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/toplevel_centered/centered_demo1.py` & `pygubu_designer-0.39.1/examples/toplevel_centered/centered_demo1.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/toplevel_centered/centered_demo2.py` & `pygubu_designer-0.39.1/examples/toplevel_centered/centered_demo2.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/toplevel_centered/demo.ui` & `pygubu_designer-0.39.1/examples/toplevel_centered/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/toplevel_menu/menu.py` & `pygubu_designer-0.39.1/examples/toplevel_menu/menu.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/toplevel_menu/menu.ui` & `pygubu_designer-0.39.1/examples/toplevel_menu/menu.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/treeview/demo1/treeview.py` & `pygubu_designer-0.39.1/examples/treeview/demo1/treeview.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/treeview/demo1/treeview.ui` & `pygubu_designer-0.39.1/examples/treeview/demo1/treeview.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/treeview/demo2/columns_stretching.ui` & `pygubu_designer-0.39.1/examples/treeview/demo2/columns_stretching.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/treeview/demo2/columnsstretchingdemo.py` & `pygubu_designer-0.39.1/examples/treeview/demo2/columnsstretchingdemo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/treeview_editable/demo1/demoapp.py` & `pygubu_designer-0.39.1/examples/treeview_editable/demo1/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/treeview_editable/demo1/demoapp.ui` & `pygubu_designer-0.39.1/examples/treeview_editable/demo1/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/treeview_editable/demo2/demo2.ui` & `pygubu_designer-0.39.1/examples/treeview_editable/demo2/demo2.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/treeview_editable/demo2/demo2app.py` & `pygubu_designer-0.39.1/examples/treeview_editable/demo2/demo2app.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/treeview_filterable/demo.ui` & `pygubu_designer-0.39.1/examples/treeview_filterable/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/treeview_filterable/demoapp.py` & `pygubu_designer-0.39.1/examples/treeview_filterable/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/user_input/userinput.ui` & `pygubu_designer-0.39.1/examples/user_input/userinput.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/user_input/userinputapp.py` & `pygubu_designer-0.39.1/examples/user_input/userinputapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/variables.ui` & `pygubu_designer-0.39.1/examples/variables.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/vscrolledframe.ui` & `pygubu_designer-0.39.1/examples/vscrolledframe.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/windowdeleteevent/demo1.py` & `pygubu_designer-0.39.1/examples/windowdeleteevent/demo1.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/windowdeleteevent/demo1.ui` & `pygubu_designer-0.39.1/examples/windowdeleteevent/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/windowdeleteevent/demo2.py` & `pygubu_designer-0.39.1/examples/windowdeleteevent/demo2.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/examples/windowdeleteevent/demo2.ui` & `pygubu_designer-0.39.1/examples/windowdeleteevent/demo2.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/pygubu-designer.png` & `pygubu_designer-0.39.1/pygubu-designer.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/pyproject.toml` & `pygubu_designer-0.39.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubu_designer.egg-info/PKG-INFO` & `pygubu_designer-0.39.1/src/pygubu_designer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygubu-designer
-Version: 0.39
+Version: 0.39.1
 Summary: A simple GUI designer for the python tkinter module
 Author-email: Alejandro Autalan <alejandroautalan@gmail.com>
 License: GPL-3
 Project-URL: Documentation, https://github.com/alejandroautalan/pygubu-designer#readme
 Project-URL: Issues, https://github.com/alejandroautalan/pygubu-designer/issues
 Project-URL: Source, https://github.com/alejandroautalan/pygubu-designer
 Keywords: gui,tkinter,designer
```

### Comparing `pygubu_designer-0.39/src/pygubu_designer.egg-info/SOURCES.txt` & `pygubu_designer-0.39.1/src/pygubu_designer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/actions.py` & `pygubu_designer-0.39.1/src/pygubudesigner/actions.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/bindingseditor.py` & `pygubu_designer-0.39.1/src/pygubudesigner/bindingseditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/codegen/codebuilder.py` & `pygubu_designer-0.39.1/src/pygubudesigner/codegen/codebuilder.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/codegen/scriptgenerator.py` & `pygubu_designer-0.39.1/src/pygubudesigner/codegen/scriptgenerator.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/containerlayouteditor.py` & `pygubu_designer-0.39.1/src/pygubudesigner/containerlayouteditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/code_templates/app.py.mako` & `pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/app.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/code_templates/appuser.py.mako` & `pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/appuser.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/code_templates/customstyles.py.mako` & `pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/customstyles.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/code_templates/script.py.mako` & `pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/script.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/code_templates/widget.py.mako` & `pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/widget.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/code_templates/widgetbo.py.mako` & `pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/widgetbo.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/code_templates/widgetuser.py.mako` & `pygubu_designer-0.39.1/src/pygubudesigner/data/code_templates/widgetuser.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/pygubu.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/pygubu.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/pygubu200.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/pygubu200.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/property_invalid.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/property_invalid.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/pygubu.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/pygubu.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/pygubu200.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/pygubu200.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png` & `pygubu_designer-0.39.1/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39.1/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39.1/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Pygubu 0.7\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2024-04-14 20:06-0300\n"
+"PO-Revision-Date: 2024-04-21 22:05-0300\n"
 "Last-Translator: Alejandro Autalán <alejandroautalan@gmail.com>\n"
 "Language-Team: \n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "X-Generator: Poedit 3.2.2\n"
@@ -455,14 +455,24 @@
 
 msgid "Remove"
 msgstr "Remover"
 
 msgid "Request new ID and set widget as nameless."
 msgstr "Solicitar nuevo ID y establecer el widget como \"sin  nombre\"."
 
+msgid "Reset layout"
+msgstr "Restablecer disposición de ventanas"
+
+msgid ""
+"Restart Pygubu Designer\n"
+"for changes to take effect."
+msgstr ""
+"Reinicia Pygubu Designer\n"
+"para que los cambios tengan efecto."
+
 msgid ""
 "Restart Pygubu Designer for\n"
 "changes to take effect."
 msgstr "Reinicia Pygubu Designer para que los cambios tengan efecto."
 
 msgid "Row index: {0}"
 msgstr "Fila: {0}"
```

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo` & `pygubu_designer-0.39.1/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/locale/pygubu-designer.pot` & `pygubu_designer-0.39.1/src/pygubudesigner/data/locale/pygubu-designer.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: pygubudesigner\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-14 19:58-0300\n"
+"POT-Creation-Date: 2024-04-21 21:44-0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -100,15 +100,15 @@
 #: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:112
 #: src/pygubudesigner/data/ui/designer_settings.ui:248
 #: src/pygubudesigner/data/ui/project_settings.ui:748
 msgid "Cancel"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/ask_save_changes_dialog.ui:125
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:46
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:68
 msgid "Save"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/container_layout_editor_base.ui:25
 #: src/pygubudesigner/containerlayouteditor.py:42
 #, python-brace-format
 msgid "Options for {0} container"
@@ -265,17 +265,17 @@
 msgstr ""
 
 #: src/pygubudesigner/data/ui/project_settings.ui:521
 msgid "Add window centering code"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/project_settings.ui:538
-#: src/pygubudesigner/services/projectsettings.py:286
-#: src/pygubudesigner/services/projectsettings.py:306
-#: src/pygubudesigner/services/projectsettings.py:316
+#: src/pygubudesigner/services/projectsettings.py:282
+#: src/pygubudesigner/services/projectsettings.py:302
+#: src/pygubudesigner/services/projectsettings.py:312
 msgid "Styles"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/project_settings.ui:547
 msgid "Style definition file:"
 msgstr ""
 
@@ -309,226 +309,230 @@
 msgid "Select a widget builder file"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/project_settings.ui:719
 msgid "-"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:7
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:29
 msgid "File"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:14
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:36
 msgid "New"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:21
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:43
 msgid "Open …"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:26
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:48
 msgid "Open recent …"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:34
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:56
 msgid "Clear list"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:52
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:74
 msgid "Save as …"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:62 src/pygubudesigner/main.py:180
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:84 src/pygubudesigner/main.py:180
 msgid "Quit …"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:69
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:91
 msgid "Edit"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:76
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:260
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:98
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:291
 msgid "Copy"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:83
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:266
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:105
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:297
 msgid "Paste"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:90
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:272
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:112
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:303
 msgid "Cut"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:97
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:287
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:119
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:318
 msgid "Duplicate"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:105
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:127
 msgid "Widget tree"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:111
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:133
 msgid "Item up"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:118
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:140
 msgid "Item down"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:127
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:149
 msgid "Item delete"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:134
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:156
 msgid "Widget grid"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:140
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:162
 msgid "Move up"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:147
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:169
 msgid "Move down"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:154
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:176
 msgid "Move left"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:161
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:183
 msgid "Move right"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:172
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:194
+msgid "Reset layout"
+msgstr ""
+
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:203
 msgid "Preferences"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:179
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:210
 msgid "Project"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:185
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:216
 msgid "Settings"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:194
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:225
 msgid "Generate code"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:201
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:651
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:232
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:682
 msgid "Preview"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:208
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:239
 msgid "Preview in Toplevel"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:215
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:246
 msgid "Close Toplevel previews"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:220
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:251
 msgid "ttk theme"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:228
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:259
 msgid "Help"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:234
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:265
 msgid "Pygubu wiki"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:240
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:271
 msgid "About Pygubu"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:251
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:282
 msgid "Go to parent"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:278
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:309
 msgid "Delete"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:296 src/pygubudesigner/main.py:150
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:327 src/pygubudesigner/main.py:150
 msgid "Pygubu Designer"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:339
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:370
 msgid "Components Palette"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:360
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:391
 msgid "Project Tree"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:381
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:412
 #: src/pygubudesigner/data/ui/treecomponent_palette.ui:25
 #: src/pygubudesigner/services/widgets/treecomponentpaletteui.py:29
 msgid "Filter:"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:403
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:434
 msgid "✖"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:432
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:463
 msgid "ID"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:444
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:475
 msgid "Class"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:456
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:487
 msgid "R"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:468
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:499
 msgid "C"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:480
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:511
 msgid " "
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:496
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:527
 msgid "Properties"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:521
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:552
 msgid "Appearance"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:540
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:571
 msgid "Layout"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:558
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:589
 msgid "Bindings"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:592
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:623
 msgid "Sequence descriptor"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:604
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:635
 msgid "Event Handler"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:616
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:647
 msgid "Add"
 msgstr ""
 
-#: src/pygubudesigner/data/ui/pygubu-ui.ui:755
+#: src/pygubudesigner/data/ui/pygubu-ui.ui:786
 msgid "Messages"
 msgstr ""
 
 #: src/pygubudesigner/data/ui/treecomponent_palette.ui:73
 #: src/pygubudesigner/services/widgets/treecomponentpaletteui.py:52
 msgid "tk"
 msgstr ""
@@ -599,15 +603,15 @@
 
 #: src/pygubudesigner/main.py:84
 #, python-brace-format
 msgid "Failed to load widget module: '{_module}'"
 msgstr ""
 
 #: src/pygubudesigner/main.py:86 src/pygubudesigner/main.py:627
-#: src/pygubudesigner/main.py:676 src/pygubudesigner/main.py:921
+#: src/pygubudesigner/main.py:676 src/pygubudesigner/main.py:933
 #: src/pygubudesigner/preferences.py:106 src/pygubudesigner/preferences.py:112
 msgid "Error"
 msgstr ""
 
 #: src/pygubudesigner/main.py:548
 msgid "Checking main window visibility."
 msgstr ""
@@ -646,23 +650,29 @@
 msgid "Do you want to save the changes before opening?"
 msgstr ""
 
 #: src/pygubudesigner/main.py:699
 msgid "Do you want to save the changes before creating?"
 msgstr ""
 
-#: src/pygubudesigner/main.py:840
+#: src/pygubudesigner/main.py:847
+msgid ""
+"Restart Pygubu Designer\n"
+"for changes to take effect."
+msgstr ""
+
+#: src/pygubudesigner/main.py:852
 msgid "Open a project first."
 msgstr ""
 
-#: src/pygubudesigner/main.py:866
+#: src/pygubudesigner/main.py:878
 msgid "Project code generated."
 msgstr ""
 
-#: src/pygubudesigner/main.py:881
+#: src/pygubudesigner/main.py:893
 msgid "newproject"
 msgstr ""
 
 #: src/pygubudesigner/preferences.py:103
 msgid ""
 "Configuration file at {CONFIG_FILE!s} is corrupted, program may not work as "
 "expected.If you delete this file, configuration will be set to default"
@@ -1849,28 +1859,28 @@
 msgid "Code Script"
 msgstr ""
 
 #: src/pygubudesigner/services/projectsettings.py:63
 msgid "Custom Widget"
 msgstr ""
 
-#: src/pygubudesigner/services/projectsettings.py:285
+#: src/pygubudesigner/services/projectsettings.py:281
 msgid ""
 "Restart Pygubu Designer for\n"
 "changes to take effect."
 msgstr ""
 
-#: src/pygubudesigner/services/projectsettings.py:304
+#: src/pygubudesigner/services/projectsettings.py:300
 msgid ""
 "File saved.\n"
 "\n"
 "Please edit the style definition file."
 msgstr ""
 
-#: src/pygubudesigner/services/projectsettings.py:315
+#: src/pygubudesigner/services/projectsettings.py:311
 msgid "Error saving template file."
 msgstr ""
 
 #: src/pygubudesigner/services/stylehandler.py:78
 msgid "Applying ttk style definitions"
 msgstr ""
```

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/locale/pygubu.pot` & `pygubu_designer-0.39.1/src/pygubudesigner/data/locale/pygubu.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: pygubu\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-14 19:58-0300\n"
+"POT-Creation-Date: 2024-04-21 21:44-0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=CHARSET\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -267,38 +267,38 @@
 
 #: ../pygubu/src/pygubu/plugins/pygubu/pathchooserinput.py:103
 msgid "Path entry state."
 msgstr ""
 
 #: ../pygubu/src/pygubu/plugins/pygubu/scrollbarhelper.py:60
 #: ../pygubu/src/pygubu/plugins/pygubu/tkscrollbarhelper.py:76
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1439
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1484
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1529
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1441
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1486
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1531
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:501
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:567
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:669
 msgid "Pygubu Helpers"
 msgstr ""
 
 #: ../pygubu/src/pygubu/plugins/pygubu/tkinterscrolledtext.py:17
 #: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:187
 #: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:271
 #: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:320
 #: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:380
 #: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:439
 #: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:480
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:578
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:669
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:700
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:745
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:778
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:854
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:896
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1544
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:580
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:671
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:702
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:747
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:780
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:856
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:898
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1546
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:69
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:89
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:112
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:136
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:177
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:193
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:204
@@ -380,30 +380,30 @@
 msgid "tksheet"
 msgstr ""
 
 #: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:65
 #: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:120
 #: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:150
 #: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:220
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:611
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:613
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:43
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:307
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:324
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:338
 msgid "Containers"
 msgstr ""
 
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:668
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:990
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1335
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1348
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1372
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1395
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1413
-#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1529
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:670
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:992
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1337
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1350
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1374
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1397
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1415
+#: ../pygubu/src/pygubu/plugins/tk/tkstdwidgets.py:1531
 #: ../pygubu/src/pygubu/plugins/ttk/ttkstdwidgets.py:368
 msgid "Menu"
 msgstr ""
 
 #: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:44
 #: ../pygubu/src/pygubu/plugins/ttkwidgets/autocomplete.py:171
 msgid "Values separated by space. In code you can pass a full list"
```

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39.1/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39.1/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo` & `pygubu_designer-0.39.1/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39.1/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo` & `pygubu_designer-0.39.1/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/ui/about_dialog.ui` & `pygubu_designer-0.39.1/src/pygubudesigner/data/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui` & `pygubu_designer-0.39.1/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/ui/container_layout_editor_base.ui` & `pygubu_designer-0.39.1/src/pygubudesigner/data/ui/container_layout_editor_base.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/ui/designer_settings.ui` & `pygubu_designer-0.39.1/src/pygubudesigner/data/ui/designer_settings.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/ui/messagebox.ui` & `pygubu_designer-0.39.1/src/pygubudesigner/data/ui/messagebox.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/ui/project_settings.ui` & `pygubu_designer-0.39.1/src/pygubudesigner/data/ui/project_settings.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/ui/pygubu-ui.ui` & `pygubu_designer-0.39.1/src/pygubudesigner/data/ui/pygubu-ui.ui`

 * *Files 0% similar despite different names*

#### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/ui/pygubu-ui.ui` & `pygubu_designer-0.39.1/src/pygubudesigner/data/ui/pygubu-ui.ui`

```diff
@@ -1,9 +1,31 @@
 <?xml version="1.0" encoding="utf-8"?>
-<interface version="1.4" author="PygubuDesigner 0.38">
+<interface version="1.4" author="PygubuDesigner 0.39">
+  <project>
+    <settings>
+      <setting id="name">pygubu-designer window</setting>
+      <setting id="description">This is the main pygubu-designer ui file.</setting>
+      <setting id="module_name">projectsettings</setting>
+      <setting id="output_dir">../../</setting>
+      <setting id="template">application</setting>
+      <setting id="main_widget">mainwindow</setting>
+      <setting id="main_classname">PygubuDesigner</setting>
+      <setting id="main_menu"/>
+      <setting id="import_tkvariables">False</setting>
+      <setting id="use_ttk_styledefinition_file">False</setting>
+      <setting id="use_i18n">False</setting>
+      <setting id="all_ids_attributes">False</setting>
+      <setting id="generate_code_onsave">False</setting>
+      <setting id="use_window_centering_code">False</setting>
+      <setting id="ttk_style_definition_file"/>
+    </settings>
+    <customwidgets>
+      <customwidget path="../../services/widgets/treecomponentpalettebo.py"/>
+    </customwidgets>
+  </project>
   <object class="tk.Menu" id="mainmenu">
     <property name="tearoff">0</property>
     <child>
       <object class="tk.Menuitem.Submenu" id="filemenu">
         <property name="label" translatable="yes">File</property>
         <property name="tearoff">0</property>
         <property name="underline">0</property>
@@ -163,14 +185,23 @@
             </child>
           </object>
         </child>
         <child>
           <object class="tk.Menuitem.Separator" id="edit_Separator2"/>
         </child>
         <child>
+          <object class="tk.Menuitem.Command" id="reset_layout" named="True">
+            <property name="command" type="command" cbtype="with_wid">on_edit_menuitem_clicked</property>
+            <property name="label" translatable="yes">Reset layout</property>
+          </object>
+        </child>
+        <child>
+          <object class="tk.Menuitem.Separator" id="separator2"/>
+        </child>
+        <child>
           <object class="tk.Menuitem.Command" id="edit_preferences">
             <property name="command" type="command" cbtype="with_wid" args="">on_edit_menuitem_clicked</property>
             <property name="label" translatable="yes">Preferences</property>
           </object>
         </child>
       </object>
     </child>
@@ -766,30 +797,8 @@
               </object>
             </child>
           </object>
         </child>
       </object>
     </child>
   </object>
-  <project>
-    <settings>
-      <setting id="name">pygubu-designer window</setting>
-      <setting id="description">This is the main pygubu-designer ui file.</setting>
-      <setting id="module_name">projectsettings</setting>
-      <setting id="output_dir">../../</setting>
-      <setting id="template">application</setting>
-      <setting id="main_widget">mainwindow</setting>
-      <setting id="main_classname">PygubuDesigner</setting>
-      <setting id="main_menu"/>
-      <setting id="import_tkvariables">False</setting>
-      <setting id="use_ttk_styledefinition_file">False</setting>
-      <setting id="use_i18n">False</setting>
-      <setting id="all_ids_attributes">False</setting>
-      <setting id="generate_code_onsave">False</setting>
-      <setting id="use_window_centering_code">False</setting>
-      <setting id="ttk_style_definition_file"/>
-    </settings>
-    <customwidgets>
-      <customwidget path="../../services/widgets/treecomponentpalettebo.py"/>
-    </customwidgets>
-  </project>
 </interface>
```

### Comparing `pygubu_designer-0.39/src/pygubudesigner/data/ui/treecomponent_palette.ui` & `pygubu_designer-0.39.1/src/pygubudesigner/data/ui/treecomponent_palette.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/designerstyles.py` & `pygubu_designer-0.39.1/src/pygubudesigner/designerstyles.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/dialogs.py` & `pygubu_designer-0.39.1/src/pygubudesigner/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/i18n.py` & `pygubu_designer-0.39.1/src/pygubudesigner/i18n.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/layouteditor.py` & `pygubu_designer-0.39.1/src/pygubudesigner/layouteditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/logpanel.py` & `pygubu_designer-0.39.1/src/pygubudesigner/logpanel.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/main.py` & `pygubu_designer-0.39.1/src/pygubudesigner/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -720,18 +720,22 @@
         action = f"<<ACTION_{itemid}>>"
         self.mainwindow.event_generate(action)
 
     # Edit menu
     def on_edit_menuitem_clicked(self, itemid):
         if itemid == "edit_preferences":
             self._edit_preferences()
+            
+        elif itemid == "reset_layout":
+            self._reset_layout()            
+            
         else:
             action = f"<<ACTION_{itemid}>>"
             self.mainwindow.event_generate(action)
-
+            
     # Project menu
     def on_project_menuitem_clicked(self, itemid):
         if itemid == "project_settings":
             self._edit_project_settings()
         if itemid == "project_codegen":
             self._project_code_generate()
 
@@ -830,14 +834,22 @@
         self.about_dialog.run()
 
     def _edit_preferences(self):
         if self.preferences is None:
             # self.preferences = pref.PreferencesUI(self.mainwindow, translator)
             self.preferences = DesignerSettings(self.mainwindow, translator)
         self.preferences.run()
+        
+    def _reset_layout(self):
+        """
+        Reset the docked frames back to their default positions.
+        """
+        self.on_dockframe_changed(reset_layout=True)
+        msg = _("Restart Pygubu Designer\nfor changes to take effect.")
+        messagebox.showinfo(self.mbox_title, msg, parent=self.mainwindow)         
 
     def _require_project_open(self):
         if self.current_project is None:
             msg = _("Open a project first.")
             messagebox.showinfo(self.mbox_title, msg, parent=self.mainwindow)
         return self.current_project is not None
 
@@ -919,18 +931,33 @@
                 show_error(
                     self.mainwindow,
                     _("Error"),
                     msg,
                     det,
                 )
 
-    def on_dockframe_changed(self, event=None):
-        """Save current layout of maindock widget."""
-        dock = self.builder.get_object("maindock")
-        dock_layout = dock.save_layout()
+    def on_dockframe_changed(self, event=None, reset_layout=False):
+        """
+        Save current layout of maindock widget.
+        
+        Arguments:
+        
+        - event
+        
+        - reset_layout: used for resetting the docked frames
+        back to their default locations/positions.
+        """
+        
+        # Should we reset the layout back to the defaults?
+        if reset_layout:
+            dock_layout = None
+        else:
+            dock = self.builder.get_object("maindock")
+            dock_layout = dock.save_layout()
+            
         pref.save_maindock_layout(dock_layout)
 
     def load_dockframe_layout(self):
         """Load layout for maindock widget."""
         layout = pref.get_maindock_layout()
         try:
             dock = self.builder.get_object("maindock")
```

### Comparing `pygubu_designer-0.39/src/pygubudesigner/preferences.py` & `pygubu_designer-0.39.1/src/pygubudesigner/preferences.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/preview/builder.py` & `pygubu_designer-0.39.1/src/pygubudesigner/preview/builder.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/preview/helper.py` & `pygubu_designer-0.39.1/src/pygubudesigner/preview/helper.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/preview/preview.py` & `pygubu_designer-0.39.1/src/pygubudesigner/preview/preview.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/properties/editors/forms.py` & `pygubu_designer-0.39.1/src/pygubudesigner/properties/editors/forms.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/properties/manager.py` & `pygubu_designer-0.39.1/src/pygubudesigner/properties/manager.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/properties/predefined.py` & `pygubu_designer-0.39.1/src/pygubudesigner/properties/predefined.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/properties/propertieshelp.py` & `pygubu_designer-0.39.1/src/pygubudesigner/properties/propertieshelp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/propertieseditor.py` & `pygubu_designer-0.39.1/src/pygubudesigner/propertieseditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/rfilemanager.py` & `pygubu_designer-0.39.1/src/pygubudesigner/rfilemanager.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/aboutdialog.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/aboutdialog.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/aboutdialogui.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/aboutdialogui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/designersettings.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/designersettings.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/designersettingsui.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/designersettingsui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/fieldvalidator.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/fieldvalidator.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/messagebox.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/messagebox.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/messageboxui.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/messageboxui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/project.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/project.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/projectsettings.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/projectsettings.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/projectsettingsui.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/projectsettingsui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/stylehandler.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/stylehandler.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/theming.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/theming.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/widgets/treecomponentpalette.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/widgets/treecomponentpalette.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/services/widgets/treecomponentpaletteui.py` & `pygubu_designer-0.39.1/src/pygubudesigner/services/widgets/treecomponentpaletteui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/uitreeeditor.py` & `pygubu_designer-0.39.1/src/pygubudesigner/uitreeeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/util/__init__.py` & `pygubu_designer-0.39.1/src/pygubudesigner/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/util/gridcalculator.py` & `pygubu_designer-0.39.1/src/pygubudesigner/util/gridcalculator.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/util/keyboard.py` & `pygubu_designer-0.39.1/src/pygubudesigner/util/keyboard.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/util/observable.py` & `pygubu_designer-0.39.1/src/pygubudesigner/util/observable.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/util/screens.py` & `pygubu_designer-0.39.1/src/pygubudesigner/util/screens.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/util/selecttool.py` & `pygubu_designer-0.39.1/src/pygubudesigner/util/selecttool.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgetdescr.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgetdescr.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/__init__.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/bindingeditor.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/bindingeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/colorentry.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/colorentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/commandentry.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/commandentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/componentpalette.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/componentpalette.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/containerlayouteditorbase.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/containerlayouteditorbase.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/cursorentry.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/cursorentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/dimensionentry.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/dimensionentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/dynamicpropeditor.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/dynamicpropeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/entryvalidatecommandeditor.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/entryvalidatecommandeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/fontentry.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/fontentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/gridselector.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/gridselector.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/imageentry.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/imageentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/namedideditor.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/namedideditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/pixelcoordinateentry.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/pixelcoordinateentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/propertyeditor.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/propertyeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/relativeentry.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/relativeentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/stickyentry.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/stickyentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/tkvarentry.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/tkvarentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/toolbarframe.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/toolbarframe.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/ttkstyleentry.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/ttkstyleentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/src/pygubudesigner/widgets/whentry.py` & `pygubu_designer-0.39.1/src/pygubudesigner/widgets/whentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39/tests/test_plugin_init.py` & `pygubu_designer-0.39.1/tests/test_plugin_init.py`

 * *Files identical despite different names*


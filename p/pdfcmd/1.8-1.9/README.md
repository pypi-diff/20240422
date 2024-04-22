# Comparing `tmp/pdfcmd-1.8.tar.gz` & `tmp/pdfcmd-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfcmd-1.8.tar", last modified: Thu Apr 13 01:15:26 2023, max compression
+gzip compressed data, was "pdfcmd-1.9.tar", last modified: Sun Sep 17 23:45:22 2023, max compression
```

## Comparing `pdfcmd-1.8.tar` & `pdfcmd-1.9.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-13 01:15:26.725440 pdfcmd-1.8/
--rw-r--r--   0 mark      (1000) mark      (1000)     5620 2023-04-13 01:15:26.722107 pdfcmd-1.8/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     5264 2023-04-13 01:11:07.000000 pdfcmd-1.8/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-13 01:15:26.718773 pdfcmd-1.8/pdfcmd/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-01-27 04:55:01.000000 pdfcmd-1.8/pdfcmd/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)       66 2022-07-21 00:18:22.000000 pdfcmd-1.8/pdfcmd/__main__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-13 01:15:26.722107 pdfcmd-1.8/pdfcmd/commands/
--rw-r--r--   0 mark      (1000) mark      (1000)     3162 2023-02-12 23:20:04.000000 pdfcmd-1.8/pdfcmd/commands/cat.py
--rw-r--r--   0 mark      (1000) mark      (1000)      113 2022-07-25 00:30:51.000000 pdfcmd-1.8/pdfcmd/commands/help.py
--rw-r--r--   0 mark      (1000) mark      (1000)      483 2022-12-24 07:53:21.000000 pdfcmd-1.8/pdfcmd/commands/info.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2630 2022-12-25 03:57:34.000000 pdfcmd-1.8/pdfcmd/commands/pages.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1373 2023-04-13 01:10:47.000000 pdfcmd-1.8/pdfcmd/pdfcmd.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-13 01:15:26.722107 pdfcmd-1.8/pdfcmd.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     5620 2023-04-13 01:15:26.000000 pdfcmd-1.8/pdfcmd.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      351 2023-04-13 01:15:26.000000 pdfcmd-1.8/pdfcmd.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-13 01:15:26.000000 pdfcmd-1.8/pdfcmd.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       46 2023-04-13 01:15:26.000000 pdfcmd-1.8/pdfcmd.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       13 2023-04-13 01:15:26.000000 pdfcmd-1.8/pdfcmd.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       23 2023-04-13 01:15:26.000000 pdfcmd-1.8/pdfcmd.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-04-13 01:15:26.725440 pdfcmd-1.8/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1029 2023-04-13 01:14:58.000000 pdfcmd-1.8/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-09-17 23:45:22.102011 pdfcmd-1.9/
+-rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-07-01 05:55:41.000000 pdfcmd-1.9/.flake8
+-rw-r--r--   0 mark      (1000) mark      (1000)       72 2022-09-06 00:53:12.000000 pdfcmd-1.9/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      337 2023-07-01 06:00:40.000000 pdfcmd-1.9/Makefile
+-rw-r--r--   0 mark      (1000) mark      (1000)     5311 2023-09-17 23:45:22.102011 pdfcmd-1.9/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     4915 2023-09-17 23:42:44.000000 pdfcmd-1.9/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-09-17 23:45:22.102011 pdfcmd-1.9/pdfcmd/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-01-27 04:55:01.000000 pdfcmd-1.9/pdfcmd/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       93 2023-04-26 03:20:55.000000 pdfcmd-1.9/pdfcmd/__main__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-09-17 23:45:22.102011 pdfcmd-1.9/pdfcmd/commands/
+-rw-r--r--   0 mark      (1000) mark      (1000)     3162 2023-02-12 23:20:04.000000 pdfcmd-1.9/pdfcmd/commands/cat.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      113 2022-07-25 00:30:51.000000 pdfcmd-1.9/pdfcmd/commands/help.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      483 2022-12-24 07:53:21.000000 pdfcmd-1.9/pdfcmd/commands/info.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2630 2022-12-25 03:57:34.000000 pdfcmd-1.9/pdfcmd/commands/pages.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1410 2023-09-17 05:05:32.000000 pdfcmd-1.9/pdfcmd/pdfcmd.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-09-17 23:45:22.102011 pdfcmd-1.9/pdfcmd.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     5311 2023-09-17 23:45:22.000000 pdfcmd-1.9/pdfcmd.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      385 2023-09-17 23:45:22.000000 pdfcmd-1.9/pdfcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-09-17 23:45:22.000000 pdfcmd-1.9/pdfcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       46 2023-09-17 23:45:22.000000 pdfcmd-1.9/pdfcmd.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       13 2023-09-17 23:45:22.000000 pdfcmd-1.9/pdfcmd.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        7 2023-09-17 23:45:22.000000 pdfcmd-1.9/pdfcmd.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      936 2023-07-01 06:04:35.000000 pdfcmd-1.9/pyproject.toml
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-09-17 23:45:22.102011 pdfcmd-1.9/setup.cfg
```

### Comparing `pdfcmd-1.8/PKG-INFO` & `pdfcmd-1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pdfcmd
-Version: 1.8
+Version: 1.9
 Summary: Utility to perform commands on PDF files
-Home-page: https://github.com/bulletmark/pdfcmd
-Author: Mark Blakeney
-Author-email: mark.blakeney@bullet-systems.net
+Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
-Keywords: PDF
+Project-URL: Homepage, https://github.com/bulletmark/pdfcmd
+Keywords: PDF,pypdf
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: pypdf>=3.1.0
 
 ## PDFCMD - Utility to Perform Commands on PDF Files
 [![PyPi](https://img.shields.io/pypi/v/pdfcmd)](https://pypi.org/project/pdfcmd/)
 [![AUR](https://img.shields.io/aur/version/pdfcmd)](https://aur.archlinux.org/packages/pdfcmd/)
 
 This is a Linux command line utility to perform commands on PDF files.
 It uses the [pypdf](https://github.com/py-pdf/pypdf) library. The
@@ -24,48 +24,34 @@
 https://github.com/bulletmark/pdfcmd.
 
 ## Usage
 
 Type `pdfcmd` or `pdfcmd -h` to view the usage summary:
 
 ```
-usage: pdfcmd [-h] {info,help,cat,pages} ...
+usage: pdfcmd [-h] {cat,help,info,pages} ...
 
 Utility to perform commands on PDF files.
 
 options:
   -h, --help            show this help message and exit
 
 Commands:
-  {info,help,cat,pages}
-    info                Show PDF document information.
-    help                Show help/usage for this utility.
+  {cat,help,info,pages}
     cat                 Concaternate selected pages of one or more PDF files
                         into a single file.
+    help                Show help/usage for this utility.
+    info                Show PDF document information.
     pages               Output list of page labels/numbers, or total number of
                         pages.
 ```
 
 Type `pdfcmd <command> -h` to see specific help/usage for any
 individual command:
 
-### Command `info`
-
-```
-usage: pdfcmd info [-h] file
-
-Show PDF document information.
-
-positional arguments:
-  file        PDF file
-
-options:
-  -h, --help  show this help message and exit
-```
-
 ### Command `cat`
 
 ```
 usage: pdfcmd cat [-h] [-o OUTFILE] [-a] ...
 
 Concaternate selected pages of one or more PDF files into a single file.
 
@@ -112,14 +98,28 @@
       5:    from the sixth page onward.  -3:-1 third & second to last.
   The third, "stride" or "step" number is also recognized.
       ::2       0 2 4 ... to the end.    3:0:-1    3 2 1 but not 0.
       1:10:2    1 3 5 7 9                2::-1     2 1 0.
       ::-1      all pages in reverse order.
 ```
 
+### Command `info`
+
+```
+usage: pdfcmd info [-h] file
+
+Show PDF document information.
+
+positional arguments:
+  file        PDF file
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ### Command `pages`
 
 ```
 usage: pdfcmd pages [-h] [-c] file
 
 Output list of page labels/numbers, or total number of pages.
 
@@ -141,45 +141,27 @@
 options:
   -h, --help  show this help message and exit
 ```
 
 ## INSTALLATION
 
 Arch Linux users can install [pdfcmd from the
-AUR](https://aur.archlinux.org/packages/pdfcmd).
-Python 3.6 or later is required. Note [pdfcmd is on
-PyPI](https://pypi.org/project/pdfcmd/) so just ensure that
-`python3-pip` and `python3-wheel` are installed then type the following
-to install (or upgrade):
+AUR](https://aur.archlinux.org/packages/pdfcmd). Python 3.6 or later is
+required. Note [pdfcmd is on PyPI](https://pypi.org/project/pdfcmd/) so
+just ensure that [`pipx`](https://pypa.github.io/pipx/) is installed
+then type the following:
 
 ```
-$ sudo pip3 install -U pdfcmd
+$ pipx install pdfcmd
 ```
 
-Alternatively, do the following to install from the source repository.
-Note that the `python-pypdf` package is required.
+To upgrade:
 
-```sh
-$ git clone http://github.com/bulletmark/pdfcmd
-$ cd pdfcmd
-$ sudo pip3 install -U .
 ```
-
-## UPGRADE
-
-```sh
-$ cd pdfcmd  # Source dir, as above
-$ git pull
-$ sudo pip3 install -U .
-```
-
-## REMOVAL
-
-```sh
-$ sudo pip3 uninstall pdfcmd
+$ pipx upgrade pdfcmd
 ```
 
 ## LICENSE
 
 Copyright (C) 2021 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License.
 This program is free software: you can redistribute it and/or modify it
```

### Comparing `pdfcmd-1.8/README.md` & `pdfcmd-1.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,48 +11,34 @@
 https://github.com/bulletmark/pdfcmd.
 
 ## Usage
 
 Type `pdfcmd` or `pdfcmd -h` to view the usage summary:
 
 ```
-usage: pdfcmd [-h] {info,help,cat,pages} ...
+usage: pdfcmd [-h] {cat,help,info,pages} ...
 
 Utility to perform commands on PDF files.
 
 options:
   -h, --help            show this help message and exit
 
 Commands:
-  {info,help,cat,pages}
-    info                Show PDF document information.
-    help                Show help/usage for this utility.
+  {cat,help,info,pages}
     cat                 Concaternate selected pages of one or more PDF files
                         into a single file.
+    help                Show help/usage for this utility.
+    info                Show PDF document information.
     pages               Output list of page labels/numbers, or total number of
                         pages.
 ```
 
 Type `pdfcmd <command> -h` to see specific help/usage for any
 individual command:
 
-### Command `info`
-
-```
-usage: pdfcmd info [-h] file
-
-Show PDF document information.
-
-positional arguments:
-  file        PDF file
-
-options:
-  -h, --help  show this help message and exit
-```
-
 ### Command `cat`
 
 ```
 usage: pdfcmd cat [-h] [-o OUTFILE] [-a] ...
 
 Concaternate selected pages of one or more PDF files into a single file.
 
@@ -99,14 +85,28 @@
       5:    from the sixth page onward.  -3:-1 third & second to last.
   The third, "stride" or "step" number is also recognized.
       ::2       0 2 4 ... to the end.    3:0:-1    3 2 1 but not 0.
       1:10:2    1 3 5 7 9                2::-1     2 1 0.
       ::-1      all pages in reverse order.
 ```
 
+### Command `info`
+
+```
+usage: pdfcmd info [-h] file
+
+Show PDF document information.
+
+positional arguments:
+  file        PDF file
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ### Command `pages`
 
 ```
 usage: pdfcmd pages [-h] [-c] file
 
 Output list of page labels/numbers, or total number of pages.
 
@@ -128,45 +128,27 @@
 options:
   -h, --help  show this help message and exit
 ```
 
 ## INSTALLATION
 
 Arch Linux users can install [pdfcmd from the
-AUR](https://aur.archlinux.org/packages/pdfcmd).
-Python 3.6 or later is required. Note [pdfcmd is on
-PyPI](https://pypi.org/project/pdfcmd/) so just ensure that
-`python3-pip` and `python3-wheel` are installed then type the following
-to install (or upgrade):
+AUR](https://aur.archlinux.org/packages/pdfcmd). Python 3.6 or later is
+required. Note [pdfcmd is on PyPI](https://pypi.org/project/pdfcmd/) so
+just ensure that [`pipx`](https://pypa.github.io/pipx/) is installed
+then type the following:
 
 ```
-$ sudo pip3 install -U pdfcmd
+$ pipx install pdfcmd
 ```
 
-Alternatively, do the following to install from the source repository.
-Note that the `python-pypdf` package is required.
+To upgrade:
 
-```sh
-$ git clone http://github.com/bulletmark/pdfcmd
-$ cd pdfcmd
-$ sudo pip3 install -U .
 ```
-
-## UPGRADE
-
-```sh
-$ cd pdfcmd  # Source dir, as above
-$ git pull
-$ sudo pip3 install -U .
-```
-
-## REMOVAL
-
-```sh
-$ sudo pip3 uninstall pdfcmd
+$ pipx upgrade pdfcmd
 ```
 
 ## LICENSE
 
 Copyright (C) 2021 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License.
 This program is free software: you can redistribute it and/or modify it
```

### Comparing `pdfcmd-1.8/pdfcmd/commands/cat.py` & `pdfcmd-1.9/pdfcmd/commands/cat.py`

 * *Files identical despite different names*

### Comparing `pdfcmd-1.8/pdfcmd/commands/pages.py` & `pdfcmd-1.9/pdfcmd/commands/pages.py`

 * *Files identical despite different names*

### Comparing `pdfcmd-1.8/pdfcmd/pdfcmd.py` & `pdfcmd-1.9/pdfcmd/pdfcmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     'Main code'
     mainparser = argparse.ArgumentParser(description=__doc__)
     subparser = mainparser.add_subparsers(title='Commands',
             dest='func')
 
     # Iterate over the commands to set up their parsers
     prog = Path(__file__)
-    for modfile in (prog.parent / 'commands').glob('[!_]*.py'):
+    for modfile in sorted((prog.parent / 'commands').glob('[!_]*.py')):
         name = modfile.stem
         mod = importlib.import_module(f'{prog.stem}.commands.{name}')
-        docstr = mod.__doc__.strip() if mod.__doc__ else None
-        parser = subparser.add_parser(name, description=docstr,
+        docstr = mod.__doc__.strip().split('\n\n')[0] if mod.__doc__ else None
+        parser = subparser.add_parser(name, description=mod.__doc__,
                 formatter_class=argparse.RawDescriptionHelpFormatter,
                 help=docstr)
 
         # Add reference to mainparser in case subcommand needs it
         parser._mainparser = mainparser
 
         if hasattr(mod, 'init'):
@@ -36,11 +36,11 @@
     args = mainparser.parse_args()
 
     if not args.func:
         mainparser.print_help()
         return
 
     # Run the command that the user specified
-    args.func(args)
+    return args.func(args)
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `pdfcmd-1.8/pdfcmd.egg-info/PKG-INFO` & `pdfcmd-1.9/pdfcmd.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pdfcmd
-Version: 1.8
+Version: 1.9
 Summary: Utility to perform commands on PDF files
-Home-page: https://github.com/bulletmark/pdfcmd
-Author: Mark Blakeney
-Author-email: mark.blakeney@bullet-systems.net
+Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
-Keywords: PDF
+Project-URL: Homepage, https://github.com/bulletmark/pdfcmd
+Keywords: PDF,pypdf
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: pypdf>=3.1.0
 
 ## PDFCMD - Utility to Perform Commands on PDF Files
 [![PyPi](https://img.shields.io/pypi/v/pdfcmd)](https://pypi.org/project/pdfcmd/)
 [![AUR](https://img.shields.io/aur/version/pdfcmd)](https://aur.archlinux.org/packages/pdfcmd/)
 
 This is a Linux command line utility to perform commands on PDF files.
 It uses the [pypdf](https://github.com/py-pdf/pypdf) library. The
@@ -24,48 +24,34 @@
 https://github.com/bulletmark/pdfcmd.
 
 ## Usage
 
 Type `pdfcmd` or `pdfcmd -h` to view the usage summary:
 
 ```
-usage: pdfcmd [-h] {info,help,cat,pages} ...
+usage: pdfcmd [-h] {cat,help,info,pages} ...
 
 Utility to perform commands on PDF files.
 
 options:
   -h, --help            show this help message and exit
 
 Commands:
-  {info,help,cat,pages}
-    info                Show PDF document information.
-    help                Show help/usage for this utility.
+  {cat,help,info,pages}
     cat                 Concaternate selected pages of one or more PDF files
                         into a single file.
+    help                Show help/usage for this utility.
+    info                Show PDF document information.
     pages               Output list of page labels/numbers, or total number of
                         pages.
 ```
 
 Type `pdfcmd <command> -h` to see specific help/usage for any
 individual command:
 
-### Command `info`
-
-```
-usage: pdfcmd info [-h] file
-
-Show PDF document information.
-
-positional arguments:
-  file        PDF file
-
-options:
-  -h, --help  show this help message and exit
-```
-
 ### Command `cat`
 
 ```
 usage: pdfcmd cat [-h] [-o OUTFILE] [-a] ...
 
 Concaternate selected pages of one or more PDF files into a single file.
 
@@ -112,14 +98,28 @@
       5:    from the sixth page onward.  -3:-1 third & second to last.
   The third, "stride" or "step" number is also recognized.
       ::2       0 2 4 ... to the end.    3:0:-1    3 2 1 but not 0.
       1:10:2    1 3 5 7 9                2::-1     2 1 0.
       ::-1      all pages in reverse order.
 ```
 
+### Command `info`
+
+```
+usage: pdfcmd info [-h] file
+
+Show PDF document information.
+
+positional arguments:
+  file        PDF file
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ### Command `pages`
 
 ```
 usage: pdfcmd pages [-h] [-c] file
 
 Output list of page labels/numbers, or total number of pages.
 
@@ -141,45 +141,27 @@
 options:
   -h, --help  show this help message and exit
 ```
 
 ## INSTALLATION
 
 Arch Linux users can install [pdfcmd from the
-AUR](https://aur.archlinux.org/packages/pdfcmd).
-Python 3.6 or later is required. Note [pdfcmd is on
-PyPI](https://pypi.org/project/pdfcmd/) so just ensure that
-`python3-pip` and `python3-wheel` are installed then type the following
-to install (or upgrade):
+AUR](https://aur.archlinux.org/packages/pdfcmd). Python 3.6 or later is
+required. Note [pdfcmd is on PyPI](https://pypi.org/project/pdfcmd/) so
+just ensure that [`pipx`](https://pypa.github.io/pipx/) is installed
+then type the following:
 
 ```
-$ sudo pip3 install -U pdfcmd
+$ pipx install pdfcmd
 ```
 
-Alternatively, do the following to install from the source repository.
-Note that the `python-pypdf` package is required.
+To upgrade:
 
-```sh
-$ git clone http://github.com/bulletmark/pdfcmd
-$ cd pdfcmd
-$ sudo pip3 install -U .
 ```
-
-## UPGRADE
-
-```sh
-$ cd pdfcmd  # Source dir, as above
-$ git pull
-$ sudo pip3 install -U .
-```
-
-## REMOVAL
-
-```sh
-$ sudo pip3 uninstall pdfcmd
+$ pipx upgrade pdfcmd
 ```
 
 ## LICENSE
 
 Copyright (C) 2021 Mark Blakeney. This program is distributed under the
 terms of the GNU General Public License.
 This program is free software: you can redistribute it and/or modify it
```


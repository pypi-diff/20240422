# Comparing `tmp/ptyx_mcq-27.2.0.tar.gz` & `tmp/ptyx_mcq-27.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptyx_mcq-27.2.0.tar", max compression
+gzip compressed data, was "ptyx_mcq-27.3.0.tar", max compression
```

## Comparing `ptyx_mcq-27.2.0.tar` & `ptyx_mcq-27.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1808 2023-03-23 17:40:29.000000 ptyx_mcq-27.2.0/README.md
--rw-r--r--   0        0        0    18095 2022-06-29 17:25:23.274035 ptyx_mcq-27.2.0/ptyx_mcq/TODO.odt
--rw-r--r--   0        0        0     5785 2024-01-30 10:31:19.238333 ptyx_mcq-27.2.0/ptyx_mcq/__init__.py
--rwxr-xr-x   0        0        0    22014 2024-02-16 22:44:56.891990 ptyx_mcq-27.2.0/ptyx_mcq/cli.py
--rwxr-xr-x   0        0        0     4206 2024-02-09 11:30:09.387954 ptyx_mcq-27.2.0/ptyx_mcq/dev_cli.py
--rw-r--r--   0        0        0    73081 2024-01-16 19:05:05.155995 ptyx_mcq-27.2.0/ptyx_mcq/doc/exemple_complet_syntaxe.pdf
--rw-r--r--   0        0        0    10495 2024-01-16 19:05:43.547995 ptyx_mcq-27.2.0/ptyx_mcq/doc/exemple_complet_syntaxe.tex
--rw-r--r--   0        0        0   531437 2023-03-07 21:06:59.000000 ptyx_mcq-27.2.0/ptyx_mcq/dump.profile
--rw-r--r--   0        0        0        0 2022-06-29 17:25:23.290035 ptyx_mcq-27.2.0/ptyx_mcq/make/__init__.py
--rw-r--r--   0        0        0     5666 2024-02-09 11:31:06.831954 ptyx_mcq-27.2.0/ptyx_mcq/make/exercises_parsing.py
--rw-r--r--   0        0        0    29936 2024-03-05 07:52:18.263978 ptyx_mcq-27.2.0/ptyx_mcq/make/extend_latex_generator.py
--rw-r--r--   0        0        0    10413 2024-01-29 22:49:14.366305 ptyx_mcq-27.2.0/ptyx_mcq/make/generate_ptyx_code.py
--rw-r--r--   0        0        0    17770 2024-01-30 13:38:37.318290 ptyx_mcq-27.2.0/ptyx_mcq/make/header.py
--rw-r--r--   0        0        0    18135 2024-02-09 11:31:33.187954 ptyx_mcq-27.2.0/ptyx_mcq/make/include_directives_parsing.py
--rw-r--r--   0        0        0     4701 2024-02-19 21:28:08.691986 ptyx_mcq-27.2.0/ptyx_mcq/make/make.py
--rw-r--r--   0        0        0      983 2024-01-26 14:07:02.095915 ptyx_mcq-27.2.0/ptyx_mcq/make/parser_tools.py
--rw-r--r--   0        0        0      307 2022-07-09 20:44:53.565792 ptyx_mcq-27.2.0/ptyx_mcq/parameters.py
--rw-r--r--   0        0        0        0 2022-07-08 16:36:52.243505 ptyx_mcq-27.2.0/ptyx_mcq/py.typed
--rw-r--r--   0        0        0        0 2022-06-29 17:25:23.306035 ptyx_mcq-27.2.0/ptyx_mcq/scan/__init__.py
--rw-r--r--   0        0        0     8326 2024-01-17 21:53:39.679992 ptyx_mcq-27.2.0/ptyx_mcq/scan/amend.py
--rw-r--r--   0        0        0    27272 2024-02-09 11:26:49.775955 ptyx_mcq-27.2.0/ptyx_mcq/scan/calibration.py
--rw-r--r--   0        0        0     5650 2023-10-22 16:54:09.846269 ptyx_mcq-27.2.0/ptyx_mcq/scan/checkbox_analyzer.py
--rw-r--r--   0        0        0      372 2023-03-13 07:53:49.962584 ptyx_mcq-27.2.0/ptyx_mcq/scan/color.py
--rw-r--r--   0        0        0    21297 2024-02-09 11:28:23.067955 ptyx_mcq-27.2.0/ptyx_mcq/scan/conflict_solver.py
--rw-r--r--   0        0        0    21967 2024-02-09 11:26:16.735955 ptyx_mcq-27.2.0/ptyx_mcq/scan/data_handler.py
--rw-r--r--   0        0        0     2315 2023-12-21 07:31:01.898138 ptyx_mcq-27.2.0/ptyx_mcq/scan/document_data.py
--rw-r--r--   0        0        0    13316 2023-10-22 14:49:01.994227 ptyx_mcq-27.2.0/ptyx_mcq/scan/evaluation_strategies.py
--rw-r--r--   0        0        0     8153 2024-01-21 21:22:33.425900 ptyx_mcq-27.2.0/ptyx_mcq/scan/image_viewer.py
--rw-r--r--   0        0        0     2831 2023-10-15 22:15:25.291988 ptyx_mcq-27.2.0/ptyx_mcq/scan/paths_handler.py
--rw-r--r--   0        0        0     1700 2024-01-26 15:57:12.535890 ptyx_mcq-27.2.0/ptyx_mcq/scan/pdftools.py
--rw-r--r--   0        0        0    11337 2024-02-09 11:29:31.219954 ptyx_mcq-27.2.0/ptyx_mcq/scan/scan_doc.py
--rw-r--r--   0        0        0    16170 2024-02-09 11:26:30.339955 ptyx_mcq-27.2.0/ptyx_mcq/scan/scan_pic.py
--rw-r--r--   0        0        0     7447 2024-02-09 11:28:44.779955 ptyx_mcq-27.2.0/ptyx_mcq/scan/scores_manager.py
--rw-r--r--   0        0        0    11610 2024-01-21 21:41:17.777895 ptyx_mcq-27.2.0/ptyx_mcq/scan/square_detection.py
--rw-r--r--   0        0        0     2600 2023-03-13 07:53:49.978584 ptyx_mcq-27.2.0/ptyx_mcq/scan/tools.py
--rw-r--r--   0        0        0     1947 2024-01-14 22:51:03.455966 ptyx_mcq-27.2.0/ptyx_mcq/scan/types_declaration.py
--rw-r--r--   0        0        0      106 2022-06-30 12:30:07.506267 ptyx_mcq-27.2.0/ptyx_mcq/templates/original/README.txt
--rw-r--r--   0        0        0     1662 2023-04-12 09:58:51.452538 ptyx_mcq-27.2.0/ptyx_mcq/templates/original/new.ptyx
--rw-r--r--   0        0        0     1081 2023-02-25 11:03:57.438687 ptyx_mcq-27.2.0/ptyx_mcq/templates/original/questions/question1.ex
--rw-r--r--   0        0        0      185 2022-06-29 17:25:23.310035 ptyx_mcq-27.2.0/ptyx_mcq/templates/original/questions/question2.ex
--rw-r--r--   0        0        0     1581 2023-03-14 20:28:42.000810 ptyx_mcq-27.2.0/ptyx_mcq/templates/original/questions/question3.ex
--rw-r--r--   0        0        0      953 2023-06-08 21:26:37.795757 ptyx_mcq-27.2.0/ptyx_mcq/templates/original/questions/question4.ex
--rw-r--r--   0        0        0      172 2022-06-30 17:29:40.726022 ptyx_mcq-27.2.0/ptyx_mcq/templates/original/scan/README.txt
--rw-r--r--   0        0        0        0 2022-07-08 16:36:52.299506 ptyx_mcq-27.2.0/ptyx_mcq/tools/__init__.py
--rw-r--r--   0        0        0    14030 2024-01-16 22:25:28.503949 ptyx_mcq-27.2.0/ptyx_mcq/tools/config_parser.py
--rw-r--r--   0        0        0     3359 2023-04-01 14:58:06.224097 ptyx_mcq-27.2.0/ptyx_mcq/tools/extend_literal_eval.py
--rw-r--r--   0        0        0     3072 2024-02-09 11:05:14.959960 ptyx_mcq-27.2.0/ptyx_mcq/tools/io_tools.py
--rw-r--r--   0        0        0     1794 2024-03-05 08:02:50.787975 ptyx_mcq-27.2.0/pyproject.toml
--rw-r--r--   0        0        0     2882 1970-01-01 00:00:00.000000 ptyx_mcq-27.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1808 2023-03-23 17:40:29.000000 ptyx_mcq-27.3.0/README.md
+-rw-r--r--   0        0        0    18095 2022-06-29 17:25:23.274035 ptyx_mcq-27.3.0/ptyx_mcq/TODO.odt
+-rw-r--r--   0        0        0     5785 2024-04-22 08:10:49.665409 ptyx_mcq-27.3.0/ptyx_mcq/__init__.py
+-rwxr-xr-x   0        0        0    22344 2024-04-22 08:10:49.665409 ptyx_mcq-27.3.0/ptyx_mcq/cli.py
+-rwxr-xr-x   0        0        0     4206 2024-04-22 08:10:49.665409 ptyx_mcq-27.3.0/ptyx_mcq/dev_cli.py
+-rw-r--r--   0        0        0    73081 2024-01-16 19:05:05.155995 ptyx_mcq-27.3.0/ptyx_mcq/doc/exemple_complet_syntaxe.pdf
+-rw-r--r--   0        0        0    10495 2024-01-16 19:05:43.547995 ptyx_mcq-27.3.0/ptyx_mcq/doc/exemple_complet_syntaxe.tex
+-rw-r--r--   0        0        0   531437 2023-03-07 21:06:59.000000 ptyx_mcq-27.3.0/ptyx_mcq/dump.profile
+-rw-r--r--   0        0        0        0 2022-06-29 17:25:23.290035 ptyx_mcq-27.3.0/ptyx_mcq/make/__init__.py
+-rw-r--r--   0        0        0     5666 2024-04-22 08:10:49.665409 ptyx_mcq-27.3.0/ptyx_mcq/make/exercises_parsing.py
+-rw-r--r--   0        0        0    30090 2024-04-22 08:10:49.665409 ptyx_mcq-27.3.0/ptyx_mcq/make/extend_latex_generator.py
+-rw-r--r--   0        0        0    10413 2024-04-22 08:10:49.665409 ptyx_mcq-27.3.0/ptyx_mcq/make/generate_ptyx_code.py
+-rw-r--r--   0        0        0    17770 2024-04-22 08:10:49.665409 ptyx_mcq-27.3.0/ptyx_mcq/make/header.py
+-rw-r--r--   0        0        0    18135 2024-04-22 08:10:49.665409 ptyx_mcq-27.3.0/ptyx_mcq/make/include_directives_parsing.py
+-rw-r--r--   0        0        0     5935 2024-04-22 08:10:49.665409 ptyx_mcq-27.3.0/ptyx_mcq/make/make.py
+-rw-r--r--   0        0        0      983 2024-04-22 08:10:49.665409 ptyx_mcq-27.3.0/ptyx_mcq/make/parser_tools.py
+-rw-r--r--   0        0        0      307 2022-07-09 20:44:53.565792 ptyx_mcq-27.3.0/ptyx_mcq/parameters.py
+-rw-r--r--   0        0        0        0 2022-07-08 16:36:52.243505 ptyx_mcq-27.3.0/ptyx_mcq/py.typed
+-rw-r--r--   0        0        0        0 2022-06-29 17:25:23.306035 ptyx_mcq-27.3.0/ptyx_mcq/scan/__init__.py
+-rw-r--r--   0        0        0     8815 2024-04-22 08:10:49.665409 ptyx_mcq-27.3.0/ptyx_mcq/scan/amend.py
+-rw-r--r--   0        0        0    27272 2024-04-22 08:10:49.665409 ptyx_mcq-27.3.0/ptyx_mcq/scan/calibration.py
+-rw-r--r--   0        0        0     5650 2024-04-22 08:03:37.046109 ptyx_mcq-27.3.0/ptyx_mcq/scan/checkbox_analyzer.py
+-rw-r--r--   0        0        0      372 2023-03-13 07:53:49.962584 ptyx_mcq-27.3.0/ptyx_mcq/scan/color.py
+-rw-r--r--   0        0        0    21616 2024-04-22 08:13:43.176007 ptyx_mcq-27.3.0/ptyx_mcq/scan/conflict_solver.py
+-rw-r--r--   0        0        0    22055 2024-04-22 08:10:49.669409 ptyx_mcq-27.3.0/ptyx_mcq/scan/data_handler.py
+-rw-r--r--   0        0        0     2315 2024-04-22 08:03:37.046109 ptyx_mcq-27.3.0/ptyx_mcq/scan/document_data.py
+-rw-r--r--   0        0        0    13316 2023-10-22 14:49:01.994227 ptyx_mcq-27.3.0/ptyx_mcq/scan/evaluation_strategies.py
+-rw-r--r--   0        0        0     8153 2024-04-22 08:10:49.669409 ptyx_mcq-27.3.0/ptyx_mcq/scan/image_viewer.py
+-rw-r--r--   0        0        0     2831 2024-04-22 08:03:37.046109 ptyx_mcq-27.3.0/ptyx_mcq/scan/paths_handler.py
+-rw-r--r--   0        0        0     1798 2024-04-22 08:10:49.669409 ptyx_mcq-27.3.0/ptyx_mcq/scan/pdftools.py
+-rw-r--r--   0        0        0    11337 2024-04-22 08:10:49.669409 ptyx_mcq-27.3.0/ptyx_mcq/scan/scan_doc.py
+-rw-r--r--   0        0        0    16170 2024-04-22 08:10:49.669409 ptyx_mcq-27.3.0/ptyx_mcq/scan/scan_pic.py
+-rw-r--r--   0        0        0     7447 2024-04-22 08:10:49.669409 ptyx_mcq-27.3.0/ptyx_mcq/scan/scores_manager.py
+-rw-r--r--   0        0        0    11610 2024-04-22 08:10:49.669409 ptyx_mcq-27.3.0/ptyx_mcq/scan/square_detection.py
+-rw-r--r--   0        0        0     2600 2023-03-13 07:53:49.978584 ptyx_mcq-27.3.0/ptyx_mcq/scan/tools.py
+-rw-r--r--   0        0        0     1947 2024-04-22 08:10:49.669409 ptyx_mcq-27.3.0/ptyx_mcq/scan/types_declaration.py
+-rw-r--r--   0        0        0      106 2022-06-30 12:30:07.506267 ptyx_mcq-27.3.0/ptyx_mcq/templates/original/README.txt
+-rw-r--r--   0        0        0     1662 2023-04-12 09:58:51.452538 ptyx_mcq-27.3.0/ptyx_mcq/templates/original/new.ptyx
+-rw-r--r--   0        0        0     1081 2023-02-25 11:03:57.438687 ptyx_mcq-27.3.0/ptyx_mcq/templates/original/questions/question1.ex
+-rw-r--r--   0        0        0      185 2022-06-29 17:25:23.310035 ptyx_mcq-27.3.0/ptyx_mcq/templates/original/questions/question2.ex
+-rw-r--r--   0        0        0     1581 2023-03-14 20:28:42.000810 ptyx_mcq-27.3.0/ptyx_mcq/templates/original/questions/question3.ex
+-rw-r--r--   0        0        0      953 2023-06-08 21:26:37.795757 ptyx_mcq-27.3.0/ptyx_mcq/templates/original/questions/question4.ex
+-rw-r--r--   0        0        0      172 2022-06-30 17:29:40.726022 ptyx_mcq-27.3.0/ptyx_mcq/templates/original/scan/README.txt
+-rw-r--r--   0        0        0        0 2022-07-08 16:36:52.299506 ptyx_mcq-27.3.0/ptyx_mcq/tools/__init__.py
+-rw-r--r--   0        0        0    15524 2024-04-22 08:10:49.669409 ptyx_mcq-27.3.0/ptyx_mcq/tools/config_parser.py
+-rw-r--r--   0        0        0     3359 2023-04-01 14:58:06.224097 ptyx_mcq-27.3.0/ptyx_mcq/tools/extend_literal_eval.py
+-rw-r--r--   0        0        0     3072 2024-04-22 08:10:49.669409 ptyx_mcq-27.3.0/ptyx_mcq/tools/io_tools.py
+-rw-r--r--   0        0        0     1789 2024-04-22 08:14:00.028254 ptyx_mcq-27.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2874 1970-01-01 00:00:00.000000 ptyx_mcq-27.3.0/PKG-INFO
```

### Comparing `ptyx_mcq-27.2.0/README.md` & `ptyx_mcq-27.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/TODO.odt` & `ptyx_mcq-27.3.0/ptyx_mcq/TODO.odt`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/__init__.py` & `ptyx_mcq-27.3.0/ptyx_mcq/__init__.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/cli.py` & `ptyx_mcq-27.3.0/ptyx_mcq/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,22 +253,32 @@
         "--shell", type=str, default="bash", choices=("bash", "zsh", "fish")
     )
     install_shell_completion_parser.set_defaults(func=install_shell_completion)
 
     # ------------------------------------------
     argcomplete.autocomplete(parser, always_complete_options=False)
     parsed_args = parser.parse_args(args)
+
     try:
         # Launch the function corresponding to the given subcommand.
         kwargs = vars(parsed_args)
         func = kwargs.pop("func")
     except KeyError:
         # No subcommand passed.
         parser.print_help()
         return
+
+    # Make compilation more reproducible, by disabling PYTHONHASHSEED.
+    if not os.getenv("PYTHONHASHSEED"):
+        os.environ["PYTHONHASHSEED"] = "0"
+        os.execv(sys.executable, [sys.executable] + sys.argv)
+    else:
+        print("PYTHONHASHSEED:", os.getenv("PYTHONHASHSEED"))
+    assert os.getenv("PYTHONHASHSEED")
+
     func(**kwargs)
 
 
 def make(
     path: Path,
     num: int = 1,
     start: int = 1,
```

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/dev_cli.py` & `ptyx_mcq-27.3.0/ptyx_mcq/dev_cli.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/doc/exemple_complet_syntaxe.pdf` & `ptyx_mcq-27.3.0/ptyx_mcq/doc/exemple_complet_syntaxe.pdf`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/doc/exemple_complet_syntaxe.tex` & `ptyx_mcq-27.3.0/ptyx_mcq/doc/exemple_complet_syntaxe.tex`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/dump.profile` & `ptyx_mcq-27.3.0/ptyx_mcq/dump.profile`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/make/exercises_parsing.py` & `ptyx_mcq-27.3.0/ptyx_mcq/make/exercises_parsing.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/make/extend_latex_generator.py` & `ptyx_mcq-27.3.0/ptyx_mcq/make/extend_latex_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,17 @@
     latex_code = re.sub(r" (?=\W)", "", latex_code)
     return latex_code
 
 
 class SameAnswerError(PtyxRuntimeError):
     """Error raised when the same answer appears twice in a question."""
 
-    def __init__(self, *args, answer: str):
+    def __init__(self, *args, answer: str = ""):
+        # Strangely, `answer` parameter must have a default value,
+        # or else this class won't be serializable with pickle.
         super().__init__(*args)
         self.answer = answer
 
 
 # Extend LatexGenerator with new tags.
 
 
@@ -714,15 +716,15 @@
                     print(f"incorrect = {wrong}")
                     print(f"skipped = {skipped}")
                     print(20 * "-")
                 raise NameError(f"Unknown key {key!r} in the header of the pTyX file.")
 
             check_id_or_name = code if not self.WITH_ANSWERS else ""
             self.mcq_cache["check_id_or_name"] = check_id_or_name
-            if check_id_or_name:
+            if check_id_or_name and self.NUM == 1:
                 check_id_or_name += r"""
             \vspace{1em}
 
             \tikz{\draw[dotted] ([xshift=2cm]current page.west) -- ([xshift=-1cm]current page.east);}
             """
 
         header = self.mcq_cache["header"]
```

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/make/generate_ptyx_code.py` & `ptyx_mcq-27.3.0/ptyx_mcq/make/generate_ptyx_code.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/make/header.py` & `ptyx_mcq-27.3.0/ptyx_mcq/make/header.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/make/include_directives_parsing.py` & `ptyx_mcq-27.3.0/ptyx_mcq/make/include_directives_parsing.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/make/make.py` & `ptyx_mcq-27.3.0/ptyx_mcq/make/make.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """
 Generate pdf file from raw mcq file.
 """
 import sys
+import tempfile
 from functools import partial
 from pathlib import Path
 from typing import Any
 
-from ptyx.compilation import make_files
+from ptyx.compilation import make_files, compile_latex_to_pdf
 from ptyx.compilation_options import CompilationOptions
 from ptyx.latex_generator import Compiler
 from ptyx.shell import print_error, print_info
+from ptyx.utilities import force_hardlink_to
 
 from ptyx_mcq.scan.document_data import Page
 from ptyx_mcq.tools.io_tools import get_file_or_sysexit
 from ptyx_mcq.tools.config_parser import Configuration
+from ptyx_mcq.make.exercises_parsing import wrap_exercise
+
+DEFAULT_PTYX_MCQ_COMPILATION_OPTIONS = CompilationOptions(same_number_of_pages_compact=True, compress=True)
 
 
 def generate_config_file(_compiler: Compiler) -> None:
     mcq_data: Configuration = _compiler.latex_generator.mcq_data
     file_path = _compiler.file_path
     assert file_path is not None
     folder = file_path.parent
@@ -47,14 +52,39 @@
                     continue
                 page_, x_, y_ = [s.strip("p() \n") for s in v.split(",")]
                 checkboxes_positions.setdefault(Page(int(page_)), {})[k] = (float(x_), float(y_))
 
     mcq_data.dump(file_path.with_suffix(".ptyx.mcq.config.json"))
 
 
+def compile_exercise_to_latex(path: Path, **context: Any) -> tuple[str, Path]:
+    """Compile an exercise to LaTeX code."""
+    exercise_path = get_file_or_sysexit(path, extension=".ex")
+    print(f"\n == Compiling exercise '{exercise_path}'. == \n")
+    code = wrap_exercise(exercise_path.read_text(encoding="utf8"), exercise_path)
+    context["MCQ_REMOVE_HEADER"] = True
+    context["MCQ_PREVIEW_MODE"] = True
+    print("Temporary pTyX file code:")
+    print("\n" + 5 * "---✂---")
+    print(code)
+    print(5 * "---✂---" + "\n")
+    compiler = Compiler()
+    return compiler.parse(code=code, **context), exercise_path
+
+
+def compile_exercise(path: Path) -> None:
+    """Compile an exercise."""
+    latex, ex_path = compile_exercise_to_latex(path)
+    with tempfile.TemporaryDirectory() as tmpdir:
+        texfile = Path(tmpdir) / ex_path.with_suffix(".tex").name
+        texfile.write_text(latex, encoding="utf8")
+        info = compile_latex_to_pdf(texfile)
+        force_hardlink_to(ex_path.with_suffix(".pdf"), info.dest)
+
+
 def make_command(
     path: Path,
     num: int = 1,
     start: int = 1,
     quiet: bool = False,
     with_correction: bool = False,
     for_review: bool = False,
@@ -94,30 +124,28 @@
             output_basename=f"{ptyx_filename.stem}.review",
             correction=True,
             options=CompilationOptions(context=context | {"PTYX_WITH_ANSWERS": True}, quiet=quiet),
         )
 
     else:
         # Compile and generate output files (tex or pdf)
-        all_info = make(
+        all_info, _ = make(
             ptyx_filename,
             number_of_documents=num,
-            options=CompilationOptions(
-                same_number_of_pages_compact=True, compress=True, start=start, quiet=quiet
-            )
+            options=DEFAULT_PTYX_MCQ_COMPILATION_OPTIONS.updated(start=start, quiet=quiet)
             # cpu_cores=1,
         )
         generate_config_file(compiler)
 
         # Keep track of the seed used.
         seed_value = compiler.seed
         with open(all_info.directory / ".seed", "w") as seed_file:
             seed_file.write(str(seed_value))
 
         if with_correction:
-            corr_info = make(
+            corr_info, _ = make(
                 ptyx_filename,
                 correction=True,
                 doc_ids_selection=all_info.doc_ids,
                 options=CompilationOptions(compress=True, quiet=quiet),
             )
             assert corr_info.doc_ids == all_info.doc_ids, repr((all_info.doc_ids, corr_info.doc_ids))
```

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/make/parser_tools.py` & `ptyx_mcq-27.3.0/ptyx_mcq/make/parser_tools.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/amend.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/amend.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 Created on Thu Aug 29 14:49:37 2019
 
 @author: nicolas
 """
 from collections.abc import Generator
 from itertools import chain
+from multiprocessing import Pool
 from os.path import join
 
 # from typing import TYPE_CHECKING
 
 from PIL import ImageDraw, ImageFont
 from PIL.Image import Image
 from ptyx_mcq.scan.data_handler import DataHandler
@@ -41,19 +42,37 @@
 
     # Global maximal score.
     # Note that the global maximal score can not be easily deduced from the dict `max_score_per_question`,
     # since this dict only include customized questions scores, and since many versions of the same question
     # may appear in the dict, but only one of those versions was included in each generated document.
     max_score = data_storage.config.max_score
     assert isinstance(max_score, (float, int)), repr(max_score)
-    N = len(data_storage.data)
+    number_of_documents = len(data_storage.data)
+    counter = 0
+
+    def print_progression(_):
+        nonlocal counter
+        counter += 1
+        print(f"Generating the amended pdf files: {counter}/{number_of_documents}...", end="\r")
+
+    print(f"Generating the amended pdf files: 0/{number_of_documents}", end="\r")
+    pool = Pool()
     for i, (doc_id, doc_data) in enumerate(data_storage.data.items(), start=1):
-        print(f"Generating the amended pdf files: {i}/{N}...", end="\r")
-        amend_doc(doc_data, doc_id, max_score, max_score_per_question, data_storage)
-    print("Generating the amended pdf files: OK" + len(f"{N}/{N}...") * " ")
+        pool.apply_async(
+            amend_doc,
+            (doc_data, doc_id, max_score, max_score_per_question, data_storage),
+            callback=print_progression,
+        )
+    pool.close()
+    # noinspection PyTestUnpassedFixture
+    pool.join()
+
+    print(
+        "Generating the amended pdf files: OK" + len(f"{number_of_documents}/{number_of_documents}...") * " "
+    )
 
 
 def amend_doc(
     doc_data: DocumentData,
     doc_id: DocumentId,
     max_score: float,
     max_score_per_question: dict[QuestionNumberOrDefault, float],
```

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/calibration.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/calibration.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/checkbox_analyzer.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/checkbox_analyzer.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/conflict_solver.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/conflict_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from ptyx.shell import print_error, print_warning, print_success, print_info
 
 from ptyx_mcq.scan.color import Color, RGB
 from ptyx_mcq.scan.data_handler import DataHandler
 from ptyx_mcq.scan.document_data import Page, DetectionStatus, RevisionStatus, PicData, DocumentData
 from ptyx_mcq.scan.image_viewer import ImageViewer
+from ptyx_mcq.scan.tools import levenshtein_distance
 from ptyx_mcq.tools.config_parser import (
     DocumentId,
     ApparentQuestionNumber,
     apparent2real,
     ApparentAnswerNumber,
     StudentName,
     StudentId,
@@ -152,14 +153,20 @@
                 name = default
             elif id_name_dict:
                 if name in id_name_dict:
                     name, student_id = id_name_dict[StudentId(name)], name
                 elif any((digit in name) for digit in string.digits):
                     # This is not a student name !
                     print("Unknown ID.")
+
+                    def proximity(id_):
+                        return levenshtein_distance(name, id_)
+
+                    suggestion: StudentId = min(id_name_dict, key=proximity)
+                    print(f"Suggestion: {suggestion} ({id_name_dict[suggestion]})")
                     name = ""
             if name:
                 print("Name: %s" % name)
                 if input("Is it correct ? (Y/n)").lower() not in ("y", "yes", ""):
                     name = ""
         assert process is not None
         process.terminate()
```

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/data_handler.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/data_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,17 @@
                 elif number_of_pages(pdfpath) != len(
                     [f for f in folder.iterdir() if f.suffix.lower() in PIC_EXTS]
                 ):
                     # Extraction was probably interrupted
                     rmtree(folder)
                     folder.mkdir()
                     to_extract.append((pdfpath, folder))
-            pool.starmap(extract_pdf_pictures, to_extract)
+            if to_extract:
+                print("Extracting pictures from pdf...")
+                pool.starmap(extract_pdf_pictures, to_extract)
 
     def _remove_obsolete_files(self, hash2pdf: dict[str, Path]) -> None:
         """For each removed pdf files, remove corresponding pictures and data."""
         for path in self.dirs.pic.iterdir():
             if not path.is_dir():
                 raise RuntimeError(
                     f'Folder "{path.parent}" should only contain folders.\n'
```

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/document_data.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/document_data.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/evaluation_strategies.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/evaluation_strategies.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/image_viewer.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/image_viewer.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/paths_handler.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/paths_handler.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/pdftools.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/pdftools.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 from shutil import rmtree
 
 import fitz  # type: ignore
 
 PIC_EXTS = (".jpg", ".jpeg", ".png")
 
 
-def extract_pdf_pictures(pdf_file: Path, dest: Path) -> None:
+def extract_pdf_pictures(pdf_file: Path, dest: Path, verbose=True) -> None:
     """Clear `dest` folder, then extract all pages of the pdf files inside."""
     rmtree(dest, ignore_errors=True)
     dest.mkdir()
 
     page: fitz.Page
     doc = fitz.Document(pdf_file)
+    if verbose:
+        print(f"Extracting pages from '{pdf_file}' as pictures...")
     for i, page in enumerate(doc.pages()):
         # Extract picture if the page contains only a picture (this is quite fast).
         if _contain_only_a_single_image(page):
             xref: int = page.get_images()[0][0]
             img_info = doc.extract_image(xref)
             ext = img_info["ext"].lower()
             if f".{ext}" in PIC_EXTS:
```

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/scan_doc.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/scan_doc.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/scan_pic.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/scan_pic.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/scores_manager.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/scores_manager.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/square_detection.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/square_detection.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/tools.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/tools.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/scan/types_declaration.py` & `ptyx_mcq-27.3.0/ptyx_mcq/scan/types_declaration.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/templates/original/new.ptyx` & `ptyx_mcq-27.3.0/ptyx_mcq/templates/original/new.ptyx`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/templates/original/questions/question1.ex` & `ptyx_mcq-27.3.0/ptyx_mcq/templates/original/questions/question1.ex`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/templates/original/questions/question3.ex` & `ptyx_mcq-27.3.0/ptyx_mcq/templates/original/questions/question3.ex`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/templates/original/questions/question4.ex` & `ptyx_mcq-27.3.0/ptyx_mcq/templates/original/questions/question4.ex`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/tools/config_parser.py` & `ptyx_mcq-27.3.0/ptyx_mcq/tools/config_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from pathlib import Path
 from typing import Any, TypeVar, TypedDict, Literal, NewType, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from ptyx_mcq.scan.document_data import Page
 
 T = TypeVar("T")
+K = TypeVar("K", bound=typing.Hashable)
+V = TypeVar("V")
 
 DocumentId = NewType("DocumentId", int)
 StudentId = NewType("StudentId", str)
 StudentName = NewType("StudentName", str)
 
 OriginalQuestionNumber = NewType("OriginalQuestionNumber", int)
 ApparentQuestionNumber = NewType("ApparentQuestionNumber", int)
@@ -59,14 +61,49 @@
 # "ordering": {},
 # # {NUM: {'questions': [2,1,3...],
 # #        'answers': {1: [(2, True), (1, False), (3, True)...], ...}}, ...}
 # "boxes": {},  # {NUM: {'tag': 'p4, (23.456, 34.667)', ...}, ...}
 # "id_format": None,
 
 
+# @typing.overload
+# def recursively_update_dict(
+#     d1: dict[K, V], d2: dict[K, Any], verify_types: Literal[False], new_key_allowed: bool
+# ) -> None:
+#     """Signature overload when verify_types is False"""
+#
+#
+# @typing.overload
+# def recursively_update_dict(
+#     d1: dict[K, V], d2: dict[K, V], verify_types: Literal[True], new_key_allowed: bool
+# ) -> None:
+#     """Signature overload when verify_types is True"""
+
+
+def recursively_update_dict(
+    d1: dict[K, V], d2: dict[K, V], verify_types: bool = True, new_key_allowed: bool = True
+) -> None:
+    for key in d2:
+        if key not in d1:
+            if not new_key_allowed:
+                raise ValueError(f"Incorrect key: {key!r}.")
+            d1[key] = d2[key]
+        elif isinstance(d1[key], dict) and isinstance(d2[key], dict):
+            recursively_update_dict(
+                d1[key], d2[key], verify_types=verify_types, new_key_allowed=new_key_allowed  # type: ignore
+            )
+        else:
+            if verify_types and key in d1 and not isinstance(d2[key], type(d1[key])):
+                raise ValueError(
+                    f"Incompatible types for key {key!r}: {d1[key]!r} (type: {type(d1[key])})"
+                    f" and {d2[key]!r} (type: {type(d2[key])})."
+                )
+            d1[key] = d2[key]
+
+
 # TODO: improve typing precision
 @dataclass(kw_only=True, slots=True)
 class Configuration:
     mode: dict[QuestionNumberOrDefault, str] = field(default_factory=lambda: {"default": "all"})
     correct: dict[QuestionNumberOrDefault, float] = field(default_factory=lambda: {"default": 1})
     incorrect: dict[QuestionNumberOrDefault, float] = field(default_factory=lambda: {"default": 0})
     skipped: dict[QuestionNumberOrDefault, float] = field(default_factory=lambda: {"default": 0})
@@ -91,17 +128,18 @@
         """Dump `cfg` dict to `path` as json."""
         with open(path, "w") as f:
             f.write(encode2js(self.as_dict(), formatter=(lambda s: s.upper().center(40, "-"))))
 
     def as_dict(self):
         return asdict(self)
 
-    #
-    # def update(self, d:dict[str, Any]) -> None:
-    #     self.__dict__.update(d)
+    def updated_copy(self, d: dict[str, Any]) -> "Configuration":
+        original_dict = self.as_dict()
+        recursively_update_dict(original_dict, d, verify_types=False)
+        return Configuration(**original_dict)
 
     @classmethod
     def load(cls, path: Path | str) -> "Configuration":
         """Load `path` configuration file (json) and return a dict."""
         with open(path) as f:
             js = f.read()
         try:
```

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/tools/extend_literal_eval.py` & `ptyx_mcq-27.3.0/ptyx_mcq/tools/extend_literal_eval.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/ptyx_mcq/tools/io_tools.py` & `ptyx_mcq-27.3.0/ptyx_mcq/tools/io_tools.py`

 * *Files identical despite different names*

### Comparing `ptyx_mcq-27.2.0/pyproject.toml` & `ptyx_mcq-27.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptyx-mcq"
-version = "27.2.0"
+version = "27.3.0"
 description = "pTyX-MCQ is a generator/scanner of MCQ, based on pTyX."
 authors = ["Nicolas Pourcelot <nicolas.pourcelot@gmail.com>"]
 repository = "https://github.com/wxgeo/ptyx"
 license = "GPL-3.0-or-later"
 readme = "README.md"
 keywords = ["python", "tikz", "latex", "pdf", "exam", "mcq", "student"]
 
@@ -12,26 +12,26 @@
 python = "^3.10"
 numpy = "^1.23.0"
 Pillow = "^9.2"
 sympy = "~1.11"
 pymupdf = "^1.21.1"
 ptyx = "^28.2"
 smallgraphlib = "^0.7"
-platformdirs = "^3.2.0"
+platformdirs = "^4"
 openpyxl = "^3.1.2"
 argcomplete = "^3.1.2"
 
 
 [tool.poetry.group.dev.dependencies]
 types-openpyxl = "^3.1.0.12"
 types-Pillow = "^9.0.20"
 pytest = "^7"
 mypy = "^1.0"
 black = "^23.3.0"
-tox = "^4.1.2"
+tox = "^4.14"
 sphinx-autodoc-typehints = "^1.18.3"
 sphinx-rtd-theme = "^1.0.0"#
 myst-parser = "^1.0.0"
 # Version 7.29+ are buggy !
 python-semantic-release = "7.28.1"
 ptyx = {path = "../ptyx", develop = true}
 ruff = "^0.2.1"
```

### Comparing `ptyx_mcq-27.2.0/PKG-INFO` & `ptyx_mcq-27.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptyx-mcq
-Version: 27.2.0
+Version: 27.3.0
 Summary: pTyX-MCQ is a generator/scanner of MCQ, based on pTyX.
 Home-page: https://github.com/wxgeo/ptyx
 License: GPL-3.0-or-later
 Keywords: python,tikz,latex,pdf,exam,mcq,student
 Author: Nicolas Pourcelot
 Author-email: nicolas.pourcelot@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Pillow (>=9.2,<10.0)
 Requires-Dist: argcomplete (>=3.1.2,<4.0.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
-Requires-Dist: platformdirs (>=3.2.0,<4.0.0)
+Requires-Dist: platformdirs (>=4,<5)
 Requires-Dist: ptyx (>=28.2,<29.0)
 Requires-Dist: pymupdf (>=1.21.1,<2.0.0)
 Requires-Dist: smallgraphlib (>=0.7,<0.8)
 Requires-Dist: sympy (>=1.11,<1.12)
 Project-URL: Repository, https://github.com/wxgeo/ptyx
 Description-Content-Type: text/markdown
```


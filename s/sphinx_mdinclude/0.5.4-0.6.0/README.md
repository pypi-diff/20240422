# Comparing `tmp/sphinx_mdinclude-0.5.4.tar.gz` & `tmp/sphinx_mdinclude-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_mdinclude-0.5.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_mdinclude-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_mdinclude-0.5.4.tar` & `sphinx_mdinclude-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0      180 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/.flake8
--rw-r--r--   0        0        0      207 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/.github/dependabot.yml
--rw-r--r--   0        0        0      139 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/.github/issue_template.md
--rw-r--r--   0        0        0       61 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/.github/pull_request_template.md
--rw-r--r--   0        0        0      682 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/.github/workflows/build.yml
--rw-r--r--   0        0        0     1091 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/.gitignore
--rw-r--r--   0        0        0       50 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/.mailmap
--rw-r--r--   0        0        0      194 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/.readthedocs.yml
--rw-r--r--   0        0        0     6845 2024-04-19 06:14:55.165367 sphinx_mdinclude-0.5.4/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/LICENSE
--rw-r--r--   0        0        0     3026 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/README.md
--rw-r--r--   0        0        0      598 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/docs/_static/custom.css
--rw-r--r--   0        0        0    42080 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/docs/_static/omnilib.png
--rw-r--r--   0        0        0      342 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/docs/_templates/badges.html
--rw-r--r--   0        0        0     1145 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/docs/_templates/omnilib.html
--rw-r--r--   0        0        0       71 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/docs/changelog.rst
--rw-r--r--   0        0        0     2703 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/docs/conf.py
--rw-r--r--   0        0        0     2988 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/docs/example.md
--rw-r--r--   0        0        0       51 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/docs/included.md
--rw-r--r--   0        0        0       99 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/docs/index.md
--rw-r--r--   0        0        0      812 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/makefile
--rw-r--r--   0        0        0     1806 2024-04-19 06:09:05.540177 sphinx_mdinclude-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      310 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/sphinx_mdinclude/__init__.py
--rw-r--r--   0        0        0      156 2024-04-19 06:14:55.169367 sphinx_mdinclude-0.5.4/sphinx_mdinclude/__version__.py
--rw-r--r--   0        0        0    15230 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/sphinx_mdinclude/legacy.py
--rw-r--r--   0        0        0     3514 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/sphinx_mdinclude/parse.py
--rw-r--r--   0        0        0     9691 2024-04-19 04:44:52.358949 sphinx_mdinclude-0.5.4/sphinx_mdinclude/render.py
--rw-r--r--   0        0        0     5086 2024-04-19 05:15:04.198993 sphinx_mdinclude-0.5.4/sphinx_mdinclude/sphinx.py
--rw-r--r--   0        0        0      280 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/__init__.py
--rw-r--r--   0        0        0      167 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/__main__.py
--rw-r--r--   0        0        0      357 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/test.md
--rw-r--r--   0        0        0      419 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/test.rst
--rw-r--r--   0        0        0    22034 2024-04-19 04:44:52.362949 sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/test_renderer.py
--rw-r--r--   0        0        0     2105 2024-04-19 04:56:45.641861 sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/test_smoke.py
--rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 sphinx_mdinclude-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      180 2024-04-21 05:12:02.608182 sphinx_mdinclude-0.6.0/.flake8
+-rw-r--r--   0        0        0      207 2024-04-21 05:13:19.859896 sphinx_mdinclude-0.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      139 2024-04-21 05:12:02.608456 sphinx_mdinclude-0.6.0/.github/issue_template.md
+-rw-r--r--   0        0        0       61 2024-04-21 05:12:02.608551 sphinx_mdinclude-0.6.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      682 2024-04-22 03:04:23.203972 sphinx_mdinclude-0.6.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1091 2024-04-21 05:12:02.608833 sphinx_mdinclude-0.6.0/.gitignore
+-rw-r--r--   0        0        0       50 2024-04-21 05:13:19.860138 sphinx_mdinclude-0.6.0/.mailmap
+-rw-r--r--   0        0        0      194 2024-04-21 05:13:19.860231 sphinx_mdinclude-0.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0     7240 2024-04-22 04:15:31.799081 sphinx_mdinclude-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2024-04-21 05:12:02.609184 sphinx_mdinclude-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3026 2024-04-21 05:13:19.860494 sphinx_mdinclude-0.6.0/README.md
+-rw-r--r--   0        0        0      598 2024-04-21 05:13:19.860593 sphinx_mdinclude-0.6.0/docs/_static/custom.css
+-rw-r--r--   0        0        0    42080 2024-04-21 05:13:19.860779 sphinx_mdinclude-0.6.0/docs/_static/omnilib.png
+-rw-r--r--   0        0        0      342 2024-04-21 05:12:02.609680 sphinx_mdinclude-0.6.0/docs/_templates/badges.html
+-rw-r--r--   0        0        0     1145 2024-04-21 05:13:19.860912 sphinx_mdinclude-0.6.0/docs/_templates/omnilib.html
+-rw-r--r--   0        0        0       71 2024-04-21 05:12:02.609868 sphinx_mdinclude-0.6.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2703 2024-04-21 05:13:19.861006 sphinx_mdinclude-0.6.0/docs/conf.py
+-rw-r--r--   0        0        0     2991 2024-04-22 03:04:23.205071 sphinx_mdinclude-0.6.0/docs/example.md
+-rw-r--r--   0        0        0       51 2024-04-21 05:12:02.610170 sphinx_mdinclude-0.6.0/docs/included.md
+-rw-r--r--   0        0        0       99 2024-04-21 05:12:02.610262 sphinx_mdinclude-0.6.0/docs/index.md
+-rw-r--r--   0        0        0      812 2024-04-22 03:04:23.205541 sphinx_mdinclude-0.6.0/makefile
+-rw-r--r--   0        0        0     1841 2024-04-22 04:13:12.002236 sphinx_mdinclude-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      310 2024-04-21 05:12:02.610809 sphinx_mdinclude-0.6.0/sphinx_mdinclude/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-22 04:15:31.808781 sphinx_mdinclude-0.6.0/sphinx_mdinclude/__version__.py
+-rw-r--r--   0        0        0     3473 2024-04-22 04:13:12.002541 sphinx_mdinclude-0.6.0/sphinx_mdinclude/parse.py
+-rw-r--r--   0        0        0    12736 2024-04-22 04:13:12.003277 sphinx_mdinclude-0.6.0/sphinx_mdinclude/render.py
+-rw-r--r--   0        0        0     5144 2024-04-22 04:13:12.003530 sphinx_mdinclude-0.6.0/sphinx_mdinclude/sphinx.py
+-rw-r--r--   0        0        0      280 2024-04-22 03:04:23.207825 sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-22 03:04:23.208071 sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/__main__.py
+-rw-r--r--   0        0        0      357 2024-04-22 03:04:23.208341 sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/test.md
+-rw-r--r--   0        0        0      419 2024-04-22 03:04:23.208723 sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/test.rst
+-rw-r--r--   0        0        0    24025 2024-04-22 04:13:12.003836 sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/test_renderer.py
+-rw-r--r--   0        0        0     2121 2024-04-22 04:13:12.004172 sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/test_smoke.py
+-rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 sphinx_mdinclude-0.6.0/PKG-INFO
```

### Comparing `sphinx_mdinclude-0.5.4/.github/workflows/build.yml` & `sphinx_mdinclude-0.6.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.4/.gitignore` & `sphinx_mdinclude-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.4/CHANGELOG.md` & `sphinx_mdinclude-0.6.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 sphinx-mdinclude
 ================
 
 [![Generated by attribution][attribution-badge]][attribution-url]
 
 
+v0.6.0
+------
+
+Feature release
+
+- Added support for mistune v3, dropped support for mistune v2 (#22, #46)
+- Added strict type annotations and type checking (#62)
+- Cleaned up legacy implementation from m2r (#58)
+
+Many thanks to Julian Gilbey for the help upgrading to mistune v3!
+
+```text
+$ git shortlog -s v0.5.4...v0.6.0
+     3	Amethyst Reese
+     1	Julian Gilbey
+     3	dependabot[bot]
+```
+
+
 v0.5.4
 ------
 
 Maintenance release
 
 - Better testing of sphinx extension and docutils directive (#48)
 - Support fixes for docutils v0.21 (#55)
```

### Comparing `sphinx_mdinclude-0.5.4/LICENSE` & `sphinx_mdinclude-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.4/README.md` & `sphinx_mdinclude-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.4/docs/_static/custom.css` & `sphinx_mdinclude-0.6.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.4/docs/_static/omnilib.png` & `sphinx_mdinclude-0.6.0/docs/_static/omnilib.png`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.4/docs/_templates/omnilib.html` & `sphinx_mdinclude-0.6.0/docs/_templates/omnilib.html`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.4/docs/conf.py` & `sphinx_mdinclude-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.4/docs/example.md` & `sphinx_mdinclude-0.6.0/docs/example.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 This page is written in mixed markdown and reST.
 Source code is [here](https://github.com/omnilib/sphinx-mdinclude/raw/main/docs/example.md).
 
 ## Basic Markups (inline)
 
 A **strong**, *emphasis*, ~~deleted~~, `code with single-backtick`,
 ``code with two-backticks``, ```code can include multiple (``) backticks```,
-:code:`reST's code role`, and <del>inline html</del>delete.
+:code:`reST's code role`, and <del>inline html</del> delete.
 
 ### Link
 
-Auto link to http://example.com/.
+Auto link to <http://example.com/>.
 
 Link to [example.com](http://example.com/) in markdown.
 
 Link to [anchor](#testlabel) in markdown.
 
 Link to `example.com <http://example.com/>`_ in reST.
```

### Comparing `sphinx_mdinclude-0.5.4/makefile` & `sphinx_mdinclude-0.6.0/makefile`

 * *Files identical despite different names*

### Comparing `sphinx_mdinclude-0.5.4/pyproject.toml` & `sphinx_mdinclude-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -21,35 +21,35 @@
     "Natural Language :: English",
     "Topic :: Text Processing",
 ]
 keywords = ["Markdown", "reStructuredText", "sphinx-extension"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 dependencies = [
-    "mistune >=2.0,<3.0",
+    "mistune >=3.0,<4.0",
     "docutils >=0.16,<1.0",
     "pygments >= 2.8",
 ]
 
 [project.optional-dependencies]
 dev = [
     "docutils==0.20.1; python_version < '3.9'",
     "docutils==0.21.1; python_version >= '3.9'",
-    "mistune==2.0.4",
+    "mistune==3.0.2",
 
-    "attribution==1.6.2",
+    "attribution==1.7.1",
     "black==24.4.0",
-    "coverage==7.3.2",
+    "coverage==7.4.4",
     "flake8==7.0.0",
     "flit==3.9.0",
     "mypy==1.9.0",
     "sphinx==7.1.2; python_version < '3.9'",
     "sphinx==7.3.7; python_version >= '3.9'",
     "ufmt==2.5.1",
-    "usort==1.0.7",
+    "usort==1.0.8.post1",
 ]
 
 [project.urls]
 Github = "https://github.com/omnilib/sphinx-mdinclude"
 
 
 [tool.attribution]
@@ -68,9 +68,10 @@
 fail_under = 50
 precision = 1
 show_missing = true
 skip_covered = true
 
 [tool.mypy]
 python_version = "3.8"
-# strict = true
+strict = true
 ignore_missing_imports = true
+disallow_untyped_calls = false
```

### Comparing `sphinx_mdinclude-0.5.4/sphinx_mdinclude/render.py` & `sphinx_mdinclude-0.6.0/sphinx_mdinclude/render.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import re
 import textwrap
 from functools import partial
+from importlib import import_module
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple
 
 from docutils.utils import column_width
 from mistune import Markdown
-from mistune.plugins import PLUGINS
-from mistune.renderers import BaseRenderer
+from mistune.core import BaseRenderer, BlockState
+from mistune.plugins import _plugins
 
 from .parse import RestBlockParser, RestInlineParser
 
+CACHED_MODULES: Dict[str, Any] = {}
 DEFAULT_PLUGINS = ["strikethrough", "footnotes", "table"]
 
 PROLOG = """\
 .. role:: raw-html-md(raw)
    :format: html
 
 """
@@ -27,306 +30,371 @@
         2: "-",
         3: "^",
         4: "~",
         5: '"',
         6: "#",
     }
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         self._indent_block = partial(textwrap.indent, prefix=self.indent)
         super().__init__(*args, **kwargs)
 
-    def finalize(self, data):
+    def render_token(self, token: Dict[str, Any], state: BlockState) -> str:
+        # based on mistune 3.0.2, mistune/renderers/html.py
+        func: Callable[..., str] = self._get_method(token["type"])
+        attrs = token.get("attrs")
+        style = token.get("style")
+
+        if "raw" in token:
+            text = token["raw"]
+        elif "children" in token:
+            text = self.render_tokens(token["children"], state)
+        else:
+            if attrs:
+                return func(**attrs)
+            else:
+                return func()
+
+        # We have to special-case block_code, as it needs to know the
+        # style as well to determine whether to add a blank line at the
+        # end (so as to retain the original behaviour)
+        if token["type"] == "block_code":
+            if attrs:
+                return func(text, style=style, **attrs)
+            else:
+                return func(text, style=style)
+
+        if attrs:
+            return func(text, **attrs)
+        else:
+            return func(text)
+
+    def finalize(self, data: Iterable[str]) -> str:
         return "".join(data)
 
-    def _raw_html(self, html):
+    def _raw_html(self, html: str) -> str:
         self._include_raw_html = True
         return r":raw-html-md:`{}`".format(html)
 
-    def block_code(self, code, lang=None):
-        if lang == "math":
+    def block_code(self, code: str, style: str, info: Optional[str] = None) -> str:
+        if info == "math":
             first_line = "\n.. math::\n\n"
-        elif lang:
-            first_line = "\n.. code-block:: {}\n\n".format(lang)
+        elif info:
+            first_line = "\n.. code-block:: {}\n\n".format(info)
         else:
             # first_line = "\n::\n\n"
             first_line = "\n.. code-block::\n\n"
-        return first_line + self._indent_block(code)
+        newline = "\n" if style == "indent" else ""
+        return first_line + self._indent_block(code + newline)
 
-    def block_quote(self, text):
+    def block_quote(self, text: str) -> str:
         # text includes some empty line
         return "\n..\n\n{}\n\n".format(self._indent_block(text.strip("\n")))
 
-    def block_text(self, text):
+    def block_text(self, text: str) -> str:
         return text
 
-    def block_html(self, html):
+    def block_html(self, html: str) -> str:
         """Rendering block level pure html content.
 
         :param html: text content of the html snippet.
         """
-        return "\n\n.. raw:: html\n\n" + self._indent_block(html) + "\n\n"
+        return "\n\n.. raw:: html\n\n" + self._indent_block(html) + "\n"
 
-    def heading(self, text, level, raw=None):
+    def heading(self, text: str, level: int, **attrs: Any) -> str:
         """Rendering header/heading tags like ``<h1>`` ``<h2>``.
 
         :param text: rendered text content for the header.
         :param level: a number for the header level, for example: 1.
-        :param raw: raw text content of the header.
+        :param attrs: other attributes of the header.
         """
         return "\n{0}\n{1}\n".format(text, self.hmarks[level] * column_width(text))
 
-    def thematic_break(self):
+    def thematic_break(self) -> str:
         """Rendering method for ``<hr>`` tag."""
         return "\n----\n"
 
-    def list(self, body, ordered, level, start):
+    def list(self, text: str, ordered: bool, **attrs: Any) -> str:
         """Rendering list tags like ``<ul>`` and ``<ol>``.
 
-        :param body: body contents of the list.
+        :param text: body contents of the list.
         :param ordered: whether this list is ordered or not.
+        :param attrs: other attributes of the list.
         """
         mark = "#. " if ordered else "* "
-        lines = body.splitlines()
+        lines = text.splitlines()
         for i, line in enumerate(lines):
             if line and not line.startswith(self.list_marker):
                 lines[i] = " " * len(mark) + line
         result = "\n{}\n".format("\n".join(lines)).replace(self.list_marker, mark)
         return result
 
-    def list_item(self, text, level):
+    def list_item(self, text: str) -> str:
         """Rendering list item snippet. Like ``<li>``."""
         return "\n" + self.list_marker + text
 
-    def paragraph(self, text):
+    def paragraph(self, text: str) -> str:
         """Rendering paragraph tags. Like ``<p>``."""
         return "\n" + text + "\n"
 
-    def table(self, body):
+    def table(self, body: str) -> str:
         """Rendering table element. Wrap header and body in it.
 
         :param header: header part of the table.
         :param body: body part of the table.
         """
         table = "\n.. list-table::\n"
         table = table + self._indent_block(body) + "\n"
         return table
 
-    def table_head(self, text):
+    def table_head(self, text: str) -> str:
         return ":header-rows: 1\n\n" + self.table_row(text)
 
-    def table_body(self, text):
+    def table_body(self, text: str) -> str:
         return text
 
-    def table_row(self, content):
+    def table_row(self, content: str) -> str:
         """Rendering a table row. Like ``<tr>``.
 
         :param content: content of current table row.
         """
         contents = content.splitlines()
         if not contents:
             return ""
         clist = ["* " + contents[0]]
         if len(contents) > 1:
             for c in contents[1:]:
                 clist.append("  " + c)
         return "\n".join(clist) + "\n"
 
-    def table_cell(self, content, align=None, is_head=False):
+    def table_cell(self, content: str, align: None = None, head: bool = False) -> str:
         """Rendering a table cell. Like ``<th>`` ``<td>``.
 
         :param content: content of current table cell.
-        :param header: whether this is header or not.
         :param align: align of current table cell.
+        :param head: whether this is header or not.
         """
         return "- " + content + "\n"
 
-    def double_emphasis(self, text):
+    def double_emphasis(self, text: str) -> str:
         """Rendering **strong** text.
 
         :param text: text content for emphasis.
         """
         return r"**{}**".format(text)
 
-    def emphasis(self, text):
+    def emphasis(self, text: str) -> str:
         """Rendering *emphasis* text.
 
         :param text: text content for emphasis.
         """
         return r"*{}*".format(text)
 
-    def strong(self, text):
+    def strong(self, text: str) -> str:
         return r"**{}**".format(text)
 
-    def codespan(self, text):
+    def codespan(self, text: str) -> str:
         """Rendering inline `code` text.
 
         :param text: text content for inline code.
         """
-        if "``" not in text:
-            return r"``{}``".format(text)
-        else:
+        cannot_inline = "``" in text or text[0] in [" ", "`"] or text[-1] in [" ", "`"]
+        if cannot_inline:
             # actually, docutils split spaces in literal
             return self._raw_html(
                 '<code class="docutils literal">'
                 '<span class="pre">{}</span>'
                 "</code>".format(text.replace("`", "&#96;"))
             )
+        else:
+            return r"``{}``".format(text)
 
-    def linebreak(self):
+    def linebreak(self) -> str:
         """Rendering line break like ``<br>``."""
         return " " + self._raw_html("<br />") + "\n"
 
-    def strikethrough(self, text):
+    def softbreak(self) -> str:
+        """Rendering soft line break."""
+        return "\n"
+
+    def strikethrough(self, text: str) -> str:
         """Rendering ~~strikethrough~~ text.
 
         :param text: text content for strikethrough.
         """
         return self._raw_html("<del>{}</del>".format(text))
 
-    def text(self, text):
+    def text(self, text: str) -> str:
         """Rendering unformatted text.
 
         :param text: text content.
         """
         return text
 
-    def link(self, link, text, title=None):
+    def link(self, text: str, url: str, title: Optional[str] = None) -> str:
         """Rendering a given link with content and title.
 
-        :param link: href link for ``<a>`` tag.
-        :param title: title content for `title` attribute.
         :param text: text content for description.
+        :param url: URL for ``<a>`` tag.
+        :param title: title content for `title` attribute.
         """
         if text.startswith("\n.. image::"):
-            text = re.sub(r":target: (.*)\n", f":target: {link}\n", text)
+            text = re.sub(r":target: (.*)\n", f":target: {url}\n", text)
             return text
 
         underscore = "_"
         if title:
             return self._raw_html(
-                '<a href="{link}" title="{title}">{text}</a>'.format(
-                    link=link, title=title, text=text
+                '<a href="{url}" title="{title}">{text}</a>'.format(
+                    url=url, title=title, text=text
                 )
             )
-        if link.startswith("#"):
-            target = link[1:]
+        if url.startswith("#"):
+            target = url[1:]
             return r":ref:`{text} <{target}>`".format(target=target, text=text)
 
         return r"`{text} <{target}>`{underscore}".format(
-            target=link, text=text, underscore=underscore
+            target=url, text=text, underscore=underscore
         )
 
-    def image(self, src, alt, title):
+    def image(self, text: str, url: str, title: Optional[str] = None) -> str:
         """Rendering a image with title and text.
 
-        :param src: source link of the image.
-        :param title: title text of the image.
         :param text: alt text of the image.
+        :param url: source link of the image.
+        :param title: title text of the image.
         """
         # rst does not support title option
         # and I couldn't find title attribute in HTML standard
         return "\n".join(
             [
                 "",
-                ".. image:: {}".format(src),
-                "   :target: {}".format(src),
-                "   :alt: {}".format(alt),
+                ".. image:: {}".format(url),
+                "   :target: {}".format(url),
+                "   :alt: {}".format(text),
                 "",
             ]
         )
 
-    def image_link(self, url, target, alt):
+    def image_link(self, url: str, target: str, alt: str) -> str:
         return "\n".join(
             [
                 "",
                 ".. image:: {}".format(url),
                 "   :target: {}".format(target),
                 "   :alt: {}".format(alt),
                 "",
             ]
         )
 
-    def inline_html(self, html):
+    def inline_html(self, html: str) -> str:
         """Rendering span level pure html content.
 
         :param html: text content of the html snippet.
         """
         return self._raw_html(html)
 
-    def newline(self):
+    def newline(self) -> str:
         """Rendering newline element."""
         return ""
 
-    def footnote_ref(self, key, index):
+    def footnote_ref(self, key: str, index: int) -> str:
         """Rendering the ref anchor of a footnote.
 
         :param key: identity key for the footnote.
         :param index: the index count of current footnote.
         """
         return r"[#fn-{}]_".format(key)
 
-    def footnote_item(self, text, key, index):
+    def footnote_item(self, text: str, key: str, index: int) -> str:
         """Rendering a footnote item.
 
         :param key: identity key for the footnote.
         :param text: text content of the footnote.
         """
         return ".. [#fn-{0}] {1}\n".format(key, text.strip())
 
-    def footnotes(self, text):
+    def footnotes(self, text: str) -> str:
         """Wrapper for all footnotes.
 
         :param text: contents of all footnotes.
         """
         if text:
             return "\n\n" + text
         else:
             return ""
 
     """Below outputs are for rst."""
 
-    def rest_role(self, text):
-        return text
+    def rest_role(self, raw: str) -> str:
+        return raw
 
-    def rest_link(self, text):
-        return text
+    def rest_link(self, raw: str) -> str:
+        return raw
 
-    def inline_math(self, math):
+    def inline_math(self, raw: str) -> str:
         """Extension of recommonmark."""
-        return r":math:`{}`".format(math)
+        return r":math:`{}`".format(raw)
 
-    def eol_literal_marker(self, marker):
+    def eol_literal_marker(self, raw: str) -> str:
         """Extension of recommonmark."""
-        return marker
+        return raw
 
-    def directive(self, text):
+    def directive(self, text: str) -> str:
         return "\n" + text
 
-    def rest_code_block(self, text):
+    def rest_code_block(self, text: str) -> str:
         return "\n\n"
 
+    def blank_line(self) -> str:
+        return ""
+
 
 class RestMarkdown(Markdown):
-    def __init__(self, renderer=None, block=None, inline=None, plugins=None, **kwargs):
+    def __init__(
+        self,
+        renderer: Optional[BaseRenderer] = None,
+        block: Optional[RestBlockParser] = None,
+        inline: Optional[RestInlineParser] = None,
+        plugins: Optional[List[Any]] = None,
+        **kwargs: Any,
+    ) -> None:
         renderer = renderer or RestRenderer()
         block = block or RestBlockParser()
-        inline = inline or RestInlineParser(renderer)
-        plugins = plugins or [PLUGINS[p] for p in DEFAULT_PLUGINS]
+        inline = inline or RestInlineParser()
+        plugins_str = plugins or [_plugins[p] for p in DEFAULT_PLUGINS]
+        plugins = []
+        for plugin_str in plugins_str:
+            if plugin_str in CACHED_MODULES:
+                plugins.append(CACHED_MODULES[plugin_str])
+            else:
+                if isinstance(plugin_str, str):
+                    module_path, func_name = plugin_str.rsplit(".", 1)
+                    module = import_module(module_path)
+                    plugin = getattr(module, func_name)
+                else:
+                    # Presumably a function has been passed
+                    plugin = plugin_str
+                CACHED_MODULES[plugin_str] = plugin
+                plugins.append(plugin)
 
         super().__init__(renderer, block=block, inline=inline, plugins=plugins)
 
-    def parse(self, text):
-        output = super().parse(text)
+    def parse(
+        self,
+        text: str,
+        state: Optional[BlockState] = None,
+    ) -> Tuple[str, Optional[BlockState]]:
+        output, state = super().parse(text)
         output = self.post_process(output)
 
-        return output
+        return output, state
 
-    def post_process(self, text):
+    def post_process(self, text: str) -> str:
         if self.renderer._include_raw_html:
             return PROLOG + text
         else:
             return text
 
 
-def convert(text, **kwargs):
-    return RestMarkdown(**kwargs)(text)
+def convert(text: str, **kwargs: Any) -> str:
+    return str(RestMarkdown(**kwargs)(text))
```

### Comparing `sphinx_mdinclude-0.5.4/sphinx_mdinclude/sphinx.py` & `sphinx_mdinclude-0.6.0/sphinx_mdinclude/sphinx.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 """
 Sphinx extension
 """
 
 import os
 import os.path
+from typing import Any, Dict, List, Union
 
 from docutils import io, statemachine, utils
+from docutils.io import error_string as ErrorString
+from docutils.nodes import document as Document
 from docutils.parsers import rst
 from docutils.parsers.rst import directives as rst_directives
-
-try:  # new
-    from docutils.io import (  # type: ignore  # typeshed  #8716
-        error_string as ErrorString,
-    )
-
-    SafeString = str
-except ImportError:  # old
-    from docutils.core import ErrorString  # type: ignore
-    from docutils.utils import SafeString  # type: ignore
+from sphinx.application import Sphinx
 
 from . import RestMarkdown
-
 from .__version__ import __version__
 
 
 class MdIncludeParser(rst.Parser, object):
     # Explicitly tell supported formats to sphinx
     supported = ("markdown", "md", "mkd")
 
-    def parse(self, inputstrings, document):
+    def parse(
+        self,
+        inputstrings: Union[str, statemachine.StringList],
+        document: Document,
+    ) -> None:
         if isinstance(inputstrings, statemachine.StringList):
             inputstring = "\n".join(inputstrings)
         else:
             inputstring = inputstrings
         config = document.settings.env.config
         converter = RestMarkdown(
             no_underscore_emphasis=config.no_underscore_emphasis,
@@ -53,15 +50,15 @@
     required_arguments = 1
     optional_arguments = 0
     option_spec = {
         "start-line": int,
         "end-line": int,
     }
 
-    def run(self):
+    def run(self) -> List[Any]:
         """Most of this method is from ``docutils.parser.rst.Directive``.
 
         docutils version: 0.12
         """
         if not self.state.document.settings.file_insertion_enabled:
             raise self.warning('"%s" directive disabled.' % self.name)
         source = self.state_machine.input_lines.source(
@@ -88,15 +85,15 @@
             include_file = io.FileInput(
                 source_path=path, encoding=encoding, error_handler=e_handler
             )
         except UnicodeEncodeError:
             raise self.severe(
                 'Problems with "%s" directive path:\n'
                 'Cannot encode input file path "%s" '
-                "(wrong locale?)." % (self.name, SafeString(path))
+                "(wrong locale?)." % (self.name, str(path))
             )
         except IOError as error:
             raise self.severe(
                 'Problems with "%s" directive path:\n%s.'
                 % (self.name, ErrorString(error))
             )
 
@@ -124,22 +121,22 @@
         include_lines = statemachine.string2lines(
             converter(rawtext), tab_width, convert_whitespace=True
         )
         self.state_machine.insert_input(include_lines, path)
         return []
 
 
-def setup(app):
+def setup(app: Sphinx) -> Dict[str, Union[str, bool]]:
     """When used for sphinx extension."""
     app.add_config_value("no_underscore_emphasis", False, "env")
     app.add_config_value("md_parse_relative_links", False, "env")
     app.add_config_value("md_anonymous_references", False, "env")
     app.add_config_value("md_disable_inline_math", False, "env")
     app.add_source_suffix(".md", "markdown")
     app.add_source_parser(MdIncludeParser)
     app.add_directive("mdinclude", MdInclude)
-    metadata = dict(
-        version=__version__,
-        parallel_read_safe=True,
-        parallel_write_safe=True,
-    )
+    metadata: Dict[str, Union[str, bool]] = {
+        "version": __version__,
+        "parallel_read_safe": True,
+        "parallel_write_safe": True,
+    }
     return metadata
```

### Comparing `sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/test_renderer.py` & `sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/test_renderer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+from typing import Any, Tuple
 from unittest import skip, TestCase
 
 from docutils import io
 from docutils.core import Publisher
 
 from ..render import convert, PROLOG
 
 
 class RendererTestBase(TestCase):
-    def conv(self, src, **kwargs):
+    def conv(self, src: str, **kwargs: Any) -> str:
         out = convert(src, **kwargs)
         self.check_rst(out)
         return out
 
-    def conv_no_check(self, src, **kwargs):
+    def conv_no_check(self, src: str, **kwargs: Any) -> str:
         out = convert(src, **kwargs)
         return out
 
-    def check_rst(self, rst):
+    def check_rst(self, rst: str) -> Tuple[str, Publisher]:
         pub = Publisher(
             reader=None,
             parser=None,
             writer=None,
             settings=None,
             source_class=io.StringInput,
             destination_class=io.StringOutput,
@@ -42,307 +43,345 @@
         pub.set_destination(destination=None, destination_path=None)
         output = pub.publish(enable_exit_status=False)
         self.assertLess(pub.document.reporter.max_level, 0)
         return output, pub
 
 
 class TestBasic(RendererTestBase):
-    def test_fail_rst(self):
+    def test_fail_rst(self) -> None:
         with self.assertRaises(AssertionError):
             # This check should be failed and report warning
             self.check_rst("```")
 
-    def test_simple_paragraph(self):
+    def test_simple_paragraph(self) -> None:
         src = "this is a sentence.\n"
         out = self.conv(src)
         self.assertEqual(out, "\n" + src)
 
-    def test_multiline_paragraph(self):
+    def test_multiline_paragraph(self) -> None:
         src = "\n".join(
             [
                 "first sentence.",
                 "second sentence.",
             ]
         )
         out = self.conv(src)
         self.assertEqual(out, "\n" + src + "\n")
 
-    def test_multi_paragraph(self):
+    def test_multi_paragraph(self) -> None:
         src = "\n".join(
             [
                 "first paragraph.",
                 "",
                 "second paragraph.",
             ]
         )
         out = self.conv(src)
         self.assertEqual(out, "\n" + src + "\n")
 
-    def test_hr(self):
+    def test_hr(self) -> None:
         src = "a\n\n---\n\nb"
         out = self.conv(src)
         self.assertEqual(out, "\na\n\n----\n\nb\n")
 
-    def test_linebreak(self):
+    def test_linebreak(self) -> None:
         src = "abc def  \nghi"
         out = self.conv(src)
         self.assertEqual(
             out,
             PROLOG + "\nabc def :raw-html-md:`<br />`\nghi" + "\n",
         )
 
 
 class TestInlineMarkdown(RendererTestBase):
-    def test_inline_code(self):
+    def test_inline_code(self) -> None:
         src = "`a`"
         out = self.conv(src)
         self.assertEqual(out.replace("\n", ""), "``a``")
 
-    def test_inline_code_with_backticks(self):
+    def test_inline_code_with_backticks(self) -> None:
         src = "```a``a```"
         out = self.conv(src)
         self.assertEqual(
             out.strip(),
             ".. role:: raw-html-md(raw)\n"
             "   :format: html\n\n\n"
             ':raw-html-md:`<code class="docutils literal">'
             '<span class="pre">a&#96;&#96;a</span></code>`',
         )
 
-    def test_strikethrough(self):
+    def test_inline_code_with_opening_space(self) -> None:
+        src = "`` `a`:role:``"
+        out = self.conv(src)
+        self.assertEqual(
+            out.strip(),
+            ".. role:: raw-html-md(raw)\n"
+            "   :format: html\n\n\n"
+            ':raw-html-md:`<code class="docutils literal">'
+            '<span class="pre"> &#96;a&#96;:role:</span></code>`',
+        )
+
+    def test_inline_code_with_closing_space(self) -> None:
+        src = "``:role:`a` ``"
+        out = self.conv(src)
+        self.assertEqual(
+            out.strip(),
+            ".. role:: raw-html-md(raw)\n"
+            "   :format: html\n\n\n"
+            ':raw-html-md:`<code class="docutils literal">'
+            '<span class="pre">:role:&#96;a&#96; </span></code>`',
+        )
+
+    def test_inline_code_with_opening_and_closing_space(self) -> None:
+        src = "`` a ``"
+        out = self.conv(src)
+        self.assertEqual(out, "\n``a``\n")
+
+    def test_inline_code_with_opening_and_closing_space_and_backtick(self) -> None:
+        src = "`` `a` ``"
+        out = self.conv(src)
+        self.assertEqual(
+            out.strip(),
+            ".. role:: raw-html-md(raw)\n"
+            "   :format: html\n\n\n"
+            ':raw-html-md:`<code class="docutils literal">'
+            '<span class="pre">&#96;a&#96;</span></code>`',
+        )
+
+    def test_strikethrough(self) -> None:
         src = "~~a~~"
         self.conv(src)
 
-    def test_emphasis(self):
+    def test_emphasis(self) -> None:
         src = "*a*"
         out = self.conv(src)
         self.assertEqual(out.replace("\n", ""), "*a*")
 
-    def test_emphasis_(self):
+    def test_emphasis_(self) -> None:
         src = "_a_"
         out = self.conv(src)
         self.assertEqual(out.replace("\n", ""), "*a*")
 
-    def test_double_emphasis(self):
+    def test_double_emphasis(self) -> None:
         src = "**a**"
         out = self.conv(src)
         self.assertEqual(out.replace("\n", ""), "**a**")
 
-    def test_double_emphasis__(self):
+    def test_double_emphasis__(self) -> None:
         src = "__a__"
         out = self.conv(src)
         self.assertEqual(out.replace("\n", ""), "**a**")
 
-    def test_not_an_autolink(self):
+    def test_not_an_autolink(self) -> None:
         src = "link to http://example.com/ in sentence."
         out = self.conv(src)
         self.assertEqual(out, "\n" + src + "\n")
 
-    def test_link(self):
+    def test_link(self) -> None:
         src = "this is a [link](http://example.com/)."
         out = self.conv(src)
         self.assertEqual(out, "\nthis is a `link <http://example.com/>`_.\n")
 
-    def test_anchor(self):
+    def test_anchor(self) -> None:
         src = "this is an [anchor link](#anchor)."
         out = self.conv_no_check(src)
         self.assertEqual(out, "\nthis is an :ref:`anchor link <anchor>`.\n")
 
-    def test_autolink(self):
+    def test_autolink(self) -> None:
         src = "link <http://example.com>"
         out = self.conv(src)
         self.assertEqual(out, "\nlink `http://example.com <http://example.com>`_\n")
 
-    def test_link_title(self):
+    def test_link_title(self) -> None:
         src = 'this is a [link](http://example.com/ "example").'
         out = self.conv(src)
         self.assertEqual(
             out,
             ".. role:: raw-html-md(raw)\n"
             "   :format: html\n\n\n"
             "this is a :raw-html-md:"
             '`<a href="http://example.com/" title="example">link</a>`.\n',
         )
 
-    def test_image_link(self):
+    def test_image_link(self) -> None:
         src = "[![Alt Text](image_taget_url)](link_target_url)"
         out = self.conv(src)
         self.assertEqual(
             out,
             "\n\n.. image:: image_taget_url\n"
             "   :target: link_target_url\n   :alt: Alt Text\n\n",
         )
 
-    def test_rest_role(self):
+    def test_rest_role(self) -> None:
         src = "a :code:`some code` inline."
         out = self.conv(src)
         self.assertEqual(out, "\n" + src + "\n")
 
-    def test_rest_role2(self):
+    def test_rest_role2(self) -> None:
         src = "a `some code`:code: inline."
         out = self.conv(src)
         self.assertEqual(out, "\n" + src + "\n")
 
-    def test_rest_link(self):
+    def test_rest_link(self) -> None:
         src = "a `RefLink <http://example.com>`_ here."
         out = self.conv(src)
         self.assertEqual(out, "\n" + src + "\n")
 
-    def test_rest_link_and_role(self):
+    def test_rest_link_and_role(self) -> None:
         src = "a :code:`a` and `RefLink <http://example.com>`_ here."
         out = self.conv(src)
         self.assertEqual(out, "\n" + src + "\n")
 
-    def test_rest_link_and_role2(self):
+    def test_rest_link_and_role2(self) -> None:
         src = "a `a`:code: and `RefLink <http://example.com>`_ here."
         out = self.conv(src)
         self.assertEqual(out, "\n" + src + "\n")
 
-    def test_rest_role_incomplete(self):
+    def test_rest_role_incomplete(self) -> None:
         src = "a co:`de` and `RefLink <http://example.com>`_ here."
         out = self.conv(src)
         self.assertEqual(
             out,
             "\na co:``de`` and `RefLink <http://example.com>`_ here.\n",
         )
 
-    def test_rest_role_incomplete2(self):
+    def test_rest_role_incomplete2(self) -> None:
         src = "a `RefLink <http://example.com>`_ and co:`de` here."
         out = self.conv(src)
         self.assertEqual(
             out,
             "\na `RefLink <http://example.com>`_ and co:``de`` here.\n",
         )
 
-    def test_rest_role_with_code(self):
+    def test_rest_role_with_code(self) -> None:
         src = "a `code` and :code:`rest` here."
         out = self.conv(src)
         self.assertEqual(out, "\na ``code`` and :code:`rest` here.\n")
 
-    def test_rest2_role_with_code(self):
+    def test_rest2_role_with_code(self) -> None:
         src = "a `code` and `rest`:code: here."
         out = self.conv(src)
         self.assertEqual(out, "\na ``code`` and `rest`:code: here.\n")
 
-    def test_code_with_rest_role(self):
+    def test_code_with_rest_role(self) -> None:
         src = "a :code:`rest` and `code` here."
         out = self.conv(src)
         self.assertEqual(out, "\na :code:`rest` and ``code`` here.\n")
 
-    def test_code_with_rest_role2(self):
+    def test_code_with_rest_role2(self) -> None:
         src = "a `rest`:code: and `code` here."
         out = self.conv(src)
         self.assertEqual(out, "\na `rest`:code: and ``code`` here.\n")
 
-    def test_rest_link_with_code(self):
+    def test_rest_link_with_code(self) -> None:
         src = "a `RefLink <a>`_ and `code` here."
         out = self.conv(src)
         self.assertEqual(out, "\na `RefLink <a>`_ and ``code`` here.\n")
 
-    def test_code_with_rest_link(self):
+    def test_code_with_rest_link(self) -> None:
         src = "a `code` and `RefLink <a>`_ here."
         out = self.conv(src)
         self.assertEqual(out, "\na ``code`` and `RefLink <a>`_ here.\n")
 
-    def test_inline_math(self):
+    def test_inline_math(self) -> None:
         src = "this is `$E = mc^2$` inline math."
         out = self.conv(src)
         self.assertEqual(out, "\nthis is :math:`E = mc^2` inline math.\n")
 
-    def test_inline_html(self):
+    def test_inline_html(self) -> None:
         src = "this is <s>html</s>."
         out = self.conv(src)
         self.assertEqual(out, PROLOG + "\nthis is :raw-html-md:`<s>html</s>`.\n")
 
-    def test_block_html(self):
+    def test_block_html(self) -> None:
         src = "<h1>title</h1>"
         out = self.conv(src)
         self.assertEqual(out, "\n\n.. raw:: html\n\n   <h1>title</h1>\n\n")
 
 
 class TestBlockQuote(RendererTestBase):
-    def test_block_quote(self):
+    def test_block_quote(self) -> None:
         src = "> q1\n> q2"
         out = self.conv(src)
         self.assertEqual(out, "\n..\n\n   q1\n   q2\n\n")
 
-    def test_block_quote_nested(self):
+    def test_block_quote_nested(self) -> None:
         src = "> q1\n> > q2"
         out = self.conv(src)
         # one extra empty line is inserted, but still valid rst anyway
         self.assertEqual(out, "\n..\n\n   q1\n\n   ..\n\n      q2\n\n")
 
     @skip("markdown does not support dedent in block quote")
-    def test_block_quote_nested_2(self):
+    def test_block_quote_nested_2(self) -> None:
         src = "> q1\n> > q2\n> q3"
         out = self.conv(src)
         self.assertEqual(out, "\n..\n\n   q1\n\n   ..\n      q2\n\n   q3\n\n")
 
 
 class TestCodeBlock(RendererTestBase):
-    def test_plain_code_block(self):
+    def test_plain_code_block(self) -> None:
         src = "\n".join(
             [
                 "```",
                 "pip install sphinx",
                 "```",
             ]
         )
         out = self.conv(src)
         self.assertEqual(out, "\n.. code-block::\n\n   pip install sphinx\n")
 
-    def test_plain_code_block_tilda(self):
+    def test_plain_code_block_tilda(self) -> None:
         src = "\n".join(
             [
                 "~~~",
                 "pip install sphinx",
                 "~~~",
             ]
         )
         out = self.conv(src)
         self.assertEqual(out, "\n.. code-block::\n\n   pip install sphinx\n")
 
-    def test_code_block_math(self):
+    def test_code_block_math(self) -> None:
         src = "\n".join(
             [
                 "```math",
                 "E = mc^2",
                 "```",
             ]
         )
         out = self.conv(src)
         self.assertEqual(out, "\n.. math::\n\n   E = mc^2\n")
 
-    def test_plain_code_block_indent(self):
+    def test_plain_code_block_indent(self) -> None:
         src = "\n".join(
             [
                 "```",
                 "pip install sphinx",
                 "    new line",
                 "```",
             ]
         )
         out = self.conv(src)
         self.assertEqual(
             out,
             "\n.. code-block::\n\n   pip install sphinx\n       new line\n",
         )
 
-    def test_python_code_block(self):
+    def test_python_code_block(self) -> None:
         src = "\n".join(
             [
                 "```python",
                 "print(1)",
                 "```",
             ]
         )
         out = self.conv(src)
         self.assertEqual(out, "\n.. code-block:: python\n\n   print(1)\n")
 
-    def test_python_code_block_indent(self):
+    def test_python_code_block_indent(self) -> None:
         src = "\n".join(
             [
                 "```python",
                 "def a(i):",
                 "    print(i)",
                 "```",
             ]
@@ -351,53 +390,53 @@
         self.assertEqual(
             out,
             "\n.. code-block:: python\n\n   def a(i):\n       print(i)\n",
         )
 
 
 class TestImage(RendererTestBase):
-    def test_image(self):
+    def test_image(self) -> None:
         src = "![alt text](a.png)"
         out = self.conv(src)
         # first and last newline is inserted by paragraph
         self.assertEqual(
             out,
             "\n\n.. image:: a.png\n   :target: a.png\n   :alt: alt text\n\n",
         )
 
-    def test_image_title(self):
+    def test_image_title(self) -> None:
         src = '![alt text](a.png "title")'
         self.conv(src)
         # title is not supported now
 
 
 class TestHeading(RendererTestBase):
-    def test_heading(self):
+    def test_heading(self) -> None:
         src = "# head 1"
         out = self.conv(src)
         self.assertEqual(out, "\nhead 1\n" + "=" * 6 + "\n")
 
-    def test_heading_multibyte(self):
+    def test_heading_multibyte(self) -> None:
         src = "# マルチバイト文字\n"
         out = self.conv(src)
         self.assertEqual(out, "\nマルチバイト文字\n" + "=" * 16 + "\n")
 
 
 class TestList(RendererTestBase):
-    def test_ul(self):
+    def test_ul(self) -> None:
         src = "* list"
         out = self.conv(src)
         self.assertEqual(out, "\n\n* list\n")
 
-    def test_ol(self):
+    def test_ol(self) -> None:
         src = "1. list"
         out = self.conv(src)
         self.assertEqual(out, "\n\n#. list\n")
 
-    def test_nested_ul(self):
+    def test_nested_ul(self) -> None:
         src = "\n".join(
             [
                 "* list 1",
                 "* list 2",
                 "  * list 2.1",
                 "  * list 2.2",
                 "* list 3",
@@ -409,15 +448,15 @@
             "\n\n* list 1\n"
             "* list 2\n\n"
             "  * list 2.1\n"
             "  * list 2.2\n\n"
             "* list 3\n",
         )
 
-    def test_nested_ul_2(self):
+    def test_nested_ul_2(self) -> None:
         src = "\n".join(
             [
                 "* list 1",
                 "* list 2",
                 "  * list 2.1",
                 "  * list 2.2",
                 "    * list 2.2.1",
@@ -433,15 +472,15 @@
             "  * list 2.1\n"
             "  * list 2.2\n\n"
             "    * list 2.2.1\n"
             "    * list 2.2.2\n\n"
             "* list 3\n",
         )
 
-    def test_nested_ol(self):
+    def test_nested_ol(self) -> None:
         src = "\n".join(
             [
                 "1. list 1",
                 "1. list 2",
                 "    1. list 2.1",
                 "    1. list 2.2",
                 "1. list 3",
@@ -455,15 +494,15 @@
             "\n"
             "   #. list 2.1\n"
             "   #. list 2.2\n"
             "\n"
             "#. list 3\n",
         )
 
-    def test_nested_ol_2(self):
+    def test_nested_ol_2(self) -> None:
         src = "\n".join(
             [
                 "1. list 1",
                 "1. list 2",
                 "    1. list 2.1",
                 "    1. list 2.2",
                 "        1. list 2.2.1",
@@ -486,15 +525,15 @@
                     "      #. list 2.2.2",
                     "",
                     "#. list 3\n",
                 ]
             ),
         )
 
-    def test_nested_mixed_1(self):
+    def test_nested_mixed_1(self) -> None:
         src = "\n".join(
             [
                 "1. list 1",
                 "2. list 2",
                 "   * list 2.1",
                 "   * list 2.2",
                 "     1. list 2.2.1",
@@ -517,15 +556,15 @@
                     "     #. list 2.2.2",
                     "",
                     "#. list 3\n",
                 ]
             ),
         )
 
-    def test_nested_multiline_1(self):
+    def test_nested_multiline_1(self) -> None:
         src = "\n".join(
             [
                 "* list 1",
                 "  list 1 cont",
                 "* list 2",
                 "  list 2 cont",
                 "  * list 2.1",
@@ -557,15 +596,15 @@
                     "    * list 2.2.2",
                     "",
                     "* list 3\n",
                 ]
             ),
         )
 
-    def test_nested_multiline_2(self):
+    def test_nested_multiline_2(self) -> None:
         src = "\n".join(
             [
                 "1. list 1",
                 "   list 1 cont",
                 "1. list 2",
                 "   list 2 cont",
                 "   1. list 2.1",
@@ -597,15 +636,15 @@
                     "      #. list 2.2.2",
                     "",
                     "#. list 3\n",
                 ]
             ),
         )
 
-    def test_nested_multiline_3(self):
+    def test_nested_multiline_3(self) -> None:
         src = "\n".join(
             [
                 "1. list 1",
                 "   list 1 cont",
                 "1. list 2",
                 "   list 2 cont",
                 "   * list 2.1",
@@ -638,16 +677,16 @@
                     "",
                     "#. list 3\n",
                 ]
             ),
         )
 
 
-class TestConplexText(RendererTestBase):
-    def test_code(self):
+class TestComplexText(RendererTestBase):
+    def test_code(self) -> None:
         src = """
 some sentence
 ```python
 print(1)
 ```
 some sentence
 
@@ -658,15 +697,15 @@
 ---
 end
 """
         self.conv(src)
 
 
 class TestTable(RendererTestBase):
-    def test_table(self):
+    def test_table(self) -> None:
         src = """h1 | h2 | h3\n--- | --- | ---\n1 | 2 | 3\n4 | 5 | 6"""
         out = self.conv(src)
         self.assertEqual(
             out,
             "\n".join(
                 [
                     "",
@@ -686,15 +725,15 @@
                     "",
                 ]
             ),
         )
 
 
 class TestFootNote(RendererTestBase):
-    def test_footnote(self):
+    def test_footnote(self) -> None:
         src = "\n".join(
             [
                 "This is a[^1] footnote[^2] ref[^ref] with rst [#a]_.",
                 "",
                 "[^1]: note 1",
                 "[^2]: note 2",
                 "[^ref]: note ref",
@@ -704,71 +743,71 @@
         out = self.conv(src)
         self.assertEqual(
             out,
             "\n".join(
                 [
                     "",
                     "This is a[#fn-1]_ "
-                    "footnote[#fn-2]_ ref[#fn-ref]_ with rst [#a]_.",
+                    "footnote[#fn-2]_ ref[#fn-REF]_ with rst [#a]_.",
                     "",
                     ".. [#a] note rst",  # one empty line inserted...
                     "",
                     ".. [#fn-1] note 1",
                     ".. [#fn-2] note 2",
-                    ".. [#fn-ref] note ref",
+                    ".. [#fn-REF] note ref",
                     "",
                 ]
             ),
         )
 
-    def test_sphinx_ref(self):
+    def test_sphinx_ref(self) -> None:
         src = "This is a sphinx [ref]_ global ref.\n\n.. [ref] ref text"
         out = self.conv(src)
         self.assertEqual(out, "\n" + src)
 
 
 class TestDirective(RendererTestBase):
-    def test_comment_oneline(self):
+    def test_comment_oneline(self) -> None:
         src = ".. a"
         out = self.conv(src)
         self.assertEqual(out, "\n.. a")
 
     @skip("not sure why this should work")
-    def test_comment_indented(self):
+    def test_comment_indented(self) -> None:
         src = "    .. a"
         out = self.conv(src)
         self.assertEqual(out, "\n    .. a")
 
-    def test_comment_newline(self):
+    def test_comment_newline(self) -> None:
         src = "..\n\n   comment\n\nnewline"
         out = self.conv(src)
         self.assertEqual(out, "\n..\n\n   comment\n\nnewline\n")
 
-    def test_comment_multiline(self):
+    def test_comment_multiline(self) -> None:
         comment = (
             ".. this is comment.\n"
             "   this is also comment.\n"
             "\n"
             "\n"
             "    comment may include empty line.\n"
             "\n\n"
         )
         src = comment + "`eoc`"
         out = self.conv(src)
         self.assertEqual(out, "\n" + comment + "``eoc``\n")
 
 
 class TestRestCode(RendererTestBase):
-    def test_rest_code_block_empty(self):
+    def test_rest_code_block_empty(self) -> None:
         src = "\n\n::\n\n"
         out = self.conv(src)
         self.assertEqual(out, "\n\n")
 
-    def test_eol_marker(self):
+    def test_eol_marker(self) -> None:
         src = "a::\n\n    code\n"
         out = self.conv(src)
         self.assertEqual(out, "\na:\n\n.. code-block::\n\n   code\n")
 
-    def test_eol_marker_remove(self):
+    def test_eol_marker_remove(self) -> None:
         src = "a ::\n\n    code\n"
         out = self.conv(src)
         self.assertEqual(out, "\na\n\n.. code-block::\n\n   code\n")
```

### Comparing `sphinx_mdinclude-0.5.4/sphinx_mdinclude/tests/test_smoke.py` & `sphinx_mdinclude-0.6.0/sphinx_mdinclude/tests/test_smoke.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,22 +34,22 @@
 class SmokeTest(unittest.TestCase):
     maxDiff = None
 
     @unittest.skipIf(
         platform.system() == "Windows",
         "inconsistent column widths on Windows",
     )
-    def test_convert(self):
+    def test_convert(self) -> None:
         content = TEST_MD.read_text()
         expected = TEST_RST.read_text()
 
         result = convert(content)
         self.assertEqual(expected, result)
 
-    def test_mdinclude_basic(self):
+    def test_mdinclude_basic(self) -> None:
         content = dedent(
             f"""
             .. mdinclude:: {TEST_MD}
 
             """
         )
         expected = dedent(
```

### Comparing `sphinx_mdinclude-0.5.4/PKG-INFO` & `sphinx_mdinclude-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: sphinx_mdinclude
-Version: 0.5.4
+Version: 0.6.0
 Summary: Markdown extension for Sphinx
 Keywords: Markdown,reStructuredText,sphinx-extension
 Author-email: Hiroyuki Takagi <miyako.dev@gmail.com>, CrossNox <ijmermet+m2r2@gmail.com>, Amethyst Reese <amy@noswap.com>
 Maintainer-email: Amethyst Reese <amy@noswap.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Topic :: Text Processing
-Requires-Dist: mistune >=2.0,<3.0
+Requires-Dist: mistune >=3.0,<4.0
 Requires-Dist: docutils >=0.16,<1.0
 Requires-Dist: pygments >= 2.8
 Requires-Dist: docutils==0.20.1 ; extra == "dev" and ( python_version < '3.9')
 Requires-Dist: docutils==0.21.1 ; extra == "dev" and ( python_version >= '3.9')
-Requires-Dist: mistune==2.0.4 ; extra == "dev"
-Requires-Dist: attribution==1.6.2 ; extra == "dev"
+Requires-Dist: mistune==3.0.2 ; extra == "dev"
+Requires-Dist: attribution==1.7.1 ; extra == "dev"
 Requires-Dist: black==24.4.0 ; extra == "dev"
-Requires-Dist: coverage==7.3.2 ; extra == "dev"
+Requires-Dist: coverage==7.4.4 ; extra == "dev"
 Requires-Dist: flake8==7.0.0 ; extra == "dev"
 Requires-Dist: flit==3.9.0 ; extra == "dev"
 Requires-Dist: mypy==1.9.0 ; extra == "dev"
 Requires-Dist: sphinx==7.1.2 ; extra == "dev" and ( python_version < '3.9')
 Requires-Dist: sphinx==7.3.7 ; extra == "dev" and ( python_version >= '3.9')
 Requires-Dist: ufmt==2.5.1 ; extra == "dev"
-Requires-Dist: usort==1.0.7 ; extra == "dev"
+Requires-Dist: usort==1.0.8.post1 ; extra == "dev"
 Project-URL: Github, https://github.com/omnilib/sphinx-mdinclude
 Provides-Extra: dev
 
 sphinx-mdinclude
 ================
 
 Sphinx extension for including or writing pages in Markdown format.
```


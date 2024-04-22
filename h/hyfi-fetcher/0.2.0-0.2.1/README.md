# Comparing `tmp/hyfi_fetcher-0.2.0.tar.gz` & `tmp/hyfi_fetcher-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_fetcher-0.2.0.tar", max compression
+gzip compressed data, was "hyfi_fetcher-0.2.1.tar", max compression
```

## Comparing `hyfi_fetcher-0.2.0.tar` & `hyfi_fetcher-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2024-04-19 08:09:29.932331 hyfi_fetcher-0.2.0/LICENSE
--rw-r--r--   0        0        0     1997 2024-04-19 08:09:29.932331 hyfi_fetcher-0.2.0/README.md
--rw-r--r--   0        0        0     3385 2024-04-19 08:09:54.288398 hyfi_fetcher-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      185 2024-04-19 08:09:29.932331 hyfi_fetcher-0.2.0/src/hyfetcher/__cli__.py
--rw-r--r--   0        0        0      524 2024-04-19 08:09:29.932331 hyfi_fetcher-0.2.0/src/hyfetcher/__init__.py
--rw-r--r--   0        0        0       22 2024-04-19 08:09:54.252398 hyfi_fetcher-0.2.0/src/hyfetcher/_version.py
--rw-r--r--   0        0        0        0 2024-04-19 08:09:29.932331 hyfi_fetcher-0.2.0/src/hyfetcher/agents/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/chains/__init__.py
--rw-r--r--   0        0        0      499 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/chains/extraction.py
--rw-r--r--   0        0        0        0 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/conf/__init__.py
--rw-r--r--   0        0        0      297 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/conf/about/hyfetcher.yaml
--rw-r--r--   0        0        0      742 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/conf/fetcher/sierraclub.yaml
--rw-r--r--   0        0        0       52 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/conf/llm/__init__.yaml
--rw-r--r--   0        0        0       91 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/conf/llm/gpt35.yaml
--rw-r--r--   0        0        0       80 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/conf/llm/gpt4.yaml
--rw-r--r--   0        0        0      141 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/conf/llm/openai.yaml
--rw-r--r--   0        0        0        0 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/fetcher/__init__.py
--rw-r--r--   0        0        0    20729 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/fetcher/base.py
--rw-r--r--   0        0        0      176 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/fetcher/schemas.py
--rw-r--r--   0        0        0     4332 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/fetcher/sierra.py
--rw-r--r--   0        0        0       57 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/llms/__init__.py
--rw-r--r--   0        0        0     3394 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/llms/openai.py
--rw-r--r--   0        0        0        0 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/py.typed
--rw-r--r--   0        0        0        0 2024-04-19 08:09:29.936332 hyfi_fetcher-0.2.0/src/hyfetcher/tools/__init__.py
--rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 hyfi_fetcher-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-22 09:04:59.235656 hyfi_fetcher-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1997 2024-04-22 09:04:59.235656 hyfi_fetcher-0.2.1/README.md
+-rw-r--r--   0        0        0     3385 2024-04-22 09:05:28.663763 hyfi_fetcher-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      185 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/__cli__.py
+-rw-r--r--   0        0        0      524 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-22 09:05:28.631763 hyfi_fetcher-0.2.1/src/hyfetcher/_version.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/agents/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/chains/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/chains/extraction.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/conf/__init__.py
+-rw-r--r--   0        0        0      297 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/conf/about/hyfetcher.yaml
+-rw-r--r--   0        0        0      730 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/conf/fetcher/sample.yaml
+-rw-r--r--   0        0        0       52 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/conf/llm/__init__.yaml
+-rw-r--r--   0        0        0       91 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/conf/llm/gpt35.yaml
+-rw-r--r--   0        0        0       80 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/conf/llm/gpt4.yaml
+-rw-r--r--   0        0        0      141 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/conf/llm/openai.yaml
+-rw-r--r--   0        0        0        0 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/fetcher/__init__.py
+-rw-r--r--   0        0        0    20723 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/fetcher/base.py
+-rw-r--r--   0        0        0     4474 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/fetcher/sample.py
+-rw-r--r--   0        0        0      176 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/fetcher/schemas.py
+-rw-r--r--   0        0        0       57 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/llms/__init__.py
+-rw-r--r--   0        0        0     3394 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/llms/openai.py
+-rw-r--r--   0        0        0        0 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/py.typed
+-rw-r--r--   0        0        0        0 2024-04-22 09:04:59.239656 hyfi_fetcher-0.2.1/src/hyfetcher/tools/__init__.py
+-rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 hyfi_fetcher-0.2.1/PKG-INFO
```

### Comparing `hyfi_fetcher-0.2.0/LICENSE` & `hyfi_fetcher-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_fetcher-0.2.0/README.md` & `hyfi_fetcher-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_fetcher-0.2.0/pyproject.toml` & `hyfi_fetcher-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi-fetcher"
-version = "0.2.0"
+version = "0.2.1"
 description = "HyFI-Fetcher is a Python package for programmatically scraping websites to extract various data, serving as a plugin for HyFI."
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-fetcher.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi-fetcher"
 readme = "README.md"
 packages = [{ include = "hyfetcher", from = "src" }]
```

### Comparing `hyfi_fetcher-0.2.0/src/hyfetcher/__init__.py` & `hyfi_fetcher-0.2.1/src/hyfetcher/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi_fetcher-0.2.0/src/hyfetcher/conf/fetcher/sierraclub.yaml` & `hyfi_fetcher-0.2.1/src/hyfetcher/conf/fetcher/sample.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-_target_: hyfetcher.fetcher.sierra.SierraClubFetcher
-_config_name_: sierraclub
+_target_: hyfetcher.fetcher.sample.SampleFetcher
+_config_name_: sample
 _config_group_: /fetcher
 article_filename: articles.jsonl
 base_url: https://www.sierraclub.org
 delay_between_requests: 0.5
 key_field: url
 keyword_placeholder: '{keyword}'
 link_filename: links.jsonl
 max_num_articles: 30
 max_num_pages: 2
 num_workers: 1
-output_dir: workspace/datasets/fetcher/sierraclub
+output_dir: workspace/datasets/fetcher/sample
 overwrite_existing: false
 page_placeholder: '{page}'
 print_every: 10
 search_keywords: []
 search_url: https://www.sierraclub.org/press-releases?_wrapper_format=html&page={page}
 start_page: 1
 start_urls: []
```

### Comparing `hyfi_fetcher-0.2.0/src/hyfetcher/fetcher/base.py` & `hyfi_fetcher-0.2.1/src/hyfetcher/fetcher/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,28 +232,28 @@
     def _load_articles(self) -> List[dict]:
         if Path(self.article_filepath).exists():
             self._articles = HyFI.load_jsonl(self.article_filepath)
         return self._articles
 
     def fetch_links(self):
         parse_page_func = partial(
-            self._parse_page_links,
+            self.parse_page_links,
             print_every=self.print_every,
             verbose=self.verbose,
         )
 
         next_page_func = partial(
-            self._next_page_func,
+            self.next_page_func,
             page_placeholder=self.page_placeholder,
         )
 
         self._fetch_links(parse_page_func, next_page_func)
 
     def fetch_articles(self):
-        parse_article_text = partial(self._parse_article_text)
+        parse_article_text = partial(self.parse_article_text)
 
         self._fetch_articles(parse_article_text)
 
     def _fetch_links(self, parse_page_func: Callable, next_page_func: Callable):
         num_workers = min(self.num_workers, len(self.search_keywords))
         num_workers = max(num_workers, 1)
         link_urls = [link["url"] for link in self.links]
@@ -365,15 +365,15 @@
         ]
         with mp.Pool(num_workers) as pool:
             results = pool.map(batch_func, batches)
         for result in results:
             articles.extend(result)
         return articles
 
-    def _next_page_func(
+    def next_page_func(
         self,
         start_url: str,
         current_url: Optional[str],
         page: int,
         page_placeholder: Optional[str],
     ) -> Optional[str]:
         if page_placeholder and page_placeholder in start_url:
@@ -383,26 +383,26 @@
             page_url = start_url
         else:
             # TODO: implement your next page logic to return None if no more pages
             raise NotImplementedError("Next page logic not implemented in base class")
         logger.info("Page url: %s", page_url)
         return page_url
 
-    def _parse_page_links(
+    def parse_page_links(
         self,
         page_url: str,
         print_every: int = 10,
         verbose: bool = False,
     ) -> Optional[List[dict]]:
         """Get the links from the given page."""
 
         # TODO: Parse the page and extract all links
         raise NotImplementedError("Parsing links is not implemented in base class")
 
-    def _parse_article_text(self, url: str) -> dict:
+    def parse_article_text(self, url: str) -> dict:
         # TODO: Scrape the article page and extract the text
         raise NotImplementedError(
             "Parsing article text is not implemented in base class"
         )
 
 
 def crawl_links(
```

### Comparing `hyfi_fetcher-0.2.0/src/hyfetcher/fetcher/sierra.py` & `hyfi_fetcher-0.2.1/src/hyfetcher/fetcher/sample.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List, Optional
 
 from .base import BaseFetcher
 
 logger = logging.getLogger(__name__)
 
 
-class SierraClubFetcher(BaseFetcher):
+class SampleFetcher(BaseFetcher):
     """
     Fetcher for Sierra Club website.
 
     This class provides methods to fetch press releases from the Sierra Club website.
     It inherits from the BaseFetcher class.
 
     Attributes:
@@ -28,29 +28,29 @@
 
         link_find_all_name (str): The HTML tag name for finding links.
         link_find_all_attrs (dict): The attributes for finding links.
         lint_article_name (str): The HTML tag name for finding article titles.
         lint_article_attrs (dict): The attributes for finding article titles.
     """
 
-    _config_name_: str = "sierraclub"
+    _config_name_: str = "sample"
     _config_group_: str = "/fetcher"
     output_dir: str = f"workspace/datasets{_config_group_}/{_config_name_}"
 
     base_url: str = "https://www.sierraclub.org"
     search_url: str = base_url + "/press-releases?_wrapper_format=html&page={page}"
     search_keywords: List[str] = []
     use_playwright: bool = False
 
     link_find_all_name: str = "div"
     link_find_all_attrs: dict = {"class": "post"}
     lint_article_name: str = "h3"
     lint_article_attrs: dict = {"class": "post-title"}
 
-    def _parse_page_links(
+    def parse_page_links(
         self,
         page_url: str,
         print_every: int = 10,
         verbose: bool = False,
     ) -> Optional[List[dict]]:
         """
         Get the links from the given page.
@@ -78,15 +78,19 @@
             title_div = article.find(
                 self.lint_article_name, attrs=self.lint_article_attrs
             )
             if title_div is None:
                 logger.info("No title found for article %s", article_no)
                 continue
             title = title_div.text
-            url = self.base_url + article.find("a")["href"]
+            if a_link := article.find("a"):
+                url = self.base_url + a_link["href"]
+            else:
+                logger.info("No link found for article %s", article_no)
+                continue
 
             date_ = article.find("div", class_="views-field-field-published-date").find(
                 "div", class_="field-content"
             )
             item_date = date_.text.strip() if date_ else ""
 
             if verbose and article_no % print_every == 0:
@@ -96,15 +100,15 @@
                 "title": title,
                 "timestamp": item_date,
                 "url": url,
             }
             links.append(link)
         return links
 
-    def _parse_article_text(self, url: str) -> Optional[dict]:
+    def parse_article_text(self, url: str) -> Optional[dict]:
         """
         Parse the article text from the given URL.
 
         Args:
             url (str): The URL of the article to parse.
 
         Returns:
```

### Comparing `hyfi_fetcher-0.2.0/src/hyfetcher/llms/openai.py` & `hyfi_fetcher-0.2.1/src/hyfetcher/llms/openai.py`

 * *Files identical despite different names*

### Comparing `hyfi_fetcher-0.2.0/PKG-INFO` & `hyfi_fetcher-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi-fetcher
-Version: 0.2.0
+Version: 0.2.1
 Summary: HyFI-Fetcher is a Python package for programmatically scraping websites to extract various data, serving as a plugin for HyFI.
 Home-page: https://hyfi-fetcher.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
```


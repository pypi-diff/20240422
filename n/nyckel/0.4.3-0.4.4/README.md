# Comparing `tmp/nyckel-0.4.3.tar.gz` & `tmp/nyckel-0.4.4.tar.gz`

## Comparing `nyckel-0.4.3.tar` & `nyckel-0.4.4.tar`

### file list

```diff
@@ -1,70 +1,72 @@
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 nyckel-0.4.3/mkdocs.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.3/requirements.txt
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.3/.github/workflows/docs.yml
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.3/.vscode/extensions.json
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 nyckel-0.4.3/.vscode/settings.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/copy_function.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/credentials.md
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/data_classes.md
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/delete_label.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/delete_samples.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/image_classification.md
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/image_tags.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/index.md
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/merge_labels.md
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/multimodal_classification.md
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/quickstart.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/requirements.txt
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/tabular_classification.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/text_classification.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/text_tags.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/assets/favicon.ico
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/assets/nyckel-logo.png
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.3/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/__init__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/auth.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/config.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/data_classes.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/image_processing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/py.typed
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/request_utils.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/__init__.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/__init__.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/classification.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/factory.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/function_handler.py
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/image_classification.py
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/label_handler.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/sample_handler.py
--rw-r--r--   0        0        0    14966 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/tabular_classification.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/classification/text_classification.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/__init__.py
--rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/image_tags.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/tags.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/tags_function_factory.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/tags_function_handler.py
--rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/tags_sample_handler.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 nyckel-0.4.3/src/nyckel/functions/tags/text_tags.py
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/conftest.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_duplicates_handling.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_field_handler.py
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_image_classification_function.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_image_decoder.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_image_tags_function.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_label_handler.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_sample_handler.py
--rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_tabular_classification_function.py
--rw-r--r--   0        0        0     8886 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_tags_shared.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_text_classification_function.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/test_white_background.py
--rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/fixtures/flower.jpg
--rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.3/tests/fixtures/mixed-alpha-background.png
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.3/LICENSE
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.3/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 nyckel-0.4.4/mkdocs.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.4/requirements.txt
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.4/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.4/.vscode/extensions.json
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 nyckel-0.4.4/.vscode/settings.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/copy_function.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/credentials.md
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/data_classes.md
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/delete_label.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/delete_samples.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/image_classification.md
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/image_tags.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/index.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/merge_labels.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/multimodal_classification.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/quickstart.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/requirements.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/tabular_classification.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/text_classification.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/text_tags.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/assets/nyckel-logo.png
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.4/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/__init__.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/auth.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/config.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/data_classes.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/image_processing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/py.typed
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/request_utils.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/__init__.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/classification.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/factory.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/function_handler.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/image_classification.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/label_handler.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/sample_handler.py
+-rw-r--r--   0        0        0    14969 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/tabular_classification.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/classification/text_classification.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/__init__.py
+-rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/image_tags.py
+-rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/tabular_tags.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/tags.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/tags_function_factory.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/tags_function_handler.py
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/tags_sample_handler.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 nyckel-0.4.4/src/nyckel/functions/tags/text_tags.py
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_duplicates_handling.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_field_handler.py
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_image_classification_function.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_image_decoder.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_image_tags_function.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_label_handler.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_sample_handler.py
+-rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_tabular_classification_function.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_tabular_tags_function.py
+-rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_tags_shared.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_text_classification_function.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/test_white_background.py
+-rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/fixtures/flower.jpg
+-rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.4/tests/fixtures/mixed-alpha-background.png
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.4/LICENSE
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.4/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.4/PKG-INFO
```

### Comparing `nyckel-0.4.3/mkdocs.yml` & `nyckel-0.4.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/.github/workflows/build.yml` & `nyckel-0.4.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/.github/workflows/docs.yml` & `nyckel-0.4.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/.github/workflows/test.yml` & `nyckel-0.4.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/.vscode/settings.json` & `nyckel-0.4.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/docs/copy_function.md` & `nyckel-0.4.4/docs/copy_function.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/docs/delete_label.md` & `nyckel-0.4.4/docs/delete_label.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/docs/delete_samples.md` & `nyckel-0.4.4/docs/delete_samples.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/docs/index.md` & `nyckel-0.4.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/docs/merge_labels.md` & `nyckel-0.4.4/docs/merge_labels.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/docs/multimodal_classification.md` & `nyckel-0.4.4/docs/multimodal_classification.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/docs/quickstart.md` & `nyckel-0.4.4/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/docs/assets/favicon.ico` & `nyckel-0.4.4/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/docs/assets/nyckel-logo.png` & `nyckel-0.4.4/docs/assets/nyckel-logo.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/__init__.py` & `nyckel-0.4.4/src/nyckel/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,7 +30,8 @@
 from .image_processing import ImageResizer, ImageDecoder, ImageEncoder  # noqa: F401
 from .functions.classification.factory import ClassificationFunctionFactory  # noqa: F401
 from .functions.classification.image_classification import ImageClassificationFunction  # noqa: F401
 from .functions.classification.tabular_classification import TabularClassificationFunction  # noqa: F401
 from .functions.classification.text_classification import TextClassificationFunction  # noqa: F401
 from .functions.tags.text_tags import TextTagsFunction  # noqa: F401
 from .functions.tags.image_tags import ImageTagsFunction  # noqa: F401
+from .functions.tags.tabular_tags import TabularTagsFunction  # noqa: F401
```

### Comparing `nyckel-0.4.3/src/nyckel/auth.py` & `nyckel-0.4.4/src/nyckel/auth.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/image_processing.py` & `nyckel-0.4.4/src/nyckel/image_processing.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/request_utils.py` & `nyckel-0.4.4/src/nyckel/request_utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/functions/utils.py` & `nyckel-0.4.4/src/nyckel/functions/utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/functions/classification/classification.py` & `nyckel-0.4.4/src/nyckel/functions/classification/classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/functions/classification/factory.py` & `nyckel-0.4.4/src/nyckel/functions/classification/factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/functions/classification/function_handler.py` & `nyckel-0.4.4/src/nyckel/functions/classification/function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/functions/classification/image_classification.py` & `nyckel-0.4.4/src/nyckel/functions/classification/image_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/functions/classification/label_handler.py` & `nyckel-0.4.4/src/nyckel/functions/classification/label_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 class ClassificationLabelHandler:
     def __init__(self, function_id: str, credentials: Credentials):
         self._function_id = function_id
         self._credentials = credentials
         self._url_handler = ClassificationFunctionURLHandler(function_id, credentials.server_url)
 
     def create_labels(self, labels: List[ClassificationLabel]) -> List[str]:
+        for label in labels:
+            label.name = label.name.strip()
         session = self._credentials.get_session()
         bodies = [
             {"name": label.name, "description": label.description, "metadata": label.metadata} for label in labels
         ]
         url = self._url_handler.api_endpoint(path="labels")
         progress_bar = tqdm(total=len(bodies), ncols=80, desc="Posting labels")
         responses = ParallelPoster(session, url, progress_bar)(bodies)
```

### Comparing `nyckel-0.4.3/src/nyckel/functions/classification/sample_handler.py` & `nyckel-0.4.4/src/nyckel/functions/classification/sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/functions/classification/tabular_classification.py` & `nyckel-0.4.4/src/nyckel/functions/classification/tabular_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         self._function_handler.delete()
 
     def invoke(  # type: ignore
         self,
         sample_data_list: List[TabularSampleData],
         model_id: str = "",
     ) -> List[ClassificationPrediction]:
-        return self._sample_handler.invoke(sample_data_list, self.get_image_field_transformer(), model_id=model_id)
+        return self._sample_handler.invoke(sample_data_list, self._get_image_field_transformer(), model_id=model_id)
 
     def has_trained_model(self) -> bool:
         return self._function_handler.is_trained
 
     def create_labels(self, labels: Sequence[Union[ClassificationLabel, str]]) -> List[NyckelId]:
         typed_labels = [
             label if isinstance(label, ClassificationLabel) else ClassificationLabel(name=label) for label in labels
@@ -136,17 +136,17 @@
             return []
 
         typed_samples = self._wrangle_post_samples_input(samples)
         typed_samples = self._strip_label_names(typed_samples)
         self._assert_fields_created(typed_samples)
         self._create_labels_as_needed(typed_samples)
         typed_samples = self._switch_field_names_to_field_ids(typed_samples)
-        return self._sample_handler.create_samples(typed_samples, self.get_image_field_transformer())
+        return self._sample_handler.create_samples(typed_samples, self._get_image_field_transformer())
 
-    def get_image_field_transformer(self) -> Callable:
+    def _get_image_field_transformer(self) -> Callable:
         fields = self.list_fields()
         image_field_transformer = lambda x: x  # type: ignore  # noqa: E731
         for field in fields:
             if field.type == "Image":
                 # There is only one image field (max) per function, so we can break here.
                 image_field_transformer = ImageFieldTransformer(field.id)  # type: ignore
                 break
```

### Comparing `nyckel-0.4.3/src/nyckel/functions/classification/text_classification.py` & `nyckel-0.4.4/src/nyckel/functions/classification/text_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/functions/tags/image_tags.py` & `nyckel-0.4.4/src/nyckel/functions/tags/image_tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/functions/tags/tags.py` & `nyckel-0.4.4/src/nyckel/functions/tags/tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/functions/tags/tags_function_factory.py` & `nyckel-0.4.4/src/nyckel/functions/tags/tags_function_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import time
 
 from nyckel import Credentials
-from nyckel.functions.tags import image_tags, text_tags
+from nyckel.functions.tags import image_tags, tabular_tags, text_tags
 from nyckel.functions.tags.tags_function_handler import TagsFunctionHandler
 from nyckel.functions.utils import strip_nyckel_prefix
 
 
 class TagsFunctionFactory:
 
     def __init__(self) -> None:
         self.function_type_by_input = {
             "Text": text_tags.TextTagsFunction,
             "Image": image_tags.ImageTagsFunction,
-            # "Tabular": tabular_classification.TabularClassificationFunction,
+            "Tabular": tabular_tags.TabularTagsFunction,
         }
 
     @classmethod
     def load(self, function_id: str, credentials: Credentials):
         function_handler = TagsFunctionHandler(function_id, credentials)
         input_modality = function_handler.get_input_modality()
         return self.function_type_by_input[input_modality](function_id, credentials)
```

### Comparing `nyckel-0.4.3/src/nyckel/functions/tags/tags_function_handler.py` & `nyckel-0.4.4/src/nyckel/functions/tags/tags_function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/functions/tags/tags_sample_handler.py` & `nyckel-0.4.4/src/nyckel/functions/tags/tags_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/src/nyckel/functions/tags/text_tags.py` & `nyckel-0.4.4/src/nyckel/functions/tags/text_tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/tests/conftest.py` & `nyckel-0.4.4/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import random
+import string
 import time
 from typing import Iterator
 
 import numpy as np
 import pytest
 import requests
 from nyckel import (
@@ -12,27 +14,41 @@
     Credentials,
     ImageClassificationFunction,
     ImageClassificationSample,
     ImageEncoder,
     ImageTagsFunction,
     TabularClassificationFunction,
     TabularClassificationSample,
+    TabularTagsFunction,
     TextClassificationFunction,
     TextClassificationSample,
     TextTagsFunction,
 )
+from nyckel.functions.classification.classification import TabularFunctionField
 from PIL import Image
 
 
 def make_random_image(size: int = 100) -> str:
     imarray = np.random.rand(size, size, 3) * 255
     img = Image.fromarray(imarray.astype("uint8")).convert("RGB")
     return ImageEncoder().to_base64(img)
 
 
+def make_random_text() -> str:
+    return "".join(random.choices(string.ascii_uppercase, k=50))
+
+
+def make_random_tabular() -> dict:
+    return {
+        "name": make_random_text(),
+        "age": random.randint(0, 100),
+        "mug": make_random_image(),
+    }
+
+
 def hold_until_list_samples_available(function: ClassificationFunction, expected_count: int) -> None:
     actual_count = 0
     while not actual_count == expected_count:
         actual_count = len(function.list_samples())
         time.sleep(0.25)
 
 
@@ -142,14 +158,34 @@
 @pytest.fixture
 def image_tags_function(auth_test_credentials: Credentials) -> Iterator[ImageTagsFunction]:
     func = ImageTagsFunction.create("PYTHON-SDK IMAGE TAGS TEST FUNCTION", auth_test_credentials)
     yield func
     func.delete()
 
 
+@pytest.fixture
+def tabular_tags_function(auth_test_credentials: Credentials) -> Iterator[ImageTagsFunction]:
+    func = TabularTagsFunction.create("PYTHON-SDK TABULAR TAGS TEST FUNCTION", auth_test_credentials)
+    yield func
+    func.delete()
+
+
+@pytest.fixture
+def tabular_tags_function_with_fields(auth_test_credentials: Credentials) -> Iterator[ImageTagsFunction]:
+    func = TabularTagsFunction.create("PYTHON-SDK TABULAR TAGS TEST FUNCTION", auth_test_credentials)
+    fields = [
+        TabularFunctionField(name="name", type="Text"),
+        TabularFunctionField(name="age", type="Number"),
+        TabularFunctionField(name="mug", type="Image"),
+    ]
+    func.create_fields(fields)
+    yield func
+    func.delete()
+
+
 def get_test_credentials() -> Credentials:
     if "NYCKEL_PYTHON_SDK_CLIENT_SECRET" in os.environ:
         credentials = Credentials(
             client_id="python-sdk-test",
             client_secret=os.environ["NYCKEL_PYTHON_SDK_CLIENT_SECRET"],
             server_url="https://www.nyckel-staging.com",
         )
```

### Comparing `nyckel-0.4.3/tests/test_duplicates_handling.py` & `nyckel-0.4.4/tests/test_duplicates_handling.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/tests/test_field_handler.py` & `nyckel-0.4.4/tests/test_field_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/tests/test_image_classification_function.py` & `nyckel-0.4.4/tests/test_image_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/tests/test_image_decoder.py` & `nyckel-0.4.4/tests/test_image_decoder.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/tests/test_image_tags_function.py` & `nyckel-0.4.4/tests/test_image_tags_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/tests/test_label_handler.py` & `nyckel-0.4.4/tests/test_label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/tests/test_sample_handler.py` & `nyckel-0.4.4/tests/test_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/tests/test_tabular_classification_function.py` & `nyckel-0.4.4/tests/test_tabular_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/tests/test_tags_shared.py` & `nyckel-0.4.4/tests/test_tags_shared.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 """ Shared tests for all Tags functions."""
 
-import random
-import string
 import time
 
 import pytest
-from conftest import make_random_image
+from conftest import make_random_image, make_random_tabular, make_random_text
 from nyckel import (
     ClassificationLabel,
     ClassificationPrediction,
     ImageTagsFunction,
     ImageTagsSample,
+    TabularFunctionField,
+    TabularTagsFunction,
+    TabularTagsSample,
     TagsAnnotation,
     TextTagsFunction,
     TextTagsSample,
 )
 
 
-def random_test_image_maker() -> str:
-    return make_random_image()
-
-
-def random_test_text_maker() -> str:
-    return "".join(random.choices(string.ascii_uppercase, k=50))
-
-
 @pytest.mark.parametrize(
     "function_type,function_class",
-    [("image_tags_function", ImageTagsFunction), ("text_tags_function", TextTagsFunction)],
+    [
+        ("image_tags_function", ImageTagsFunction),
+        ("text_tags_function", TextTagsFunction),
+        ("tabular_tags_function", TabularTagsFunction),
+    ],
 )
 class TestFunction:
 
     # Create & Delete happens in the test fixture, and there is no update operation
     # So remains to test read.
 
     def test_read(self, function_type, function_class, auth_test_credentials, request):
@@ -39,21 +36,32 @@
         function_id = func.function_id
         reloaded_function = function_class(function_id, auth_test_credentials)
         assert reloaded_function.function_id == function_id
 
 
 @pytest.mark.parametrize(
     "function_class,sample_data_maker",
-    [(ImageTagsFunction, random_test_image_maker), (TextTagsFunction, random_test_text_maker)],
+    [
+        (ImageTagsFunction, make_random_image),
+        (TextTagsFunction, make_random_text),
+        (TabularTagsFunction, make_random_tabular),
+    ],
 )
 class TestProperties:
 
     def test_all(self, function_class, sample_data_maker, auth_test_credentials):
-        name = "PYTHON-SDK IMAGE TAGS PROPERTIES TEST FUNCTION"
+        name = "PYTHON-SDK TAGS PROPERTIES TEST FUNCTION"
         func = function_class.create(name, auth_test_credentials)
+        if isinstance(func, TabularTagsFunction):
+            fields = [
+                TabularFunctionField(name="name", type="Text"),
+                TabularFunctionField(name="age", type="Number"),
+                TabularFunctionField(name="mug", type="Image"),
+            ]
+            func.create_fields(fields)
         assert func.name == name
         assert func.sample_count == 0
         assert func.label_count == 0
 
         func.create_labels(["cat", "dog"])
         time.sleep(0.5)
         assert func.label_count == 2
@@ -61,22 +69,27 @@
         func.create_samples([sample_data_maker(), sample_data_maker()])
         time.sleep(0.5)
         assert func.sample_count == 2
 
         func.delete()
 
 
-@pytest.mark.parametrize("function_type", ["image_tags_function", "text_tags_function"])
+@pytest.mark.parametrize("function_type", ["image_tags_function", "text_tags_function", "tabular_tags_function"])
 class TestLabels:
 
-    def test_create(self, function_type, request):
+    def test_create_untyped(self, function_type, request):
         func = request.getfixturevalue(function_type)
         label_ids = func.create_labels(["cat", "dog"])
         assert len(label_ids) == 2
 
+    def test_create_typed(self, function_type, request):
+        func = request.getfixturevalue(function_type)
+        label_ids = func.create_labels([ClassificationLabel("cat"), ClassificationLabel("dog")])
+        assert len(label_ids) == 2
+
     def test_read(self, function_type, request):
         func = request.getfixturevalue(function_type)
         label_id = func.create_labels(["dog"])[0]
         label = func.read_label(label_id)
         assert label.name == "dog"
         assert label.id == label_id
 
@@ -93,35 +106,60 @@
         func = request.getfixturevalue(function_type)
         label_id = func.create_labels(["dog"])[0]
         func.delete_labels([label_id])
         time.sleep(0.5)
         labels = func.list_labels()
         assert len(labels) == 0
 
+    def test_strip_whitespaces(self, function_type, request):
+        func = request.getfixturevalue(function_type)
+        func.create_labels(["  cat  "])
+        labels = func.list_labels()
+        assert labels[0].name == "cat"
+
 
 @pytest.mark.parametrize(
     "function_type,sample_data_maker,sample_class",
     [
-        ("image_tags_function", random_test_image_maker, ImageTagsSample),
-        ("text_tags_function", random_test_text_maker, TextTagsSample),
+        ("image_tags_function", make_random_image, ImageTagsSample),
+        ("text_tags_function", make_random_text, TextTagsSample),
+        ("tabular_tags_function_with_fields", make_random_tabular, TabularTagsSample),
     ],
 )
 class TestSamples:
 
-    def test_create(self, function_type, sample_data_maker, sample_class, request):
+    def test_create_untyped(self, function_type, sample_data_maker, sample_class, request):
         func = request.getfixturevalue(function_type)
         sample_ids = func.create_samples([sample_data_maker(), sample_data_maker()])
         assert len(sample_ids) == 2
 
+    def test_create_typed(self, function_type, sample_data_maker, sample_class, request):
+        func = request.getfixturevalue(function_type)
+        sample_ids = func.create_samples(
+            [sample_class(data=sample_data_maker()), sample_class(data=sample_data_maker())]
+        )
+        assert len(sample_ids) == 2
+
+    def test_create_annotated(self, function_type, sample_data_maker, sample_class, request):
+        func = request.getfixturevalue(function_type)
+        sample_ids = func.create_samples([sample_class(data=sample_data_maker(), annotation=[TagsAnnotation("Nice")])])
+        assert len(sample_ids) == 1
+        assert func.label_count == 1  # Labels are created automatically
+
     def test_read(self, function_type, sample_data_maker, sample_class, request):
         func = request.getfixturevalue(function_type)
-        sample_id = func.create_samples([sample_data_maker()])[0]
+        sample_to_be_created = sample_data_maker()
+        sample_id = func.create_samples([sample_to_be_created])[0]
         time.sleep(0.5)
         sample = func.read_sample(sample_id)
         assert sample.id == sample_id
+        if function_type == "text_tags_function":
+            # We can't test for exact equality for image and (tabular with image fields) because
+            # the image data is recoded by the server.
+            assert sample.data == sample_to_be_created
 
     def test_update(self, function_type, sample_data_maker, sample_class, request):
         func = request.getfixturevalue(function_type)
         func.create_labels(["Nice"])
         original_sample = sample_class(data=sample_data_maker())
         sample_id = func.create_samples([original_sample])[0]
         time.sleep(0.5)
@@ -195,16 +233,17 @@
         assert TagsAnnotation("label1") in sample2.annotation
         assert TagsAnnotation("label2", present=False) in sample2.annotation
 
 
 @pytest.mark.parametrize(
     "function_type,sample_data_maker,sample_class",
     [
-        ("image_tags_function", random_test_image_maker, ImageTagsSample),
-        ("text_tags_function", random_test_text_maker, TextTagsSample),
+        ("image_tags_function", make_random_image, ImageTagsSample),
+        ("text_tags_function", make_random_text, TextTagsSample),
+        ("tabular_tags_function_with_fields", make_random_tabular, TabularTagsSample),
     ],
 )
 class TestEndToEnd:
 
     def test_end_to_end(self, function_type, sample_data_maker, sample_class, request):
         func = request.getfixturevalue(function_type)
 
@@ -214,15 +253,15 @@
         samples = [
             sample_class(data=sample_data_maker(), annotation=[TagsAnnotation("Nice")]),
             sample_class(data=sample_data_maker(), annotation=[TagsAnnotation("Nice"), TagsAnnotation("Boo")]),
             sample_class(data=sample_data_maker(), annotation=[TagsAnnotation("Boo")]),
             sample_class(data=sample_data_maker(), annotation=[TagsAnnotation("Boo")]),
             sample_class(data=sample_data_maker(), annotation=[]),
         ]
-
+        assert not func.has_trained_model()
         func.create_samples(samples)
 
         while not func.has_trained_model():
             print("-> No trained model yet. Sleeping 1 sec...")
             time.sleep(1)
 
         predictions = func.invoke([sample_data_maker(), sample_data_maker(), sample_data_maker()])
```

### Comparing `nyckel-0.4.3/tests/test_text_classification_function.py` & `nyckel-0.4.4/tests/test_text_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/tests/test_white_background.py` & `nyckel-0.4.4/tests/test_white_background.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/tests/fixtures/flower.jpg` & `nyckel-0.4.4/tests/fixtures/flower.jpg`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/tests/fixtures/mixed-alpha-background.png` & `nyckel-0.4.4/tests/fixtures/mixed-alpha-background.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/.gitignore` & `nyckel-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/LICENSE` & `nyckel-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/README.md` & `nyckel-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.3/pyproject.toml` & `nyckel-0.4.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 [project]
 name = "nyckel"
-version = "0.4.3"
+version = "0.4.4"
 authors = [{ name = "Oscar Beijbom", email = "oscar@nyckel.com" }]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `nyckel-0.4.3/PKG-INFO` & `nyckel-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nyckel
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python package for the Nyckel API
 Project-URL: Homepage, https://github.com/NyckelAI/python-sdk
 Author-email: Oscar Beijbom <oscar@nyckel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


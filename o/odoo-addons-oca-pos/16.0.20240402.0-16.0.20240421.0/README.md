# Comparing `tmp/odoo_addons_oca_pos-16.0.20240402.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_pos-16.0.20240421.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1713 bytes, number of entries: 4
--rw-r--r--  2.0 unx     3261 b- defN 24-Apr-03 05:14 odoo_addons_oca_pos-16.0.20240402.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 05:14 odoo_addons_oca_pos-16.0.20240402.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 05:14 odoo_addons_oca_pos-16.0.20240402.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 24-Apr-03 05:14 odoo_addons_oca_pos-16.0.20240402.0.dist-info/RECORD
-4 files, 3739 bytes uncompressed, 955 bytes compressed:  74.5%
+Zip file size: 1734 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3426 b- defN 24-Apr-22 04:52 odoo_addons_oca_pos-16.0.20240421.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 04:52 odoo_addons_oca_pos-16.0.20240421.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-22 04:52 odoo_addons_oca_pos-16.0.20240421.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      385 b- defN 24-Apr-22 04:52 odoo_addons_oca_pos-16.0.20240421.0.dist-info/RECORD
+4 files, 3904 bytes uncompressed, 976 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_pos-16.0.20240402.0.dist-info/METADATA
+Filename: odoo_addons_oca_pos-16.0.20240421.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240402.0.dist-info/WHEEL
+Filename: odoo_addons_oca_pos-16.0.20240421.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240402.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_pos-16.0.20240421.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240402.0.dist-info/RECORD
+Filename: odoo_addons_oca_pos-16.0.20240421.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_pos-16.0.20240402.0.dist-info/METADATA` & `odoo_addons_oca_pos-16.0.20240421.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-pos
-Version: 16.0.20240402.0
+Version: 16.0.20240421.0
 Summary: Meta package for oca-pos Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -42,14 +42,16 @@
 Requires-Dist: odoo-addon-pos-product-display-default-code <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-label <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-multi-barcode <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-packaging-container-deposit <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-packaging-multi-barcode <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-quick-info <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-receipt-hide-price <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-pos-receipt-replace-user-by-trigram <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-pos-receipt-replace-user-by-trigram-hr <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-reset-search <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-sale-order-print <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-sale-product-config-no-variant <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-stock-available-online <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-to-weight-by-product-uom <16.1dev,>=16.0dev
 
 UNKNOWN
```


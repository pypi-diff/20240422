# Comparing `tmp/pyqqq-0.8.3.tar.gz` & `tmp/pyqqq-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.8.3.tar", max compression
+gzip compressed data, was "pyqqq-0.8.4.tar", max compression
```

## Comparing `pyqqq-0.8.3.tar` & `pyqqq-0.8.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      588 2024-03-27 01:29:00.427186 pyqqq-0.8.3/README.md
--rw-r--r--   0        0        0      770 2024-04-19 14:39:15.094293 pyqqq-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      668 2024-04-19 02:11:04.495312 pyqqq-0.8.3/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681470 pyqqq-0.8.3/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-06 00:30:01.958621 pyqqq-0.8.3/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    39223 2024-04-15 23:38:31.904216 pyqqq-0.8.3/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-27 01:29:00.428888 pyqqq-0.8.3/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24284 2024-04-19 02:11:04.495645 pyqqq-0.8.3/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-27 03:32:53.313827 pyqqq-0.8.3/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681703 pyqqq-0.8.3/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-03 06:40:50.199892 pyqqq-0.8.3/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-27 01:29:00.429820 pyqqq-0.8.3/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-06 00:30:01.960145 pyqqq-0.8.3/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24453 2024-04-19 02:11:04.496012 pyqqq-0.8.3/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-13 01:10:46.718207 pyqqq-0.8.3/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-15 23:38:31.905431 pyqqq-0.8.3/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-06 03:23:32.374681 pyqqq-0.8.3/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     6677 2024-04-19 02:11:04.496254 pyqqq-0.8.3/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     5939 2024-04-15 23:38:31.905682 pyqqq-0.8.3/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1535 2024-04-15 23:38:31.905855 pyqqq-0.8.3/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4230 2024-04-19 14:37:58.064200 pyqqq-0.8.3/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-12 13:30:35.556769 pyqqq-0.8.3/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-15 23:38:31.906083 pyqqq-0.8.3/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38035 2024-04-19 02:11:04.496835 pyqqq-0.8.3/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-03-06 03:23:38.166158 pyqqq-0.8.3/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-04-15 23:38:31.906445 pyqqq-0.8.3/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3205 2024-04-15 23:38:31.906508 pyqqq-0.8.3/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 21:29:24.457837 pyqqq-0.8.3/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 13:30:35.556892 pyqqq-0.8.3/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-28 02:16:13.684707 pyqqq-0.8.3/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-27 01:29:00.430437 pyqqq-0.8.3/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-02 21:29:24.458374 pyqqq-0.8.3/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0    10571 2024-04-19 02:11:04.497052 pyqqq-0.8.3/pyqqq/utils/mock_api.py
--rw-r--r--   0        0        0     1425 2024-02-28 02:16:13.684870 pyqqq-0.8.3/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.8.4/README.md
+-rw-r--r--   0        0        0      770 2024-04-22 04:52:47.355214 pyqqq-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-04-16 05:13:25.694767 pyqqq-0.8.4/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.8.4/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.8.4/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.8.4/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.8.4/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24284 2024-04-16 05:02:35.915572 pyqqq-0.8.4/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.8.4/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.8.4/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.8.4/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.8.4/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.8.4/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24390 2024-04-22 04:52:35.372119 pyqqq-0.8.4/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.8.4/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.8.4/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.8.4/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     6677 2024-04-22 04:52:35.362423 pyqqq-0.8.4/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.8.4/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.8.4/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4230 2024-04-22 04:52:35.362865 pyqqq-0.8.4/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.8.4/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.8.4/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.8.4/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.8.4/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.8.4/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3205 2024-04-16 02:15:48.378231 pyqqq-0.8.4/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.8.4/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.8.4/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.8.4/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.8.4/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.8.4/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.8.4/pyqqq/utils/mock_api.py
+-rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.8.4/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.8.4/PKG-INFO
```

### Comparing `pyqqq-0.8.3/README.md` & `pyqqq-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyproject.toml` & `pyqqq-0.8.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.8.3"
+version = "0.8.4"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.8.3/pyqqq/__init__.py` & `pyqqq-0.8.4/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.8.4/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.8.4/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.8.4/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.8.4/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.8.4/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.8.4/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.8.4/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.8.4/pyqqq/brokerage/kis/simple.py`

 * *Files 3% similar despite different names*

```diff
@@ -581,29 +581,28 @@
             for item in r["output"]:
                 filled_amount = int(item.get("tot_ccld_amt", 0))
                 filled_quantity = int(item.get("tot_ccld_qty", 0))
                 filled_price = (
                     filled_amount // filled_quantity if filled_quantity > 0 else 0
                 )
                 asset_code = item["pdno"]
-                side = (
-                    OrderSide.SELL if item["sll_buy_dvsn_cd"] == "01" else OrderSide.BUY
-                )
 
                 order = KISStockOrder(
                     order_no=item["odno"],
                     asset_code=asset_code,
-                    side=side,
+                    side=self._get_order_side_code(item["sll_buy_dvsn_cd"]),
                     price=int(item["ord_unpr"]),
                     filled_price=filled_price,
                     current_price=0,
                     quantity=int(item["ord_qty"]),
                     filled_quantity=filled_quantity,
                     pending_quantity=item["psbl_qty"],
                     order_time=item["ord_tmd"],
+                    order_type=self._get_order_type(item["ord_dvsn_cd"]),
+                    req_type=self._get_req_type(item["rvse_cncl_dvsn_name"]),
                 )
 
                 asset_codes.append(asset_code)
                 result.append(order)
 
             if r["tr_cont"] in ["F", "M"]:
                 ctx_area_fk100 = r["ctx_area_fk100"]
@@ -634,56 +633,14 @@
         fetching = True
         ctx_area_fk100 = ""
         ctx_area_nk100 = ""
         tr_cont = ""
 
         pending_order_list = [item.order_no for item in self.get_pending_orders()]
 
-        def __get_order_side_code(sll_buy_dvsn_cd: str) -> OrderSide:
-            if sll_buy_dvsn_cd == "01":
-                return OrderSide.SELL
-            elif sll_buy_dvsn_cd == "02":
-                return OrderSide.BUY
-            else:
-                raise ValueError("지원하지 않는 주문 방향입니다.")
-
-        def __get_req_type(sll_buy_dvsn_cd_name: str) -> OrderRequestType:
-            if "취소" in sll_buy_dvsn_cd_name:
-                return OrderRequestType.CANCEL
-            elif "정정" in sll_buy_dvsn_cd_name:
-                return OrderRequestType.MODIFY
-            else:
-                return OrderRequestType.NEW
-
-        def __get_order_type(ord_dvsn_cd: str) -> OrderType:
-            if ord_dvsn_cd == "00":
-                return OrderType.LIMIT
-            elif ord_dvsn_cd == "01":
-                return OrderType.MARKET
-            elif ord_dvsn_cd == "02":
-                return OrderType.LIMIT_CONDITIONAL
-            elif ord_dvsn_cd == "03":
-                return OrderType.BEST_PRICE
-            elif ord_dvsn_cd == "04":
-                return OrderType.PRIMARY_PRICE
-            elif ord_dvsn_cd == "11":
-                return OrderType.LIMIT_IOC
-            elif ord_dvsn_cd == "12":
-                return OrderType.LIMIT_FOK
-            elif ord_dvsn_cd == "13":
-                return OrderType.MARKET_IOC
-            elif ord_dvsn_cd == "14":
-                return OrderType.MARKET_FOK
-            elif ord_dvsn_cd == "15":
-                return OrderType.BEST_PRICE_IOC
-            elif ord_dvsn_cd == "16":
-                return OrderType.BEST_PRICE_FOK
-            else:
-                raise ValueError(f"지원하지 않는 주문 유형입니다. {ord_dvsn_cd}")
-
         if target_date is None:
             target_date = dtm.date.today()
 
         while fetching:
             r = self.stock_api.inquire_daily_ccld(
                 self.account_no,
                 self.account_product_code,
@@ -705,26 +662,26 @@
                 filled_price = (
                     filled_amount // filled_quantity if filled_quantity > 0 else 0
                 )
 
                 order = KISStockOrder(
                     order_no=item["odno"],
                     asset_code=item["pdno"],
-                    side=__get_order_side_code(item["sll_buy_dvsn_cd"]),
+                    side=self._get_order_side_code(item["sll_buy_dvsn_cd"]),
                     quantity=quantity,
                     price=int(item["ord_unpr"]),
                     filled_quantity=filled_quantity,
                     filled_price=filled_price,
                     pending_quantity=pending_quantity,
                     order_time=item["ord_tmd"],
                     current_price=0,
                     is_pending=item["odno"] in pending_order_list,
                     org_order_no=item["orgn_odno"],
-                    order_type=__get_order_type(item["ord_dvsn_cd"]),
-                    req_type=__get_req_type(item["sll_buy_dvsn_cd_name"]),
+                    order_type=self._get_order_type(item["ord_dvsn_cd"]),
+                    req_type=self._get_req_type(item["sll_buy_dvsn_cd_name"]),
                 )
                 result.append(order)
 
             if r["tr_cont"] in ["F", "M"]:
                 ctx_area_fk100 = r["ctx_area_fk100"]
                 ctx_area_nk100 = r["ctx_area_nk100"]
                 tr_cont = "N"
@@ -746,7 +703,49 @@
             KISStockOrder: 주문 정보
         """
         result = self.get_today_order_history(order_no=odno)
         if len(result) > 0:
             return result[0]
         else:
             return None
+
+    def _get_order_side_code(self, sll_buy_dvsn_cd: str) -> OrderSide:
+        if sll_buy_dvsn_cd == "01":
+            return OrderSide.SELL
+        elif sll_buy_dvsn_cd == "02":
+            return OrderSide.BUY
+        else:
+            raise ValueError("지원하지 않는 주문 방향입니다.")
+
+    def _get_req_type(self, sll_buy_dvsn_cd_name: str) -> OrderRequestType:
+        if "취소" in sll_buy_dvsn_cd_name:
+            return OrderRequestType.CANCEL
+        elif "정정" in sll_buy_dvsn_cd_name:
+            return OrderRequestType.MODIFY
+        else:
+            return OrderRequestType.NEW
+
+    def _get_order_type(self, ord_dvsn_cd: str) -> OrderType:
+        if ord_dvsn_cd == "00":
+            return OrderType.LIMIT
+        elif ord_dvsn_cd == "01":
+            return OrderType.MARKET
+        elif ord_dvsn_cd == "02":
+            return OrderType.LIMIT_CONDITIONAL
+        elif ord_dvsn_cd == "03":
+            return OrderType.BEST_PRICE
+        elif ord_dvsn_cd == "04":
+            return OrderType.PRIMARY_PRICE
+        elif ord_dvsn_cd == "11":
+            return OrderType.LIMIT_IOC
+        elif ord_dvsn_cd == "12":
+            return OrderType.LIMIT_FOK
+        elif ord_dvsn_cd == "13":
+            return OrderType.MARKET_IOC
+        elif ord_dvsn_cd == "14":
+            return OrderType.MARKET_FOK
+        elif ord_dvsn_cd == "15":
+            return OrderType.BEST_PRICE_IOC
+        elif ord_dvsn_cd == "16":
+            return OrderType.BEST_PRICE_FOK
+        else:
+            raise ValueError(f"지원하지 않는 주문 유형입니다. {ord_dvsn_cd}")
```

### Comparing `pyqqq-0.8.3/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.8.4/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/data/domestic.py` & `pyqqq-0.8.4/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/data/minutes.py` & `pyqqq-0.8.4/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/data/realtime.py` & `pyqqq-0.8.4/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/data/ticks.py` & `pyqqq-0.8.4/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/datatypes.py` & `pyqqq-0.8.4/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/executors/hook.py` & `pyqqq-0.8.4/pyqqq/executors/hook.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/utils/array.py` & `pyqqq-0.8.4/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/utils/compute.py` & `pyqqq-0.8.4/pyqqq/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/utils/display.py` & `pyqqq-0.8.4/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/utils/kvstore.py` & `pyqqq-0.8.4/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/utils/limiter.py` & `pyqqq-0.8.4/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/utils/logger.py` & `pyqqq-0.8.4/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/utils/market_schedule.py` & `pyqqq-0.8.4/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/utils/mock_api.py` & `pyqqq-0.8.4/pyqqq/utils/mock_api.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/pyqqq/utils/retry.py` & `pyqqq-0.8.4/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.3/PKG-INFO` & `pyqqq-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.8.3
+Version: 0.8.4
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


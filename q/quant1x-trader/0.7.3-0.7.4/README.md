# Comparing `tmp/quant1x-trader-0.7.3.tar.gz` & `tmp/quant1x-trader-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant1x-trader-0.7.3.tar", last modified: Mon Feb 19 01:20:53 2024, max compression
+gzip compressed data, was "quant1x-trader-0.7.4.tar", last modified: Mon Mar 18 03:34:24 2024, max compression
```

## Comparing `quant1x-trader-0.7.3.tar` & `quant1x-trader-0.7.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-02-19 01:20:53.941996 quant1x-trader-0.7.3/
--rw-rw-rw-   0        0        0     1087 2023-11-13 03:59:57.000000 quant1x-trader-0.7.3/LICENSE
--rw-rw-rw-   0        0        0     1342 2024-02-19 01:20:53.940991 quant1x-trader-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-12-07 15:33:00.000000 quant1x-trader-0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-19 01:20:53.939487 quant1x-trader-0.7.3/quant1x_trader.egg-info/
--rw-rw-rw-   0        0        0     1342 2024-02-19 01:20:53.000000 quant1x-trader-0.7.3/quant1x_trader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2024-02-19 01:20:53.000000 quant1x-trader-0.7.3/quant1x_trader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-19 01:20:53.000000 quant1x-trader-0.7.3/quant1x_trader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2024-02-19 01:20:53.000000 quant1x-trader-0.7.3/quant1x_trader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-02-19 01:20:53.000000 quant1x-trader-0.7.3/quant1x_trader.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      290 2024-02-19 01:20:53.000000 quant1x-trader-0.7.3/quant1x_trader.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-19 01:20:53.000000 quant1x-trader-0.7.3/quant1x_trader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-19 01:20:53.941996 quant1x-trader-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0     2284 2024-01-21 09:52:15.000000 quant1x-trader-0.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-19 01:20:53.939487 quant1x-trader-0.7.3/trader1x/
--rw-rw-rw-   0        0        0      103 2024-02-19 01:20:42.000000 quant1x-trader-0.7.3/trader1x/__init__.py
--rw-rw-rw-   0        0        0      197 2023-12-11 07:07:15.000000 quant1x-trader-0.7.3/trader1x/__main__.py
--rw-rw-rw-   0        0        0    16143 2024-02-19 01:20:42.000000 quant1x-trader-0.7.3/trader1x/auto.py
--rw-rw-rw-   0        0        0     8648 2024-02-19 01:20:42.000000 quant1x-trader-0.7.3/trader1x/config.py
--rw-rw-rw-   0        0        0     7922 2024-02-19 01:20:42.000000 quant1x-trader-0.7.3/trader1x/context.py
--rw-rw-rw-   0        0        0     1193 2024-02-19 01:20:42.000000 quant1x-trader-0.7.3/trader1x/log4py.py
--rw-rw-rw-   0        0        0    18688 2024-02-19 01:20:42.000000 quant1x-trader-0.7.3/trader1x/proxy.py
--rw-rw-rw-   0        0        0     1266 2024-02-19 01:20:42.000000 quant1x-trader-0.7.3/trader1x/qmt.py
--rw-rw-rw-   0        0        0    19739 2024-02-19 01:20:42.000000 quant1x-trader-0.7.3/trader1x/thinktrader.py
--rw-rw-rw-   0        0        0     1368 2024-02-19 01:20:42.000000 quant1x-trader-0.7.3/trader1x/utils.py
--rw-rw-rw-   0        0        0    38933 2024-01-21 09:52:15.000000 quant1x-trader-0.7.3/trader1x/win32serviceutil.py
+drwxrwxrwx   0        0        0        0 2024-03-18 03:34:24.429702 quant1x-trader-0.7.4/
+-rw-rw-rw-   0        0        0     1087 2023-11-13 03:59:57.000000 quant1x-trader-0.7.4/LICENSE
+-rw-rw-rw-   0        0        0     1342 2024-03-18 03:34:24.428703 quant1x-trader-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-12-07 15:33:00.000000 quant1x-trader-0.7.4/README.md
+drwxrwxrwx   0        0        0        0 2024-03-18 03:34:24.428703 quant1x-trader-0.7.4/quant1x_trader.egg-info/
+-rw-rw-rw-   0        0        0     1342 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      290 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-03-18 03:34:24.000000 quant1x-trader-0.7.4/quant1x_trader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-18 03:34:24.429702 quant1x-trader-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     2284 2024-01-21 09:52:15.000000 quant1x-trader-0.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-18 03:34:24.426701 quant1x-trader-0.7.4/trader1x/
+-rw-rw-rw-   0        0        0      103 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-12-11 07:07:15.000000 quant1x-trader-0.7.4/trader1x/__main__.py
+-rw-rw-rw-   0        0        0    16143 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/auto.py
+-rw-rw-rw-   0        0        0     8648 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/config.py
+-rw-rw-rw-   0        0        0     7922 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/context.py
+-rw-rw-rw-   0        0        0     1193 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/log4py.py
+-rw-rw-rw-   0        0        0    18538 2024-03-18 03:34:16.000000 quant1x-trader-0.7.4/trader1x/proxy.py
+-rw-rw-rw-   0        0        0     1266 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/qmt.py
+-rw-rw-rw-   0        0        0    19739 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/thinktrader.py
+-rw-rw-rw-   0        0        0     1368 2024-02-19 01:20:42.000000 quant1x-trader-0.7.4/trader1x/utils.py
+-rw-rw-rw-   0        0        0    38933 2024-01-21 09:52:15.000000 quant1x-trader-0.7.4/trader1x/win32serviceutil.py
```

### Comparing `quant1x-trader-0.7.3/LICENSE` & `quant1x-trader-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.3/PKG-INFO` & `quant1x-trader-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant1x-trader
-Version: 0.7.3
+Version: 0.7.4
 Summary: Quant1X程序化自动化交易
 Home-page: https://gitee.com/quant1x/trader
 Author: WangFeng
 Author-email: wangfengxy@sina.cn
 License: MIT license
 Keywords: quant1x auto trader
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `quant1x-trader-0.7.3/quant1x_trader.egg-info/PKG-INFO` & `quant1x-trader-0.7.4/quant1x_trader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant1x-trader
-Version: 0.7.3
+Version: 0.7.4
 Summary: Quant1X程序化自动化交易
 Home-page: https://gitee.com/quant1x/trader
 Author: WangFeng
 Author-email: wangfengxy@sina.cn
 License: MIT license
 Keywords: quant1x auto trader
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `quant1x-trader-0.7.3/quant1x_trader.egg-info/SOURCES.txt` & `quant1x-trader-0.7.4/quant1x_trader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.3/setup.py` & `quant1x-trader-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.3/trader1x/auto.py` & `quant1x-trader-0.7.4/trader1x/auto.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.3/trader1x/config.py` & `quant1x-trader-0.7.4/trader1x/config.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.3/trader1x/context.py` & `quant1x-trader-0.7.4/trader1x/context.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.3/trader1x/log4py.py` & `quant1x-trader-0.7.4/trader1x/log4py.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.3/trader1x/proxy.py` & `quant1x-trader-0.7.4/trader1x/proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,74 +109,74 @@
     :return:
     """
     logger.info('{} shutdown...', __application_proxy)
     __trader.close()
     logger.info('{} shutdown...OK', __application_proxy)
 
 
-@app.api_route(__uri_prefix + '/health')
+@app.api_route('/health')
 async def hello(name: str = 'anonymous'):
     """
     探测服务接口(√)
     :param name:
     :return:
     """
     return {rf'hello, {name}'}
 
 
-@app.api_route(__uri_prefix + '/data/subscribe_whole_quote')
+@app.api_route('/data/subscribe_whole_quote')
 async def data_subscribe_whole_quote(code: str = 'SH,SZ'):
     """
     订阅全推行情
     :param code:
     :return:
     """
     code_list = code.split(",")
     data = xtquant.xtdata.subscribe_whole_quote(code_list)
     return {'status': OPERATION_STATUS_SUCCESS, 'message': OPERATION_MESSAGE_SUCCESS, 'seq': data}
 
 
-@app.api_route(__uri_prefix + '/data/unsubscribe_quote')
+@app.api_route('/data/unsubscribe_quote')
 async def data_unsubscribe_quote(seq: str = ''):
     """
     反订阅行情数据
     :param seq: 订阅号
     :return:
     """
     seq_id = int(seq)
     data = xtquant.xtdata.unsubscribe_quote(seq_id)
     return data
 
 
-@app.api_route(__uri_prefix + '/data/tick')
+@app.api_route('/data/tick')
 async def data_full_tick(code: str = 'SH,SZ'):
     """
     获取tick(√)
     :param code:
     :return:
     """
     code_list = code.split(",")
     data = xtquant.xtdata.get_full_tick(code_list)
     return data
 
 
-@app.api_route(__uri_prefix + '/query/asset', methods=['GET', 'POST'])
+@app.api_route('/query/asset', methods=['GET', 'POST'])
 async def query_assets():
     """
     查询总资产(√)
     """
     asset = __trader.query_asset()
     return {"total_asset": asset.total_asset,
             "cash": asset.cash,
             "market_value": asset.market_value,
             "frozen_cash": asset.frozen_cash
             }
 
 
-@app.api_route(__uri_prefix + '/query/holding', methods=['GET', 'POST'])
+@app.api_route('/query/holding', methods=['GET', 'POST'])
 async def query_holding():
     """
     查询当前持仓(√)
     """
     holding = []
     for p in __trader.query_positions():
         holding.append(
@@ -192,15 +192,15 @@
              'yesterday_volume': p.yesterday_volume,
              'avg_price': p.avg_price,
              }
         )
     return holding
 
 
-@app.api_route(__uri_prefix + '/query/trade', methods=['GET', 'POST'])
+@app.api_route('/query/trade', methods=['GET', 'POST'])
 async def query_trade():
     """
     查询当日成交(√)
     """
     trades = __trader.query_trades()
     result = []
     for trade in trades:
@@ -211,15 +211,15 @@
              'traded_price': trade.traded_price,
              'traded_amount': trade.traded_amount,
              'traded_time': base1x.seconds_to_timestamp(trade.traded_time),
              "traded_id": trade.traded_id, "order_sysid": trade.order_sysid})
     return result
 
 
-@app.api_route(__uri_prefix + '/query/order', methods=['GET', 'POST'])
+@app.api_route('/query/order', methods=['GET', 'POST'])
 async def query_order(order_id: str = ''):
     """
     查询当日委托(√)
     :param order_id: 订单id
     """
     order_id = order_id.strip()
     if order_id == '' or order_id == '0':
@@ -260,15 +260,15 @@
     :param status: 状态码, 0-成功, 非0-失败
     :param message: 错误信息
     :return:
     """
     return {'status': status, 'message': message}
 
 
-@app.api_route(__uri_prefix + '/trade/order', methods=['POST'])
+@app.api_route('/trade/order', methods=['POST'])
 async def trade_place_order(direction: str = Form(''),
                             code: str = Form(''),
                             price_type: str = Form(''),
                             price: str = Form(''),
                             volume: str = Form(''),
                             strategy: str = Form(''),
                             remark: str = Form('')
@@ -343,15 +343,15 @@
     order_id = __trader.order(stock_code, trade_direction, stock_volume, stock_price_type, stock_price,
                               strategy_name, order_remark)
     logger.warning('order[{}]: code={}, direction={}, price={}, volume={}, strategy_name={}, order_remark={}', order_id,
                    stock_code, direction, stock_price, stock_volume, strategy_name, order_remark)
     return {'status': status, 'message': message, 'order_id': order_id}
 
 
-@app.api_route(__uri_prefix + '/trade/cancel', methods=['POST'])
+@app.api_route('/trade/cancel', methods=['POST'])
 async def trade_cancel_order(order_id: str = Form('')):
     """
     撤单(√)
     """
     cancel_errno = 20000
     order_id = order_id.strip()
     if order_id == '':
```

### Comparing `quant1x-trader-0.7.3/trader1x/qmt.py` & `quant1x-trader-0.7.4/trader1x/qmt.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.3/trader1x/thinktrader.py` & `quant1x-trader-0.7.4/trader1x/thinktrader.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.3/trader1x/utils.py` & `quant1x-trader-0.7.4/trader1x/utils.py`

 * *Files identical despite different names*

### Comparing `quant1x-trader-0.7.3/trader1x/win32serviceutil.py` & `quant1x-trader-0.7.4/trader1x/win32serviceutil.py`

 * *Files identical despite different names*


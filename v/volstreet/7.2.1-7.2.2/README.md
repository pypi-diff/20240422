# Comparing `tmp/volstreet-7.2.1.tar.gz` & `tmp/volstreet-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-7.2.1.tar", last modified: Fri Apr 19 03:41:58 2024, max compression
+gzip compressed data, was "volstreet-7.2.2.tar", last modified: Mon Apr 22 06:14:37 2024, max compression
```

## Comparing `volstreet-7.2.1.tar` & `volstreet-7.2.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.730476 volstreet-7.2.1/
--rw-rw-rw-   0        0        0     1293 2024-04-19 03:41:58.730476 volstreet-7.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.2.1/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     1104 2024-04-19 03:41:58.730476 volstreet-7.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.644511 volstreet-7.2.1/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.2.1/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.665516 volstreet-7.2.1/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.2.1/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.2.1/volstreet/angel_interface/access_rate_handlers.py
--rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     2713 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    17998 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-7.2.1/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    30608 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.2.1/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.675588 volstreet-7.2.1/volstreet/backtests/
--rw-rw-rw-   0        0        0      157 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.2.1/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    46315 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-7.2.1/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0      972 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/backtests/proxy_functions.py
--rw-rw-rw-   0        0        0       66 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/backtests/state.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.2.1/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-7.2.1/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     2441 2024-04-13 07:18:24.000000 volstreet-7.2.1/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    20783 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     6134 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.690998 volstreet-7.2.1/volstreet/datamodule/
--rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-7.2.1/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     8882 2024-04-13 05:28:03.000000 volstreet-7.2.1/volstreet/datamodule/data_handling.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.2.1/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.2.1/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.2.1/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.690998 volstreet-7.2.1/volstreet/historical_info/
--rw-rw-rw-   0        0        0    18674 2024-04-13 07:50:10.000000 volstreet-7.2.1/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-7.2.1/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.690998 volstreet-7.2.1/volstreet/position_dashboard/
--rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/position_dashboard/__init__.py
--rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/position_dashboard/app.py
--rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/position_dashboard/formatting.py
-drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.707443 volstreet-7.2.1/volstreet/strategies/
--rw-rw-rw-   0        0        0      156 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0    29068 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/strategies/deployment.py
--rw-rw-rw-   0        0        0     5194 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    56285 2024-04-18 03:26:14.000000 volstreet-7.2.1/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     2949 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/strategies/monitoring.py
--rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-7.2.1/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0    90356 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/strategies/strats.py
--rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-7.2.1/volstreet/strategies/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.710445 volstreet-7.2.1/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26268 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0    18977 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    19897 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.720302 volstreet-7.2.1/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-7.2.1/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    13047 2024-04-19 03:39:44.000000 volstreet-7.2.1/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6487 2024-03-14 04:36:05.000000 volstreet-7.2.1/volstreet/vectorized_blackscholes.py
-drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.729474 volstreet-7.2.1/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.2.1/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.2.1/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.2.1/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.2.1/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-7.2.1/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-04-19 03:41:58.730476 volstreet-7.2.1/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-04-19 03:41:58.000000 volstreet-7.2.1/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2584 2024-04-19 03:41:58.000000 volstreet-7.2.1/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 03:41:58.000000 volstreet-7.2.1/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-04-19 03:41:58.000000 volstreet-7.2.1/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 03:41:58.000000 volstreet-7.2.1/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 06:14:37.008657 volstreet-7.2.2/
+-rw-rw-rw-   0        0        0     1293 2024-04-22 06:14:37.008657 volstreet-7.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-7.2.2/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-7.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1104 2024-04-22 06:14:37.008657 volstreet-7.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.898680 volstreet-7.2.2/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-7.2.2/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.930448 volstreet-7.2.2/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-03 08:06:51.000000 volstreet-7.2.2/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     6878 2024-04-01 07:48:55.000000 volstreet-7.2.2/volstreet/angel_interface/access_rate_handlers.py
+-rw-rw-rw-   0        0        0       61 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     2713 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    18049 2024-04-22 01:56:59.000000 volstreet-7.2.2/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-7.2.2/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    30663 2024-04-22 05:33:33.000000 volstreet-7.2.2/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6661 2024-04-01 08:48:27.000000 volstreet-7.2.2/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.946091 volstreet-7.2.2/volstreet/backtests/
+-rw-rw-rw-   0        0        0      157 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0    11155 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-7.2.2/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    46315 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-7.2.2/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0      972 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/backtests/proxy_functions.py
+-rw-rw-rw-   0        0        0       66 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/backtests/state.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-7.2.2/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-7.2.2/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     2441 2024-04-13 07:18:24.000000 volstreet-7.2.2/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    20783 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     6152 2024-04-22 04:46:05.000000 volstreet-7.2.2/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.961761 volstreet-7.2.2/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-7.2.2/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     8882 2024-04-13 05:28:03.000000 volstreet-7.2.2/volstreet/datamodule/data_handling.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-7.2.2/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    27286 2024-03-26 10:23:44.000000 volstreet-7.2.2/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-7.2.2/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.961761 volstreet-7.2.2/volstreet/historical_info/
+-rw-rw-rw-   0        0        0    18674 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-7.2.2/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.961761 volstreet-7.2.2/volstreet/position_dashboard/
+-rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/position_dashboard/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/position_dashboard/app.py
+-rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/position_dashboard/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.977395 volstreet-7.2.2/volstreet/strategies/
+-rw-rw-rw-   0        0        0      156 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0    29068 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/strategies/deployment.py
+-rw-rw-rw-   0        0        0     5194 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    56277 2024-04-22 05:03:30.000000 volstreet-7.2.2/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     2949 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/strategies/monitoring.py
+-rw-rw-rw-   0        0        0    17179 2024-04-10 07:52:35.000000 volstreet-7.2.2/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0    91100 2024-04-22 06:10:10.000000 volstreet-7.2.2/volstreet/strategies/strats.py
+-rw-rw-rw-   0        0        0      349 2024-04-12 11:13:05.000000 volstreet-7.2.2/volstreet/strategies/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.992946 volstreet-7.2.2/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26544 2024-04-22 01:51:54.000000 volstreet-7.2.2/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0    19700 2024-04-22 04:16:47.000000 volstreet-7.2.2/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    19897 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:14:36.992946 volstreet-7.2.2/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-7.2.2/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    13047 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9779 2024-03-14 04:36:05.000000 volstreet-7.2.2/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6487 2024-04-22 01:31:42.000000 volstreet-7.2.2/volstreet/vectorized_blackscholes.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:14:37.008657 volstreet-7.2.2/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-7.2.2/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-7.2.2/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-7.2.2/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-7.2.2/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-7.2.2/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-04-22 06:14:37.008657 volstreet-7.2.2/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-04-22 06:14:36.000000 volstreet-7.2.2/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2584 2024-04-22 06:14:36.000000 volstreet-7.2.2/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 06:14:36.000000 volstreet-7.2.2/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-04-22 06:14:36.000000 volstreet-7.2.2/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-22 06:14:36.000000 volstreet-7.2.2/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-7.2.1/PKG-INFO` & `volstreet-7.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.2.1
+Version: 7.2.2
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.2.1/setup.cfg` & `volstreet-7.2.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 372e 322e 310d 0a61  rsion = 7.2.1..a
+00000020: 7273 696f 6e20 3d20 372e 322e 320d 0a61  rsion = 7.2.2..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-7.2.1/volstreet/angel_interface/access_rate_handlers.py` & `volstreet-7.2.2/volstreet/angel_interface/access_rate_handlers.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/angel_interface/async_interface.py` & `volstreet-7.2.2/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/angel_interface/base_websocket.py` & `volstreet-7.2.2/volstreet/angel_interface/base_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/angel_interface/interface.py` & `volstreet-7.2.2/volstreet/angel_interface/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 
 
 def generate_order_params(
     symbol: str,
     token: str,
     qty: int,
     action: str,
-    price: float | int,
+    price: float | int | str,
     order_tag: str = "",
     stop_loss_order: bool = False,
 ) -> dict:
     """Price can be a str or a float because "market" is an acceptable value for price."""
     action = action.upper()
     order_tag = (
         "Automated Order" if (order_tag == "" or order_tag is None) else order_tag
@@ -214,20 +214,21 @@
                 "price": round(execution_price, 1),
             }
         )
     else:
         order_type, execution_price = (
             ("MARKET", 0) if price == "MARKET" else ("LIMIT", price)
         )
-        execution_price = custom_round(execution_price)
+        if order_type == "LIMIT":
+            execution_price = max(custom_round(execution_price), 0.05)
         params.update(
             {
                 "variety": "NORMAL",
                 "ordertype": order_type,
-                "price": max(execution_price, 0.05),
+                "price": execution_price,
             }
         )
 
     return params
 
 
 def update_order_params(
@@ -266,15 +267,15 @@
 
 
 def place_order(
     symbol: str,
     token: str,
     qty: int,
     action: str,
-    price: str | float,
+    price: str | float | int,
     order_tag: str = "",
     stop_loss_order: bool = False,
 ) -> str:
     params = generate_order_params(
         symbol, token, qty, action, price, order_tag, stop_loss_order
     )
     return _place_order_params(params)
```

### Comparing `volstreet-7.2.1/volstreet/angel_interface/login.py` & `volstreet-7.2.2/volstreet/angel_interface/login.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/angel_interface/order_websocket.py` & `volstreet-7.2.2/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/angel_interface/price_websocket.py` & `volstreet-7.2.2/volstreet/angel_interface/price_websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -634,15 +634,18 @@
                     underlying.name, strike, expiry
                 )
                 subscription_dict[mode].append(call_token)
                 subscription_dict[mode].append(put_token)
         return dict(subscription_dict)
 
     def subscribe_indices(self):
-        self.subscribe(["99926000", "99926009", "99926037", "99926074", "99919000"], 1)
+        self.subscribe(
+            ["99926000", "99926009", "99926037", "99926074", "99919000", "99919012"],
+            mode=1,
+        )
 
     def subscribe_options(
         self, *underlyings, range_of_strikes: int = None, expiry_sub_modes=None
     ):
         for underlying in underlyings:
             strike_range = self.get_active_strike_range(underlying, range_of_strikes)
             subscription_dict = self._prepare_subscription_dict(
```

### Comparing `volstreet-7.2.1/volstreet/angel_interface/smart_connect.py` & `volstreet-7.2.2/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/backtests/database.py` & `volstreet-7.2.2/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/backtests/delta_hedging.py` & `volstreet-7.2.2/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/backtests/delta_optimizer.py` & `volstreet-7.2.2/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/backtests/framework.py` & `volstreet-7.2.2/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-7.2.2/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/backtests/proxy_functions.py` & `volstreet-7.2.2/volstreet/backtests/proxy_functions.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/backtests/tools.py` & `volstreet-7.2.2/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/backtests/trend.py` & `volstreet-7.2.2/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/backtests/underlying_info.py` & `volstreet-7.2.2/volstreet/backtests/underlying_info.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/blackscholes.py` & `volstreet-7.2.2/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/config.py` & `volstreet-7.2.2/volstreet/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 CACHE_INTERVAL = 3  # in seconds
 EXPIRY_FREQUENCIES: dict = {
     "MIDCPNIFTY": 0,
     "FINNIFTY": 1,
     "BANKNIFTY": 2,
     "NIFTY": 3,
     "SENSEX": 4,
+    "BANKEX": 0,
 }
 
 # Create loggers
 setup_logging()
 logger = logging.getLogger("volstreet")
 
 # Get the list of scrips
```

### Comparing `volstreet-7.2.1/volstreet/database_connection.py` & `volstreet-7.2.2/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/datamodule/analysis.py` & `volstreet-7.2.2/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/datamodule/archive.py` & `volstreet-7.2.2/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/datamodule/data_handling.py` & `volstreet-7.2.2/volstreet/datamodule/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/datamodule/eod_client.py` & `volstreet-7.2.2/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/datamodule/gambling.py` & `volstreet-7.2.2/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/datamodule/intraday_data.py` & `volstreet-7.2.2/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/datamodule/stockmock.py` & `volstreet-7.2.2/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/datamodule/trading_assistance.py` & `volstreet-7.2.2/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/dealingroom.py` & `volstreet-7.2.2/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/decorators.py` & `volstreet-7.2.2/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/discord_bot.py` & `volstreet-7.2.2/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/exceptions.py` & `volstreet-7.2.2/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/historical_info/index_expiries.pkl` & `volstreet-7.2.2/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/parallelization.py` & `volstreet-7.2.2/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/performance_tracking.py` & `volstreet-7.2.2/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/position_dashboard/app.py` & `volstreet-7.2.2/volstreet/position_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/position_dashboard/formatting.py` & `volstreet-7.2.2/volstreet/position_dashboard/formatting.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/strategies/deployment.py` & `volstreet-7.2.2/volstreet/strategies/deployment.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/strategies/error_handling.py` & `volstreet-7.2.2/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/strategies/helpers.py` & `volstreet-7.2.2/volstreet/strategies/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -837,25 +837,24 @@
         """Adjusts the recommended qty to account for active qty in order to avoid unnecessary
         orders."""
         for option in self.all_options:
             if option.recommended_qty == 0 and option.active_qty == 0:
                 continue
             option.recommended_qty = option.recommended_qty - option.active_qty
 
-    def enter_positions(self) -> None:
+    def enter_positions(self, at_market: bool) -> None:
         instructions = {
             option: {
                 "action": Action.BUY if option.recommended_qty >= 0 else Action.SELL,
-                "price": option.current_ltp,
                 "quantity_in_lots": abs(option.recommended_qty) / option.lot_size,
                 "order_tag": self.order_tag,
             }
             for option in self.recommended_options
         }
-        execution_details = execute_instructions(instructions)
+        execution_details = execute_instructions(instructions, at_market=at_market)
         for option, avg_price in execution_details.items():
             option.update_active_qty_and_premium(option.recommended_qty, avg_price)
             option.recommended_qty = 0
 
     def reset_trigger_flags(self):
         self.exit_triggers = {"end_time": False, "qty_breach_exit": False}
 
@@ -900,26 +899,25 @@
             breach = (
                 abs(self.aggregate_put_active_qty) + adjustment_qty
             ) > max_qty_shares
         else:
             raise ValueError("Invalid option type")
         return breach
 
-    def exit_positions(self):
+    def exit_positions(self, at_market: bool) -> None:
         """Handles squaring up of the position"""
         instructions = {
             option: {
                 "action": Action.BUY if option.active_qty <= 0 else Action.SELL,
-                "price": option.current_ltp,
                 "quantity_in_lots": abs(option.active_qty) / option.lot_size,
                 "order_tag": self.order_tag,
             }
             for option in self.active_options
         }
-        execution_details = execute_instructions(instructions)
+        execution_details = execute_instructions(instructions, at_market=at_market)
         for option, avg_price in execution_details.items():
             option.update_active_qty_and_premium(-option.active_qty, avg_price)
 
     def record_position_status(self) -> None:
         """Designed to periodically save the position status to a file."""
         """
         Saves the current position status to a JSON file periodically.
```

### Comparing `volstreet-7.2.1/volstreet/strategies/monitoring.py` & `volstreet-7.2.2/volstreet/strategies/monitoring.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/strategies/optimization.py` & `volstreet-7.2.2/volstreet/strategies/optimization.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/strategies/strats.py` & `volstreet-7.2.2/volstreet/strategies/strats.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,28 +290,38 @@
     optimize_gamma: bool = False,
     theta_time_jump_hours: float = 1,  # In hours
     delta_interval_minutes: int | float = 1,
     delta_threshold_pct: float = 0.04,
     hedge_margin: float | None = None,  # eg 0.2
     exit_time: Optional[tuple] = (15, 29),
     use_cache: Optional[bool] = True,
+    at_market: bool = False,
     notification_url: Optional[str] = None,
     strategy_tag: Optional[str] = "Delta hedged strangle",
 ):
     """Theta time jump is defined in hours. Delta interval is in minutes. Delta threshold is in percentage terms
     eg: 0.02 for 2%
     """
 
     # Setting the exposure
     start_time = current_time()
     if hedge_margin is None:
         base_exposure = exposure
     else:
         base_exposure = exposure / (1 + hedge_margin)
 
+    # Entering the main function
+    if time(*exit_time) < current_time().time():
+        notifier(
+            f"{underlying.name} {strategy_tag} not being deployed after exit time",
+            notification_url,
+            "INFO",
+        )
+        return
+
     # Setting the exit time
     if time_to_expiry(underlying.current_expiry, in_days=True) < 1:
         exit_time = min([tuple(exit_time), (14, 40)])
         logger.info(
             f"{underlying.name} exit time changed to {exit_time} because expiry is today"
         )
 
@@ -354,15 +364,15 @@
             logger.info(
                 f"{current_time()} {underlying.name} set active options and set "
                 f"{len(delta_position.all_options)} prospective options"
             )
         delta_position.update_underlying()
         delta_position.set_recommended_qty(target_delta, optimized, optimize_gamma)
         delta_position.adjust_recommended_qty()
-        delta_position.enter_positions()
+        delta_position.enter_positions(at_market=at_market)
         delta_position.reset_trigger_flags()
 
         def interruption_condition():
             # Hard coded 7% of base qty shares as the threshold for interruption
             condition_1 = (
                 (abs(delta_position.aggregate_greeks().delta) > 0.07 * base_qty_shares)
                 if not optimized
@@ -440,15 +450,15 @@
                 delta_position.exit_triggers["qty_breach_exit"] = True
                 message = f"{underlying.name}. Shuffling position."
                 logger.info(message)
 
     # Exiting the position
     message = f"{underlying.name} {strategy_tag} exit time reached."
     notifier(message, notification_url, "INFO")
-    delta_position.exit_positions()
+    delta_position.exit_positions(at_market=at_market)
 
     notify_pnl(
         "delta hedged",
         start_time=start_time,
         underlying=underlying,
         notification_url=notification_url,
     )
@@ -1836,14 +1846,15 @@
     iv_threshold: float,
     take_profit: float,
     scan_exit_time: tuple[int, int],
     exposure: int | float = 0,
     investment: int | float = 0,
     stop_loss: Optional[float] = None,
     trade_exit_time: tuple[int, int] = (10, 10),
+    at_market: bool = False,
     notification_url: Optional[str] = None,
     strategy_tag: Optional[str] = "Quick Strangle",
 ):
 
     if not exposure and not investment:
         raise ValueError("Exposure or investment must be provided")
 
@@ -1944,15 +1955,16 @@
             execution_details = execute_instructions(
                 {
                     position.instrument: {
                         "action": action,
                         "quantity_in_lots": quantity_in_lots,
                         "order_tag": strategy_tag,
                     }
-                }
+                },
+                at_market=at_market,
             )
             call_avg_price, put_avg_price = execution_details[position.instrument]
 
             notifier(
                 f"Entered {underlying.name} {strategy_tag} on {position.instrument} "
                 f"with avg price {call_avg_price + put_avg_price}",
                 notification_url,
@@ -2005,15 +2017,16 @@
         execution_details = execute_instructions(
             {
                 position.instrument: {
                     "action": ~action,
                     "quantity_in_lots": quantity_in_lots,
                     "order_tag": strategy_tag,
                 }
-            }
+            },
+            at_market=at_market,
         )
         call_exit_price, put_exit_price = execution_details[position.instrument]
         exit_price = call_exit_price + put_exit_price
         profit_points = (exit_price - position.initiating_price) * action.num_value
         notifier(
             f"Exited {underlying.name} {strategy_tag} with profit points {profit_points}",
             notification_url,
@@ -2027,14 +2040,15 @@
     exposure: int | float,
     exit_time: tuple[int, int] = (15, 27),
     threshold_movement: Optional[float] = None,
     beta: Optional[float] = 0.8,
     stop_loss: Optional[float] = 0.003,
     max_entries: Optional[int] = 3,
     hedge_offset: Optional[float | bool] = 0.004,
+    at_market: bool = False,
     notification_url: Optional[str] = None,
     strategy_tag: Optional[str] = "Intraday trend",
 ):
     def get_futures_basis(traded_price):
         try:
             underlying.set_future_symbol_tokens()
             fut_1_price, fut_2_price = underlying.fetch_ltp(
@@ -2047,15 +2061,21 @@
         spot_price = underlying.fetch_ltp()
         b1 = traded_price - spot_price
         b2 = fut_1_price - spot_price
         b3 = fut_2_price - fut_1_price
         return b1, b2, b3
 
     # Entering the main function
-
+    if time(*exit_time) < current_time().time():
+        notifier(
+            f"{underlying.name} {strategy_tag} not being deployed after exit time",
+            notification_url,
+            "INFO",
+        )
+        return
     # Start time
     start_time = current_time()
 
     # Quantity
     quantity_in_lots = convert_exposure_to_lots(
         exposure, underlying.fetch_ltp(), underlying.lot_size, 5
     )
@@ -2178,15 +2198,15 @@
             f"{underlying.name} at {price}. "
             f"Stop loss at {stop_loss_price}.",
             notification_url,
             "INFO",
         )
 
         # Entering the positions
-        execution_details = execute_instructions(instructions)
+        execution_details = execute_instructions(instructions, at_market=at_market)
         call_entry_price, put_entry_price = execution_details[atm_synthetic_fut]
         hedge_entry_price = execution_details.get(hedge_instrument, 0)
 
         # Spot-Future basis calculation
         entry_price = atm_strike + call_entry_price - put_entry_price
         traded_basis, spot_future_basis, arbitrage_basis = get_futures_basis(
             entry_price
@@ -2246,15 +2266,15 @@
             instructions[hedge_instrument] = {
                 "action": Action.BUY,
                 "quantity_in_lots": quantity_in_lots,
                 "order_tag": strategy_tag,
                 "square_off_order": True,
             }
 
-        execution_details = execute_instructions(instructions)
+        execution_details = execute_instructions(instructions, at_market=at_market)
         call_exit_price, put_exit_price = execution_details[atm_synthetic_fut]
         hedge_exit_price = execution_details.get(hedge_instrument, 0)
 
         exit_price = atm_strike + call_exit_price - put_exit_price
         hedge_pnl = hedge_entry_price - hedge_exit_price
         pnl = (
             (exit_price - entry_price)
```

### Comparing `volstreet-7.2.1/volstreet/trade_interface/instruments.py` & `volstreet-7.2.2/volstreet/trade_interface/instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,15 @@
             order_ids.append(order_id)
         return order_ids
 
     def generate_order_params(
         self,
         action: Action,
         quantity_in_lots: int,
-        price: float | int,
+        price: float | int | str,
         stop_loss_order: bool = False,
         order_tag: str = "",
     ) -> list[dict]:
         spliced_orders = splice_orders(quantity_in_lots, self.freeze_qty_in_lots)
         return [
             generate_order_params(
                 self.symbol,
@@ -587,19 +587,22 @@
             put_order_ids.append(put_order_id)
         return call_order_ids, put_order_ids
 
     def generate_order_params(
         self,
         action: Action,
         quantity_in_lots: int,
-        price: tuple[float, float],
+        price: tuple[float, float] | str,
         stop_loss_order: bool = False,
         order_tag: str = "",
     ) -> list[dict]:
-        call_price, put_price = price
+        if isinstance(price, str) and price.upper() == "MARKET":
+            call_price = put_price = price
+        else:
+            call_price, put_price = price
         spliced_orders = splice_orders(quantity_in_lots, self.freeze_qty_in_lots)
         return [
             generate_order_params(
                 self.call_symbol,
                 self.call_token,
                 qty * self.lot_size,
                 action.value,
@@ -684,20 +687,23 @@
             put_order_ids.append(put_order_id)
         return call_order_ids, put_order_ids
 
     def generate_order_params(
         self,
         action: Action,
         quantity_in_lots: int,
-        price: tuple[float, float],
+        price: tuple[float, float] | str,
         stop_loss_order: bool = False,
         order_tag: str = "",
     ) -> list[dict]:
 
-        call_price, put_price = price
+        if isinstance(price, str) and price.upper() == "MARKET":
+            call_price = put_price = price
+        else:
+            call_price, put_price = price
 
         spliced_orders = splice_orders(quantity_in_lots, self.freeze_qty_in_lots)
         return [
             generate_order_params(
                 self.call_symbol,
                 self.call_token,
                 qty * self.lot_size,
```

### Comparing `volstreet-7.2.1/volstreet/trade_interface/order_execution.py` & `volstreet-7.2.2/volstreet/trade_interface/order_execution.py`

 * *Files 6% similar despite different names*

```diff
@@ -205,14 +205,23 @@
             for token in (instrument.call_token, instrument.put_token)
         }
         tokens = option_tokens | strangle_tokens
         return fetch_quotes(tokens, structure="dict", from_source=True)
 
     order_params = []
 
+    # If price is present in all the instructions, then we can directly use that
+
+    if all("price" in params for params in instructions.values()):
+        logger.info(f"Prices are present in all instructions. Using them directly.")
+        for instr, params in instructions.items():
+            order_params.extend(instr.generate_order_params(**params))
+        return order_params
+
+    logger.info(f"Fetching quotes to generate order params.")
     quotes = fetch_market_depth([instr for instr in instructions.keys()])
 
     for instr, params in instructions.items():
         action = params["action"]
 
         if isinstance(instr, Option):
             target_price = "best_bid" if action == Action.SELL else "best_ask"
@@ -234,17 +243,17 @@
             else:
                 put_target_key = call_target_key
 
             quote_for_call, quote_for_put = (
                 quotes[instr.call_token],
                 quotes[instr.put_token],
             )
-            call_price, put_price = (
-                quote_for_call[call_target_key],
-                quote_for_put[put_target_key],
+            call_price, put_price = params.pop(
+                "price",
+                (quote_for_call[call_target_key], quote_for_put[put_target_key]),
             )
             if isinstance(instr, SyntheticFuture):
                 call_modifier, put_modifier = (
                     (1 + config.LIMIT_PRICE_BUFFER, 1 - config.LIMIT_PRICE_BUFFER)
                     if action == Action.BUY
                     else (1 - config.LIMIT_PRICE_BUFFER, 1 + config.LIMIT_PRICE_BUFFER)
                 )
@@ -261,15 +270,16 @@
             )
 
     return order_params
 
 
 @timeit()
 def _execute_instructions(
-    instructions: dict[Option | Strangle | Straddle | SyntheticFuture, dict]
+    instructions: dict[Option | Strangle | Straddle | SyntheticFuture, dict],
+    at_market: bool,
 ) -> dict[Option | Strangle | Straddle | SyntheticFuture, float]:
     """Executes orders for a given set of instructions.
     Instructions is a dictionary where the keys are Instrument objects and
     the values are dictionaries containing the order parameters.
     The order parameters MUST contain the following keys:
     - action: Action.BUY or Action.SELL
     - quantity_in_lots: int
@@ -306,14 +316,19 @@
     }
 
     average_prices = {}
 
     # If instructions has at-least one option, we need to execute the orders
     # Or else skip to the next step
     if instructions:
+        if at_market:
+            instructions = {
+                instr: {**params, "price": "MARKET"}
+                for instr, params in instructions.items()
+            }
         order_params = generate_bulk_params(instructions)
         executed_prices = asyncio.run(execute_orders(order_params))
         executed_prices = identify_average_prices(instructions.keys(), executed_prices)
         average_prices.update(executed_prices)
 
     average_prices.update(
         {
@@ -322,19 +337,20 @@
             if instr not in instructions
         }
     )
     return average_prices
 
 
 def execute_instructions(
-    instructions: dict[Option | Strangle | Straddle | SyntheticFuture, dict]
+    instructions: dict[Option | Strangle | Straddle | SyntheticFuture, dict],
+    at_market: bool = False,
 ) -> dict[Option | Strangle | Straddle | SyntheticFuture, float]:
     with order_placement_lock:
         logger.info(f"{threading.current_thread().name} is executing orders.")
-        result = _execute_instructions(instructions)
+        result = _execute_instructions(instructions, at_market)
         return result
 
 
 @timeit()
 def place_option_order_and_notify(
     instrument: Option | Strangle | Straddle | SyntheticFuture,
     action: Action | str,
```

### Comparing `volstreet-7.2.1/volstreet/trade_interface/underlyings.py` & `volstreet-7.2.2/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/utils/change_config.py` & `volstreet-7.2.2/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/utils/communication.py` & `volstreet-7.2.2/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/utils/core.py` & `volstreet-7.2.2/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/utils/data_io.py` & `volstreet-7.2.2/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/utils/scrip_processing.py` & `volstreet-7.2.2/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/vectorized_blackscholes.py` & `volstreet-7.2.2/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/vslogging/formatters.py` & `volstreet-7.2.2/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/vslogging/logging_config.json` & `volstreet-7.2.2/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/vslogging/logging_setup.py` & `volstreet-7.2.2/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet/vslogging/parsing.py` & `volstreet-7.2.2/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-7.2.1/volstreet.egg-info/PKG-INFO` & `volstreet-7.2.2/volstreet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 7.2.1
+Version: 7.2.2
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-7.2.1/volstreet.egg-info/SOURCES.txt` & `volstreet-7.2.2/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*


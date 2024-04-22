# Comparing `tmp/vietfin-0.1.0.tar.gz` & `tmp/vietfin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vietfin-0.1.0.tar", max compression
+gzip compressed data, was "vietfin-0.2.0.tar", max compression
```

## Comparing `vietfin-0.1.0.tar` & `vietfin-0.2.0.tar`

### file list

```diff
@@ -1,117 +1,130 @@
--rw-r--r--   0        0        0     9233 2024-03-19 22:49:00.224607 vietfin-0.1.0/LICENSE
--rw-r--r--   0        0        0     2764 2024-03-19 22:49:00.311157 vietfin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5891 2024-03-19 23:30:33.720116 vietfin-0.1.0/README.md
--rw-r--r--   0        0        0      822 2024-03-19 22:49:00.314149 vietfin-0.1.0/src/vietfin/__init__.py
--rw-r--r--   0        0        0       42 2024-03-19 22:49:00.320506 vietfin-0.1.0/src/vietfin/abstract/__init__.py
--rw-r--r--   0        0        0     1790 2024-03-19 22:49:00.321506 vietfin-0.1.0/src/vietfin/abstract/data.py
--rw-r--r--   0        0        0    10177 2024-03-19 22:49:00.321506 vietfin-0.1.0/src/vietfin/abstract/factory.py
--rw-r--r--   0        0        0     6814 2024-03-19 22:49:00.322503 vietfin-0.1.0/src/vietfin/abstract/interface.py
--rw-r--r--   0        0        0     8470 2024-03-19 22:49:00.323500 vietfin-0.1.0/src/vietfin/abstract/vfobject.py
--rw-r--r--   0        0        0       35 2024-03-19 22:49:00.324530 vietfin-0.1.0/src/vietfin/components/__init__.py
--rw-r--r--   0        0        0     1764 2024-03-19 22:49:00.325496 vietfin-0.1.0/src/vietfin/components/derivatives.py
--rw-r--r--   0        0        0     1884 2024-03-19 22:49:00.327490 vietfin-0.1.0/src/vietfin/components/equity.py
--rw-r--r--   0        0        0      765 2024-03-19 22:49:00.327490 vietfin-0.1.0/src/vietfin/components/equity_calendar.py
--rw-r--r--   0        0        0     1650 2024-03-19 22:49:00.328487 vietfin-0.1.0/src/vietfin/components/equity_discovery.py
--rw-r--r--   0        0        0     2911 2024-03-19 22:49:00.329484 vietfin-0.1.0/src/vietfin/components/equity_fundamental.py
--rw-r--r--   0        0        0     2340 2024-03-19 22:49:00.330483 vietfin-0.1.0/src/vietfin/components/equity_ownership.py
--rw-r--r--   0        0        0     1647 2024-03-19 22:49:00.331511 vietfin-0.1.0/src/vietfin/components/equity_price.py
--rw-r--r--   0        0        0     1557 2024-03-19 22:49:00.332476 vietfin-0.1.0/src/vietfin/components/etf.py
--rw-r--r--   0        0        0     1784 2024-03-19 22:49:00.332476 vietfin-0.1.0/src/vietfin/components/funds.py
--rw-r--r--   0        0        0     2349 2024-03-19 22:49:00.333474 vietfin-0.1.0/src/vietfin/components/index.py
--rw-r--r--   0        0        0      894 2024-03-19 22:49:00.334504 vietfin-0.1.0/src/vietfin/components/news.py
--rw-r--r--   0        0        0       36 2024-03-19 22:49:00.334504 vietfin-0.1.0/src/vietfin/providers/__init__.py
--rw-r--r--   0        0        0       32 2024-03-19 22:49:00.335468 vietfin-0.1.0/src/vietfin/providers/cafef/__init__.py
--rw-r--r--   0        0        0       36 2024-03-19 22:49:00.336467 vietfin-0.1.0/src/vietfin/providers/cafef/models/__init__.py
--rw-r--r--   0        0        0     2810 2024-03-19 22:49:00.337464 vietfin-0.1.0/src/vietfin/providers/cafef/models/equity_ownership_foreign.py
--rw-r--r--   0        0        0     1515 2024-03-19 22:49:00.338461 vietfin-0.1.0/src/vietfin/providers/cafef/models/equity_ownership_prop.py
--rw-r--r--   0        0        0     1641 2024-03-19 22:49:00.339458 vietfin-0.1.0/src/vietfin/providers/cafef/provider.py
--rw-r--r--   0        0        0     3277 2024-03-19 22:49:00.340455 vietfin-0.1.0/src/vietfin/providers/cafef/utils/equity_ownership_foreign.py
--rw-r--r--   0        0        0     3287 2024-03-19 22:49:00.341452 vietfin-0.1.0/src/vietfin/providers/cafef/utils/equity_ownership_prop.py
--rw-r--r--   0        0        0      719 2024-03-19 22:49:00.342451 vietfin-0.1.0/src/vietfin/providers/cafef/utils/helpers.py
--rw-r--r--   0        0        0       31 2024-03-19 22:49:00.342451 vietfin-0.1.0/src/vietfin/providers/dnse/__init__.py
--rw-r--r--   0        0        0       35 2024-03-19 22:49:00.343447 vietfin-0.1.0/src/vietfin/providers/dnse/models/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-19 22:49:00.344445 vietfin-0.1.0/src/vietfin/providers/dnse/models/equity_price_historical.py
--rw-r--r--   0        0        0     2439 2024-03-19 22:49:00.345443 vietfin-0.1.0/src/vietfin/providers/dnse/provider.py
--rw-r--r--   0        0        0       27 2024-03-19 22:49:00.346440 vietfin-0.1.0/src/vietfin/providers/dnse/utils/__init__.py
--rw-r--r--   0        0        0     7218 2024-03-19 22:49:00.347437 vietfin-0.1.0/src/vietfin/providers/dnse/utils/equity_price_historical.py
--rw-r--r--   0        0        0      685 2024-03-19 22:49:00.348434 vietfin-0.1.0/src/vietfin/providers/dnse/utils/helpers.py
--rw-r--r--   0        0        0       36 2024-03-19 22:49:00.349431 vietfin-0.1.0/src/vietfin/providers/fmarket/__init__.py
--rw-r--r--   0        0        0       38 2024-03-19 22:49:00.349431 vietfin-0.1.0/src/vietfin/providers/fmarket/models/__init__.py
--rw-r--r--   0        0        0      618 2024-03-19 22:49:00.350428 vietfin-0.1.0/src/vietfin/providers/fmarket/models/fund_asset_types.py
--rw-r--r--   0        0        0      480 2024-03-19 22:49:00.351426 vietfin-0.1.0/src/vietfin/providers/fmarket/models/fund_historical_nav.py
--rw-r--r--   0        0        0     1345 2024-03-19 22:49:00.352424 vietfin-0.1.0/src/vietfin/providers/fmarket/models/fund_historical_nav_performance.py
--rw-r--r--   0        0        0      771 2024-03-19 22:49:00.352424 vietfin-0.1.0/src/vietfin/providers/fmarket/models/fund_holdings.py
--rw-r--r--   0        0        0      313 2024-03-19 22:49:00.353421 vietfin-0.1.0/src/vietfin/providers/fmarket/models/fund_industries.py
--rw-r--r--   0        0        0     2071 2024-03-19 22:49:00.354418 vietfin-0.1.0/src/vietfin/providers/fmarket/models/fund_search.py
--rw-r--r--   0        0        0     1062 2024-03-19 22:49:00.355415 vietfin-0.1.0/src/vietfin/providers/fmarket/provider.py
--rw-r--r--   0        0        0       51 2024-03-19 22:49:00.356413 vietfin-0.1.0/src/vietfin/providers/fmarket/py.typed
--rw-r--r--   0        0        0       30 2024-03-19 22:49:00.357410 vietfin-0.1.0/src/vietfin/providers/fmarket/utils/__init__.py
--rw-r--r--   0        0        0     4595 2024-03-19 22:49:00.358552 vietfin-0.1.0/src/vietfin/providers/fmarket/utils/funds_historical.py
--rw-r--r--   0        0        0     2482 2024-03-19 22:49:00.359638 vietfin-0.1.0/src/vietfin/providers/fmarket/utils/funds_holdings.py
--rw-r--r--   0        0        0     3742 2024-03-19 22:49:00.360975 vietfin-0.1.0/src/vietfin/providers/fmarket/utils/funds_search.py
--rw-r--r--   0        0        0     1879 2024-03-19 22:49:00.362237 vietfin-0.1.0/src/vietfin/providers/fmarket/utils/helpers.py
--rw-r--r--   0        0        0       32 2024-03-19 22:49:00.363591 vietfin-0.1.0/src/vietfin/providers/ssi/__init__.py
--rw-r--r--   0        0        0       34 2024-03-19 22:49:00.363591 vietfin-0.1.0/src/vietfin/providers/ssi/models/__init__.py
--rw-r--r--   0        0        0      871 2024-03-19 22:49:00.364590 vietfin-0.1.0/src/vietfin/providers/ssi/models/equity_discovery.py
--rw-r--r--   0        0        0      454 2024-03-19 22:49:00.365630 vietfin-0.1.0/src/vietfin/providers/ssi/models/equity_fundamental_income.py
--rw-r--r--   0        0        0      530 2024-03-19 22:49:00.365630 vietfin-0.1.0/src/vietfin/providers/ssi/models/equity_search.py
--rw-r--r--   0        0        0     1114 2024-03-19 22:49:00.366630 vietfin-0.1.0/src/vietfin/providers/ssi/models/etf_historical.py
--rw-r--r--   0        0        0      867 2024-03-19 22:49:00.367626 vietfin-0.1.0/src/vietfin/providers/ssi/models/etf_search.py
--rw-r--r--   0        0        0      844 2024-03-19 22:49:00.368623 vietfin-0.1.0/src/vietfin/providers/ssi/models/index_constituents.py
--rw-r--r--   0        0        0      397 2024-03-19 22:49:00.368623 vietfin-0.1.0/src/vietfin/providers/ssi/models/index_search.py
--rw-r--r--   0        0        0     5978 2024-03-19 22:49:00.369621 vietfin-0.1.0/src/vietfin/providers/ssi/provider.py
--rw-r--r--   0        0        0       26 2024-03-19 22:49:00.370618 vietfin-0.1.0/src/vietfin/providers/ssi/utils/__init__.py
--rw-r--r--   0        0        0     2147 2024-03-19 22:49:00.370618 vietfin-0.1.0/src/vietfin/providers/ssi/utils/equity_discovery.py
--rw-r--r--   0        0        0     4552 2024-03-19 22:49:00.371617 vietfin-0.1.0/src/vietfin/providers/ssi/utils/equity_fundamental_income.py
--rw-r--r--   0        0        0     2355 2024-03-19 22:49:00.372613 vietfin-0.1.0/src/vietfin/providers/ssi/utils/equity_search.py
--rw-r--r--   0        0        0     6120 2024-03-19 22:49:00.373610 vietfin-0.1.0/src/vietfin/providers/ssi/utils/etf_historical.py
--rw-r--r--   0        0        0     2154 2024-03-19 22:49:00.374607 vietfin-0.1.0/src/vietfin/providers/ssi/utils/etf_search.py
--rw-r--r--   0        0        0      868 2024-03-19 22:49:00.374607 vietfin-0.1.0/src/vietfin/providers/ssi/utils/helpers.py
--rw-r--r--   0        0        0     1988 2024-03-19 22:49:00.375605 vietfin-0.1.0/src/vietfin/providers/ssi/utils/index_constituents.py
--rw-r--r--   0        0        0     2322 2024-03-19 22:49:00.376603 vietfin-0.1.0/src/vietfin/providers/ssi/utils/index_search.py
--rw-r--r--   0        0        0       31 2024-03-19 22:49:00.377599 vietfin-0.1.0/src/vietfin/providers/tcbs/__init__.py
--rw-r--r--   0        0        0       35 2024-03-19 22:49:00.377599 vietfin-0.1.0/src/vietfin/providers/tcbs/models/__init__.py
--rw-r--r--   0        0        0     1713 2024-03-19 22:49:00.378974 vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_calendar_events.py
--rw-r--r--   0        0        0      982 2024-03-19 22:49:00.379973 vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_fundamental_dividends.py
--rw-r--r--   0        0        0     1870 2024-03-19 22:49:00.380837 vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_fundamental_income.py
--rw-r--r--   0        0        0      588 2024-03-19 22:49:00.380837 vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_fundamental_management.py
--rw-r--r--   0        0        0      630 2024-03-19 22:49:00.381835 vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_fundamental_ratios.py
--rw-r--r--   0        0        0     2048 2024-03-19 22:49:00.382833 vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_ownership_insider_trading.py
--rw-r--r--   0        0        0      419 2024-03-19 22:49:00.382833 vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_ownership_major_holders.py
--rw-r--r--   0        0        0      637 2024-03-19 22:49:00.383920 vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_price_historical.py
--rw-r--r--   0        0        0      729 2024-03-19 22:49:00.384827 vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_price_quote.py
--rw-r--r--   0        0        0     1406 2024-03-19 22:49:00.384827 vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_profile.py
--rw-r--r--   0        0        0      918 2024-03-19 22:49:00.385825 vietfin-0.1.0/src/vietfin/providers/tcbs/models/news_company.py
--rw-r--r--   0        0        0     8600 2024-03-19 22:49:00.386823 vietfin-0.1.0/src/vietfin/providers/tcbs/provider.py
--rw-r--r--   0        0        0       27 2024-03-19 22:49:00.387819 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/__init__.py
--rw-r--r--   0        0        0     3071 2024-03-19 22:49:00.387819 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_calendar_events.py
--rw-r--r--   0        0        0     3245 2024-03-19 22:49:00.388817 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_fundamental_dividends.py
--rw-r--r--   0        0        0     3472 2024-03-19 22:49:00.389815 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_fundamental_income.py
--rw-r--r--   0        0        0     2895 2024-03-19 22:49:00.390812 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_fundamental_management.py
--rw-r--r--   0        0        0     2651 2024-03-19 22:49:00.391809 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_fundamental_ratios.py
--rw-r--r--   0        0        0     3324 2024-03-19 22:49:00.392792 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_ownership_insider_trading.py
--rw-r--r--   0        0        0     2253 2024-03-19 22:49:00.392792 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_ownership_major_holders.py
--rw-r--r--   0        0        0     5528 2024-03-19 22:49:00.393791 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_price_historical.py
--rw-r--r--   0        0        0     3110 2024-03-19 22:49:00.395129 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_price_quote.py
--rw-r--r--   0        0        0     2383 2024-03-19 22:49:00.396128 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_profile.py
--rw-r--r--   0        0        0      507 2024-03-19 22:49:00.396128 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/helpers.py
--rw-r--r--   0        0        0     3017 2024-03-19 22:49:00.398122 vietfin-0.1.0/src/vietfin/providers/tcbs/utils/news_company.py
--rw-r--r--   0        0        0       41 2024-03-19 22:49:00.398122 vietfin-0.1.0/src/vietfin/providers/vdsc/__init__.py
--rw-r--r--   0        0        0       45 2024-03-19 22:49:00.399120 vietfin-0.1.0/src/vietfin/providers/vdsc/models/__init__.py
--rw-r--r--   0        0        0     2648 2024-03-19 22:49:00.400117 vietfin-0.1.0/src/vietfin/providers/vdsc/models/derivatives_futures_quote.py
--rw-r--r--   0        0        0     1003 2024-03-19 22:49:00.401115 vietfin-0.1.0/src/vietfin/providers/vdsc/provider.py
--rw-r--r--   0        0        0       37 2024-03-19 22:49:00.402112 vietfin-0.1.0/src/vietfin/providers/vdsc/utils/__init__.py
--rw-r--r--   0        0        0     3666 2024-03-19 22:49:00.402112 vietfin-0.1.0/src/vietfin/providers/vdsc/utils/derivatives_futures_quote.py
--rw-r--r--   0        0        0     2175 2024-03-19 22:49:00.403110 vietfin-0.1.0/src/vietfin/providers/vdsc/utils/helpers.py
--rw-r--r--   0        0        0       35 2024-03-19 22:49:00.404106 vietfin-0.1.0/src/vietfin/providers/wifeed/__init__.py
--rw-r--r--   0        0        0       37 2024-03-19 22:49:00.405104 vietfin-0.1.0/src/vietfin/providers/wifeed/models/__init__.py
--rw-r--r--   0        0        0      329 2024-03-19 22:49:00.406101 vietfin-0.1.0/src/vietfin/providers/wifeed/models/equity_search.py
--rw-r--r--   0        0        0      693 2024-03-19 22:49:00.406101 vietfin-0.1.0/src/vietfin/providers/wifeed/provider.py
--rw-r--r--   0        0        0       31 2024-03-19 22:49:00.407098 vietfin-0.1.0/src/vietfin/providers/wifeed/utils/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-19 22:49:00.408096 vietfin-0.1.0/src/vietfin/providers/wifeed/utils/equity_search.py
--rw-r--r--   0        0        0       23 2024-03-19 22:49:00.408096 vietfin-0.1.0/src/vietfin/providers/wifeed/utils/helpers.py
--rw-r--r--   0        0        0       51 2024-03-19 22:49:00.409094 vietfin-0.1.0/src/vietfin/py.typed
--rw-r--r--   0        0        0       32 2024-03-19 22:49:00.409094 vietfin-0.1.0/src/vietfin/utils/__init__.py
--rw-r--r--   0        0        0      617 2024-03-19 22:49:00.410091 vietfin-0.1.0/src/vietfin/utils/errors.py
--rw-r--r--   0        0        0     9183 2024-03-19 22:49:00.411088 vietfin-0.1.0/src/vietfin/utils/helpers.py
--rw-r--r--   0        0        0     7056 1970-01-01 00:00:00.000000 vietfin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9233 2024-03-19 22:49:00.224607 vietfin-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2611 2024-04-22 00:06:11.243191 vietfin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6290 2024-04-22 00:06:11.215538 vietfin-0.2.0/README.md
+-rw-r--r--   0        0        0      822 2024-03-19 22:49:00.314149 vietfin-0.2.0/src/vietfin/__init__.py
+-rw-r--r--   0        0        0       42 2024-03-19 22:49:00.320506 vietfin-0.2.0/src/vietfin/abstract/__init__.py
+-rw-r--r--   0        0        0     1790 2024-03-19 22:49:00.321506 vietfin-0.2.0/src/vietfin/abstract/data.py
+-rw-r--r--   0        0        0    10957 2024-04-22 00:06:11.243191 vietfin-0.2.0/src/vietfin/abstract/factory.py
+-rw-r--r--   0        0        0     7294 2024-04-22 00:06:11.243191 vietfin-0.2.0/src/vietfin/abstract/interface.py
+-rw-r--r--   0        0        0     8468 2024-04-22 00:06:11.243191 vietfin-0.2.0/src/vietfin/abstract/vfobject.py
+-rw-r--r--   0        0        0       35 2024-03-19 22:49:00.324530 vietfin-0.2.0/src/vietfin/components/__init__.py
+-rw-r--r--   0        0        0     2825 2024-04-22 00:06:11.243191 vietfin-0.2.0/src/vietfin/components/derivatives.py
+-rw-r--r--   0        0        0     1884 2024-03-19 22:49:00.327490 vietfin-0.2.0/src/vietfin/components/equity.py
+-rw-r--r--   0        0        0      765 2024-03-19 22:49:00.327490 vietfin-0.2.0/src/vietfin/components/equity_calendar.py
+-rw-r--r--   0        0        0     1631 2024-04-22 00:06:11.247705 vietfin-0.2.0/src/vietfin/components/equity_discovery.py
+-rw-r--r--   0        0        0     2911 2024-03-19 22:49:00.329484 vietfin-0.2.0/src/vietfin/components/equity_fundamental.py
+-rw-r--r--   0        0        0     2340 2024-03-19 22:49:00.330483 vietfin-0.2.0/src/vietfin/components/equity_ownership.py
+-rw-r--r--   0        0        0     1647 2024-03-19 22:49:00.331511 vietfin-0.2.0/src/vietfin/components/equity_price.py
+-rw-r--r--   0        0        0     1557 2024-03-19 22:49:00.332476 vietfin-0.2.0/src/vietfin/components/etf.py
+-rw-r--r--   0        0        0     1784 2024-03-19 22:49:00.332476 vietfin-0.2.0/src/vietfin/components/funds.py
+-rw-r--r--   0        0        0     2349 2024-03-19 22:49:00.333474 vietfin-0.2.0/src/vietfin/components/index.py
+-rw-r--r--   0        0        0      894 2024-03-19 22:49:00.334504 vietfin-0.2.0/src/vietfin/components/news.py
+-rw-r--r--   0        0        0       36 2024-03-19 22:49:00.334504 vietfin-0.2.0/src/vietfin/providers/__init__.py
+-rw-r--r--   0        0        0       32 2024-03-19 22:49:00.335468 vietfin-0.2.0/src/vietfin/providers/cafef/__init__.py
+-rw-r--r--   0        0        0       36 2024-03-19 22:49:00.336467 vietfin-0.2.0/src/vietfin/providers/cafef/models/__init__.py
+-rw-r--r--   0        0        0     2810 2024-03-19 22:49:00.337464 vietfin-0.2.0/src/vietfin/providers/cafef/models/equity_ownership_foreign.py
+-rw-r--r--   0        0        0     1515 2024-03-19 22:49:00.338461 vietfin-0.2.0/src/vietfin/providers/cafef/models/equity_ownership_prop.py
+-rw-r--r--   0        0        0     1641 2024-03-19 22:49:00.339458 vietfin-0.2.0/src/vietfin/providers/cafef/provider.py
+-rw-r--r--   0        0        0     3292 2024-04-22 00:06:11.247705 vietfin-0.2.0/src/vietfin/providers/cafef/utils/equity_ownership_foreign.py
+-rw-r--r--   0        0        0     3296 2024-04-22 00:06:11.247705 vietfin-0.2.0/src/vietfin/providers/cafef/utils/equity_ownership_prop.py
+-rw-r--r--   0        0        0      719 2024-03-19 22:49:00.342451 vietfin-0.2.0/src/vietfin/providers/cafef/utils/helpers.py
+-rw-r--r--   0        0        0       31 2024-03-19 22:49:00.342451 vietfin-0.2.0/src/vietfin/providers/dnse/__init__.py
+-rw-r--r--   0        0        0       35 2024-03-19 22:49:00.343447 vietfin-0.2.0/src/vietfin/providers/dnse/models/__init__.py
+-rw-r--r--   0        0        0     1163 2024-04-22 00:06:11.247705 vietfin-0.2.0/src/vietfin/providers/dnse/models/equity_price_historical.py
+-rw-r--r--   0        0        0     2439 2024-03-19 22:49:00.345443 vietfin-0.2.0/src/vietfin/providers/dnse/provider.py
+-rw-r--r--   0        0        0       27 2024-03-19 22:49:00.346440 vietfin-0.2.0/src/vietfin/providers/dnse/utils/__init__.py
+-rw-r--r--   0        0        0     7227 2024-04-22 00:06:11.247705 vietfin-0.2.0/src/vietfin/providers/dnse/utils/equity_price_historical.py
+-rw-r--r--   0        0        0      685 2024-03-19 22:49:00.348434 vietfin-0.2.0/src/vietfin/providers/dnse/utils/helpers.py
+-rw-r--r--   0        0        0       36 2024-03-19 22:49:00.349431 vietfin-0.2.0/src/vietfin/providers/fmarket/__init__.py
+-rw-r--r--   0        0        0       38 2024-03-19 22:49:00.349431 vietfin-0.2.0/src/vietfin/providers/fmarket/models/__init__.py
+-rw-r--r--   0        0        0      618 2024-03-19 22:49:00.350428 vietfin-0.2.0/src/vietfin/providers/fmarket/models/fund_asset_types.py
+-rw-r--r--   0        0        0      480 2024-03-19 22:49:00.351426 vietfin-0.2.0/src/vietfin/providers/fmarket/models/fund_historical_nav.py
+-rw-r--r--   0        0        0     1345 2024-03-19 22:49:00.352424 vietfin-0.2.0/src/vietfin/providers/fmarket/models/fund_historical_nav_performance.py
+-rw-r--r--   0        0        0      771 2024-03-19 22:49:00.352424 vietfin-0.2.0/src/vietfin/providers/fmarket/models/fund_holdings.py
+-rw-r--r--   0        0        0      313 2024-03-19 22:49:00.353421 vietfin-0.2.0/src/vietfin/providers/fmarket/models/fund_industries.py
+-rw-r--r--   0        0        0     2071 2024-03-19 22:49:00.354418 vietfin-0.2.0/src/vietfin/providers/fmarket/models/fund_search.py
+-rw-r--r--   0        0        0     1062 2024-03-19 22:49:00.355415 vietfin-0.2.0/src/vietfin/providers/fmarket/provider.py
+-rw-r--r--   0        0        0       51 2024-03-19 22:49:00.356413 vietfin-0.2.0/src/vietfin/providers/fmarket/py.typed
+-rw-r--r--   0        0        0       30 2024-03-19 22:49:00.357410 vietfin-0.2.0/src/vietfin/providers/fmarket/utils/__init__.py
+-rw-r--r--   0        0        0     4604 2024-04-22 00:06:11.247705 vietfin-0.2.0/src/vietfin/providers/fmarket/utils/funds_historical.py
+-rw-r--r--   0        0        0     2491 2024-04-22 00:06:11.252709 vietfin-0.2.0/src/vietfin/providers/fmarket/utils/funds_holdings.py
+-rw-r--r--   0        0        0     3751 2024-04-22 00:06:11.252709 vietfin-0.2.0/src/vietfin/providers/fmarket/utils/funds_search.py
+-rw-r--r--   0        0        0     1811 2024-04-22 00:06:11.252709 vietfin-0.2.0/src/vietfin/providers/fmarket/utils/helpers.py
+-rw-r--r--   0        0        0       31 2024-04-22 00:06:11.252709 vietfin-0.2.0/src/vietfin/providers/ssi/__init__.py
+-rw-r--r--   0        0        0       34 2024-03-19 22:49:00.363591 vietfin-0.2.0/src/vietfin/providers/ssi/models/__init__.py
+-rw-r--r--   0        0        0     2178 2024-04-22 00:06:11.252709 vietfin-0.2.0/src/vietfin/providers/ssi/models/derivatives_coveredwarrant_search.py
+-rw-r--r--   0        0        0     3396 2024-04-22 00:06:11.252709 vietfin-0.2.0/src/vietfin/providers/ssi/models/derivatives_futures_quote.py
+-rw-r--r--   0        0        0     1526 2024-04-22 00:06:11.252709 vietfin-0.2.0/src/vietfin/providers/ssi/models/derivatives_futures_search.py
+-rw-r--r--   0        0        0      872 2024-04-22 00:06:11.252709 vietfin-0.2.0/src/vietfin/providers/ssi/models/equity_discovery.py
+-rw-r--r--   0        0        0      454 2024-03-19 22:49:00.365630 vietfin-0.2.0/src/vietfin/providers/ssi/models/equity_fundamental_income.py
+-rw-r--r--   0        0        0      530 2024-03-19 22:49:00.365630 vietfin-0.2.0/src/vietfin/providers/ssi/models/equity_search.py
+-rw-r--r--   0        0        0     1138 2024-04-22 00:06:11.252709 vietfin-0.2.0/src/vietfin/providers/ssi/models/etf_historical.py
+-rw-r--r--   0        0        0      867 2024-03-19 22:49:00.367626 vietfin-0.2.0/src/vietfin/providers/ssi/models/etf_search.py
+-rw-r--r--   0        0        0      844 2024-03-19 22:49:00.368623 vietfin-0.2.0/src/vietfin/providers/ssi/models/index_constituents.py
+-rw-r--r--   0        0        0      397 2024-03-19 22:49:00.368623 vietfin-0.2.0/src/vietfin/providers/ssi/models/index_search.py
+-rw-r--r--   0        0        0     7604 2024-04-22 00:06:11.257335 vietfin-0.2.0/src/vietfin/providers/ssi/provider.py
+-rw-r--r--   0        0        0       26 2024-03-19 22:49:00.370618 vietfin-0.2.0/src/vietfin/providers/ssi/utils/__init__.py
+-rw-r--r--   0        0        0     2395 2024-04-22 00:06:11.258327 vietfin-0.2.0/src/vietfin/providers/ssi/utils/derivatives_coveredwarrant_search.py
+-rw-r--r--   0        0        0     3512 2024-04-22 00:06:11.258327 vietfin-0.2.0/src/vietfin/providers/ssi/utils/derivatives_futures_quote.py
+-rw-r--r--   0        0        0     2391 2024-04-22 00:06:11.259323 vietfin-0.2.0/src/vietfin/providers/ssi/utils/derivatives_futures_search.py
+-rw-r--r--   0        0        0     2699 2024-04-22 00:06:11.260320 vietfin-0.2.0/src/vietfin/providers/ssi/utils/equity_discovery.py
+-rw-r--r--   0        0        0     4594 2024-04-22 00:06:11.260762 vietfin-0.2.0/src/vietfin/providers/ssi/utils/equity_fundamental_income.py
+-rw-r--r--   0        0        0     2364 2024-04-22 00:06:11.260762 vietfin-0.2.0/src/vietfin/providers/ssi/utils/equity_search.py
+-rw-r--r--   0        0        0     6129 2024-04-22 00:06:11.260762 vietfin-0.2.0/src/vietfin/providers/ssi/utils/etf_historical.py
+-rw-r--r--   0        0        0     2164 2024-04-22 00:06:11.260762 vietfin-0.2.0/src/vietfin/providers/ssi/utils/etf_search.py
+-rw-r--r--   0        0        0      868 2024-03-19 22:49:00.374607 vietfin-0.2.0/src/vietfin/providers/ssi/utils/helpers.py
+-rw-r--r--   0        0        0     1997 2024-04-22 00:06:11.260762 vietfin-0.2.0/src/vietfin/providers/ssi/utils/index_constituents.py
+-rw-r--r--   0        0        0     2331 2024-04-22 00:06:11.260762 vietfin-0.2.0/src/vietfin/providers/ssi/utils/index_search.py
+-rw-r--r--   0        0        0       31 2024-03-19 22:49:00.377599 vietfin-0.2.0/src/vietfin/providers/tcbs/__init__.py
+-rw-r--r--   0        0        0       35 2024-03-19 22:49:00.377599 vietfin-0.2.0/src/vietfin/providers/tcbs/models/__init__.py
+-rw-r--r--   0        0        0     1795 2024-04-22 00:06:11.260762 vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_calendar_events.py
+-rw-r--r--   0        0        0      982 2024-03-19 22:49:00.379973 vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_fundamental_dividends.py
+-rw-r--r--   0        0        0     1870 2024-03-19 22:49:00.380837 vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_fundamental_income.py
+-rw-r--r--   0        0        0      588 2024-03-19 22:49:00.380837 vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_fundamental_management.py
+-rw-r--r--   0        0        0      630 2024-03-19 22:49:00.381835 vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_fundamental_ratios.py
+-rw-r--r--   0        0        0     2048 2024-03-19 22:49:00.382833 vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_ownership_insider_trading.py
+-rw-r--r--   0        0        0      419 2024-03-19 22:49:00.382833 vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_ownership_major_holders.py
+-rw-r--r--   0        0        0      637 2024-03-19 22:49:00.383920 vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_price_historical.py
+-rw-r--r--   0        0        0      729 2024-03-19 22:49:00.384827 vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_price_quote.py
+-rw-r--r--   0        0        0     1490 2024-04-22 00:06:11.260762 vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_profile.py
+-rw-r--r--   0        0        0      918 2024-03-19 22:49:00.385825 vietfin-0.2.0/src/vietfin/providers/tcbs/models/news_company.py
+-rw-r--r--   0        0        0     8967 2024-04-22 00:06:11.260762 vietfin-0.2.0/src/vietfin/providers/tcbs/provider.py
+-rw-r--r--   0        0        0       27 2024-03-19 22:49:00.387819 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/__init__.py
+-rw-r--r--   0        0        0     3080 2024-04-22 00:06:11.260762 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_calendar_events.py
+-rw-r--r--   0        0        0     3254 2024-04-22 00:06:11.260762 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_fundamental_dividends.py
+-rw-r--r--   0        0        0     3481 2024-04-22 00:06:11.260762 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_fundamental_income.py
+-rw-r--r--   0        0        0     2904 2024-04-22 00:06:11.267781 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_fundamental_management.py
+-rw-r--r--   0        0        0     2660 2024-04-22 00:06:11.267781 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_fundamental_ratios.py
+-rw-r--r--   0        0        0     3333 2024-04-22 00:06:11.267781 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_ownership_insider_trading.py
+-rw-r--r--   0        0        0     2262 2024-04-22 00:06:11.267781 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_ownership_major_holders.py
+-rw-r--r--   0        0        0     5537 2024-04-22 00:06:11.267781 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_price_historical.py
+-rw-r--r--   0        0        0     3119 2024-04-22 00:06:11.267781 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_price_quote.py
+-rw-r--r--   0        0        0     2392 2024-04-22 00:06:11.267781 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_profile.py
+-rw-r--r--   0        0        0      507 2024-03-19 22:49:00.396128 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/helpers.py
+-rw-r--r--   0        0        0     3026 2024-04-22 00:06:11.267781 vietfin-0.2.0/src/vietfin/providers/tcbs/utils/news_company.py
+-rw-r--r--   0        0        0       41 2024-03-19 22:49:00.398122 vietfin-0.2.0/src/vietfin/providers/vdsc/__init__.py
+-rw-r--r--   0        0        0       45 2024-03-19 22:49:00.399120 vietfin-0.2.0/src/vietfin/providers/vdsc/models/__init__.py
+-rw-r--r--   0        0        0     2637 2024-04-22 00:06:11.267781 vietfin-0.2.0/src/vietfin/providers/vdsc/models/derivatives_futures_quote.py
+-rw-r--r--   0        0        0     1259 2024-04-22 00:06:11.267781 vietfin-0.2.0/src/vietfin/providers/vdsc/provider.py
+-rw-r--r--   0        0        0       37 2024-03-19 22:49:00.402112 vietfin-0.2.0/src/vietfin/providers/vdsc/utils/__init__.py
+-rw-r--r--   0        0        0     3946 2024-04-22 00:06:11.274120 vietfin-0.2.0/src/vietfin/providers/vdsc/utils/derivatives_futures_quote.py
+-rw-r--r--   0        0        0     2175 2024-03-19 22:49:00.403110 vietfin-0.2.0/src/vietfin/providers/vdsc/utils/helpers.py
+-rw-r--r--   0        0        0       36 2024-04-22 00:06:11.274120 vietfin-0.2.0/src/vietfin/providers/vndirect/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-22 00:06:11.275117 vietfin-0.2.0/src/vietfin/providers/vndirect/models/__init__.py
+-rw-r--r--   0        0        0      991 2024-04-22 00:06:11.275117 vietfin-0.2.0/src/vietfin/providers/vndirect/models/equity_discovery.py
+-rw-r--r--   0        0        0     1069 2024-04-22 00:06:11.276115 vietfin-0.2.0/src/vietfin/providers/vndirect/provider.py
+-rw-r--r--   0        0        0       31 2024-04-22 00:06:11.276115 vietfin-0.2.0/src/vietfin/providers/vndirect/utils/__init__.py
+-rw-r--r--   0        0        0     3033 2024-04-22 00:06:11.277112 vietfin-0.2.0/src/vietfin/providers/vndirect/utils/equity_discovery.py
+-rw-r--r--   0        0        0      660 2024-04-22 00:06:11.277112 vietfin-0.2.0/src/vietfin/providers/vndirect/utils/helpers.py
+-rw-r--r--   0        0        0       35 2024-03-19 22:49:00.404106 vietfin-0.2.0/src/vietfin/providers/wifeed/__init__.py
+-rw-r--r--   0        0        0       37 2024-03-19 22:49:00.405104 vietfin-0.2.0/src/vietfin/providers/wifeed/models/__init__.py
+-rw-r--r--   0        0        0      329 2024-03-19 22:49:00.406101 vietfin-0.2.0/src/vietfin/providers/wifeed/models/equity_search.py
+-rw-r--r--   0        0        0      693 2024-03-19 22:49:00.406101 vietfin-0.2.0/src/vietfin/providers/wifeed/provider.py
+-rw-r--r--   0        0        0       31 2024-03-19 22:49:00.407098 vietfin-0.2.0/src/vietfin/providers/wifeed/utils/__init__.py
+-rw-r--r--   0        0        0     2404 2024-04-22 00:06:11.278109 vietfin-0.2.0/src/vietfin/providers/wifeed/utils/equity_search.py
+-rw-r--r--   0        0        0       23 2024-03-19 22:49:00.408096 vietfin-0.2.0/src/vietfin/providers/wifeed/utils/helpers.py
+-rw-r--r--   0        0        0       51 2024-03-19 22:49:00.409094 vietfin-0.2.0/src/vietfin/py.typed
+-rw-r--r--   0        0        0       32 2024-03-19 22:49:00.409094 vietfin-0.2.0/src/vietfin/utils/__init__.py
+-rw-r--r--   0        0        0      617 2024-03-19 22:49:00.410091 vietfin-0.2.0/src/vietfin/utils/errors.py
+-rw-r--r--   0        0        0     9597 2024-04-22 00:06:11.279107 vietfin-0.2.0/src/vietfin/utils/helpers.py
+-rw-r--r--   0        0        0     7455 1970-01-01 00:00:00.000000 vietfin-0.2.0/PKG-INFO
```

### Comparing `vietfin-0.1.0/LICENSE` & `vietfin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/pyproject.toml` & `vietfin-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2276 6965 7466 696e 220d  ame = "vietfin".
-00000020: 0a76 6572 7369 6f6e 203d 2022 302e 312e  .version = "0.1.
+00000020: 0a76 6572 7369 6f6e 203d 2022 302e 322e  .version = "0.2.
 00000030: 3022 0d0a 6465 7363 7269 7074 696f 6e20  0"..description 
 00000040: 3d20 2250 7974 686f 6e20 7061 636b 6167  = "Python packag
 00000050: 6520 746f 2066 6574 6368 2056 6965 746e  e to fetch Vietn
 00000060: 616d 2073 746f 636b 206d 6172 6b65 7420  am stock market 
 00000070: 6461 7461 220d 0a61 7574 686f 7273 203d  data"..authors =
 00000080: 205b 2248 7579 203c 7669 6574 6669 6e2e   ["Huy <vietfin.
 00000090: 6e75 6d62 6e65 7373 3137 3940 7369 6d70  numbness179@simp
@@ -60,114 +60,105 @@
 000003b0: 0d0a 7079 7468 6f6e 203d 2022 5e33 2e31  ..python = "^3.1
 000003c0: 3022 0d0a 7079 6461 6e74 6963 203d 2022  0"..pydantic = "
 000003d0: 5e32 2e35 2e33 2220 2023 206e 6565 6465  ^2.5.3"  # neede
 000003e0: 6420 746f 2076 616c 6964 6174 6520 6461  d to validate da
 000003f0: 7461 0d0a 7061 6e64 6173 203d 2022 5e32  ta..pandas = "^2
 00000400: 2e31 2e34 2220 2023 206e 6565 6465 6420  .1.4"  # needed 
 00000410: 746f 206d 616e 6970 756c 6174 6520 6461  to manipulate da
-00000420: 7461 0d0a 7265 7175 6573 7473 203d 2022  ta..requests = "
-00000430: 5e32 2e33 312e 3022 2020 2320 6e65 6564  ^2.31.0"  # need
-00000440: 6564 2074 6f20 6665 7463 6820 6461 7461  ed to fetch data
-00000450: 2066 726f 6d20 7765 620d 0a62 7334 203d   from web..bs4 =
-00000460: 2022 5e30 2e30 2e32 2220 2023 206e 6565   "^0.0.2"  # nee
-00000470: 6465 6420 746f 2070 6172 7365 2068 746d  ded to parse htm
-00000480: 6c0d 0a6f 7065 6e70 7978 6c20 3d20 225e  l..openpyxl = "^
-00000490: 332e 312e 3222 2020 2320 7265 6164 2065  3.1.2"  # read e
-000004a0: 7863 656c 2066 696c 650d 0a0d 0a5b 746f  xcel file....[to
-000004b0: 6f6c 2e70 6f65 7472 792e 6772 6f75 702e  ol.poetry.group.
-000004c0: 6465 762e 6465 7065 6e64 656e 6369 6573  dev.dependencies
-000004d0: 5d0d 0a70 7974 6573 7420 3d20 225e 372e  ]..pytest = "^7.
-000004e0: 342e 3422 2020 2320 6e65 6564 6564 2074  4.4"  # needed t
-000004f0: 6f20 7275 6e20 7465 7374 730d 0a72 7566  o run tests..ruf
-00000500: 6620 3d20 225e 302e 312e 3131 2220 2023  f = "^0.1.11"  #
-00000510: 206e 6565 6465 6420 746f 2066 6f72 6d61   needed to forma
-00000520: 7420 636f 6465 0d0a 6d79 7079 203d 2022  t code..mypy = "
-00000530: 5e31 2e38 2e30 2220 2023 206e 6565 6465  ^1.8.0"  # neede
-00000540: 6420 746f 2074 7970 6520 6869 6e74 2063  d to type hint c
-00000550: 6f64 650d 0a69 7079 6b65 726e 656c 203d  ode..ipykernel =
-00000560: 2022 5e36 2e32 382e 3022 2020 2320 6e65   "^6.28.0"  # ne
-00000570: 6564 6564 2074 6f20 6578 6563 7574 6520  eded to execute 
-00000580: 6675 6e63 7469 6f6e 7320 696e 206a 7570  functions in jup
-00000590: 7974 6572 206e 6f74 6562 6f6f 6b73 0d0a  yter notebooks..
-000005a0: 7061 6e64 6173 2d73 7475 6273 203d 2022  pandas-stubs = "
-000005b0: 5e32 2e31 2e34 2e32 3331 3232 3722 2020  ^2.1.4.231227"  
-000005c0: 2320 6e65 6564 6564 2066 6f72 206d 7970  # needed for myp
-000005d0: 7920 746f 2074 7970 6520 6869 6e74 2070  y to type hint p
-000005e0: 616e 6461 730d 0a74 7970 6573 2d72 6571  andas..types-req
-000005f0: 7565 7374 7320 3d20 225e 322e 3331 2e30  uests = "^2.31.0
-00000600: 2e32 3032 3430 3130 3622 2020 2320 6e65  .20240106"  # ne
-00000610: 6564 6564 2066 6f72 206d 7970 7920 746f  eded for mypy to
-00000620: 2074 7970 6520 6869 6e74 2072 6571 7565   type hint reque
-00000630: 7374 730d 0a74 7970 6573 2d62 6561 7574  sts..types-beaut
-00000640: 6966 756c 736f 7570 3420 3d20 225e 342e  ifulsoup4 = "^4.
-00000650: 3132 2e30 2e32 3032 3430 3130 3622 2020  12.0.20240106"  
-00000660: 2320 6e65 6564 6564 2066 6f72 206d 7970  # needed for myp
-00000670: 7920 746f 2074 7970 6520 6869 6e74 2062  y to type hint b
-00000680: 7334 0d0a 0d0a 5b74 6f6f 6c2e 706f 6574  s4....[tool.poet
-00000690: 7279 2e67 726f 7570 2e64 6f63 732e 6465  ry.group.docs.de
-000006a0: 7065 6e64 656e 6369 6573 5d0d 0a73 7068  pendencies]..sph
-000006b0: 696e 7820 3d20 225e 372e 322e 3622 2020  inx = "^7.2.6"  
-000006c0: 2320 6e65 6564 6564 2074 6f20 6765 6e65  # needed to gene
-000006d0: 7261 7465 2064 6f63 756d 656e 7461 7469  rate documentati
-000006e0: 6f6e 2077 6562 7369 7465 0d0a 7368 6962  on website..shib
-000006f0: 7579 6120 3d20 225e 3230 3234 2e31 2e31  uya = "^2024.1.1
-00000700: 3722 2020 2320 6375 7374 6f6d 2074 6865  7"  # custom the
-00000710: 6d65 2066 6f72 2073 7068 696e 780d 0a6d  me for sphinx..m
-00000720: 7973 742d 7061 7273 6572 203d 2022 5e32  yst-parser = "^2
-00000730: 2e30 2e30 2220 2023 2065 6e61 626c 6520  .0.0"  # enable 
-00000740: 7370 6869 6e78 2074 6f20 7061 7273 6520  sphinx to parse 
-00000750: 4d61 726b 646f 776e 0d0a 7370 6869 6e78  Markdown..sphinx
-00000760: 2d63 6f70 7962 7574 746f 6e20 3d20 225e  -copybutton = "^
-00000770: 302e 352e 3222 2020 2320 6164 6420 636f  0.5.2"  # add co
-00000780: 7079 2062 7574 746f 6e20 746f 2063 6f64  py button to cod
-00000790: 6520 626c 6f63 6b20 696e 2064 6f63 756d  e block in docum
-000007a0: 656e 7461 7469 6f6e 2077 6562 7369 7465  entation website
-000007b0: 2e0d 0a73 7068 696e 7863 6f6e 7472 6962  ...sphinxcontrib
-000007c0: 2d6d 6572 6d61 6964 203d 2022 5e30 2e39  -mermaid = "^0.9
-000007d0: 2e32 2220 2023 2072 656e 6465 7220 6d65  .2"  # render me
-000007e0: 726d 6169 6420 6469 6167 7261 6d73 2069  rmaid diagrams i
-000007f0: 6e20 646f 6375 6d65 6e74 6174 696f 6e20  n documentation 
-00000800: 7765 6273 6974 652e 0d0a 7370 6869 6e78  website...sphinx
-00000810: 2d73 6974 656d 6170 203d 2022 5e32 2e35  -sitemap = "^2.5
-00000820: 2e31 2220 2023 2061 6464 2073 6974 656d  .1"  # add sitem
-00000830: 6170 2074 6f20 5370 6869 6e78 2064 6f63  ap to Sphinx doc
-00000840: 730d 0a6e 6273 7068 696e 7820 3d20 225e  s..nbsphinx = "^
-00000850: 302e 392e 3322 2020 2320 656e 6162 6c65  0.9.3"  # enable
-00000860: 2053 7068 696e 7820 746f 2070 6172 7365   Sphinx to parse
-00000870: 204a 7570 7974 6572 206e 6f74 6562 6f6f   Jupyter noteboo
-00000880: 6b73 0d0a 7370 6869 6e78 2d64 6573 6967  ks..sphinx-desig
-00000890: 6e20 3d20 225e 302e 352e 3022 2020 2320  n = "^0.5.0"  # 
-000008a0: 6164 6420 7265 7370 6f6e 7369 7665 2077  add responsive w
-000008b0: 6562 2063 6f6d 706f 6e65 6e74 7320 746f  eb components to
-000008c0: 2053 7068 696e 7820 646f 6373 2c20 7265   Sphinx docs, re
-000008d0: 706c 6163 6520 7370 6869 6e78 2d74 6f67  place sphinx-tog
-000008e0: 676c 6562 7574 746f 6e20 616e 6420 7370  glebutton and sp
-000008f0: 6869 6e78 2d69 6e6c 696e 652d 7461 6273  hinx-inline-tabs
-00000900: 0d0a 0d0a 5b62 7569 6c64 2d73 7973 7465  ....[build-syste
-00000910: 6d5d 0d0a 7265 7175 6972 6573 203d 205b  m]..requires = [
-00000920: 2270 6f65 7472 792d 636f 7265 225d 0d0a  "poetry-core"]..
-00000930: 6275 696c 642d 6261 636b 656e 6420 3d20  build-backend = 
-00000940: 2270 6f65 7472 792e 636f 7265 2e6d 6173  "poetry.core.mas
-00000950: 6f6e 7279 2e61 7069 220d 0a0d 0a5b 746f  onry.api"....[to
-00000960: 6f6c 2e72 7566 665d 0d0a 2320 6d61 7820  ol.ruff]..# max 
-00000970: 6368 6172 2070 6572 206c 696e 650d 0a6c  char per line..l
-00000980: 696e 652d 6c65 6e67 7468 203d 2038 300d  ine-length = 80.
-00000990: 0a0d 0a23 2069 6e64 656e 7420 7769 7468  ...# indent with
-000009a0: 2034 2073 7061 6365 730d 0a69 6e64 656e   4 spaces..inden
-000009b0: 742d 7769 6474 6820 3d20 340d 0a0d 0a23  t-width = 4....#
-000009c0: 2041 7373 756d 6520 5079 7468 6f6e 2033   Assume Python 3
-000009d0: 2e31 300d 0a74 6172 6765 742d 7665 7273  .10..target-vers
-000009e0: 696f 6e20 3d20 2270 7933 3130 220d 0a0d  ion = "py310"...
-000009f0: 0a5b 746f 6f6c 2e72 7566 662e 666f 726d  .[tool.ruff.form
-00000a00: 6174 5d0d 0a23 2075 7365 2064 6f75 626c  at]..# use doubl
-00000a10: 6520 7175 6f74 6520 666f 7220 7374 7269  e quote for stri
-00000a20: 6e67 732e 0d0a 7175 6f74 652d 7374 796c  ngs...quote-styl
-00000a30: 6520 3d20 2264 6f75 626c 6522 0d0a 0d0a  e = "double"....
-00000a40: 2320 696e 6465 6e74 2077 6974 6820 7370  # indent with sp
-00000a50: 6163 6573 2c20 7261 7468 6572 2074 6861  aces, rather tha
-00000a60: 6e20 7461 6273 2e0d 0a69 6e64 656e 742d  n tabs...indent-
-00000a70: 7374 796c 6520 3d20 2273 7061 6365 220d  style = "space".
-00000a80: 0a0d 0a23 2061 7574 6f6d 6174 6963 616c  ...# automatical
-00000a90: 6c79 2064 6574 6563 7420 7468 6520 6170  ly detect the ap
-00000aa0: 7072 6f70 7269 6174 6520 6c69 6e65 2065  propriate line e
-00000ab0: 6e64 696e 672e 0d0a 6c69 6e65 2d65 6e64  nding...line-end
-00000ac0: 696e 6720 3d20 2261 7574 6f22            ing = "auto"
+00000420: 7461 0d0a 6f70 656e 7079 786c 203d 2022  ta..openpyxl = "
+00000430: 5e33 2e31 2e32 2220 2023 2072 6561 6420  ^3.1.2"  # read 
+00000440: 6578 6365 6c20 6669 6c65 0d0a 7365 6c65  excel file..sele
+00000450: 6374 6f6c 6178 203d 2022 5e30 2e33 2e32  ctolax = "^0.3.2
+00000460: 3122 2020 2320 6e65 6564 6564 2074 6f20  1"  # needed to 
+00000470: 7061 7273 6520 6874 6d6c 0d0a 6874 7470  parse html..http
+00000480: 7820 3d20 225e 302e 3237 2e30 2220 2023  x = "^0.27.0"  #
+00000490: 206e 6565 6465 6420 746f 2066 6574 6368   needed to fetch
+000004a0: 2064 6174 6120 6672 6f6d 2077 6562 0d0a   data from web..
+000004b0: 0d0a 5b74 6f6f 6c2e 706f 6574 7279 2e67  ..[tool.poetry.g
+000004c0: 726f 7570 2e64 6576 2e64 6570 656e 6465  roup.dev.depende
+000004d0: 6e63 6965 735d 0d0a 7079 7465 7374 203d  ncies]..pytest =
+000004e0: 2022 5e37 2e34 2e34 2220 2023 206e 6565   "^7.4.4"  # nee
+000004f0: 6465 6420 746f 2072 756e 2074 6573 7473  ded to run tests
+00000500: 0d0a 7275 6666 203d 2022 5e30 2e31 2e31  ..ruff = "^0.1.1
+00000510: 3122 2020 2320 6e65 6564 6564 2074 6f20  1"  # needed to 
+00000520: 666f 726d 6174 2063 6f64 650d 0a6d 7970  format code..myp
+00000530: 7920 3d20 225e 312e 382e 3022 2020 2320  y = "^1.8.0"  # 
+00000540: 6e65 6564 6564 2074 6f20 7479 7065 2068  needed to type h
+00000550: 696e 7420 636f 6465 0d0a 6970 796b 6572  int code..ipyker
+00000560: 6e65 6c20 3d20 225e 362e 3238 2e30 2220  nel = "^6.28.0" 
+00000570: 2023 206e 6565 6465 6420 746f 2065 7865   # needed to exe
+00000580: 6375 7465 2066 756e 6374 696f 6e73 2069  cute functions i
+00000590: 6e20 6a75 7079 7465 7220 6e6f 7465 626f  n jupyter notebo
+000005a0: 6f6b 730d 0a70 616e 6461 732d 7374 7562  oks..pandas-stub
+000005b0: 7320 3d20 225e 322e 312e 342e 3233 3132  s = "^2.1.4.2312
+000005c0: 3237 2220 2023 206e 6565 6465 6420 666f  27"  # needed fo
+000005d0: 7220 6d79 7079 2074 6f20 7479 7065 2068  r mypy to type h
+000005e0: 696e 7420 7061 6e64 6173 0d0a 0d0a 5b74  int pandas....[t
+000005f0: 6f6f 6c2e 706f 6574 7279 2e67 726f 7570  ool.poetry.group
+00000600: 2e64 6f63 732e 6465 7065 6e64 656e 6369  .docs.dependenci
+00000610: 6573 5d0d 0a73 7068 696e 7820 3d20 225e  es]..sphinx = "^
+00000620: 372e 322e 3622 2020 2320 6e65 6564 6564  7.2.6"  # needed
+00000630: 2074 6f20 6765 6e65 7261 7465 2064 6f63   to generate doc
+00000640: 756d 656e 7461 7469 6f6e 2077 6562 7369  umentation websi
+00000650: 7465 0d0a 7368 6962 7579 6120 3d20 225e  te..shibuya = "^
+00000660: 3230 3234 2e34 2e38 2220 2023 2063 7573  2024.4.8"  # cus
+00000670: 746f 6d20 7468 656d 6520 666f 7220 7370  tom theme for sp
+00000680: 6869 6e78 0d0a 6d79 7374 2d70 6172 7365  hinx..myst-parse
+00000690: 7220 3d20 225e 322e 302e 3022 2020 2320  r = "^2.0.0"  # 
+000006a0: 656e 6162 6c65 2073 7068 696e 7820 746f  enable sphinx to
+000006b0: 2070 6172 7365 204d 6172 6b64 6f77 6e0d   parse Markdown.
+000006c0: 0a73 7068 696e 782d 636f 7079 6275 7474  .sphinx-copybutt
+000006d0: 6f6e 203d 2022 5e30 2e35 2e32 2220 2023  on = "^0.5.2"  #
+000006e0: 2061 6464 2063 6f70 7920 6275 7474 6f6e   add copy button
+000006f0: 2074 6f20 636f 6465 2062 6c6f 636b 2069   to code block i
+00000700: 6e20 646f 6375 6d65 6e74 6174 696f 6e20  n documentation 
+00000710: 7765 6273 6974 652e 0d0a 7370 6869 6e78  website...sphinx
+00000720: 636f 6e74 7269 622d 6d65 726d 6169 6420  contrib-mermaid 
+00000730: 3d20 225e 302e 392e 3222 2020 2320 7265  = "^0.9.2"  # re
+00000740: 6e64 6572 206d 6572 6d61 6964 2064 6961  nder mermaid dia
+00000750: 6772 616d 7320 696e 2064 6f63 756d 656e  grams in documen
+00000760: 7461 7469 6f6e 2077 6562 7369 7465 2e0d  tation website..
+00000770: 0a73 7068 696e 782d 7369 7465 6d61 7020  .sphinx-sitemap 
+00000780: 3d20 225e 322e 352e 3122 2020 2320 6164  = "^2.5.1"  # ad
+00000790: 6420 7369 7465 6d61 7020 746f 2053 7068  d sitemap to Sph
+000007a0: 696e 7820 646f 6373 0d0a 6e62 7370 6869  inx docs..nbsphi
+000007b0: 6e78 203d 2022 5e30 2e39 2e33 2220 2023  nx = "^0.9.3"  #
+000007c0: 2065 6e61 626c 6520 5370 6869 6e78 2074   enable Sphinx t
+000007d0: 6f20 7061 7273 6520 4a75 7079 7465 7220  o parse Jupyter 
+000007e0: 6e6f 7465 626f 6f6b 730d 0a73 7068 696e  notebooks..sphin
+000007f0: 782d 6465 7369 676e 203d 2022 5e30 2e35  x-design = "^0.5
+00000800: 2e30 2220 2023 2061 6464 2072 6573 706f  .0"  # add respo
+00000810: 6e73 6976 6520 7765 6220 636f 6d70 6f6e  nsive web compon
+00000820: 656e 7473 2074 6f20 5370 6869 6e78 2064  ents to Sphinx d
+00000830: 6f63 732c 2072 6570 6c61 6365 2073 7068  ocs, replace sph
+00000840: 696e 782d 746f 6767 6c65 6275 7474 6f6e  inx-togglebutton
+00000850: 2061 6e64 2073 7068 696e 782d 696e 6c69   and sphinx-inli
+00000860: 6e65 2d74 6162 730d 0a0d 0a5b 6275 696c  ne-tabs....[buil
+00000870: 642d 7379 7374 656d 5d0d 0a72 6571 7569  d-system]..requi
+00000880: 7265 7320 3d20 5b22 706f 6574 7279 2d63  res = ["poetry-c
+00000890: 6f72 6522 5d0d 0a62 7569 6c64 2d62 6163  ore"]..build-bac
+000008a0: 6b65 6e64 203d 2022 706f 6574 7279 2e63  kend = "poetry.c
+000008b0: 6f72 652e 6d61 736f 6e72 792e 6170 6922  ore.masonry.api"
+000008c0: 0d0a 0d0a 5b74 6f6f 6c2e 7275 6666 5d0d  ....[tool.ruff].
+000008d0: 0a23 206d 6178 2063 6861 7220 7065 7220  .# max char per 
+000008e0: 6c69 6e65 0d0a 6c69 6e65 2d6c 656e 6774  line..line-lengt
+000008f0: 6820 3d20 3830 0d0a 0d0a 2320 696e 6465  h = 80....# inde
+00000900: 6e74 2077 6974 6820 3420 7370 6163 6573  nt with 4 spaces
+00000910: 0d0a 696e 6465 6e74 2d77 6964 7468 203d  ..indent-width =
+00000920: 2034 0d0a 0d0a 2320 4173 7375 6d65 2050   4....# Assume P
+00000930: 7974 686f 6e20 332e 3130 0d0a 7461 7267  ython 3.10..targ
+00000940: 6574 2d76 6572 7369 6f6e 203d 2022 7079  et-version = "py
+00000950: 3331 3022 0d0a 0d0a 5b74 6f6f 6c2e 7275  310"....[tool.ru
+00000960: 6666 2e66 6f72 6d61 745d 0d0a 2320 7573  ff.format]..# us
+00000970: 6520 646f 7562 6c65 2071 756f 7465 2066  e double quote f
+00000980: 6f72 2073 7472 696e 6773 2e0d 0a71 756f  or strings...quo
+00000990: 7465 2d73 7479 6c65 203d 2022 646f 7562  te-style = "doub
+000009a0: 6c65 220d 0a0d 0a23 2069 6e64 656e 7420  le"....# indent 
+000009b0: 7769 7468 2073 7061 6365 732c 2072 6174  with spaces, rat
+000009c0: 6865 7220 7468 616e 2074 6162 732e 0d0a  her than tabs...
+000009d0: 696e 6465 6e74 2d73 7479 6c65 203d 2022  indent-style = "
+000009e0: 7370 6163 6522 0d0a 0d0a 2320 6175 746f  space"....# auto
+000009f0: 6d61 7469 6361 6c6c 7920 6465 7465 6374  matically detect
+00000a00: 2074 6865 2061 7070 726f 7072 6961 7465   the appropriate
+00000a10: 206c 696e 6520 656e 6469 6e67 2e0d 0a6c   line ending...l
+00000a20: 696e 652d 656e 6469 6e67 203d 2022 6175  ine-ending = "au
+00000a30: 746f 22                                  to"
```

### Comparing `vietfin-0.1.0/README.md` & `vietfin-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 <p align="center">
-  <img src="/docs/_static/logo.jpg" alt="VietFin" width="228" />
+  <img src="https://github.com/vietfin/vietfin/blob/main/docs/_static/logo.jpg" alt="VietFin" width="228" />
 </p>
 
 <h2 align="center">VietFin</h2>
 
 <div align="center">A python library to fetch Vietnam stock market data.</div>
 
 <p align="center">
-    <a href="https://github.com/vietfin/vietfin/blob/main/LICENSE"><img src="https://img.shields.io/github/license/vietfin/vietfin?style=for-the-badge" alt="License"></a>
+    <a href="https://github.com/vietfin/vietfin/blob/main/LICENSE"><img src="https://img.shields.io/github/license/vietfin/vietfin?style=for-the-badge" alt="License" /></a>
     <a href='https://vietfin.readthedocs.io/en/latest/?badge=latest'><img src='https://readthedocs.org/projects/vietfin/badge/?version=latest&style=for-the-badge' alt='Documentation Status' /></a>
+    <a href='https://pypi.org/project/vietfin/'><img src='https://img.shields.io/pypi/v/vietfin?style=for-the-badge' alt='PyPI - Version' /></a>
     <br />
     <a href="http://vietfin.readthedocs.io/" target="_blank" rel="noopener noreferrer"><strong>» Explore the docs »</strong></a>
     <br />
 </p>
 
 <hr />
 
@@ -36,40 +37,42 @@
 
 This package aims to reproduce the hierarchical structure of commands used in OpenBB, but for Vietnamese market data.
 
 VietFin is intended for personal use, research and educational purposes.
 
 ## 2. Installation
 
-VietFin is available on [PyPI](https://pypi.org/). To use the package:
+VietFin is available on [PyPI](https://pypi.org/project/vietfin/). To use the package:
 
 1. Install VietFin in your project's virtual environment.
 
     ``` {.sourceCode .bash}
     $ pip install vietfin
     ```
 
-    Or using [Poetry](https://python-poetry.org/) as my preferred dependency manager:
+    Or using [Poetry](https://python-poetry.org/), my preferred dependency manager:
 
     ``` {.sourceCode .bash}
     $ poetry add vietfin
     ```
 
 2. Import the package then use the package
 
     ``` {.sourceCode .python}
     from vietfin import vf
     ```
 
 Requirements:
 
 - [Python](https://www.python.org) \>= 3.10
-- [requests](https://requests.readthedocs.io/en/latest/) \>= 2.31
 - [pandas](https://pandas.pydata.org/) \>= 2.1.4
 - [Pydantic](https://github.com/pydantic/pydantic) \>= 2.5
+- [httpx](https://www.python-httpx.org/) \>= 0.27
+- [selectolax](https://github.com/rushter/selectolax) \>= 0.3
+- [openpyxl](https://pypi.org/project/openpyxl/) \>= 3.1.2
 
 ## 3. Usage
 
 ```python
 from vietfin import vf
 # Get list of all stocks
 vf.equity.search()
@@ -99,14 +102,17 @@
 vf.funds.search()
 
 # Get the list of available ETFs
 vf.etf.search()
 
 # Get the list of constituents of an index
 vf.index.constituents(symbol='vn30')
+
+# Get the list of available futures contract
+vf.derivatives.futures.search()
 ```
 
 ## 4. Contributing
 
 More information on our [Contributing Guidelines](/CONTRIBUTING.md) and [Code of Conduct](/CONDUCT.md).
 
 `VietFin` relies on community to investigate bugs and contribute code.
@@ -119,16 +125,16 @@
 
 Feel free to reach out to us in [our GitHub Discussions](https://github.com/vietfin/vietfin/discussions) for other feedbacks (e.g. Q&A, ideas, etc.).
 
 ## 5. Attributions
 
 VietFin is built on top of the inspiration and work of the following projects:
 
-- [Openbb](https://github.com/OpenBB-finance/OpenBBTerminal), its [Data Standardization Infrastructure](https://docs.openbb.co/platform/development/developer-guidelines/architectural_considerations), the hierarchical structure of user-facing commands, and the documentation style of [OpenBB Platform's API reference](https://docs.openbb.co/platform/reference).
-- [vnstock](https://github.com/thinh-vu/vnstock) and its findinds on publicly available APIs from brokerage firms in Vietnam.
+- [OpenBB](https://github.com/OpenBB-finance/OpenBBTerminal), its [Data Standardization Infrastructure](https://docs.openbb.co/platform/development/developer-guidelines/architectural_considerations), the hierarchical structure of user-facing commands, and the documentation style of [OpenBB Platform's API reference](https://docs.openbb.co/platform/reference).
+- [vnstock](https://github.com/thinh-vu/vnstock) and its findinds on publicly available APIs from many brokerage firms in Vietnam.
 
 ## 6. Disclaimer
 
 VietFin is not affiliated, endorsed, or vetted by any of the brokerage firms or research entities which provide the data. It's an open-source tool which fetches data from the publicly available APIs of these firms. VietFin is intended for personal use, research and educational purposes.
 
 You should refer to each of the data provider's terms of use for details on your rights to use the actual data downloaded.
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                                    [VietFin]
                               ********** VViieettFFiinn **********
              A python library to fetch Vietnam stock market data.
-                        _[_L_i_c_e_n_s_e_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]
+                _[_L_i_c_e_n_s_e_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]
                             _?Â_?»_ _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 ===============================================================================
 ********** TTaabbllee ooff CCoonntteennttss **********
    1. _W_h_y_ _V_i_e_t_F_i_n_?
    2. _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
    4. _C_o_n_t_r_i_b_u_t_i_n_g
@@ -14,60 +14,63 @@
    7. _C_o_n_t_a_c_t_s
 ## 1. Why VietFin? Heavily inspired by [OpenBB](https://github.com/OpenBB-
 finance/OpenBBTerminal), VietFin is a Python package which provides a wrapper
 around the publicly available APIs from multiple brokerage firms. This package
 aims to reproduce the hierarchical structure of commands used in OpenBB, but
 for Vietnamese market data. VietFin is intended for personal use, research and
 educational purposes. ## 2. Installation VietFin is available on [PyPI](https:/
-/pypi.org/). To use the package: 1. Install VietFin in your project's virtual
-environment. ``` {.sourceCode .bash} $ pip install vietfin ``` Or using
-[Poetry](https://python-poetry.org/) as my preferred dependency manager: ```
-{.sourceCode .bash} $ poetry add vietfin ``` 2. Import the package then use the
-package ``` {.sourceCode .python} from vietfin import vf ``` Requirements: -
-[Python](https://www.python.org) \>= 3.10 - [requests](https://
-requests.readthedocs.io/en/latest/) \>= 2.31 - [pandas](https://
+/pypi.org/project/vietfin/). To use the package: 1. Install VietFin in your
+project's virtual environment. ``` {.sourceCode .bash} $ pip install vietfin
+``` Or using [Poetry](https://python-poetry.org/), my preferred dependency
+manager: ``` {.sourceCode .bash} $ poetry add vietfin ``` 2. Import the package
+then use the package ``` {.sourceCode .python} from vietfin import vf ```
+Requirements: - [Python](https://www.python.org) \>= 3.10 - [pandas](https://
 pandas.pydata.org/) \>= 2.1.4 - [Pydantic](https://github.com/pydantic/
-pydantic) \>= 2.5 ## 3. Usage ```python from vietfin import vf # Get list of
-all stocks vf.equity.search() # Get general info of a stock vf.equity.profile
-(symbol='vnm') # Get historical price of a stock vf.equity.historical
-(symbol='vnm') # Get the historical dividends data of a company
-vf.equity.fundamental.dividends(symbol='vnm') # Get list of key executives of a
-company vf.equity.fundamental.management(symbol='vnm') # Get the key financial
-ratios of a company vf.equity.fundamental.ratios(symbol='vnm') # Get the report
-on the income statement of a company vf.equity.fundamental.income(symbol='vnm')
-# Get the historical events of a stock ticker vf.equity.calendar.events
-(symbol='vnm') # Get the list of available mutual funds vf.funds.search() # Get
-the list of available ETFs vf.etf.search() # Get the list of constituents of an
-index vf.index.constituents(symbol='vn30') ``` ## 4. Contributing More
+pydantic) \>= 2.5 - [httpx](https://www.python-httpx.org/) \>= 0.27 -
+[selectolax](https://github.com/rushter/selectolax) \>= 0.3 - [openpyxl](https:
+//pypi.org/project/openpyxl/) \>= 3.1.2 ## 3. Usage ```python from vietfin
+import vf # Get list of all stocks vf.equity.search() # Get general info of a
+stock vf.equity.profile(symbol='vnm') # Get historical price of a stock
+vf.equity.historical(symbol='vnm') # Get the historical dividends data of a
+company vf.equity.fundamental.dividends(symbol='vnm') # Get list of key
+executives of a company vf.equity.fundamental.management(symbol='vnm') # Get
+the key financial ratios of a company vf.equity.fundamental.ratios
+(symbol='vnm') # Get the report on the income statement of a company
+vf.equity.fundamental.income(symbol='vnm') # Get the historical events of a
+stock ticker vf.equity.calendar.events(symbol='vnm') # Get the list of
+available mutual funds vf.funds.search() # Get the list of available ETFs
+vf.etf.search() # Get the list of constituents of an index
+vf.index.constituents(symbol='vn30') # Get the list of available futures
+contract vf.derivatives.futures.search() ``` ## 4. Contributing More
 information on our [Contributing Guidelines](/CONTRIBUTING.md) and [Code of
 Conduct](/CONDUCT.md). `VietFin` relies on community to investigate bugs and
 contribute code. Before creating a ticket, please check our [Issues tracker]
 (https://github.com/vietfin/vietfin/issues) to avoid duplicates. - [Report bug]
 (https://github.com/vietfin/vietfin/issues/
 new?assignees=&labels=type%3Abug&projects=&template=bug_report.md&title=%5BBug%5D)
 - [Suggest improvement](https://github.com/vietfin/vietfin/issues/
 new?assignees=&labels=type%3Aenhancement&projects=&template=enhancement.md&title=%5BIMPROVE%5D)
 - [Request a feature](https://github.com/vietfin/vietfin/issues/
 new?assignees=&labels=type%3Afeature&projects=&template=feature_request.md&title=%5BFR%5D)
 Feel free to reach out to us in [our GitHub Discussions](https://github.com/
 vietfin/vietfin/discussions) for other feedbacks (e.g. Q&A, ideas, etc.). ## 5.
 Attributions VietFin is built on top of the inspiration and work of the
-following projects: - [Openbb](https://github.com/OpenBB-finance/
+following projects: - [OpenBB](https://github.com/OpenBB-finance/
 OpenBBTerminal), its [Data Standardization Infrastructure](https://
 docs.openbb.co/platform/development/developer-guidelines/
 architectural_considerations), the hierarchical structure of user-facing
 commands, and the documentation style of [OpenBB Platform's API reference]
 (https://docs.openbb.co/platform/reference). - [vnstock](https://github.com/
-thinh-vu/vnstock) and its findinds on publicly available APIs from brokerage
-firms in Vietnam. ## 6. Disclaimer VietFin is not affiliated, endorsed, or
-vetted by any of the brokerage firms or research entities which provide the
-data. It's an open-source tool which fetches data from the publicly available
-APIs of these firms. VietFin is intended for personal use, research and
-educational purposes. You should refer to each of the data provider's terms of
-use for details on your rights to use the actual data downloaded. The data
+thinh-vu/vnstock) and its findinds on publicly available APIs from many
+brokerage firms in Vietnam. ## 6. Disclaimer VietFin is not affiliated,
+endorsed, or vetted by any of the brokerage firms or research entities which
+provide the data. It's an open-source tool which fetches data from the publicly
+available APIs of these firms. VietFin is intended for personal use, research
+and educational purposes. You should refer to each of the data provider's terms
+of use for details on your rights to use the actual data downloaded. The data
 retrieved by the VietFin package is not necessarily accurate. VietFin and any
 provider of the data contained in this website will not accept liability for
 any loss or damage as a result of your trading, or your reliance on the
 information displayed. ## 7. Contacts If you have any questions about `VietFin`
 or just to say hi, feel free to [open a new public discussion in our GitHub
 repo](https://github.com/vietfin/vietfin/discussions/new/choose), or send an
 email to `vietfin.numbness179(at)simplelogin.fr`.
```

### Comparing `vietfin-0.1.0/src/vietfin/__init__.py` & `vietfin-0.2.0/src/vietfin/__init__.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/abstract/data.py` & `vietfin-0.2.0/src/vietfin/abstract/data.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/abstract/factory.py` & `vietfin-0.2.0/src/vietfin/abstract/factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,24 +5,26 @@
     IEquity,
     IEquityPrice,
     IEquityOwnership,
     IEquityCalendar,
     IEquityFundamental,
     IEquityDiscovery,
     IDerivativesFutures,
+    IDerivativesCoveredWarrant,
     IIndex,
     IIndexPrice,
     IEtf,
     INews,
 )
 from vietfin.providers.fmarket.provider import FundsFmarket
 from vietfin.providers.ssi.provider import (
     EquitySsi,
     EquityPriceSsi,
     EquityFundamentalSsi,
+    DerivativesCoveredWarrantSsi,
     IndexSsi,
     EquityDiscoverySsi,
     EtfSsi,
 )
 from vietfin.providers.wifeed.provider import EquityWifeed
 from vietfin.providers.dnse.provider import (
     EquityPriceDnse,
@@ -38,271 +40,296 @@
     DerivativesFuturesTcbs,
     EtfTcbs,
     NewsTcbs,
     IndexPriceTcbs,
 )
 from vietfin.providers.vdsc.provider import DerivativesFuturesVdsc
 from vietfin.providers.cafef.provider import EquityOwnershipCafef
+from vietfin.providers.vndirect.provider import EquityDiscoveryVndirect
+from vietfin.providers.ssi.provider import DerivativesFuturesSsi
 
 
 class FundsFactory:
     """Factory class for Funds component.
 
     Factory represents a combination of the IFunds's concrete implementations based on provider_name.
     The factory doesn't maintain any of the instances which it creates.
     """
 
-    funds_providers_implementations = {
+    providers_implementations = {
         "fmarket": FundsFmarket(),
     }
 
     def get_provider(self, provider: str) -> IFunds:
         """Returns a new concrete implementation of IFunds instance based on the provider name."""
 
-        if provider in self.funds_providers_implementations:
-            return self.funds_providers_implementations[provider]
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
         else:
             raise NotImplementedError(
                 f"Provider {provider} is not implemented yet."
             )
 
 
 class EquityFactory:
     """Factory class for Equity component.
 
     Factory represents a combination of the IEquity's concrete implementations based on provider_name.
     """
 
-    equity_providers_implementations = {
+    providers_implementations = {
         "ssi": EquitySsi(),
         "wifeed": EquityWifeed(),
         "tcbs": EquityTcbs(),
     }
 
     def get_provider(self, provider: str) -> IEquity:
         """Returns a new concrete implementation of IEquity instance based on the provider name."""
 
-        if provider in self.equity_providers_implementations:
-            return self.equity_providers_implementations[provider]
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
         else:
             raise NotImplementedError(
                 f"Provider {provider} is not implemented yet."
             )
 
 
 class EquityPriceFactory:
     """Factory class for Equity.Price component.
 
     Factory represents a combination of the IEquityPrice's concrete implementations based on provider_name.
     """
 
-    equity_price_providers_implementations = {
+    providers_implementations = {
         "dnse": EquityPriceDnse(),
         "tcbs": EquityPriceTcbs(),
         "ssi": EquityPriceSsi(),
     }
 
     def get_provider(self, provider: str) -> IEquityPrice:
         """Returns a new concrete implementation of IEquityPrice instance based on the provider name."""
 
-        if provider in self.equity_price_providers_implementations:
-            return self.equity_price_providers_implementations[provider]
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
         else:
             raise NotImplementedError(
                 f"Provider {provider} is not implemented yet."
             )
 
 
 class EquityOwnershipFactory:
     """Factory class for Equity.Ownership component.
 
     Factory represents a combination of the IEquityOwnership's concrete implementations based on provider_name.
     """
 
-    equity_ownership_provider_implementations = {
+    providers_implementations = {
         "tcbs": EquityOwnershipTcbs(),
         "cafef": EquityOwnershipCafef(),
     }
 
     def get_provider(self, provider: str) -> IEquityOwnership:
         """Returns a new concrete implementation of IEquityOwnership instance based on the provider name."""
 
-        if provider in self.equity_ownership_provider_implementations:
-            return self.equity_ownership_provider_implementations[provider]
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
         else:
             raise NotImplementedError(
                 f"Provider {provider} is not implemented yet."
             )
 
 
 class EquityCalendarFactory:
     """Factory class for Equity.Calendar component.
 
     Factory represents a combination of the IEquityCalendar's concrete implementations based on provider_name.
     """
 
-    equity_calendar_implementations = {
+    providers_implementations = {
         "tcbs": EquityCalendarTcbs(),
     }
 
     def get_provider(self, provider: str) -> IEquityCalendar:
         """Returns a new concrete implementation of IEquityCalendar instance based on the provider name."""
 
-        if provider in self.equity_calendar_implementations:
-            return self.equity_calendar_implementations[provider]
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
         else:
             raise NotImplementedError(
                 f"Provider {provider} is not implemented yet."
             )
 
 
 class EquityFundamentalFactory:
     """Factory class for Equity.Fundamental component.
 
     Factory represents a combination of the IEquityFundamental's concrete implementations based on provider_name.
     """
 
-    equity_fundamental_implementations = {
+    providers_implementations = {
         "tcbs": EquityFundamentalTcbs(),
         "ssi": EquityFundamentalSsi(),
     }
 
     def get_provider(self, provider: str) -> IEquityFundamental:
         """Returns a new concrete implementation of IEquityFundamental instance based on the provider name."""
 
-        if provider in self.equity_fundamental_implementations:
-            return self.equity_fundamental_implementations[provider]
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
         else:
             raise NotImplementedError(
                 f"Provider {provider} is not implemented yet."
             )
 
 
 class EquityDiscoveryFactory:
     """Factory class for Equity.Discovery component.
 
     Factory represents a combination of the IEquityDiscovery's concrete implementations based on provider_name.
     """
 
-    equity_discovery_implementations = {
+    providers_implementations = {
         "ssi": EquityDiscoverySsi(),
+        "vndirect": EquityDiscoveryVndirect(),
     }
 
     def get_provider(self, provider: str) -> IEquityDiscovery:
         """Returns a new concrete implementation of IEquityFundamental instance based on the provider name."""
 
-        if provider in self.equity_discovery_implementations:
-            return self.equity_discovery_implementations[provider]
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
         else:
             raise NotImplementedError(
                 f"Provider {provider} is not implemented yet."
             )
 
 
 class DerivativesFuturesFactory:
     """Factory class for Derivatives.Futures component.
 
     Factory represents a combination of the IDerivativesFutures's concrete implementations based on provider_name.
     """
 
-    derivatives_futures_providers_implementations = {
+    providers_implementations = {
         "vdsc": DerivativesFuturesVdsc(),
         "tcbs": DerivativesFuturesTcbs(),
+        "ssi": DerivativesFuturesSsi(),
     }
 
     def get_provider(self, provider: str) -> IDerivativesFutures:
         """Returns a new concrete implementation of IDerivativesFutures instance based on the provider name."""
 
-        if provider in self.derivatives_futures_providers_implementations:
-            return self.derivatives_futures_providers_implementations[provider]
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
+        else:
+            raise NotImplementedError(
+                f"Provider {provider} is not implemented yet."
+            )
+
+
+class DerivativesCoveredWarrantFactory:
+    """Factory class for Derivatives.CoveredWarrant component.
+
+    Factory represents a combination of the IDerivativesCoveredWarrant's concrete implementations based on provider_name.
+    """
+
+    providers_implementations = {
+        "ssi": DerivativesCoveredWarrantSsi(),
+    }
+
+    def get_provider(self, provider: str) -> IDerivativesCoveredWarrant:
+        """Returns a new concrete implementation of IDerivativesCoveredWarrant instance based on the provider name."""
+
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
         else:
             raise NotImplementedError(
                 f"Provider {provider} is not implemented yet."
             )
 
 
 class IndexFactory:
     """Factory class for Index component.
 
     Factory represents a combination of the IIndex's concrete implementations based on provider_name.
     """
 
-    index_providers_implementations = {
+    providers_implementations = {
         "ssi": IndexSsi(),
     }
 
     def get_provider(self, provider: str) -> IIndex:
         """Returns a new concrete implementation of IIndex instance based on the provider name."""
 
-        if provider in self.index_providers_implementations:
-            return self.index_providers_implementations[provider]
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
         else:
             raise NotImplementedError(
                 f"Provider {provider} is not implemented yet."
             )
 
 
 class IndexPriceFactory:
     """Factory class for Index.Price component.
 
     Factory represents a combination of the IIndexPrice's concrete implementations based on provider_name.
     """
 
-    index_price_implementations = {
+    providers_implementations = {
         "tcbs": IndexPriceTcbs(),
         "dnse": IndexPriceDnse(),
     }
 
     def get_provider(self, provider: str) -> IIndexPrice:
         """Returns a new concrete implementation of IIndexPrice instance based on the provider name."""
 
-        if provider in self.index_price_implementations:
-            return self.index_price_implementations[provider]
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
         else:
             raise NotImplementedError(
                 f"Provider {provider} is not implemented yet."
             )
 
 
 class EtfFactory:
     """Factory class for Etf component.
 
     Factory represents a combination of the IEtf's concrete implementations based on provider_name.
 
     """
 
-    etf_providers_implementations = {
+    providers_implementations = {
         "dnse": EtfDnse(),
         "tcbs": EtfTcbs(),
         "ssi": EtfSsi(),
     }
 
     def get_provider(self, provider: str) -> IEtf:
         """Returns a new concrete implementation of IEtf instance based on the provider name."""
 
-        if provider in self.etf_providers_implementations:
-            return self.etf_providers_implementations[provider]
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
         else:
             raise NotImplementedError(
                 f"Provider {provider} is not implemented yet."
             )
 
 
 class NewsFactory:
     """Factory class for News component.
 
     Factory represents a combination of the INews's concrete implementations based on provider_name.
     """
 
-    news_provider_implementations = {
+    providers_implementations = {
         "tcbs": NewsTcbs(),
     }
 
     def get_provider(self, provider: str) -> INews:
         """Returns a new concrete implementation of INews instance based on the provider name."""
 
-        if provider in self.news_provider_implementations:
-            return self.news_provider_implementations[provider]
+        if provider in self.providers_implementations:
+            return self.providers_implementations[provider]
         else:
             raise NotImplementedError(
                 f"Provider {provider} is not implemented yet."
             )
```

### Comparing `vietfin-0.1.0/src/vietfin/abstract/interface.py` & `vietfin-0.2.0/src/vietfin/abstract/interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,25 +67,28 @@
 
     @abstractmethod
     def major_holders(self, symbol: str) -> VfObject:
         """Equity Ownership Major Holders. Load major holders data for a specific ticker."""
         pass
 
     @abstractmethod
-    def foreign_trading(self, symbol: str, start_date: Any, end_date: Any) -> VfObject:
+    def foreign_trading(
+        self, symbol: str, start_date: Any, end_date: Any
+    ) -> VfObject:
         """Equity Ownership Foreign Trading. Load the trading data of foreign entities for a specific ticker."""
         pass
 
     @abstractmethod
-    def prop_trading(self, symbol: str, start_date: Any, end_date: Any) -> VfObject:
+    def prop_trading(
+        self, symbol: str, start_date: Any, end_date: Any
+    ) -> VfObject:
         """Equity Ownership Proprietary trading. Load the trading data of proprietary trading firms for a specific ticker."""
         pass
 
 
-
 class IEquityCalendar(ABC):
     """Interface for Equity Calendar component."""
 
     @abstractmethod
     def events(self, symbol: str, limit: int) -> VfObject:
         """Equity Calendar Events. Load Historical All-event-type Calendar data for a specific ticker."""
         pass
@@ -109,30 +112,31 @@
         """Equity Fundamental Dividends. Load Historical dividends data for a specific ticker."""
         pass
 
     @abstractmethod
     def income(self, symbol: str, period: Any) -> VfObject:
         """Equity Fundamental Income. Load Historical income statement data for a specific ticker."""
         pass
-    
+
     @abstractmethod
     def balance(self, symbol: str, period: Any) -> VfObject:
         """Equity Fundamental Balance. Load Historical balance sheet statement data for a specific ticker."""
         pass
-    
+
     @abstractmethod
     def cash(self, symbol: str, period: Any) -> VfObject:
         """Equity Fundamental Cash. Load Historical cash flow statement data for a specific ticker."""
         pass
 
     @abstractmethod
     def multiples(self, symbol: str, period: Any) -> VfObject:
         """Equity Fundamental Multiples. Load Historical valuation multiples data for a specific ticker."""
         pass
 
+
 class IEquityDiscovery(ABC):
     """Interface for Equity Discovery component."""
 
     @abstractmethod
     def active(self, exchange: Any) -> VfObject:
         """Equity Discovery Active. Load the list of most active stocks based on trading value."""
         pass
@@ -154,18 +158,32 @@
     def historical(
         self, symbol: str, start_date: Any, end_date: Any
     ) -> VfObject:
         """Derivatives Futures Historical. Load historical price data for a specific futures contract."""
         pass
 
     @abstractmethod
-    def quote(self, symbol: str, limit: int, cookie: str) -> VfObject:
+    def quote(self, symbol: str, limit: int) -> VfObject:
         """Derivatives Futures Quote. Load quote data for a specific futures contract."""
         pass
 
+    @abstractmethod
+    def search(self, symbol: str) -> VfObject:
+        """Derivatives Futures Search. Search for a specific futures contract."""
+        pass
+
+
+class IDerivativesCoveredWarrant(ABC):
+    """Interface for Derivatives Covered Warrant component."""
+
+    @abstractmethod
+    def search(self, symbol: str) -> VfObject:
+        """Derivatives Covered Warrant Search. Search for a specific covered warrant."""
+        pass
+
 
 class IIndex(ABC):
     """Interface for Index component."""
 
     @abstractmethod
     def search(self, symbol: str) -> VfObject:
         """Index Search. Search for an index."""
@@ -177,15 +195,17 @@
         pass
 
 
 class IIndexPrice(ABC):
     """Interface for Index Price component."""
 
     @abstractmethod
-    def historical(self, symbol: str, start_date: Any, end_date: Any, interval: Any) -> VfObject:
+    def historical(
+        self, symbol: str, start_date: Any, end_date: Any, interval: Any
+    ) -> VfObject:
         """Index Price Historical. Load historical price data for a specific index."""
         pass
 
 
 class IEtf(ABC):
     """Interface for Etf component."""
 
@@ -197,14 +217,15 @@
         pass
 
     @abstractmethod
     def search(self, symbol: str) -> VfObject:
         """Etf Search. Search for an ETF ticker."""
         pass
 
+
 class INews(ABC):
     """Interface for News component."""
 
     @abstractmethod
     def company(self, symbol: str, limit: int) -> VfObject:
         """News Company. Load company news data for a specific ticker."""
         pass
```

### Comparing `vietfin-0.1.0/src/vietfin/abstract/vfobject.py` & `vietfin-0.2.0/src/vietfin/abstract/vfobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
 
     def to_polars(self) -> "PolarsDataFrame":
         """Convert results field of the VfObject class to polars dataframe."""
         try:
             from polars import from_pandas  # type: ignore # pylint: disable=import-outside-toplevel
         except ImportError as exc:
             raise ImportError(
-                "Please install polars: `pip install polars pyarrow`  to use this method."
+                "Please install polars: `poetry add polars pyarrow` to use this method."
             ) from exc
 
         return from_pandas(self.to_df(index=None))
 
     def to_csv(self, file_path: str) -> None:
         """Write results field of the VfObject class to a csv file.
```

### Comparing `vietfin-0.1.0/src/vietfin/components/derivatives.py` & `vietfin-0.2.0/src/vietfin/components/equity_price.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,52 @@
-"""VietFin Derivatives class."""
+"""VietFin Equity.Price class."""
 
 from typing import Literal
 
 from vietfin.abstract.vfobject import VfObject
-from vietfin.abstract.factory import DerivativesFuturesFactory
-from vietfin.abstract.interface import IDerivativesFutures
+from vietfin.abstract.factory import EquityPriceFactory
+from vietfin.abstract.interface import IEquityPrice
+from vietfin.utils.helpers import INTERVALS
 
 
-class Derivatives:
-    """VietFin Derivatives related group of commands."""
+class EquityPrice:
+    """VietFin Equity.Price-related group of commands.
 
-    def __init__(self) -> None:
-        self.futures = DerivativesFutures()
-
-
-class DerivativesFutures:
-    """VietFin Derivatives.Futures-related group of commands."""
+    This is the Client code in Factory Design Pattern.
+    """
 
     # list of implemented providers
-    PROVIDERS = Literal["tcbs", "vdsc"]
+    PROVIDERS = Literal["tcbs", "dnse", "ssi"]
 
     @staticmethod
-    def _get_provider(provider: PROVIDERS) -> IDerivativesFutures:
+    def _get_provider(provider: PROVIDERS) -> IEquityPrice:
         provider_name = provider.lower()
-        return DerivativesFuturesFactory().get_provider(provider_name)
+        return EquityPriceFactory().get_provider(provider_name)
 
     def historical(
         self,
         symbol: str,
         start_date: str | None = None,
         end_date: str | None = None,
+        interval: INTERVALS = "1d",
         provider: PROVIDERS = "tcbs",
     ) -> VfObject:
-        """Futures Historical price. Load Futures Historical data for a specific futures contract."""
+        """Equity Historical price. Load stock historical price data for a specific ticker."""
 
         provider_instance = self._get_provider(provider)
         return provider_instance.historical(
             symbol=symbol,
             start_date=start_date,  # type: ignore
             end_date=end_date,  # type: ignore
+            interval=interval,
         )
 
     def quote(
-        self,
-        symbol: str,
-        cookie: str,
-        limit: int = 100,
-        provider: PROVIDERS = "vdsc",
+        self, symbol: str, limit: int = 100, provider: PROVIDERS = "tcbs"
     ) -> VfObject:
-        """Futures Quote. Load Futures quote for a specific futures contract."""
+        """Equity Quote. Load quote data for a specific ticker."""
 
         provider_instance = self._get_provider(provider)
         return provider_instance.quote(
             symbol=symbol,
             limit=limit,
-            cookie=cookie,
         )
```

### Comparing `vietfin-0.1.0/src/vietfin/components/equity.py` & `vietfin-0.2.0/src/vietfin/components/equity.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/components/equity_calendar.py` & `vietfin-0.2.0/src/vietfin/components/equity_calendar.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/components/equity_discovery.py` & `vietfin-0.2.0/src/vietfin/components/equity_discovery.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 """VietFin Equity.Discovery class."""
 
 from typing import Literal
 
 from vietfin.abstract.vfobject import VfObject
 from vietfin.abstract.factory import EquityDiscoveryFactory
 from vietfin.abstract.interface import IEquityDiscovery
-from vietfin.providers.ssi.utils.equity_discovery import EXCHANGE_NAMES
+from vietfin.utils.helpers import EXCHANGE_NAMES
 
 
 class EquityDiscovery:
     """VietFin Equity.Discovery-related group of commands."""
 
     # list of implemented providers
-    PROVIDERS = Literal["ssi"]
+    PROVIDERS = Literal["vndirect"]
 
     @staticmethod
     def _get_provider(provider: PROVIDERS) -> IEquityDiscovery:
         provider_name = provider.lower()
         return EquityDiscoveryFactory().get_provider(provider_name)
 
     def active(
-        self, exchange: EXCHANGE_NAMES = "ALL", provider: PROVIDERS = "ssi"
+        self, exchange: EXCHANGE_NAMES = "hose", provider: PROVIDERS = "vndirect"
     ) -> VfObject:
         """Equity Discovery Active. Load the list of most active stocks based on trading value."""
 
         provider_instance = self._get_provider(provider)
         return provider_instance.active(exchange=exchange)
 
     def gainers(
-        self, exchange: EXCHANGE_NAMES = "ALL", provider: PROVIDERS = "ssi"
+        self, exchange: EXCHANGE_NAMES = "hose", provider: PROVIDERS = "vndirect"
     ) -> VfObject:
         """Equity Discovery Gainers. Load the list of top gainer stocks."""
 
         provider_instance = self._get_provider(provider)
         return provider_instance.gainers(exchange=exchange)
 
-    @staticmethod
     def losers(
-        self, exchange: EXCHANGE_NAMES = "ALL", provider: PROVIDERS = "ssi"
+        self, exchange: EXCHANGE_NAMES = "hose", provider: PROVIDERS = "vndirect"
     ) -> VfObject:
         """Equity Discovery Losers. Load the list of top loser stocks."""
 
         provider_instance = self._get_provider(provider)
         return provider_instance.losers(exchange=exchange)
```

### Comparing `vietfin-0.1.0/src/vietfin/components/equity_fundamental.py` & `vietfin-0.2.0/src/vietfin/components/equity_fundamental.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/components/equity_ownership.py` & `vietfin-0.2.0/src/vietfin/components/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/components/equity_price.py` & `vietfin-0.2.0/src/vietfin/components/etf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-"""VietFin Equity.Price class."""
+"""VietFin Etf class."""
 
 from typing import Literal
 
 from vietfin.abstract.vfobject import VfObject
-from vietfin.abstract.factory import EquityPriceFactory
-from vietfin.abstract.interface import IEquityPrice
+from vietfin.abstract.factory import EtfFactory
+from vietfin.abstract.interface import IEtf
 from vietfin.utils.helpers import INTERVALS
 
 
-class EquityPrice:
-    """VietFin Equity.Price-related group of commands.
-
-    This is the Client code in Factory Design Pattern.
-    """
+class Etf:
+    """VietFin ETF-related group of commands."""
 
     # list of implemented providers
     PROVIDERS = Literal["tcbs", "dnse", "ssi"]
 
     @staticmethod
-    def _get_provider(provider: PROVIDERS) -> IEquityPrice:
+    def _get_provider(provider: PROVIDERS) -> IEtf:
         provider_name = provider.lower()
-        return EquityPriceFactory().get_provider(provider_name)
+        return EtfFactory().get_provider(provider_name)
 
     def historical(
         self,
         symbol: str,
         start_date: str | None = None,
         end_date: str | None = None,
         interval: INTERVALS = "1d",
-        provider: PROVIDERS = "tcbs",
+        provider: PROVIDERS = "ssi",
     ) -> VfObject:
-        """Equity Historical price. Load stock historical price data for a specific ticker."""
+        """ETF Historical price. Load historical price data of a specific ETF ticker."""
 
         provider_instance = self._get_provider(provider)
         return provider_instance.historical(
             symbol=symbol,
             start_date=start_date,  # type: ignore
             end_date=end_date,  # type: ignore
             interval=interval,
         )
 
-    def quote(
-        self, symbol: str, limit: int = 100, provider: PROVIDERS = "tcbs"
+    def search(
+        self,
+        symbol: str = "",
+        provider: PROVIDERS = "ssi",
     ) -> VfObject:
-        """Equity Quote. Load quote data for a specific ticker."""
+        """Etf Search. Search for an ETF ticker.
+
+        An empty string (by default) returns the full list of currently listed ETFs.
+        """
 
         provider_instance = self._get_provider(provider)
-        return provider_instance.quote(
-            symbol=symbol,
-            limit=limit,
-        )
+        return provider_instance.search(symbol=symbol)
```

### Comparing `vietfin-0.1.0/src/vietfin/components/etf.py` & `vietfin-0.2.0/src/vietfin/components/funds.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,57 @@
-"""VietFin Etf class."""
+"""VietFin Funds class."""
 
 from typing import Literal
 
 from vietfin.abstract.vfobject import VfObject
-from vietfin.abstract.factory import EtfFactory
-from vietfin.abstract.interface import IEtf
-from vietfin.utils.helpers import INTERVALS
+from vietfin.abstract.factory import FundsFactory
+from vietfin.abstract.interface import IFunds
 
 
-class Etf:
-    """VietFin ETF-related group of commands."""
+class Funds:
+    """VietFin Funds-related group of commands.
+
+    This is the Client code in Factory Design Pattern.
+    """
 
     # list of implemented providers
-    PROVIDERS = Literal["tcbs", "dnse", "ssi"]
+    PROVIDERS = Literal["fmarket"]
 
     @staticmethod
-    def _get_provider(provider: PROVIDERS) -> IEtf:
+    def _get_provider(provider: PROVIDERS) -> IFunds:
         provider_name = provider.lower()
-        return EtfFactory().get_provider(provider_name)
+        return FundsFactory().get_provider(provider_name)
+
+    def search(
+        self, symbol: str = "", provider: PROVIDERS = "fmarket"
+    ) -> VfObject:
+        """Funds Search. Search for a fund.
+
+        An empty query (by default) returns the list of all funds from selected provider.
+        """
+
+        provider_instance = self._get_provider(provider)
+        return provider_instance.search(symbol=symbol)
 
     def historical(
         self,
         symbol: str,
         start_date: str | None = None,
         end_date: str | None = None,
-        interval: INTERVALS = "1d",
-        provider: PROVIDERS = "ssi",
+        provider: PROVIDERS = "fmarket",
     ) -> VfObject:
-        """ETF Historical price. Load historical price data of a specific ETF ticker."""
+        """Funds Historical price. Load historical NAV for a specific fund."""
 
         provider_instance = self._get_provider(provider)
         return provider_instance.historical(
             symbol=symbol,
             start_date=start_date,  # type: ignore
             end_date=end_date,  # type: ignore
-            interval=interval,
         )
 
-    def search(
-        self,
-        symbol: str = "",
-        provider: PROVIDERS = "ssi",
+    def holdings(
+        self, symbol: str, provider: PROVIDERS = "fmarket"
     ) -> VfObject:
-        """Etf Search. Search for an ETF ticker.
-
-        An empty string (by default) returns the full list of currently listed ETFs.
-        """
+        """Funds Holdings. Load the top 10 holdings for a specific fund."""
 
         provider_instance = self._get_provider(provider)
-        return provider_instance.search(symbol=symbol)
+        return provider_instance.holdings(symbol=symbol)
```

### Comparing `vietfin-0.1.0/src/vietfin/components/funds.py` & `vietfin-0.2.0/src/vietfin/components/index.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,73 @@
-"""VietFin Funds class."""
+"""VietFin Index class."""
 
 from typing import Literal
 
 from vietfin.abstract.vfobject import VfObject
-from vietfin.abstract.factory import FundsFactory
-from vietfin.abstract.interface import IFunds
+from vietfin.abstract.factory import IndexFactory, IndexPriceFactory
+from vietfin.abstract.interface import IIndex, IIndexPrice
+from vietfin.utils.helpers import INTERVALS
 
 
-class Funds:
-    """VietFin Funds-related group of commands.
-
-    This is the Client code in Factory Design Pattern.
-    """
+class IndexPrice:
+    """VietFin Index.Price-related group of commands."""
 
     # list of implemented providers
-    PROVIDERS = Literal["fmarket"]
+    PROVIDERS = Literal["tcbs", "dnse"]
 
     @staticmethod
-    def _get_provider(provider: PROVIDERS) -> IFunds:
+    def _get_provider(provider: PROVIDERS) -> IIndexPrice:
         provider_name = provider.lower()
-        return FundsFactory().get_provider(provider_name)
-
-    def search(
-        self, symbol: str = "", provider: PROVIDERS = "fmarket"
-    ) -> VfObject:
-        """Funds Search. Search for a fund.
-
-        An empty query (by default) returns the list of all funds from selected provider.
-        """
-
-        provider_instance = self._get_provider(provider)
-        return provider_instance.search(symbol=symbol)
+        return IndexPriceFactory().get_provider(provider_name)
 
     def historical(
         self,
         symbol: str,
         start_date: str | None = None,
         end_date: str | None = None,
-        provider: PROVIDERS = "fmarket",
+        interval: INTERVALS = "1d",
+        provider: PROVIDERS = "tcbs",
     ) -> VfObject:
-        """Funds Historical price. Load historical NAV for a specific fund."""
+        """Index Historical price. Load historical price data for a specific index."""
 
         provider_instance = self._get_provider(provider)
         return provider_instance.historical(
             symbol=symbol,
             start_date=start_date,  # type: ignore
             end_date=end_date,  # type: ignore
+            interval=interval,
         )
 
-    def holdings(
-        self, symbol: str, provider: PROVIDERS = "fmarket"
+
+class Index:
+    """VietFin Index-related group of commands.
+
+    This is the Client code in Factory Design Pattern.
+    """
+
+    # list of implemented providers
+    PROVIDERS = Literal["ssi"]
+
+    def __init__(self) -> None:
+        self.price = IndexPrice()
+
+    @staticmethod
+    def _get_provider(provider: PROVIDERS) -> IIndex:
+        provider_name = provider.lower()
+        return IndexFactory().get_provider(provider_name)
+
+    def search(self, symbol: str = "", provider: PROVIDERS = "ssi") -> VfObject:
+        """Index Search. Search for an index.
+
+        An empty query (by default) returns the list of all available indexes from selected provider.
+        """
+
+        provider_instance = self._get_provider(provider)
+        return provider_instance.search(symbol=symbol)
+
+    def constituents(
+        self, symbol: str, provider: PROVIDERS = "ssi"
     ) -> VfObject:
-        """Funds Holdings. Load the top 10 holdings for a specific fund."""
+        """Index Constituents. Load the constituents for a specific index."""
 
         provider_instance = self._get_provider(provider)
-        return provider_instance.holdings(symbol=symbol)
+        return provider_instance.constituents(symbol=symbol)
```

### Comparing `vietfin-0.1.0/src/vietfin/components/news.py` & `vietfin-0.2.0/src/vietfin/components/news.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/cafef/models/equity_ownership_foreign.py` & `vietfin-0.2.0/src/vietfin/providers/cafef/models/equity_ownership_foreign.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/cafef/models/equity_ownership_prop.py` & `vietfin-0.2.0/src/vietfin/providers/cafef/models/equity_ownership_prop.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/cafef/provider.py` & `vietfin-0.2.0/src/vietfin/providers/cafef/provider.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/cafef/utils/equity_ownership_foreign.py` & `vietfin-0.2.0/src/vietfin/providers/cafef/utils/equity_ownership_foreign.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # """Cafef Equity Ownership Foreign Trading command."""
 
-import requests
+import httpx as requests
 
 from vietfin.providers.cafef.utils.helpers import cafef_headers
 from vietfin.providers.cafef.models.equity_ownership_foreign import (
     CafefEquityOwnershipForeignTradingData,
 )
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
@@ -71,32 +71,33 @@
     page_size = 20
     trading_data = []
     url_list = []
     data = []
 
     while True:
         url = f"https://s.cafef.vn/Ajax/PageNew/DataHistory/GDKhoiNgoai.ashx?Symbol={symbol}&StartDate={start_date}&EndDate={end_date}&PageIndex={page_index}&PageSize={page_size}"
-        response = requests.get(url, headers=cafef_headers)        
-        check_response_error(response)        
+        response = requests.get(url, headers=cafef_headers)
+        check_response_error(response)
         data_chunk = response.json()
         rows = data_chunk.get("Data", {}).get("Data", [])
 
         if not rows:
             break  # stop if no more data
 
         url_list.append(url)
         data.append(data_chunk)
 
         # Unpack dictionary to data model and return the results
-        trading_data.extend([CafefEquityOwnershipForeignTradingData(**r) for r in rows])
+        trading_data.extend(
+            [CafefEquityOwnershipForeignTradingData(**r) for r in rows]
+        )
 
         # increment page_index to continue fetching until no more data
         page_index += 1
 
-
     if not trading_data:
         raise EmptyDataError
 
     # Additional metadata about the command run
     extra = generate_extra_metadata(
         symbol=symbol,
         result=trading_data,
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/cafef/utils/equity_ownership_prop.py` & `vietfin-0.2.0/src/vietfin/providers/cafef/utils/equity_ownership_prop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # """Cafef Equity Ownership Proprietary Trading command."""
 
-import requests
+import httpx as requests
 
 from vietfin.providers.cafef.utils.helpers import cafef_headers
 from vietfin.providers.cafef.models.equity_ownership_prop import (
     CafefEquityOwnershipPropTradingData,
 )
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/cafef/utils/helpers.py` & `vietfin-0.2.0/src/vietfin/providers/cafef/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/dnse/models/equity_price_historical.py` & `vietfin-0.2.0/src/vietfin/providers/dnse/models/equity_price_historical.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """DNSE Equity Historical Price Model."""
 
-from datetime import date, datetime
+from datetime import date, datetime, timezone
 from typing import Any
 
 from pydantic import field_validator, model_validator
 
 from vietfin.abstract.data import Data
 
 
@@ -28,15 +28,15 @@
     volume: int
 
     @model_validator(mode="before")
     @classmethod
     def parse_unix_timestamp(cls, data: Any) -> Any:
         """Before model validators are applied, parse the raw input, convert the value of `t` key from unix timestamp to date."""
         if isinstance(data, dict):
-            data["t"] = datetime.utcfromtimestamp(data["t"]).date()
+            data["t"] = datetime.fromtimestamp(data["t"], tz=timezone.utc).date()
         return data
 
     @field_validator("open", "high", "low", "close")
     @classmethod
     def multiply_1k(cls, value: float) -> float:
         """Multiply the price value by 1000."""
         return value * 1000
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/dnse/provider.py` & `vietfin-0.2.0/src/vietfin/providers/dnse/provider.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/dnse/utils/equity_price_historical.py` & `vietfin-0.2.0/src/vietfin/providers/dnse/utils/equity_price_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """DNSE Equity Price Historical command."""
 
 from datetime import datetime, timedelta
 from typing import Literal
 
-import requests
+import httpx as requests
 from pydantic import field_validator, model_validator
 
 from vietfin.providers.dnse.utils.helpers import dnse_headers
 from vietfin.providers.dnse.models.equity_price_historical import (
     DnseEquityHistoricalPriceData,
 )
 from vietfin.abstract.vfobject import VfObject
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/dnse/utils/helpers.py` & `vietfin-0.2.0/src/vietfin/providers/dnse/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/fmarket/models/fund_asset_types.py` & `vietfin-0.2.0/src/vietfin/providers/fmarket/models/fund_asset_types.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/fmarket/models/fund_historical_nav_performance.py` & `vietfin-0.2.0/src/vietfin/providers/fmarket/models/fund_historical_nav_performance.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/fmarket/models/fund_holdings.py` & `vietfin-0.2.0/src/vietfin/providers/fmarket/models/fund_holdings.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/fmarket/models/fund_search.py` & `vietfin-0.2.0/src/vietfin/providers/fmarket/models/fund_search.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/fmarket/provider.py` & `vietfin-0.2.0/src/vietfin/providers/fmarket/provider.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/fmarket/utils/funds_historical.py` & `vietfin-0.2.0/src/vietfin/providers/fmarket/utils/funds_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Fmarket Funds Historical function."""
 
 from datetime import datetime
-import requests
+import httpx as requests
 from pydantic import model_validator
 
 from vietfin.providers.fmarket.utils.helpers import fmarket_headers, get_fund_id
 from vietfin.providers.fmarket.models.fund_historical_nav import (
     FmarketFundHistoricalNavData,
 )
 from vietfin.abstract.vfobject import VfObject
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/fmarket/utils/funds_holdings.py` & `vietfin-0.2.0/src/vietfin/providers/fmarket/utils/funds_holdings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Fmarket Funds Top Holdings function."""
 
-import requests
+import httpx as requests
 
 from vietfin.abstract.vfobject import VfObject
 from vietfin.providers.fmarket.utils.helpers import fmarket_headers, get_fund_id
 from vietfin.providers.fmarket.models.fund_holdings import (
     FmarketFundHoldingsData,
 )
 from vietfin.utils.helpers import generate_extra_metadata, check_response_error, BaseOtherParams
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/fmarket/utils/funds_search.py` & `vietfin-0.2.0/src/vietfin/providers/fmarket/utils/funds_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Fmarket Funds Search function."""
 
-import requests
+import httpx as requests
 from pydantic import BaseModel, ConfigDict, field_validator
 
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import generate_extra_metadata, check_response_error
 from vietfin.providers.fmarket.models.fund_search import FmarketFundInfoData
 from vietfin.providers.fmarket.utils.helpers import fmarket_headers
 from vietfin.utils.errors import EmptyDataError
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/fmarket/utils/helpers.py` & `vietfin-0.2.0/src/vietfin/providers/fmarket/utils/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Fmarket utils."""
 
-import json
-
-import requests
+import httpx as requests
 
 from vietfin.utils.errors import VietFinError
 
 
 # Requests headers
 
 fmarket_headers = {
@@ -42,21 +40,20 @@
     """
 
     payload = {
         "searchField": symbol,
         "types": ["NEW_FUND", "TRADING_FUND"],
         "pageSize": 100,
     }
-    payload = json.dumps(payload)  # type: ignore
 
     url = "https://api.fmarket.vn/res/products/filter"
-    response = requests.post(url, headers=fmarket_headers, data=payload)
+    response = requests.post(url, headers=fmarket_headers, json=payload)
 
     if response.status_code != 200:
-        raise requests.exceptions.HTTPError(
+        raise requests.HTTPError(
             f"Error in API response: {response.status_code} - {response.text}"
         )
 
     data = response.json()
 
     # This logic is handcrafted for the data structure of response from the API
     if data["data"]["total"] == 0:
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/models/equity_discovery.py` & `vietfin-0.2.0/src/vietfin/providers/vndirect/models/equity_discovery.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-"""Ssi Equity Discovery group of Models."""
+"""VNDIRECT Equity Discovery group of Models."""
+
+from datetime import datetime
 
 from vietfin.abstract.data import Data
 
 
-class SsiEquityDiscoveryData(Data):
-    """Ssi Equity Discovery Data. Most top mover stocks based on certain criteria."""
+class VndirectEquityDiscoveryData(Data):
+    """VNDIRECT Equity Discovery Data. Most top mover stocks based on certain criteria."""
 
     __alias_dict__ = {
-        "symbol": "ticker",
-        "price": "price",
-        "change": "priceChange",
-        "percent_change": "percentPriceChange",
-        "volume": "volume",
-        "trading_value": "value",
-        "industry": "sectorName",
+        "symbol": "code",
+        "price": "lastPrice",
+        "change": "priceChgCr1D",
+        "percent_change": "priceChgPctCr1D",
+        "volume": "totalVolumeAvgCr20D",
+        "trading_value": "accumulatedVal",
+        "updated_at": "lastUpdated",
     }
 
-    symbol: str  # Symbol representing the entity requested in the data.
+    symbol: str  # Symbol representing the stock satisfying the criteria.
     price: float  # Last price of the stock.
     change: float  # Change in price value.
     percent_change: float  # Percent change in price value.
-    volume: int  # Trading volume.
-    trading_value: float  # Trading value, i.e. price * volume
-    industry: str  # Operating industry of the company.
+    volume: float  # Trading volume averaged over 20 days.
+    trading_value: float  # Trading value, i.e. price * volume, unit VND.
+    updated_at: datetime  # Date and time of the last data update.
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/models/equity_search.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/models/etf_historical.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/models/etf_historical.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """SSI Etf Historical Model."""
 
-from datetime import date, datetime
+from datetime import date, datetime, timezone
 from typing import Any
 
 from pydantic import field_validator, model_validator
 
 from vietfin.abstract.data import Data
 
 
@@ -28,15 +28,15 @@
     volume: int
 
     @model_validator(mode="before")
     @classmethod
     def parse_unix_timestamp(cls, data: Any) -> Any:
         """Before model validators are applied, parse the raw input, convert the value of `t` key from unix timestamp to date."""
         if isinstance(data, dict):
-            data["t"] = datetime.utcfromtimestamp(data["t"]).date()
+            data["t"] = datetime.fromtimestamp(data["t"], tz=timezone.utc).date()
         return data
 
     @field_validator("open", "high", "low", "close")
     @classmethod
     def multiply_1k(cls, value: float) -> float:
         """Multiply the price value by 1000."""
         return value * 1000
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/models/etf_search.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/models/index_constituents.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/provider.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,27 +4,39 @@
 from vietfin.abstract.interface import (
     IEquity,
     IIndex,
     IEquityDiscovery,
     IEquityFundamental,
     IEtf,
     IEquityPrice,
+    IDerivativesFutures,
+    IDerivativesCoveredWarrant,
 )
 from vietfin.abstract.vfobject import VfObject
+from vietfin.utils.helpers import PERIODS, EXCHANGE_NAMES
 from vietfin.providers.ssi.utils.equity_search import search as equity_search
 from vietfin.providers.ssi.utils.index_search import search as index_search
 from vietfin.providers.ssi.utils.equity_discovery import (
     get_top_movers,
-    EXCHANGE_NAMES,
 )
 from vietfin.providers.ssi.utils.etf_search import search as etf_search
 from vietfin.providers.ssi.utils.etf_historical import historical
 from vietfin.providers.ssi.utils.index_constituents import constituents
-from vietfin.utils.helpers import PERIODS
-from vietfin.providers.ssi.utils.equity_fundamental_income import get_financial_report
+from vietfin.providers.ssi.utils.equity_fundamental_income import (
+    get_financial_report,
+)
+from vietfin.providers.ssi.utils.derivatives_futures_search import (
+    search as futures_search,
+)
+from vietfin.providers.ssi.utils.derivatives_futures_quote import (
+    quote as futures_quote,
+)
+from vietfin.providers.ssi.utils.derivatives_coveredwarrant_search import (
+    search as cw_search,
+)
 
 
 class EquitySsi(IEquity):
     """The concrete implementation of Equity component with Ssi as provider."""
 
     def search(self, symbol: str) -> VfObject:
         """Equity Search. Search for a stock ticker."""
@@ -63,24 +75,24 @@
 
 
 class EquityDiscoverySsi(IEquityDiscovery):
     """The concrete implementation of Equity Discovery component with Ssi as provider."""
 
     def active(self, exchange: EXCHANGE_NAMES) -> VfObject:
         """Equity Discovery Active. Load the list of most active stocks based on trading value."""
-        return get_top_movers(name="Value", exchange=exchange)
+        return get_top_movers(name="value", exchange=exchange)
 
     def gainers(self, exchange: EXCHANGE_NAMES) -> VfObject:
         """Equity Discovery Gainers. Load the list of top gainer stocks."""
-        return get_top_movers(name="Gainers", exchange=exchange)
+        return get_top_movers(name="gainers", exchange=exchange)
 
     def losers(self, exchange: EXCHANGE_NAMES) -> VfObject:
         """Equity Discovery Losers. Load the list of top loser stocks."""
-        return get_top_movers(name="Losers", exchange=exchange)
-    
+        return get_top_movers(name="losers", exchange=exchange)
+
 
 class EquityFundamentalSsi(IEquityFundamental):
     """The concrete implementation of Equity.Fundamental component with Ssi as provider."""
 
     def management(self, symbol: str) -> VfObject:
         """Equity Fundamental Management. Load Key executives data for a specific ticker."""
         raise NotImplementedError(
@@ -94,27 +106,29 @@
         )
 
     def dividends(self, symbol: str, limit: int) -> VfObject:
         """Equity Fundamental Dividends. Load Historical dividends data for a specific ticker."""
         raise NotImplementedError(
             "equity.fundamental.dividends() command is not implemented for SSI provider."
         )
-    
+
     def income(self, symbol: str, period: PERIODS) -> VfObject:
         """Equity Fundamental Income. Load Historical income statement data for a specific ticker."""
         return get_financial_report(symbol=symbol, period=period, name="income")
-    
+
     def balance(self, symbol: str, period: PERIODS) -> VfObject:
         """Equity Fundamental Balance. Load Historical balance sheet statement data for a specific ticker."""
-        return get_financial_report(symbol=symbol, period=period, name="balance")
-    
+        return get_financial_report(
+            symbol=symbol, period=period, name="balance"
+        )
+
     def cash(self, symbol: str, period: PERIODS) -> VfObject:
         """Equity Fundamental Cash. Load Historical cash flow statement data for a specific ticker."""
         return get_financial_report(symbol=symbol, period=period, name="cash")
-    
+
     def multiples(self, symbol: str, period: PERIODS) -> VfObject:
         """Equity Fundamental Multiples. Load Historical valuation multiples data for a specific ticker."""
         raise NotImplementedError(
             "equity.fundamental.multiples() command is not implemented for SSI provider."
         )
 
 
@@ -143,7 +157,39 @@
     ) -> VfObject:
         return historical(
             symbol=symbol,
             start_date=start_date,
             end_date=end_date,
             interval=interval,
         )
+
+
+class DerivativesFuturesSsi(IDerivativesFutures):
+    """The concrete implementation of Derivatives.Futures component with SSI as provider."""
+
+    def historical(
+        self, symbol: str, start_date: str, end_date: str
+    ) -> VfObject:
+        """Derivatives Futures Historical. Load historical price data for a specific futures contract."""
+
+        raise NotImplementedError(
+            "derivatives.futures.historical() command is not implemented for SSI provider."
+        )
+
+    def quote(self, symbol: str, limit: int) -> VfObject:
+        """Derivatives Futures Quote. Load quote data for a specific futures contract."""
+
+        return futures_quote(symbol=symbol, limit=limit)
+
+    def search(self, symbol: str) -> VfObject:
+        """Derivatives Futures Search. Search for a specific futures contract."""
+
+        return futures_search(symbol=symbol)
+
+
+class DerivativesCoveredWarrantSsi(IDerivativesCoveredWarrant):
+    """The concrete implementation of Derivatives.CoveredWarrant component with SSI as provider."""
+
+    def search(self, symbol: str) -> VfObject:
+        """Derivatives Covered Warrant Search. Search for a specific covered warrant."""
+
+        return cw_search(symbol=symbol)
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/utils/equity_discovery.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/utils/equity_discovery.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """SSI Equity Discovery group of functions."""
 
-import requests
-from typing import Literal
+import httpx as requests
 
 from vietfin.abstract.vfobject import VfObject
-from vietfin.utils.helpers import generate_extra_metadata, check_response_error
+from vietfin.utils.helpers import (
+    generate_extra_metadata,
+    check_response_error,
+    TOP_MOVERS_REPORT_NAMES,
+    EXCHANGE_NAMES,
+    BaseOtherParams,
+)
 from vietfin.providers.ssi.utils.helpers import ssi_headers
 from vietfin.providers.ssi.models.equity_discovery import SsiEquityDiscoveryData
 from vietfin.utils.errors import EmptyDataError
 
 
-REPORT_NAMES = Literal["Gainers", "Losers", "Value"]
-EXCHANGE_NAMES = Literal["HOSE", "HNX", "UPCOM", "ALL"]
-
-
-def get_top_movers(name: REPORT_NAMES, exchange: EXCHANGE_NAMES) -> VfObject:
+def get_top_movers(
+    name: TOP_MOVERS_REPORT_NAMES, exchange: EXCHANGE_NAMES
+) -> VfObject:
     """Equity Discovery. Retrieve a report from SSI provider.
 
     Parameters
     ----------
     name : str
-        name of the report. Options: Literal["Gainers", "Losers", "Value"]
+        name of the report.
     exchange : srt
-        name of the exchange. Options: Literal["HOSE", "HNX", "UPCOM", "ALL"]
+        name of the exchange.
 
     Returns
     -------
     VfObject
         results : list[SsiEquityDiscoveryData]
             list of stock tickers listed the specific report.
         provider : str
@@ -39,17 +42,39 @@
     Raises
     ------
     HttpError
         if the API call failed
     EmptyDataError
         if the API response is empty
     """
+    # Validate input
+    params = BaseOtherParams(top_movers_report=name, exchange=exchange)
+    name = params.top_movers_report
+    exchange = params.exchange
+
+    # Map user friendly string to API value
+    name_mapping = {
+        "gainers": "Gainers",
+        "losers": "Losers",
+        "value": "Value",
+    }
+    name_api = name_mapping.get(name)
+
+    exchange_mapping = {
+        "hose": "HOSE",
+        "hnx": "HNX",
+        "upcom": "UPCOM",
+        "all": "ALL",
+    }
+    exchange_api = exchange_mapping.get(exchange)
+    if not exchange_api:
+        raise ValueError(f"Exchange {exchange} is not supported by this provider SSI.")
 
     # API call
-    url = f"https://fiin-market.ssi.com.vn/TopMover/GetTop{name}?language=vi&ComGroupCode={exchange}"
+    url = f"https://fiin-market.ssi.com.vn/TopMover/GetTop{name_api}?language=vi&ComGroupCode={exchange_api}"
     response = requests.get(url, headers=ssi_headers)
     check_response_error(response)
     data = response.json()
     rows = data.get("items", [])
 
     if not rows:
         raise EmptyDataError(
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/utils/equity_fundamental_income.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/utils/equity_fundamental_income.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """SSI Equity Fundamental Income command."""
 
 from datetime import datetime
 from io import BytesIO
 import re
 
-import requests
+import httpx as requests
 import pandas as pd
 
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
     check_response_error,
     generate_extra_metadata,
     PERIODS,
@@ -86,15 +86,15 @@
     number_periods = 100  # i.e. retrieve 100 years or 100 quarters of data
     current_year = str(datetime.now().year)
 
     url = f"https://fiin-fundamental.ssi.com.vn/FinancialStatement/Download{name_api}?language=en&OrganCode={organ_code}&Skip=0&Frequency={period_api}&numberOfPeriod={number_periods}&latestYear={current_year}"
     response = requests.get(url, headers=ssi_headers)
     check_response_error(response)
 
-    # Parse API response then remove the first 7 rows and last 3 rows
+    # Parse API response then remove the first 7 rows and the last 3 rows
     df = pd.read_excel(BytesIO(response.content), skiprows=7)
     df = df.iloc[:-3]
 
     if df.empty:
         raise EmptyDataError(f"No data found for the symbol {symbol}.")
 
     # Make column labels of cashflow statement similar to other two statements
@@ -103,23 +103,25 @@
 
     # Prepare raw_data for VfObject
     raw = df.to_dict(orient="list")
 
     # Add 'period' column
     df["period"] = period
 
-    # Unpivot the DataFrame
-    # This regex match any string that starts with 'Q' followed by 1 or 2 digits and a space,
-    # then ends with 4 digits (for quarters) or just 4 digits (for years)
+
+    # This regex match any string that starts with 'Q' followed by 1 or 2 digits and a space then ends with 4 digits (for quarters, e.g. Q01 2023)
+    # or just 4 digits (for years, e.g. 2023)
     year_quarter_regex = re.compile(r"^(Q\d{1,2}\s)?\d{4}$")
+
     # Identify column labels that represent years or quarters
     period_columns = [
         col for col in df.columns if year_quarter_regex.match(col)
     ]
 
+    # Unpivot the DataFrame
     df = pd.melt(
         df,
         id_vars=["ITEMS", "period"],
         value_vars=period_columns,
         var_name="fiscal_period",
         value_name="values",
     )
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/utils/equity_search.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/utils/equity_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """SSI Equity Search function."""
 
-import requests
+import httpx as requests
 
 from vietfin.providers.ssi.utils.helpers import ssi_headers
 from vietfin.abstract.vfobject import VfObject
 from vietfin.providers.ssi.models.equity_search import SsiEquitySearchData
 from vietfin.utils.helpers import generate_extra_metadata, check_response_error
 from vietfin.utils.errors import EmptyDataError
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/utils/etf_historical.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/utils/etf_historical.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """SSI Etf Historical function."""
 
 from datetime import datetime, timedelta
 
-import requests
+import httpx as requests
 from pydantic import field_validator, model_validator
 
 from vietfin.providers.ssi.utils.helpers import ssi_headers
 from vietfin.abstract.vfobject import VfObject
 from vietfin.providers.ssi.models.etf_historical import SsiEtfHistoricalData
 from vietfin.utils.helpers import (
     generate_extra_metadata,
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/utils/etf_search.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/utils/etf_search.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """SSI Etf Search function."""
 
-import requests
+import httpx as requests
 
 from vietfin.providers.ssi.utils.helpers import ssi_headers
 from vietfin.abstract.vfobject import VfObject
 from vietfin.providers.ssi.models.etf_search import SsiEtfSearchData
 from vietfin.utils.helpers import generate_extra_metadata, check_response_error
 from vietfin.utils.errors import EmptyDataError
 
@@ -46,15 +46,15 @@
     check_response_error(response)
     data = response.json()
     rows = data["data"]
 
     if not rows:
         raise EmptyDataError
 
-    # Filter results based on the provided symbol if it's not an empty string
+    # Filter results by comparing the provided symbol to the value of key "ss"
     if symbol:
         rows = [r for r in rows if r.get("ss", "").upper() == symbol.upper()]
 
         if not rows:
             raise EmptyDataError(f"No data found for Etf symbol: {symbol}")
 
     # Unpack json dict to data model
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/utils/helpers.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/utils/index_constituents.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/utils/index_constituents.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """SSI Index Constituents function."""
 
-import requests
+import httpx as requests
 
 from vietfin.providers.ssi.utils.helpers import ssi_headers
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import generate_extra_metadata, check_response_error
 from vietfin.providers.ssi.models.index_constituents import (
     SsiIndexConstituentsData,
 )
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/ssi/utils/index_search.py` & `vietfin-0.2.0/src/vietfin/providers/ssi/utils/index_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """SSI Index Search function."""
 
-import requests
+import httpx as requests
 
 from vietfin.providers.ssi.utils.helpers import ssi_headers
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import generate_extra_metadata, check_response_error
 from vietfin.providers.ssi.models.index_search import SsiIndexSearchData
 from vietfin.utils.errors import EmptyDataError
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_calendar_events.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_calendar_events.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """TCBS Equity Calendar Events Model."""
 
-from bs4 import BeautifulSoup as bs
+from selectolax.parser import HTMLParser
 from pydantic import field_validator
 
 from vietfin.abstract.data import Data
 from vietfin.utils.helpers import ValidatedDatetime
 
 
 class TcbsEquityCalendarEventsData(Data):
@@ -36,10 +36,12 @@
     date_ex_right: ValidatedDatetime | None  # Ex-right date of the event.
     symbol: str  # Symbol representing the entity requested in the data.
 
     @field_validator("event_desc")
     @classmethod
     def parse_html(cls, v: str) -> str:
         """Parse HTML to text."""
-        soup = bs(v, "html.parser")
-        v = soup.get_text(separator="\n", strip=True)
-        return v
+        tree = HTMLParser(v)
+        if tree.body is None:
+            return "No event description available."
+        v = tree.body.text(separator="\n", strip=True)
+        return v
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_fundamental_dividends.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_fundamental_dividends.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_fundamental_income.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_fundamental_income.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_fundamental_management.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_fundamental_management.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_fundamental_ratios.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_fundamental_ratios.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_ownership_insider_trading.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_ownership_insider_trading.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_price_historical.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_price_historical.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_price_quote.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_price_quote.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/models/equity_profile.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/models/equity_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """TCBS Equity Profile Model."""
 
 from pydantic import AnyHttpUrl, field_validator
-from bs4 import BeautifulSoup as bs
+from selectolax.parser import HTMLParser
 
 from vietfin.abstract.data import Data
 
 
 class TcbsEquityProfileData(Data):
     """TCBS Equity Profile Data."""
 
@@ -29,10 +29,12 @@
     employees: int | None = None  # Number of employees working for the company.
     industry: str | None = None  # Category of industry in which the company operates.
     
     @field_validator("long_description")
     @classmethod
     def parse_html(cls, v: str) -> str:
         """Parse HTML to text."""
-        soup = bs(v, "html.parser")
-        v = soup.get_text(separator="\n", strip=True)
+        tree = HTMLParser(v)
+        if tree.body is None:
+            return "No event description available."
+        v = tree.body.text(separator="\n", strip=True)
         return v
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/models/news_company.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/models/news_company.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/provider.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,21 +76,21 @@
         """Equity Insider Trading. Load insider trading data of a specific ticker."""
         return insider_trading(symbol=symbol, limit=limit)
 
     def major_holders(self, symbol: str) -> VfObject:
         """Equity Major Holders. Load major holders data of a specific ticker."""
         return major_holders(symbol=symbol)
 
-    def foreign_trading(self, symbol: str) -> VfObject:
+    def foreign_trading(self, symbol: str, start_date: str, end_date: str) -> VfObject:
         """Equity Ownership Foreign Trading. Load the trading data of foreign entities for a specific ticker."""
         raise NotImplementedError(
             "equity.ownership.foreign_trading() command is not implemented for Tcbs provider."
         )
     
-    def prop_trading(self, symbol: str) -> VfObject:
+    def prop_trading(self, symbol: str, start_date: str, end_date: str) -> VfObject:
         """Equity Ownership Proprietary trading. Load the trading data of proprietary trading firms for a specific ticker."""
         raise NotImplementedError(
             "equity.ownership.prop_trading() command is not implemented for Tcbs provider."
         )
 
 
 class EquityCalendarTcbs(IEquityCalendar):
@@ -153,17 +153,23 @@
             end_date=end_date,
             interval="1d",
             api_endpoint="futures",
             query_param="derivative",
         )
 
     def quote(self, symbol: str, limit: int, cookie: str) -> VfObject:
-        """Equity Quote. Load quote data of a specific ticker."""
+        """Derivatives Futures Quote. Load quote data of a specific contract symbol."""
         raise NotImplementedError(
-            "equity.price.quote() command is not implemented for Tcbs provider."
+            "derivatives.futures.quote() command is not implemented for Tcbs provider."
+        )
+    
+    def search(self, symbol: str) -> VfObject:
+        """Derivatives Futures Search. Search for a specific futures contract."""
+        raise NotImplementedError(
+            "derivatives.futures.search() command is not implemented for Tcbs provider."
         )
 
 
 class EtfTcbs(IEtf):
     """The concrete implementation of ETF component with Tcbs as provider."""
 
     def historical(
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_calendar_events.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_calendar_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """TCBS Equity Calendar dividend() command."""
 
-import requests
+import httpx as requests
 
 from vietfin.providers.tcbs.utils.helpers import tcbs_headers
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
     generate_extra_metadata,
     check_response_error,
     BaseOtherParams,
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_fundamental_dividends.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_fundamental_dividends.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """TCBS Equity Fundamental Dividends command."""
 
-import requests
+import httpx as requests
 
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
     check_response_error,
     generate_extra_metadata,
     BaseOtherParams,
 )
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_fundamental_income.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_fundamental_income.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """TCBS Equity Fundamental Income command."""
 
-import requests
+import httpx as requests
 import pandas as pd
 
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
     check_response_error,
     generate_extra_metadata,
     FINANCIAL_STATEMENTS,
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_fundamental_management.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_fundamental_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """TCBS Equity Fundamental Management command."""
 
-import requests
+import httpx as requests
 
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
     check_response_error,
     generate_extra_metadata,
     BaseOtherParams,
 )
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_fundamental_ratios.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_fundamental_ratios.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """TCBS Equity Fundamental Ratios command."""
 
-import requests
+import httpx as requests
 
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
     check_response_error,
     generate_extra_metadata,
     BaseOtherParams,
     PERIODS,
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_ownership_insider_trading.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_ownership_insider_trading.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """TCBS Equity Ownership insider_trading() command."""
 
-import requests
+import httpx as requests
 
 from vietfin.providers.tcbs.utils.helpers import tcbs_headers
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
     generate_extra_metadata,
     check_response_error,
     BaseOtherParams,
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_ownership_major_holders.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_ownership_major_holders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """TCBS Equity Ownership major_holders() command."""
 
-import requests
+import httpx as requests
 
 from vietfin.providers.tcbs.utils.helpers import tcbs_headers
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
     generate_extra_metadata,
     check_response_error,
     BaseOtherParams,
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_price_historical.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_price_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """TCBS Equity Price Historical command."""
 
 from datetime import timedelta, datetime
 from typing import Literal
 
-import requests
+import httpx as requests
 from pydantic import field_validator
 
 from vietfin.providers.tcbs.utils.helpers import tcbs_headers
 from vietfin.providers.tcbs.models.equity_price_historical import (
     TcbsEquityHistoricalPriceData,
 )
 from vietfin.abstract.vfobject import VfObject
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_price_quote.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_price_quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """TCBS Equity Price Quote command."""
 
-import requests
+import httpx as requests
 
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
     check_response_error,
     generate_extra_metadata,
     BaseOtherParams,
 )
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/utils/equity_profile.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/utils/equity_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """TCBS Equity Profile command."""
 
-import requests
+import httpx as requests
 
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
     check_response_error,
     generate_extra_metadata,
     BaseOtherParams,
 )
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/tcbs/utils/news_company.py` & `vietfin-0.2.0/src/vietfin/providers/tcbs/utils/news_company.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """TCBS News Company command."""
 
-import requests
+import httpx as requests
 
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
     check_response_error,
     generate_extra_metadata,
     BaseOtherParams,
 )
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/vdsc/models/derivatives_futures_quote.py` & `vietfin-0.2.0/src/vietfin/providers/vdsc/models/derivatives_futures_quote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""VDSC Rong Viet Derivatives Futures Historical Price Model."""
+"""VDSC Rong Viet Derivatives Futures Quote Model."""
 
 from datetime import time
 
 from vietfin.abstract.data import Data
 
 
 class VdscDerivativesFuturesQuoteData(Data):
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/vdsc/provider.py` & `vietfin-0.2.0/src/vietfin/providers/vdsc/provider.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """Vdsc Rong Viet provider concrete class."""
 
 from vietfin.abstract.interface import IDerivativesFutures
 from vietfin.abstract.vfobject import VfObject
-from vietfin.providers.vdsc.utils.derivatives_futures_quote import quote as derivatives_futures_quote
+# from vietfin.providers.vdsc.utils.derivatives_futures_quote import quote
     
 
 class DerivativesFuturesVdsc(IDerivativesFutures):
     """The concrete implementation of Derivatives.Futures component with Vdsc Rong Viet as provider."""
 
     def historical(self, symbol: str, start_date: str, end_date: str) -> VfObject:
         """Derivatives Futures Historical. Load historical price data for a specific futures contract."""
 
         raise NotImplementedError("derivatives.futures.historical() command is not implemented for Vdsc Rong Viet provider.")
     
-    def quote(self, symbol: str, limit: int, cookie: str) -> VfObject:
+    def quote(self, symbol: str, limit: int) -> VfObject:
         """Derivatives Futures Quote. Load quote data for a specific futures contract."""
 
-        return derivatives_futures_quote(symbol=symbol, limit=limit, cookie=cookie)
+        raise NotImplementedError("derivatives.futures.quote() command is currently disabled for Vdsc Rong Viet provider.")
+
+    def search(self, symbol: str) -> VfObject:
+        """Derivatives Futures Search. Search for a specific futures contract."""
+
+        raise NotImplementedError("derivatives.futures.search() command is not implemented for Vdsc Rong Viet provider.")
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/vdsc/utils/derivatives_futures_quote.py` & `vietfin-0.2.0/src/vietfin/providers/vdsc/utils/derivatives_futures_quote.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,58 @@
-"""VDSC Rong Viet Derivatives Futures Historical Price command."""
+"""VDSC Rong Viet Derivatives Futures Quote command."""
 
 from datetime import datetime
 
-import requests
+import httpx as requests
 
 from vietfin.providers.vdsc.utils.helpers import rv_headers
 from vietfin.providers.vdsc.models.derivatives_futures_quote import (
     VdscDerivativesFuturesQuoteData,
 )
 from vietfin.abstract.vfobject import VfObject
 from vietfin.utils.helpers import (
     generate_extra_metadata,
     check_response_error,
     BaseOtherParams,
 )
 from vietfin.utils.errors import EmptyDataError
 
 
-class HistoricalParams(BaseOtherParams):
-    """Class to validate input of historical() function."""
+def get_cookies_selenium():
+    """Retrieve cookies from VDSC Rong Viet website using Selenium."""
+    try:
+        from selenium import webdriver  # type: ignore # pylint: disable=import-outside-toplevel
+    except ImportError as exc:
+        raise ImportError(
+            "Please install selenium to use this function. e.g. `poetry add selenium`."
+        ) from exc
+
+    driver = webdriver.Chrome()
+    driver.get("https://livedragon.vdsc.com.vn/general/intradayBoard.rv")
+    cookies = driver.get_cookies()
+    requests_cookies = {}
+    for c in cookies:
+        requests_cookies[c["name"]] = c["value"]
 
-    cookie: str
+    return requests_cookies
 
 
-def quote(symbol: str, limit: int, cookie: str) -> VfObject:
-    """Retrieve Derivatives Futures Historical price of a specific contract symbol.
+def quote(symbol: str, limit: int) -> VfObject:
+    """Retrieve Derivatives Futures intraday quote data of a specific contract symbol.
 
     Data from VDSC Rong Viet https://livedragon.vdsc.com.vn/
     As of 2024-02-08, this API is not stable, long runtime and requires cookies.
 
     Parameters
     ----------
     symbol : str
         Futures contract symbol
     limit : int
         limit of number of records to be retrieved.
         0 will return all records.
-    cookie: str
-        cookie string required for the request headers.
 
     Returns
     -------
     VfObject
         results : list[VdscEquityHistoricalPriceData]
             derivatives futures historical price data of the given contract symbol on current date
         provider : str
@@ -58,62 +69,57 @@
     HttpError
         if the API call failed
     EmptyDataError
         if the API response is empty
     """
 
     # Validate input param
-    params = HistoricalParams(symbol=symbol, limit=limit, cookie=cookie)
+    params = BaseOtherParams(symbol=symbol, limit=limit)
     symbol = params.symbol
     limit = params.limit
-    cookie = params.cookie
 
     current_date = datetime.now()
     current_date_string_api = current_date.strftime("%d/%m/%Y")
     current_date_string_iso = current_date.strftime("%Y-%m-%d")
 
-    # Update headers with the user-provided cookies
-    headers = rv_headers.copy()
-    headers["Cookie"] = cookie
-
     # API call
+    requests_cookies = get_cookies_selenium()
+
     payload = {"stockCode": symbol, "boardDate": current_date_string_api}
     url = "https://livedragon.vdsc.com.vn/general/intradaySearch.rv"
-    response = requests.post(url, headers=headers, data=payload)
-
+    response = requests.post(
+        url, headers=rv_headers, data=payload, cookies=requests_cookies
+    )
     check_response_error(response)
 
     data = response.json()
     rows = data.get("list", [])
 
     if not rows:
         raise EmptyDataError(
             f"No data found for the given symbol {symbol} on {current_date_string_iso}"
         )
 
     # Return only the number of records specified by `limit`
     if limit == 0:
         limit = len(rows)  # return all available data points
     limited_rows = rows[:limit]
-    print(
-        f"Retrieved {limit} intraday quotes for futures contract {symbol} traded on {current_date_string_iso}"
-    )
 
     # Unpack json data into data model
     derivatives_futures_quote: list[VdscDerivativesFuturesQuoteData] = [
         VdscDerivativesFuturesQuoteData(**r) for r in limited_rows
     ]
 
     # Generate extra metadata
     extra = generate_extra_metadata(
         symbol=symbol, result=derivatives_futures_quote, api_url=url
     )
 
     print(
-        f"Retrieved {extra.get('records_count',[])} intraday quotes for futures contract {symbol}."
+        f"Retrieved {extra.get('records_count',[])} intraday quotes for futures contract {symbol} traded on {current_date_string_iso}."
     )
 
     return VfObject(
         results=derivatives_futures_quote,
         provider="vdsc",
         extra=extra,
         raw_data=data,
```

### Comparing `vietfin-0.1.0/src/vietfin/providers/vdsc/utils/helpers.py` & `vietfin-0.2.0/src/vietfin/providers/vdsc/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/wifeed/provider.py` & `vietfin-0.2.0/src/vietfin/providers/wifeed/provider.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/providers/wifeed/utils/equity_search.py` & `vietfin-0.2.0/src/vietfin/providers/wifeed/utils/equity_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """WiFeed Equity Search function."""
 
-import requests
+import httpx as requests
 
 from vietfin.abstract.vfobject import VfObject
 from vietfin.providers.wifeed.models.equity_search import WifeedEquitySearchData
 from vietfin.utils.helpers import (
     generate_extra_metadata,
     check_response_error,
     BaseOtherParams,
```

### Comparing `vietfin-0.1.0/src/vietfin/utils/errors.py` & `vietfin-0.2.0/src/vietfin/utils/errors.py`

 * *Files identical despite different names*

### Comparing `vietfin-0.1.0/src/vietfin/utils/helpers.py` & `vietfin-0.2.0/src/vietfin/utils/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,27 @@
 import re
 import ast
 from datetime import datetime, timezone, timedelta
 
 import pandas as pd
 from pydantic.functional_validators import AfterValidator
 from pydantic import BaseModel, field_validator, model_validator
-import requests
+import httpx as requests
 
 from vietfin.abstract.data import Data
 
+# Constants
+
+INTERVALS = Literal["1m", "15m", "30m", "1h", "1d"]
+FINANCIAL_STATEMENTS = Literal["income", "balance", "cash"]
+PERIODS = Literal["annual", "quarter"]
+TOP_MOVERS_REPORT_NAMES = Literal["gainers", "losers", "value"]
+EXCHANGE_NAMES = Literal["hose", "hnx", "upcom", "all"]
+
+# Helper functions
 
 def to_snake_case(string: str) -> str:
     """Convert a string to snake case."""
     s1 = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", string)
     return (
         re.sub("([a-z0-9])([A-Z])", r"\1_\2", s1)
         .lower()
@@ -128,20 +137,20 @@
     Parameters
     ----------
     response : requests.Response
         The HTTP response to check.
 
     Raises
     ------
-    requests.exceptions.HTTPError
+    requests.HTTPError
         If the response status code indicates an error.
     """
 
     if response.status_code != 200:
-        raise requests.exceptions.HTTPError(
+        raise requests.HTTPError(
             f"Error in API response: {response.status_code} - {response.text}"
         )
 
 
 def convert_dictlists_to_listdicts(data: dict) -> list:
     """Transpose a dictionary of lists into a list of dictionaries.
 
@@ -251,35 +260,34 @@
                     f"The end_date {self.end_date} is invalid. Set to today {current_date}."
                 )
                 self.end_date = current_date.strftime("%Y-%m-%d")
 
         return self
 
 
-INTERVALS = Literal["1m", "15m", "30m", "1h", "1d"]
-FINANCIAL_STATEMENTS = Literal["income", "balance", "cash"]
-PERIODS = Literal["annual", "quarter"]
-
-
 class BaseOtherParams(BaseModel):
     """Base class to validate other params (not start_date end_date) in function.
 
     Base validation rules:
-    - symbol must be a string
-    - limit must be an integer. Set to default as 100, if not provided
+    - symbol must be a string. Set to default as "" an empty string, if not provided
+    - limit must be an integer. Set to default as 100
     - interval must be in Literal. Set to default as "1d"
     - financial_statement must be in Literal. Set to default as "income"
     - period must be in Literal. Set to default as "annual"
+    - top_movers_report must be in Literal. Set to default as "value"
+    - exchange must be in Literal. Set to default as "hose"
     """
 
-    symbol: str
+    symbol: str = ""
     limit: int = 100
     interval: INTERVALS = "1d"
     financial_statement: FINANCIAL_STATEMENTS = "income"
     period: PERIODS = "annual"
+    top_movers_report: TOP_MOVERS_REPORT_NAMES = "value"
+    exchange: EXCHANGE_NAMES = "hose"
 
     @field_validator("symbol")
     @classmethod
     def upper_str(cls, v: str) -> str:
         """Convert a string to uppercase."""
 
         if isinstance(v, str):
```

### Comparing `vietfin-0.1.0/PKG-INFO` & `vietfin-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vietfin
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package to fetch Vietnam stock market data
 Home-page: https://github.com/vietfin/vietfin
 License: Apache-2.0
 Keywords: vietnam,stock,market,data,finance,etf,investment,funds
 Author: Huy
 Author-email: vietfin.numbness179@simplelogin.fr
 Requires-Python: >=3.10,<4.0
@@ -16,34 +16,35 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: bs4 (>=0.0.2,<0.0.3)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: selectolax (>=0.3.21,<0.4.0)
 Project-URL: Documentation, https://github.com/vietfin/vietfin
 Project-URL: Repository, https://github.com/vietfin/vietfin
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img src="/docs/_static/logo.jpg" alt="VietFin" width="228" />
+  <img src="https://github.com/vietfin/vietfin/blob/main/docs/_static/logo.jpg" alt="VietFin" width="228" />
 </p>
 
 <h2 align="center">VietFin</h2>
 
 <div align="center">A python library to fetch Vietnam stock market data.</div>
 
 <p align="center">
-    <a href="https://github.com/vietfin/vietfin/blob/main/LICENSE"><img src="https://img.shields.io/github/license/vietfin/vietfin?style=for-the-badge" alt="License"></a>
+    <a href="https://github.com/vietfin/vietfin/blob/main/LICENSE"><img src="https://img.shields.io/github/license/vietfin/vietfin?style=for-the-badge" alt="License" /></a>
     <a href='https://vietfin.readthedocs.io/en/latest/?badge=latest'><img src='https://readthedocs.org/projects/vietfin/badge/?version=latest&style=for-the-badge' alt='Documentation Status' /></a>
+    <a href='https://pypi.org/project/vietfin/'><img src='https://img.shields.io/pypi/v/vietfin?style=for-the-badge' alt='PyPI - Version' /></a>
     <br />
     <a href="http://vietfin.readthedocs.io/" target="_blank" rel="noopener noreferrer"><strong>» Explore the docs »</strong></a>
     <br />
 </p>
 
 <hr />
 
@@ -67,40 +68,42 @@
 
 This package aims to reproduce the hierarchical structure of commands used in OpenBB, but for Vietnamese market data.
 
 VietFin is intended for personal use, research and educational purposes.
 
 ## 2. Installation
 
-VietFin is available on [PyPI](https://pypi.org/). To use the package:
+VietFin is available on [PyPI](https://pypi.org/project/vietfin/). To use the package:
 
 1. Install VietFin in your project's virtual environment.
 
     ``` {.sourceCode .bash}
     $ pip install vietfin
     ```
 
-    Or using [Poetry](https://python-poetry.org/) as my preferred dependency manager:
+    Or using [Poetry](https://python-poetry.org/), my preferred dependency manager:
 
     ``` {.sourceCode .bash}
     $ poetry add vietfin
     ```
 
 2. Import the package then use the package
 
     ``` {.sourceCode .python}
     from vietfin import vf
     ```
 
 Requirements:
 
 - [Python](https://www.python.org) \>= 3.10
-- [requests](https://requests.readthedocs.io/en/latest/) \>= 2.31
 - [pandas](https://pandas.pydata.org/) \>= 2.1.4
 - [Pydantic](https://github.com/pydantic/pydantic) \>= 2.5
+- [httpx](https://www.python-httpx.org/) \>= 0.27
+- [selectolax](https://github.com/rushter/selectolax) \>= 0.3
+- [openpyxl](https://pypi.org/project/openpyxl/) \>= 3.1.2
 
 ## 3. Usage
 
 ```python
 from vietfin import vf
 # Get list of all stocks
 vf.equity.search()
@@ -130,14 +133,17 @@
 vf.funds.search()
 
 # Get the list of available ETFs
 vf.etf.search()
 
 # Get the list of constituents of an index
 vf.index.constituents(symbol='vn30')
+
+# Get the list of available futures contract
+vf.derivatives.futures.search()
 ```
 
 ## 4. Contributing
 
 More information on our [Contributing Guidelines](/CONTRIBUTING.md) and [Code of Conduct](/CONDUCT.md).
 
 `VietFin` relies on community to investigate bugs and contribute code.
@@ -150,16 +156,16 @@
 
 Feel free to reach out to us in [our GitHub Discussions](https://github.com/vietfin/vietfin/discussions) for other feedbacks (e.g. Q&A, ideas, etc.).
 
 ## 5. Attributions
 
 VietFin is built on top of the inspiration and work of the following projects:
 
-- [Openbb](https://github.com/OpenBB-finance/OpenBBTerminal), its [Data Standardization Infrastructure](https://docs.openbb.co/platform/development/developer-guidelines/architectural_considerations), the hierarchical structure of user-facing commands, and the documentation style of [OpenBB Platform's API reference](https://docs.openbb.co/platform/reference).
-- [vnstock](https://github.com/thinh-vu/vnstock) and its findinds on publicly available APIs from brokerage firms in Vietnam.
+- [OpenBB](https://github.com/OpenBB-finance/OpenBBTerminal), its [Data Standardization Infrastructure](https://docs.openbb.co/platform/development/developer-guidelines/architectural_considerations), the hierarchical structure of user-facing commands, and the documentation style of [OpenBB Platform's API reference](https://docs.openbb.co/platform/reference).
+- [vnstock](https://github.com/thinh-vu/vnstock) and its findinds on publicly available APIs from many brokerage firms in Vietnam.
 
 ## 6. Disclaimer
 
 VietFin is not affiliated, endorsed, or vetted by any of the brokerage firms or research entities which provide the data. It's an open-source tool which fetches data from the publicly available APIs of these firms. VietFin is intended for personal use, research and educational purposes.
 
 You should refer to each of the data provider's terms of use for details on your rights to use the actual data downloaded.
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: vietfin Version: 0.1.0 Summary: Python package to
+Metadata-Version: 2.1 Name: vietfin Version: 0.2.0 Summary: Python package to
 fetch Vietnam stock market data Home-page: https://github.com/vietfin/vietfin
 License: Apache-2.0 Keywords:
 vietnam,stock,market,data,finance,etf,investment,funds Author: Huy Author-
 email: vietfin.numbness179@simplelogin.fr Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Topic :: Office/Business :: Financial ::
 Investment Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
-Requires-Dist: bs4 (>=0.0.2,<0.0.3) Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
-Requires-Dist: pandas (>=2.1.4,<3.0.0) Requires-Dist: pydantic (>=2.5.3,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0) Project-URL: Documentation, https://
-github.com/vietfin/vietfin Project-URL: Repository, https://github.com/vietfin/
-vietfin Description-Content-Type: text/markdown
+Requires-Dist: httpx (>=0.27.0,<0.28.0) Requires-Dist: openpyxl
+(>=3.1.2,<4.0.0) Requires-Dist: pandas (>=2.1.4,<3.0.0) Requires-Dist: pydantic
+(>=2.5.3,<3.0.0) Requires-Dist: selectolax (>=0.3.21,<0.4.0) Project-URL:
+Documentation, https://github.com/vietfin/vietfin Project-URL: Repository,
+https://github.com/vietfin/vietfin Description-Content-Type: text/markdown
                                    [VietFin]
                               ********** VViieettFFiinn **********
              A python library to fetch Vietnam stock market data.
-                        _[_L_i_c_e_n_s_e_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]
+                _[_L_i_c_e_n_s_e_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]
                             _?Â_?»_ _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 ===============================================================================
 ********** TTaabbllee ooff CCoonntteennttss **********
    1. _W_h_y_ _V_i_e_t_F_i_n_?
    2. _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
    4. _C_o_n_t_r_i_b_u_t_i_n_g
@@ -32,60 +32,63 @@
    7. _C_o_n_t_a_c_t_s
 ## 1. Why VietFin? Heavily inspired by [OpenBB](https://github.com/OpenBB-
 finance/OpenBBTerminal), VietFin is a Python package which provides a wrapper
 around the publicly available APIs from multiple brokerage firms. This package
 aims to reproduce the hierarchical structure of commands used in OpenBB, but
 for Vietnamese market data. VietFin is intended for personal use, research and
 educational purposes. ## 2. Installation VietFin is available on [PyPI](https:/
-/pypi.org/). To use the package: 1. Install VietFin in your project's virtual
-environment. ``` {.sourceCode .bash} $ pip install vietfin ``` Or using
-[Poetry](https://python-poetry.org/) as my preferred dependency manager: ```
-{.sourceCode .bash} $ poetry add vietfin ``` 2. Import the package then use the
-package ``` {.sourceCode .python} from vietfin import vf ``` Requirements: -
-[Python](https://www.python.org) \>= 3.10 - [requests](https://
-requests.readthedocs.io/en/latest/) \>= 2.31 - [pandas](https://
+/pypi.org/project/vietfin/). To use the package: 1. Install VietFin in your
+project's virtual environment. ``` {.sourceCode .bash} $ pip install vietfin
+``` Or using [Poetry](https://python-poetry.org/), my preferred dependency
+manager: ``` {.sourceCode .bash} $ poetry add vietfin ``` 2. Import the package
+then use the package ``` {.sourceCode .python} from vietfin import vf ```
+Requirements: - [Python](https://www.python.org) \>= 3.10 - [pandas](https://
 pandas.pydata.org/) \>= 2.1.4 - [Pydantic](https://github.com/pydantic/
-pydantic) \>= 2.5 ## 3. Usage ```python from vietfin import vf # Get list of
-all stocks vf.equity.search() # Get general info of a stock vf.equity.profile
-(symbol='vnm') # Get historical price of a stock vf.equity.historical
-(symbol='vnm') # Get the historical dividends data of a company
-vf.equity.fundamental.dividends(symbol='vnm') # Get list of key executives of a
-company vf.equity.fundamental.management(symbol='vnm') # Get the key financial
-ratios of a company vf.equity.fundamental.ratios(symbol='vnm') # Get the report
-on the income statement of a company vf.equity.fundamental.income(symbol='vnm')
-# Get the historical events of a stock ticker vf.equity.calendar.events
-(symbol='vnm') # Get the list of available mutual funds vf.funds.search() # Get
-the list of available ETFs vf.etf.search() # Get the list of constituents of an
-index vf.index.constituents(symbol='vn30') ``` ## 4. Contributing More
+pydantic) \>= 2.5 - [httpx](https://www.python-httpx.org/) \>= 0.27 -
+[selectolax](https://github.com/rushter/selectolax) \>= 0.3 - [openpyxl](https:
+//pypi.org/project/openpyxl/) \>= 3.1.2 ## 3. Usage ```python from vietfin
+import vf # Get list of all stocks vf.equity.search() # Get general info of a
+stock vf.equity.profile(symbol='vnm') # Get historical price of a stock
+vf.equity.historical(symbol='vnm') # Get the historical dividends data of a
+company vf.equity.fundamental.dividends(symbol='vnm') # Get list of key
+executives of a company vf.equity.fundamental.management(symbol='vnm') # Get
+the key financial ratios of a company vf.equity.fundamental.ratios
+(symbol='vnm') # Get the report on the income statement of a company
+vf.equity.fundamental.income(symbol='vnm') # Get the historical events of a
+stock ticker vf.equity.calendar.events(symbol='vnm') # Get the list of
+available mutual funds vf.funds.search() # Get the list of available ETFs
+vf.etf.search() # Get the list of constituents of an index
+vf.index.constituents(symbol='vn30') # Get the list of available futures
+contract vf.derivatives.futures.search() ``` ## 4. Contributing More
 information on our [Contributing Guidelines](/CONTRIBUTING.md) and [Code of
 Conduct](/CONDUCT.md). `VietFin` relies on community to investigate bugs and
 contribute code. Before creating a ticket, please check our [Issues tracker]
 (https://github.com/vietfin/vietfin/issues) to avoid duplicates. - [Report bug]
 (https://github.com/vietfin/vietfin/issues/
 new?assignees=&labels=type%3Abug&projects=&template=bug_report.md&title=%5BBug%5D)
 - [Suggest improvement](https://github.com/vietfin/vietfin/issues/
 new?assignees=&labels=type%3Aenhancement&projects=&template=enhancement.md&title=%5BIMPROVE%5D)
 - [Request a feature](https://github.com/vietfin/vietfin/issues/
 new?assignees=&labels=type%3Afeature&projects=&template=feature_request.md&title=%5BFR%5D)
 Feel free to reach out to us in [our GitHub Discussions](https://github.com/
 vietfin/vietfin/discussions) for other feedbacks (e.g. Q&A, ideas, etc.). ## 5.
 Attributions VietFin is built on top of the inspiration and work of the
-following projects: - [Openbb](https://github.com/OpenBB-finance/
+following projects: - [OpenBB](https://github.com/OpenBB-finance/
 OpenBBTerminal), its [Data Standardization Infrastructure](https://
 docs.openbb.co/platform/development/developer-guidelines/
 architectural_considerations), the hierarchical structure of user-facing
 commands, and the documentation style of [OpenBB Platform's API reference]
 (https://docs.openbb.co/platform/reference). - [vnstock](https://github.com/
-thinh-vu/vnstock) and its findinds on publicly available APIs from brokerage
-firms in Vietnam. ## 6. Disclaimer VietFin is not affiliated, endorsed, or
-vetted by any of the brokerage firms or research entities which provide the
-data. It's an open-source tool which fetches data from the publicly available
-APIs of these firms. VietFin is intended for personal use, research and
-educational purposes. You should refer to each of the data provider's terms of
-use for details on your rights to use the actual data downloaded. The data
+thinh-vu/vnstock) and its findinds on publicly available APIs from many
+brokerage firms in Vietnam. ## 6. Disclaimer VietFin is not affiliated,
+endorsed, or vetted by any of the brokerage firms or research entities which
+provide the data. It's an open-source tool which fetches data from the publicly
+available APIs of these firms. VietFin is intended for personal use, research
+and educational purposes. You should refer to each of the data provider's terms
+of use for details on your rights to use the actual data downloaded. The data
 retrieved by the VietFin package is not necessarily accurate. VietFin and any
 provider of the data contained in this website will not accept liability for
 any loss or damage as a result of your trading, or your reliance on the
 information displayed. ## 7. Contacts If you have any questions about `VietFin`
 or just to say hi, feel free to [open a new public discussion in our GitHub
 repo](https://github.com/vietfin/vietfin/discussions/new/choose), or send an
 email to `vietfin.numbness179(at)simplelogin.fr`.
```


# Comparing `tmp/bookio_fetchfox-2.4.2.tar.gz` & `tmp/bookio_fetchfox-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-2.4.2.tar", max compression
+gzip compressed data, was "bookio_fetchfox-2.4.3.tar", max compression
```

## Comparing `bookio_fetchfox-2.4.2.tar` & `bookio_fetchfox-2.4.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     3734 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/README.md
--rw-r--r--   0        0        0        0 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2510 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      609 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1427 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     2156 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      605 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0      259 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/cardano/cexplorerio.py
--rw-r--r--   0        0        0      891 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1908 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/cardano/dexhunterio.py
--rw-r--r--   0        0        0     6920 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/cardano/gomaestroorg.py
--rw-r--r--   0        0        0     1798 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/cardano/jpgstore.py
--rw-r--r--   0        0        0      536 2024-04-21 22:02:05.271620 bookio_fetchfox-2.4.2/fetchfox/apis/cardano/muesliswap.py
--rwxr-xr-x   0        0        0     1572 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      988 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     5658 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     3037 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      228 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/apis/pinatacloud.py
--rw-r--r--   0        0        0      228 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/apis/price.py
--rw-r--r--   0        0        0      120 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0    10494 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      689 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/algorand/exceptions.py
--rw-r--r--   0        0        0      502 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     3408 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    17318 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0      679 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/cardano/exceptions.py
--rw-r--r--   0        0        0     1060 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0     1696 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0    11892 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      753 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/evm/exceptions.py
--rw-r--r--   0        0        0      617 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0      443 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/exceptions.py
--rw-r--r--   0        0        0       32 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0     1706 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      146 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      299 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/constants/beard.py
--rw-r--r--   0        0        0      158 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      399 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/constants/book.py
--rw-r--r--   0        0        0       82 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/constants/cardano.py
--rw-r--r--   0        0        0      163 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0       66 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/constants/evm.py
--rw-r--r--   0        0        0      341 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0   453386 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/constants/ranks.py
--rw-r--r--   0        0        0       95 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       62 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      329 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     3619 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     3666 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      285 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/dtos/floor.py
--rw-r--r--   0        0        0      495 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1572 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      948 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/dtos/order.py
--rw-r--r--   0        0        0     1203 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/dtos/pair_stats.py
--rw-r--r--   0        0        0      365 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     2023 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0        0 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/pools/__init__.py
--rw-r--r--   0        0        0     1135 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/pools/book_pool.py
--rw-r--r--   0        0        0     5794 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/rest.py
--rw-r--r--   0        0        0      106 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/tokens/__init__.py
--rw-r--r--   0        0        0     4155 2024-04-21 22:02:05.275620 bookio_fetchfox-2.4.2/fetchfox/tokens/base.py
--rw-r--r--   0        0        0      647 2024-04-21 22:02:05.279620 bookio_fetchfox-2.4.2/fetchfox/tokens/beard_token.py
--rw-r--r--   0        0        0      714 2024-04-21 22:02:05.279620 bookio_fetchfox-2.4.2/fetchfox/tokens/book_token.py
--rw-r--r--   0        0        0      671 2024-04-21 22:02:05.279620 bookio_fetchfox-2.4.2/fetchfox/tokens/hosky_token.py
--rw-r--r--   0        0        0     1148 2024-04-21 22:02:05.287620 bookio_fetchfox-2.4.2/pyproject.toml
--rw-r--r--   0        0        0     5036 1970-01-01 00:00:00.000000 bookio_fetchfox-2.4.2/setup.py
--rw-r--r--   0        0        0     4949 1970-01-01 00:00:00.000000 bookio_fetchfox-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     3734 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2510 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      609 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1427 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     2156 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      605 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      262 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/cardano/cexplorerio.py
+-rw-r--r--   0        0        0      891 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/cardano/cnfttools.py
+-rw-r--r--   0        0        0     1908 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/cardano/dexhunterio.py
+-rw-r--r--   0        0        0     6920 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/cardano/gomaestroorg.py
+-rw-r--r--   0        0        0     1798 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/cardano/jpgstore.py
+-rw-r--r--   0        0        0      536 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/cardano/muesliswap.py
+-rwxr-xr-x   0        0        0     1572 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0      988 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     5658 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     3037 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      228 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/pinatacloud.py
+-rw-r--r--   0        0        0      228 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/apis/price.py
+-rw-r--r--   0        0        0      120 2024-04-22 04:20:16.815003 bookio_fetchfox-2.4.3/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0    10494 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      689 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/algorand/exceptions.py
+-rw-r--r--   0        0        0      502 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     3408 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    17407 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0      679 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/cardano/exceptions.py
+-rw-r--r--   0        0        0     1060 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0     1696 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0    11892 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      753 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/evm/exceptions.py
+-rw-r--r--   0        0        0      617 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0      443 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/exceptions.py
+-rw-r--r--   0        0        0       32 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0     1706 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      146 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      299 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/constants/beard.py
+-rw-r--r--   0        0        0      158 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      399 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/constants/book.py
+-rw-r--r--   0        0        0       82 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/constants/cardano.py
+-rw-r--r--   0        0        0      163 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0       66 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/constants/evm.py
+-rw-r--r--   0        0        0      341 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0   453386 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/constants/ranks.py
+-rw-r--r--   0        0        0       95 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       62 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      329 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     3619 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     3666 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      285 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/dtos/floor.py
+-rw-r--r--   0        0        0      495 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1572 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      948 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/dtos/order.py
+-rw-r--r--   0        0        0     1203 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/dtos/pair_stats.py
+-rw-r--r--   0        0        0      365 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     2023 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0        0 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/pools/__init__.py
+-rw-r--r--   0        0        0     1135 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/pools/book_pool.py
+-rw-r--r--   0        0        0     5794 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/rest.py
+-rw-r--r--   0        0        0      106 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/tokens/__init__.py
+-rw-r--r--   0        0        0     4155 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/tokens/base.py
+-rw-r--r--   0        0        0      647 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/tokens/beard_token.py
+-rw-r--r--   0        0        0      714 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/tokens/book_token.py
+-rw-r--r--   0        0        0      671 2024-04-22 04:20:16.819003 bookio_fetchfox-2.4.3/fetchfox/tokens/hosky_token.py
+-rw-r--r--   0        0        0     1148 2024-04-22 04:20:16.831003 bookio_fetchfox-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0     5036 1970-01-01 00:00:00.000000 bookio_fetchfox-2.4.3/setup.py
+-rw-r--r--   0        0        0     4949 1970-01-01 00:00:00.000000 bookio_fetchfox-2.4.3/PKG-INFO
```

### Comparing `bookio_fetchfox-2.4.2/README.md` & `bookio_fetchfox-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/algorand/algonodecloud.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/algorand/nfdomains.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/algorand/randswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/cardano/cnfttools.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/cardano/cnfttools.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/cardano/dexhunterio.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/cardano/dexhunterio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/cardano/gomaestroorg.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/cardano/gomaestroorg.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/cardano/jpgstore.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/cardano/muesliswap.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/cardano/muesliswap.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/coingeckocom.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/coingeckocom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/evm/ensideascom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/evm/moralisio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-2.4.3/fetchfox/apis/evm/openseaio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-2.4.3/fetchfox/blockchains/algorand/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/blockchains/algorand/exceptions.py` & `bookio_fetchfox-2.4.3/fetchfox/blockchains/algorand/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/blockchains/base.py` & `bookio_fetchfox-2.4.3/fetchfox/blockchains/base.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-2.4.3/fetchfox/blockchains/cardano/blockchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,25 +235,29 @@
             asset_id=asset_id,
             rank=CNFT_RANKS[collection_id][asset_name],
         )
 
     # Collections
 
     def get_collection_assets(
-        self, collection_id: str, discriminator: str = None, fetch_metadata: bool = True, *args, **kwargs
+        self, collection_id: str, discriminator: str = None, fetch_metadata: bool = True, *args, **kwargs,
     ) -> Iterable[AssetDTO]:
         self.check_collection_id(collection_id)
 
         collection_assets = gomaestroorg.get_collection_assets(
             collection_id,
             api_key=self.maestro_api_key,
         )
 
         for asset in collection_assets:
             encoded_asset_name = asset["asset_name"]
+
+            if not encoded_asset_name:  # skip royalty token
+                continue
+
             asset_id = f"{collection_id}{encoded_asset_name}"
             cip25_metadata = asset["asset_standards"].get("cip25_metadata")
             cip68_metadata = asset["asset_standards"].get("cip68_metadata")
 
             policy_id, asset_name = utils.split_asset_id(asset_id)
 
             # required for multi-book policies (e.g. monsters, greek classics)
```

### Comparing `bookio_fetchfox-2.4.2/fetchfox/blockchains/cardano/exceptions.py` & `bookio_fetchfox-2.4.3/fetchfox/blockchains/cardano/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-2.4.3/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/blockchains/ethereum/blockchain.py` & `bookio_fetchfox-2.4.3/fetchfox/blockchains/ethereum/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-2.4.3/fetchfox/blockchains/evm/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/blockchains/evm/exceptions.py` & `bookio_fetchfox-2.4.3/fetchfox/blockchains/evm/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-2.4.3/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/blockchains/polygon/blockchain.py` & `bookio_fetchfox-2.4.3/fetchfox/blockchains/polygon/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/constants/ranks.py` & `bookio_fetchfox-2.4.3/fetchfox/constants/ranks.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/dtos/asset.py` & `bookio_fetchfox-2.4.3/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/dtos/campaign.py` & `bookio_fetchfox-2.4.3/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/dtos/listing.py` & `bookio_fetchfox-2.4.3/fetchfox/dtos/listing.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/dtos/order.py` & `bookio_fetchfox-2.4.3/fetchfox/dtos/order.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/dtos/pair_stats.py` & `bookio_fetchfox-2.4.3/fetchfox/dtos/pair_stats.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/dtos/sale.py` & `bookio_fetchfox-2.4.3/fetchfox/dtos/sale.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/pools/book_pool.py` & `bookio_fetchfox-2.4.3/fetchfox/pools/book_pool.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/rest.py` & `bookio_fetchfox-2.4.3/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/tokens/base.py` & `bookio_fetchfox-2.4.3/fetchfox/tokens/base.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/tokens/beard_token.py` & `bookio_fetchfox-2.4.3/fetchfox/tokens/beard_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/tokens/book_token.py` & `bookio_fetchfox-2.4.3/fetchfox/tokens/book_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/fetchfox/tokens/hosky_token.py` & `bookio_fetchfox-2.4.3/fetchfox/tokens/hosky_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.2/pyproject.toml` & `bookio_fetchfox-2.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "2.4.2"
+version = "2.4.3"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
```

### Comparing `bookio_fetchfox-2.4.2/setup.py` & `bookio_fetchfox-2.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'asyncio>=3.4.3,<4.0.0',
  'backoff>=2.2.1,<3.0.0',
  'cachetools>=5.3.1,<6.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '2.4.2',
+    'version': '2.4.3',
     'description': 'Collection of API services to fetch information from several blockchains.',
     'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_collection_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
```

### Comparing `bookio_fetchfox-2.4.2/PKG-INFO` & `bookio_fetchfox-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 2.4.2
+Version: 2.4.3
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
```


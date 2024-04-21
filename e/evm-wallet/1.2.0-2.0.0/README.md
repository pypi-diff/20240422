# Comparing `tmp/evm_wallet-1.2.0.tar.gz` & `tmp/evm_wallet-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evm_wallet-1.2.0.tar", max compression
+gzip compressed data, was "evm_wallet-2.0.0.tar", max compression
```

## Comparing `evm_wallet-1.2.0.tar` & `evm_wallet-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1063 2023-12-12 20:18:06.436480 evm_wallet-1.2.0/LICENSE
--rw-r--r--   0        0        0    10327 2024-01-29 19:31:45.276121 evm_wallet-1.2.0/README.md
--rw-r--r--   0        0        0      786 2023-12-26 19:59:24.213882 evm_wallet-1.2.0/evm_wallet/__init__.py
--rw-r--r--   0        0        0     2572 2023-12-12 20:18:06.436806 evm_wallet-1.2.0/evm_wallet/erc20.abi
--rw-r--r--   0        0        0      345 2023-12-12 20:18:06.436857 evm_wallet-1.2.0/evm_wallet/exceptions.py
--rw-r--r--   0        0        0     4026 2024-01-28 14:44:57.552349 evm_wallet-1.2.0/evm_wallet/globals.py
--rw-r--r--   0        0        0      858 2024-01-29 19:06:44.210527 evm_wallet-1.2.0/evm_wallet/types.py
--rw-r--r--   0        0        0     1086 2024-01-29 19:08:54.944670 evm_wallet-1.2.0/evm_wallet/utils.py
--rw-r--r--   0        0        0    18668 2024-01-29 19:28:32.528175 evm_wallet-1.2.0/evm_wallet/wallet.py
--rw-r--r--   0        0        0     1051 2024-01-29 19:31:45.278453 evm_wallet-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    11290 1970-01-01 00:00:00.000000 evm_wallet-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-12-12 20:18:06.436480 evm_wallet-2.0.0/LICENSE
+-rw-r--r--   0        0        0     9536 2024-04-21 23:05:54.000340 evm_wallet-2.0.0/README.md
+-rw-r--r--   0        0        0      846 2024-04-21 23:00:37.178645 evm_wallet-2.0.0/evm_wallet/__init__.py
+-rw-r--r--   0        0        0    13913 2024-04-21 23:09:11.577523 evm_wallet-2.0.0/evm_wallet/_base_wallet.py
+-rw-r--r--   0        0        0     8383 2024-04-21 22:56:33.722361 evm_wallet-2.0.0/evm_wallet/async_wallet.py
+-rw-r--r--   0        0        0     2572 2023-12-12 20:18:06.436806 evm_wallet-2.0.0/evm_wallet/erc20.abi
+-rw-r--r--   0        0        0      967 2024-04-21 21:23:36.163727 evm_wallet-2.0.0/evm_wallet/types.py
+-rw-r--r--   0        0        0      442 2024-04-21 21:58:55.419926 evm_wallet-2.0.0/evm_wallet/utils.py
+-rw-r--r--   0        0        0     8185 2024-04-21 22:56:33.724023 evm_wallet-2.0.0/evm_wallet/wallet.py
+-rw-r--r--   0        0        0     1073 2024-04-21 22:09:58.947167 evm_wallet-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10496 1970-01-01 00:00:00.000000 evm_wallet-2.0.0/PKG-INFO
```

### Comparing `evm_wallet-1.2.0/LICENSE` & `evm_wallet-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evm_wallet-1.2.0/README.md` & `evm_wallet-2.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # evm-wallet
 
 [![Croco Logo](https://i.ibb.co/G5Pjt6M/logo.png)](https://t.me/crocofactory)
 
-
 The package, containing wrapper over EVM operations for interacting through Wallet entities.
 
 - **[Telegram channel](https://t.me/crocofactory)**
 - **[Overview](#quick-overview)**
 - **[Bug reports](https://github.com/blnkoff/evm-wallet/issues)**
 
 
@@ -18,162 +17,142 @@
 - quick performing useful functions of Web3.py
    
 evm-wallet's source code is made available under the [MIT License](LICENSE)
 
 ##  Quick start
 You can quickly use supported networks as RPC:  
 
-| Network         | Native Token | Testnet  |
-|-----------------|--------------|----------|
-| Arbitrum Goerli | AGOR         | ✅        |
-| Arbitrum        | ETH          | ❌        |
-| Avalanche       | AVAX         | ❌        |
-| Base            | ETH          | ❌        |
-| Base Goerli     | ETH          | ✅        |
-| BSC             | BNB          | ❌        |
-| BSC Testnet     | tBNB         | ✅        |
-| Ethereum        | ETH          | ❌        |
-| Fantom          | FTM          | ❌        |
-| Fantom Testnet  | FTM          | ✅        |
-| Fuji            | AVAX         | ✅        |
-| Goerli          | GETH         | ✅        |
-| Linea           | ETH          | ❌        |
-| Linea Goerli    | ETH          | ✅        |
-| Mumbai          | MATIC        | ✅        |
-| opBNB           | BNB          | ❌        |
-| opBNB Testnet   | BNB          | ✅        |
-| Optimism        | ETH          | ❌        |
-| Optimism Goerli | OGOR         | ✅        |
-| Polygon         | MATIC        | ❌        |
-| Sepolia         | SETH         | ❌        |
-| zkSync          | ETH          | ❌        |
-
-
+| Network          | Native Token | Testnet |
+|------------------|--------------|---------|
+| Arbitrum Goerli  | ETH          | ✅       |
+| Arbitrum Sepolia | ETH          | ✅       |
+| Arbitrum         | ETH          | ❌       |
+| Avalanche        | AVAX         | ❌       |
+| Base             | ETH          | ❌       |
+| Base Sepolia     | ETH          | ✅       |
+| Base Goerli      | ETH          | ✅       |
+| BSC              | BNB          | ❌       |
+| BSC Testnet      | BNB          | ✅       |
+| Ethereum         | ETH          | ❌       |
+| Fantom           | FTM          | ❌       |
+| Fantom Testnet   | FTM          | ✅       |
+| Fuji             | AVAX         | ✅       |
+| Goerli           | ETH          | ✅       |
+| Linea            | ETH          | ❌       |
+| Linea Goerli     | ETH          | ✅       |
+| Linea Sepolia    | ETH          | ✅       |
+| Mumbai           | MATIC        | ✅       |
+| opBNB            | BNB          | ❌       |
+| opBNB Testnet    | BNB          | ✅       |
+| Optimism         | ETH          | ❌       |
+| Optimism Sepolia | ETH          | ✅       |
+| Optimism Goerli  | ETH          | ✅       |
+| Polygon          | MATIC        | ❌       |
+| Sepolia          | ETH          | ❌       |
+| zkSync           | ETH          | ❌       |
 
 For specifying network you only need to pass network's name.
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
+my_wallet = Wallet('your_private_key', 'Arbitrum')
 ```
 
 If you use unsupported network, you can specify it using type NetworkInfo
 ```python
 from evm_wallet import Wallet, NetworkInfo
 
 network_info = NetworkInfo(
     network='Custom',
-    rpc='https://custom.publicnode.com',
+    rpc='wss://custom.publicnode.com',
     token='CUSTOM'
 )
 custom_wallet = Wallet('your_private_key', network_info)
 ```
 
-evm-wallet also asynchronous approach
+Library supports asynchronous approach
 ```python
 from evm_wallet import AsyncWallet
 
 async def validate_balance():
     async_wallet = AsyncWallet('your_private_key', 'Arbitrum')
     balance = await async_wallet.get_balance()
     assert balance > 0.1
 ```
      
-<h2 id="#quick-overview">Quick overview</h2> 
+<h2 id="quick-overview">Quick overview</h2> 
 You can perform the following actions, using evm-wallet:
 
 - **[approve](#approve)**
 - **[build_and_transact](#build_and_transact)**
-- **[build_transaction_params](#build_transaction_params)**
+- **[build_tx_params](#build_tx_params)**
 - **[create](#create)**
 - **[estimate_gas](#estimate_gas)**
 - **[get_balance](#get_balance)**
 - **[get_balance_of](#get_balance_of)**
-- **[get_decimals](#get_decimals)**
+- **[get_token](#get_token)**
 - **[get_explorer_url](#get_explorer_url)**
-- **[get_transactions](#get_transactions)**
 - **[is_native_token](#is_native_token)**
 - **[transact](#transact)**
 - **[transfer](#transfer)**
 
 <h3 id="approve">approve</h3>
 
 When you want to spend non-native tokens, for instance USDT, you need to perform approving operation.
 
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-provider = arb_wallet.provider
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+provider = my_wallet.provider
 
 stargate_router = '0x8731d54E9D02c286767d56ac03e8037C07e01e98'
-usdt = '0xdAC17F958D2ee523a2206206994597C13D831ec7'
+usdt = my_wallet.get_token('0xdAC17F958D2ee523a2206206994597C13D831ec7')
 usdt_amount = provider.to_wei(0.001, 'ether')
 
-arb_wallet.approve(usdt, stargate_router, usdt_amount)
+my_wallet.approve(usdt, stargate_router, usdt_amount)
 ```
 
 <h3 id="build_and_transact">build_and_transact</h3>
 If you don't need to check estimated gas or directly use transact, you can call build_and_transact. It's based on getting
 closure as argument. Closure is transaction's function, called with arguments. Notice that it has to be not built or 
 awaited
 
 ```python
 from evm_wallet import Wallet
-from web3.contract import Contract
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-provider = arb_wallet.provider
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+provider = my_wallet.provider
 
-stargate_router = '0x8731d54E9D02c286767d56ac03e8037C07e01e98'
 stargate_abi = [...]
-stargate = Contract(stargate_router, stargate_abi)
+stargate_router = '0x8731d54E9D02c286767d56ac03e8037C07e01e98'
+stargate = my_wallet.provider.eth.contract(stargate_router, abi=stargate_abi)
 
 eth_amount = provider.to_wei(0.001, 'ether')
 closure = stargate.functions.swapETH(...) 
-arb_wallet.build_and_transact(closure, eth_amount)
+my_wallet.build_and_transact(closure, eth_amount)
 ```
 
-<h3 id="build_transaction_params">build_transaction_params</h3>
-You can use build_transaction_params to quickly get dictionary of params for building transaction. Public key, chain id 
+<h3 id="build_tx_params">build_tx_params</h3>
+You can use build_tx_params to quickly get dictionary of params for building transaction. Public key, chain id 
 and nonce are generated automatically. You also can also choose not to set a gas and the gas price
 
 ```python
-async def build_transaction_params(
-        self,
-        value: TokenAmount,
-        recipient: Optional[AnyAddress] = None,
-        raw_data: Optional[Union[bytes, HexStr]] = None,
-        gas: Optional[int] = None,
-        gas_price: Optional[Wei] = None
-) -> TxParams:
-    """
-    Returns transaction's params
-    :param value: A quantity of network currency to be paid in Wei units
-    :param recipient: An address of recipient
-    :param raw_data: Transaction's data provided as HexStr or bytes
-    :param gas: A quantity of gas to be spent
-    :param gas_price: A price of gas in Wei units
-    :return: Transaction's params
-    """
-    provider = self.provider
-
-    tx_params = {
-        'from': self.public_key,
-        'chainId': self.__chain_id,
-        'nonce': self.nonce,
-        'value': value,
-        'gas': gas if gas else Wei(250_000),
-        'gasPrice': gas_price if gas_price else await provider.eth.gas_price,
-    }
-
-    if recipient:
-        tx_params['to'] = self.provider.to_checksum_address(recipient)
+from evm_wallet import Wallet
+my_wallet = Wallet('your_private_key', 'BSC')
 
-    if raw_data:
-        tx_params['data'] = raw_data
+my_wallet.build_tx_params(0)
+```
 
-    return tx_params
+```json
+{
+  "from": "0xe977Fa8D8AE7D3D6e28c17A868EF04bD301c583f", 
+  "chainId": 56, 
+  "nonce": 168, 
+  "value": 0, 
+  "gas": 250000, 
+  "gasPrice": 1000000000
+}
 ```
 
 <h3 id="create">create</h3>
 You can use that, when you want to create all-new wallet
 
 ```python
 from evm_wallet import Wallet
@@ -181,138 +160,135 @@
 ```
             
 <h3 id="estimate_gas">estimate_gas</h3>
 When you want to estimate an amount of gas to send a transaction, you can use estimate_gas
 
 ```python
 from evm_wallet import Wallet
-from web3.contract import Contract
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-provider = arb_wallet.provider
+
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+provider = my_wallet.provider
 
 stargate_router = '0x8731d54E9D02c286767d56ac03e8037C07e01e98'
 stargate_abi = [...]
 eth_amount = provider.to_wei(0.001, 'ether')
 
-stargate = Contract(stargate_router, stargate_abi)
-params = arb_wallet.build_transaction_params(eth_amount)
-tx_data = stargate.functions.swapETH(...).buildTransaction(params)
-gas = arb_wallet.estimate_gas(tx_data)
-tx_data['gas'] = gas
+stargate = my_wallet.provider.eth.contract(stargate_router, abi=stargate_abi)
+params = my_wallet.build_tx_params(eth_amount)
+tx_params = stargate.functions.swapETH(...).buildTransaction(params)
+gas = my_wallet.estimate_gas(tx_params)
+tx_params['gas'] = gas
+
+my_wallet.transact(tx_params)
 ```
 
 <h3 id="get_balance">get_balance</h3>
 You can get the balance of the native token of your wallet.
 
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-balance = arb_wallet.get_balance()
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+balance = my_wallet.get_balance()
 ```
 
 <h3 id="get_balance_of">get_balance_of</h3>
 You can get the balance of specified token of your wallet
 
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-balance = arb_wallet.get_balance_of('0x82af49447d8a07e3bd95bd0d56f35241523fbab1', convert=True)
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+
+usdt = my_wallet.get_token('0xdAC17F958D2ee523a2206206994597C13D831ec7')
+balance = my_wallet.get_balance_of(usdt, convert=True)
 print(balance)
 ```
 
-<h3 id="get_decimals">get_decimals</h3>
-You can get the decimals of specified token 
+<h3 id="get_token">get_token</h3>
+You can get the ERC20Token instance, containing information about symbol and decimals. Also this function used for 
+another instance-methods of Wallet.
 
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-decimals = arb_wallet.get_decimals('0x82af49447d8a07e3bd95bd0d56f35241523fbab1')
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+usdt = my_wallet.get_token('0xdAC17F958D2ee523a2206206994597C13D831ec7')
+print(usdt.decimals)
 ```
             
 <h3 id="get_explorer_url">get_explorer_url</h3>
 You can get entire wallet's list of transactions
 
 ```python
 from evm_wallet import Wallet
 from web3.contract import Contract
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-provider = arb_wallet.provider
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+provider = my_wallet.provider
 
 stargate_router = '0x8731d54E9D02c286767d56ac03e8037C07e01e98'
 stargate_abi = [...]
 stargate = Contract(stargate_router, stargate_abi)
 
 eth_amount = provider.to_wei(0.001, 'ether')
 closure = stargate.functions.swapETH(...) 
-tx_hash = arb_wallet.build_and_transact(closure, eth_amount)
-print(arb_wallet.get_explorer_url(tx_hash))
-```
-
-
-<h3 id="get_transactions">get_transactions</h3>
-You can get entire wallet's list of transactions
-
-```python
-from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-transactions = arb_wallet.get_transactions()
+tx_hash = my_wallet.build_and_transact(closure, eth_amount)
+print(my_wallet.get_explorer_url(tx_hash))
 ```
 
 <h3 id="is_native_token">is_native_token</h3>
 If you want to check, if the specific token is native token of network, you can use is_native_token.
 
 You can use any case in a token's ticker.
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-assert arb_wallet.is_native_token('eTh')
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+assert my_wallet.is_native_token('eTh')
 ```
 
 Or you can pass zero-address meaning address of network's native token.
 ```python
 from evm_wallet import Wallet, ZERO_ADDRESS
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-assert arb_wallet.is_native_token(ZERO_ADDRESS)
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+assert my_wallet.is_native_token(ZERO_ADDRESS)
 ```
 
 <h3 id="transact">transact</h3>
 After building transaction you can perform it, passing transaction data to transact
 
 ```python
 from evm_wallet import Wallet
 from web3.contract import Contract
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-provider = arb_wallet.provider
+
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+provider = my_wallet.provider
 
 stargate_router = '0x8731d54E9D02c286767d56ac03e8037C07e01e98'
 stargate_abi = [...]
 eth_amount = provider.to_wei(0.001, 'ether')
 
-stargate = Contract(stargate_router, stargate_abi)
-params = arb_wallet.build_transaction_params(eth_amount)
+stargate = my_wallet.provider.eth.contract(stargate_router, abi=stargate_abi)
+params = my_wallet.build_tx_params(eth_amount)
 tx_data = stargate.functions.swapETH(...).buildTransaction(params)
-gas = arb_wallet.estimate_gas(tx_data)
+gas = my_wallet.estimate_gas(tx_data)
 tx_data['gas'] = gas
 
-arb_wallet.transact(tx_data)
+my_wallet.transact(tx_data)
 ```
 
 <h3 id="transfer">transfer</h3>
 You can transfer tokens to another wallet
 
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-provider = arb_wallet.provider
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+provider = my_wallet.provider
 
 recipient = '0xe977Fa8D8AE7D3D6e28c17A868EF04bD301c583f'
-usdt = '0xdAC17F958D2ee523a2206206994597C13D831ec7'
+usdt = my_wallet.get_token('0xdAC17F958D2ee523a2206206994597C13D831ec7')
 usdt_amount = provider.to_wei(0.001, 'ether')
 
-arb_wallet.transfer(usdt, recipient, usdt_amount)
+my_wallet.transfer(usdt, recipient, usdt_amount)
 ```
 
 # Installing evm-wallet
         
 To install the package from GitHub you can use:
 
 ```shell
```

### Comparing `evm_wallet-1.2.0/evm_wallet/__init__.py` & `evm_wallet-2.0.0/evm_wallet/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 evm-wallet
 ~~~~~~~~~~~~~~
 The package, containing wrapper over EVM operations for interacting through Wallet units.
 Author github - https://github.com/blnkoff
 
 Usage example:
    >>> from evm_wallet import Wallet
-   >>> arb_wallet = Wallet('your_private_key', 'Arbitrum')
-   >>> provider = arb_wallet.provider
+   >>> my_wallet = Wallet('your_private_key', 'Arbitrum')
+   >>> provider = my_wallet.provider
    >>> recipient = '0xe977Fa8D8AE7D3D6e28c17A868EF04bD301c583f'
-   >>> usdt = '0xdAC17F958D2ee523a2206206994597C13D831ec7'
+   >>> 
+   >>> usdt = my_wallet.get_token('0xdAC17F958D2ee523a2206206994597C13D831ec7')
    >>> usdt_amount = provider.to_wei(0.001)
    >>>
-   >>> if arb_wallet.get_balance() >= 0.01:
-   >>>     arb_wallet.transfer(usdt, recipient, usdt_amount)
+   >>> if my_wallet.get_balance() >= 0.01:
+   >>>     my_wallet.transfer(usdt, recipient, usdt_amount)
 
 :copyright: (c) 2023 by Alexey
-:license: Apache 2.0, see LICENSE for more details.
+:license: MIT, see LICENSE for more details.
 """
 
-from .wallet import AsyncWallet, Wallet
-from .types import NetworkInfo
-from .globals import ZERO_ADDRESS
+from .wallet import Wallet
+from .async_wallet import AsyncWallet
+from .types import NetworkInfo, ERC20Token
+from ._base_wallet import ZERO_ADDRESS
```

### Comparing `evm_wallet-1.2.0/evm_wallet/erc20.abi` & `evm_wallet-2.0.0/evm_wallet/erc20.abi`

 * *Files identical despite different names*

### Comparing `evm_wallet-1.2.0/pyproject.toml` & `evm_wallet-2.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = 'evm_wallet'
-version = '1.2.0'
+version = '2.0.0'
 description = 'The package, containing wrapper over EVM operations for interacting through Wallet entities'
-authors = ['Alexey <abelenkov2006@gmail.com>']
+authors = ['Alexey <axbelenkov@gmail.com>']
 license = 'MIT'
 readme = 'README.md'
 repository = 'https://github.com/blnkoff/evm-wallet'
 homepage = 'https://github.com/blnkoff/evm-wallet'
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
@@ -20,15 +20,16 @@
 packages = [{ include = 'evm_wallet' }]
 
 [tool.poetry.dependencies]
 python = '^3.11'
 web3 = "^6.12.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.3"
 pytest-asyncio = "^0.23.2"
 build = "^1.0.3"
 twine = "^4.0.2"
+python-dotenv = "^1.0.1"
+pytest = "^8.1.1"
 
 [build-system]
 requires = ['poetry-core']
 build-backend = 'poetry.core.masonry.api'
```

### Comparing `evm_wallet-1.2.0/PKG-INFO` & `evm_wallet-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: evm_wallet
-Version: 1.2.0
+Version: 2.0.0
 Summary: The package, containing wrapper over EVM operations for interacting through Wallet entities
 Home-page: https://github.com/blnkoff/evm-wallet
 License: MIT
 Author: Alexey
-Author-email: abelenkov2006@gmail.com
+Author-email: axbelenkov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,14 @@
 Project-URL: Repository, https://github.com/blnkoff/evm-wallet
 Description-Content-Type: text/markdown
 
 # evm-wallet
 
 [![Croco Logo](https://i.ibb.co/G5Pjt6M/logo.png)](https://t.me/crocofactory)
 
-
 The package, containing wrapper over EVM operations for interacting through Wallet entities.
 
 - **[Telegram channel](https://t.me/crocofactory)**
 - **[Overview](#quick-overview)**
 - **[Bug reports](https://github.com/blnkoff/evm-wallet/issues)**
 
 
@@ -41,162 +40,142 @@
 - quick performing useful functions of Web3.py
    
 evm-wallet's source code is made available under the [MIT License](LICENSE)
 
 ##  Quick start
 You can quickly use supported networks as RPC:  
 
-| Network         | Native Token | Testnet  |
-|-----------------|--------------|----------|
-| Arbitrum Goerli | AGOR         | ✅        |
-| Arbitrum        | ETH          | ❌        |
-| Avalanche       | AVAX         | ❌        |
-| Base            | ETH          | ❌        |
-| Base Goerli     | ETH          | ✅        |
-| BSC             | BNB          | ❌        |
-| BSC Testnet     | tBNB         | ✅        |
-| Ethereum        | ETH          | ❌        |
-| Fantom          | FTM          | ❌        |
-| Fantom Testnet  | FTM          | ✅        |
-| Fuji            | AVAX         | ✅        |
-| Goerli          | GETH         | ✅        |
-| Linea           | ETH          | ❌        |
-| Linea Goerli    | ETH          | ✅        |
-| Mumbai          | MATIC        | ✅        |
-| opBNB           | BNB          | ❌        |
-| opBNB Testnet   | BNB          | ✅        |
-| Optimism        | ETH          | ❌        |
-| Optimism Goerli | OGOR         | ✅        |
-| Polygon         | MATIC        | ❌        |
-| Sepolia         | SETH         | ❌        |
-| zkSync          | ETH          | ❌        |
-
-
+| Network          | Native Token | Testnet |
+|------------------|--------------|---------|
+| Arbitrum Goerli  | ETH          | ✅       |
+| Arbitrum Sepolia | ETH          | ✅       |
+| Arbitrum         | ETH          | ❌       |
+| Avalanche        | AVAX         | ❌       |
+| Base             | ETH          | ❌       |
+| Base Sepolia     | ETH          | ✅       |
+| Base Goerli      | ETH          | ✅       |
+| BSC              | BNB          | ❌       |
+| BSC Testnet      | BNB          | ✅       |
+| Ethereum         | ETH          | ❌       |
+| Fantom           | FTM          | ❌       |
+| Fantom Testnet   | FTM          | ✅       |
+| Fuji             | AVAX         | ✅       |
+| Goerli           | ETH          | ✅       |
+| Linea            | ETH          | ❌       |
+| Linea Goerli     | ETH          | ✅       |
+| Linea Sepolia    | ETH          | ✅       |
+| Mumbai           | MATIC        | ✅       |
+| opBNB            | BNB          | ❌       |
+| opBNB Testnet    | BNB          | ✅       |
+| Optimism         | ETH          | ❌       |
+| Optimism Sepolia | ETH          | ✅       |
+| Optimism Goerli  | ETH          | ✅       |
+| Polygon          | MATIC        | ❌       |
+| Sepolia          | ETH          | ❌       |
+| zkSync           | ETH          | ❌       |
 
 For specifying network you only need to pass network's name.
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
+my_wallet = Wallet('your_private_key', 'Arbitrum')
 ```
 
 If you use unsupported network, you can specify it using type NetworkInfo
 ```python
 from evm_wallet import Wallet, NetworkInfo
 
 network_info = NetworkInfo(
     network='Custom',
-    rpc='https://custom.publicnode.com',
+    rpc='wss://custom.publicnode.com',
     token='CUSTOM'
 )
 custom_wallet = Wallet('your_private_key', network_info)
 ```
 
-evm-wallet also asynchronous approach
+Library supports asynchronous approach
 ```python
 from evm_wallet import AsyncWallet
 
 async def validate_balance():
     async_wallet = AsyncWallet('your_private_key', 'Arbitrum')
     balance = await async_wallet.get_balance()
     assert balance > 0.1
 ```
      
-<h2 id="#quick-overview">Quick overview</h2> 
+<h2 id="quick-overview">Quick overview</h2> 
 You can perform the following actions, using evm-wallet:
 
 - **[approve](#approve)**
 - **[build_and_transact](#build_and_transact)**
-- **[build_transaction_params](#build_transaction_params)**
+- **[build_tx_params](#build_tx_params)**
 - **[create](#create)**
 - **[estimate_gas](#estimate_gas)**
 - **[get_balance](#get_balance)**
 - **[get_balance_of](#get_balance_of)**
-- **[get_decimals](#get_decimals)**
+- **[get_token](#get_token)**
 - **[get_explorer_url](#get_explorer_url)**
-- **[get_transactions](#get_transactions)**
 - **[is_native_token](#is_native_token)**
 - **[transact](#transact)**
 - **[transfer](#transfer)**
 
 <h3 id="approve">approve</h3>
 
 When you want to spend non-native tokens, for instance USDT, you need to perform approving operation.
 
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-provider = arb_wallet.provider
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+provider = my_wallet.provider
 
 stargate_router = '0x8731d54E9D02c286767d56ac03e8037C07e01e98'
-usdt = '0xdAC17F958D2ee523a2206206994597C13D831ec7'
+usdt = my_wallet.get_token('0xdAC17F958D2ee523a2206206994597C13D831ec7')
 usdt_amount = provider.to_wei(0.001, 'ether')
 
-arb_wallet.approve(usdt, stargate_router, usdt_amount)
+my_wallet.approve(usdt, stargate_router, usdt_amount)
 ```
 
 <h3 id="build_and_transact">build_and_transact</h3>
 If you don't need to check estimated gas or directly use transact, you can call build_and_transact. It's based on getting
 closure as argument. Closure is transaction's function, called with arguments. Notice that it has to be not built or 
 awaited
 
 ```python
 from evm_wallet import Wallet
-from web3.contract import Contract
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-provider = arb_wallet.provider
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+provider = my_wallet.provider
 
-stargate_router = '0x8731d54E9D02c286767d56ac03e8037C07e01e98'
 stargate_abi = [...]
-stargate = Contract(stargate_router, stargate_abi)
+stargate_router = '0x8731d54E9D02c286767d56ac03e8037C07e01e98'
+stargate = my_wallet.provider.eth.contract(stargate_router, abi=stargate_abi)
 
 eth_amount = provider.to_wei(0.001, 'ether')
 closure = stargate.functions.swapETH(...) 
-arb_wallet.build_and_transact(closure, eth_amount)
+my_wallet.build_and_transact(closure, eth_amount)
 ```
 
-<h3 id="build_transaction_params">build_transaction_params</h3>
-You can use build_transaction_params to quickly get dictionary of params for building transaction. Public key, chain id 
+<h3 id="build_tx_params">build_tx_params</h3>
+You can use build_tx_params to quickly get dictionary of params for building transaction. Public key, chain id 
 and nonce are generated automatically. You also can also choose not to set a gas and the gas price
 
 ```python
-async def build_transaction_params(
-        self,
-        value: TokenAmount,
-        recipient: Optional[AnyAddress] = None,
-        raw_data: Optional[Union[bytes, HexStr]] = None,
-        gas: Optional[int] = None,
-        gas_price: Optional[Wei] = None
-) -> TxParams:
-    """
-    Returns transaction's params
-    :param value: A quantity of network currency to be paid in Wei units
-    :param recipient: An address of recipient
-    :param raw_data: Transaction's data provided as HexStr or bytes
-    :param gas: A quantity of gas to be spent
-    :param gas_price: A price of gas in Wei units
-    :return: Transaction's params
-    """
-    provider = self.provider
-
-    tx_params = {
-        'from': self.public_key,
-        'chainId': self.__chain_id,
-        'nonce': self.nonce,
-        'value': value,
-        'gas': gas if gas else Wei(250_000),
-        'gasPrice': gas_price if gas_price else await provider.eth.gas_price,
-    }
-
-    if recipient:
-        tx_params['to'] = self.provider.to_checksum_address(recipient)
+from evm_wallet import Wallet
+my_wallet = Wallet('your_private_key', 'BSC')
 
-    if raw_data:
-        tx_params['data'] = raw_data
+my_wallet.build_tx_params(0)
+```
 
-    return tx_params
+```json
+{
+  "from": "0xe977Fa8D8AE7D3D6e28c17A868EF04bD301c583f", 
+  "chainId": 56, 
+  "nonce": 168, 
+  "value": 0, 
+  "gas": 250000, 
+  "gasPrice": 1000000000
+}
 ```
 
 <h3 id="create">create</h3>
 You can use that, when you want to create all-new wallet
 
 ```python
 from evm_wallet import Wallet
@@ -204,138 +183,135 @@
 ```
             
 <h3 id="estimate_gas">estimate_gas</h3>
 When you want to estimate an amount of gas to send a transaction, you can use estimate_gas
 
 ```python
 from evm_wallet import Wallet
-from web3.contract import Contract
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-provider = arb_wallet.provider
+
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+provider = my_wallet.provider
 
 stargate_router = '0x8731d54E9D02c286767d56ac03e8037C07e01e98'
 stargate_abi = [...]
 eth_amount = provider.to_wei(0.001, 'ether')
 
-stargate = Contract(stargate_router, stargate_abi)
-params = arb_wallet.build_transaction_params(eth_amount)
-tx_data = stargate.functions.swapETH(...).buildTransaction(params)
-gas = arb_wallet.estimate_gas(tx_data)
-tx_data['gas'] = gas
+stargate = my_wallet.provider.eth.contract(stargate_router, abi=stargate_abi)
+params = my_wallet.build_tx_params(eth_amount)
+tx_params = stargate.functions.swapETH(...).buildTransaction(params)
+gas = my_wallet.estimate_gas(tx_params)
+tx_params['gas'] = gas
+
+my_wallet.transact(tx_params)
 ```
 
 <h3 id="get_balance">get_balance</h3>
 You can get the balance of the native token of your wallet.
 
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-balance = arb_wallet.get_balance()
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+balance = my_wallet.get_balance()
 ```
 
 <h3 id="get_balance_of">get_balance_of</h3>
 You can get the balance of specified token of your wallet
 
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-balance = arb_wallet.get_balance_of('0x82af49447d8a07e3bd95bd0d56f35241523fbab1', convert=True)
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+
+usdt = my_wallet.get_token('0xdAC17F958D2ee523a2206206994597C13D831ec7')
+balance = my_wallet.get_balance_of(usdt, convert=True)
 print(balance)
 ```
 
-<h3 id="get_decimals">get_decimals</h3>
-You can get the decimals of specified token 
+<h3 id="get_token">get_token</h3>
+You can get the ERC20Token instance, containing information about symbol and decimals. Also this function used for 
+another instance-methods of Wallet.
 
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-decimals = arb_wallet.get_decimals('0x82af49447d8a07e3bd95bd0d56f35241523fbab1')
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+usdt = my_wallet.get_token('0xdAC17F958D2ee523a2206206994597C13D831ec7')
+print(usdt.decimals)
 ```
             
 <h3 id="get_explorer_url">get_explorer_url</h3>
 You can get entire wallet's list of transactions
 
 ```python
 from evm_wallet import Wallet
 from web3.contract import Contract
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-provider = arb_wallet.provider
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+provider = my_wallet.provider
 
 stargate_router = '0x8731d54E9D02c286767d56ac03e8037C07e01e98'
 stargate_abi = [...]
 stargate = Contract(stargate_router, stargate_abi)
 
 eth_amount = provider.to_wei(0.001, 'ether')
 closure = stargate.functions.swapETH(...) 
-tx_hash = arb_wallet.build_and_transact(closure, eth_amount)
-print(arb_wallet.get_explorer_url(tx_hash))
-```
-
-
-<h3 id="get_transactions">get_transactions</h3>
-You can get entire wallet's list of transactions
-
-```python
-from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-transactions = arb_wallet.get_transactions()
+tx_hash = my_wallet.build_and_transact(closure, eth_amount)
+print(my_wallet.get_explorer_url(tx_hash))
 ```
 
 <h3 id="is_native_token">is_native_token</h3>
 If you want to check, if the specific token is native token of network, you can use is_native_token.
 
 You can use any case in a token's ticker.
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-assert arb_wallet.is_native_token('eTh')
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+assert my_wallet.is_native_token('eTh')
 ```
 
 Or you can pass zero-address meaning address of network's native token.
 ```python
 from evm_wallet import Wallet, ZERO_ADDRESS
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-assert arb_wallet.is_native_token(ZERO_ADDRESS)
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+assert my_wallet.is_native_token(ZERO_ADDRESS)
 ```
 
 <h3 id="transact">transact</h3>
 After building transaction you can perform it, passing transaction data to transact
 
 ```python
 from evm_wallet import Wallet
 from web3.contract import Contract
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-provider = arb_wallet.provider
+
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+provider = my_wallet.provider
 
 stargate_router = '0x8731d54E9D02c286767d56ac03e8037C07e01e98'
 stargate_abi = [...]
 eth_amount = provider.to_wei(0.001, 'ether')
 
-stargate = Contract(stargate_router, stargate_abi)
-params = arb_wallet.build_transaction_params(eth_amount)
+stargate = my_wallet.provider.eth.contract(stargate_router, abi=stargate_abi)
+params = my_wallet.build_tx_params(eth_amount)
 tx_data = stargate.functions.swapETH(...).buildTransaction(params)
-gas = arb_wallet.estimate_gas(tx_data)
+gas = my_wallet.estimate_gas(tx_data)
 tx_data['gas'] = gas
 
-arb_wallet.transact(tx_data)
+my_wallet.transact(tx_data)
 ```
 
 <h3 id="transfer">transfer</h3>
 You can transfer tokens to another wallet
 
 ```python
 from evm_wallet import Wallet
-arb_wallet = Wallet('your_private_key', 'Arbitrum')
-provider = arb_wallet.provider
+my_wallet = Wallet('your_private_key', 'Arbitrum')
+provider = my_wallet.provider
 
 recipient = '0xe977Fa8D8AE7D3D6e28c17A868EF04bD301c583f'
-usdt = '0xdAC17F958D2ee523a2206206994597C13D831ec7'
+usdt = my_wallet.get_token('0xdAC17F958D2ee523a2206206994597C13D831ec7')
 usdt_amount = provider.to_wei(0.001, 'ether')
 
-arb_wallet.transfer(usdt, recipient, usdt_amount)
+my_wallet.transfer(usdt, recipient, usdt_amount)
 ```
 
 # Installing evm-wallet
         
 To install the package from GitHub you can use:
 
 ```shell
```


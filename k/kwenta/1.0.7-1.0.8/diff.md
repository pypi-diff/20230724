# Comparing `tmp/kwenta-1.0.7.tar.gz` & `tmp/kwenta-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwenta-1.0.7.tar", last modified: Fri Jul  7 12:19:11 2023, max compression
+gzip compressed data, was "kwenta-1.0.8.tar", last modified: Mon Jul 24 15:44:23 2023, max compression
```

## Comparing `kwenta-1.0.7.tar` & `kwenta-1.0.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.773059 kwenta-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 12:18:42.000000 kwenta-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 12:19:11.773059 kwenta-1.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.769058 kwenta-1.0.7/kwenta/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.769058 kwenta-1.0.7/kwenta/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/alerts/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.769058 kwenta-1.0.7/kwenta/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/cli/kwenta_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.769058 kwenta-1.0.7/kwenta/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.773059 kwenta-1.0.7/kwenta/contracts/json/
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/PerpsV2ExchangeRate.json
--rw-r--r--   0 runner    (1001) docker     (123)    37179 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/PerpsV2Market.json
--rw-r--r--   0 runner    (1001) docker     (123)    43146 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/SMAccount.json
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/SMFactory.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/sUSD.json
--rw-r--r--   0 runner    (1001) docker     (123)    57026 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/kwenta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.773059 kwenta-1.0.7/kwenta/pyth/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/pyth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/pyth/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/pyth/pyth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.773059 kwenta-1.0.7/kwenta/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/queries/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/queries/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/queries/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.769058 kwenta-1.0.7/kwenta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 12:19:11.000000 kwenta-1.0.7/kwenta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-07 12:19:11.000000 kwenta-1.0.7/kwenta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:19:11.000000 kwenta-1.0.7/kwenta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 12:19:11.000000 kwenta-1.0.7/kwenta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:19:11.000000 kwenta-1.0.7/kwenta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 12:19:11.000000 kwenta-1.0.7/kwenta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:19:11.773059 kwenta-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 12:18:42.000000 kwenta-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 15:43:49.000000 kwenta-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 15:44:23.055659 kwenta-1.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.051658 kwenta-1.0.8/kwenta/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/alerts/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/cli/kwenta_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta/contracts/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/PerpsV2ExchangeRate.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37179 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/PerpsV2Market.json
+-rw-r--r--   0 runner    (1001) docker     (123)    43146 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/SMAccount.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/SMFactory.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/contracts/json/sUSD.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57402 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/kwenta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta/pyth/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/pyth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/pyth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/pyth/pyth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/queries/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/queries/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-24 15:43:49.000000 kwenta-1.0.8/kwenta/queries/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:44:23.055659 kwenta-1.0.8/kwenta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 15:44:23.000000 kwenta-1.0.8/kwenta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-24 15:44:23.000000 kwenta-1.0.8/kwenta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:44:23.000000 kwenta-1.0.8/kwenta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 15:44:23.000000 kwenta-1.0.8/kwenta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:44:23.000000 kwenta-1.0.8/kwenta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 15:44:23.000000 kwenta-1.0.8/kwenta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:44:23.055659 kwenta-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-24 15:43:49.000000 kwenta-1.0.8/setup.py
```

### Comparing `kwenta-1.0.7/PKG-INFO` & `kwenta-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.7/kwenta/alerts/alerts.py` & `kwenta-1.0.8/kwenta/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/cli/kwenta_cli.py` & `kwenta-1.0.8/kwenta/cli/kwenta_cli.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/constants.py` & `kwenta-1.0.8/kwenta/constants.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/contracts/contracts.py` & `kwenta-1.0.8/kwenta/contracts/contracts.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/contracts/json/PerpsV2ExchangeRate.json` & `kwenta-1.0.8/kwenta/contracts/json/PerpsV2ExchangeRate.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/contracts/json/PerpsV2Market.json` & `kwenta-1.0.8/kwenta/contracts/json/PerpsV2Market.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/contracts/json/PerpsV2MarketData.json` & `kwenta-1.0.8/kwenta/contracts/json/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/contracts/json/SMAccount.json` & `kwenta-1.0.8/kwenta/contracts/json/SMAccount.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/contracts/json/SMFactory.json` & `kwenta-1.0.8/kwenta/contracts/json/SMFactory.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/contracts/json/sUSD.json` & `kwenta-1.0.8/kwenta/contracts/json/sUSD.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/kwenta.py` & `kwenta-1.0.8/kwenta/kwenta.py`

 * *Files 2% similar despite different names*

```diff
@@ -754,85 +754,93 @@
         str: token transfer Tx id
         """
         sm_account_contract = self.web3.eth.contract(
             self.web3.to_checksum_address(self.sm_account), abi=abis["SM_Account"]
         )
         if token_amount == 0:
             raise Exception("token_amount Cannot be 0.")
-
+        #Check for withdrawal 
         is_withdrawal = -1 if token_amount < 0 else 1
         token_amount = self.web3.to_wei(abs(token_amount), "ether") * is_withdrawal
         print(token_amount)
         if is_withdrawal > 0:
             susd_balance = self.get_susd_balance(self.wallet_address)
         else:
             susd_balance = self.get_susd_balance(self.sm_account)
         print(f"sUSD Balance: {susd_balance['balance_usd']}")
-        if token_amount < susd_balance["balance"]:
-            if execute_now:
-                if (token_amount > 0) and (skip_approval is False):
-                    self.approve_susd(token_amount)
-                    print("Waiting for Approval...")
-                    time.sleep(4.5)
-                if token_amount > 0:
-                    print(f"Adding sUSD to {token_symbol} Market.")
-                    time.sleep(4.5)
-                    print(
-                        f"Market_address: {(self.markets[token_symbol.upper()]['market_address'])}"
-                    )
-                    commandBytes1 = encode(["int256"], [token_amount])
-                    commandBytes2 = encode(
-                        ["address", "int256"],
-                        [
-                            str(self.markets[token_symbol.upper()]["market_address"]),
-                            token_amount,
-                        ],
-                    )
-                    data_tx = sm_account_contract.encodeABI(
-                        fn_name="execute", args=[[0, 2], [commandBytes1, commandBytes2]]
-                    )
-                    tx_params = self._get_tx_params(to=self.sm_account, value=0)
-                    tx_params["data"] = data_tx
-                    tx_params["nonce"] = self.web3.eth.get_transaction_count(
-                        self.wallet_address
-                    )
-                    tx_token = self.execute_transaction(tx_params)
-                    return tx_token
-                else:
-                    # Execute Commands: https://github.com/Kwenta/smart-margin/wiki/Commands
-                    # args[0] == Command ID, args[1] == command inputs, in bytes
-                    if withdrawal_all:
-                        token_amount = (
-                            int(
-                                self.get_accessible_margin(self.sm_account)[
-                                    "margin_remaining_usd"
-                                ]
-                            )
-                            * -1
-                        )
-                    commandBytes = encode(["int256"], [token_amount])
-                    data_tx = sm_account_contract.encodeABI(
-                        fn_name="execute", args=[[0], [commandBytes]]
-                    )
-                    tx_params = self._get_tx_params(to=self.sm_account, value=0)
-                    tx_params["data"] = data_tx
-                    tx_params["nonce"] = self.web3.eth.get_transaction_count(
-                        self.wallet_address
-                    )
+        #check that withdrawal is less than account balance
+        if (token_amount > susd_balance["balance"]):
+            raise Exception(f"Token amount: {token_amount} is greater than Account Balance: {{susd_balance['balance_usd']}}! Verify your balance.")
+        #Move amount from EOA Wallet to SM Account 
+        if (is_withdrawal > 0):
+            if (token_amount > 0) and (skip_approval is False):
+                self.approve_susd(token_amount)
+                print("Waiting for Approval...")
+                time.sleep(4.5)
+            #adding to sm account
+            if token_amount > 0:
+                print(f"Adding sUSD to {token_symbol} Market.")
+                time.sleep(4.5)
+                print(
+                    f"Market_address: {(self.markets[token_symbol.upper()]['market_address'])}"
+                )
+                commandBytes1 = encode(["int256"], [token_amount])
+                commandBytes2 = encode(
+                    ["address", "int256"],
+                    [
+                        str(self.markets[token_symbol.upper()]["market_address"]),
+                        token_amount,
+                    ],
+                )
+                data_tx = sm_account_contract.encodeABI(
+                    fn_name="execute", args=[[0, 2], [commandBytes1, commandBytes2]]
+                )
+                tx_params = self._get_tx_params(to=self.sm_account, value=0)
+                tx_params["data"] = data_tx
+                tx_params["nonce"] = self.web3.eth.get_transaction_count(
+                    self.wallet_address
+                )
+                if execute_now:
                     tx_token = self.execute_transaction(tx_params)
                     print(f"Adding {token_amount} sUSD to Account.")
                     print(f"TX: {tx_token}")
                     return tx_token
+                else:
+                    return {
+                        "token_amount": token_amount / (10**18),
+                        "susd_balance": susd_balance,
+                        "tx_data": tx_params,
+                    }
+        #token Amount Negative == Withdrawal to EOA Wallet
+        else:
+            # Execute Commands: https://github.com/Kwenta/smart-margin/wiki/Commands
+            # args[0] == Command ID, args[1] == command inputs, in bytes
+            if withdrawal_all:
+                token_amount = (int(self.get_accessible_margin(self.sm_account)["margin_remaining"])* -1)
+            commandBytes = encode(["int256"], [token_amount])
+            data_tx = sm_account_contract.encodeABI(
+                fn_name="execute", args=[[0], [commandBytes]]
+            )
+            tx_params = self._get_tx_params(to=self.sm_account, value=0)
+            tx_params["data"] = data_tx
+            tx_params["nonce"] = self.web3.eth.get_transaction_count(
+                self.wallet_address
+            )
+            if execute_now:
+                tx_token = self.execute_transaction(tx_params)
+                print(f"Adding {token_amount} sUSD Moved to EOA Account.")
+                print(f"TX: {tx_token}")
+                return tx_token
             else:
                 return {
                     "token_amount": token_amount / (10**18),
                     "susd_balance": susd_balance,
                     "tx_data": tx_params,
                 }
-
+                
     def modify_position(
         self,
         token_symbol: str,
         position_size: float,
         wallet_address: str,
         slippage: float = DEFAULT_SLIPPAGE,
         execute_now: bool = False,
```

### Comparing `kwenta-1.0.7/kwenta/pyth/constants.py` & `kwenta-1.0.8/kwenta/pyth/constants.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/queries/config.py` & `kwenta-1.0.8/kwenta/queries/config.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/queries/gql.py` & `kwenta-1.0.8/kwenta/queries/gql.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta/queries/queries.py` & `kwenta-1.0.8/kwenta/queries/queries.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/kwenta.egg-info/PKG-INFO` & `kwenta-1.0.8/kwenta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.7/kwenta.egg-info/SOURCES.txt` & `kwenta-1.0.8/kwenta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.7/setup.py` & `kwenta-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kwenta",
-    version="1.0.7",
+    version="1.0.8",
     description="Python SDK for Kwenta",
     long_description="Python SDK for Kwenta",
     author="Kwenta DAO",
     packages=[
         "kwenta",
         "kwenta.alerts",
         "kwenta.cli",
```


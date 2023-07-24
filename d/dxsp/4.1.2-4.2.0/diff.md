# Comparing `tmp/dxsp-4.1.2.tar.gz` & `tmp/dxsp-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-4.1.2.tar", max compression
+gzip compressed data, was "dxsp-4.2.0.tar", max compression
```

## Comparing `dxsp-4.1.2.tar` & `dxsp-4.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-07-21 21:13:31.448468 dxsp-4.1.2/LICENSE
--rw-r--r--   0        0        0     2857 2023-07-21 21:13:31.448468 dxsp-4.1.2/README.md
--rw-r--r--   0        0        0      158 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/config.py
--rw-r--r--   0        0        0    12100 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/default_settings.toml
--rw-r--r--   0        0        0     5701 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/main.py
--rw-r--r--   0        0        0      104 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1864 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0     1037 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0      102 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/utils/__init__.py
--rw-r--r--   0        0        0     4834 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/utils/account_utils.py
--rw-r--r--   0        0        0     6619 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/utils/contract_utils.py
--rw-r--r--   0        0        0     1990 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/utils/explorer_utils.py
--rw-r--r--   0        0        0      363 2023-07-21 21:13:31.452468 dxsp-4.1.2/dxsp/utils/utils.py
--rw-r--r--   0        0        0     4008 2023-07-21 21:13:36.244546 dxsp-4.1.2/pyproject.toml
--rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 dxsp-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-24 10:54:31.353398 dxsp-4.2.0/LICENSE
+-rw-r--r--   0        0        0     2857 2023-07-24 10:54:31.353398 dxsp-4.2.0/README.md
+-rw-r--r--   0        0        0      158 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/config.py
+-rw-r--r--   0        0        0    12100 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0     5743 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/main.py
+-rw-r--r--   0        0        0      104 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1864 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0     1037 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0      102 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/utils/__init__.py
+-rw-r--r--   0        0        0     4834 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/utils/account_utils.py
+-rw-r--r--   0        0        0     6619 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/utils/contract_utils.py
+-rw-r--r--   0        0        0     1990 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/utils/explorer_utils.py
+-rw-r--r--   0        0        0      363 2023-07-24 10:54:31.353398 dxsp-4.2.0/dxsp/utils/utils.py
+-rw-r--r--   0        0        0     4028 2023-07-24 10:54:36.465433 dxsp-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 dxsp-4.2.0/PKG-INFO
```

### Comparing `dxsp-4.1.2/LICENSE` & `dxsp-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.2/README.md` & `dxsp-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.2/dxsp/default_settings.toml` & `dxsp-4.2.0/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.2/dxsp/main.py` & `dxsp-4.2.0/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
  DEX SWAP Main
 """
 
 import decimal
-import logging
 from typing import Optional
 
+from loguru import logger
 from web3 import Web3
 from web3.gas_strategies.time_based import medium_gas_price_strategy
 
 from dxsp.config import settings
 from dxsp.utils import AccountUtils, ContractUtils
 
 
 class DexSwap:
     """swap  class"""
     def __init__(self, w3: Optional[Web3] = None):
-        self.logger = logging.getLogger(name="DexSwap")
+        # self.logger = logging.getLogger(name="DexSwap")
+        self.logger = logger
         self.w3 = w3 or Web3(Web3.HTTPProvider(settings.dex_rpc))
         if not self.w3.net.listening:
             raise ValueError("w3 not connected")
         self.w3.eth.set_gas_price_strategy(medium_gas_price_strategy)
 
         self.account = AccountUtils(w3=self.w3)
```

### Comparing `dxsp-4.1.2/dxsp/protocols/oneinch.py` & `dxsp-4.2.0/dxsp/protocols/oneinch.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,18 @@
         #         + str(sell_address)
         #         + "&amount="
         #         + str(min_amount))
         #     quote_response = await self._get(
         #         url=quote_url,
         #         params=None,
         #         headers=settings.headers)
-        #     self.logger.debug("quote_response %s", quote_response)
+        #     self.logger.debug("quote_response {}", quote_response)
         #     if quote_response:
         #         quote_amount = quote_response['toTokenAmount']
-        #         self.logger.debug("quote_amount %s", quote_amount)
+        #         self.logger.debug("quote_amount {}", quote_amount)
         #         # quote_decimals = quote_response['fromToken']['decimals']
         #         quote = self.w3.from_wei(int(quote_amount), 'ether')
         #         # /(10 ** quote_decimals))
         #         return round(quote, 2)
     #     except Exception as error:
     #         raise ValueError(f"Approval failed {error}")
```

### Comparing `dxsp-4.1.2/dxsp/protocols/uniswap.py` & `dxsp-4.2.0/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.2/dxsp/protocols/zerox.py` & `dxsp-4.2.0/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.2/dxsp/utils/account_utils.py` & `dxsp-4.2.0/dxsp/utils/account_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.2/dxsp/utils/contract_utils.py` & `dxsp-4.2.0/dxsp/utils/contract_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,25 +68,25 @@
                 coin_dict = self.cg.get_coin_by_id(i)
                 try:
                     if coin_dict['platforms'][f'{await self.search_cg_platform()}']:
                         return coin_dict
                 except (KeyError, requests.exceptions.HTTPError):
                     pass
         except Exception as e:
-            self.logger.error("search_cg %s", e)
+            self.logger.error("search_cg {}", e)
             return
 
     async def search_cg_contract(self, token):
         """search coingecko contract"""
         try:
             coin_info = await self.search_cg(token)
             return (coin_info['platforms'][f'{await self.search_cg_platform()}']
                     if coin_info is not None else None)
         except Exception as e:
-            self.logger.error(" search_cg_contract: %s", e)
+            self.logger.error(" search_cg_contract: {}", e)
             return
 
     async def get_token_address(self, token_list_url, symbol):
         """Given a token symbol and json tokenlist, get token address"""
         token_list = await get(token_list_url)
         token_search = token_list['tokens']
         for keyval in token_search:
```

### Comparing `dxsp-4.1.2/dxsp/utils/explorer_utils.py` & `dxsp-4.2.0/dxsp/utils/explorer_utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-4.1.2/pyproject.toml` & `dxsp-4.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "4.1.2"
+version = "4.2.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
@@ -18,21 +18,22 @@
 "Changelog" =  "https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/dxsp/discussions"
 "Issues" =  "https://github.com/mraniki/dxsp/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
+loguru = "^0.7.0"
 web3 = "^6.4.0"
 pycoingecko = "^3.1.0"
 uniswap-python = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^8.0.2"
-ruff = "^0.0.279"
+ruff = "^0.0.280"
   
 [tool.ruff]
 select = [
   "E",  # pycodestyle
   "F",  # pyflakes
   "I",  # isort
 ]
@@ -43,14 +44,15 @@
 ignore = ["F401"]
 format = "github"
 fixable = ["ALL"]
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 eth_tester = "^0.9.0b2"
 
@@ -67,14 +69,15 @@
     "examples/*",
     "docs/*",
     "*/config.py"
 ]
 
 
 
+
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.0.0"
 sphinx_bootstrap_theme = "^0.8.1"
 sphinx-autoapi = "^2.1.1"
```

### Comparing `dxsp-4.1.2/PKG-INFO` & `dxsp-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 4.1.2
+Version: 4.2.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pycoingecko (>=3.1.0,<4.0.0)
 Requires-Dist: uniswap-python (>=0.7.0,<0.8.0)
 Requires-Dist: web3 (>=6.4.0,<7.0.0)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: dxsp Version: 4.1.2 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 4.2.0 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
-(>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
-uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst Project-
-URL: Issues, https://github.com/mraniki/dxsp/issues Project-URL: Support,
-https://github.com/mraniki/dxsp/discussions Description-Content-Type: text/
-markdown
+(>=3.1.12,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist:
+pycoingecko (>=3.1.0,<4.0.0) Requires-Dist: uniswap-python (>=0.7.0,<0.8.0)
+Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-URL: Changelog, https://
+github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst Project-URL: Issues, https://
+github.com/mraniki/dxsp/issues Project-URL: Support, https://github.com/
+mraniki/dxsp/discussions Description-Content-Type: text/markdown
 [https://img.shields.io/badge/Wiki-%23000000.svg?style=for-
 the-badge&logo=wikipedia&logoColor=white]
 [https://img.shields.io/badge/github-
 %23000000.svg?style=for-the-
 badge&logo=github&logoColor=white] [https://img.shields.io/
 docker/pulls/mraniki/tt?style=for-the-badge]                       [Logo]
 [https://img.shields.io/badge/tips-000000?style=for-the-
```


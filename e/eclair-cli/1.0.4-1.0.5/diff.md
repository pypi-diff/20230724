# Comparing `tmp/eclair-cli-1.0.4.tar.gz` & `tmp/eclair-cli-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eclair-cli-1.0.4.tar", last modified: Sun Jul 23 22:43:26 2023, max compression
+gzip compressed data, was "eclair-cli-1.0.5.tar", last modified: Sun Jul 23 22:46:12 2023, max compression
```

## Comparing `eclair-cli-1.0.4.tar` & `eclair-cli-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-23 22:43:26.951424 eclair-cli-1.0.4/
--rw-r--r--   0 abhinavmir   (501) staff       (20)     6405 2023-07-23 22:43:26.951284 eclair-cli-1.0.4/PKG-INFO
--rw-r--r--   0 abhinavmir   (501) staff       (20)     6129 2023-07-23 22:43:06.000000 eclair-cli-1.0.4/README.md
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-23 22:43:26.949609 eclair-cli-1.0.4/eclair_cli.egg-info/
--rw-r--r--   0 abhinavmir   (501) staff       (20)     6405 2023-07-23 22:43:26.000000 eclair-cli-1.0.4/eclair_cli.egg-info/PKG-INFO
--rw-r--r--   0 abhinavmir   (501) staff       (20)      333 2023-07-23 22:43:26.000000 eclair-cli-1.0.4/eclair_cli.egg-info/SOURCES.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)        1 2023-07-23 22:43:26.000000 eclair-cli-1.0.4/eclair_cli.egg-info/dependency_links.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       54 2023-07-23 22:43:26.000000 eclair-cli-1.0.4/eclair_cli.egg-info/entry_points.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       12 2023-07-23 22:43:26.000000 eclair-cli-1.0.4/eclair_cli.egg-info/requires.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)        4 2023-07-23 22:43:26.000000 eclair-cli-1.0.4/eclair_cli.egg-info/top_level.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       38 2023-07-23 22:43:26.951465 eclair-cli-1.0.4/setup.cfg
--rw-r--r--   0 abhinavmir   (501) staff       (20)      756 2023-07-23 22:43:23.000000 eclair-cli-1.0.4/setup.py
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-23 22:43:26.950957 eclair-cli-1.0.4/src/
--rw-r--r--   0 abhinavmir   (501) staff       (20)     4560 2023-07-17 15:40:38.000000 eclair-cli-1.0.4/src/ABI_class.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)        0 2023-07-20 16:30:21.000000 eclair-cli-1.0.4/src/__init__.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)      355 2023-07-08 15:29:28.000000 eclair-cli-1.0.4/src/get_all_files.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)     3555 2023-07-22 13:37:11.000000 eclair-cli-1.0.4/src/main.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)      416 2023-07-11 18:11:51.000000 eclair-cli-1.0.4/src/sol_to_json.py
--rw-r--r--   0 abhinavmir   (501) staff       (20)    10985 2023-07-22 11:31:45.000000 eclair-cli-1.0.4/src/templating_logic.py
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-23 22:46:12.630049 eclair-cli-1.0.5/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     6638 2023-07-23 22:46:12.629897 eclair-cli-1.0.5/PKG-INFO
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     6362 2023-07-23 22:45:20.000000 eclair-cli-1.0.5/README.md
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-23 22:46:12.628053 eclair-cli-1.0.5/eclair_cli.egg-info/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     6638 2023-07-23 22:46:12.000000 eclair-cli-1.0.5/eclair_cli.egg-info/PKG-INFO
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      333 2023-07-23 22:46:12.000000 eclair-cli-1.0.5/eclair_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)        1 2023-07-23 22:46:12.000000 eclair-cli-1.0.5/eclair_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       54 2023-07-23 22:46:12.000000 eclair-cli-1.0.5/eclair_cli.egg-info/entry_points.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       12 2023-07-23 22:46:12.000000 eclair-cli-1.0.5/eclair_cli.egg-info/requires.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)        4 2023-07-23 22:46:12.000000 eclair-cli-1.0.5/eclair_cli.egg-info/top_level.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       38 2023-07-23 22:46:12.630094 eclair-cli-1.0.5/setup.cfg
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      756 2023-07-23 22:46:02.000000 eclair-cli-1.0.5/setup.py
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-23 22:46:12.629528 eclair-cli-1.0.5/src/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     4560 2023-07-17 15:40:38.000000 eclair-cli-1.0.5/src/ABI_class.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)        0 2023-07-20 16:30:21.000000 eclair-cli-1.0.5/src/__init__.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      355 2023-07-08 15:29:28.000000 eclair-cli-1.0.5/src/get_all_files.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     3555 2023-07-22 13:37:11.000000 eclair-cli-1.0.5/src/main.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      416 2023-07-11 18:11:51.000000 eclair-cli-1.0.5/src/sol_to_json.py
+-rw-r--r--   0 abhinavmir   (501) staff       (20)    10985 2023-07-22 11:31:45.000000 eclair-cli-1.0.5/src/templating_logic.py
```

### Comparing `eclair-cli-1.0.4/PKG-INFO` & `eclair-cli-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eclair-cli
-Version: 1.0.4
+Version: 1.0.5
 Summary: A tool to create library wrappers for Blockchain Business Logic code.
 Home-page: https://github.com/abhinavmir/eclair
 Author: August Radjoe
 Author-email: atg271@gmail.com
 Description-Content-Type: text/markdown
 
 # Eclair CLI Tool
@@ -47,28 +47,55 @@
 
 ```bash
 eclair wrap
 ```
 
 This will process Solidity files found in the `contracts` directory of your project, generate an ABI for each contract, and then generate a Python class for each ABI in the `wrappers` directory.
 
+
+## Configuration
+
+Eclair's behavior can be customized via the `eclair.config.json` file in your project directory. This file is created when you initialize a project and includes a number of settings:
+
+- `run_compile`: Whether to compile the Solidity files before processing (default is `true`).
+
+- `constructor_args`: Arguments to be passed to the contract constructor when deploying.
+
+- `network_name`: Network to deploy to (e.g., `http://example.com`).
+
+- `private_key`: Your private key for signing transactions.
+
+- `abi_path`: Path to the ABI file for the contract.
+
+- `from_address`: Your address (will be used as the sender of transactions).
+
+- `gas`: Gas limit for transactions.
+
+- `gas_price`: Gas price for transactions.
+
+- `nonce`: Nonce for transactions.
+
+- `output_directory`: Directory to output the Python wrapper classes to (default is `wrappers`).
+
 ### Example
 
 ```solidity
 // SPDX-License-Identifier: MIT
 pragma solidity ^0.8.6;
 
 contract HelloWorld {
     string public greet = "Hello, World!";
 
     function sayHello() public view returns (string memory) {
         return greet;
     }
 }
 ```
+
+Will generate the following Python wrapper:
 ```python
 
 import os
 import json
 from typing import Dict, Tuple
 from web3 import Web3
 
@@ -151,42 +178,26 @@
     def execute_transaction_greet(self) -> (str):
         return self.execute_transaction('greet')
     
     def execute_transaction_sayHello(self) -> (str):
         return self.execute_transaction('sayHello')
 ```
 
-## Configuration
-
-Eclair's behavior can be customized via the `eclair.config.json` file in your project directory. This file is created when you initialize a project and includes a number of settings:
-
-- `run_compile`: Whether to compile the Solidity files before processing (default is `true`).
-
-- `constructor_args`: Arguments to be passed to the contract constructor when deploying.
-
-- `network_name`: Network to deploy to (e.g., `http://example.com`).
-
-- `private_key`: Your private key for signing transactions.
-
-- `abi_path`: Path to the ABI file for the contract.
-
-- `from_address`: Your address (will be used as the sender of transactions).
-
-- `gas`: Gas limit for transactions.
-
-- `gas_price`: Gas price for transactions.
-
-- `nonce`: Nonce for transactions.
-
-- `output_directory`: Directory to output the Python wrapper classes to (default is `wrappers`).
-
 ## Contributing
 
 Contributions to Eclair are welcome! Please read our contributing guidelines for how to proceed.
 
+## Todos
+
+- [] Support Rust
+- [] Support JavaScript
+- [] Write extensive tests
+- [] Allow for rudiementary test generation
+- [] Allow for advanced wrapper customisation from config file
+
 ## License
 
 Eclair is released under the MIT License. See the LICENSE file for more details.
 
 ## Contact
 
 If you have any issues or feature requests, please open an issue on the Eclair GitHub page. For other inquiries, you can reach out ioc.exchange/@formalcurryfication ~!
```

### Comparing `eclair-cli-1.0.4/README.md` & `eclair-cli-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,28 +38,55 @@
 
 ```bash
 eclair wrap
 ```
 
 This will process Solidity files found in the `contracts` directory of your project, generate an ABI for each contract, and then generate a Python class for each ABI in the `wrappers` directory.
 
+
+## Configuration
+
+Eclair's behavior can be customized via the `eclair.config.json` file in your project directory. This file is created when you initialize a project and includes a number of settings:
+
+- `run_compile`: Whether to compile the Solidity files before processing (default is `true`).
+
+- `constructor_args`: Arguments to be passed to the contract constructor when deploying.
+
+- `network_name`: Network to deploy to (e.g., `http://example.com`).
+
+- `private_key`: Your private key for signing transactions.
+
+- `abi_path`: Path to the ABI file for the contract.
+
+- `from_address`: Your address (will be used as the sender of transactions).
+
+- `gas`: Gas limit for transactions.
+
+- `gas_price`: Gas price for transactions.
+
+- `nonce`: Nonce for transactions.
+
+- `output_directory`: Directory to output the Python wrapper classes to (default is `wrappers`).
+
 ### Example
 
 ```solidity
 // SPDX-License-Identifier: MIT
 pragma solidity ^0.8.6;
 
 contract HelloWorld {
     string public greet = "Hello, World!";
 
     function sayHello() public view returns (string memory) {
         return greet;
     }
 }
 ```
+
+Will generate the following Python wrapper:
 ```python
 
 import os
 import json
 from typing import Dict, Tuple
 from web3 import Web3
 
@@ -142,42 +169,26 @@
     def execute_transaction_greet(self) -> (str):
         return self.execute_transaction('greet')
     
     def execute_transaction_sayHello(self) -> (str):
         return self.execute_transaction('sayHello')
 ```
 
-## Configuration
-
-Eclair's behavior can be customized via the `eclair.config.json` file in your project directory. This file is created when you initialize a project and includes a number of settings:
-
-- `run_compile`: Whether to compile the Solidity files before processing (default is `true`).
-
-- `constructor_args`: Arguments to be passed to the contract constructor when deploying.
-
-- `network_name`: Network to deploy to (e.g., `http://example.com`).
-
-- `private_key`: Your private key for signing transactions.
-
-- `abi_path`: Path to the ABI file for the contract.
-
-- `from_address`: Your address (will be used as the sender of transactions).
-
-- `gas`: Gas limit for transactions.
-
-- `gas_price`: Gas price for transactions.
-
-- `nonce`: Nonce for transactions.
-
-- `output_directory`: Directory to output the Python wrapper classes to (default is `wrappers`).
-
 ## Contributing
 
 Contributions to Eclair are welcome! Please read our contributing guidelines for how to proceed.
 
+## Todos
+
+- [] Support Rust
+- [] Support JavaScript
+- [] Write extensive tests
+- [] Allow for rudiementary test generation
+- [] Allow for advanced wrapper customisation from config file
+
 ## License
 
 Eclair is released under the MIT License. See the LICENSE file for more details.
 
 ## Contact
 
 If you have any issues or feature requests, please open an issue on the Eclair GitHub page. For other inquiries, you can reach out ioc.exchange/@formalcurryfication ~!
```

### Comparing `eclair-cli-1.0.4/eclair_cli.egg-info/PKG-INFO` & `eclair-cli-1.0.5/eclair_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eclair-cli
-Version: 1.0.4
+Version: 1.0.5
 Summary: A tool to create library wrappers for Blockchain Business Logic code.
 Home-page: https://github.com/abhinavmir/eclair
 Author: August Radjoe
 Author-email: atg271@gmail.com
 Description-Content-Type: text/markdown
 
 # Eclair CLI Tool
@@ -47,28 +47,55 @@
 
 ```bash
 eclair wrap
 ```
 
 This will process Solidity files found in the `contracts` directory of your project, generate an ABI for each contract, and then generate a Python class for each ABI in the `wrappers` directory.
 
+
+## Configuration
+
+Eclair's behavior can be customized via the `eclair.config.json` file in your project directory. This file is created when you initialize a project and includes a number of settings:
+
+- `run_compile`: Whether to compile the Solidity files before processing (default is `true`).
+
+- `constructor_args`: Arguments to be passed to the contract constructor when deploying.
+
+- `network_name`: Network to deploy to (e.g., `http://example.com`).
+
+- `private_key`: Your private key for signing transactions.
+
+- `abi_path`: Path to the ABI file for the contract.
+
+- `from_address`: Your address (will be used as the sender of transactions).
+
+- `gas`: Gas limit for transactions.
+
+- `gas_price`: Gas price for transactions.
+
+- `nonce`: Nonce for transactions.
+
+- `output_directory`: Directory to output the Python wrapper classes to (default is `wrappers`).
+
 ### Example
 
 ```solidity
 // SPDX-License-Identifier: MIT
 pragma solidity ^0.8.6;
 
 contract HelloWorld {
     string public greet = "Hello, World!";
 
     function sayHello() public view returns (string memory) {
         return greet;
     }
 }
 ```
+
+Will generate the following Python wrapper:
 ```python
 
 import os
 import json
 from typing import Dict, Tuple
 from web3 import Web3
 
@@ -151,42 +178,26 @@
     def execute_transaction_greet(self) -> (str):
         return self.execute_transaction('greet')
     
     def execute_transaction_sayHello(self) -> (str):
         return self.execute_transaction('sayHello')
 ```
 
-## Configuration
-
-Eclair's behavior can be customized via the `eclair.config.json` file in your project directory. This file is created when you initialize a project and includes a number of settings:
-
-- `run_compile`: Whether to compile the Solidity files before processing (default is `true`).
-
-- `constructor_args`: Arguments to be passed to the contract constructor when deploying.
-
-- `network_name`: Network to deploy to (e.g., `http://example.com`).
-
-- `private_key`: Your private key for signing transactions.
-
-- `abi_path`: Path to the ABI file for the contract.
-
-- `from_address`: Your address (will be used as the sender of transactions).
-
-- `gas`: Gas limit for transactions.
-
-- `gas_price`: Gas price for transactions.
-
-- `nonce`: Nonce for transactions.
-
-- `output_directory`: Directory to output the Python wrapper classes to (default is `wrappers`).
-
 ## Contributing
 
 Contributions to Eclair are welcome! Please read our contributing guidelines for how to proceed.
 
+## Todos
+
+- [] Support Rust
+- [] Support JavaScript
+- [] Write extensive tests
+- [] Allow for rudiementary test generation
+- [] Allow for advanced wrapper customisation from config file
+
 ## License
 
 Eclair is released under the MIT License. See the LICENSE file for more details.
 
 ## Contact
 
 If you have any issues or feature requests, please open an issue on the Eclair GitHub page. For other inquiries, you can reach out ioc.exchange/@formalcurryfication ~!
```

### Comparing `eclair-cli-1.0.4/setup.py` & `eclair-cli-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the content of the README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='eclair-cli',
-    version='1.0.4',
+    version='1.0.5',
     author='August Radjoe',
     author_email='atg271@gmail.com',
     description='A tool to create library wrappers for Blockchain Business Logic code.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['src'],
     entry_points={
```

### Comparing `eclair-cli-1.0.4/src/ABI_class.py` & `eclair-cli-1.0.5/src/ABI_class.py`

 * *Files identical despite different names*

### Comparing `eclair-cli-1.0.4/src/main.py` & `eclair-cli-1.0.5/src/main.py`

 * *Files identical despite different names*

### Comparing `eclair-cli-1.0.4/src/templating_logic.py` & `eclair-cli-1.0.5/src/templating_logic.py`

 * *Files identical despite different names*


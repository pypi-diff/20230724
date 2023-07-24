# Comparing `tmp/chainbench-0.4.0.tar.gz` & `tmp/chainbench-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.4.0.tar", max compression
+gzip compressed data, was "chainbench-0.4.1.tar", max compression
```

## Comparing `chainbench-0.4.0.tar` & `chainbench-0.4.1.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0    11357 2023-07-14 03:10:04.505115 chainbench-0.4.0/LICENSE
--rw-r--r--   0        0        0     8428 2023-07-14 03:10:04.505115 chainbench-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/__main__.py
--rw-r--r--   0        0        0     8455 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/main.py
--rw-r--r--   0        0        0        0 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     3681 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/avalanche/general.py
--rw-r--r--   0        0        0     2777 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/bsc/general.py
--rw-r--r--   0        0        0     2987 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/ethereum/general.py
--rw-r--r--   0        0        0      410 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/evm/get_logs.py
--rw-r--r--   0        0        0     4234 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/evm/heavy.py
--rw-r--r--   0        0        0     1711 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/evm/light.py
--rw-r--r--   0        0        0     1922 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/oasis/general.py
--rw-r--r--   0        0        0     2919 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/profile/polygon/general.py
--rw-r--r--   0        0        0      168 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     5356 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/test_data/base.py
--rw-r--r--   0        0        0      166 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/test_data/dummy.py
--rw-r--r--   0        0        0     3497 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/test_data/evm.py
--rw-r--r--   0        0        0        0 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/user/__init__.py
--rw-r--r--   0        0        0     3837 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/user/base.py
--rw-r--r--   0        0        0     2873 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/user/evm.py
--rw-r--r--   0        0        0        0 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/__init__.py
--rw-r--r--   0        0        0     3907 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/cli.py
--rw-r--r--   0        0        0     2511 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/event.py
--rw-r--r--   0        0        0     3436 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/monitor.py
--rw-r--r--   0        0        0     3463 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/notify.py
--rw-r--r--   0        0        0      863 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/rng.py
--rw-r--r--   0        0        0      279 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/rpc.py
--rw-r--r--   0        0        0      438 2023-07-14 03:10:04.505115 chainbench-0.4.0/chainbench/util/timer.py
--rw-r--r--   0        0        0      895 2023-07-14 03:10:04.505115 chainbench-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     9033 1970-01-01 00:00:00.000000 chainbench-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-21 10:49:59.513181 chainbench-0.4.1/LICENSE
+-rw-r--r--   0        0        0     8503 2023-07-21 10:49:59.513181 chainbench-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/__main__.py
+-rw-r--r--   0        0        0     8576 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/main.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     3681 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/profile/avalanche/general.py
+-rw-r--r--   0        0        0     2777 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/profile/bsc/general.py
+-rw-r--r--   0        0        0     2987 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/profile/ethereum/general.py
+-rw-r--r--   0        0        0      410 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/profile/evm/get_logs.py
+-rw-r--r--   0        0        0     4234 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/profile/evm/heavy.py
+-rw-r--r--   0        0        0     1711 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/profile/evm/light.py
+-rw-r--r--   0        0        0     1922 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/profile/oasis/general.py
+-rw-r--r--   0        0        0     2919 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/profile/polygon/general.py
+-rw-r--r--   0        0        0     3581 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/profile/solana/general.py
+-rw-r--r--   0        0        0      225 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     6564 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/test_data/base.py
+-rw-r--r--   0        0        0      166 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/test_data/dummy.py
+-rw-r--r--   0        0        0     3814 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0     3609 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/test_data/solana.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     3733 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/user/base.py
+-rw-r--r--   0        0        0     2835 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/user/evm.py
+-rw-r--r--   0        0        0     4887 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/user/solana.py
+-rw-r--r--   0        0        0        0 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     4097 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/util/cli.py
+-rw-r--r--   0        0        0     4063 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/util/event.py
+-rw-r--r--   0        0        0     2392 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/util/monitor.py
+-rw-r--r--   0        0        0     3449 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/util/notify.py
+-rw-r--r--   0        0        0      863 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/util/rng.py
+-rw-r--r--   0        0        0      279 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/util/rpc.py
+-rw-r--r--   0        0        0      438 2023-07-21 10:49:59.513181 chainbench-0.4.1/chainbench/util/timer.py
+-rw-r--r--   0        0        0      967 2023-07-21 10:49:59.517181 chainbench-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9190 1970-01-01 00:00:00.000000 chainbench-0.4.1/PKG-INFO
```

### Comparing `chainbench-0.4.0/LICENSE` & `chainbench-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.4.0/README.md` & `chainbench-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 ## Project Details
 
 Chainbench lets you to easily define profiles for any EVM-compatible chain. 
 You can use not only hard-coded values but also real chain data to generate dynamic call parameters.
 
 Main features:
-- Built-in profiles for Ethereum, Binance Smart Chain, Polygon, Oasis, and Avalanche
+- Built-in profiles for Ethereum, Binance Smart Chain, Polygon, Oasis, Avalanche and Solana
 - Support for custom profiles
 - Dynamic call params generation using real chain data
 - Headless and web UI modes
 
 Check out the [docs](docs/PROFILE.md) for more information about the profile creation.
 
 ## Prerequisites
@@ -100,15 +100,15 @@
 - `-t, --test-time`: Sets the duration of the test to run.
 - `--target`: Specifies the target blockchain node URL that the benchmark will connect to.
 - `--headless`: Runs the benchmark in headless mode, meaning that no graphical user interface (GUI) will be displayed during the test. This is useful for running the test on a remote server or when the GUI is not needed.
 - `--autoquit`: Tells the Chainbench tool to automatically quit after the test has finished. This is useful for running the benchmark in an automated environment where manual intervention is not desired.
 - `--help`: Displays the help message.
 - `--debug-trace-methods`: Enables tasks tagged with debug or trace to be executed
 - `-E, --exclude-tags`: Exclude tasks tagged with custom tags from the test. You may specify this option multiple times --help Show this message and exit.
-
+- `--use-recent-blocks`: Use recent blocks for test data generation.
 You may also run `chainbench start --help` for the full list of parameters and flags.
 
 ### Profiles
 Default profiles are located in the [`profile`](chainbench/profile) directory. For a tutorial on how to create custom profiles, please refer to [this document](docs/PROFILE.md).
 
 You can also use the `-d` or `--profile-dir` flag to specify a custom directory with profiles. For example:
 ```shell
```

### Comparing `chainbench-0.4.0/chainbench/main.py` & `chainbench-0.4.1/chainbench/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,36 +52,26 @@
 @click.option(
     "-p",
     "--profile",
     default=DEFAULT_PROFILE,
     help="Profile to run",
     show_default=True,
 )
-@click.option(
-    "-d", "--profile-dir", default=None, type=click.Path(), help="Profile directory"
-)
-@click.option(
-    "-H", "--host", default=MASTER_HOST, help="Host to run on", show_default=True
-)
-@click.option(
-    "-P", "--port", default=MASTER_PORT, help="Port to run on", show_default=True
-)
+@click.option("-d", "--profile-dir", default=None, type=click.Path(), help="Profile directory")
+@click.option("-H", "--host", default=MASTER_HOST, help="Host to run on", show_default=True)
+@click.option("-P", "--port", default=MASTER_PORT, help="Port to run on", show_default=True)
 @click.option(
     "-w",
     "--workers",
     default=WORKER_COUNT,
     help="Number of workers to run",
     show_default=True,
 )
-@click.option(
-    "-t", "--test-time", default=TEST_TIME, help="Test time", show_default=True
-)
-@click.option(
-    "-u", "--users", default=USERS, help="Target number of users", show_default=True
-)
+@click.option("-t", "--test-time", default=TEST_TIME, help="Test time", show_default=True)
+@click.option("-u", "--users", default=USERS, help="Target number of users", show_default=True)
 @click.option(
     "-r",
     "--spawn-rate",
     default=SPAWN_RATE,
     help="Number of users spawned per second",
     show_default=True,
 )
@@ -112,34 +102,28 @@
     is_flag=True,
     help="Enable tasks tagged with debug or trace to be executed",
 )
 @click.option(
     "-E",
     "--exclude-tags",
     default=[],
-    help="Exclude tasks tagged with custom tags from the test. "
-    "You may specify this option multiple times",
+    help="Exclude tasks tagged with custom tags from the test. " "You may specify this option multiple times",
     multiple=True,
 )
-@click.option(
-    "--timescale", is_flag=True, help="Export data to PG with timescale extension"
-)
-@click.option(
-    "--pg-host", default=None, help="Hostname of PG instance with timescale extension"
-)
+@click.option("--timescale", is_flag=True, help="Export data to PG with timescale extension")
+@click.option("--pg-host", default=None, help="Hostname of PG instance with timescale extension")
 @click.option(
     "--pg-port",
     default=5432,
     help="Port of PG instance with timescale extension",
     show_default=True,
 )
-@click.option(
-    "--pg-username", default="postgres", help="PG username", show_default=True
-)
+@click.option("--pg-username", default="postgres", help="PG username", show_default=True)
 @click.option("--pg-password", default=None, help="PG password")
+@click.option("--use-recent-blocks", is_flag=True, help="Uses recent blocks for test data")
 @click.pass_context
 def start(
     ctx: click.Context,
     profile: str,
     profile_dir: Path | None,
     host: str,
     port: int,
@@ -158,30 +142,29 @@
     debug_trace_methods: bool,
     exclude_tags: list[str],
     timescale: bool,
     pg_host: str | None,
     pg_port: int,
     pg_username: str,
     pg_password: str | None,
+    use_recent_blocks: bool,
 ):
     if notify:
         click.echo(f"Notify when test is finished using topic: {notify}")
         notifier = Notifier(topic=notify)
     else:
         notifier = NoopNotifier()
 
     ctx.obj.notifier = notifier
 
     if headless and target is None:
         click.echo("Target is required when running in headless mode")
         sys.exit(1)
 
-    if timescale and any(
-        pg_arg is None for pg_arg in (pg_host, pg_port, pg_username, pg_password)
-    ):
+    if timescale and any(pg_arg is None for pg_arg in (pg_host, pg_port, pg_username, pg_password)):
         click.echo(
             "PG connection parameters are required "
             "when --timescale flag is used: pg_host, pg_port, pg_username, pg_password"
         )
         sys.exit(1)
 
     if not profile_dir:
@@ -193,17 +176,15 @@
         click.echo(f"Profile file {profile_path} does not exist")
         sys.exit(1)
 
     results_dir = Path(results_dir).resolve()
 
     click.echo(f"Results directory: {results_dir}")
 
-    results_path = ensure_results_dir(
-        profile=profile, parent_dir=results_dir, run_id=run_id
-    )
+    results_path = ensure_results_dir(profile=profile, parent_dir=results_dir, run_id=run_id)
 
     click.echo(f"Results will be saved to {results_path}")
 
     custom_exclude_tags: list[str] = []
     if exclude_tags:
         for tag in exclude_tags:
             custom_exclude_tags.append(tag)
@@ -226,14 +207,15 @@
         target=target,
         exclude_tags=custom_exclude_tags,
         timescale=timescale,
         pg_host=pg_host,
         pg_port=pg_port,
         pg_username=pg_username,
         pg_password=pg_password,
+        use_recent_blocks=use_recent_blocks,
     )
     if headless:
         click.echo(f"Starting master in headless mode for {profile}")
     else:
         click.echo(f"Starting master for {profile}")
 
     is_posix = os.name == "posix"
@@ -255,14 +237,15 @@
             log_level=log_level,
             exclude_tags=custom_exclude_tags,
             timescale=timescale,
             pg_host=pg_host,
             pg_port=pg_port,
             pg_username=pg_username,
             pg_password=pg_password,
+            use_recent_blocks=use_recent_blocks,
         )
         worker_args = shlex.split(worker_command, posix=is_posix)
         worker_process = subprocess.Popen(worker_args)
         ctx.obj.workers.append(worker_process)
         click.echo(f"Starting worker {worker_id + 1} for {profile}")
     if headless:
         click.echo(f"Running test in headless mode for {profile}")
@@ -289,14 +272,12 @@
         process.join()
 
     if autoquit:
         ctx.obj.master.wait()
         click.echo("Quitting...")
         ctx.obj.master.terminate()
 
-    ctx.obj.notifier.notify(
-        title="Test finished", message=f"Test finished for {profile}", tags=["tada"]
-    )
+    ctx.obj.notifier.notify(title="Test finished", message=f"Test finished for {profile}", tags=["tada"])
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `chainbench-0.4.0/chainbench/profile/avalanche/general.py` & `chainbench-0.4.1/chainbench/profile/avalanche/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.4.0/chainbench/profile/bsc/general.py` & `chainbench-0.4.1/chainbench/profile/bsc/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.4.0/chainbench/profile/ethereum/general.py` & `chainbench-0.4.1/chainbench/profile/ethereum/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.4.0/chainbench/profile/evm/heavy.py` & `chainbench-0.4.1/chainbench/profile/evm/heavy.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.4.0/chainbench/profile/evm/light.py` & `chainbench-0.4.1/chainbench/profile/evm/light.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.4.0/chainbench/profile/oasis/general.py` & `chainbench-0.4.1/chainbench/profile/oasis/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.4.0/chainbench/profile/polygon/general.py` & `chainbench-0.4.1/chainbench/profile/polygon/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.4.0/chainbench/test_data/base.py` & `chainbench-0.4.1/chainbench/test_data/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import json
 import logging
 import typing as t
+from argparse import Namespace
 from dataclasses import dataclass, field
 from secrets import token_hex
 
 import httpx
 from gevent.lock import Semaphore as GeventSemaphore
 
 from chainbench.util.rng import RNG, get_rng
@@ -25,14 +27,32 @@
     start_block_number: BlockNumber = 0
     end_block_number: BlockNumber = 0
     blocks: Blocks = field(default_factory=list)
     txs: Txs = field(default_factory=list)
     tx_hashes: TxHashes = field(default_factory=list)
     accounts: Accounts = field(default_factory=list)
 
+    def to_json(self):
+        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
+
+    def from_json(self, json_data):
+        data = json.loads(json_data)
+        self.start_block_number = data["start_block_number"]
+        self.end_block_number = data["end_block_number"]
+        self.blocks = data["blocks"]
+        self.txs = data["txs"]
+        self.tx_hashes = data["tx_hashes"]
+        self.accounts = data["accounts"]
+
+
+class ChainInfo(t.TypedDict):
+    name: str
+    start_block: int
+    end_block: int
+
 
 class BaseTestData:
     def __init__(self, rpc_version: str = "2.0"):
         self._logger = logging.getLogger(__name__)
         self._host: str | None = None
         self._client: httpx.Client = httpx.Client()
         self._rpc_version = rpc_version
@@ -40,30 +60,37 @@
         self._lock = GeventSemaphore()
         self._logger.debug("Locking")
         self._lock.acquire()
         self._logger.debug("Locked")
 
         self._data: BlockchainData | None = None
 
-    def update(self, host_url: str):
+    def update(self, host_url: str, parsed_options: Namespace) -> BlockchainData:
         self._logger.info("Updating data")
         self._host = host_url
         self._logger.debug("Host: %s", self._host)
-        data = self._get_init_data()
+        data = self._get_init_data(parsed_options)
         self._logger.info("Data fetched")
         self._logger.debug("Data: %s", data)
         self._data = data
         self._logger.info("Data updated. Releasing lock")
         self._lock.release()
         self._logger.info("Lock released")
         return data
 
-    def _get_init_data(self) -> BlockchainData:
+    def _get_init_data(self, parsed_options) -> BlockchainData:
         raise NotImplementedError
 
+    def init_data_from_json(self, json_data: str):
+        self._data = BlockchainData()
+        self._data.from_json(json_data)
+        self._logger.info("Data updated. Releasing lock")
+        self._lock.release()
+        self._logger.info("Lock released")
+
     @property
     def initialized(self) -> bool:
         return self._data is not None
 
     @property
     def host(self) -> str:
         if self._host is None:
@@ -74,14 +101,26 @@
     @property
     def data(self) -> BlockchainData:
         if self._data is None:
             raise ValueError("Data is not initialized")
 
         return self._data
 
+    @staticmethod
+    def _parse_hex_to_int(value: str) -> int:
+        return int(value, 16)
+
+    @staticmethod
+    def _append_if_not_none(data, val):
+        if val is not None:
+            if isinstance(data, list):
+                data.append(val)
+            elif isinstance(data, set):
+                data.add(val)
+
     def _make_body(self, method: str, params: list[t.Any] | None = None):
         if params is None:
             params = []
 
         return {
             "jsonrpc": self._rpc_version,
             "method": method,
@@ -94,17 +133,15 @@
             params = []
 
         response = self._client.post(
             self.host,
             json=self._make_body(method, params),
         )
 
-        self._logger.debug(
-            f"Making call to {self.host} with method {method} and params {params}"
-        )
+        self._logger.debug(f"Making call to {self.host} with method {method} and params {params}")
         self._logger.debug(f"Response: {response.text}")
 
         response.raise_for_status()
 
         # check if response is json
         try:
             data = response.json()
@@ -148,17 +185,15 @@
         return block_hash
 
     def get_random_tx_hash(self, rng: RNG | None = None) -> TxHash:
         if rng is None:
             rng = get_rng()
         return rng.random.choice(self.tx_hashes)
 
-    def get_random_recent_block_number(
-        self, n: int, rng: RNG | None = None
-    ) -> BlockNumber:
+    def get_random_recent_block_number(self, n: int, rng: RNG | None = None) -> BlockNumber:
         if rng is None:
             rng = get_rng()
         return rng.random.randint(
             self.end_block_number - n,
             self.end_block_number,
         )
```

### Comparing `chainbench-0.4.0/chainbench/test_data/evm.py` & `chainbench-0.4.1/chainbench/test_data/solana.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,90 @@
-from typing import Mapping, TypedDict
+from tenacity import retry, stop_after_attempt
 
-from chainbench.test_data.base import BaseTestData, BlockchainData
+from chainbench.test_data.base import BaseTestData, Block, BlockchainData
 from chainbench.util.rng import get_rng
 
 
-class ChainInfo(TypedDict):
-    name: str
-    start_block: int
-    end_block: int
-
-
-class EVMTestData(BaseTestData):
-    TXS_REQUIRED = 50
-    ACCOUNTS_REQUIRED = 100
-    SAVE_LAST_BLOCKS = 100
-
-    CHAIN_INFO: Mapping[int, ChainInfo] = {
-        1: {
-            "name": "ethereum-mainnet",
-            "start_block": 10000000,
-            "end_block": 17000000,
-        },
-        56: {
-            "name": "binance-smart-chain",
-            "start_block": 20000000,
-            "end_block": 29000000,
-        },
-        137: {
-            "name": "polygon-mainnet",
-            "start_block": 35000000,
-            "end_block": 45000000,
-        },
-        26863: {
-            "name": "oasis-mainnet",
-            "start_block": 8000000,
-            "end_block": 14000000,
-        },
-        43114: {
-            "name": "avalanche-mainnet",
-            "start_block": 20000000,
-            "end_block": 32000000,
-        },
-    }
-
-    @staticmethod
-    def _parse_hex_to_int(value: str) -> int:
-        return int(value, 16)
-
-    @staticmethod
-    def _append_if_not_none(data, val):
-        if val is not None:
-            if isinstance(data, list):
-                data.append(val)
-            elif isinstance(data, set):
-                data.add(val)
-
-    def _fetch_chain_id(self) -> int:
-        return self._parse_hex_to_int(self._make_call("eth_chainId"))
-
-    def _fetch_block(
-        self, block_number: int | str, return_txs: bool = True
-    ) -> tuple[int, dict]:
-        if isinstance(block_number, int):
-            block_number = hex(block_number)
-        elif (block_number := block_number.lower()) not in (
-            "latest",
-            "earliest",
-            "pending",
-        ):
-            raise ValueError("Invalid block number")
-        result = self._make_call("eth_getBlockByNumber", [block_number, return_txs])
-        return self._parse_hex_to_int(result["number"]), result
+class SolanaTestData(BaseTestData):
+    TXS_REQUIRED = 100
+    ACCOUNTS_REQUIRED = 200
+    BLOCK_TIME = 0.4
+
+    def _fetch_block(self, block_number: int, return_txs: bool = True) -> dict:
+        if return_txs:
+            transaction_details = "accounts"
+        else:
+            transaction_details = "none"
+        config_object = {
+            "encoding": "json",
+            "transactionDetails": transaction_details,
+            "rewards": False,
+            "maxSupportedTransactionVersion": 0,
+        }
+        try:
+            result = self._make_call("getBlock", [block_number, config_object])
+        except Exception as e:
+            self._logger.error(f"Failed to fetch block {block_number}: {e}")
+            raise e
+        return result
 
-    def _fetch_random_block(self, start, end, return_txs=True) -> tuple[int, dict]:
+    @retry(reraise=True, stop=stop_after_attempt(5))
+    def _fetch_random_block(self, start, end, return_txs=True) -> dict:
         rng = get_rng()
         block_number = rng.random.randint(start, end)
-        return self._fetch_block(block_number, return_txs=return_txs)
+        block = self._fetch_block(block_number, return_txs=return_txs)
+        return block
+
+    def _fetch_latest_slot_number(self):
+        slot = self._make_call("getLatestBlockhash")["context"]["slot"]
+        return slot
+
+    @retry(reraise=True, stop=stop_after_attempt(5))
+    def _fetch_latest_block(self):
+        slot_number = self._fetch_latest_slot_number()
+        latest_block = self._fetch_block(slot_number, return_txs=True)
+        return slot_number, latest_block
+
+    def _fetch_first_available_block(self):
+        block = self._make_call("getFirstAvailableBlock")
+        return block
 
     # get initial data from blockchain
-    def _get_init_data(self) -> BlockchainData:
+    def _get_init_data(self, parsed_options) -> BlockchainData:
         txs: list[dict] = []
         tx_hashes: list[str] = []
         accounts: set[str] = set()
-        blocks = []
-        chain_id = self._fetch_chain_id()
-        start_block_number = self.CHAIN_INFO[chain_id]["start_block"]
-        end_block_number = self.CHAIN_INFO[chain_id]["end_block"]
-
-        while self.TXS_REQUIRED > len(txs) and self.ACCOUNTS_REQUIRED > len(accounts):
-            block_number, block = self._fetch_random_block(
-                start_block_number, end_block_number
-            )
-            blocks.append((block_number, block["hash"]))
+        blocks: list[Block] = []
+        end_block_number, _latest_block = self._fetch_latest_block()
+        start_block_number = self._fetch_first_available_block()
+
+        # factor in run_time and add 10% buffer to ensure blocks used in test data are
+        # not removed from the ledger
+        start_block_number += int((parsed_options.run_time / self.BLOCK_TIME) * 1.1)
+
+        while self.TXS_REQUIRED > len(txs) or self.ACCOUNTS_REQUIRED > len(accounts):
+            if self.ACCOUNTS_REQUIRED > len(accounts) or self.TXS_REQUIRED > len(blocks):
+                return_txs = True
+            else:
+                return_txs = False
+            block = self._fetch_random_block(start_block_number, end_block_number, return_txs)
             for tx in block["transactions"]:
-                self._append_if_not_none(txs, tx)
-                self._append_if_not_none(tx_hashes, tx["hash"])
-                self._append_if_not_none(accounts, tx["from"])
-                self._append_if_not_none(accounts, tx["to"])
+                if self.TXS_REQUIRED > len(txs):
+                    self._append_if_not_none(txs, tx)
+                    self._append_if_not_none(tx_hashes, tx["transaction"]["signatures"][0])
+                    for account in tx["transaction"]["accountKeys"]:
+                        if (
+                            self.ACCOUNTS_REQUIRED > len(accounts)
+                            and account["pubkey"] != "TokenkegQfeZyiNwAJbNbGKPFXCWuBvf9Ss623VQ5DA"
+                        ):
+                            self._append_if_not_none(accounts, account["pubkey"])
+                        else:
+                            break
 
         return BlockchainData(
             end_block_number=end_block_number,
             start_block_number=start_block_number,
-            blocks=blocks,
+            blocks=[],
             txs=txs,
             tx_hashes=tx_hashes,
             accounts=sorted(list(accounts)),
         )
```

### Comparing `chainbench-0.4.0/chainbench/user/base.py` & `chainbench-0.4.1/chainbench/user/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,15 @@
 
     def check_fatal(self, response: RestResponseContextManager):
         if response.status_code == 401:
             self.logger.critical(f"Unauthorized request to {response.url}")
         elif response.status_code == 404:
             self.logger.critical(f"Not found: {response.url}")
         elif 500 <= response.status_code <= 599:
-            self.logger.critical(
-                f"Got internal server error when requesting {response.url}"
-            )
+            self.logger.critical(f"Got internal server error when requesting {response.url}")
         elif 300 <= response.status_code <= 399:
             self.logger.critical(f"Redirect error: {response.url}")
 
     def check_response(self, response: RestResponseContextManager, name: str):
         """Check the response for errors."""
         if response.status_code != 200:
             self.logger.info(f"Request failed with {response.status_code} code")
@@ -73,33 +71,27 @@
 
         if "jsonrpc" not in response.js:
             self.logger.error(f"Response for {name} is not a JSON-RPC: {response.text}")
             response.failure(f"Response for {name} is not a JSON-RPC")
             raise RescheduleTask()
 
         if "error" in response.js:
-            self.logger.error(
-                f"Response for {name} has a JSON-RPC error: {response.text}"
-            )
+            self.logger.error(f"Response for {name} has a JSON-RPC error: {response.text}")
             if "code" in response.js["error"]:
                 response.failure(
                     f"Response for {name} has a JSON-RPC error {response.js['error']['code']}"  # noqa: E501
                 )
                 raise RescheduleTask()
             response.failure("Unspecified JSON-RPC error")
             raise RescheduleTask()
 
         if not response.js.get("result"):
-            self.logger.error(
-                f"Response for {name} call has no result: {response.text}"
-            )
+            self.logger.error(f"Response for {name} call has no result: {response.text}")
 
-    def make_call(
-        self, method: str, params: list[t.Any] | None = None, name: str | None = None
-    ):
+    def make_call(self, method: str, params: list[t.Any] | None = None, name: str | None = None):
         name = name if name else method
         return self._post(name, data=generate_request(method, params))
 
     def _post(self, name: str, data: t.Optional[dict] = None):
         """Make a JSON-RPC call."""
         with self.rest("POST", self.rpc_path, json=data, name=name) as response:
             self.check_response(response, name=name)
```

### Comparing `chainbench-0.4.0/chainbench/user/evm.py` & `chainbench-0.4.1/chainbench/user/evm.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 class EVMBenchUser(BaseBenchUser):
     abstract = True
     test_data = EVMTestData()
 
     def _get_logs_params_factory(self, rng: RNG):
         return [
             {
-                "fromBlock": hex(
-                    self.test_data.get_random_recent_block_number(20, rng)
-                ),
+                "fromBlock": hex(self.test_data.get_random_recent_block_number(20, rng)),
                 "toBlock": hex(self.test_data.end_block_number),
             }
         ]
 
     def _transaction_by_hash_params_factory(self, rng: RNG):
         return [self.test_data.get_random_tx_hash(rng)]
```

### Comparing `chainbench-0.4.0/chainbench/util/cli.py` & `chainbench-0.4.1/chainbench/util/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     return profile_path
 
 
 def generate_unique_dir_name() -> str:
     return datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
 
 
-def ensure_results_dir(
-    profile: str, parent_dir: Path, run_id: str | None = None
-) -> Path:
+def ensure_results_dir(profile: str, parent_dir: Path, run_id: str | None = None) -> Path:
     if run_id is not None:
         results_dir = (parent_dir / run_id).resolve()
     else:
         results_dir = (parent_dir / profile / generate_unique_dir_name()).resolve()
     if not results_dir.exists():
         results_dir.mkdir(parents=True, exist_ok=True)
 
@@ -42,18 +40,15 @@
 
 def get_timescale_args(
     pg_host: str | None,
     pg_port: int | None,
     pg_username: str | None,
     pg_password: str | None,
 ) -> str:
-    return (
-        f" --timescale --pghost={pg_host} --pgport={pg_port}"
-        f" --pgpassword={pg_password} --pguser={pg_username}"
-    )
+    return f" --timescale --pghost={pg_host} --pgport={pg_port}" f" --pgpassword={pg_password} --pguser={pg_username}"
 
 
 def get_master_command(
     profile_path: Path,
     host: str,
     port: int,
     users: int,
@@ -66,14 +61,15 @@
     target: str | None = None,
     headless: bool = False,
     timescale: bool = False,
     pg_host: str | None = None,
     pg_port: int | None = None,
     pg_username: str | None = None,
     pg_password: str | None = None,
+    use_recent_blocks: bool = False,
 ) -> str:
     """Generate master command."""
     command = (
         f"locust -f {profile_path} --master "
         f"--master-bind-host {host} --master-bind-port {port} "
         f"--web-host {host} "
         f"-u {users} -r {spawn_rate} --run-time {test_time} "
@@ -90,14 +86,16 @@
 
     if headless:
         command += " --headless"
 
     if len(exclude_tags) > 0:
         command += f" --exclude-tags {' '.join(exclude_tags)}"
 
+    if use_recent_blocks:
+        command += " --use-recent-blocks True"
     return command
 
 
 def get_worker_command(
     profile_path: Path,
     host: str,
     port: int,
@@ -108,14 +106,15 @@
     headless: bool = False,
     worker_id: int = 0,
     timescale: bool = False,
     pg_host: str | None = None,
     pg_port: int | None = None,
     pg_username: str | None = None,
     pg_password: str | None = None,
+    use_recent_blocks: bool = False,
 ) -> str:
     """Generate worker command."""
     command = (
         f"locust -f {profile_path} --worker --master-host {host} --master-port {port} "
         f"--logfile {results_path}/worker_{worker_id}.log --loglevel {log_level}"
     )
 
@@ -127,14 +126,16 @@
 
     if headless:
         command += " --headless"
 
     if len(exclude_tags) > 0:
         command += f" --exclude-tags {' '.join(exclude_tags)}"
 
+    if use_recent_blocks:
+        command += " --use-recent-blocks True"
     return command
 
 
 @dataclass
 class ContextData:
     workers: list[subprocess.Popen] = field(default_factory=list)
     master: subprocess.Popen | None = None
```

### Comparing `chainbench-0.4.0/chainbench/util/event.py` & `chainbench-0.4.1/chainbench/util/event.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,29 +4,94 @@
 from locust.runners import MasterRunner, WorkerRunner
 
 from chainbench.util.timer import Timer
 
 logger = logging.getLogger(__name__)
 
 
+def cli_custom_arguments(parser):
+    parser.add_argument(
+        "--use-recent-blocks",
+        type=bool,
+        default=False,
+        help="Use recent blocks as test data",
+    )
+
+
+def setup_test_data(environment, msg, **kwargs):
+    # Fired when the worker receives a message of type 'test_data'
+    test_data = msg.data[0]
+    worker_index = msg.data[1]
+
+    for user in environment.runner.user_classes:
+        if not hasattr(user, "test_data"):
+            continue
+
+        user.test_data.init_data_from_json(test_data[user.__class__.__name__])
+    environment.runner.send_message("acknowledge_data", f"Test data received by worker {worker_index}")
+    logger.info("Test Data received from master")
+
+
+def on_acknowledge(msg, **kwargs):
+    # Fired when the master receives a message of type 'acknowledge_data'
+    print(msg.data)
+
+
+# Listener for the init event
+def on_init(environment, **_kwargs):
+    # It will be called for any runner (master, worker, local)
+    logger.debug("init.add_listener: Init is started")
+    logger.debug("init.add_listener: Environment: %s", environment.runner)
+    logger.debug("init.add_listener: Host: %s", environment.host)
+
+    host_under_test = environment.host or "Default host"
+
+    if not isinstance(environment.runner, MasterRunner):
+        # Print worker details to the log
+        logger.info("I'm a worker. Running tests for %s", host_under_test)
+        environment.runner.register_message("test_data", setup_test_data)
+
+    if not isinstance(environment.runner, WorkerRunner):
+        # Print master details to the log
+        logger.info("I'm a master. Running tests for %s", host_under_test)
+        environment.runner.register_message("acknowledge_data", on_acknowledge)
+
+
 def on_test_start(environment, **_kwargs):
+    test_data = {}
+
     # It will be called for any runner (master, worker, local)
+    if not isinstance(environment.runner, WorkerRunner):
+        logger.info("Initializing test data...")
+        print("Initializing test data...\n")
+        for user in environment.runner.user_classes:
+            if not hasattr(user, "test_data"):
+                continue
+
+            if user.__class__.__name__ not in test_data:
+                user.test_data.update(environment.host, environment.parsed_options)
+                test_data[user.__class__.__name__] = user.test_data.data.to_json()
+
+        logger.info("Test data is ready")
+        for i, worker in enumerate(environment.runner.clients):
+            environment.runner.send_message("test_data", (test_data, i), worker)
+            logger.info(f"Test data is sent to worker {i}")
+
+        # Print master details to the log
+        logger.info(
+            f"Master: test_start.add_listener: The test is started, " f"Environment: {environment.runner}",
+        )
+
     if not isinstance(environment.runner, MasterRunner):
         # Print worker details to the log
         logger.info(
             f"Worker[{environment.runner.worker_index:02d}]: "
             f"The test is started, Environment: {environment.runner}",
         )
         Timer.set_timer(environment.runner.worker_index)
-    else:
-        # Print master details to the log
-        logger.info(
-            f"Master: test_start.add_listener: The test is started, "
-            f"Environment: {environment.runner}",
-        )
 
 
 # Listener for the test stop event
 def on_test_stop(environment, **_kwargs):
     # It will be called for any runner (master, worker, local)
     runner = environment.runner
     if not isinstance(runner, MasterRunner):
@@ -36,36 +101,12 @@
             f"{Timer.get_time_diff(runner.worker_index):>.3f} seconds"
         )
     else:
         # Print master details to the log
         logger.info("Master: The test is stopped")
 
 
-# Listener for the init event
-def on_init(environment, **_kwargs):
-    # It will be called for any runner (master, worker, local)
-    logger.debug("init.add_listener: Init is started")
-    logger.debug("init.add_listener: Environment: %s", environment.runner)
-    logger.debug("init.add_listener: Host: %s", environment.host)
-
-    host_under_test = environment.host or "Default host"
-
-    if isinstance(environment.runner, MasterRunner):
-        # Print master details to the log
-        logger.info("I'm a master. Running tests for %s", host_under_test)
-
-    if isinstance(environment.runner, WorkerRunner):
-        # Print worker details to the log
-        logger.info("I'm a worker. Running tests for %s", host_under_test)
-        logger.info("Initializing test data...")
-        for user in environment.runner.user_classes:
-            if not hasattr(user, "test_data"):
-                continue
-
-            user.test_data.update(environment.host)
-            logger.info("Test data is ready")
-
-
 def setup_event_listeners():
+    events.init_command_line_parser.add_listener(cli_custom_arguments)
     events.test_start.add_listener(on_test_start)
     events.test_stop.add_listener(on_test_stop)
     events.init.add_listener(on_init)
```

### Comparing `chainbench-0.4.0/chainbench/util/notify.py` & `chainbench-0.4.1/chainbench/util/notify.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,17 +76,15 @@
             "headers": self._headers(),
         }
 
 
 class Notifier:
     """A notification service."""
 
-    def __init__(
-        self, topic: str, url: str = DEFAULT_NTFY_SERVER, timeout: int = 30
-    ) -> None:
+    def __init__(self, topic: str, url: str = DEFAULT_NTFY_SERVER, timeout: int = 30) -> None:
         self.topic: str = topic
 
         self.url: str = url
         self.timeout: int = timeout
 
         self.client = httpx.Client(base_url=url, timeout=timeout)
```

### Comparing `chainbench-0.4.0/chainbench/util/rng.py` & `chainbench-0.4.1/chainbench/util/rng.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.4.0/pyproject.toml` & `chainbench-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainbench"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = [
     "Egor Molodik <egor.molodik@chainstack.com>",
     "Erwin Wee <erwin.wee@chainstack.com>"
 ]
 maintainers = ["Erwin Wee <erwin.wee@chainstack.com>"]
 readme = "README.md"
@@ -13,14 +13,16 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = "0.24.0"
 locust = "^2.15.0"
 click = "^8.1.3"
 locust-plugins = "^3.3.0"
 httpcore = "0.17.0"
+tenacity = "^8.2.2"
+psycopg2 = "^2.9.6"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.2.0"
 pre-commit = "^3.2.2"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
@@ -37,9 +39,12 @@
 python_version = "3.10"
 ignore_missing_imports = true
 
 [tool.isort]
 profile = "black"
 
 [tool.flake8]
-max-line-length = 88
+max-line-length = 120
 extend-ignore = ['E203']
+
+[tool.black]
+line-length = 120
```

### Comparing `chainbench-0.4.0/PKG-INFO` & `chainbench-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
 Maintainer: Erwin Wee
 Maintainer-email: erwin.wee@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: httpcore (==0.17.0)
 Requires-Dist: httpx (==0.24.0)
 Requires-Dist: locust (>=2.15.0,<3.0.0)
 Requires-Dist: locust-plugins (>=3.3.0,<4.0.0)
+Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Description-Content-Type: text/markdown
 
 <img width="1200" alt="Labs" src="https://user-images.githubusercontent.com/99700157/213291931-5a822628-5b8a-4768-980d-65f324985d32.png">
 
 <p>
  <h3 align="center">Chainstack is the leading suite of services connecting developers with Web3 infrastructure</h3>
 </p>
@@ -50,15 +52,15 @@
 
 ## Project Details
 
 Chainbench lets you to easily define profiles for any EVM-compatible chain. 
 You can use not only hard-coded values but also real chain data to generate dynamic call parameters.
 
 Main features:
-- Built-in profiles for Ethereum, Binance Smart Chain, Polygon, Oasis, and Avalanche
+- Built-in profiles for Ethereum, Binance Smart Chain, Polygon, Oasis, Avalanche and Solana
 - Support for custom profiles
 - Dynamic call params generation using real chain data
 - Headless and web UI modes
 
 Check out the [docs](docs/PROFILE.md) for more information about the profile creation.
 
 ## Prerequisites
@@ -119,15 +121,15 @@
 - `-t, --test-time`: Sets the duration of the test to run.
 - `--target`: Specifies the target blockchain node URL that the benchmark will connect to.
 - `--headless`: Runs the benchmark in headless mode, meaning that no graphical user interface (GUI) will be displayed during the test. This is useful for running the test on a remote server or when the GUI is not needed.
 - `--autoquit`: Tells the Chainbench tool to automatically quit after the test has finished. This is useful for running the benchmark in an automated environment where manual intervention is not desired.
 - `--help`: Displays the help message.
 - `--debug-trace-methods`: Enables tasks tagged with debug or trace to be executed
 - `-E, --exclude-tags`: Exclude tasks tagged with custom tags from the test. You may specify this option multiple times --help Show this message and exit.
-
+- `--use-recent-blocks`: Use recent blocks for test data generation.
 You may also run `chainbench start --help` for the full list of parameters and flags.
 
 ### Profiles
 Default profiles are located in the [`profile`](chainbench/profile) directory. For a tutorial on how to create custom profiles, please refer to [this document](docs/PROFILE.md).
 
 You can also use the `-d` or `--profile-dir` flag to specify a custom directory with profiles. For example:
 ```shell
```


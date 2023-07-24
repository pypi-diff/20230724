# Comparing `tmp/py_experimenter-1.3.0.tar.gz` & `tmp/py_experimenter-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_experimenter-1.3.0.tar", max compression
+gzip compressed data, was "py_experimenter-1.3.1.tar", max compression
```

## Comparing `py_experimenter-1.3.0.tar` & `py_experimenter-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1183 2023-02-16 12:30:15.046670 py_experimenter-1.3.0/LICENSE
--rw-r--r--   0        0        0     3461 2023-06-23 13:03:20.172030 py_experimenter-1.3.0/README.md
--rw-r--r--   0        0        0        1 2023-02-16 12:30:15.050204 py_experimenter-1.3.0/py_experimenter/__init__.py
--rw-r--r--   0        0        0    15392 2023-06-23 18:02:36.562762 py_experimenter-1.3.0/py_experimenter/database_connector.py
--rw-r--r--   0        0        0     3226 2023-06-23 18:02:36.562916 py_experimenter-1.3.0/py_experimenter/database_connector_lite.py
--rw-r--r--   0        0        0     5099 2023-06-23 18:02:36.563473 py_experimenter-1.3.0/py_experimenter/database_connector_mysql.py
--rw-r--r--   0        0        0      907 2023-04-04 09:33:58.357634 py_experimenter-1.3.0/py_experimenter/exceptions.py
--rw-r--r--   0        0        0      156 2023-02-16 12:30:15.050509 py_experimenter-1.3.0/py_experimenter/experiment_status.py
--rw-r--r--   0        0        0    24341 2023-06-23 18:02:36.563701 py_experimenter-1.3.0/py_experimenter/experimenter.py
--rw-r--r--   0        0        0     5274 2023-06-23 18:02:36.564378 py_experimenter-1.3.0/py_experimenter/result_processor.py
--rw-r--r--   0        0        0    11246 2023-06-23 18:02:36.564714 py_experimenter-1.3.0/py_experimenter/utils.py
--rw-r--r--   0        0        0     1680 2023-06-23 20:03:32.020159 py_experimenter-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4446 1970-01-01 00:00:00.000000 py_experimenter-1.3.0/setup.py
--rw-r--r--   0        0        0     4879 1970-01-01 00:00:00.000000 py_experimenter-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1183 2023-02-16 12:30:15.046670 py_experimenter-1.3.1/LICENSE
+-rw-r--r--   0        0        0     3461 2023-06-23 13:03:20.172030 py_experimenter-1.3.1/README.md
+-rw-r--r--   0        0        0        1 2023-02-16 12:30:15.050204 py_experimenter-1.3.1/py_experimenter/__init__.py
+-rw-r--r--   0        0        0    15499 2023-07-24 14:49:25.879340 py_experimenter-1.3.1/py_experimenter/database_connector.py
+-rw-r--r--   0        0        0     3242 2023-07-24 14:49:25.879560 py_experimenter-1.3.1/py_experimenter/database_connector_lite.py
+-rw-r--r--   0        0        0     5131 2023-07-24 14:49:25.879813 py_experimenter-1.3.1/py_experimenter/database_connector_mysql.py
+-rw-r--r--   0        0        0      965 2023-07-24 14:49:25.879965 py_experimenter-1.3.1/py_experimenter/exceptions.py
+-rw-r--r--   0        0        0      156 2023-02-16 12:30:15.050509 py_experimenter-1.3.1/py_experimenter/experiment_status.py
+-rw-r--r--   0        0        0    25938 2023-07-24 14:49:25.880291 py_experimenter-1.3.1/py_experimenter/experimenter.py
+-rw-r--r--   0        0        0     6808 2023-07-24 14:49:25.880586 py_experimenter-1.3.1/py_experimenter/result_processor.py
+-rw-r--r--   0        0        0    11344 2023-07-24 14:49:25.880811 py_experimenter-1.3.1/py_experimenter/utils.py
+-rw-r--r--   0        0        0     1680 2023-07-24 14:49:25.881086 py_experimenter-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4446 1970-01-01 00:00:00.000000 py_experimenter-1.3.1/setup.py
+-rw-r--r--   0        0        0     4879 1970-01-01 00:00:00.000000 py_experimenter-1.3.1/PKG-INFO
```

### Comparing `py_experimenter-1.3.0/LICENSE` & `py_experimenter-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_experimenter-1.3.0/README.md` & `py_experimenter-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `py_experimenter-1.3.0/py_experimenter/database_connector.py` & `py_experimenter-1.3.1/py_experimenter/database_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from py_experimenter.exceptions import (CreatingTableError, DatabaseConnectionError, EmptyFillDatabaseCallError, NoExperimentsLeftException,
                                         TableHasWrongStructureError)
 from py_experimenter.experiment_status import ExperimentStatus
 
 
 class DatabaseConnector(abc.ABC):
 
-    def __init__(self, config: ConfigParser, use_codecarbon: bool, codecarbon_config: ConfigParser):
+    def __init__(self, config: ConfigParser, use_codecarbon: bool, codecarbon_config: ConfigParser, logger):
+        self.logger = logger
         self.config = config
         self.codecarbon_config = codecarbon_config
         self.table_name = self.config.get('PY_EXPERIMENTER', 'table')
         self.database_name = self.config.get('PY_EXPERIMENTER', 'database')
 
         self.database_credentials = self._extract_credentials()
         self.timestamp_on_result_fields = utils.timestamps_for_result_fields(self.config)
@@ -69,19 +70,19 @@
     def fetchall(self, cursor):
         try:
             return cursor.fetchall()
         except Exception as e:
             raise DatabaseConnectionError(f'error \n{e}\n raised when fetching all rows from database.')
 
     def create_table_if_not_existing(self) -> None:
-        logging.debug("Create table if not exist")
+        self.logger.debug("Create table if not exist")
 
         keyfields = utils.get_keyfields(self.config)
         resultfields = utils.get_resultfields(self.config)
-        if self.timestamp_on_result_fields:
+        if resultfields and self.timestamp_on_result_fields:
             resultfields = utils.add_timestep_result_columns(resultfields)
 
         connection = self.connect()
         cursor = self.cursor(connection)
         if self._table_exists(cursor):
             if not self._table_has_correct_structure(cursor, keyfields + resultfields):
                 raise TableHasWrongStructureError("Keyfields or resultfields from the configuration do not match columns in the existing "
@@ -151,47 +152,47 @@
         pass
 
     @abc.abstractmethod
     def _table_has_correct_structure(self, cursor, typed_fields):
         pass
 
     def fill_table(self, parameters=None, fixed_parameter_combinations=None) -> None:
-        logging.debug("Fill table with parameters.")
+        self.logger.debug("Fill table with parameters.")
         parameters = parameters if parameters is not None else {}
         fixed_parameter_combinations = fixed_parameter_combinations if fixed_parameter_combinations is not None else []
 
         keyfield_names = utils.get_keyfield_names(self.config)
         combinations = utils.combine_fill_table_parameters(keyfield_names, parameters, fixed_parameter_combinations)
 
         if len(combinations) == 0:
             raise EmptyFillDatabaseCallError("No combinations to execute found.")
 
         column_names = list(combinations[0].keys())
-        logging.debug("Getting existing rows.")
+        self.logger.debug("Getting existing rows.")
         existing_rows = set(self._get_existing_rows(column_names))
         time = utils.get_timestamp_representation()
 
         rows_skipped = 0
         rows = []
-        logging.debug("Checking which of the experiments to be inserted already exist.")
+        self.logger.debug("Checking which of the experiments to be inserted already exist.")
         for combination in combinations:
             if self._check_combination_in_existing_rows(combination, existing_rows, keyfield_names):
                 rows_skipped += 1
                 continue
             values = list(combination.values())
             values.append(ExperimentStatus.CREATED.value)
             values.append(time)
             rows.append(values)
 
         if rows:
-            logging.debug(f"Now adding {len(rows)} rows to database. {rows_skipped} rows were skipped.")
+            self.logger.debug(f"Now adding {len(rows)} rows to database. {rows_skipped} rows were skipped.")
             self._write_to_database(rows, column_names + ["status", "creation_date"])
-            logging.info(f"{len(rows)} rows successfully added to database. {rows_skipped} rows were skipped.")
+            self.logger.info(f"{len(rows)} rows successfully added to database. {rows_skipped} rows were skipped.")
         else:
-            logging.info(f"No rows to add. All the {len(combinations)} experiments already exist.")
+            self.logger.info(f"No rows to add. All the {len(combinations)} experiments already exist.")
 
     def _check_combination_in_existing_rows(self, combination, existing_rows, keyfield_names) -> bool:
         def _get_column_values():
             return [combination[keyfield_name] for keyfield_name in keyfield_names]
         return ("[" + " ".join([str(value) for value in _get_column_values()]) + "]") in existing_rows
 
     @abc.abstractmethod
@@ -203,33 +204,34 @@
             experiment_id, description, values = self._pull_open_experiment()
         except IndexError as e:
             raise NoExperimentsLeftException("No experiments left to execute")
         except Exception as e:
             raise DatabaseConnectionError(f'error \n {e} raised. \n Please check if fill_table() was called correctly.')
 
         return experiment_id, dict(zip([i[0] for i in description], *values))
+    
+    @abc.abstractmethod
+    def _pull_open_experiment(self) -> Tuple[int, List, List]:
+        pass
 
-    def _execute_queries(self, connection, cursor) -> Tuple[int, List, List]:
+    def _select_open_experiments_from_db(self, connection, cursor) -> Tuple[int, List, List]:
         order_by = "id"
         time = utils.get_timestamp_representation()
 
         self.execute(cursor, f"SELECT id FROM {self.table_name} WHERE status = 'created' ORDER BY {order_by} LIMIT 1;")
         experiment_id = self.fetchall(cursor)[0][0]
         self.execute(
             cursor, f"UPDATE {self.table_name} SET status = {self._prepared_statement_placeholder}, start_date = {self._prepared_statement_placeholder} WHERE id = {self._prepared_statement_placeholder};", (ExperimentStatus.RUNNING.value, time, experiment_id))
         keyfields = ','.join(utils.get_keyfield_names(self.config))
         self.execute(cursor, f"SELECT {keyfields} FROM {self.table_name} WHERE id = {experiment_id};")
         values = self.fetchall(cursor)
         self.commit(connection)
         description = cursor.description
         return experiment_id, description, values
 
-    @abc.abstractmethod
-    def _pull_open_experiment(self) -> Tuple[int, List, List]:
-        pass
 
     def _write_to_database(self, values: List, columns=List[str]) -> None:
         values_prepared = ','.join([f"({', '.join([self._prepared_statement_placeholder] * len(columns))})"] * len(values))
         values = list(map(lambda x: str(x) if x is not None else x, itertools.chain(*values)))
         stmt = f"INSERT INTO {self.table_name} ({','.join(columns)}) VALUES {values_prepared}"
 
         connection = self.connect()
@@ -258,15 +260,15 @@
             return [{key: value for key, value in zip(keyfields, row)} for row in rows]
 
         for state in states:
             keyfields, rows = self._pop_experiments_with_status(state)
             rows = get_dict_for_keyfields_and_rows(keyfields, rows)
             if rows:
                 self.fill_table(fixed_parameter_combinations=rows)
-        logging.info(f"{len(rows)} experiments with status {' '.join(list(states))} were reset")
+        self.logger.info(f"{len(rows)} experiments with status {' '.join(list(states))} were reset")
 
     def _pop_experiments_with_status(self, status: Optional[str] = None) -> Tuple[List[str], List[List]]:
         if status == ExperimentStatus.ALL.value:
             condition = None
         else:
             condition = f"WHERE status = '{status}'"
```

### Comparing `py_experimenter-1.3.0/py_experimenter/database_connector_lite.py` & `py_experimenter-1.3.1/py_experimenter/database_connector_lite.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         except Error as err:
             raise DatabaseConnectionError(err)
 
     def _pull_open_experiment(self) -> Tuple[int, List, List]:
         with connect(**self.database_credentials) as connection:
             try:
                 cursor = self.cursor(connection)
-                experiment_id, description, values = self._execute_queries(connection, cursor)
+                experiment_id, description, values = self._select_open_experiments_from_db(connection, cursor)
             except Exception as err:
                 connection.rollback()
                 raise err
 
         return experiment_id, description, values
 
     def _table_exists(self, cursor) -> bool:
```

### Comparing `py_experimenter-1.3.0/py_experimenter/database_connector_mysql.py` & `py_experimenter-1.3.1/py_experimenter/database_connector_mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from py_experimenter.exceptions import DatabaseConnectionError, DatabaseCreationError
 from py_experimenter.utils import load_config
 
 
 class DatabaseConnectorMYSQL(DatabaseConnector):
     _prepared_statement_placeholder = '%s'
 
-    def __init__(self, experiment_configuration: ConfigParser, use_codecarbon:bool, codecarbon_config:ConfigParser, database_credential_file_path:str):
+    def __init__(self, experiment_configuration: ConfigParser, use_codecarbon:bool, codecarbon_config:ConfigParser, database_credential_file_path:str, logger):
         database_credentials = load_config(database_credential_file_path)
         self.host = database_credentials.get('CREDENTIALS', 'host')
         self.user = database_credentials.get('CREDENTIALS', 'user')
         self.password = database_credentials.get('CREDENTIALS', 'password')
 
-        super().__init__(experiment_configuration, use_codecarbon, codecarbon_config)
+        super().__init__(experiment_configuration, use_codecarbon, codecarbon_config, logger)
 
         self._create_database_if_not_existing()
 
     def _test_connection(self):
         modified_credentials = self.database_credentials.copy()
         del modified_credentials['database']
         try:
@@ -84,15 +84,15 @@
         return set(columns) == set(config_columns) 
 
     def _pull_open_experiment(self) -> Tuple[int, List, List]:
         try:
             connection = self.connect()
             cursor = self.cursor(connection)
             self._start_transaction(connection, readonly=False)
-            experiment_id, description, values = self._execute_queries(connection, cursor)
+            experiment_id, description, values = self._select_open_experiments_from_db(connection, cursor)
         except Exception as err:
             connection.rollback()
             raise err
         self.close_connection(connection)
 
         return experiment_id, description, values
```

### Comparing `py_experimenter-1.3.0/py_experimenter/exceptions.py` & `py_experimenter-1.3.1/py_experimenter/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     pass
 
 
 class InvalidResultFieldError(DatabaseError):
     pass
 
 
+class InvalidLogFieldError(DatabaseError):
+    pass
+
+
 class TableHasWrongStructureError(CreatingTableError):
     pass
 
 
 class NoExperimentsLeftException(PyExperimenterError):
     pass
 
@@ -53,9 +57,10 @@
 class InvalidConfigError(ConfigError):
     pass
 
 
 class InvalidValuesInConfiguration(ConfigError):
     pass
 
+
 class MissingLogTableError(ConfigError):
-	pass
+    pass
```

### Comparing `py_experimenter-1.3.0/py_experimenter/experimenter.py` & `py_experimenter-1.3.1/py_experimenter/experimenter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 import socket
 import traceback
 from configparser import ConfigParser
-from typing import Callable, Dict, List, Tuple
+from typing import Callable, Dict, List, Tuple, Union
 
 import pandas as pd
 from codecarbon import EmissionsTracker, OfflineEmissionsTracker
 from joblib import Parallel, delayed
 
 from py_experimenter import utils
 from py_experimenter.database_connector_lite import DatabaseConnectorLITE
@@ -24,17 +24,22 @@
 
     def __init__(self,
                  experiment_configuration_file_path: str = os.path.join('config', 'experiment_configuration.cfg'),
                  database_credential_file_path: str = os.path.join('config', 'database_credentials.cfg'),
                  table_name: str = None,
                  database_name: str = None,
                  use_codecarbon: bool = True,
-                 name='PyExperimenter'):
+                 name='PyExperimenter',
+                 logger_name: str = 'py-experimenter',
+                 log_level: Union[int, str] = logging.INFO,
+                 log_file: str = "./logs/py-experimenter.log"
+                 ):
         """
-        Initializes the PyExperimenter with the given information.
+        Initializes the PyExperimenter with the given information. If no loger `logger_name` exists, a new logger
+        is created with the given `logger_name` and `log_level`. 
 
         :param experiment_configuration_file_path: The path to the experiment configuration file. Defaults to
             'config/experiment_configuration.cfg'.
         :type experiment_configuration_file_path: str, optional
         :param database_credential_file_path: The path to the database configuration file storing the credentials
             for the database connection, i.e., host, user and password. Defaults to 'config/database_credentials.cfg'.
         :type database_credential_file_path: str, optional
@@ -47,49 +52,77 @@
             file. Defaults to None.
         :type database_name: str, optional
         :param use_codecarbon: If True, the carbon emissions are tracked and stored in the database. Defaults to True.
         :type use_codecarbon: bool, optional
         :param name: The name of the PyExperimenter, which will be logged in the according column in the database table.
             Defaults to 'PyExperimenter'.
         :type name: str, optional
+        :param logger_name: The name of the logger. Defaults to 'PyExperimenter'.
+        :type logger_name: str
+        :param log_level: The log level of the logger. Defaults to logging.INFO.
+        :type log_level: Union[int,str]
+        :param log_file: The path to the log file. Defaults to "./py_experimenter.log".
+        :type log_file: str
         :raises InvalidConfigError: If either the experiment or database configuration are missing mandatory information.
         :raises ValueError: If an unsupported or unknown database connection provider is given.
         """
+        # If the logger is not allready craeted, create it with the given name and level
+        self.logger_name = logger_name
+
+        logger_initialization_needed = self.logger_name not in logging.root.manager.loggerDict.keys()
+        self.logger = logging.getLogger(logger_name)
+        self.logger.setLevel(log_level)
+
+        if logger_initialization_needed:
+            if not os.path.exists('logs'):
+                os.makedirs('logs')
+
+            formatter = logging.Formatter('%(asctime)s  | %(name)s - %(levelname)-8s | %(message)s')
+
+            handler = logging.StreamHandler()
+            handler.setFormatter(formatter)
+            self.logger.addHandler(handler)
+
+            handler = logging.FileHandler(log_file)
+            handler.setFormatter(formatter)
+            self.logger.addHandler(handler)
+
         self.config = utils.load_config(experiment_configuration_file_path)
 
         self.use_codecarbon = use_codecarbon
         self.config, self.codecarbon_config = utils.extract_codecarbon_config(self.config)
         if self.codecarbon_config.has_option('codecarbon', 'offline_mode'):
             self.codecarbon_offline_mode = self.codecarbon_config['codecarbon']['offline_mode'] == 'True'
         else:
             self.codecarbon_offline_mode = False
             self.codecarbon_config.set('codecarbon', 'offline_mode', 'False')
         utils.write_codecarbon_config(self.codecarbon_config)
 
         self.database_credential_file_path = database_credential_file_path
-        if not PyExperimenter._is_valid_configuration(self.config, database_credential_file_path):
-            raise InvalidConfigError('Invalid configuration')
+        if not self._is_valid_configuration(self.config, database_credential_file_path):
+            raise InvalidConfigError('Invalid configuration. See previous log messages for details')
 
         if table_name is not None:
             self.config.set('PY_EXPERIMENTER', 'table', table_name)
         if database_name is not None:
             self.config.set('PY_EXPERIMENTER', 'database', database_name)
         self.name = name
 
         self.experiment_configuration_file_path = experiment_configuration_file_path
         self.timestamp_on_result_fields = utils.timestamps_for_result_fields(self.config)
 
         if self.config['PY_EXPERIMENTER']['provider'] == 'sqlite':
-            self.dbconnector = DatabaseConnectorLITE(self.config, self.use_codecarbon, self.codecarbon_config)
+            self.dbconnector = DatabaseConnectorLITE(self.config, self.use_codecarbon, self.codecarbon_config, self.logger)
         elif self.config['PY_EXPERIMENTER']['provider'] == 'mysql':
-            self.dbconnector = DatabaseConnectorMYSQL(self.config, self.use_codecarbon, self.codecarbon_config, database_credential_file_path)
+            self.dbconnector = DatabaseConnectorMYSQL(self.config, self.use_codecarbon, self.codecarbon_config, database_credential_file_path,
+                                                      self.logger)
         else:
             raise ValueError('The provider indicated in the config file is not supported')
 
-        logging.info('Initialized and connected to database')
+        self.logger.info('Initialized and connected to database')
 
     def set_config_value(self, section_name: str, key: str, value: str) -> None:
         """
         Modifies the experiment configuration so that within the given `section_name` the value of the  property identified by
         the given `key` is overwritten, or created if it was not existing beforehand.
 
         :param section_name: The name of the section of the experiment configuration in which a value should be set.
@@ -99,15 +132,15 @@
         :param value: The value which should be set to the property identified by the given key in the given section.
         :type value: str
         :raises InvalidConfigError: If the modified configuration either misses, or has invalid information.
         """
         if not self.config.has_section(section_name):
             self.config.add_section(section_name)
         self.config.set(section_name, key, value)
-        if not PyExperimenter._is_valid_configuration(self.config, self.database_credential_file_path):
+        if not self._is_valid_configuration(self.config, self.database_credential_file_path):
             raise InvalidConfigError('Invalid configuration')
 
     def get_config_value(self, section_name: str, key: str) -> str:
         """
         Returns the value of the property of the experiment configuration identified by the given key. If the `key`
         is not contained within the section, an exception is raised.
 
@@ -147,50 +180,48 @@
         :type key: str
         :return: True if the given `key` is contained in the experiment configuration within the section called
             `section_name`. False otherwise.
         :rtype: bool
         """
         return self.config.has_option(section_name, key)
 
-    @ staticmethod
-    def _is_valid_configuration(config: ConfigParser, database_credential_file_path: str = None) -> bool:
+    def _is_valid_configuration(self, config: ConfigParser, database_credential_file_path: str = None) -> bool:
         """
         Checks whether the given experiment configuration is valid, i.e., it contains all necessary fields, the database provider
         is either mysql or sqlite, and in case of a mysql database provider, that the database credentials are available.
 
         :param config: The experiment configuration.
         :type config: ConfigParser
         :param database_credential_file_path: The path to the database configuration file, i.e., the file defining
             the host, user and password. Defaults to None.
         :type database_credential_file_path: str, optional
         :return: True if the experiment configuration contains all necessary fields.
         :rtype: bool
         """
         if not config.has_section('PY_EXPERIMENTER'):
-            return False
-
-        if set(config.keys()) > {'PY_EXPERIMENTER', 'CUSTOM', 'DEFAULT'}:
+            self.logger.error('Error in config file: PY_EXPERIMENTER section is missing')
             return False
 
         if not {'provider', 'database', 'table'}.issubset(set(config.options('PY_EXPERIMENTER'))):
-            logging.error('Error in config file: DATABASE section must contain provider, database, and table')
+            self.logger.error('Error in config file: DATABASE section must contain provider, database, and table')
             return False
 
         if config['PY_EXPERIMENTER']['provider'] not in ['sqlite', 'mysql']:
-            logging.error('Error in config file: DATABASE provider must be either sqlite or mysql')
+            self.logger.error('Error in config file: DATABASE provider must be either sqlite or mysql')
             return False
 
         if config['PY_EXPERIMENTER']['provider'] == 'mysql':
             credentials = utils.load_config(database_credential_file_path)
             if not {'host', 'user', 'password'}.issubset(set(credentials.options('CREDENTIALS'))):
-                logging.error(
-                    f'Error in config file: DATABASE section must contain host, user, and password since provider is {config["DATABASE"]["provider"]}')
+                self.logger.error(
+                    f'Error in config file: CREDENTIALS file and section must contain host, user, and password since provider is {config["DATABASE"]["provider"]}')
                 return False
 
-        if not {'keyfields', 'resultfields'}.issubset(set(config.options('PY_EXPERIMENTER'))):
+        if not 'keyfields' in config.options('PY_EXPERIMENTER'):
+            self.logger.error('Error in config file: PY_EXPERIMENTER section must contain keyfields')
             return False
         return True
 
     def fill_table_from_combination(self, fixed_parameter_combinations: List[dict] = None, parameters: dict = None) -> None:
         """
         Adds rows to the database table based on the given information.
 
@@ -314,15 +345,15 @@
 
         with Parallel(n_jobs=n_jobs) as parallel:
             if max_experiments == -1:
                 parallel(delayed(self._worker)(experiment_function) for _ in range(n_jobs))
             else:
                 parallel(delayed(self._execution_wrapper)(experiment_function)
                          for _ in range(max_experiments))
-        logging.info("All configured executions finished.")
+        self.logger.info("All configured executions finished.")
 
     def _worker(self, experiment_function: Callable[[Dict, Dict, ResultProcessor], None]) -> None:
         """
         Worker that repeatedly pulls open experiments from the database table and executes them.
 
         :param experiment_function: The function that should be executed with the different parametrizations.
         :type experiment_function: Callable[[Dict, Dict, ResultProcessor], None]
@@ -353,40 +384,39 @@
         :param experiment_function: The function that should be executed with the different parametrizations.
         :type experiment_function: Callable[[dict, dict, ResultProcessor], None]
         :raises NoExperimentsLeftError: If there are no experiments left to be executed.
         :raises DatabaseConnectionError: If an error occurred during the connection to the database.
         """
         experiment_id, keyfield_values = self.dbconnector.get_experiment_configuration()
 
-        result_field_names = utils.get_result_field_names(self.config)
         custom_fields = dict(self.config.items('CUSTOM')) if self.has_section('CUSTOM') else None
         table_name = self.get_config_value('PY_EXPERIMENTER', 'table')
 
         result_processor = ResultProcessor(self.config, self.use_codecarbon, self.codecarbon_config, self.database_credential_file_path, table_name=table_name,
-                                           result_fields=result_field_names, experiment_id=experiment_id)
+                                           experiment_id=experiment_id, logger=self.logger)
         result_processor._set_name(self.name)
         result_processor._set_machine(socket.gethostname())
 
         if self.use_codecarbon:
             if self.codecarbon_offline_mode:
                 if not self.codecarbon_config.has_option('codecarbon', 'country_iso_code'):
                     raise InvalidConfigError(('CodeCarbon offline mode requires a `country_iso_code` in the config file.'
                                               'For more information see `https://mlco2.github.io/codecarbon/index.html`.'))
                 tracker = OfflineEmissionsTracker()
             else:
                 tracker = EmissionsTracker()
 
         try:
-            logging.debug(f"Start of experiment_function on process {socket.gethostname()}")
+            self.logger.debug(f"Start of experiment_function on process {socket.gethostname()}")
             if self.use_codecarbon:
                 tracker.start()
             experiment_function(keyfield_values, result_processor, custom_fields)
         except Exception:
             error_msg = traceback.format_exc()
-            logging.error(error_msg)
+            self.logger.error(error_msg)
             result_processor._write_error(error_msg)
             result_processor._change_status(ExperimentStatus.ERROR.value)
         else:
             result_processor._change_status(ExperimentStatus.DONE.value)
         finally:
             if self.use_codecarbon:
                 tracker.stop()
@@ -399,15 +429,15 @@
         table again. 
 
         :param states: The status of experiments that should be reset. Either `created`, `running`, `error`, `done`, or `all`.
         Note that `states` is a variable-length argument, so multiple states can be given as a tuple.
         :type status: Tuple[str]
         """
         if not states:
-            logging.warning('No states given to reset experiments. No experiments are reset.')
+            self.logger.warning('No states given to reset experiments. No experiments are reset.')
         else:
             self.dbconnector.reset_experiments(*states)
 
     def delete_table(self) -> None:
         """
         Drops the table defined in the configuration file. Additionally, all associated log tables are dropped.
         """
```

### Comparing `py_experimenter-1.3.0/py_experimenter/utils.py` & `py_experimenter-1.3.1/py_experimenter/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     try:
         with open(path) as f:
             config.read_file(f)
     except FileNotFoundError:
         raise NoConfigFileError(f'Configuration file missing! Please add file: {path}')
 
     return config
-    
+
 
 def extract_codecarbon_config(config: ConfigParser) -> Tuple[ConfigParser]:
     codecarbon_config = ConfigParser()
     if config.has_section("codecarbon"):
         codecarbon_config.read_dict({"codecarbon": dict(config["codecarbon"])})
         config.remove_section("codecarbon")
     else:
@@ -47,28 +47,28 @@
 
 
 def write_codecarbon_config(codecarbon_config: ConfigParser):
     with open('.codecarbon.config', 'w') as f:
         codecarbon_config.write(f)
 
 
-def extract_codecarbon_columns(with_type:bool = True):
+def extract_codecarbon_columns(with_type: bool = True):
     if with_type:
         return [
             ('codecarbon_timestamp', 'DATETIME '), ('project_name', 'VARCHAR(255)'), ('run_id', 'VARCHAR(255)'),
             ('duration_seconds', 'DOUBLE'), ('emissions_kg', 'DOUBLE'), ('emissions_rate_kg_sec', 'DOUBLE'),
             ('cpu_power_watt', 'DOUBLE'), ('gpu_power_watt', 'DOUBLE'), ('ram_power_watt', 'DOUBLE'),
             ('cpu_energy_kw', 'DOUBLE'), ('gpu_energy_kw', 'DOUBLE'), ('ram_energy_kw', 'DOUBLE'),
             ('energy_consumed_kw', 'DOUBLE'), ('country_name', 'VARCHAR(255)'), ('country_iso_code', 'VARCHAR(255)'),
             ('region', 'VARCHAR(255)'), ('cloud_provider', 'VARCHAR(255)'), ('cloud_region', 'VARCHAR(255)'),
             ('os', 'VARCHAR(255)'), ('python_version', 'VARCHAR(255)'), ('codecarbon_version', 'VARCHAR(255)'),
             ('cpu_count', 'DOUBLE'), ('cpu_model', 'VARCHAR(255)'), ('gpu_count', 'DOUBLE'),
             ('gpu_model', 'VARCHAR(255)'), ('longitude', 'VARCHAR(255)'), ('latitude', 'VARCHAR(255)'),
-            ('ram_total_size', 'DOUBLE'), ('tracking_mode', 'VARCHAR(255)'), ('on_cloud', 'VARCHAR(255)'), 
-            ('power_usage_efficiency', 'DOUBLE'),('offline_mode', 'BOOL')
+            ('ram_total_size', 'DOUBLE'), ('tracking_mode', 'VARCHAR(255)'), ('on_cloud', 'VARCHAR(255)'),
+            ('power_usage_efficiency', 'DOUBLE'), ('offline_mode', 'BOOL')
         ]
     else:
         return [
             'codecarbon_timestamp', 'project_name', 'run_id', 'duration_seconds', 'emissions_kg',
             'emissions_rate_kg_sec', 'cpu_power_watt', 'gpu_power_watt', 'ram_power_watt', 'cpu_energy_kw',
             'gpu_energy_kw', 'ram_energy_kw', 'energy_consumed_kw', 'country_name', 'country_iso_code', 'region',
             'cloud_provider', 'cloud_region', 'os', 'python_version', 'codecarbon_version', 'cpu_count', 'cpu_model',
@@ -134,16 +134,35 @@
 
 def get_result_field_names(config: ConfigParser) -> List[str]:
     result_fields = get_resultfields(config)
     return [name for name, _ in result_fields]
 
 
 def get_resultfields(config: ConfigParser) -> List[Tuple[str, str]]:
-    result_fields = extract_columns(config['PY_EXPERIMENTER']['resultfields'])
-    return result_fields
+    if config.has_option('PY_EXPERIMENTER', 'resultfields'):
+        result_fields = extract_columns(config['PY_EXPERIMENTER']['resultfields'])
+        return result_fields
+    else:
+        return list()
+
+
+def extract_logtables(config: ConfigParser, experiment_table_name: str) -> Optional[Dict[str, List[str]]]:
+    logtable_configs = dict()
+    if config.has_option('PY_EXPERIMENTER', 'logtables'):
+        logtable_definitions = [logtable_name.strip().split(':') for logtable_name in config['PY_EXPERIMENTER']['logtables'].split(',')]
+    else:
+        logtable_definitions = list()
+
+    for logtable_definer, column_definer in logtable_definitions:
+        logtable_name = f'{experiment_table_name}__{logtable_definer}'
+        if config.has_option('PY_EXPERIMENTER', column_definer):
+            logtable_configs[logtable_name] = extract_columns(config['PY_EXPERIMENTER'][column_definer])
+        else:
+            logtable_configs[logtable_name] = [(logtable_definer, column_definer)]
+    return logtable_configs
 
 
 def extract_columns(fields: str) -> List[Tuple[str, str]]:
     """
     Clean field names
     :param fields: List of field names
     :return: Cleaned list of field names
@@ -170,30 +189,14 @@
     result_fields_with_timestamp = list()
     for result_field in result_field_configuration:
         result_fields_with_timestamp.append(result_field)
         result_fields_with_timestamp.append((f'{result_field[0]}_timestamp', 'VARCHAR(255)'))
     return result_fields_with_timestamp
 
 
-def extract_logtables(config: ConfigParser, experiment_table_name: str) -> Optional[Dict[str, List[str]]]:
-    logtable_configs = dict()
-    if config.has_option('PY_EXPERIMENTER', 'logtables'):
-        logtable_definitions = [logtable_name.strip().split(':') for logtable_name in config['PY_EXPERIMENTER']['logtables'].split(',')]
-    else:
-        logtable_definitions = list()
-
-    for logtable_definer, column_definer in logtable_definitions:
-        logtable_name = f'{experiment_table_name}__{logtable_definer}'
-        if config.has_option('PY_EXPERIMENTER', column_definer):
-            logtable_configs[logtable_name] = extract_columns(config['PY_EXPERIMENTER'][column_definer])
-        else:
-            logtable_configs[logtable_name] = [(logtable_definer, column_definer)]
-    return logtable_configs
-
-
 def combine_fill_table_parameters(keyfield_names, parameters, fixed_parameter_combinations):
     def create_combination_from_parameters():
         keyfield_data = list()
         used_keys = list()
 
         for keyfield_name in keyfield_names:
             if keyfield_name in parameters.keys():
```

### Comparing `py_experimenter-1.3.0/pyproject.toml` & `py_experimenter-1.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-experimenter"
-version = "1.3.0"
+version = "1.3.1"
 description = "The PyExperimenter is a tool for the automatic execution of experiments, e.g. for machine learning (ML), capturing corresponding results in a unified manner in a database."
 authors = [
     "Tanja Tornede <t.tornede@ai.uni-hannover.de>",
     "Alexander Tornede <a.tornede@ai.uni-hannover.de>",
     "Lukas Fehring <lukas.fehring@stud.uni-hannover.de>",
     "Lukas Gehring",
     "Helena Graf <h.graf@ai.uni-hannover.de>",
```

### Comparing `py_experimenter-1.3.0/setup.py` & `py_experimenter-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'jupyterlab>=3.5.0,<4.0.0',
  'numpy>=1.15',
  'pandas>=1.0',
  'pymysql>=1.0.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'py-experimenter',
-    'version': '1.3.0',
+    'version': '1.3.1',
     'description': 'The PyExperimenter is a tool for the automatic execution of experiments, e.g. for machine learning (ML), capturing corresponding results in a unified manner in a database.',
     'long_description': '[![Project Homepage](https://img.shields.io/badge/Project%20Homepage-tornede.github.io/py_experimenter-0092CD)](https://tornede.github.io/py_experimenter)\n[![Pypi](https://img.shields.io/pypi/v/py_experimenter)](https://pypi.org/project/py-experimenter/)\n[![License](https://img.shields.io/github/license/tornede/py_experimenter)](https://tornede.github.io/py_experimenter/license.html)\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.05149/status.svg)](https://doi.org/10.21105/joss.05149)\n\n![Tests](https://github.com/tornede/py_experimenter/actions/workflows/tests.yml/badge.svg)\n![GitHub Pages](https://github.com/tornede/py_experimenter/actions/workflows/github-pages.yml/badge.svg)\n\n<img src="docs/source/_static/py-experimenter-logo.png" alt="PyExperimenter Logo: Python biting a database" width="200px"/>\n\n# PyExperimenter\n\n`PyExperimenter` is a tool to facilitate the setup, documentation, execution, and subsequent evaluation of results from an empirical study of algorithms and in particular is designed to reduce the involved manual effort significantly.\nIt is intended to be used by researchers in the field of artificial intelligence, but is not limited to those.\n\nThe empirical analysis of algorithms is often accompanied by the execution of algorithms for different inputs and variants of the algorithms (specified via parameters) and the measurement of non-functional properties.\nSince the individual evaluations are usually independent, the evaluation can be performed in a distributed manner on an HPC system.\nHowever, setting up, documenting, and evaluating the results of such a study is often file-based.\nUsually, this requires extensive manual work to create configuration files for the inputs or to read and aggregate measured results from a report file.\nIn addition, monitoring and restarting individual executions is tedious and time-consuming.\n\nThese challenges are addressed by `PyExperimenter` by means of a single well defined configuration file and a central database for managing massively parallel evaluations, as well as collecting and aggregating their results.\nThereby, `PyExperimenter` alleviates the aforementioned overhead and allows experiment executions to be defined and monitored with ease.\n\n![General schema of `PyExperimenter`.](docs/source/_static/workflow.png)\n\nFor more details check out the [`PyExperimenter` documentation](https://tornede.github.io/py_experimenter/):\n\n- [Installation](https://tornede.github.io/py_experimenter/installation.html)\n- [Examples](https://tornede.github.io/py_experimenter/examples/example_general_usage.html)\n\n## Cite PyExperimenter\n\nIf you use `PyExperimenter` in a scientific publication, we would appreciate a citation in one of the following ways.\n\n### Citation String\n\nTornede et al., (2023). PyExperimenter: Easily distribute experiments and track results. Journal of Open Source Software, 8(84), 5149, https://doi.org/10.21105/joss.05149\n\n### BibTex\n```\n@article{Tornede2023, \n    title = {{PyExperimenter}: Easily distribute experiments and track results}, \n    author = {Tanja Tornede and Alexander Tornede and Lukas Fehring and Lukas Gehring and Helena Graf and Jonas Hanselle and Felix Mohr and Marcel Wever}, \n    journal = {Journal of Open Source Software},\n    publisher = {The Open Journal},  \n    year = {2023}, \n    volume = {8}, \n    number = {84}, \n    pages = {5149}, \n    doi = {10.21105/joss.05149}, \n    url = {https://doi.org/10.21105/joss.05149}\n}\n```\n',
     'author': 'Tanja Tornede',
     'author_email': 't.tornede@ai.uni-hannover.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tornede/py_experimenter',
```

### Comparing `py_experimenter-1.3.0/PKG-INFO` & `py_experimenter-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-experimenter
-Version: 1.3.0
+Version: 1.3.1
 Summary: The PyExperimenter is a tool for the automatic execution of experiments, e.g. for machine learning (ML), capturing corresponding results in a unified manner in a database.
 Home-page: https://github.com/tornede/py_experimenter
 License: MIT
 Keywords: python,experiments,database,executor
 Author: Tanja Tornede
 Author-email: t.tornede@ai.uni-hannover.de
 Requires-Python: >=3.9,<4.0
```


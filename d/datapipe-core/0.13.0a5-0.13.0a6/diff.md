# Comparing `tmp/datapipe_core-0.13.0a5.tar.gz` & `tmp/datapipe_core-0.13.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapipe_core-0.13.0a5.tar", max compression
+gzip compressed data, was "datapipe_core-0.13.0a6.tar", max compression
```

## Comparing `datapipe_core-0.13.0a5.tar` & `datapipe_core-0.13.0a6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a5/LICENSE
--rw-r--r--   0        0        0      779 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/README.md
--rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.13.0a5/datapipe/__init__.py
--rw-r--r--   0        0        0    18208 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/cli.py
--rw-r--r--   0        0        0    14869 2023-07-20 12:40:57.390942 datapipe_core-0.13.0a5/datapipe/compute.py
--rw-r--r--   0        0        0    31657 2023-07-20 14:04:54.916006 datapipe_core-0.13.0a5/datapipe/core_steps.py
--rw-r--r--   0        0        0     6780 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/datatable.py
--rw-r--r--   0        0        0     4649 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/event_logger.py
--rw-r--r--   0        0        0     1562 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/executor/__init__.py
--rw-r--r--   0        0        0     1972 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/executor/ray.py
--rw-r--r--   0        0        0     4168 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/lints.py
--rw-r--r--   0        0        0    21906 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/metastore.py
--rw-r--r--   0        0        0      969 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/run_config.py
--rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a5/datapipe/store/__init__.py
--rw-r--r--   0        0        0     8415 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/store/database.py
--rw-r--r--   0        0        0    18238 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/store/filedir.py
--rw-r--r--   0        0        0     3595 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/store/milvus.py
--rw-r--r--   0        0        0     1337 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/store/pandas.py
--rw-r--r--   0        0        0     8674 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/store/qdrant.py
--rw-r--r--   0        0        0     3209 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/store/redis.py
--rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.13.0a5/datapipe/store/table_store.py
--rw-r--r--   0        0        0     9985 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a5/datapipe/types.py
--rw-r--r--   0        0        0     2145 2023-07-20 14:04:54.916006 datapipe_core-0.13.0a5/pyproject.toml
--rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 datapipe_core-0.13.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a6/LICENSE
+-rw-r--r--   0        0        0      779 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.13.0a6/datapipe/__init__.py
+-rw-r--r--   0        0        0    18265 2023-07-24 12:14:18.558583 datapipe_core-0.13.0a6/datapipe/cli.py
+-rw-r--r--   0        0        0     9584 2023-07-24 12:14:18.558583 datapipe_core-0.13.0a6/datapipe/compute.py
+-rw-r--r--   0        0        0    37210 2023-07-24 12:14:18.558583 datapipe_core-0.13.0a6/datapipe/core_steps.py
+-rw-r--r--   0        0        0     6780 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/datatable.py
+-rw-r--r--   0        0        0     4649 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/event_logger.py
+-rw-r--r--   0        0        0     1562 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/executor/__init__.py
+-rw-r--r--   0        0        0     1972 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/executor/ray.py
+-rw-r--r--   0        0        0     4168 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/lints.py
+-rw-r--r--   0        0        0    21906 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/metastore.py
+-rw-r--r--   0        0        0      969 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/run_config.py
+-rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a6/datapipe/store/__init__.py
+-rw-r--r--   0        0        0     8435 2023-07-24 12:14:18.558583 datapipe_core-0.13.0a6/datapipe/store/database.py
+-rw-r--r--   0        0        0    18238 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/store/filedir.py
+-rw-r--r--   0        0        0     3595 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/store/milvus.py
+-rw-r--r--   0        0        0     1337 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/store/pandas.py
+-rw-r--r--   0        0        0     8674 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/store/qdrant.py
+-rw-r--r--   0        0        0     3209 2023-07-20 11:34:29.730532 datapipe_core-0.13.0a6/datapipe/store/redis.py
+-rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.13.0a6/datapipe/store/table_store.py
+-rw-r--r--   0        0        0     9945 2023-07-24 12:14:18.558583 datapipe_core-0.13.0a6/datapipe/types.py
+-rw-r--r--   0        0        0     2145 2023-07-24 12:14:18.558583 datapipe_core-0.13.0a6/pyproject.toml
+-rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 datapipe_core-0.13.0a6/PKG-INFO
```

### Comparing `datapipe_core-0.13.0a5/LICENSE` & `datapipe_core-0.13.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/README.md` & `datapipe_core-0.13.0a6/README.md`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/cli.py` & `datapipe_core-0.13.0a6/datapipe/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,15 +395,16 @@
     steps_to_run: List[ComputeStep] = ctx.obj["steps"]
     steps_to_run_names = [f"'{i.name}'" for i in steps_to_run]
     print(f"Running following steps: {', '.join(steps_to_run_names)}")
 
     idx_dict = {k: v for k, v in (i.split("=") for i in idx.split(","))}
 
     for step in steps_to_run:
-        step.run_idx(ds=app.ds, idx=cast(IndexDF, pd.DataFrame([idx_dict])))
+        if isinstance(step, BaseBatchTransformStep):
+            step.run_idx(ds=app.ds, idx=cast(IndexDF, pd.DataFrame([idx_dict])))
 
 
 @step.command()  # type: ignore
 @click.option("--loop", is_flag=True, default=False, help="Run continuosly in a loop")
 @click.option(
     "--loop-delay", type=click.INT, default=1, help="Delay between loops in seconds"
 )
```

### Comparing `datapipe_core-0.13.0a5/datapipe/core_steps.py` & `datapipe_core-0.13.0a6/datapipe/core_steps.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     select,
     tuple_,
 )
 from tqdm_loggable.auto import tqdm
 
 from datapipe.compute import Catalog, ComputeStep, PipelineStep
 from datapipe.datatable import DataStore, DataTable
-from datapipe.executor import Executor, ExecutorConfig
+from datapipe.executor import Executor, ExecutorConfig, SingleThreadExecutor
 from datapipe.metastore import MetaTable, TransformMetaTable
 from datapipe.run_config import LabelDict, RunConfig
 from datapipe.store.database import sql_apply_runconfig_filter
 from datapipe.types import (
     ChangeList,
     DataDF,
     IndexDF,
@@ -282,15 +282,15 @@
     def _build_changed_idx_sql(
         self,
         ds: DataStore,
         filters_idx: Optional[IndexDF] = None,
         order_by: Optional[List[str]] = None,
         order: Literal["asc", "desc"] = "asc",
         run_config: Optional[RunConfig] = None,  # TODO remove
-    ) -> Tuple[Iterable[str], select]:
+    ) -> Tuple[Iterable[str], Any]:
         if len(self.transform_keys) == 0:
             raise NotImplementedError()
 
         all_input_keys_counts: Dict[str, int] = {}
         for col in itertools.chain(*[dt.primary_schema for dt in self.input_dts]):
             all_input_keys_counts[col.name] = all_input_keys_counts.get(col.name, 0) + 1
 
@@ -327,15 +327,15 @@
             dt: DataTable, agg_fun, agg_col: str
         ) -> Tuple[List[str], Any]:
             tbl = dt.meta_table.sql_table
 
             keys = [k for k in self.transform_keys if k in dt.primary_keys]
             key_cols = [column(k) for k in keys]
 
-            sql = (
+            sql: Any = (
                 select(*key_cols + [agg_fun(tbl.c[agg_col]).label(agg_col)])
                 .select_from(tbl)
                 .group_by(*key_cols)
             )
 
             sql = _apply_filters_idx(sql, keys, filters_idx)
 
@@ -393,15 +393,15 @@
             return sql.cte(name=f"all__{agg_col}")
 
         inp_ctes = [_make_agg_cte(tbl, func.max, "update_ts") for tbl in self.input_dts]
 
         inp = _make_agg_of_agg(inp_ctes, "update_ts")
 
         tr_tbl = self.meta_table.sql_table
-        out = (
+        out: Any = (
             select(
                 *[column(k) for k in self.transform_keys]
                 + [tr_tbl.c.process_ts, tr_tbl.c.priority, tr_tbl.c.is_success]
             )
             .select_from(tr_tbl)
             .group_by(*[column(k) for k in self.transform_keys])
         )
@@ -485,15 +485,15 @@
         with ds.meta_dbconn.con.begin() as con:
             idx_count = con.execute(
                 select([func.count()]).select_from(
                     alias(sql.subquery(), name="union_select")
                 )
             ).scalar()
 
-        return idx_count
+        return cast(int, idx_count)
 
     def get_full_process_ids(
         self,
         ds: DataStore,
         chunk_size: Optional[int] = None,
         run_config: Optional[RunConfig] = None,
     ) -> Tuple[int, Iterable[IndexDF]]:
@@ -586,32 +586,70 @@
         ds: DataStore,
         idx: IndexDF,
         output_dfs: Optional[TransformResult],
         process_ts: float,
         run_config: Optional[RunConfig] = None,
     ) -> ChangeList:
         run_config = self._apply_filters_to_run_config(run_config)
-        res = super().store_batch_result(ds, idx, output_dfs, process_ts, run_config)
+
+        changes = ChangeList()
+
+        if output_dfs is not None:
+            with tracer.start_as_current_span("store output batch"):
+                if isinstance(output_dfs, (list, tuple)):
+                    assert len(output_dfs) == len(self.output_dts)
+                else:
+                    assert len(self.output_dts) == 1
+                    output_dfs = [output_dfs]
+
+                for k, res_dt in enumerate(self.output_dts):
+                    # Берем k-ое значение функции для k-ой таблички
+                    # Добавляем результат в результирующие чанки
+                    change_idx = res_dt.store_chunk(
+                        data_df=output_dfs[k],
+                        processed_idx=idx,
+                        now=process_ts,
+                        run_config=run_config,
+                    )
+
+                    changes.append(res_dt.name, change_idx)
+
+        else:
+            with tracer.start_as_current_span("delete missing data from output"):
+                for k, res_dt in enumerate(self.output_dts):
+                    del_idx = res_dt.meta_table.get_existing_idx(idx)
+
+                    res_dt.delete_by_idx(del_idx, run_config=run_config)
+
+                    changes.append(res_dt.name, del_idx)
 
         self.meta_table.mark_rows_processed_success(
             idx, process_ts=process_ts, run_config=run_config
         )
 
-        return res
+        return changes
 
     def store_batch_err(
         self,
         ds: DataStore,
         idx: IndexDF,
         e: Exception,
         process_ts: float,
         run_config: Optional[RunConfig] = None,
     ) -> None:
         run_config = self._apply_filters_to_run_config(run_config)
-        super().store_batch_err(ds, idx, e, process_ts, run_config)
+
+        logger.error(f"Process batch failed: {str(e)}")
+        ds.event_logger.log_exception(
+            e,
+            run_config=RunConfig.add_labels(
+                run_config,
+                {"idx": idx.to_dict(orient="records"), "process_ts": process_ts},
+            ),
+        )
 
         self.meta_table.mark_rows_processed_error(
             idx,
             process_ts=process_ts,
             error=str(e),
             run_config=run_config,
         )
@@ -621,14 +659,155 @@
 
         for idx in tqdm(idx_gen, total=idx_len):
             self.meta_table.insert_rows(idx)
 
     def reset_metadata(self, ds: DataStore) -> None:
         self.meta_table.mark_all_rows_unprocessed()
 
+    def get_batch_input_dfs(
+        self,
+        ds: DataStore,
+        idx: IndexDF,
+        run_config: Optional[RunConfig] = None,
+    ) -> List[DataDF]:
+        return [inp.get_data(idx) for inp in self.input_dts]
+
+    def process_batch_dfs(
+        self,
+        ds: DataStore,
+        idx: IndexDF,
+        input_dfs: List[DataDF],
+        run_config: Optional[RunConfig] = None,
+    ) -> TransformResult:
+        raise NotImplementedError()
+
+    def process_batch_dts(
+        self,
+        ds: DataStore,
+        idx: IndexDF,
+        run_config: Optional[RunConfig] = None,
+    ) -> Optional[TransformResult]:
+        with tracer.start_as_current_span("get input data"):
+            input_dfs = self.get_batch_input_dfs(ds, idx, run_config)
+
+        if sum(len(j) for j in input_dfs) == 0:
+            return None
+
+        with tracer.start_as_current_span("run transform"):
+            output_dfs = self.process_batch_dfs(
+                ds=ds,
+                idx=idx,
+                input_dfs=input_dfs,
+                run_config=run_config,
+            )
+
+        return output_dfs
+
+    def process_batch(
+        self,
+        ds: DataStore,
+        idx: IndexDF,
+        run_config: Optional[RunConfig] = None,
+    ) -> ChangeList:
+        with tracer.start_as_current_span("process batch"):
+            logger.debug(f"Idx to process: {idx.to_records()}")
+
+            process_ts = time.time()
+
+            try:
+                output_dfs = self.process_batch_dts(ds, idx, run_config)
+
+                return self.store_batch_result(
+                    ds, idx, output_dfs, process_ts, run_config
+                )
+
+            except Exception as e:
+                self.store_batch_err(ds, idx, e, process_ts, run_config)
+
+                return ChangeList()
+
+    def run_full(
+        self,
+        ds: DataStore,
+        run_config: Optional[RunConfig] = None,
+        executor: Optional[Executor] = None,
+    ) -> None:
+        if executor is None:
+            executor = SingleThreadExecutor()
+
+        logger.info(f"Running: {self.name}")
+        run_config = RunConfig.add_labels(run_config, {"step_name": self.name})
+
+        (idx_count, idx_gen) = self.get_full_process_ids(ds=ds, run_config=run_config)
+
+        logger.info(f"Batches to process {idx_count}")
+
+        if idx_count is not None and idx_count == 0:
+            return
+
+        executor.run_process_batch(
+            ds=ds,
+            idx_count=idx_count,
+            idx_gen=idx_gen,
+            process_fn=self.process_batch,
+            run_config=run_config,
+            executor_config=self.executor_config,
+        )
+
+        ds.event_logger.log_step_full_complete(self.name)
+
+    def run_changelist(
+        self,
+        ds: DataStore,
+        change_list: ChangeList,
+        run_config: Optional[RunConfig] = None,
+        executor: Optional[Executor] = None,
+    ) -> ChangeList:
+        if executor is None:
+            executor = SingleThreadExecutor()
+
+        logger.info(f"Running: {self.name}")
+        run_config = RunConfig.add_labels(run_config, {"step_name": self.name})
+
+        (idx_count, idx_gen) = self.get_change_list_process_ids(
+            ds, change_list, run_config
+        )
+
+        logger.info(f"Batches to process {idx_count}")
+
+        if idx_count is not None and idx_count == 0:
+            return ChangeList()
+
+        res_changelist = ChangeList()
+
+        for idx in tqdm(idx_gen, total=idx_count):
+            changes = self.process_batch(
+                ds=ds,
+                idx=idx,
+                run_config=run_config,
+            )
+            res_changelist.extend(changes)
+
+        return res_changelist
+
+    def run_idx(
+        self,
+        ds: DataStore,
+        idx: IndexDF,
+        run_config: Optional[RunConfig] = None,
+    ) -> ChangeList:
+        logger.info(f"Running: {self.name}")
+        run_config = RunConfig.add_labels(run_config, {"step_name": self.name})
+
+        return self.process_batch(
+            ds=ds,
+            idx=idx,
+            run_config=run_config,
+        )
+
 
 @dataclass
 class DatatableBatchTransform(PipelineStep):
     func: DatatableBatchTransformFunc
     inputs: List[str]
     outputs: List[str]
     chunk_size: int = 1000
```

### Comparing `datapipe_core-0.13.0a5/datapipe/datatable.py` & `datapipe_core-0.13.0a6/datapipe/datatable.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/event_logger.py` & `datapipe_core-0.13.0a6/datapipe/event_logger.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/executor/__init__.py` & `datapipe_core-0.13.0a6/datapipe/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/executor/ray.py` & `datapipe_core-0.13.0a6/datapipe/executor/ray.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/lints.py` & `datapipe_core-0.13.0a6/datapipe/lints.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/metastore.py` & `datapipe_core-0.13.0a6/datapipe/metastore.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/run_config.py` & `datapipe_core-0.13.0a6/datapipe/run_config.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/store/database.py` & `datapipe_core-0.13.0a6/datapipe/store/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,41 +82,41 @@
         }
 
     def __setstate__(self, state):
         self._init(state["connstr"], state["schema"])
 
 
 def sql_apply_runconfig_filter(
-    sql: Executable,
+    sql: Any,
     table: Table,
     primary_keys: List[str],
     run_config: Optional[RunConfig] = None,
-) -> Executable:
+) -> Any:
     if run_config is not None:
         for k, v in run_config.filters.items():
             if k in primary_keys:
                 sql = sql.where(table.c[k] == v)
 
     return sql
 
 
 def sql_apply_idx_filter(
-    sql: Executable,
+    sql: Any,
     table: Table,
     primary_keys: List[str],
     idx: IndexDF,
-) -> Executable:
+) -> Any:
     if len(primary_keys) == 1:
         # Когда ключ один - сравниваем напрямую
         key = primary_keys[0]
         sql = sql.where(table.c[key].in_(idx[key].to_list()))
 
     else:
         # Когда ключей много - сравниваем по кортежу
-        keys = tuple_(*[table.c[key] for key in primary_keys])
+        keys = tuple_(*[table.c[key] for key in primary_keys])  # type: ignore
 
         sql = sql.where(
             keys.in_(
                 [
                     tuple([r[key] for key in primary_keys])  # type: ignore
                     for r in idx.to_dict(orient="records")
                 ]
@@ -128,18 +128,18 @@
 
 class MetaKey(SchemaItem):
     def __init__(self, target_name: Optional[str] = None) -> None:
         self.target_name = target_name
 
     def _set_parent(self, parent: SchemaEventTarget, **kw: Any) -> None:
         self.parent = parent
-        self.parent.meta_key = self
+        self.parent.meta_key = self  # type: ignore
 
         if not self.target_name:
-            self.target_name = parent.name
+            self.target_name = parent.name  # type: ignore
 
     @classmethod
     def get_property_name(cls) -> str:
         return "meta_key"
 
 
 class TableStoreDB(TableStore):
```

### Comparing `datapipe_core-0.13.0a5/datapipe/store/filedir.py` & `datapipe_core-0.13.0a6/datapipe/store/filedir.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/store/milvus.py` & `datapipe_core-0.13.0a6/datapipe/store/milvus.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/store/pandas.py` & `datapipe_core-0.13.0a6/datapipe/store/pandas.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/store/qdrant.py` & `datapipe_core-0.13.0a6/datapipe/store/qdrant.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/store/redis.py` & `datapipe_core-0.13.0a6/datapipe/store/redis.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/store/table_store.py` & `datapipe_core-0.13.0a6/datapipe/store/table_store.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a5/datapipe/types.py` & `datapipe_core-0.13.0a6/datapipe/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,27 +67,25 @@
 
 
 def meta_to_index(meta_df: MetadataDF, primary_keys: List[str]) -> IndexDF:
     return cast(IndexDF, meta_df[primary_keys])
 
 
 def index_difference(idx1_df: IndexDF, idx2_df: IndexDF) -> IndexDF:
-    assert list(idx1_df.columns) == list(idx2_df.columns)
+    assert sorted(idx1_df.columns) == sorted(idx2_df.columns)
     cols = idx1_df.columns.to_list()
 
     idx1_idx = idx1_df.set_index(cols).index
     idx2_idx = idx2_df.set_index(cols).index
 
     return cast(IndexDF, idx1_idx.difference(idx2_idx).to_frame(index=False))
 
 
 def index_intersection(idx1_df: IndexDF, idx2_df: IndexDF) -> IndexDF:
-    assert sorted(list(idx1_df.columns.tolist())) == sorted(
-        list(idx2_df.columns.tolist())
-    )
+    assert sorted(idx1_df.columns) == sorted(idx2_df.columns)
     cols = idx1_df.columns.to_list()
 
     idx1_idx = idx1_df.set_index(cols).index
     idx2_idx = idx2_df.set_index(cols).index
 
     return cast(IndexDF, idx1_idx.intersection(idx2_idx).to_frame(index=False))
```

### Comparing `datapipe_core-0.13.0a5/pyproject.toml` & `datapipe_core-0.13.0a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datapipe-core"
-version = "0.13.0-alpha.5"
+version = "0.13.0-alpha.6"
 description = "`datapipe` is a realtime incremental ETL library for Python application"
 readme = "README.md"
 repository = "https://github.com/epoch8/datapipe"
 authors = ["Andrey Tatarinov <a@tatarinov.co>"]
 packages = [
     { include = "datapipe" }
 ]
```

### Comparing `datapipe_core-0.13.0a5/PKG-INFO` & `datapipe_core-0.13.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapipe-core
-Version: 0.13.0a5
+Version: 0.13.0a6
 Summary: `datapipe` is a realtime incremental ETL library for Python application
 Home-page: https://github.com/epoch8/datapipe
 Author: Andrey Tatarinov
 Author-email: a@tatarinov.co
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```


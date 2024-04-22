# Comparing `tmp/odbc2deltalake-0.8.5.tar.gz` & `tmp/odbc2deltalake-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbc2deltalake-0.8.5.tar", max compression
+gzip compressed data, was "odbc2deltalake-0.8.7.tar", max compression
```

## Comparing `odbc2deltalake-0.8.5.tar` & `odbc2deltalake-0.8.7.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1081 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/LICENSE
--rw-r--r--   0        0        0     3563 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/README.md
--rw-r--r--   0        0        0      126 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/__init__.py
--rw-r--r--   0        0        0    42985 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/db_to_delta.py
--rw-r--r--   0        0        0     3809 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/delta_logger.py
--rw-r--r--   0        0        0       38 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/destination/__init__.py
--rw-r--r--   0        0        0     2554 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/destination/azure.py
--rw-r--r--   0        0        0     2923 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/destination/azure_utils.py
--rw-r--r--   0        0        0     2541 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/destination/databricks.py
--rw-r--r--   0        0        0     1196 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/destination/destination.py
--rw-r--r--   0        0        0     1592 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/destination/file_system.py
--rw-r--r--   0        0        0     5458 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/metadata.py
--rw-r--r--   0        0        0     1221 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/odbc_utils.py
--rw-r--r--   0        0        0     1851 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/query.py
--rw-r--r--   0        0        0       38 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/reader/__init__.py
--rw-r--r--   0        0        0     7195 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/reader/odbc_reader.py
--rw-r--r--   0        0        0     1961 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/reader/reader.py
--rw-r--r--   0        0        0     4932 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/reader/spark_reader.py
--rw-r--r--   0        0        0     1976 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/sql_glot_utils.py
--rw-r--r--   0        0        0      951 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/sql_schema.py
--rw-r--r--   0        0        0        0 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/write_utils/__init__.py
--rw-r--r--   0        0        0     6107 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/odbc2deltalake/write_utils/restore_pk.py
--rw-r--r--   0        0        0     1373 2024-04-16 09:53:15.537098 odbc2deltalake-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 odbc2deltalake-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/LICENSE
+-rw-r--r--   0        0        0     3563 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/README.md
+-rw-r--r--   0        0        0      571 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/__init__.py
+-rw-r--r--   0        0        0    36123 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/db_to_delta.py
+-rw-r--r--   0        0        0     3992 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/delta_logger.py
+-rw-r--r--   0        0        0       38 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/destination/__init__.py
+-rw-r--r--   0        0        0     2554 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/destination/azure.py
+-rw-r--r--   0        0        0     2923 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/destination/azure_utils.py
+-rw-r--r--   0        0        0     2541 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/destination/databricks.py
+-rw-r--r--   0        0        0     1196 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/destination/destination.py
+-rw-r--r--   0        0        0     1592 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/destination/file_system.py
+-rw-r--r--   0        0        0     5458 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/metadata.py
+-rw-r--r--   0        0        0     1221 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/odbc_utils.py
+-rw-r--r--   0        0        0     1851 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/query.py
+-rw-r--r--   0        0        0       38 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/reader/__init__.py
+-rw-r--r--   0        0        0     7295 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/reader/odbc_reader.py
+-rw-r--r--   0        0        0     1961 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/reader/reader.py
+-rw-r--r--   0        0        0     4932 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/reader/spark_reader.py
+-rw-r--r--   0        0        0     1976 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/sql_glot_utils.py
+-rw-r--r--   0        0        0      951 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/sql_schema.py
+-rw-r--r--   0        0        0      249 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/utils.py
+-rw-r--r--   0        0        0     7525 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/write_init.py
+-rw-r--r--   0        0        0        0 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/write_utils/__init__.py
+-rw-r--r--   0        0        0     6958 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/odbc2deltalake/write_utils/restore_pk.py
+-rw-r--r--   0        0        0     1392 2024-04-22 06:51:26.587419 odbc2deltalake-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 odbc2deltalake-0.8.7/PKG-INFO
```

### Comparing `odbc2deltalake-0.8.5/LICENSE` & `odbc2deltalake-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/README.md` & `odbc2deltalake-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/db_to_delta.py` & `odbc2deltalake-0.8.7/odbc2deltalake/db_to_delta.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 import dataclasses
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Callable, Iterable, Literal, Mapping, Sequence, TypeVar, cast
 import sqlglot as sg
+from .utils import concat_seq
 from odbc2deltalake.destination.destination import (
     Destination,
 )
 from odbc2deltalake.reader import DataSourceReader
 from .query import sql_quote_name
 from .metadata import (
     get_primary_keys,
@@ -18,106 +19,37 @@
 import json
 import time
 import sqlglot.expressions as ex
 from .sql_glot_utils import table_from_tuple, union, count_limit_one
 import logging
 import pydantic
 from .delta_logger import DeltaLogger
-
-is_pydantic_2 = int(pydantic.__version__.split(".")[0]) > 1
-
-
-IS_DELETED_COL_NAME = "__is_deleted"
-IS_DELETED_COL_INFO = InformationSchemaColInfo.from_name_type(
-    IS_DELETED_COL_NAME, "bit"
-)
-VALID_FROM_COL_NAME = "__timestamp"
-VALID_FROM_COL_INFO = InformationSchemaColInfo.from_name_type(
-    VALID_FROM_COL_NAME, "datetimeoffset"
-)
-IS_FULL_LOAD_COL_NAME = "__is_full_load"
-IS_FULL_LOAD_COL_INFO = InformationSchemaColInfo.from_name_type(
-    IS_FULL_LOAD_COL_NAME, "bit"
+from .write_init import (
+    WriteConfig,
+    WriteConfigAndInfos,
+    is_pydantic_2,
+    IS_DELETED_COL_INFO,
+    IS_DELETED_COL_NAME,
+    IS_FULL_LOAD_COL_INFO,
+    IS_FULL_LOAD_COL_NAME,
+    IS_DELETED_COL_NAME,
+    VALID_FROM_COL_NAME,
+    VALID_FROM_COL_INFO,
+    DBDeltaPathConfigs,
 )
 
 T = TypeVar("T")
 
-_default_type_map = {
-    "datetime": ex.DataType(this="datetime2(6)"),
-    "datetime2": ex.DataType(this="datetime2(6)"),
-    "rowversion": ex.DataType.Type.BIGINT,
-    "timestamp": ex.DataType.Type.BIGINT,
-}
-DEFAULT_DATA_TYPE_MAP: Mapping[str, ex.DATA_TYPE] = _default_type_map
-
-
-def compat_name(inf: InformationSchemaColInfo) -> str:
-    invalid_chars = " ,;{}()\n\t="
-    res = inf.column_name
-    for ic in invalid_chars:
-        res = res.replace(ic, "_")
-    return res
-
-
-@dataclass(frozen=True)
-class WriteConfig:
-
-    dialect: str = "tsql"
-    """The sqlglot dialect to use for the SQL generation against the source"""
-
-    primary_keys: list[str] | None = None
-    """A list of primary keys to use for the delta load. If None, the primary keys will be determined from the source"""
-
-    delta_col: str | None = None
-    """The column to use for the delta load. If None, the column will be determined from the source. Should be mostly increasing to make load efficient"""
-
-    load_mode: Literal[
-        "overwrite", "append", "force_full", "append_inserts", "simple_delta"
-    ] = "append"
-    """The load mode to use. Attention: overwrite will not help you build scd2, the history is in the delta table only
-        append_inserts is for when you have a delta column which is strictly increasing and you want to append new rows only. No deletes of rows. might be good for logs
-        simple_delta is for sources where the delta col is a datetime and you can be sure that there are no deletes or additional updates
-    """
-
-    data_type_map: Mapping[str, ex.DATA_TYPE] = dataclasses.field(
-        default_factory=lambda: _default_type_map.copy()
-    )
-    """Set this if you want to map stuff like decimal to double before writing to delta. We recommend doing so later in ETL usually"""
-
-    no_complex_entries_load: bool = False
-    """If true, will not load 'strange updates' via OPENJSON. Use if your db does not support OPENJSON or you're fine to get some additional updates in order to reduce complexity"""
-
-    get_target_name: Callable[[InformationSchemaColInfo], str] = dataclasses.field(
-        default_factory=lambda: compat_name
-    )
-    """A method that returns the target name of a column. This is used to map the source column names to the target column names.
-    Use if you want to apply some naming convention or avoid special characters in the target. """
-
 
 def _not_none(v: T | None) -> T:
     if v is None:
         raise ValueError("Value is None")
     return v
 
 
-class DBDeltaPathConfigs:
-    DELTA_1_NAME = "delta_1"
-    """common data for delta load contains data that has changed after last full load via naive criteria timestamp > last_timestamp (or similar, can also be dates)"""
-    DELTA_2_NAME = "delta_2"
-    """delta 2 is data where timestamp is different for whatever reason, eg restore"""
-    PRIMARY_KEYS_TS = "primary_keys_ts"
-    """file with primary keys and timestamps as of now, before load"""
-
-    LATEST_PK_VERSION = "latest_pk_version"
-    """file with primary keys and timestamps as of after load. 
-      this will be identital to primary_keys file IF there are no updates in the source within the load. 
-      this is unlikely, but possible
-    """
-
-
 def _cast(
     name: str,
     data_type: str,
     *,
     table_alias: str | None = None,
     type_map: Mapping[str, ex.DATA_TYPE] | None = None,
 ):
@@ -129,15 +61,15 @@
 
 valid_from_expr = ex.cast(
     ex.func("GETUTCDATE", dialect="tsql"), ex.DataType(this="datetime2(6)")
 ).as_(VALID_FROM_COL_NAME)
 
 
 def _get_cols_select(
-    cols: list[InformationSchemaColInfo],
+    cols: Sequence[InformationSchemaColInfo],
     *,
     is_deleted: bool | None = None,
     is_full: bool | None = None,
     with_valid_from: bool = False,
     table_alias: str | None = None,
     source_uses_compat: bool,
     data_type_map: Mapping[str, ex.DATA_TYPE] | None = None,
@@ -165,50 +97,29 @@
             [ex.cast(ex.convert(int(is_full)), "bit").as_(IS_FULL_LOAD_COL_NAME)]
             if is_full is not None
             else []
         )
     )
 
 
-def get_delta_col(
-    cols: list[InformationSchemaColInfo],
-) -> InformationSchemaColInfo | None:
-    row_start_col: InformationSchemaColInfo | None = None
-    for c in cols:
-        if c.data_type.lower() in ["rowversion", "timestamp"]:
-            return c
-        if c.generated_always_type_desc == "AS_ROW_START":
-            row_start_col = c
-    return row_start_col
-
-
 def _vacuum(source: DataSourceReader, dest: Destination):
     if source.local_delta_table_exists(dest):
         source.get_local_delta_ops(dest).vacuum()
 
 
-def write_db_to_delta(
-    source: DataSourceReader | str,
-    table: tuple[str, str],
-    destination: Destination | Path,
-    write_config: WriteConfig | None = None,
-):
-    if write_config is None:
-        write_config = WriteConfig()
-    if isinstance(destination, Path):
-        from .destination.file_system import FileSystemDestination
-
-        destination = cast(Destination, FileSystemDestination(destination))
-    if isinstance(source, str):
-        from .reader.odbc_reader import ODBCReader
-
-        source = ODBCReader(source)
+def exec_write_db_to_delta(infos: WriteConfigAndInfos):
+    write_config = infos.write_config
+    cols = infos.col_infos
+    pk_cols = infos.pk_cols
+    destination = infos.destination
+    source = infos.source
+    table = infos.table
     delta_path = destination / "delta"
-    cols = get_columns(source, table, dialect=write_config.dialect)
-    dest_logger = DeltaLogger(destination / "log", source, logging.getLogger(__name__))
+    dest_logger = infos.logger
+    delta_col = infos.delta_col
     (destination / "meta").mkdir()
     (destination / "meta/schema.json").upload_str(
         json.dumps(
             [c.model_dump() if is_pydantic_2 else c.dict() for c in cols], indent=4
         )
     )
     if source.local_delta_table_exists(
@@ -237,107 +148,42 @@
                 datetime.now(tz=timezone.utc) - lock_file_path.modified_time()
             ).total_seconds()
             > 60 * 60
         ):
             lock_file_path.remove()
         lock_file_path.upload_str("")
 
-        if write_config.delta_col:
-            delta_col = next(
-                (c for c in cols if c.column_name == write_config.delta_col), None
-            )
-            if delta_col is None:
-                delta_col = next(
-                    (
-                        c
-                        for c in cols
-                        if write_config.get_target_name(c) == write_config.delta_col
-                    ),
-                    None,
-                )
-            if delta_col is None:
-                raise ValueError(
-                    f"Delta column {write_config.delta_col} not found in source"
-                )
-        else:
-            delta_col = get_delta_col(cols)
-
-        _pks = write_config.primary_keys or get_primary_keys(
-            source, table, dialect=write_config.dialect
-        )
-        pk_cols: list[InformationSchemaColInfo] = []
-        for pk in _pks:
-            pk_col = next((c for c in cols if c.column_name == pk), None)
-            if pk_col is None:
-                pk_col = next(
-                    (c for c in cols if write_config.get_target_name(c) == pk), None
-                )
-            if pk_col is None:
-                raise ValueError(f"Primary key {pk} not found in source")
-            pk_cols.append(pk_col)
-        assert len(_pks) == len(pk_cols), f"Primary keys not found: {_pks}"
         if (
             not source.local_delta_table_exists(delta_path)
             or write_config.load_mode == "overwrite"
         ):
             delta_path.mkdir()
             dest_logger.info(f"{table}: Start Full Load")
-            do_full_load(
-                dest_logger,
-                source,
-                table,
-                delta_path,
-                mode="overwrite",
-                cols=cols,
-                pk_cols=pk_cols,
-                delta_col=delta_col,
-                write_config=write_config,
-            )
+            do_full_load(infos=infos, mode="overwrite")
         elif write_config.load_mode == "append_inserts":
             if delta_col is None and len(pk_cols) == 1 and pk_cols[0].is_identity:
                 delta_col = pk_cols[0]  # identity columns are usually increasing
+                infos = dataclasses.replace(infos, delta_col=delta_col)
             assert (
                 delta_col is not None
             ), "Must provide delta column for append_inserts load"
-            do_append_inserts_load(
-                dest_logger,
-                source,
-                table,
-                destination=destination,
-                delta_col=delta_col,
-                cols=cols,
-                write_config=write_config,
-            )
+            do_append_inserts_load(infos)
         else:
             if (
                 delta_col is None
                 or len(pk_cols) == 0
                 or write_config.load_mode == "force_full"
             ):
                 do_full_load(
-                    dest_logger,
-                    source,
-                    table,
-                    delta_path,
+                    infos=infos,
                     mode="append",
-                    cols=cols,
-                    pk_cols=pk_cols,
-                    delta_col=delta_col,
-                    write_config=write_config,
                 )
             else:
                 do_delta_load(
-                    dest_logger,
-                    source,
-                    table,
-                    destination=destination,
-                    delta_col=delta_col,
-                    cols=cols,
-                    pk_cols=pk_cols,
-                    write_config=write_config,
+                    infos=infos,
                     simple=write_config.load_mode == "simple_delta",
                 )
         lock_file_path.remove()
         _vacuum(
             source, destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION
         )
         _vacuum(source, destination / "delta_load" / DBDeltaPathConfigs.DELTA_1_NAME)
@@ -374,15 +220,15 @@
         base_destination / f"delta_load/{name}", name, version=version
     )
 
 
 def write_latest_pk(
     reader: DataSourceReader,
     destination: Destination,
-    pks: list[InformationSchemaColInfo],
+    pks: Sequence[InformationSchemaColInfo],
     delta_col: InformationSchemaColInfo,
     write_config: WriteConfig,
 ):
     reader.local_register_update_view(
         destination / f"delta_load/{DBDeltaPathConfigs.DELTA_1_NAME}",
         DBDeltaPathConfigs.DELTA_1_NAME,
     )
@@ -396,24 +242,24 @@
         DBDeltaPathConfigs.PRIMARY_KEYS_TS,
     )
 
     latest_pk_query = union(
         [
             ex.select(
                 *_get_cols_select(
-                    cols=pks + [delta_col],
+                    cols=concat_seq(pks, [delta_col]),
                     table_alias="au",
                     source_uses_compat=True,
                     get_target_name=write_config.get_target_name,
                 )
             ).from_(table_from_tuple("delta_2", alias="au")),
             (
                 ex.select(
                     *_get_cols_select(
-                        cols=pks + [delta_col],
+                        cols=concat_seq(pks, [delta_col]),
                         table_alias="d1",
                         source_uses_compat=True,
                         get_target_name=write_config.get_target_name,
                     )
                 )
                 .from_(ex.table_(DBDeltaPathConfigs.DELTA_1_NAME, alias="d1"))
                 .join(
@@ -432,15 +278,15 @@
                     ),
                     join_type="anti",
                 )
             ),
             (
                 ex.select(
                     *_get_cols_select(
-                        cols=pks + [delta_col],
+                        cols=concat_seq(pks, [delta_col]),
                         table_alias="cpk",
                         source_uses_compat=True,
                         get_target_name=write_config.get_target_name,
                     )
                 )
                 .from_(ex.table_(DBDeltaPathConfigs.PRIMARY_KEYS_TS, alias="cpk"))
                 .join(
@@ -489,66 +335,47 @@
 def _temp_table(table: table_name_type):
     if isinstance(table, str):
         return "temp_" + table
     return "temp_" + "_".join(table)
 
 
 def do_delta_load(
-    logger: DeltaLogger,
-    reader: DataSourceReader,
-    table: table_name_type,
-    destination: Destination,
-    *,
-    delta_col: InformationSchemaColInfo,
-    cols: list[InformationSchemaColInfo],
-    pk_cols: list[InformationSchemaColInfo],
-    write_config: WriteConfig,
+    infos: WriteConfigAndInfos,
     simple=False,  # a simple delta load assumes that there are no deletes and no additional updates (eg, when soft-delete is implemented in source properly)
 ):
+    destination = infos.destination
+    logger = infos.logger
+    delta_col = infos.delta_col
+    write_config = infos.write_config
+    assert delta_col is not None, "Must have a delta_col for delta loads"
+    reader = infos.source
+    table = infos.table
     last_pk_path = (
         destination / f"delta_load/{DBDeltaPathConfigs.LATEST_PK_VERSION}"
         if not simple
         else None
     )
     logger.info(
-        f"{table}: Start { 'SIMPLE ' if simple else '' }Delta Load with Delta Column {delta_col.column_name} and pks: {', '.join((c.column_name for c in pk_cols))}"
+        f"{table}: Start { 'SIMPLE ' if simple else '' }Delta Load with Delta Column {delta_col.column_name} and pks: {', '.join((c.column_name for c in infos.pk_cols))}"
     )
 
     if last_pk_path and not reader.local_delta_table_exists(
         last_pk_path
     ):  # or do a full load?
         logger.warning(f"{table}: Primary keys missing, try to restore")
         try:
             from .write_utils.restore_pk import restore_last_pk
 
-            restore_success = restore_last_pk(
-                reader,
-                table,
-                destination,
-                delta_col,
-                pk_cols,
-                write_config=write_config,
-                logger=logger,
-            )
+            restore_success = restore_last_pk(infos=infos)
         except Exception as e:
             logger.warning(f"{table}: Could not restore primary keys: {e}")
             restore_success = False
         if not restore_success:
             logger.warning(f"{table}: No primary keys found, do a full load")
-            do_full_load(
-                logger,
-                reader,
-                table,
-                delta_path=destination / "delta",
-                mode="append",
-                cols=cols,
-                pk_cols=pk_cols,
-                delta_col=delta_col,
-                write_config=write_config,
-            )
+            do_full_load(infos=infos, mode="append")
             return
     old_pk_version = (
         reader.get_local_delta_ops(
             destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION
         ).version()
         if not simple
         else None
@@ -557,47 +384,43 @@
     delta_load_value = _get_latest_delta_value(
         reader, delta_path, table, delta_col, write_config
     )
 
     if delta_load_value is None:
         logger.warning(f"{table}: No delta load value, do a full load")
         do_full_load(
-            logger,
-            reader,
-            table,
-            delta_path,
+            infos=infos,
             mode="append",
-            cols=cols,
-            pk_cols=pk_cols,
-            delta_col=delta_col,
-            write_config=write_config,
         )
         return
     logger.info(
         f"{table}: Start delta step 1, get primary keys and timestamps. MAX({delta_col.column_name}): {delta_load_value}"
     )
     if not simple:
         _retrieve_primary_key_data(
             reader=reader,
             table=table,
             delta_col=delta_col,
-            pk_cols=pk_cols,
+            pk_cols=infos.pk_cols,
             destination=destination,
             write_config=write_config,
         )
 
     criterion = _cast(
         delta_col.column_name,
         delta_col.data_type,
         table_alias="t",
         type_map=write_config.data_type_map,
     ) > ex.convert(delta_load_value)
     logger.info(f"{table}: Start delta step 2, load updates by timestamp")
     upds_sql = _get_update_sql(
-        cols=cols, criterion=criterion, table=table, write_config=write_config
+        cols=infos.col_infos,
+        criterion=criterion,
+        table=table,
+        write_config=write_config,
     )
     logger.info("execute sql", load="delta", sub_load="delta_1", sql=upds_sql)
     _load_updates_to_delta(
         logger,
         reader,
         sql=upds_sql,
         delta_path=delta_path,
@@ -607,87 +430,84 @@
     if not simple:
         assert old_pk_version is not None
         _handle_additional_updates(
             logger,
             reader=reader,
             table=table,
             delta_path=delta_path,
-            pk_cols=pk_cols,
+            pk_cols=infos.pk_cols,
             delta_col=delta_col,
-            cols=cols,
+            cols=infos.col_infos,
             write_config=write_config,
             old_pk_version=old_pk_version,
         )
         reader.local_register_update_view(delta_path, _temp_table(table))
 
         logger.info(f"{table}: Start delta step 3.5, write meta for next delta load")
 
         write_latest_pk(
-            reader, destination, pk_cols, delta_col, write_config=write_config
+            reader, destination, infos.pk_cols, delta_col, write_config=write_config
         )
 
         logger.info(f"{table}: Start delta step 4.5, write deletes")
         do_deletes(
-            reader=reader,
-            destination=destination,
-            cols=cols,
-            pk_cols=pk_cols,
+            reader=infos.source,
+            destination=infos.destination,
+            cols=infos.col_infos,
+            pk_cols=infos.pk_cols,
             old_pk_version=old_pk_version,
-            write_config=write_config,
+            write_config=infos.write_config,
         )
         logger.info(f"{table}: Done delta load")
     else:
         if (destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION).exists():
             (destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION).remove(
                 True
             )
 
 
-def do_append_inserts_load(
-    logger: DeltaLogger,
-    reader: DataSourceReader,
-    table: table_name_type,
-    destination: Destination,
-    *,
-    delta_col: InformationSchemaColInfo,
-    cols: list[InformationSchemaColInfo],
-    write_config: WriteConfig,
-):
+def do_append_inserts_load(infos: WriteConfigAndInfos):
+    logger = infos.logger
+    write_config = infos.write_config
+    assert infos.delta_col is not None, "must have a delta col"
     logger.info(
-        f"{table}: Start Append Only Load with Delta Column {delta_col.column_name}"
+        f"{infos.table}: Start Append Only Load with Delta Column {infos.delta_col.column_name}"
     )
-    delta_path = destination / "delta"
+    delta_path = infos.destination / "delta"
     delta_load_value = _get_latest_delta_value(
-        reader, delta_path, table, delta_col, write_config
+        infos.source, delta_path, infos.table, infos.delta_col, infos.write_config
     )
 
     criterion = (
         _cast(
-            delta_col.column_name,
-            delta_col.data_type,
+            infos.delta_col.column_name,
+            infos.delta_col.data_type,
             table_alias="t",
             type_map=write_config.data_type_map,
         )
         > ex.convert(delta_load_value)
         if delta_load_value
         else None
     )
-    logger.info(f"{table}: Start delta step 2, load updates by timestamp")
+    logger.info(f"{infos.table}: Start delta step 2, load updates by timestamp")
     _load_updates_to_delta(
         logger,
-        reader,
+        infos.source,
         sql=_get_update_sql(
-            cols=cols, criterion=criterion, table=table, write_config=write_config
+            cols=infos.col_infos,
+            criterion=criterion,
+            table=infos.table,
+            write_config=write_config,
         ),
         delta_path=delta_path,
         delta_name="delta_1",
         write_config=write_config,
     )
 
-    logger.info(f"{table}: Done Append only load")
+    logger.info(f"{infos.table}: Done Append only load")
 
 
 def _get_latest_delta_value(
     reader: DataSourceReader,
     delta_path: Destination,
     table: table_name_type,
     delta_col: InformationSchemaColInfo,
@@ -707,16 +527,16 @@
     )[0]["max_ts"]
 
 
 def do_deletes(
     reader: DataSourceReader,
     destination: Destination,
     # delta_table: DeltaTable,
-    cols: list[InformationSchemaColInfo],
-    pk_cols: list[InformationSchemaColInfo],
+    cols: Sequence[InformationSchemaColInfo],
+    pk_cols: Sequence[InformationSchemaColInfo],
     old_pk_version: int,
     write_config: WriteConfig,
 ):
     reader.local_register_update_view(
         destination / f"delta_load/{ DBDeltaPathConfigs.LATEST_PK_VERSION}",
         DBDeltaPathConfigs.LATEST_PK_VERSION,
     )
@@ -808,23 +628,23 @@
         )
 
 
 def _retrieve_primary_key_data(
     reader: DataSourceReader,
     table: table_name_type,
     delta_col: InformationSchemaColInfo,
-    pk_cols: list[InformationSchemaColInfo],
+    pk_cols: Sequence[InformationSchemaColInfo],
     destination: Destination,
     write_config: WriteConfig,
 ):
     pk_ts_col_select = ex.select(
         *_get_cols_select(
             is_full=None,
             is_deleted=None,
-            cols=pk_cols + [delta_col],
+            cols=concat_seq(pk_cols, [delta_col]),
             with_valid_from=False,
             data_type_map=write_config.data_type_map,
             source_uses_compat=False,
             get_target_name=write_config.get_target_name,
         )
     ).from_(table_from_tuple(table))
     pk_ts_reader_sql = pk_ts_col_select.sql(write_config.dialect)
@@ -852,23 +672,23 @@
 
 
 def _handle_additional_updates(
     logger: DeltaLogger,
     reader: DataSourceReader,
     table: table_name_type,
     delta_path: Destination,
-    pk_cols: list[InformationSchemaColInfo],
+    pk_cols: Sequence[InformationSchemaColInfo],
     delta_col: InformationSchemaColInfo,
-    cols: list[InformationSchemaColInfo],
+    cols: Sequence[InformationSchemaColInfo],
     write_config: WriteConfig,
     old_pk_version: int,
 ):
     """Handles updates that are not logical by their timestamp. This can happen on a restore from backup, for example."""
     folder = delta_path.parent
-    pk_ds_cols = pk_cols + [delta_col]
+    pk_ds_cols = concat_seq(pk_cols, [delta_col])
     reader.local_register_update_view(
         folder / f"delta_load/{ DBDeltaPathConfigs.PRIMARY_KEYS_TS}",
         DBDeltaPathConfigs.PRIMARY_KEYS_TS,
     )
     LAST_PK_VERSION = "LAST_PK_VERSION"
     reader.local_register_update_view(
         folder / f"delta_load/{ DBDeltaPathConfigs.LATEST_PK_VERSION}",
@@ -1082,15 +902,15 @@
             sg.from_("delta_2").select(ex.Star()),
             delta_path,
             mode="append",
         )
 
 
 def _get_update_sql(
-    cols: list[InformationSchemaColInfo],
+    cols: Sequence[InformationSchemaColInfo],
     criterion: str | Sequence[str | ex.Expression] | ex.Expression | None,
     table: table_name_type,
     write_config: WriteConfig,
 ):
     if isinstance(criterion, ex.Expression):
         criterion = [criterion]
     if isinstance(criterion, ex.Expression):
@@ -1132,79 +952,76 @@
     delta_name: str,
     write_config: WriteConfig,
 ):
     if isinstance(sql, ex.Query):
         sql = sql.sql(write_config.dialect)
 
     delta_name_path = delta_path.parent / f"delta_load/{delta_name}"
-    logger.info(f"Executing {sql}")
+    logger.info("Executing sql", load="delta", sub_load=delta_name, sql=sql)
     reader.source_write_sql_to_delta(sql, delta_name_path, mode="overwrite")
     reader.local_register_update_view(delta_name_path, delta_name)
     count = reader.local_execute_sql_to_py(count_limit_one(delta_name))[0]["cnt"]
     if count == 0:
         return
     reader.local_execute_sql_to_delta(
         sg.from_(delta_name).select(ex.Star()), delta_path, mode="append"
     )
 
 
-def do_full_load(
-    logger: DeltaLogger,
-    reader: DataSourceReader,
-    table: table_name_type,
-    delta_path: Destination,
-    mode: Literal["overwrite", "append"],
-    cols: list[InformationSchemaColInfo],
-    delta_col: InformationSchemaColInfo | None,
-    pk_cols: list[InformationSchemaColInfo],
-    write_config: WriteConfig,
-):
-    logger.info(f"{table}: Start Full Load")
+def do_full_load(infos: WriteConfigAndInfos, mode: Literal["overwrite", "append"]):
+    logger = infos.logger
+    write_config = infos.write_config
+    delta_path = infos.destination / "delta"
+    reader = infos.source
+    logger.info(f"{infos.table}: Start Full Load")
     sql = (
         ex.select(
             *_get_cols_select(
                 is_deleted=False,
                 is_full=True,
-                cols=cols,
+                cols=infos.col_infos,
                 with_valid_from=True,
                 data_type_map=write_config.data_type_map,
                 source_uses_compat=False,
                 get_target_name=write_config.get_target_name,
             )
         )
-        .from_(table_from_tuple(table))
+        .from_(table_from_tuple(infos.table))
         .sql(write_config.dialect)
     )
     if reader.local_delta_table_exists(
         delta_path, extended_check=True
     ):  # the extended check checks if there is any column in the table
-        reader.local_register_update_view(delta_path, _temp_table(table))
+        reader.local_register_update_view(delta_path, _temp_table(infos.table))
         res = reader.local_execute_sql_to_py(
-            sg.from_(ex.to_identifier(_temp_table(table))).select(
+            sg.from_(ex.to_identifier(_temp_table(infos.table))).select(
                 ex.func("max", ex.column(VALID_FROM_COL_NAME)).as_(VALID_FROM_COL_NAME)
             )
         )
         max_valid_from = res[0][VALID_FROM_COL_NAME] if res else None
     else:
         max_valid_from = None
         logger.info("executing sql", sql=sql, load="full")
     reader.source_write_sql_to_delta(sql, delta_path, mode=mode)
-    if delta_col is None:
-        logger.info(f"{table}: Full Load done")
+    if infos.delta_col is None:
+        logger.info(f"{infos.table}: Full Load done")
         return
-    logger.info(f"{table}: Full Load done, write meta for delta load")
+    logger.info(f"{infos.table}: Full Load done, write meta for delta load")
 
-    reader.local_register_update_view(delta_path, _temp_table(table))
+    reader.local_register_update_view(delta_path, _temp_table(infos.table))
     (delta_path.parent / "delta_load").mkdir()
-    query = sg.from_(ex.to_identifier(_temp_table(table))).select(
+    query = sg.from_(ex.to_identifier(_temp_table(infos.table))).select(
         *(
-            [ex.column(write_config.get_target_name(pk), quoted=True) for pk in pk_cols]
+            [
+                ex.column(write_config.get_target_name(pk), quoted=True)
+                for pk in infos.pk_cols
+            ]
             + (
-                [ex.column(write_config.get_target_name(delta_col), quoted=True)]
-                if delta_col
+                [ex.column(write_config.get_target_name(infos.delta_col), quoted=True)]
+                if infos.delta_col
                 else []
             )
         )
     )
     if max_valid_from:
         query = query.where(
             ex.column(VALID_FROM_COL_NAME, quoted=True) > ex.convert(max_valid_from)
```

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/delta_logger.py` & `odbc2deltalake-0.8.7/odbc2deltalake/delta_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,24 +112,31 @@
         if self.base_logger:
             self.base_logger.error(
                 message if isinstance(message, str) else json.dumps(message)
             )
         if len(self._pending_logs) > 10:
             self.flush()
 
+    def _append_fields(self, log: dict) -> dict:
+        log["logger_id"] = str(self.id)
+        return log
+
     def flush(self):
         dummy = LogMessage(
             message="",
             type="",
             date=datetime.now(tz=timezone.utc),
             sql="",
             load="",
             sub_load="",
             error_trackback="",
         )
         self.source.local_pylist_to_delta(
-            [p.model_dump() if is_pydantic_2 else p.dict() for p in self._pending_logs],
+            [
+                self._append_fields(p.model_dump() if is_pydantic_2 else p.dict())
+                for p in self._pending_logs
+            ],
             self.log_file_path,
             "append",
             dummy_record=dummy.model_dump() if is_pydantic_2 else dummy.dict(),
         )
         self._pending_logs.clear()
```

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/destination/azure.py` & `odbc2deltalake-0.8.7/odbc2deltalake/destination/azure.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/destination/azure_utils.py` & `odbc2deltalake-0.8.7/odbc2deltalake/destination/azure_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/destination/databricks.py` & `odbc2deltalake-0.8.7/odbc2deltalake/destination/databricks.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/destination/destination.py` & `odbc2deltalake-0.8.7/odbc2deltalake/destination/destination.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/destination/file_system.py` & `odbc2deltalake-0.8.7/odbc2deltalake/destination/file_system.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/metadata.py` & `odbc2deltalake-0.8.7/odbc2deltalake/metadata.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/odbc_utils.py` & `odbc2deltalake-0.8.7/odbc2deltalake/odbc_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/query.py` & `odbc2deltalake-0.8.7/odbc2deltalake/query.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/reader/odbc_reader.py` & `odbc2deltalake-0.8.7/odbc2deltalake/reader/odbc_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,48 +19,48 @@
         f = schema.field(n)
         if not f.nullable:
             sc = sc.set(i, f.with_nullable(True))
     return sc
 
 
 class ODBCReader(DataSourceReader):
-    def __init__(self, connection_string: str) -> None:
+    def __init__(self, connection_string: str, local_db: str = ":memory:") -> None:
         from deltalake import WriterProperties
 
         self.connection_string = connection_string
         self.writer_properties = WriterProperties(compression="ZSTD")
         self.duck_con = None
-        pass
+        self.local_db = local_db
 
     def local_register_update_view(
         self, delta_path: Destination, view_name: str, *, version: int | None = None
     ):
         import duckdb
         from deltalake2db import duckdb_create_view_for_delta
 
-        self.duck_con = self.duck_con or duckdb.connect()
+        self.duck_con = self.duck_con or duckdb.connect(self.local_db)
         dt = delta_path.as_delta_table()
         if version is not None:
             dt.load_as_version(version)
         duckdb_create_view_for_delta(self.duck_con, dt, view_name)
 
     def local_execute_sql_to_py(self, sql: Query) -> list[dict]:
         import duckdb
 
-        self.duck_con = self.duck_con or duckdb.connect()
+        self.duck_con = self.duck_con or duckdb.connect(self.local_db)
         with self.duck_con.cursor() as cursor:
             cursor.execute(sql.sql("duckdb"))
             assert cursor.description is not None
             col_names = [desc[0] for desc in cursor.description]
             return [dict(zip(col_names, row)) for row in cursor.fetchall()]
 
     def local_register_view(self, sql: Query, view_name: str):
         import duckdb
 
-        self.duck_con = self.duck_con or duckdb.connect()
+        self.duck_con = self.duck_con or duckdb.connect(self.local_db)
         self.duck_con.sql(f"CREATE OR REPLACE VIEW {view_name} AS {sql.sql('duckdb')}")
 
     def local_pylist_to_delta(
         self,
         pylist: list[dict],
         delta_path: Destination,
         mode: Literal["overwrite", "append"],
@@ -108,15 +108,15 @@
     def local_execute_sql_to_delta(
         self, sql: Query, delta_path: Destination, mode: Literal["overwrite", "append"]
     ):
         import duckdb
         from deltalake import write_deltalake
         from deltalake.exceptions import DeltaError
 
-        self.duck_con = self.duck_con or duckdb.connect()
+        self.duck_con = self.duck_con or duckdb.connect(self.local_db)
 
         with self.duck_con.cursor() as cur:
             cur.execute(sql.sql("duckdb"))
             dp, do = delta_path.as_path_options("object_store")
             batch_reader = cur.fetch_record_batch()
             schema = batch_reader.schema
             try:
```

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/reader/reader.py` & `odbc2deltalake-0.8.7/odbc2deltalake/reader/reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/reader/spark_reader.py` & `odbc2deltalake-0.8.7/odbc2deltalake/reader/spark_reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/sql_glot_utils.py` & `odbc2deltalake-0.8.7/odbc2deltalake/sql_glot_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/sql_schema.py` & `odbc2deltalake-0.8.7/odbc2deltalake/sql_schema.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.5/odbc2deltalake/write_utils/restore_pk.py` & `odbc2deltalake-0.8.7/odbc2deltalake/write_utils/restore_pk.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,165 +1,191 @@
-from odbc2deltalake.db_to_delta import (
+from odbc2deltalake.write_init import (
     IS_DELETED_COL_NAME,
     IS_FULL_LOAD_COL_NAME,
     VALID_FROM_COL_NAME,
     DBDeltaPathConfigs,
     WriteConfig,
 )
 from odbc2deltalake.delta_logger import DeltaLogger
 from odbc2deltalake.destination.destination import Destination
 from odbc2deltalake.metadata import InformationSchemaColInfo
 from odbc2deltalake.reader.reader import DataSourceReader
+from odbc2deltalake.write_init import WriteConfigAndInfos
 import sqlglot.expressions as ex
 import sqlglot as sg
 
 from odbc2deltalake.sql_glot_utils import count_limit_one
 
 table_name_type = str | tuple[str, str] | tuple[str, str, str]
 
 
 def _temp_table(table: table_name_type):
     if isinstance(table, str):
         return "temp_" + table
     return "temp_" + "_".join(table)
 
 
-def restore_last_pk(
-    reader: DataSourceReader,
-    table: table_name_type,
-    destination: Destination,
-    delta_col: InformationSchemaColInfo,
-    pk_cols: list[InformationSchemaColInfo],
-    write_config: WriteConfig,
-    logger: DeltaLogger,
+def create_last_pk_version_view(
+    infos: WriteConfigAndInfos,
+    view_prefix: str = "",
 ):
-    delta_path = destination / "delta"
-    reader.local_register_update_view(delta_path, _temp_table(table))
+    delta_path = infos.destination / "delta"
+    reader = infos.source
+    write_config = infos.write_config
+
+    temp_table = "tmp_" + str(hash(str(delta_path)))
+    reader.local_register_update_view(delta_path, temp_table)
 
     sq_valid_from = reader.local_execute_sql_to_py(
-        sg.from_(ex.to_identifier(_temp_table(table)))
+        sg.from_(ex.to_identifier(temp_table))
         .select(ex.func("max", ex.column(VALID_FROM_COL_NAME)).as_(VALID_FROM_COL_NAME))
         .where(ex.column(IS_FULL_LOAD_COL_NAME).eq(True))
     )
     if sq_valid_from is None or len(sq_valid_from) == 0:
-        return False
+        return None, None, False
+    assert infos.delta_col is not None, "must have a delta column"
     latest_full_load_date = sq_valid_from[0][VALID_FROM_COL_NAME]
     reader.local_register_view(
-        sg.from_(ex.table_(ex.to_identifier(_temp_table(table)), alias="tr"))
+        sg.from_(ex.table_(ex.to_identifier(temp_table), alias="tr"))
         .select(
             *(
-                [ex.column(write_config.get_target_name(c)) for c in pk_cols]
-                + [ex.column(delta_col.column_name), ex.column(VALID_FROM_COL_NAME)]
+                [ex.column(write_config.get_target_name(c)) for c in infos.pk_cols]
+                + [
+                    ex.column(write_config.get_target_name(infos.delta_col)),
+                    ex.column(VALID_FROM_COL_NAME),
+                ]
             ),
             copy=False
         )
         .where(
             ex.column(IS_FULL_LOAD_COL_NAME).eq(True)
             and ex.column(VALID_FROM_COL_NAME).eq(
                 ex.Subquery(
                     this=ex.select(ex.func("MAX", ex.column(VALID_FROM_COL_NAME, "ts")))
-                    .from_(ex.table_(ex.to_identifier(_temp_table(table)), alias="ts"))
+                    .from_(ex.table_(ex.to_identifier(temp_table), alias="ts"))
                     .where(ex.column(IS_FULL_LOAD_COL_NAME).eq(True))
                 )
             )
         ),
-        "last_full_load",
+        view_prefix + "last_full_load",
     )
 
     sq = (
-        sg.from_(ex.table_(_temp_table(table), alias="tr"))
+        sg.from_(ex.table_(temp_table, alias="tr"))
         .select(
             *(
-                [ex.column(write_config.get_target_name(c), "tr") for c in pk_cols]
-                + [ex.column(write_config.get_target_name(delta_col), "tr")]
+                [
+                    ex.column(write_config.get_target_name(c), "tr")
+                    for c in infos.pk_cols
+                ]
+                + [ex.column(write_config.get_target_name(infos.delta_col), "tr")]
                 + [ex.column(IS_DELETED_COL_NAME, "tr")]
                 + [ex.column(VALID_FROM_COL_NAME, "tr")]
             )
         )
         .where(ex.column(VALID_FROM_COL_NAME) > ex.convert(latest_full_load_date))
     )
     sq = sq.qualify(
         ex.EQ(
             this=ex.Window(
                 this=ex.RowNumber(),
                 partition_by=[
-                    ex.column(write_config.get_target_name(pk)) for pk in pk_cols
+                    ex.column(write_config.get_target_name(pk)) for pk in infos.pk_cols
                 ],
                 order=ex.Order(
                     expressions=[
                         ex.Ordered(
-                            this=ex.column(write_config.get_target_name(delta_col)),
+                            this=ex.column(VALID_FROM_COL_NAME),
                             desc=True,
                             nulls_first=False,
                         )
                     ]
                 ),
                 over="OVER",
             ),
             expression=ex.convert(1),
         )
     )
-    reader.local_register_view(sq, "delta_after_full_load")
+    reader.local_register_view(sq, view_prefix + "delta_after_full_load")
     last_pk_query = (
         sg.from_("base")
         .where(~ex.column(IS_DELETED_COL_NAME))
         .with_(
             "base",
             as_=ex.union(
-                left=sg.from_(ex.table_("delta_after_full_load", alias="df")).select(
+                left=sg.from_(
+                    ex.table_(view_prefix + "delta_after_full_load", alias="df")
+                ).select(
                     *(
                         [
                             ex.column(write_config.get_target_name(c), "df")
-                            for c in pk_cols
+                            for c in infos.pk_cols
                         ]
                         + [
-                            ex.column(write_config.get_target_name(delta_col), "df"),
+                            ex.column(
+                                write_config.get_target_name(infos.delta_col), "df"
+                            ),
                             ex.column(IS_DELETED_COL_NAME, "df"),
                         ]
                     )
                 ),
-                right=sg.from_(ex.table_("last_full_load", alias="f"))
+                right=sg.from_(ex.table_(view_prefix + "last_full_load", alias="f"))
                 .select(
                     *(
                         [
                             ex.column(write_config.get_target_name(c), "f")
-                            for c in pk_cols
+                            for c in infos.pk_cols
                         ]
                         + [
-                            ex.column(write_config.get_target_name(delta_col), "f"),
+                            ex.column(
+                                write_config.get_target_name(infos.delta_col), "f"
+                            ),
                             ex.convert(False).as_(IS_DELETED_COL_NAME),
                         ]
                     )
                 )
                 .join(
-                    ex.table_("delta_after_full_load", alias="d"),
+                    ex.table_(view_prefix + "delta_after_full_load", alias="d"),
                     join_type="anti",
                     on=ex.and_(
                         *[
                             ex.column(write_config.get_target_name(c), "f").eq(
                                 ex.column(write_config.get_target_name(c), "d")
                             )
-                            for c in pk_cols
+                            for c in infos.pk_cols
                         ]
                     ),
                 ),
                 distinct=False,
             ),
         )
         .select(ex.Star(**{"except": [ex.column(IS_DELETED_COL_NAME)]}), append=False)
     )
-    logger.info(
-        "Restoring last pk version", sql=last_pk_query.sql(reader.query_dialect)
-    )
     reader.local_register_view(
         last_pk_query,
-        "v_last_pk_version",
+        view_prefix + "last_pk_version",
     )
-    cnt = reader.local_execute_sql_to_py(count_limit_one("v_last_pk_version"))[0]["cnt"]
+    return last_pk_query, view_prefix + "last_pk_version", True
+
+
+def restore_last_pk(infos: WriteConfigAndInfos):
+    query, view_name, success = create_last_pk_version_view(
+        infos=infos,
+        view_prefix="v_odbc_load_",
+    )
+    if not success:
+        return False
+    assert query is not None
+    assert view_name is not None
+    infos.logger.info(
+        "Restoring last pk version", sql=query.sql(infos.source.query_dialect)
+    )
+
+    cnt = infos.source.local_execute_sql_to_py(count_limit_one(view_name))[0]["cnt"]
     if cnt == 0:
         return False
-    reader.local_execute_sql_to_delta(
-        sg.from_("v_last_pk_version").select(ex.Star()),
-        destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION,
+    infos.source.local_execute_sql_to_delta(
+        sg.from_(view_name).select(ex.Star()),
+        infos.destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION,
         mode="overwrite",
     )
     return True
```

### Comparing `odbc2deltalake-0.8.5/pyproject.toml` & `odbc2deltalake-0.8.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odbc2deltalake"
-version = "0.8.5"
+version = "0.8.7"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -28,14 +28,15 @@
 pytest = "^8.0.2"
 pytest-asyncio = "^0.23.5"
 pytest-order = "^1.2.0"
 pytest-cov = "^4.1.0"
 docker = "^7.0.0"
 python-dotenv = "^1.0.1"
 azure-storage-blob = "^12.19.1"
+pandas = "^2.2.2"
 
 
 [tool.poetry.group.spark.dependencies]
 delta-spark = "^3.1.0"
 
 [tool.poetry.extras]
 local = ["pyodbc", "deltalake2db", "arrow-odbc", "deltalake", "duckdb"]
```

### Comparing `odbc2deltalake-0.8.5/PKG-INFO` & `odbc2deltalake-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbc2deltalake
-Version: 0.8.5
+Version: 0.8.7
 Summary: 
 License: MIT
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


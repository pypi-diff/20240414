# Comparing `tmp/sqlrepo-0.1.1.tar.gz` & `tmp/sqlrepo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlrepo-0.1.1.tar", last modified: Fri Apr  5 13:38:55 2024, max compression
+gzip compressed data, was "sqlrepo-0.2.0.tar", last modified: Sun Apr 14 13:14:49 2024, max compression
```

## Comparing `sqlrepo-0.1.1.tar` & `sqlrepo-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,16 @@
--rw-r--r--   0        0        0       42 2024-04-05 13:35:41.660632 sqlrepo-0.1.1/README.md
--rw-r--r--   0        0        0     2962 2024-04-05 13:38:55.792411 sqlrepo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-0.1.1/sqlrepo/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-0.1.1/sqlrepo/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-0.1.1/sqlrepo/.pytest_cache/README.md
--rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-0.1.1/sqlrepo/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-0.1.1/sqlrepo/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-0.1.1/sqlrepo/__init__.py
--rw-r--r--   0        0        0      452 2024-04-05 11:55:17.627373 sqlrepo-0.1.1/sqlrepo/exc.py
--rw-r--r--   0        0        0      748 2024-02-01 12:42:25.901679 sqlrepo-0.1.1/sqlrepo/logging.py
--rw-r--r--   0        0        0    25304 2024-04-05 13:37:24.140459 sqlrepo-0.1.1/sqlrepo/queries.py
--rw-r--r--   0        0        0     9025 2024-04-05 11:56:15.997606 sqlrepo-0.1.1/sqlrepo/repositories.py
--rw-r--r--   0        0        0     2567 2024-04-05 11:55:46.626489 sqlrepo-0.1.1/sqlrepo/uow.py
--rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     6707 2024-03-14 08:50:16.900302 sqlrepo-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0    15461 2024-04-05 11:55:32.230431 sqlrepo-0.1.1/tests/test_base_queries.py
--rw-r--r--   0        0        0     9418 2024-04-05 11:55:40.630465 sqlrepo-0.1.1/tests/test_sync_queries.py
--rw-r--r--   0        0        0        0 2024-04-05 11:56:33.229687 sqlrepo-0.1.1/tests/test_uow.py
--rw-r--r--   0        0        0      820 2024-03-16 09:53:25.702604 sqlrepo-0.1.1/tests/types.py
--rw-r--r--   0        0        0     7107 2024-03-29 07:55:43.678659 sqlrepo-0.1.1/tests/utils.py
--rw-r--r--   0        0        0      386 1970-01-01 00:00:00.000000 sqlrepo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2024-04-14 11:04:24.825878 sqlrepo-0.2.0/README.md
+-rw-r--r--   0        0        0     3013 2024-04-14 13:14:49.595104 sqlrepo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-23 13:08:38.602420 sqlrepo-0.2.0/sqlrepo/__init__.py
+-rw-r--r--   0        0        0      452 2024-04-14 11:04:24.825878 sqlrepo-0.2.0/sqlrepo/exc.py
+-rw-r--r--   0        0        0      748 2024-04-14 11:18:40.730497 sqlrepo-0.2.0/sqlrepo/logging.py
+-rw-r--r--   0        0        0    26229 2024-04-14 13:11:15.769849 sqlrepo-0.2.0/sqlrepo/queries.py
+-rw-r--r--   0        0        0    15641 2024-04-14 13:11:24.489836 sqlrepo-0.2.0/sqlrepo/repositories.py
+-rw-r--r--   0        0        0     2565 2024-04-14 11:07:16.846888 sqlrepo-0.2.0/sqlrepo/uow.py
+-rw-r--r--   0        0        0        0 2024-02-23 13:08:38.602420 sqlrepo-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     6707 2024-04-14 11:07:16.846888 sqlrepo-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0    15461 2024-04-14 11:07:16.846888 sqlrepo-0.2.0/tests/test_base_queries.py
+-rw-r--r--   0        0        0     9417 2024-04-14 11:07:16.846888 sqlrepo-0.2.0/tests/test_sync_queries.py
+-rw-r--r--   0        0        0        0 2024-02-23 13:08:38.602420 sqlrepo-0.2.0/tests/test_uow.py
+-rw-r--r--   0        0        0      804 2024-04-14 11:07:16.846888 sqlrepo-0.2.0/tests/types.py
+-rw-r--r--   0        0        0     7107 2024-04-14 11:07:16.846888 sqlrepo-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0      395 1970-01-01 00:00:00.000000 sqlrepo-0.2.0/PKG-INFO
```

### Comparing `sqlrepo-0.1.1/pyproject.toml` & `sqlrepo-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,24 @@
 [tool.ruff]
+line-length = 100
+output-format = "full"
+exclude = [
+    ".git",
+    "__pycache__",
+    ".venv",
+    ".eggs",
+    "*.egg",
+    "dist",
+    "tests/fixtures/**",
+    "tests/**/snapshots/**",
+    "alembic",
+    "airich",
+]
+
+[tool.ruff.lint]
 select = [
     "A",
     "B",
     "D",
     "E",
     "F",
     "G",
@@ -27,55 +43,41 @@
     "SIM",
     "TCH",
     "INT",
     "PTH",
     "ERA",
     "TRY",
 ]
-line-length = 100
-show-source = true
-exclude = [
-    ".git",
-    "__pycache__",
-    ".venv",
-    ".eggs",
-    "*.egg",
-    "dist",
-    "tests/fixtures/**",
-    "tests/**/snapshots/**",
-    "alembic",
-    "airich",
-]
 ignore = [
     "D100",
     "B008",
     "D104",
     "Q000",
     "S101",
     "PT016",
     "ANN101",
     "ANN102",
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 ignore-decorators = [
     "typing.overload",
 ]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 11
 
-[tool.ruff.flake8-bugbear]
+[tool.ruff.lint.flake8-bugbear]
 extend-immutable-calls = [
     "fastapi.Depends",
     "fastapi.Query",
 ]
 
-[tool.ruff.extend-per-file-ignores]
+[tool.ruff.lint.extend-per-file-ignores]
 "__init__.py" = [
     "F401",
 ]
 "*/migrations/versions/*" = [
     "D103",
 ]
 "src/app/main.py" = [
@@ -168,24 +170,24 @@
     "httpx>=0.27.0",
     "pyment>=0.3.3",
     "ipython>=8.19.0",
 ]
 
 [project]
 name = "sqlrepo"
-version = "0.1.1"
+version = "0.2.0"
 description = "sqlalchemy repositories with crud operations and other utils for it."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = [
     "sqlalchemy>=2.0.29",
-    "python-dev-utils[filtering]>=0.1.1",
+    "python-dev-utils[sqlalchemy_filters]>=1.0.6",
 ]
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
```

### Comparing `sqlrepo-0.1.1/sqlrepo/logging.py` & `sqlrepo-0.2.0/sqlrepo/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
     "loggers": {
         "sqlrepo": {"handlers": ["console"], "level": "DEBUG"},
     },
 }
 
 
 logging.config.dictConfig(LOGGER_CONFIG)
-logger = logging.getLogger('sqlrepo')
+logger = logging.getLogger("sqlrepo")
```

### Comparing `sqlrepo-0.1.1/sqlrepo/queries.py` & `sqlrepo-0.2.0/sqlrepo/queries.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,44 +6,46 @@
 from dev_utils.sqlalchemy.filters.converters import BaseFilterConverter  # type: ignore
 from dev_utils.sqlalchemy.utils import (  # type: ignore
     apply_joins,
     apply_loads,
     get_sqlalchemy_attribute,
     get_utc_now,
 )
-from sqlalchemy import CursorResult, and_, delete, func, or_, select, text, update
+from sqlalchemy import CursorResult, and_, delete
 from sqlalchemy import exc as sqlalchemy_exc
+from sqlalchemy import func, or_, select, text, update
 from sqlalchemy.orm import joinedload
 
-from sqlrepo.logging import logger
+from sqlrepo.logging import logger as default_logger
 
 
 class JoinKwargs(TypedDict):
     """Kwargs for join statement."""
 
     isouter: NotRequired[bool]
     full: NotRequired[bool]
 
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
+    from logging import Logger
 
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import DeclarativeBase as Base
     from sqlalchemy.orm import QueryableAttribute
     from sqlalchemy.orm.attributes import InstrumentedAttribute
     from sqlalchemy.orm.session import Session
     from sqlalchemy.orm.strategy_options import _AbstractLoad  # type: ignore
     from sqlalchemy.sql._typing import _ColumnExpressionOrStrLabelArgument  # type: ignore
     from sqlalchemy.sql.dml import Delete, ReturningUpdate, Update
     from sqlalchemy.sql.elements import ColumnElement
     from sqlalchemy.sql.selectable import Select
 
-    BaseSQLAlchemyModel = TypeVar('BaseSQLAlchemyModel', bound=Base)
-    T = TypeVar('T')
+    BaseSQLAlchemyModel = TypeVar("BaseSQLAlchemyModel", bound=Base)
+    T = TypeVar("T")
     Count = int
     Deleted = bool
     Updated = bool
     Model = type[Base]
     JoinClause = ColumnElement[bool]
     ModelWithOnclause = tuple[Model, JoinClause]
     CompleteModel = tuple[Model, JoinClause, JoinKwargs]
@@ -53,122 +55,134 @@
     SearchParam = str | QueryableAttribute[Any]
     ColumnParam = str | QueryableAttribute[Any]
     OrderByParam = _ColumnExpressionOrStrLabelArgument[Any]
     DataDict = dict[str, Any]
 
 
 class BaseQuery:
+    """Base query class.
+
+    Implements base logic for queries like generating statements or filters. Don't use it directly.
+    """
 
     def __init__(
         self,
         filter_converter_class: type[BaseFilterConverter],
         specific_column_mapping: dict[str, "ColumnElement[Any]"] | None = None,
-        load_strategy: Callable[..., '_AbstractLoad'] = joinedload,
+        load_strategy: Callable[..., "_AbstractLoad"] = joinedload,
+        logger: "Logger" = default_logger,
     ) -> None:
         self.specific_column_mapping = specific_column_mapping
         self.filter_converter_class = filter_converter_class
         self.load_strategy = load_strategy
+        self.logger = logger
 
     def _resolve_specific_columns(
         self,
         *,
-        elements: 'Sequence[T]',
-    ) -> 'Sequence[T]':
+        elements: "Sequence[T]",
+    ) -> "Sequence[T]":
+        """Get all SQLAlchemy columns from strings (uses specific columns)."""
         if not self.specific_column_mapping:
             return elements
-        new_elements: 'list[T]' = []
+        new_elements: "list[T]" = []
         for ele in elements:
             if not isinstance(ele, str) or ele not in self.specific_column_mapping:
                 new_elements.append(ele)
             else:
                 new_elements.append(self.specific_column_mapping[ele])  # type: ignore
         return new_elements
 
     def _resolve_and_apply_joins(
         self,
         *,
-        stmt: 'Select[tuple[T]]',
-        joins: 'Sequence[Join]',
-    ) -> 'Select[tuple[T]]':
+        stmt: "Select[tuple[T]]",
+        joins: "Sequence[Join]",
+    ) -> "Select[tuple[T]]":
+        """Resolve joins from strings."""
         for join in joins:
             if isinstance(join, tuple | list):
                 target, clause, *kw_list = join
                 join_kwargs = kw_list[0] if len(kw_list) == 1 else JoinKwargs()
                 stmt = stmt.join(target, clause, **join_kwargs)
             elif isinstance(join, str):
                 stmt = apply_joins(stmt, join)
             else:
                 stmt = stmt.join(join)
         return stmt
 
     def _resolve_and_apply_loads(
         self,
         *,
-        stmt: 'Select[tuple[T]]',
-        loads: 'Sequence[Load]',
-    ) -> 'Select[tuple[T]]':
+        stmt: "Select[tuple[T]]",
+        loads: "Sequence[Load]",
+    ) -> "Select[tuple[T]]":
         for load in loads:
             stmt = (
                 apply_loads(stmt, load, load_strategy=self.load_strategy)
                 if isinstance(load, str)
                 else stmt.options(load)
             )
         return stmt
 
     def _make_disable_filters(  # noqa: C901
         self,
         *,
-        model: 'type[BaseSQLAlchemyModel]',
-        id_field: 'QueryableAttribute[Any]',
+        model: "type[BaseSQLAlchemyModel]",
+        id_field: "QueryableAttribute[Any]",
         ids_to_disable: set[Any],
-        disable_field: 'QueryableAttribute[Any]',
+        disable_field: "QueryableAttribute[Any]",
         field_type: type[datetime.datetime] | type[bool] = datetime.datetime,
         allow_filter_by_value: bool = True,
-        extra_filters: 'Filter | None' = None,
-    ) -> list['ColumnElement[bool]']:
-        filters: list['ColumnElement[bool]'] = list()
+        extra_filters: "Filter | None" = None,
+    ) -> list["ColumnElement[bool]"]:
+        """Generate disable filters from given data."""
+        filters: list["ColumnElement[bool]"] = list()
         filters.append(id_field.in_(ids_to_disable))
         if allow_filter_by_value and field_type == bool:
             filters.append(disable_field.is_not(True))
         elif allow_filter_by_value and field_type == datetime.datetime:
             filters.append(disable_field.is_(None))
         if extra_filters is not None:
             sqlalchemy_filters = self.filter_converter_class.convert(model, extra_filters)
             filters.extend(sqlalchemy_filters)
         return filters
 
     def _make_search_filter(
         self,
         search: str,
-        model: type['BaseSQLAlchemyModel'],
-        *search_by_args: 'SearchParam',
+        model: type["BaseSQLAlchemyModel"],
+        *search_by_args: "SearchParam",
         use_and_clause: bool = False,
-        # TODO: добавить флаг case_insensitive: bool = True
-    ) -> 'ColumnElement[bool]':
-        filters: list['ColumnElement[bool]'] = []
+        case_insensitive: bool = True,
+    ) -> "ColumnElement[bool]":
+        """Generate search filters from given data."""
+        filters: list["ColumnElement[bool]"] = []
         search_by_args = self._resolve_specific_columns(elements=search_by_args)  # type: ignore
         for search_by in search_by_args:
             if isinstance(search_by, str):
-                column = get_sqlalchemy_attribute(model, search_by)
-                clause = column.ilike(f'%{search}%')
-                filters.append(clause)
-            else:
-                filters.append(search_by.ilike(f'%{search}%'))
+                search_by = get_sqlalchemy_attribute(model, search_by)
+            (
+                filters.append(search_by.ilike(f"%{search}%"))
+                if case_insensitive
+                else search_by.like(f"%{search}%")
+            )
         if use_and_clause:
             return and_(*filters)
         return or_(*filters)
 
     def _get_item_stmt(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        filters: 'Filter | None' = None,
-        joins: 'Sequence[Join] | None' = None,
-        loads: 'Sequence[Load] | None' = None,
-    ) -> 'Select[tuple[BaseSQLAlchemyModel]]':
+        model: type["BaseSQLAlchemyModel"],
+        filters: "Filter | None" = None,
+        joins: "Sequence[Join] | None" = None,
+        loads: "Sequence[Load] | None" = None,
+    ) -> "Select[tuple[BaseSQLAlchemyModel]]":
+        """Generate SQLAlchemy stmt to get one item from filters, joins and loads."""
         stmt = select(model)
         if joins is not None:
             stmt = self._resolve_and_apply_joins(stmt=stmt, joins=joins)
         if loads is not None:
             stmt = self._resolve_and_apply_loads(
                 stmt=stmt,
                 loads=loads,
@@ -177,45 +191,45 @@
             sqlalchemy_filters = self.filter_converter_class.convert(model, filters)
             stmt = stmt.where(*sqlalchemy_filters)
         return stmt
 
     def _get_items_count_stmt(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        joins: 'Sequence[Join] | None' = None,
-        filters: 'Filter | None' = None,
-    ) -> 'Select[tuple[int]]':
+        model: type["BaseSQLAlchemyModel"],
+        joins: "Sequence[Join] | None" = None,
+        filters: "Filter | None" = None,
+    ) -> "Select[tuple[int]]":
+        """Generate SQLAlchemy stmt to get count of items from filters and joins."""
         stmt = select(func.count()).select_from(model)
         if joins is not None:
             stmt = self._resolve_and_apply_joins(stmt=stmt, joins=joins)
         if filters is not None:
             sqlalchemy_filters = self.filter_converter_class.convert(model, filters)
             stmt = stmt.where(*sqlalchemy_filters)
         return stmt
 
     def _get_item_list_stmt(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        joins: 'Sequence[Join] | None' = None,
-        loads: 'Sequence[Load] | None' = None,
-        filters: 'Filter | None' = None,
+        model: type["BaseSQLAlchemyModel"],
+        joins: "Sequence[Join] | None" = None,
+        loads: "Sequence[Load] | None" = None,
+        filters: "Filter | None" = None,
         search: str | None = None,
-        search_by: 'Sequence[SearchParam] | None' = None,
-        order_by: 'Sequence[OrderByParam] | None' = None,
+        search_by: "Sequence[SearchParam] | None" = None,
+        order_by: "Sequence[OrderByParam] | None" = None,
         limit: int | None = None,
         offset: int | None = None,
-    ) -> 'Select[tuple[BaseSQLAlchemyModel]]':
+    ) -> "Select[tuple[BaseSQLAlchemyModel]]":
+        """Generate SQLAlchemy stmt to get list of items from given data."""
         stmt = self._get_item_stmt(model=model, filters=filters, joins=joins, loads=loads)
         if search is not None and search_by is not None:
-            # TODO: нужно проверить, действительно ли escape и transform нужны. Может, оно только
-            #       создает баги.
             search = re.escape(search)
-            search = search.translate(str.maketrans({'%': r'\%', '_': r'\_', '/': r'\/'}))
+            search = search.translate(str.maketrans({"%": r"\%", "_": r"\_", "/": r"\/"}))
             stmt = stmt.where(self._make_search_filter(search, model, *search_by))
         if order_by is not None:
             order_by_resolved = self._resolve_specific_columns(elements=order_by)
             order_by_resolved = [
                 text(ele) if isinstance(ele, str) else ele for ele in order_by_resolved
             ]
             stmt = stmt.order_by(*order_by_resolved)
@@ -224,63 +238,65 @@
         if offset is not None:
             stmt = stmt.offset(offset)
         return stmt
 
     def _db_update_stmt(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        data: 'DataDict',
-        # TODO: add joins for it (because of filters - they can be nested.)
-        filters: 'Filter | None' = None,
-    ) -> 'ReturningUpdate[tuple[BaseSQLAlchemyModel]]':
+        model: type["BaseSQLAlchemyModel"],
+        data: "DataDict",
+        filters: "Filter | None" = None,
+    ) -> "ReturningUpdate[tuple[BaseSQLAlchemyModel]]":
+        """Generate SQLAlchemy stmt to update items with given data."""
         stmt = update(model)
         if filters is not None:
             sqlalchemy_filters = self.filter_converter_class.convert(model, filters)
             stmt = stmt.where(*sqlalchemy_filters)
         stmt = stmt.values(**data).returning(model)
         return stmt
 
     def _db_delete_stmt(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        filters: 'Filter | None' = None,
-    ) -> 'Delete':
+        model: type["BaseSQLAlchemyModel"],
+        filters: "Filter | None" = None,
+    ) -> "Delete":
+        """Generate SQLAlchemy stmt to delete items with given data."""
         stmt = delete(model)
         if filters is not None:
             sqlalchemy_filters = self.filter_converter_class.convert(model, filters)
             stmt = stmt.where(*sqlalchemy_filters)
         return stmt
 
     def _disable_items_stmt(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
+        model: type["BaseSQLAlchemyModel"],
         ids_to_disable: set[Any],
-        id_field: 'InstrumentedAttribute[Any]',
-        disable_field: 'InstrumentedAttribute[Any]',
+        id_field: "InstrumentedAttribute[Any]",
+        disable_field: "InstrumentedAttribute[Any]",
         field_type: type[datetime.datetime] | type[bool] = datetime.datetime,
         allow_filter_by_value: bool = True,
-        extra_filters: 'Filter | None' = None,
-    ) -> 'Update':
+        extra_filters: "Filter | None" = None,
+    ) -> "Update":
+        """Generate SQLAlchemy stmt to disable items with given data."""
         if issubclass(field_type, bool):
             field_value = True
         elif issubclass(field_type, datetime.datetime):  # type: ignore
             field_value = get_utc_now()
         else:
             msg = (
                 'Parameter "field_type" should be one of the following: bool, datetime. '
-                f'{field_type} was passed.'
+                f"{field_type} was passed."
             )
-            logger.error(msg)
+            self.logger.error(msg)
             raise TypeError(msg)
         if len(ids_to_disable) == 0:
             msg = 'Parameter "ids_to_disable" should contains at least one element.'
-            logger.error(msg)
+            self.logger.error(msg)
             raise ValueError(msg)
         filters = self._make_disable_filters(
             model=model,
             ids_to_disable=ids_to_disable,
             id_field=id_field,
             disable_field=disable_field,
             field_type=field_type,
@@ -288,48 +304,50 @@
             extra_filters=extra_filters,
         )
         stmt = update(model).where(*filters).values({disable_field: field_value})
         return stmt
 
 
 class BaseSyncQuery(BaseQuery):
+    """Base query class with sync interface."""
 
     def __init__(
         self,
-        session: 'Session',
+        session: "Session",
         filter_converter_class: type[BaseFilterConverter],
         specific_column_mapping: dict[str, "ColumnElement[Any]"] | None = None,
-        load_strategy: Callable[[Any], '_AbstractLoad'] = joinedload,
+        load_strategy: Callable[[Any], "_AbstractLoad"] = joinedload,
+        logger: "Logger" = default_logger,
     ) -> None:
         self.session = session
-        super().__init__(filter_converter_class, specific_column_mapping, load_strategy)
+        super().__init__(filter_converter_class, specific_column_mapping, load_strategy, logger)
 
     def get_item(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        filters: 'Filter | None' = None,
-        joins: 'Sequence[Join] | None' = None,
-        loads: 'Sequence[Load] | None' = None,
-    ) -> 'BaseSQLAlchemyModel | None':
+        model: type["BaseSQLAlchemyModel"],
+        filters: "Filter | None" = None,
+        joins: "Sequence[Join] | None" = None,
+        loads: "Sequence[Load] | None" = None,
+    ) -> "BaseSQLAlchemyModel | None":
         stmt = self._get_item_stmt(
             model=model,
             filters=filters,
             joins=joins,
             loads=loads,
         )
         result = self.session.scalars(stmt)
         return result.first()
 
     def get_items_count(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        joins: 'Sequence[Join] | None' = None,
-        filters: 'Filter | None' = None,
+        model: type["BaseSQLAlchemyModel"],
+        joins: "Sequence[Join] | None" = None,
+        filters: "Filter | None" = None,
     ) -> int:
         stmt = self._get_items_count_stmt(
             model=model,
             joins=joins,
             filters=filters,
         )
         count = self.session.scalar(stmt)
@@ -337,25 +355,25 @@
         if count is None:  # pragma: no cover
             count = 0
         return count
 
     def get_item_list(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        joins: 'Sequence[Join] | None' = None,
-        loads: 'Sequence[Load] | None' = None,
-        filters: 'Filter | None' = None,
+        model: type["BaseSQLAlchemyModel"],
+        joins: "Sequence[Join] | None" = None,
+        loads: "Sequence[Load] | None" = None,
+        filters: "Filter | None" = None,
         search: str | None = None,
-        search_by: 'Sequence[SearchParam] | None' = None,
-        order_by: 'Sequence[OrderByParam] | None' = None,
+        search_by: "Sequence[SearchParam] | None" = None,
+        order_by: "Sequence[OrderByParam] | None" = None,
         limit: int | None = None,
         offset: int | None = None,
         unique_items: bool = False,
-    ) -> 'Sequence[BaseSQLAlchemyModel]':
+    ) -> "Sequence[BaseSQLAlchemyModel]":
         stmt = self._get_item_list_stmt(
             model=model,
             joins=joins,
             loads=loads,
             filters=filters,
             search=search,
             search_by=search_by,
@@ -367,41 +385,41 @@
         if unique_items:
             return result.unique().all()
         return result.all()
 
     def create_item(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
+        model: type["BaseSQLAlchemyModel"],
         # TODO: add sequence of data to make more than one object at the same time.
-        data: 'DataDict | None' = None,
+        data: "DataDict | None" = None,
         use_flush: bool = False,
-    ) -> 'BaseSQLAlchemyModel':
+    ) -> "BaseSQLAlchemyModel":
         item = model() if data is None else model(**data)
         self.session.add(item)
         if use_flush:
             self.session.flush()
         else:
             self.session.commit()
 
         msg = (
             f"Create row in database. Item: {item}. "
             f"{'Flush used.' if use_flush else 'Commit used.'}."
         )
-        logger.debug(msg)
+        self.logger.debug(msg)
         return item
 
     def db_update(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        data: 'DataDict',
-        filters: 'Filter | None' = None,
+        model: type["BaseSQLAlchemyModel"],
+        data: "DataDict",
+        filters: "Filter | None" = None,
         use_flush: bool = False,
-    ) -> 'Sequence[BaseSQLAlchemyModel]':
+    ) -> "Sequence[BaseSQLAlchemyModel]":
         stmt = self._db_update_stmt(
             model=model,
             data=data,
             filters=filters,
         )
         result = self.session.scalars(stmt)
         if use_flush:
@@ -409,52 +427,52 @@
         else:
             self.session.commit()
         return result.unique().all()
 
     def change_item(
         self,
         *,
-        data: 'DataDict',
+        data: "DataDict",
         # TODO: add sequence items to make more than one object update at the same time.
-        item: 'BaseSQLAlchemyModel',
+        item: "BaseSQLAlchemyModel",
         set_none: bool = False,
-        allowed_none_fields: 'Literal["*"] | set[str]' = '*',
+        allowed_none_fields: 'Literal["*"] | set[str]' = "*",
         use_flush: bool = False,
-    ) -> 'tuple[Updated, BaseSQLAlchemyModel]':
+    ) -> "tuple[Updated, BaseSQLAlchemyModel]":
         is_updated = False
         if not set_none:
             data = {key: value for key, value in data.items() if value is not None}
         for field, value in data.items():
             if (
                 set_none
                 and value is None
-                and (allowed_none_fields != '*' and field not in allowed_none_fields)
+                and (allowed_none_fields != "*" and field not in allowed_none_fields)
             ):
                 continue
             if not is_updated and getattr(item, field, None) != value:
                 is_updated = True
             setattr(item, field, value)
         if use_flush:
             self.session.flush()
         else:
             self.session.commit()
         msg = (
-            f'Update database row success. Item: {repr(item)}. Params: {data}, '
-            f'set_none: {set_none}, use_flush: {use_flush}.'
+            f"Update database row success. Item: {repr(item)}. Params: {data}, "
+            f"set_none: {set_none}, use_flush: {use_flush}."
         )
-        logger.debug(msg)
+        self.logger.debug(msg)
         return is_updated, item
 
     def db_delete(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        filters: 'Filter | None' = None,
+        model: type["BaseSQLAlchemyModel"],
+        filters: "Filter | None" = None,
         use_flush: bool = False,
-    ) -> 'Count':
+    ) -> "Count":
         stmt = self._db_delete_stmt(
             model=model,
             filters=filters,
         )
         result = self.session.execute(stmt)
         if use_flush:
             self.session.flush()
@@ -463,45 +481,45 @@
         if isinstance(result, CursorResult):  # type: ignore
             return result.rowcount
         return 0
 
     def delete_item(
         self,
         *,
-        item: 'Base',
+        item: "Base",
         use_flush: bool = False,
-    ) -> 'Deleted':
+    ) -> "Deleted":
         item_repr = repr(item)
         try:
             self.session.delete(item)
             if use_flush:
                 self.session.flush()
             else:
                 self.session.commit()
         except sqlalchemy_exc.SQLAlchemyError as exc:
             self.session.rollback()
-            msg = f'Delete from database error: {exc}'  # noqa: S608
-            logger.warning(msg)
+            msg = f"Delete from database error: {exc}"  # noqa: S608
+            self.logger.warning(msg)
             return False
-        msg = f'Delete from database success. Item: {item_repr}'  # noqa: S608
-        logger.debug(msg)
+        msg = f"Delete from database success. Item: {item_repr}"  # noqa: S608
+        self.logger.debug(msg)
         return True
 
     def disable_items(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
+        model: type["BaseSQLAlchemyModel"],
         ids_to_disable: set[Any],
-        id_field: 'InstrumentedAttribute[Any]',
-        disable_field: 'InstrumentedAttribute[Any]',
+        id_field: "InstrumentedAttribute[Any]",
+        disable_field: "InstrumentedAttribute[Any]",
         field_type: type[datetime.datetime] | type[bool] = datetime.datetime,
         allow_filter_by_value: bool = True,
-        extra_filters: 'Filter | None' = None,
+        extra_filters: "Filter | None" = None,
         use_flush: bool = False,
-    ) -> 'Count':
+    ) -> "Count":
         stmt = self._disable_items_stmt(
             model=model,
             ids_to_disable=ids_to_disable,
             id_field=id_field,
             disable_field=disable_field,
             field_type=field_type,
             allow_filter_by_value=allow_filter_by_value,
@@ -516,48 +534,50 @@
             self.session.commit()
         if isinstance(result, CursorResult):  # type: ignore
             return result.rowcount
         return 0
 
 
 class BaseAsyncQuery(BaseQuery):
+    """Base query class with async interface."""
 
     def __init__(
         self,
-        session: 'AsyncSession',
+        session: "AsyncSession",
         filter_converter_class: type[BaseFilterConverter],
         specific_column_mapping: dict[str, "ColumnElement[Any]"] | None = None,
-        load_strategy: Callable[..., '_AbstractLoad'] = joinedload,
+        load_strategy: Callable[..., "_AbstractLoad"] = joinedload,
+        logger: "Logger" = default_logger,
     ) -> None:
         self.session = session
-        super().__init__(filter_converter_class, specific_column_mapping, load_strategy)
+        super().__init__(filter_converter_class, specific_column_mapping, load_strategy, logger)
 
     async def get_item(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        filters: 'Filter | None' = None,
-        joins: 'Sequence[Join] | None' = None,
-        loads: 'Sequence[Load] | None' = None,
-    ) -> 'BaseSQLAlchemyModel | None':
+        model: type["BaseSQLAlchemyModel"],
+        filters: "Filter | None" = None,
+        joins: "Sequence[Join] | None" = None,
+        loads: "Sequence[Load] | None" = None,
+    ) -> "BaseSQLAlchemyModel | None":
         stmt = self._get_item_stmt(
             model=model,
             filters=filters,
             joins=joins,
             loads=loads,
         )
         result = await self.session.scalars(stmt)
         return result.first()
 
     async def get_items_count(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        joins: 'Sequence[Join] | None' = None,
-        filters: 'Filter | None' = None,
+        model: type["BaseSQLAlchemyModel"],
+        joins: "Sequence[Join] | None" = None,
+        filters: "Filter | None" = None,
     ) -> int:
         stmt = self._get_items_count_stmt(
             model=model,
             joins=joins,
             filters=filters,
         )
         count = await self.session.scalar(stmt)
@@ -565,25 +585,25 @@
         if count is None:  # pragma: no cover
             count = 0
         return count
 
     async def get_item_list(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        joins: 'Sequence[Join] | None' = None,
-        loads: 'Sequence[Load] | None' = None,
-        filters: 'Filter | None' = None,
+        model: type["BaseSQLAlchemyModel"],
+        joins: "Sequence[Join] | None" = None,
+        loads: "Sequence[Load] | None" = None,
+        filters: "Filter | None" = None,
         search: str | None = None,
-        search_by: 'Sequence[SearchParam] | None' = None,
-        order_by: 'Sequence[OrderByParam] | None' = None,
+        search_by: "Sequence[SearchParam] | None" = None,
+        order_by: "Sequence[OrderByParam] | None" = None,
         limit: int | None = None,
         offset: int | None = None,
         unique_items: bool = False,
-    ) -> 'Sequence[BaseSQLAlchemyModel]':
+    ) -> "Sequence[BaseSQLAlchemyModel]":
         stmt = self._get_item_list_stmt(
             model=model,
             joins=joins,
             loads=loads,
             filters=filters,
             search=search,
             search_by=search_by,
@@ -595,40 +615,40 @@
         if unique_items:
             return result.unique().all()
         return result.all()
 
     async def create_item(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        data: 'DataDict | None' = None,
+        model: type["BaseSQLAlchemyModel"],
+        data: "DataDict | None" = None,
         use_flush: bool = False,
-    ) -> 'BaseSQLAlchemyModel':
+    ) -> "BaseSQLAlchemyModel":
         item = model() if data is None else model(**data)
         self.session.add(item)
         if use_flush:
             await self.session.flush()
         else:
             await self.session.commit()
 
         msg = (
             f"Create row in database. Item: {item}. "
             f"{'Flush used.' if use_flush else 'Commit used.'}."
         )
-        logger.debug(msg)
+        self.logger.debug(msg)
         return item
 
     async def db_update(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        data: 'DataDict',
-        filters: 'Filter | None' = None,
+        model: type["BaseSQLAlchemyModel"],
+        data: "DataDict",
+        filters: "Filter | None" = None,
         use_flush: bool = False,
-    ) -> 'Sequence[BaseSQLAlchemyModel] | None':
+    ) -> "Sequence[BaseSQLAlchemyModel] | None":
         stmt = self._db_update_stmt(
             model=model,
             data=data,
             filters=filters,
         )
         result = await self.session.scalars(stmt)
         if use_flush:
@@ -636,51 +656,51 @@
         else:
             await self.session.commit()
         return result.unique().all()
 
     async def change_item(
         self,
         *,
-        data: 'DataDict',
-        item: 'BaseSQLAlchemyModel',
+        data: "DataDict",
+        item: "BaseSQLAlchemyModel",
         set_none: bool = False,
-        allowed_none_fields: 'Literal["*"] | Sequence[str]' = '*',
+        allowed_none_fields: 'Literal["*"] | set[str]' = "*",
         use_flush: bool = False,
-    ) -> 'tuple[bool, BaseSQLAlchemyModel]':
+    ) -> "tuple[bool, BaseSQLAlchemyModel]":
         is_updated = False
         if not set_none:
             data = {key: value for key, value in data.items() if value is not None}
         for field, value in data.items():
             if (
                 set_none
                 and value is None
-                and (allowed_none_fields != '*' and field not in allowed_none_fields)
+                and (allowed_none_fields != "*" and field not in allowed_none_fields)
             ):
                 continue
             if not is_updated and getattr(item, field, None) != value:
                 is_updated = True
             setattr(item, field, value)
         if use_flush:
             await self.session.flush()
         else:
             await self.session.commit()
         msg = (
-            f'Update database row success. Item: {repr(item)}. Params: {data}, '
-            f'set_none: {set_none}, use_flush: {use_flush}.'
+            f"Update database row success. Item: {repr(item)}. Params: {data}, "
+            f"set_none: {set_none}, use_flush: {use_flush}."
         )
-        logger.debug(msg)
+        self.logger.debug(msg)
         return is_updated, item
 
     async def db_delete(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
-        filters: 'Filter | None' = None,
+        model: type["BaseSQLAlchemyModel"],
+        filters: "Filter | None" = None,
         use_flush: bool = False,
-    ) -> 'Count':
+    ) -> "Count":
         stmt = self._db_delete_stmt(
             model=model,
             filters=filters,
         )
         result = await self.session.execute(stmt)
         if use_flush:
             await self.session.flush()
@@ -689,45 +709,45 @@
         if isinstance(result, CursorResult):  # type: ignore
             return result.rowcount
         return 0
 
     async def delete_item(
         self,
         *,
-        item: 'Base',
+        item: "Base",
         use_flush: bool = False,
-    ) -> 'Deleted':
+    ) -> "Deleted":
         item_repr = repr(item)
         try:
             await self.session.delete(item)
             if use_flush:
                 await self.session.flush()
             else:
                 await self.session.commit()
         except sqlalchemy_exc.SQLAlchemyError as exc:
             await self.session.rollback()
-            msg = f'Delete from database error: {exc}'  # noqa: S608
-            logger.warning(msg)
+            msg = f"Delete from database error: {exc}"  # noqa: S608
+            self.logger.warning(msg)
             return False
-        msg = f'Delete from database success. Item: {item_repr}'  # noqa: S608
-        logger.debug(msg)
+        msg = f"Delete from database success. Item: {item_repr}"  # noqa: S608
+        self.logger.debug(msg)
         return True
 
     async def disable_items(
         self,
         *,
-        model: type['BaseSQLAlchemyModel'],
+        model: type["BaseSQLAlchemyModel"],
         ids_to_disable: set[Any],
-        id_field: 'InstrumentedAttribute[Any]',
-        disable_field: 'InstrumentedAttribute[Any]',
+        id_field: "InstrumentedAttribute[Any]",
+        disable_field: "InstrumentedAttribute[Any]",
         field_type: type[datetime.datetime] | type[bool] = datetime.datetime,
         allow_filter_by_value: bool = True,
-        extra_filters: 'Filter | None' = None,
+        extra_filters: "Filter | None" = None,
         use_flush: bool = False,
-    ) -> 'Count':
+    ) -> "Count":
         stmt = self._disable_items_stmt(
             model=model,
             ids_to_disable=ids_to_disable,
             id_field=id_field,
             disable_field=disable_field,
             field_type=field_type,
             allow_filter_by_value=allow_filter_by_value,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sqlrepo-0.1.1/sqlrepo/repositories.py` & `sqlrepo-0.2.0/sqlrepo/repositories.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import datetime
+import warnings
 from collections.abc import Callable
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Final,
+    ForwardRef,
     Generic,
     Literal,
     NotRequired,
     TypedDict,
     TypeVar,
     get_args,
 )
@@ -20,21 +22,24 @@
     SimpleFilterConverter,
 )
 from dev_utils.sqlalchemy.filters.types import FilterConverterStrategiesLiteral  # type: ignore
 from sqlalchemy.orm import DeclarativeBase as Base
 from sqlalchemy.orm import joinedload
 
 from sqlrepo import exc as sqlrepo_exc
-from sqlrepo.queries import BaseAsyncQuery
+from sqlrepo.logging import logger as default_logger
+from sqlrepo.queries import BaseAsyncQuery, BaseSyncQuery
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
+    from logging import Logger
 
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm.attributes import InstrumentedAttribute, QueryableAttribute
+    from sqlalchemy.orm.session import Session
     from sqlalchemy.orm.strategy_options import _AbstractLoad  # type: ignore
     from sqlalchemy.sql._typing import _ColumnExpressionOrStrLabelArgument  # type: ignore
     from sqlalchemy.sql.elements import ColumnElement
 
     class JoinKwargs(TypedDict):
         """Kwargs for join."""
 
@@ -51,131 +56,186 @@
     Load = str | _AbstractLoad
     SearchParam = str | QueryableAttribute[Any]
     OrderByParam = _ColumnExpressionOrStrLabelArgument[Any]
     DataDict = dict[str, Any]
 
 
 StrField = str
-BaseSQLAlchemyModel = TypeVar('BaseSQLAlchemyModel', bound=Base)
+BaseSQLAlchemyModel = TypeVar("BaseSQLAlchemyModel", bound=Base)
 
 
 class BaseRepository(Generic[BaseSQLAlchemyModel]):
-    _model_class: type['BaseSQLAlchemyModel']
+    """Base repository class.
+
+    Don't Use it directly. Use BaseAsyncRepository and BaseSyncRepository, or pass query_class
+    directly (not recommended.)
+    """
+
+    __inheritance_check_model_class__: bool = True
+    _model_class: type["BaseSQLAlchemyModel"]
 
     # TODO: добавить specific_column_mapping в фильтры, joins и loads.
-    specific_column_mapping: ClassVar['dict[str, ColumnElement[Any]]'] = {}
+    specific_column_mapping: ClassVar["dict[str, ColumnElement[Any]]"] = {}
+    """
+    Uses as mapping for some attributes, that you need to alias or need to specify column
+    from other models.
+
+    Warning: if you specify column from other model, it may cause errors. For example, update
+    doesn't use it for filters, because joins are not presents in update.
+    """
     use_flush: ClassVar[bool] = True
-    get_item_identity_field: ClassVar[StrField] = 'id'
-    disable_allow_filter_by_value: ClassVar[bool] = True
+    """
+    Uses as flag of flush method in SQLAlchemy session.
+
+    By default, True, because repository has (mostly) multiple methods evaluate use. For example,
+    generally, you want to create some model instances, create some other (for example, log table)
+    and then receive other model instance in one use (for example, in Unit of work pattern).
+
+    If you will work with repositories as single methods uses, switch to use_flush=False. It will
+    make queries commit any changes.
+    """
+    allow_disable_filter_by_value: ClassVar[bool] = True
+    """
+    Uses as flag of filtering in disable method.
+
+    If True, make additional filter, which will exclude items, which already disabled.
+    Logic of disable depends on type of disable column. See ``disable_field`` docstring for more
+    information.
+
+    By default True, because it will make more efficient query to not override disable column. In
+    some cases (like datetime disable field) it may be better to turn off this flag to save disable
+    with new context (repeat disable, if your domain supports repeat disable and it make sense).
+    """
     update_set_none: ClassVar[bool] = False
-    update_allowed_none_fields: ClassVar['Literal["*"] | Sequence[StrField]'] = '*'
+    update_allowed_none_fields: ClassVar['Literal["*"] | set[StrField]'] = "*"
     disable_field_type: ClassVar[type[datetime.datetime] | type[bool]] = datetime.datetime
     unique_list_items: ClassVar[bool] = False
-    filter_convert_strategy: ClassVar[FilterConverterStrategiesLiteral] = 'simple'
-    load_strategy: ClassVar[Callable[..., '_AbstractLoad']] = joinedload
-    id_field: ClassVar['InstrumentedAttribute[Any] | None'] = None
-    disable_field: ClassVar['InstrumentedAttribute[Any] | None'] = None
+    filter_convert_strategy: ClassVar[FilterConverterStrategiesLiteral] = "simple"
+    load_strategy: ClassVar[Callable[..., "_AbstractLoad"]] = joinedload
+    id_field: ClassVar["InstrumentedAttribute[Any] | None"] = None
+    disable_field: ClassVar["InstrumentedAttribute[Any] | None"] = None
 
     _filter_convert_classes: Final[
         dict[FilterConverterStrategiesLiteral, type[BaseFilterConverter]]
     ] = {
-        'simple': SimpleFilterConverter,
-        'advanced': AdvancedOperatorFilterConverter,
-        'django': DjangoLikeFilterConverter,
+        "simple": SimpleFilterConverter,
+        "advanced": AdvancedOperatorFilterConverter,
+        "django": DjangoLikeFilterConverter,
     }
 
     def __init_subclass__(cls) -> None:  # noqa: D105
-        if cls.__name__ == 'BaseAsyncRepository':  # TODO: or cls is BaseSyncRepository
-            return
-        if hasattr(cls, '_model_class'):
+        if hasattr(cls, "_model_class"):
             msg = (
                 "Don't change _model_class attribute to class. Use generic syntax instead. "
                 "See PEP 646 (https://peps.python.org/pep-0646/)"
             )
-            raise sqlrepo_exc.RepositoryAttributeError(msg)
+            warnings.warn(msg, stacklevel=2)
+            return
+        if cls.__inheritance_check_model_class__ is False:
+            cls.__inheritance_check_model_class__ = True
+            return
         try:
             # PEP-560: https://peps.python.org/pep-0560/
             # NOTE: this code is needed for getting type from generic: Generic[int] -> int type
             # get_args get params from __orig_bases__, that contains Generic passed types.
-            # FIXME: Может быть указана типизация через строчку, из-за чего в аргументах будет typing.ForwardRef
             model, *_ = get_args(cls.__orig_bases__[0])  # type: ignore
         except Exception as exc:
-            msg = f'Error during getting information about Generic types for {cls.__name__}.'
+            msg = f"Error during getting information about Generic types for {cls.__name__}."
             raise sqlrepo_exc.RepositoryAttributeError(msg) from exc
+        if isinstance(model, ForwardRef):
+            try:
+                model = eval(model.__forward_arg__)  # noqa: S307
+            except Exception as exc:
+                msg = (
+                    "Can't evaluate ForwardRef of generic type. "
+                    "Don't use type in generic with quotes. "
+                    f"Original exception: {str(exc)}"
+                )
+                warnings.warn(msg, stacklevel=2)
+                return
         if isinstance(model, TypeVar):
-            msg = 'GenericType was not passed for SQLAlchemy model declarative class.'
-            raise sqlrepo_exc.RepositoryAttributeError(msg)
+            msg = "GenericType was not passed for SQLAlchemy model declarative class."
+            warnings.warn(msg, stacklevel=2)
+            return
         if not issubclass(model, Base):
-            msg = 'Passed GenericType is not SQLAlchemy model declarative class.'
-            raise sqlrepo_exc.RepositoryAttributeError(msg)
+            msg = "Passed GenericType is not SQLAlchemy model declarative class."
+            warnings.warn(msg, stacklevel=2)
+            return
         cls._model_class = model  # type: ignore
 
     def get_filter_convert_class(self) -> type[BaseFilterConverter]:
         """Get filter convert class from passed strategy."""
         return self._filter_convert_classes[self.filter_convert_strategy]
 
 
 class BaseAsyncRepository(BaseRepository[BaseSQLAlchemyModel]):
-    """"""
+    """Base repository class with async interface.
+
+    Has main CRUD methods for working with model. Use async session of SQLAlchemy to work with this
+    class.
+    """
 
-    query_class: type['BaseAsyncQuery'] = BaseAsyncQuery
+    __inheritance_check_model_class__ = False
+    query_class: type["BaseAsyncQuery"] = BaseAsyncQuery
 
     def __init__(
         self,
-        session: 'AsyncSession',
+        session: "AsyncSession",
+        logger: "Logger" = default_logger,
     ) -> None:
         self.session = session
+        self.logger = logger
         self.queries = self.query_class(
             session,
             self.get_filter_convert_class(),
             self.specific_column_mapping,
             self.load_strategy,
         )
 
     async def get(
         self,
         *,
-        filters: 'Filter | None' = None,
-        joins: 'Sequence[Join] | None' = None,
-        loads: 'Sequence[Load] | None' = None,
-    ) -> 'BaseSQLAlchemyModel | None':
+        filters: "Filter | None" = None,
+        joins: "Sequence[Join] | None" = None,
+        loads: "Sequence[Load] | None" = None,
+    ) -> "BaseSQLAlchemyModel | None":
         result = await self.queries.get_item(
             model=self._model_class,
             joins=joins,
             loads=loads,
             filters=filters,
         )
         return result
 
     async def count(
         self,
         *,
-        joins: 'Sequence[Join] | None' = None,
-        filters: 'Filter | None' = None,
+        joins: "Sequence[Join] | None" = None,
+        filters: "Filter | None" = None,
     ) -> int:
         result = await self.queries.get_items_count(
             model=self._model_class,
             joins=joins,
             filters=filters,
         )
         return result
 
     async def list(  # noqa: A003
         self,
         *,
         # TODO: улучшить интерфейс, чтобы можно было принимать как 1 элемент, так и несколько
-        joins: 'Sequence[Join] | None' = None,
-        loads: 'Sequence[Load] | None' = None,
-        filters: 'Filter | None' = None,
+        joins: "Sequence[Join] | None" = None,
+        loads: "Sequence[Load] | None" = None,
+        filters: "Filter | None" = None,
         search: str | None = None,
-        search_by: 'Sequence[SearchParam] | None' = None,
-        order_by: 'Sequence[OrderByParam] | None' = None,
+        search_by: "Sequence[SearchParam] | None" = None,
+        order_by: "Sequence[OrderByParam] | None" = None,
         limit: int | None = None,
         offset: int | None = None,
-    ) -> 'Sequence[BaseSQLAlchemyModel]':
+    ) -> "Sequence[BaseSQLAlchemyModel]":
         result = await self.queries.get_item_list(
             model=self._model_class,
             joins=joins,
             loads=loads,
             filters=filters,
             search=search,
             search_by=search_by,
@@ -185,68 +245,211 @@
             unique_items=self.unique_list_items,
         )
         return result
 
     async def create_instance(
         self,
         *,
-        data: 'DataDict | None' = None,
-    ) -> 'BaseSQLAlchemyModel':
+        data: "DataDict | None" = None,
+    ) -> "BaseSQLAlchemyModel":
         result = await self.queries.create_item(
             model=self._model_class,
             data=data,
             use_flush=self.use_flush,
         )
         return result
 
     async def update(
         self,
         *,
-        data: 'DataDict',
-        filters: 'Filter | None' = None,
-    ) -> 'Sequence[BaseSQLAlchemyModel] | None':
+        data: "DataDict",
+        filters: "Filter | None" = None,
+    ) -> "Sequence[BaseSQLAlchemyModel] | None":
         result = await self.queries.db_update(
             model=self._model_class,
             data=data,
             filters=filters,
             use_flush=self.use_flush,
         )
         return result
 
     async def update_instance(
         self,
         *,
-        instance: 'BaseSQLAlchemyModel',
-        data: 'DataDict',
-    ) -> 'tuple[bool, BaseSQLAlchemyModel]':
+        instance: "BaseSQLAlchemyModel",
+        data: "DataDict",
+    ) -> "tuple[bool, BaseSQLAlchemyModel]":
         result = await self.queries.change_item(
             data=data,
             item=instance,
             set_none=self.update_set_none,
             allowed_none_fields=self.update_allowed_none_fields,
             use_flush=self.use_flush,
         )
         return result
 
     async def disable(
         self,
         *,
         ids_to_disable: set[Any],
-        extra_filters: 'Filter | None' = None,
-    ) -> 'Count':
+        extra_filters: "Filter | None" = None,
+    ) -> "Count":
         if self.id_field is None or self.disable_field is None:
             msg = (
                 'Attribute "id_field" or "disable_field" not set in your repository class. '
                 "Can't disable entities."
             )
             raise sqlrepo_exc.RepositoryAttributeError(msg)
         result = await self.queries.disable_items(
             model=self._model_class,
             ids_to_disable=ids_to_disable,
             id_field=self.id_field,
             disable_field=self.disable_field,
             field_type=self.disable_field_type,
-            allow_filter_by_value=self.disable_allow_filter_by_value,
+            allow_filter_by_value=self.allow_disable_filter_by_value,
+            extra_filters=extra_filters,
+            use_flush=self.use_flush,
+        )
+        return result
+
+
+class BaseSyncRepository(BaseRepository[BaseSQLAlchemyModel]):
+    """Base repository class with sync interface.
+
+    Has main CRUD methods for working with model. Use sync session of SQLAlchemy to work with this
+    class.
+    """
+
+    __inheritance_check_model_class__ = False
+    query_class: type["BaseSyncQuery"] = BaseSyncQuery
+
+    def __init__(
+        self,
+        session: "Session",
+    ) -> None:
+        self.session = session
+        self.queries = self.query_class(
+            session,
+            self.get_filter_convert_class(),
+            self.specific_column_mapping,
+            self.load_strategy,
+        )
+
+    def get(
+        self,
+        *,
+        filters: "Filter | None" = None,
+        joins: "Sequence[Join] | None" = None,
+        loads: "Sequence[Load] | None" = None,
+    ) -> "BaseSQLAlchemyModel | None":
+        result = self.queries.get_item(
+            model=self._model_class,
+            joins=joins,
+            loads=loads,
+            filters=filters,
+        )
+        return result
+
+    def count(
+        self,
+        *,
+        joins: "Sequence[Join] | None" = None,
+        filters: "Filter | None" = None,
+    ) -> int:
+        result = self.queries.get_items_count(
+            model=self._model_class,
+            joins=joins,
+            filters=filters,
+        )
+        return result
+
+    async def list(  # noqa: A003
+        self,
+        *,
+        # TODO: улучшить интерфейс, чтобы можно было принимать как 1 элемент, так и несколько
+        joins: "Sequence[Join] | None" = None,
+        loads: "Sequence[Load] | None" = None,
+        filters: "Filter | None" = None,
+        search: str | None = None,
+        search_by: "Sequence[SearchParam] | None" = None,
+        order_by: "Sequence[OrderByParam] | None" = None,
+        limit: int | None = None,
+        offset: int | None = None,
+    ) -> "Sequence[BaseSQLAlchemyModel]":
+        result = self.queries.get_item_list(
+            model=self._model_class,
+            joins=joins,
+            loads=loads,
+            filters=filters,
+            search=search,
+            search_by=search_by,
+            order_by=order_by,
+            limit=limit,
+            offset=offset,
+            unique_items=self.unique_list_items,
+        )
+        return result
+
+    async def create_instance(
+        self,
+        *,
+        data: "DataDict | None" = None,
+    ) -> "BaseSQLAlchemyModel":
+        result = self.queries.create_item(
+            model=self._model_class,
+            data=data,
+            use_flush=self.use_flush,
+        )
+        return result
+
+    async def update(
+        self,
+        *,
+        data: "DataDict",
+        filters: "Filter | None" = None,
+    ) -> "Sequence[BaseSQLAlchemyModel] | None":
+        result = self.queries.db_update(
+            model=self._model_class,
+            data=data,
+            filters=filters,
+            use_flush=self.use_flush,
+        )
+        return result
+
+    def update_instance(
+        self,
+        *,
+        instance: "BaseSQLAlchemyModel",
+        data: "DataDict",
+    ) -> "tuple[bool, BaseSQLAlchemyModel]":
+        result = self.queries.change_item(
+            data=data,
+            item=instance,
+            set_none=self.update_set_none,
+            allowed_none_fields=self.update_allowed_none_fields,
+            use_flush=self.use_flush,
+        )
+        return result
+
+    def disable(
+        self,
+        *,
+        ids_to_disable: set[Any],
+        extra_filters: "Filter | None" = None,
+    ) -> "Count":
+        if self.id_field is None or self.disable_field is None:
+            msg = (
+                'Attribute "id_field" or "disable_field" not set in your repository class. '
+                "Can't disable entities."
+            )
+            raise sqlrepo_exc.RepositoryAttributeError(msg)
+        result = self.queries.disable_items(
+            model=self._model_class,
+            ids_to_disable=ids_to_disable,
+            id_field=self.id_field,
+            disable_field=self.disable_field,
+            field_type=self.disable_field_type,
+            allow_filter_by_value=self.allow_disable_filter_by_value,
             extra_filters=extra_filters,
             use_flush=self.use_flush,
         )
         return result
```

### Comparing `sqlrepo-0.1.1/sqlrepo/uow.py` & `sqlrepo-0.2.0/sqlrepo/uow.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,36 +6,35 @@
 from sqlalchemy.ext.asyncio import AsyncSession, async_sessionmaker
 from sqlalchemy.orm import Session, sessionmaker
 
 from sqlrepo.logging import logger
 
 
 class BaseAsyncUnitOfWork(ABC, Abstract):
-
-    session_factory: 'async_sessionmaker[AsyncSession]' = abstract_class_property(
+    session_factory: "async_sessionmaker[AsyncSession]" = abstract_class_property(
         async_sessionmaker[AsyncSession],
     )
 
     @abstractmethod
-    def init_repositories(self, session: 'AsyncSession') -> None:
+    def init_repositories(self, session: "AsyncSession") -> None:
         raise NotImplementedError()
 
     async def __aenter__(self) -> Self:
         self.session = self.session_factory()
         self.init_repositories(self.session)
         return self
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc: BaseException | None,
         traceback: types.TracebackType | None,
     ) -> None:
         if exc:
-            logger.error('UNIT-OF-WORK E0: %s', exc)
+            logger.error("UNIT-OF-WORK E0: %s", exc)
             await self.rollback()
         else:
             await self.commit()
         await self.close()
 
     async def commit(self) -> None:
         if not self.session:
@@ -50,36 +49,35 @@
     async def close(self) -> None:
         if not self.session:
             return
         await self.session.close()
 
 
 class BaseSyncUnitOfWork(ABC, Abstract):
-
-    session_factory: 'sessionmaker[Session]' = abstract_class_property(
+    session_factory: "sessionmaker[Session]" = abstract_class_property(
         sessionmaker[Session],
     )
 
     @abstractmethod
-    def init_repositories(self, session: 'Session') -> None:
+    def init_repositories(self, session: "Session") -> None:
         raise NotImplementedError()
 
     def __enter__(self) -> Self:
         self.session = self.session_factory()
         self.init_repositories(self.session)
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc: BaseException | None,
         traceback: types.TracebackType | None,
     ) -> None:
         if exc:
-            logger.error('UNIT-OF-WORK E0: %s', exc)
+            logger.error("UNIT-OF-WORK E0: %s", exc)
             self.rollback()
         else:
             self.commit()
         self.close()
 
     def commit(self) -> None:
         if not self.session:
```

### Comparing `sqlrepo-0.1.1/tests/conftest.py` & `sqlrepo-0.2.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,123 +24,123 @@
     from sqlalchemy import Engine
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Session
 
     from tests.types import AsyncFactoryFunctionProtocol, SyncFactoryFunctionProtocol
 
 
-true_stmt = {'y', 'Y', 'yes', 'Yes', 't', 'true', 'True', '1'}
-IS_DOCKER_TEST = os.environ.get('IS_DOCKER_TEST', 'false') in true_stmt
+true_stmt = {"y", "Y", "yes", "Yes", "t", "true", "True", "1"}
+IS_DOCKER_TEST = os.environ.get("IS_DOCKER_TEST", "false") in true_stmt
 
 
 @pytest.fixture(scope="session")
-def event_loop() -> 'Generator[asyncio.AbstractEventLoop, None, None]':
+def event_loop() -> "Generator[asyncio.AbstractEventLoop, None, None]":
     """Event loop fixture."""
     loop = asyncio.get_event_loop_policy().new_event_loop()
     yield loop
     loop.close()
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_name() -> str:
     """Db name as fixture."""
-    return 'test_db'
+    return "test_db"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_user() -> str:
     """DB user as fixture."""
-    return 'postgres'
+    return "postgres"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_password() -> str:
     """DB password as fixture."""
-    return 'postgres'
+    return "postgres"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_host() -> str:
     """DB host as fixture."""
     if IS_DOCKER_TEST:
-        return 'db'
-    return 'localhost'
+        return "db"
+    return "localhost"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_port() -> int:
     """DB port as fixture."""
     return 5432
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_domain(db_name: str, db_user: str, db_password: str, db_host: str, db_port: int) -> str:
     """Domain for test db without specified driver."""
-    return f'{db_user}:{db_password}@{db_host}:{db_port}/{db_name}'
+    return f"{db_user}:{db_password}@{db_host}:{db_port}/{db_name}"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_sync_url(db_domain: str) -> str:
     """URL for test db (will be created in db_engine): sync driver."""
-    return f'postgresql://{db_domain}'
+    return f"postgresql://{db_domain}"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_async_url(db_domain: str) -> str:
     """URL for test db (will be created in db_engine): async driver."""
-    return f'postgresql+asyncpg://{db_domain}'
+    return f"postgresql+asyncpg://{db_domain}"
 
 
-@pytest.fixture(scope='module')
-def db_sync_engine(db_sync_url: str) -> 'Generator[Engine, None, None]':
+@pytest.fixture(scope="module")
+def db_sync_engine(db_sync_url: str) -> "Generator[Engine, None, None]":
     """SQLAlchemy engine session-based fixture."""
     with suppress(SQLAlchemyError):
         create_db(db_sync_url)
     engine = create_engine(db_sync_url, echo=False, pool_pre_ping=True)
     try:
         yield engine
     finally:
         engine.dispose()
     with suppress(SQLAlchemyError):
         destroy_db(db_sync_url)
 
 
-@pytest.fixture(scope='module')
-def db_sync_session_factory(db_sync_engine: 'Engine') -> 'scoped_session[Session]':
+@pytest.fixture(scope="module")
+def db_sync_session_factory(db_sync_engine: "Engine") -> "scoped_session[Session]":
     """SQLAlchemy session factory session-based fixture."""
     return scoped_session(
         sessionmaker(
             bind=db_sync_engine,
             autoflush=False,
             expire_on_commit=False,
         ),
     )
 
 
 @pytest.fixture()
 def db_sync_session(
-    db_sync_engine: 'Engine',
-    db_sync_session_factory: 'scoped_session[Session]',
-) -> 'Generator[Session, None, None]':
+    db_sync_engine: "Engine",
+    db_sync_session_factory: "scoped_session[Session]",
+) -> "Generator[Session, None, None]":
     """SQLAlchemy session fixture."""
     Base.metadata.create_all(db_sync_engine)
     with db_sync_session_factory() as session:
         yield session
     Base.metadata.drop_all(db_sync_engine)
 
 
 @pytest.fixture()
 def mymodel_sync_factory(
     dt_faker: Datetime,
     text_faker: Text,
-) -> 'SyncFactoryFunctionProtocol[MyModel]':
+) -> "SyncFactoryFunctionProtocol[MyModel]":
     """Function-factory, that create MyModel instances."""
 
     def _create(
-        session: 'Session',
+        session: "Session",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
     ) -> MyModel:
         params: dict[str, Any] = dict(
             name=text_faker.sentence(),
             other_name=text_faker.sentence(),
@@ -152,28 +152,28 @@
 
     return _create
 
 
 @pytest.fixture()
 def othermodel_sync_factory(
     text_faker: Text,
-    mymodel_sync_factory: 'SyncFactoryFunctionProtocol[MyModel]',
-) -> 'SyncFactoryFunctionProtocol[OtherModel]':
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
+) -> "SyncFactoryFunctionProtocol[OtherModel]":
     """Function-factory, that create OtherModel instances."""
 
     def _create(
-        session: 'Session',
+        session: "Session",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
     ) -> OtherModel:
-        if 'model_id' not in kwargs:
+        if "model_id" not in kwargs:
             model_id = mymodel_sync_factory(session, commit=commit).id
         else:
-            model_id = kwargs.pop('model_id')
+            model_id = kwargs.pop("model_id")
         params: dict[str, Any] = dict(
             name=text_faker.sentence(),
             other_name=text_faker.sentence(),
             model_id=model_id,
         )
         params.update(kwargs)
         return create_db_item_sync(session, OtherModel, params, commit=commit)
@@ -181,19 +181,19 @@
     return _create
 
 
 @pytest.fixture()
 def mymodel_async_factory(
     text_faker: Text,
     dt_faker: Datetime,
-) -> 'AsyncFactoryFunctionProtocol[MyModel]':
+) -> "AsyncFactoryFunctionProtocol[MyModel]":
     """Function-factory, that create MyModel instances."""
 
     async def _create(
-        session: 'AsyncSession',
+        session: "AsyncSession",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
     ) -> MyModel:
         params: dict[str, Any] = dict(
             name=text_faker.sentence(),
             other_name=text_faker.sentence(),
@@ -205,29 +205,29 @@
 
     return _create
 
 
 @pytest.fixture()
 def othermodel_async_factory(
     text_faker: Text,
-    mymodel_async_factory: 'AsyncFactoryFunctionProtocol[MyModel]',
-) -> 'AsyncFactoryFunctionProtocol[OtherModel]':
+    mymodel_async_factory: "AsyncFactoryFunctionProtocol[MyModel]",
+) -> "AsyncFactoryFunctionProtocol[OtherModel]":
     """Function-factory, that create OtherModel instances."""
 
     async def _create(
-        session: 'AsyncSession',
+        session: "AsyncSession",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
     ) -> OtherModel:
-        if 'model_id' not in kwargs:
+        if "model_id" not in kwargs:
             model = await mymodel_async_factory(session, commit=commit)
             model_id = model.id
         else:
-            model_id = kwargs.pop('model_id')
+            model_id = kwargs.pop("model_id")
         params: dict[str, Any] = dict(
             name=text_faker.sentence(),
             other_name=text_faker.sentence(),
             model_id=model_id,
         )
         params.update(kwargs)
         return await create_db_item_async(session, OtherModel, params, commit=commit)
```

### Comparing `sqlrepo-0.1.1/tests/test_base_queries.py` & `sqlrepo-0.2.0/tests/test_base_queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,73 +8,73 @@
 from freezegun import freeze_time
 from sqlalchemy import ColumnElement, and_, delete, func, or_, select, text, update
 from sqlalchemy.orm import joinedload, selectinload
 
 from sqlrepo.queries import BaseQuery
 from tests.utils import MyModel, OtherModel
 
-now = datetime.datetime.now(tz=ZoneInfo('UTC'))
+now = datetime.datetime.now(tz=ZoneInfo("UTC"))
 
 
 @pytest.mark.parametrize(
-    ('specific_column_mapping', 'elements', 'expected_result'),
+    ("specific_column_mapping", "elements", "expected_result"),
     [
         (
             None,
-            ['other_model_id', MyModel.name],
-            ['other_model_id', MyModel.name],
+            ["other_model_id", MyModel.name],
+            ["other_model_id", MyModel.name],
         ),
         (
-            {'other_model_id': OtherModel.id, 'some_other_model_field': OtherModel.name},
-            ['other_model_id', MyModel.name],
+            {"other_model_id": OtherModel.id, "some_other_model_field": OtherModel.name},
+            ["other_model_id", MyModel.name],
             [OtherModel.id, MyModel.name],
         ),
         (
-            {'other_model_id': OtherModel.id, 'some_other_model_field': OtherModel.name},
-            ['not_presented_field', 'other_model_id'],
-            ['not_presented_field', OtherModel.id],
+            {"other_model_id": OtherModel.id, "some_other_model_field": OtherModel.name},
+            ["not_presented_field", "other_model_id"],
+            ["not_presented_field", OtherModel.id],
         ),
     ],
 )
 def test_resolve_specific_columns(  # noqa
     specific_column_mapping: dict[str, ColumnElement[Any]],
     elements: list[str | ColumnElement[Any]],
     expected_result: list[str | ColumnElement[Any]],  # noqa
 ) -> None:
     query = BaseQuery(SimpleFilterConverter, specific_column_mapping)
     converted_columns = query._resolve_specific_columns(elements=elements)  # type: ignore
     assert converted_columns == expected_result
 
 
 @pytest.mark.parametrize(
-    ('stmt', 'joins', 'expected_result'),
+    ("stmt", "joins", "expected_result"),
     [
         (
             select(MyModel),
             [OtherModel],
             select(MyModel).join(OtherModel),
         ),
         (
             select(MyModel),
-            ['other_models'],
+            ["other_models"],
             select(MyModel).join(OtherModel),
         ),
         (
             select(MyModel),
             [(OtherModel, MyModel.id == OtherModel.my_model_id)],
             select(MyModel).join(OtherModel),
         ),
         (
             select(MyModel),
-            [(OtherModel, MyModel.id == OtherModel.my_model_id, {'isouter': True})],
+            [(OtherModel, MyModel.id == OtherModel.my_model_id, {"isouter": True})],
             select(MyModel).join(OtherModel, isouter=True),
         ),
         (
             select(MyModel),
-            [(OtherModel, MyModel.id == OtherModel.my_model_id, {'full': True})],
+            [(OtherModel, MyModel.id == OtherModel.my_model_id, {"full": True})],
             select(MyModel).join(OtherModel, full=True),
         ),
     ],
 )
 def test_resolve_and_apply_joins(  # noqa
     stmt: Any,  # noqa
     joins: Any,  # noqa
@@ -82,26 +82,26 @@
 ) -> None:
     query = BaseQuery(SimpleFilterConverter)
     new_stmt = query._resolve_and_apply_joins(stmt=stmt, joins=joins)  # type: ignore
     assert str(new_stmt) == str(expected_result)
 
 
 @pytest.mark.parametrize(
-    ('stmt', 'strategy', 'loads', 'expected_result'),
+    ("stmt", "strategy", "loads", "expected_result"),
     [
         (
             select(MyModel),
             joinedload,
-            ['other_models'],
+            ["other_models"],
             select(MyModel).options(joinedload(MyModel.other_models)),
         ),
         (
             select(MyModel),
             selectinload,
-            ['other_models'],
+            ["other_models"],
             select(MyModel).options(selectinload(MyModel.other_models)),
         ),
     ],
 )
 def test_resolve_and_apply_loads(  # noqa
     stmt: Any,  # noqa
     strategy: Any,  # noqa
@@ -112,26 +112,26 @@
     new_stmt = query._resolve_and_apply_loads(stmt=stmt, loads=loads)  # type: ignore
     assert str(new_stmt) == str(expected_result)
 
 
 def test_resolve_and_apply_loads_incorrect():  # noqa
     query = BaseQuery(SimpleFilterConverter)
     with pytest.raises(NoModelRelationshipError):
-        query._resolve_and_apply_loads(stmt=select(MyModel), loads=['incorrect'])  # type: ignore
+        query._resolve_and_apply_loads(stmt=select(MyModel), loads=["incorrect"])  # type: ignore
 
 
 @pytest.mark.parametrize(
     (
-        'id_field',
-        'ids_to_disable',
-        'disable_field',
-        'field_type',
-        'allow_filter_by_value',
-        'extra_filters',
-        'expected_result',
+        "id_field",
+        "ids_to_disable",
+        "disable_field",
+        "field_type",
+        "allow_filter_by_value",
+        "extra_filters",
+        "expected_result",
     ),
     [
         (
             MyModel.id,
             {1, 2, 3, 4, 5},
             MyModel.dt,
             datetime.datetime,
@@ -141,16 +141,16 @@
         ),
         (
             MyModel.id,
             {1, 2, 3, 4, 5},
             MyModel.dt,
             datetime.datetime,
             False,
-            {'name': 'aboba'},
-            [MyModel.id.in_({1, 2, 3, 4, 5}), MyModel.name == 'aboba'],
+            {"name": "aboba"},
+            [MyModel.id.in_({1, 2, 3, 4, 5}), MyModel.name == "aboba"],
         ),
         (
             MyModel.id,
             {1, 2, 3, 4, 5},
             MyModel.dt,
             datetime.datetime,
             True,
@@ -187,33 +187,33 @@
         allow_filter_by_value=allow_filter_by_value,
         extra_filters=extra_filters,
     )
     assert list(map(str, disable_filters)) == list(map(str, expected_result))
 
 
 @pytest.mark.parametrize(
-    ('search', 'search_by_args', 'use_and_clause', 'expected_result'),
+    ("search", "search_by_args", "use_and_clause", "expected_result"),
     [
         (
-            'value',
+            "value",
             (MyModel.name, MyModel.other_name),
             False,
-            or_(MyModel.name.ilike(r'%value%'), MyModel.other_name.ilike(r'%value%')),
+            or_(MyModel.name.ilike(r"%value%"), MyModel.other_name.ilike(r"%value%")),
         ),
         (
-            'value',
+            "value",
             (MyModel.name, MyModel.other_name),
             True,
-            and_(MyModel.name.ilike(r'%value%'), MyModel.other_name.ilike(r'%value%')),
+            and_(MyModel.name.ilike(r"%value%"), MyModel.other_name.ilike(r"%value%")),
         ),
         (
-            'value',
-            ('name', 'other_name'),
+            "value",
+            ("name", "other_name"),
             False,
-            or_(MyModel.name.ilike(r'%value%'), MyModel.other_name.ilike(r'%value%')),
+            or_(MyModel.name.ilike(r"%value%"), MyModel.other_name.ilike(r"%value%")),
         ),
     ],
 )
 def test_make_search_filter(  # noqa
     search: str,
     search_by_args: tuple[Any, ...],
     use_and_clause: bool,  # noqa
@@ -226,38 +226,38 @@
         *search_by_args,
         use_and_clause=use_and_clause,
     )
     assert str(search_filter) == str(expected_result)
 
 
 @pytest.mark.parametrize(
-    ('filters', 'joins', 'loads', 'expected_result'),
+    ("filters", "joins", "loads", "expected_result"),
     [
         (
             None,
             None,
             None,
             select(MyModel),
         ),
         (
-            {'name': 'aboba'},
+            {"name": "aboba"},
             None,
             None,
-            select(MyModel).where(MyModel.name == 'aboba'),
+            select(MyModel).where(MyModel.name == "aboba"),
         ),
         (
             None,
-            ['other_models'],
+            ["other_models"],
             None,
             select(MyModel).join(OtherModel),
         ),
         (
             None,
             None,
-            ['other_models'],
+            ["other_models"],
             select(MyModel).options(joinedload(MyModel.other_models)),
         ),
     ],
 )
 def test_get_item_stmt(  # noqa
     filters: Any,  # noqa
     joins: Any,  # noqa
@@ -271,38 +271,38 @@
         joins=joins,
         loads=loads,
     )
     assert str(get_item_stmt) == str(expected_result)
 
 
 @pytest.mark.parametrize(
-    ('filters', 'joins', 'expected_result'),
+    ("filters", "joins", "expected_result"),
     [
         (
             None,
             None,
             select(func.count()).select_from(MyModel),
         ),
         (
-            {'name': 'aboba'},
+            {"name": "aboba"},
             None,
-            select(func.count()).select_from(MyModel).where(MyModel.name == 'aboba'),
+            select(func.count()).select_from(MyModel).where(MyModel.name == "aboba"),
         ),
         (
             None,
-            ['other_models'],
+            ["other_models"],
             select(func.count()).select_from(MyModel).join(OtherModel),
         ),
         (
-            [OtherModel.name == 'aboba'],
-            ['other_models'],
+            [OtherModel.name == "aboba"],
+            ["other_models"],
             select(func.count())
             .select_from(MyModel)
             .join(OtherModel)
-            .where(OtherModel.name == 'aboba'),
+            .where(OtherModel.name == "aboba"),
         ),
     ],
 )
 def test_get_items_count_stmt(  # noqa
     filters: Any,  # noqa
     joins: Any,  # noqa
     expected_result: Any,  # noqa
@@ -314,23 +314,23 @@
         filters=filters,
     )
     assert str(get_items_count_stmt) == str(expected_result)
 
 
 @pytest.mark.parametrize(
     (
-        'joins',
-        'loads',
-        'filters',
-        'search',
-        'search_by',
-        'order_by',
-        'limit',
-        'offset',
-        'expected_result',
+        "joins",
+        "loads",
+        "filters",
+        "search",
+        "search_by",
+        "order_by",
+        "limit",
+        "offset",
+        "expected_result",
     ),
     [
         (
             None,
             None,
             None,
             None,
@@ -340,15 +340,15 @@
             None,
             select(MyModel),
         ),
         (
             None,
             None,
             None,
-            'some_value',
+            "some_value",
             None,
             None,
             None,
             None,
             select(MyModel),
         ),
         (
@@ -362,31 +362,31 @@
             None,
             select(MyModel),
         ),
         (
             None,
             None,
             None,
-            'somevalue',
+            "somevalue",
             (MyModel.name,),
             None,
             None,
             None,
-            select(MyModel).where(MyModel.name.ilike(r'%somevalue%')),
+            select(MyModel).where(MyModel.name.ilike(r"%somevalue%")),
         ),
         (
             None,
             None,
             None,
             None,
             None,
-            ('some_value',),
+            ("some_value",),
             None,
             None,
-            select(MyModel).order_by(text('some_value')),
+            select(MyModel).order_by(text("some_value")),
         ),
         (
             None,
             None,
             None,
             None,
             None,
@@ -432,28 +432,28 @@
         offset=offset,
     )
     assert str(get_item_list_stmt) == str(expected_result)
 
 
 @pytest.mark.parametrize(
     (
-        'data',
-        'filters',
-        'expected_result',
+        "data",
+        "filters",
+        "expected_result",
     ),
     [
         (
-            {'name': 25},
+            {"name": 25},
             None,
-            update(MyModel).values({'name': 25}).returning(MyModel),
+            update(MyModel).values({"name": 25}).returning(MyModel),
         ),
         (
-            {'name': 'aboba'},
-            {'name': 'aboba'},
-            update(MyModel).where(MyModel.name == 'aboba').values({'name': 25}).returning(MyModel),
+            {"name": "aboba"},
+            {"name": "aboba"},
+            update(MyModel).where(MyModel.name == "aboba").values({"name": 25}).returning(MyModel),
         ),
     ],
 )
 def test_db_update_stmt(  # noqa
     data: Any,  # noqa
     filters: Any,  # noqa
     expected_result: Any,  # noqa
@@ -464,39 +464,39 @@
         data=data,
         filters=filters,
     )
     assert str(db_update_stmt) == str(expected_result)
 
 
 @pytest.mark.parametrize(
-    ('filters', 'expected_result'),
+    ("filters", "expected_result"),
     [
         (None, delete(MyModel)),
-        ({'name': 'aboba'}, delete(MyModel).where(MyModel.name == 'aboba')),
+        ({"name": "aboba"}, delete(MyModel).where(MyModel.name == "aboba")),
     ],
 )
 def test_db_delete_stmt(filters: Any, expected_result: Any):  # noqa
     query = BaseQuery(SimpleFilterConverter)
     db_delete_stmt = query._db_delete_stmt(  # type: ignore
         model=MyModel,
         filters=filters,
     )
     assert str(db_delete_stmt) == str(expected_result)
 
 
 @freeze_time(now)
 @pytest.mark.parametrize(
     (
-        'ids_to_disable',
-        'id_field',
-        'disable_field',
-        'field_type',
-        'allow_filter_by_value',
-        'extra_filters',
-        'expected_result',
+        "ids_to_disable",
+        "id_field",
+        "disable_field",
+        "field_type",
+        "allow_filter_by_value",
+        "extra_filters",
+        "expected_result",
     ),
     [
         (
             {1, 2, 3},
             MyModel.id,
             MyModel.dt,
             datetime.datetime,
```

### Comparing `sqlrepo-0.1.1/tests/test_sync_queries.py` & `sqlrepo-0.2.0/tests/test_sync_queries.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,110 +23,110 @@
 
 
 text_faker = Text(locale=Locale.EN)
 dt_faker = Datetime(locale=Locale.EN)
 
 
 def test_get_item(  # noqa: D103
-    db_sync_session: 'Session',
-    mymodel_sync_factory: 'SyncFactoryFunctionProtocol[MyModel]',
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
 ) -> None:
     item = mymodel_sync_factory(db_sync_session, commit=True)
     query_obj = BaseSyncQuery(db_sync_session, SimpleFilterConverter)
     db_item = query_obj.get_item(model=MyModel, filters=dict(id=item.id))
-    assert db_item is not None, f'MyModel with id {item.id} not found in db.'
+    assert db_item is not None, f"MyModel with id {item.id} not found in db."
     assert_compare_db_items(item, db_item)
 
 
 def test_get_item_not_found(  # noqa: D103
-    db_sync_session: 'Session',
-    mymodel_sync_factory: 'SyncFactoryFunctionProtocol[MyModel]',
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
 ) -> None:
     item = mymodel_sync_factory(db_sync_session, commit=True)
     query_obj = BaseSyncQuery(db_sync_session, SimpleFilterConverter)
     db_item = query_obj.get_item(model=MyModel, filters=dict(id=item.id + 1))
-    assert db_item is None, f'MyModel with id {item.id + 1} was found in db (but it shouldn\'t).'
+    assert db_item is None, f"MyModel with id {item.id + 1} was found in db (but it shouldn't)."
 
 
 def test_get_items_count(  # noqa: D103
-    db_sync_session: 'Session',
-    mymodel_sync_factory: 'SyncFactoryFunctionProtocol[MyModel]',
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
 ) -> None:
     for _ in range(3):
         mymodel_sync_factory(db_sync_session, commit=False)
     db_sync_session.commit()
     query_obj = BaseSyncQuery(db_sync_session, SimpleFilterConverter)
     count = query_obj.get_items_count(model=MyModel)
     assert count == 3
 
 
 def test_get_items_count_with_filter(  # noqa: D103
-    db_sync_session: 'Session',
-    mymodel_sync_factory: 'SyncFactoryFunctionProtocol[MyModel]',
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
 ) -> None:
     item = mymodel_sync_factory(db_sync_session, commit=False)
     for _ in range(2):
         mymodel_sync_factory(db_sync_session, commit=False)
     db_sync_session.commit()
     query_obj = BaseSyncQuery(db_sync_session, SimpleFilterConverter)
     count = query_obj.get_items_count(model=MyModel, filters=dict(id=item.id))
     assert count == 1
 
 
 def test_get_items_list(  # noqa: D103
-    db_sync_session: 'Session',
-    mymodel_sync_factory: 'SyncFactoryFunctionProtocol[MyModel]',
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
 ) -> None:
     items = [mymodel_sync_factory(db_sync_session, commit=False) for _ in range(3)]
     db_sync_session.commit()
     query_obj = BaseSyncQuery(db_sync_session, SimpleFilterConverter)
     db_items = list(query_obj.get_item_list(model=MyModel))
     assert_compare_db_item_list(items, db_items)
 
 
 # TODO: fix test. Now it just clone of test_get_items_list (previous test). Needs to check unique
 def test_get_items_list_with_unique(  # noqa: D103
-    db_sync_session: 'Session',
-    mymodel_sync_factory: 'SyncFactoryFunctionProtocol[MyModel]',
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
 ) -> None:
     items = [mymodel_sync_factory(db_sync_session, commit=False) for _ in range(3)]
     db_sync_session.commit()
     query_obj = BaseSyncQuery(db_sync_session, SimpleFilterConverter)
     db_items = list(query_obj.get_item_list(model=MyModel, unique_items=True))
     assert_compare_db_item_list(items, db_items)
 
 
 @pytest.mark.parametrize(
-    ('create_data', 'use_flush'),
+    ("create_data", "use_flush"),
     [
         (
             {
-                'name': text_faker.sentence(),
-                'other_name': text_faker.sentence(),
-                'dt': dt_faker.datetime(),
-                'bl': coin_flip(),
+                "name": text_faker.sentence(),
+                "other_name": text_faker.sentence(),
+                "dt": dt_faker.datetime(),
+                "bl": coin_flip(),
             },
             True,
         ),
         (
             {
-                'name': text_faker.sentence(),
-                'other_name': text_faker.sentence(),
-                'dt': dt_faker.datetime(),
-                'bl': coin_flip(),
+                "name": text_faker.sentence(),
+                "other_name": text_faker.sentence(),
+                "dt": dt_faker.datetime(),
+                "bl": coin_flip(),
             },
             False,
         ),
         (
             {
-                'name': text_faker.sentence(),
-                'other_name': text_faker.sentence(),
-                'dt': dt_faker.datetime(),
-                'bl': coin_flip(),
-                'other_models': [
+                "name": text_faker.sentence(),
+                "other_name": text_faker.sentence(),
+                "dt": dt_faker.datetime(),
+                "bl": coin_flip(),
+                "other_models": [
                     OtherModel(
                         name=text_faker.sentence(),
                         other_name=text_faker.sentence(),
                     ),
                     OtherModel(
                         name=text_faker.sentence(),
                         other_name=text_faker.sentence(),
@@ -134,153 +134,153 @@
                 ],
             },
             False,
         ),
     ],
 )
 def test_create_item(
-    db_sync_session: 'Session',
+    db_sync_session: "Session",
     create_data: dict[str, Any],
     use_flush: bool,  # noqa: FBT001
 ) -> None:
     query_obj = BaseSyncQuery(db_sync_session, SimpleFilterConverter)
     db_item = query_obj.create_item(model=MyModel, data=create_data, use_flush=use_flush)
     assert_compare_db_item_with_dict(db_item, create_data, skip_keys_check=True)
 
 
 @pytest.mark.parametrize(
-    ('update_data', 'use_flush', 'items_count'),
+    ("update_data", "use_flush", "items_count"),
     [
         (
             {
-                'name': text_faker.sentence(),
-                'other_name': text_faker.sentence(),
-                'dt': dt_faker.datetime(),
-                'bl': coin_flip(),
+                "name": text_faker.sentence(),
+                "other_name": text_faker.sentence(),
+                "dt": dt_faker.datetime(),
+                "bl": coin_flip(),
             },
             True,
             1,
         ),
         (
             {
-                'name': text_faker.sentence(),
-                'other_name': text_faker.sentence(),
-                'dt': dt_faker.datetime(),
-                'bl': coin_flip(),
+                "name": text_faker.sentence(),
+                "other_name": text_faker.sentence(),
+                "dt": dt_faker.datetime(),
+                "bl": coin_flip(),
             },
             False,
             1,
         ),
         (
             {
-                'name': text_faker.sentence(),
-                'other_name': text_faker.sentence(),
-                'dt': dt_faker.datetime(),
-                'bl': coin_flip(),
+                "name": text_faker.sentence(),
+                "other_name": text_faker.sentence(),
+                "dt": dt_faker.datetime(),
+                "bl": coin_flip(),
             },
             False,
             3,
         ),
     ],
 )
 def test_db_update(
-    db_sync_session: 'Session',
-    mymodel_sync_factory: 'SyncFactoryFunctionProtocol[MyModel]',
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
     update_data: dict[str, Any],
     use_flush: bool,  # noqa: FBT001
     items_count: int,
 ) -> None:
     for _ in range(items_count):
         mymodel_sync_factory(db_sync_session, commit=True)
     query_obj = BaseSyncQuery(db_sync_session, SimpleFilterConverter)
     db_item = query_obj.db_update(model=MyModel, data=update_data, use_flush=use_flush)
     assert len(db_item) == items_count
     assert_compare_db_item_list_with_dict(db_item, update_data, skip_keys_check=True)
 
 
 @pytest.mark.parametrize(
-    ('update_data', 'use_flush', 'expected_updated_flag'),
+    ("update_data", "use_flush", "expected_updated_flag"),
     [
         (
             {
-                'name': text_faker.sentence(),
-                'other_name': text_faker.sentence(),
-                'dt': dt_faker.datetime(),
-                'bl': coin_flip(),
+                "name": text_faker.sentence(),
+                "other_name": text_faker.sentence(),
+                "dt": dt_faker.datetime(),
+                "bl": coin_flip(),
             },
             True,
             True,
         ),
         (
             {
-                'name': text_faker.sentence(),
-                'other_name': text_faker.sentence(),
-                'dt': dt_faker.datetime(),
-                'bl': coin_flip(),
+                "name": text_faker.sentence(),
+                "other_name": text_faker.sentence(),
+                "dt": dt_faker.datetime(),
+                "bl": coin_flip(),
             },
             False,
             True,
         ),
         (
             {},
             False,
             False,
         ),
     ],
 )
 def test_change_item(
-    db_sync_session: 'Session',
-    mymodel_sync_factory: 'SyncFactoryFunctionProtocol[MyModel]',
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
     update_data: dict[str, Any],
     use_flush: bool,  # noqa: FBT001
     expected_updated_flag: bool,  # noqa: FBT001
 ) -> None:
     item = mymodel_sync_factory(db_sync_session)
     query_obj = BaseSyncQuery(db_sync_session, SimpleFilterConverter)
     updated, db_item = query_obj.change_item(data=update_data, item=item, use_flush=use_flush)
     assert expected_updated_flag is updated
     assert_compare_db_item_with_dict(db_item, update_data, skip_keys_check=True)
 
 
 @pytest.mark.parametrize(
-    ('update_data', 'expected_updated_flag', 'set_none', 'allowed_none_fields', 'none_set_fields'),
+    ("update_data", "expected_updated_flag", "set_none", "allowed_none_fields", "none_set_fields"),
     [
         (
             {},
             False,
             False,
             {},
             {},
         ),
         (
-            {'name': text_faker.sentence()},
+            {"name": text_faker.sentence()},
             True,
             True,
-            '*',
+            "*",
             {},
         ),
         (
-            {'name': text_faker.sentence(), 'other_name': None, 'dt': None, 'bl': None},
+            {"name": text_faker.sentence(), "other_name": None, "dt": None, "bl": None},
             True,
             True,
-            '*',
-            {'other_name', 'dt', 'bl'},
+            "*",
+            {"other_name", "dt", "bl"},
         ),
         (
-            {'name': text_faker.sentence(), 'other_name': None, 'dt': None, 'bl': None},
+            {"name": text_faker.sentence(), "other_name": None, "dt": None, "bl": None},
             True,
             True,
-            {'other_name'},
-            {'other_name'},
+            {"other_name"},
+            {"other_name"},
         ),
     ],
 )
 def test_change_item_none_check(
-    db_sync_session: 'Session',
-    mymodel_sync_factory: 'SyncFactoryFunctionProtocol[MyModel]',
+    db_sync_session: "Session",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
     update_data: dict[str, Any],
     expected_updated_flag: bool,  # noqa: FBT001
     set_none: bool,  # noqa: FBT001
     allowed_none_fields: Any,  # noqa: FBT001, ANN401
     none_set_fields: set[str],
 ) -> None:
     item = mymodel_sync_factory(db_sync_session)
```

### Comparing `sqlrepo-0.1.1/tests/types.py` & `sqlrepo-0.2.0/tests/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from typing import TYPE_CHECKING, Any, Protocol, TypeVar
 
 if TYPE_CHECKING:
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Session
 
 
-T = TypeVar('T', covariant=True)
+T = TypeVar("T", covariant=True)
 
 
 class SyncFactoryFunctionProtocol(Protocol[T]):
     """Protocol for Sync functions-factories that create db items."""
 
     @staticmethod
     def __call__(  # noqa: D102
-        session: 'Session',
+        session: "Session",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
-    ) -> T:
-        ...
+    ) -> T: ...
 
 
 class AsyncFactoryFunctionProtocol(Protocol[T]):
     """Protocol for Sync functions-factories that create db items."""
 
     @staticmethod
     async def __call__(  # noqa: D102
-        session: 'AsyncSession',
+        session: "AsyncSession",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
-    ) -> T:
-        ...
+    ) -> T: ...
```

### Comparing `sqlrepo-0.1.1/tests/utils.py` & `sqlrepo-0.2.0/tests/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from sqlalchemy_utils import create_database, database_exists, drop_database  # type: ignore
 
 if TYPE_CHECKING:
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Session
 
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 def coin_flip() -> bool:
     """Coin flip: True or False."""
     return bool(random.getrandbits(1))
 
 
@@ -39,118 +39,118 @@
     res = [now]
     for i in range(1, n):
         delta = datetime.timedelta(days=i)
         res.append(now + delta)
     return res
 
 
-def assert_compare_db_items(item1: 'DeclarativeBase', item2: 'DeclarativeBase') -> None:
+def assert_compare_db_items(item1: "DeclarativeBase", item2: "DeclarativeBase") -> None:
     """Assert if 2 models not compare to each other."""
     if item1 is item2:
         return
     assert (
         item1.__class__ == item2.__class__
-    ), 'item1 and item2 has different classes. Cant compare.'
+    ), "item1 and item2 has different classes. Cant compare."
     item1_fields = set(inspect(item1.__class__).columns.keys())
     item2_fields = set(inspect(item2.__class__).columns.keys())
-    assert item1_fields == item2_fields, ''
+    assert item1_fields == item2_fields, ""
     for field in item1_fields:
         assert getattr(
             item1,
             field,
-            float('nan'),
+            float("nan"),
         ) == getattr(
             item2,
             field,
-            float('nan'),
-        ), f'field {field} is not compared. Different values.'
+            float("nan"),
+        ), f"field {field} is not compared. Different values."
 
 
 def assert_compare_db_item_list(
-    items1: Sequence['DeclarativeBase'],
-    items2: Sequence['DeclarativeBase'],
+    items1: Sequence["DeclarativeBase"],
+    items2: Sequence["DeclarativeBase"],
 ) -> None:
     """Assert if 2 model lists not compare to each other."""
-    assert len(items1) == len(items2), f'Different lists count: {len(items1)} != {len(items2)}'
+    assert len(items1) == len(items2), f"Different lists count: {len(items1)} != {len(items2)}"
     for item1, item2 in zip(
         sorted(items1, key=lambda x: x.id),  # type: ignore
         sorted(items2, key=lambda x: x.id),  # type: ignore
     ):
         assert_compare_db_items(item1, item2)
 
 
 def assert_compare_db_item_with_dict(
-    item: 'DeclarativeBase',
+    item: "DeclarativeBase",
     data: dict[str, Any],
     *,
     skip_keys_check: bool = False,
 ) -> None:
     """Assert if model not compare to dict."""
     data_fields = set(data.keys())
     item_fields = set(inspect(item.__class__).columns.keys())
-    msg = f'data fields ({data_fields}) are not compare to item fields ({item_fields}).'
+    msg = f"data fields ({data_fields}) are not compare to item fields ({item_fields})."
     if not skip_keys_check:
         assert set(data_fields).issubset(item_fields), msg
     for field, value in data.items():
-        item_field_value = getattr(item, field, float('nan'))
+        item_field_value = getattr(item, field, float("nan"))
         msg = (
             f'data ({field=} {value=}) not compare '
             f'to item ({field=} value={getattr(item, field, "<not present in item>")})'
         )
         assert item_field_value == value, msg
 
 
 def assert_compare_db_item_list_with_dict(
-    items: Sequence['DeclarativeBase'],
+    items: Sequence["DeclarativeBase"],
     data: dict[str, Any],
     *,
     skip_keys_check: bool = False,
 ) -> None:
     """Assert if list of models not compare to dict."""
     data_fields = set(data.keys())
     for item in items:
         item_class = item.__class__
         item_fields = set(inspect(item_class).columns.keys())
         msg = (
-            f'data fields ({data_fields}) are not compare to item '
-            f'({item_class}) fields ({item_fields}).'
+            f"data fields ({data_fields}) are not compare to item "
+            f"({item_class}) fields ({item_fields})."
         )
         if not skip_keys_check:
             assert set(data_fields).issubset(item_fields), msg
         for field, value in data.items():
-            item_field_value = getattr(item, field, float('nan'))
+            item_field_value = getattr(item, field, float("nan"))
             msg = (
                 f'data ({field=} {value=}) not compare '
                 f'to item ({field=} value={getattr(item, field, "<not present in item>")})'
             )
             assert item_field_value == value, msg
 
 
-def assert_compare_db_item_none_fields(item: 'DeclarativeBase', none_fields: set[str]) -> None:
+def assert_compare_db_item_none_fields(item: "DeclarativeBase", none_fields: set[str]) -> None:
     """Assert compare model instance fields for none value."""
     for field in none_fields:
-        item_value = getattr(item, field, float('nan'))
+        item_value = getattr(item, field, float("nan"))
         msg = f'Field "{field}" is not None.'
         assert item_value is None, msg
 
 
 def assert_compare_db_item_list_none_fields(
-    items: Sequence['DeclarativeBase'],
+    items: Sequence["DeclarativeBase"],
     none_fields: set[str],
 ) -> None:
     """Assert compare list of model instances fields for none value."""
     for item in items:
         for field in none_fields:
-            item_value = getattr(item, field, float('nan'))
+            item_value = getattr(item, field, float("nan"))
             msg = f'Field "{field}" of item {item} is not None.'
             assert item_value is None, msg
 
 
 def create_db_item_sync(
-    session: 'Session',
+    session: "Session",
     model: type[T],
     params: dict[str, Any],
     *,
     commit: bool = False,
 ) -> T:
     """Create SQLAlchemy model item and add it to DB."""
     item = model(**params)
@@ -160,15 +160,15 @@
     except SQLAlchemyError:
         session.rollback()
         raise
     return item
 
 
 async def create_db_item_async(
-    session: 'AsyncSession',
+    session: "AsyncSession",
     model: type[T],
     params: dict[str, Any],
     *,
     commit: bool = False,
 ) -> T:
     """Create SQLAlchemy model item and add it to DB."""
     item = model(**params)
@@ -182,41 +182,41 @@
 
 
 class Base(DeclarativeBase):  # noqa
     pass
 
 
 class MyModel(Base):  # noqa
-    __tablename__ = 'my_model'
+    __tablename__ = "my_model"
 
     id: Mapped[int] = mapped_column(primary_key=True)  # noqa
     name: Mapped[str | None]
     other_name: Mapped[str | None]
     dt: Mapped[datetime.datetime | None]
     bl: Mapped[bool | None]
-    other_models: Mapped[list['OtherModel']] = relationship(back_populates='my_model', uselist=True)
+    other_models: Mapped[list["OtherModel"]] = relationship(back_populates="my_model", uselist=True)
 
     @hybrid_property
     def full_name(self):  # noqa # type: ignore
-        return self.name + '' + self.other_name  # type: ignore
+        return self.name + "" + self.other_name  # type: ignore
 
     @hybrid_method
     def get_full_name(self):  # noqa # type: ignore
-        return self.name + '' + self.other_name  # type: ignore
+        return self.name + "" + self.other_name  # type: ignore
 
 
 class OtherModel(Base):  # noqa
-    __tablename__ = 'other_model'
+    __tablename__ = "other_model"
 
     id: Mapped[int] = mapped_column(primary_key=True)  # noqa
     name: Mapped[str]
     other_name: Mapped[str]
-    my_model_id: Mapped[int | None] = mapped_column(ForeignKey('my_model.id', ondelete='CASCADE'))
-    my_model: Mapped['MyModel'] = relationship(back_populates='other_models', uselist=False)
+    my_model_id: Mapped[int | None] = mapped_column(ForeignKey("my_model.id", ondelete="CASCADE"))
+    my_model: Mapped["MyModel"] = relationship(back_populates="other_models", uselist=False)
 
     @hybrid_property
     def full_name(self):  # noqa
-        return self.name + '' + self.other_name
+        return self.name + "" + self.other_name
 
     @hybrid_method
     def get_full_name(self):  # noqa
-        return self.name + '' + self.other_name
+        return self.name + "" + self.other_name
```


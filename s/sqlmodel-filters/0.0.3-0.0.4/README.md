# Comparing `tmp/sqlmodel_filters-0.0.3.tar.gz` & `tmp/sqlmodel_filters-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_filters-0.0.3.tar", max compression
+gzip compressed data, was "sqlmodel_filters-0.0.4.tar", max compression
```

## Comparing `sqlmodel_filters-0.0.3.tar` & `sqlmodel_filters-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-03-30 08:49:16.062693 sqlmodel_filters-0.0.3/LICENSE
--rw-r--r--   0        0        0     7013 2024-03-30 08:49:16.062693 sqlmodel_filters-0.0.3/README.md
--rw-r--r--   0        0        0     1022 2024-03-30 08:49:31.774716 sqlmodel_filters-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       69 2024-03-30 08:49:16.062693 sqlmodel_filters-0.0.3/sqlmodel_filters/__init__.py
--rw-r--r--   0        0        0     4630 2024-03-30 08:49:16.062693 sqlmodel_filters-0.0.3/sqlmodel_filters/builder.py
--rw-r--r--   0        0        0     5506 2024-03-30 08:49:16.062693 sqlmodel_filters-0.0.3/sqlmodel_filters/components.py
--rw-r--r--   0        0        0      165 2024-03-30 08:49:16.062693 sqlmodel_filters-0.0.3/sqlmodel_filters/exceptions.py
--rw-r--r--   0        0        0      493 2024-03-30 08:49:16.062693 sqlmodel_filters-0.0.3/sqlmodel_filters/utils.py
--rw-r--r--   0        0        0     7598 1970-01-01 00:00:00.000000 sqlmodel_filters-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7420 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/README.md
+-rw-r--r--   0        0        0     1022 2024-04-13 23:39:49.324200 sqlmodel_filters-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/sqlmodel_filters/__init__.py
+-rw-r--r--   0        0        0     4550 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/sqlmodel_filters/builder.py
+-rw-r--r--   0        0        0     5689 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/sqlmodel_filters/components.py
+-rw-r--r--   0        0        0      165 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/sqlmodel_filters/exceptions.py
+-rw-r--r--   0        0        0      637 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/sqlmodel_filters/utils.py
+-rw-r--r--   0        0        0     8005 1970-01-01 00:00:00.000000 sqlmodel_filters-0.0.4/PKG-INFO
```

### Comparing `sqlmodel_filters-0.0.3/LICENSE` & `sqlmodel_filters-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel_filters-0.0.3/README.md` & `sqlmodel_filters-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -124,21 +124,30 @@
 ### `Word` (`Term`)
 
 - Double quote a value if you want to use the equal operator.
 - The `LIKE` operator is used when you don't double quote a value.
 - Use `?` (a single character wildcard) or `*` (a multiple character wildcard) to control a LIKE operator pattern.
 - `*` is converted as `IS NOT NULL`.
 
-| Query               | SQL (Where Clause)                 |
-| ------------------- | ---------------------------------- |
-| `name:"Spider-Boy"` | `WHERE hero.name = 'Spider-Boy'`   |
-| `name:Spider`       | `WHERE hero.name LIKE '%Spider%'`  |
-| `name:Deadpond?`    | `WHERE hero.name LIKE 'Deadpond_'` |
-| `name:o*`           | `WHERE hero.name LIKE 'o%'`        |
-| `name:*`            | `WHERE hero.name IS NOT NULL`      |
+| Query              | SQL (Where Clause)                 |
+| ------------------ | ---------------------------------- |
+| `name:Spider-Boy"` | `WHERE hero.name = 'Spider-Boy'`   |
+| `name:Spider`      | `WHERE hero.name LIKE '%Spider%'`  |
+| `name:Deadpond?`   | `WHERE hero.name LIKE 'Deadpond_'` |
+| `name:o*`          | `WHERE hero.name LIKE 'o%'`        |
+| `name:*`           | `WHERE hero.name IS NOT NULL`      |
+
+### `REGEX`
+
+| Query               | SQL (Where Clause)                      |
+| ------------------- | --------------------------------------- |
+| `name:/Spider?Boy/` | `WHERE hero.name <regexp> 'Spider?Boy'` |
+
+> [!NOTE]
+> Regex support works differently per backend. See [SQLAlchemy docs](https://docs.sqlalchemy.org/en/20/core/sqlelement.html#sqlalchemy.sql.expression.ColumnElement.regexp_match) for details.
 
 ### `FROM` & `TO`
 
 | Query      | SQL (Where Clause)     |
 | ---------- | ---------------------- |
 | `age:>40`  | `WHERE hero.age > 40`  |
 | `age:>=40` | `WHERE hero.age >= 40` |
```

### Comparing `sqlmodel_filters-0.0.3/pyproject.toml` & `sqlmodel_filters-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlmodel-filters"
-version = "0.0.3"
+version = "0.0.4"
 description = "A Lucene query like fliltering for SQLModel"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sqlmodel_filters-0.0.3/sqlmodel_filters/builder.py` & `sqlmodel_filters-0.0.4/sqlmodel_filters/builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 from types import MappingProxyType
 from typing import Any, TypeVar
 
-from luqum.tree import (
-    AndOperation,
-    Group,
-    Item,
-    Not,
-    OrOperation,
-    SearchField,
-    UnknownOperation,
-)
+from luqum.tree import AndOperation, Group, Item, Not, OrOperation, SearchField, UnknownOperation
 from luqum.visitor import TreeVisitor
 from sqlalchemy.sql._typing import _ColumnExpressionArgument
 from sqlmodel import SQLModel, and_, not_, or_, select
 from sqlmodel.sql.expression import Select, SelectOfScalar
 
 from sqlmodel_filters.exceptions import IllegalFilterError
 
@@ -28,63 +20,55 @@
 
         self.model = model
         self.relationships = MappingProxyType(relationships or {})
 
         self.expressions: list[_ColumnExpressionArgument] = []
         self._analyzed_positions: set[int] = set()
 
-    def get_search_fields_expressions(self, node: SearchField):
-        if (node.pos or -1) in self._analyzed_positions:
-            return
-
-        self._analyzed_positions.add(node.pos or -1)
-        for child in node.children:
-            wrapper = SearchFieldNode(child, model=self.model, name=node.name, relationships=self.relationships)
-            yield from wrapper.get_expressions()
-
     def get_expressions(self, node: Item):
         match node:
             case SearchField():
-                yield from self.get_search_fields_expressions(node)
+                yield from self._handel_search_field(node)
             case Not():
                 search_field = node.children[0]
-                for condition in self.get_search_fields_expressions(search_field):
+                for condition in self._handel_search_field(search_field):
                     yield not_(condition)
+            case Group():
+                yield from self._handle_group(node)
             case AndOperation():
                 yield from self._handle_and_operation(node)
             case OrOperation():
                 yield from self._handle_or_operation(node)
-            case Group():
-                expressions = []
-                for child in node.children:
-                    expressions.extend(list(self.get_expressions(child)))
-
-                if len(expressions) > 0:
-                    yield and_(*expressions)
-
             case unknown:
                 raise IllegalFilterError(f"{unknown.__class__} is not supported yet")
 
-    def _handle_and_operation(self, node: AndOperation):
-        expressions: list[Any] = []
-        for child in node.children:
-            expressions.extend(list(self.get_expressions(child)))
+    def _handel_search_field(self, node: SearchField):
+        if (node.pos or -1) in self._analyzed_positions:
+            return
 
-        if len(expressions) > 0:
-            yield and_(*expressions)
+        self._analyzed_positions.add(node.pos or -1)
+        for child in node.children:
+            wrapper = SearchFieldNode(child, model=self.model, name=node.name, relationships=self.relationships)
+            yield from wrapper.get_expressions()
 
     def visit_search_field(self, node: SearchField, context: dict):
         self.expressions.extend(list(self.get_expressions(node)))
         yield from super().generic_visit(node, context)
 
-    def visit_unknown_operation(self, node: UnknownOperation, context: dict):
+    def _handle_group(self, node: Group):
+        # NOTE: group can be processed as And operation
+        yield from self._handle_and_operation(node)  # type: ignore
+
+    def _handle_and_operation(self, node: AndOperation):
+        expressions: list[Any] = []
         for child in node.children:
-            self.expressions.extend(list(self.get_expressions(child)))
+            expressions.extend(list(self.get_expressions(child)))
 
-        yield from super().generic_visit(node, context)
+        if len(expressions) > 0:
+            yield and_(*expressions)
 
     def visit_and_operation(self, node: AndOperation, context: dict):
         self.expressions.extend(list(self._handle_and_operation(node)))
         yield from super().generic_visit(node, context)
 
     def _handle_or_operation(self, node: OrOperation):
         expressions: list[Any] = []
@@ -95,14 +79,20 @@
             first, *others = expressions
             yield or_(first, *others)
 
     def visit_or_operation(self, node: OrOperation, context: dict):
         self.expressions.extend(list(self._handle_or_operation(node)))
         yield from super().generic_visit(node, context)
 
+    def visit_unknown_operation(self, node: UnknownOperation, context: dict):
+        for child in node.children:
+            self.expressions.extend(list(self.get_expressions(child)))
+
+        yield from super().generic_visit(node, context)
+
     def __call__(self, tree: Item):
         # NOTE: initialize expressions and _processed_positions to ensure idempotency
         self.expressions = []
         self._analyzed_positions = set()
         self.visit(tree)
         return self.expressions
```

### Comparing `sqlmodel_filters-0.0.3/sqlmodel_filters/components.py` & `sqlmodel_filters-0.0.4/sqlmodel_filters/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 from types import MappingProxyType
 from typing import TypeVar
 
-from luqum.tree import (
-    From,
-    Item,
-    Phrase,
-    Range,
-    To,
-    Word,
-)
+from luqum.tree import From, Item, Phrase, Range, Regex, To, Word
 from sqlalchemy.orm.attributes import InstrumentedAttribute
 from sqlalchemy.sql._typing import _ColumnExpressionArgument
 from sqlmodel import SQLModel, and_
 
 from .exceptions import IllegalFieldError, IllegalFilterError
-from .utils import cast_by_annotation, dequote
+from .utils import cast_by_annotation, dequote, deslash
 
 ModelType = TypeVar("ModelType", bound=SQLModel)
 
 
 def replace_wildcards(s: str, *, mapping: MappingProxyType[str, str]):
     for k, v in mapping.items():
         s = s.replace(k, v)
@@ -136,14 +129,15 @@
     def _range_expressions(self, range: Range):
         expressions: list[_ColumnExpressionArgument] = []
 
         if range.include_high:
             expressions.append(self.field <= cast_by_annotation(range.high.value, self.annotation))
         else:
             expressions.append(self.field < cast_by_annotation(range.high.value, self.annotation))
+
         if range.include_low:
             expressions.append(self.field >= cast_by_annotation(range.low.value, self.annotation))
         else:
             expressions.append(self.field > cast_by_annotation(range.low.value, self.annotation))
 
         yield and_(*expressions)
 
@@ -157,21 +151,26 @@
     def _to_expression(self, to: To):
         child: Word = to.children[0]
         if to.include:
             yield self.field <= cast_by_annotation(child.value, self.annotation)
         else:
             yield self.field < cast_by_annotation(child.value, self.annotation)
 
+    def _regex_expression(self, regex: Regex):
+        yield self.field.regexp_match(deslash(regex.value))
+
     def get_expressions(self):
         match self.node:
             case Phrase():
                 yield from self._phrase_expression(self.node)
             case Word():
                 yield from self._word_expression(self.node)
             case Range():
                 yield from self._range_expressions(self.node)
             case From():
                 yield from self._from_expression(self.node)
             case To():
                 yield from self._to_expression(self.node)
+            case Regex():
+                yield from self._regex_expression(self.node)
             case unknown:
                 raise IllegalFilterError(f"{unknown.__class__} is not supported yet")
```

### Comparing `sqlmodel_filters-0.0.3/PKG-INFO` & `sqlmodel_filters-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmodel-filters
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Lucene query like fliltering for SQLModel
 License: MIT
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -141,21 +141,30 @@
 ### `Word` (`Term`)
 
 - Double quote a value if you want to use the equal operator.
 - The `LIKE` operator is used when you don't double quote a value.
 - Use `?` (a single character wildcard) or `*` (a multiple character wildcard) to control a LIKE operator pattern.
 - `*` is converted as `IS NOT NULL`.
 
-| Query               | SQL (Where Clause)                 |
-| ------------------- | ---------------------------------- |
-| `name:"Spider-Boy"` | `WHERE hero.name = 'Spider-Boy'`   |
-| `name:Spider`       | `WHERE hero.name LIKE '%Spider%'`  |
-| `name:Deadpond?`    | `WHERE hero.name LIKE 'Deadpond_'` |
-| `name:o*`           | `WHERE hero.name LIKE 'o%'`        |
-| `name:*`            | `WHERE hero.name IS NOT NULL`      |
+| Query              | SQL (Where Clause)                 |
+| ------------------ | ---------------------------------- |
+| `name:Spider-Boy"` | `WHERE hero.name = 'Spider-Boy'`   |
+| `name:Spider`      | `WHERE hero.name LIKE '%Spider%'`  |
+| `name:Deadpond?`   | `WHERE hero.name LIKE 'Deadpond_'` |
+| `name:o*`          | `WHERE hero.name LIKE 'o%'`        |
+| `name:*`           | `WHERE hero.name IS NOT NULL`      |
+
+### `REGEX`
+
+| Query               | SQL (Where Clause)                      |
+| ------------------- | --------------------------------------- |
+| `name:/Spider?Boy/` | `WHERE hero.name <regexp> 'Spider?Boy'` |
+
+> [!NOTE]
+> Regex support works differently per backend. See [SQLAlchemy docs](https://docs.sqlalchemy.org/en/20/core/sqlelement.html#sqlalchemy.sql.expression.ColumnElement.regexp_match) for details.
 
 ### `FROM` & `TO`
 
 | Query      | SQL (Where Clause)     |
 | ---------- | ---------------------- |
 | `age:>40`  | `WHERE hero.age > 40`  |
 | `age:>=40` | `WHERE hero.age >= 40` |
```


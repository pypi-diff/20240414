# Comparing `tmp/pyontoenv-0.1.2.tar.gz` & `tmp/pyontoenv-0.1.3.tar.gz`

## Comparing `pyontoenv-0.1.2.tar` & `pyontoenv-0.1.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0      501       20      776 2024-04-05 16:43:55.000000 pyontoenv-0.1.2/lib/Cargo.toml
--rw-r--r--   0      501       20     5083 2024-04-13 03:19:17.000000 pyontoenv-0.1.2/lib/src/config.rs
--rw-r--r--   0      501       20     2071 2024-04-06 02:39:54.000000 pyontoenv-0.1.2/lib/src/consts.rs
--rw-r--r--   0      501       20     3267 2024-04-05 19:54:52.000000 pyontoenv-0.1.2/lib/src/doctor.rs
--rw-r--r--   0      501       20    38923 2024-04-13 03:20:14.000000 pyontoenv-0.1.2/lib/src/lib.rs
--rw-r--r--   0      501       20    13388 2024-04-10 05:51:17.000000 pyontoenv-0.1.2/lib/src/ontology.rs
--rw-r--r--   0      501       20     3521 2024-04-05 19:55:30.000000 pyontoenv-0.1.2/lib/src/policy.rs
--rw-r--r--   0      501       20     5326 2024-04-09 18:57:13.000000 pyontoenv-0.1.2/lib/src/util.rs
--rw-r--r--   0      501       20  1689944 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/Brick-1.3.ttl
--rw-r--r--   0      501       20     1248 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/model
--rw-r--r--   0      501       20      321 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/model.n3
--rw-r--r--   0      501       20      537 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/model.nt
--rw-r--r--   0      501       20     1248 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/model.ttl
--rw-r--r--   0      501       20      789 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/model.xml
--rw-r--r--   0      501       20      909 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
--rw-r--r--   0      501       20   146214 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
--rw-r--r--   0      501       20    30521 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
--rw-r--r--   0      501       20   163975 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
--rw-r--r--   0      501       20    18438 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
--rw-r--r--   0      501       20    18438 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
--rw-r--r--   0      501       20  1323794 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
--rw-r--r--   0      501       20    17472 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
--rw-r--r--   0      501       20  1456008 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
--rw-r--r--   0      501       20   104496 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
--rw-r--r--   0      501       20  1255550 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/bacnet.ttl
--rw-r--r--   0      501       20    44502 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/brickpatches.ttl
--rw-r--r--   0      501       20    81761 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/rec.ttl
--rw-r--r--   0      501       20     4069 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/recimports.ttl
--rw-r--r--   0      501       20    11876 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/lib/tests/data/support/ref-schema.ttl
--rw-r--r--   0      501       20     1160 2024-04-09 16:33:12.000000 pyontoenv-0.1.2/lib/tests/data2/ont1.ttl
--rw-r--r--   0      501       20     1132 2024-04-09 16:33:13.000000 pyontoenv-0.1.2/lib/tests/data2/ont2.ttl
--rw-r--r--   0      501       20     1135 2024-04-09 16:33:29.000000 pyontoenv-0.1.2/lib/tests/data2/ont3.ttl
--rw-r--r--   0      501       20     1106 2024-04-09 16:33:46.000000 pyontoenv-0.1.2/lib/tests/data2/ont4.ttl
--rw-r--r--   0      501       20     1248 2024-04-09 16:46:26.000000 pyontoenv-0.1.2/lib/tests/fileendings/model
--rw-r--r--   0      501       20      321 2024-04-09 16:46:26.000000 pyontoenv-0.1.2/lib/tests/fileendings/model.n3
--rw-r--r--   0      501       20      537 2024-04-09 16:46:26.000000 pyontoenv-0.1.2/lib/tests/fileendings/model.nt
--rw-r--r--   0      501       20     1248 2024-04-09 16:46:26.000000 pyontoenv-0.1.2/lib/tests/fileendings/model.ttl
--rw-r--r--   0      501       20      789 2024-04-09 16:46:26.000000 pyontoenv-0.1.2/lib/tests/fileendings/model.xml
--rw-r--r--   0      501       20  1689944 2024-04-03 15:52:01.000000 pyontoenv-0.1.2/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
--rw-r--r--   0      501       20     1160 2024-04-09 19:04:23.000000 pyontoenv-0.1.2/lib/tests/updates/v1/ont1.ttl
--rw-r--r--   0      501       20     1132 2024-04-09 19:04:23.000000 pyontoenv-0.1.2/lib/tests/updates/v1/ont2.ttl
--rw-r--r--   0      501       20     1135 2024-04-09 19:04:48.000000 pyontoenv-0.1.2/lib/tests/updates/v1/ont3.ttl
--rw-r--r--   0      501       20     1106 2024-04-09 19:05:31.000000 pyontoenv-0.1.2/lib/tests/updates/v1/ont4.ttl
--rw-r--r--   0      501       20     1135 2024-04-09 19:05:07.000000 pyontoenv-0.1.2/lib/tests/updates/v2/ont3.ttl
--rw-r--r--   0      501       20     1129 2024-04-10 00:42:38.000000 pyontoenv-0.1.2/lib/tests/updates/v2/ont5.ttl
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.2/python/Cargo.toml
--rw-r--r--   0      501       20     2886 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/python/.github/workflows/CI.yml
--rw-r--r--   0      501       20      686 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/python/.gitignore
--rw-r--r--   0      501       20       71 2024-03-28 12:07:46.000000 pyontoenv-0.1.2/python/build.rs
--rw-r--r--   0      501       20     5241 2024-04-14 04:04:40.000000 pyontoenv-0.1.2/python/poetry.lock
--rw-r--r--   0      501       20       71 2024-04-05 23:45:30.000000 pyontoenv-0.1.2/python/requirements.dev.txt
--rw-r--r--   0      501       20    10002 2024-04-13 03:21:13.000000 pyontoenv-0.1.2/python/src/lib.rs
--rw-r--r--   0      501       20      496 2024-04-05 15:29:24.000000 pyontoenv-0.1.2/python/test.py
--rw-r--r--   0      501       20      206 2024-04-13 23:20:44.000000 pyontoenv-0.1.2/python/token
--rw-r--r--   0      501       20    73455 2024-04-13 23:22:53.000000 pyontoenv-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 pyontoenv-0.1.2/Cargo.toml
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 pyontoenv-0.1.2/PKG-INFO
+-rw-r--r--   0      501       20      776 2024-04-05 16:43:55.000000 pyontoenv-0.1.3/lib/Cargo.toml
+-rw-r--r--   0      501       20     5324 2024-04-14 16:26:59.000000 pyontoenv-0.1.3/lib/src/config.rs
+-rw-r--r--   0      501       20     2071 2024-04-06 02:39:54.000000 pyontoenv-0.1.3/lib/src/consts.rs
+-rw-r--r--   0      501       20     3267 2024-04-05 19:54:52.000000 pyontoenv-0.1.3/lib/src/doctor.rs
+-rw-r--r--   0      501       20      350 2024-04-14 15:35:07.000000 pyontoenv-0.1.3/lib/src/errors.rs
+-rw-r--r--   0      501       20    39347 2024-04-14 16:49:50.000000 pyontoenv-0.1.3/lib/src/lib.rs
+-rw-r--r--   0      501       20    13633 2024-04-14 04:36:13.000000 pyontoenv-0.1.3/lib/src/ontology.rs
+-rw-r--r--   0      501       20     3521 2024-04-05 19:55:30.000000 pyontoenv-0.1.3/lib/src/policy.rs
+-rw-r--r--   0      501       20     6428 2024-04-14 16:50:33.000000 pyontoenv-0.1.3/lib/src/util.rs
+-rw-r--r--   0      501       20  1689944 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/Brick-1.3.ttl
+-rw-r--r--   0      501       20     1248 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/model
+-rw-r--r--   0      501       20      321 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/model.n3
+-rw-r--r--   0      501       20      537 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/model.nt
+-rw-r--r--   0      501       20     1248 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/model.ttl
+-rw-r--r--   0      501       20      789 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/model.xml
+-rw-r--r--   0      501       20      909 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
+-rw-r--r--   0      501       20   146214 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
+-rw-r--r--   0      501       20    30521 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
+-rw-r--r--   0      501       20   163975 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
+-rw-r--r--   0      501       20    18438 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
+-rw-r--r--   0      501       20    18438 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
+-rw-r--r--   0      501       20  1323794 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
+-rw-r--r--   0      501       20    17472 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0      501       20  1456008 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0      501       20   104496 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
+-rw-r--r--   0      501       20  1255550 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/bacnet.ttl
+-rw-r--r--   0      501       20    44502 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/brickpatches.ttl
+-rw-r--r--   0      501       20    81761 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/rec.ttl
+-rw-r--r--   0      501       20     4069 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/recimports.ttl
+-rw-r--r--   0      501       20    11876 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/lib/tests/data/support/ref-schema.ttl
+-rw-r--r--   0      501       20     1160 2024-04-09 16:33:12.000000 pyontoenv-0.1.3/lib/tests/data2/ont1.ttl
+-rw-r--r--   0      501       20     1132 2024-04-09 16:33:13.000000 pyontoenv-0.1.3/lib/tests/data2/ont2.ttl
+-rw-r--r--   0      501       20     1135 2024-04-09 16:33:29.000000 pyontoenv-0.1.3/lib/tests/data2/ont3.ttl
+-rw-r--r--   0      501       20     1106 2024-04-09 16:33:46.000000 pyontoenv-0.1.3/lib/tests/data2/ont4.ttl
+-rw-r--r--   0      501       20     1248 2024-04-09 16:46:26.000000 pyontoenv-0.1.3/lib/tests/fileendings/model
+-rw-r--r--   0      501       20      321 2024-04-09 16:46:26.000000 pyontoenv-0.1.3/lib/tests/fileendings/model.n3
+-rw-r--r--   0      501       20      537 2024-04-09 16:46:26.000000 pyontoenv-0.1.3/lib/tests/fileendings/model.nt
+-rw-r--r--   0      501       20     1248 2024-04-09 16:46:26.000000 pyontoenv-0.1.3/lib/tests/fileendings/model.ttl
+-rw-r--r--   0      501       20      789 2024-04-09 16:46:26.000000 pyontoenv-0.1.3/lib/tests/fileendings/model.xml
+-rw-r--r--   0      501       20  1689944 2024-04-03 15:52:01.000000 pyontoenv-0.1.3/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
+-rw-r--r--   0      501       20     1160 2024-04-09 19:04:23.000000 pyontoenv-0.1.3/lib/tests/updates/v1/ont1.ttl
+-rw-r--r--   0      501       20     1132 2024-04-09 19:04:23.000000 pyontoenv-0.1.3/lib/tests/updates/v1/ont2.ttl
+-rw-r--r--   0      501       20     1135 2024-04-09 19:04:48.000000 pyontoenv-0.1.3/lib/tests/updates/v1/ont3.ttl
+-rw-r--r--   0      501       20     1106 2024-04-09 19:05:31.000000 pyontoenv-0.1.3/lib/tests/updates/v1/ont4.ttl
+-rw-r--r--   0      501       20     1135 2024-04-09 19:05:07.000000 pyontoenv-0.1.3/lib/tests/updates/v2/ont3.ttl
+-rw-r--r--   0      501       20     1129 2024-04-10 00:42:38.000000 pyontoenv-0.1.3/lib/tests/updates/v2/ont5.ttl
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.3/python/Cargo.toml
+-rw-r--r--   0      501       20     2886 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/python/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      686 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/python/.gitignore
+-rw-r--r--   0      501       20       71 2024-03-28 12:07:46.000000 pyontoenv-0.1.3/python/build.rs
+-rw-r--r--   0      501       20     5241 2024-04-14 04:04:40.000000 pyontoenv-0.1.3/python/poetry.lock
+-rw-r--r--   0      501       20       71 2024-04-05 23:45:30.000000 pyontoenv-0.1.3/python/requirements.dev.txt
+-rw-r--r--   0      501       20    10088 2024-04-14 16:21:17.000000 pyontoenv-0.1.3/python/src/lib.rs
+-rw-r--r--   0      501       20      349 2024-04-14 16:11:39.000000 pyontoenv-0.1.3/python/test.py
+-rw-r--r--   0      501       20      206 2024-04-13 23:20:44.000000 pyontoenv-0.1.3/python/token
+-rw-r--r--   0      501       20    73455 2024-04-14 16:51:25.000000 pyontoenv-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 pyontoenv-0.1.3/Cargo.toml
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 pyontoenv-0.1.3/PKG-INFO
```

### Comparing `pyontoenv-0.1.2/lib/Cargo.toml` & `pyontoenv-0.1.3/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/src/config.rs` & `pyontoenv-0.1.3/lib/src/config.rs`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,21 @@
         for exclude in excludes {
             let pat = Pattern::new(&exclude)?;
             config.excludes.push(pat);
         }
         Ok(config)
     }
 
+    pub fn default_offline<K>(root: PathBuf, search_directories: Option<K>) -> Result<Self>
+    where
+        K: IntoIterator<Item = PathBuf>,
+    {
+        Self::new_with_default_matches(root, search_directories, false, false, true)
+    }
+
     pub fn new_with_default_matches<K>(
         root: PathBuf,
         search_directories: Option<K>,
         require_ontology_names: bool,
         strict: bool,
         offline: bool,
     ) -> Result<Self>
```

### Comparing `pyontoenv-0.1.2/lib/src/consts.rs` & `pyontoenv-0.1.3/lib/src/consts.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/src/doctor.rs` & `pyontoenv-0.1.3/lib/src/doctor.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/src/lib.rs` & `pyontoenv-0.1.3/lib/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 extern crate derive_builder;
 
 pub mod config;
 pub mod consts;
 pub mod doctor;
+pub mod errors;
 pub mod ontology;
 pub mod policy;
 #[macro_use]
 pub mod util;
 
 use crate::config::Config;
 use crate::consts::{IMPORTS, ONTOLOGY, PREFIXES, TYPE};
@@ -20,15 +21,15 @@
 };
 use oxigraph::store::Store;
 use petgraph::graph::{Graph as DiGraph, NodeIndex};
 use serde::{Deserialize, Serialize};
 use std::collections::HashMap;
 use std::collections::{HashSet, VecDeque};
 use std::io::{BufReader, Write};
-use std::path::{Path};
+use std::path::Path;
 
 // custom derive for ontologies field as vec of Ontology
 fn ontologies_ser<S>(
     ontologies: &HashMap<GraphIdentifier, Ontology>,
     s: S,
 ) -> Result<S::Ok, S::Error>
 where
@@ -110,14 +111,21 @@
     pub fn get_ontology_by_name(&self, name: NamedNodeRef) -> Option<&Ontology> {
         // choose the first ontology with the given name
         self.ontologies
             .values()
             .find(|&ontology| ontology.name() == name)
     }
 
+    pub fn get_graph_by_name(&self, name: NamedNodeRef) -> Result<Graph> {
+        let ontology = self
+            .get_ontology_by_name(name)
+            .ok_or(anyhow::anyhow!("Ontology not found"))?;
+        self.get_graph(ontology.id())
+    }
+
     fn get_ontology_by_location(&self, location: &OntologyLocation) -> Option<&Ontology> {
         // choose the first ontology with the given location
         self.ontologies
             .values()
             .find(|&ontology| ontology.location() == Some(location))
     }
 
@@ -155,15 +163,15 @@
     fn update_dependency_graph(&mut self, updated_ids: Option<Vec<GraphIdentifier>>) -> Result<()> {
         // traverse the owl:imports closure and build the dependency graph
         let mut stack: VecDeque<GraphIdentifier> = match updated_ids {
             Some(ids) => ids.into(),
             None => self.ontologies.keys().cloned().collect(),
         };
 
-        println!("Using # updated ids: {:?}", stack.len());
+        info!("Using # updated ids: {:?}", stack.len());
 
         while let Some(ontology) = stack.pop_front() {
             info!("Building dependency graph for: {:?}", ontology);
             let ont = self
                 .ontologies
                 .get(&ontology)
                 .ok_or(anyhow::anyhow!("Ontology not found"))?;
@@ -254,15 +262,15 @@
             if let Some(location) = ontology.location() {
                 if let OntologyLocation::File(f) = location {
                     let path = f.to_path_buf();
                     let metadata = std::fs::metadata(&path)?;
 
                     let last_updated: chrono::DateTime<Utc> = metadata.modified()?.into();
 
-                    println!(
+                    info!(
                         "Ontology: {:?}, last updated: {:?}; current: {:?}",
                         id, ontology.last_updated, last_updated
                     );
                     if last_updated >= ontology.last_updated.unwrap() {
                         updates.push(id.clone());
                     }
                 }
@@ -476,15 +484,15 @@
                 return Err(e);
             }
         };
 
         let mut ontology =
             Ontology::from_graph(&graph, location, self.config.require_ontology_names)?;
         ontology.with_last_updated(Utc::now());
-        println!(
+        info!(
             "Adding ontology: {:?} updated: {:?}",
             ontology.id(),
             ontology.last_updated
         );
         let id = ontology.id().clone();
         self.ontologies.insert(id.clone(), ontology);
 
@@ -774,62 +782,66 @@
     }
 }
 
 #[cfg(test)]
 mod tests {
 
     use super::*;
-    use std::ffi::OsStr;
+    use std::path::PathBuf;
     use tempdir::TempDir;
 
+    fn copy_file(path: &PathBuf, dest: &PathBuf) -> Result<()> {
+        println!("Copying {:?} to {:?}", path, dest);
+        if path.is_file() {
+            std::fs::copy(path, dest)?;
+        } else {
+            std::fs::create_dir_all(dest)?;
+        }
+        Ok(())
+    }
+
     fn setup(dir: &str) -> Result<TempDir> {
         // copy all files from tests/ to a temp directory and return the temp directory
         let test_dir = TempDir::new("ontoenv")?;
         // where test files are located
-        let base_dir = Path::new("tests/").join(&dir);
+        let base_dir = Path::new("tests/").join(dir);
         println!("Copying files from {:?} to {:?}", base_dir, test_dir.path());
         // destination directory
         for entry in walkdir::WalkDir::new(&base_dir) {
             let entry = entry?;
             let path = entry.path();
             let dest = test_dir.path().join(path.strip_prefix(&base_dir)?);
-            copy_file(&path.to_path_buf(), &dest)?;
+            copy_file(&path.into(), &dest)?;
         }
         Ok(test_dir)
     }
 
-    fn copy_file(path: &PathBuf, dest: &PathBuf) -> Result<()> {
-        println!("Copying {:?} to {:?}", path, dest);
-        if path.is_file() {
-            std::fs::copy(path, dest)?;
-        } else {
-            std::fs::create_dir_all(dest)?;
-        }
-        Ok(())
-    }
-
     fn default_config(dir: &TempDir) -> Config {
         Config::new(
             dir.path().into(),
             Some(vec![dir.path().into()]),
             &["*.ttl"],
             &[""],
             false,
+            false,
+            true,
             "default".to_string(),
         )
         .unwrap()
     }
 
     fn default_config_with_subdir(dir: &TempDir, path: &str) -> Config {
         Config::new(
             dir.path().into(),
-            Some(vec![dir.path().join(path).into()]),
+            Some(vec![dir.path().join(path)]),
             &["*.ttl"],
             &[""],
             false,
+            false,
+            true,
             "default".to_string(),
         )
         .unwrap()
     }
 
     // we don't care about errors when cleaning up the TempDir so
     // we just drop the TempDir (looking at this doc:
@@ -846,16 +858,21 @@
         teardown(dir);
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_scans_default() -> Result<()> {
         let dir = setup("data2")?;
-        let cfg =
-            Config::new_with_default_matches(dir.path().into(), Some([dir.path().into()]), false)?;
+        let cfg = Config::new_with_default_matches(
+            dir.path().into(),
+            Some([dir.path().into()]),
+            false,
+            false,
+            true,
+        )?;
         let mut env = OntoEnv::new(cfg)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
         teardown(dir);
         Ok(())
     }
 
@@ -864,14 +881,16 @@
         let dir = setup("fileendings")?;
         let cfg1 = Config::new(
             dir.path().into(),
             Some(vec![dir.path().into()]),
             &["*.n3"],
             &[""],
             false,
+            false,
+            true,
             "default".to_string(),
         )?;
         let mut env = OntoEnv::new(cfg1)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 1);
         assert_eq!(env.num_triples()?, 5);
         teardown(dir);
```

### Comparing `pyontoenv-0.1.2/lib/src/ontology.rs` & `pyontoenv-0.1.3/lib/src/ontology.rs`

 * *Files 1% similar despite different names*

```diff
@@ -236,14 +236,21 @@
         &self.version_properties
     }
 
     pub fn location(&self) -> Option<&OntologyLocation> {
         self.location.as_ref()
     }
 
+    pub fn graph(&self) -> Result<OxigraphGraph> {
+        if let Some(location) = &self.location {
+            return location.graph();
+        }
+        return OntologyLocation::from_str(self.name.as_str()).and_then(|loc| loc.graph());
+    }
+
     ///// Returns the graph for this ontology from the OntoEnv
     //pub fn graph(&self, env: &OntoEnv) -> Result<LightGraph> {
     //    if let Some(location) = &self.location {
     //        return location.graph();
     //    }
     //    return OntologyLocation::from_str(self.name.as_str()).and_then(|loc| loc.graph());
     //}
```

### Comparing `pyontoenv-0.1.2/lib/src/policy.rs` & `pyontoenv-0.1.3/lib/src/policy.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/src/util.rs` & `pyontoenv-0.1.3/lib/src/util.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 use anyhow::Result;
 
+use std::io::Read;
 use std::path::Path;
 
 use reqwest::header::CONTENT_TYPE;
 
 use oxigraph::io::write::GraphSerializer;
 use oxigraph::io::{GraphFormat, GraphParser};
 use oxigraph::model::graph::Graph as OxigraphGraph;
 use oxigraph::model::Dataset;
 use oxigraph::model::TripleRef;
 
 use std::io::BufReader;
 
-use log::debug;
+use log::{debug, info};
 
 pub fn write_dataset_to_file(dataset: &Dataset, file: &str) -> Result<()> {
-    println!(
+    info!(
         "Writing dataset to file: {} with length {}",
         file,
         dataset.len()
     );
     let mut file = std::fs::File::create(file)?;
     let mut serializer =
         GraphSerializer::from_format(GraphFormat::Turtle).triple_writer(&mut file)?;
@@ -55,40 +56,73 @@
     }
 
     Ok(graph)
 }
 
 pub fn read_url(file: &str) -> Result<OxigraphGraph> {
     debug!("Reading url: {}", file);
+
     let client = reqwest::blocking::Client::new();
     let resp = client
         .get(file)
-        .header(CONTENT_TYPE, "text/turtle")
+        .header(CONTENT_TYPE, "application/x-turtle")
         .send()?;
     if !resp.status().is_success() {
         return Err(anyhow::anyhow!("Failed to fetch ontology from {}", file));
     }
     let content_type = resp.headers().get("Content-Type");
-    let content: BufReader<_> = BufReader::new(reqwest::blocking::get(file)?);
     let content_type = content_type.and_then(|ct| ct.to_str().ok());
     let content_type = content_type.and_then(|ext| match ext {
-        "ttl" => Some(GraphFormat::Turtle),
-        "xml" => Some(GraphFormat::RdfXml),
-        "n3" => Some(GraphFormat::NTriples),
-        "nt" => Some(GraphFormat::NTriples),
-        _ => None,
+        "application/x-turtle" => Some(GraphFormat::Turtle),
+        "application/rdf+xml" => Some(GraphFormat::RdfXml),
+        "text/rdf+n3" => Some(GraphFormat::NTriples),
+        _ => {
+            debug!("Unknown content type: {}", ext);
+            None
+        }
     });
-    let parser = GraphParser::from_format(content_type.unwrap_or(GraphFormat::Turtle));
-    let mut graph = OxigraphGraph::new();
-    let triples = parser.read_triples(content)?;
-    for triple in triples {
-        graph.insert(&triple?);
+
+    let content: BufReader<_> = BufReader::new(std::io::Cursor::new(resp.bytes()?));
+
+    // if content type is known, use it to parse the graph
+    if let Some(format) = content_type {
+        let parser = GraphParser::from_format(format);
+        let mut graph = OxigraphGraph::new();
+        let triples = parser.read_triples(content)?;
+        for triple in triples {
+            graph.insert(&triple?);
+        }
+        return Ok(graph);
     }
 
-    Ok(graph)
+    // if content  type is unknown, try all formats. Requires us to make a copy of the content
+    // since we can't rewind the reader
+    let content_vec: Vec<u8> = content.bytes().map(|b| b.unwrap()).collect();
+
+    for format in [
+        GraphFormat::Turtle,
+        GraphFormat::RdfXml,
+        GraphFormat::NTriples,
+    ] {
+        let vcontent = BufReader::new(std::io::Cursor::new(&content_vec));
+        let parser = GraphParser::from_format(format);
+        let mut graph = OxigraphGraph::new();
+
+        // if there's an error on parser.read_triples, try the next format
+
+        let triples = parser.read_triples(vcontent);
+        if triples.is_err() {
+            continue;
+        }
+        for triple in triples.unwrap() {
+            graph.insert(&triple?);
+        }
+        return Ok(graph);
+    }
+    Err(anyhow::anyhow!("Failed to parse graph from {}", file))
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use oxigraph::model::{Dataset, GraphNameRef, NamedNodeRef, QuadRef};
```

### Comparing `pyontoenv-0.1.2/lib/tests/data/Brick-1.3.ttl` & `pyontoenv-0.1.3/lib/tests/data/Brick-1.3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/model` & `pyontoenv-0.1.3/lib/tests/data/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/model.nt` & `pyontoenv-0.1.3/lib/tests/data/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/model.ttl` & `pyontoenv-0.1.3/lib/tests/data/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/model.xml` & `pyontoenv-0.1.3/lib/tests/data/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/bacnet.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/bacnet.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/brickpatches.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/brickpatches.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/rec.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/rec.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/recimports.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/recimports.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data/support/ref-schema.ttl` & `pyontoenv-0.1.3/lib/tests/data/support/ref-schema.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data2/ont1.ttl` & `pyontoenv-0.1.3/lib/tests/data2/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data2/ont2.ttl` & `pyontoenv-0.1.3/lib/tests/data2/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data2/ont3.ttl` & `pyontoenv-0.1.3/lib/tests/data2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/data2/ont4.ttl` & `pyontoenv-0.1.3/lib/tests/data2/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/fileendings/model` & `pyontoenv-0.1.3/lib/tests/fileendings/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/fileendings/model.nt` & `pyontoenv-0.1.3/lib/tests/fileendings/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/fileendings/model.ttl` & `pyontoenv-0.1.3/lib/tests/fileendings/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/fileendings/model.xml` & `pyontoenv-0.1.3/lib/tests/fileendings/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl` & `pyontoenv-0.1.3/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/updates/v1/ont1.ttl` & `pyontoenv-0.1.3/lib/tests/updates/v1/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/updates/v1/ont2.ttl` & `pyontoenv-0.1.3/lib/tests/updates/v1/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/updates/v1/ont3.ttl` & `pyontoenv-0.1.3/lib/tests/updates/v1/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/updates/v1/ont4.ttl` & `pyontoenv-0.1.3/lib/tests/updates/v1/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/updates/v2/ont3.ttl` & `pyontoenv-0.1.3/lib/tests/updates/v2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/lib/tests/updates/v2/ont5.ttl` & `pyontoenv-0.1.3/lib/tests/updates/v2/ont5.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/python/Cargo.toml` & `pyontoenv-0.1.3/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/python/.github/workflows/CI.yml` & `pyontoenv-0.1.3/python/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/python/.gitignore` & `pyontoenv-0.1.3/python/.gitignore`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/python/poetry.lock` & `pyontoenv-0.1.3/python/poetry.lock`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.2/python/src/lib.rs` & `pyontoenv-0.1.3/python/src/lib.rs`

 * *Files 13% similar despite different names*

```diff
@@ -115,44 +115,39 @@
 struct Config {
     cfg: ontoenvrs::config::Config,
 }
 
 #[pymethods]
 impl Config {
     #[new]
+    #[pyo3(signature = (root, search_directories, require_ontology_names=false, strict=false, offline=false, resolution_policy="default".to_owned(), includes=vec![], excludes=vec![]))]
     fn new(
-        root: Bound<'_, PyString>,
-        search_directories: Vec<Bound<'_, PyString>>,
-        includes: Vec<Bound<'_, PyString>>,
-        excludes: Vec<Bound<'_, PyString>>,
-        require_ontology_names: Bound<'_, PyBool>,
-        strict: Bound<'_, PyBool>,
-        offline: Bound<'_, PyBool>,
-        resolution_policy: Bound<'_, PyString>,
+        root: String,
+        search_directories: Vec<String>,
+        require_ontology_names: bool,
+        strict: bool,
+        offline: bool,
+        resolution_policy: String,
+        includes: Option<Vec<String>>,
+        excludes: Option<Vec<String>>,
     ) -> PyResult<Self> {
         Ok(Config {
             cfg: ontoenvrs::config::Config::new(
                 root.to_string().into(),
                 Some(
                     search_directories
                         .iter()
                         .map(|s| s.to_string().into())
                         .collect::<Vec<PathBuf>>(),
                 ),
-                includes
-                    .iter()
-                    .map(|s| s.to_string())
-                    .collect::<Vec<String>>(),
-                excludes
-                    .iter()
-                    .map(|s| s.to_string())
-                    .collect::<Vec<String>>(),
-                require_ontology_names.is_true(),
-                strict.is_true(),
-                offline.is_true(),
+                includes.unwrap_or_else(|| vec![]).iter().map(|s| s.to_string()).collect::<Vec<_>>(),
+                excludes.unwrap_or_else(|| vec![]).iter().map(|s| s.to_string()).collect::<Vec<_>>(),
+                require_ontology_names,
+                strict,
+                offline,
                 resolution_policy.to_string(),
             )
             .map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string()))?,
         })
     }
 }
 
@@ -201,14 +196,15 @@
         Ok(format!(
             "<OntoEnv: {} graphs, {} triples>",
             self.inner.num_graphs(),
             self.inner.num_triples().map_err(anyhow_to_pyerr)?
         ))
     }
 
+    #[pyo3(signature = (uri, destination_graph, rewrite_sh_prefixes=false, remove_owl_imports=false))]
     fn get_closure(
         &self,
         py: Python,
         uri: &str,
         destination_graph: &Bound<'_, PyAny>,
         rewrite_sh_prefixes: bool,
         remove_owl_imports: bool,
```

### Comparing `pyontoenv-0.1.2/Cargo.lock` & `pyontoenv-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1400,15 +1400,15 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ontoenv"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "derive_builder",
  "env_logger",
  "glob",
@@ -1426,15 +1426,15 @@
  "tempdir",
  "tempfile",
  "walkdir",
 ]
 
 [[package]]
 name = "ontoenv-cli"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "env_logger",
  "ontoenv",
  "oxigraph",
@@ -1794,15 +1794,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyontoenv"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anyhow",
  "env_logger",
  "log",
  "ontoenv",
  "oxigraph",
  "pyo3",
```

### Comparing `pyontoenv-0.1.2/Cargo.toml` & `pyontoenv-0.1.3/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["python"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.2"
+version = "0.1.3"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD-3-Clause"
 edition = "2021"
 rust-version = "1.70"
 repository = "https://github.com/gtfierro/ontoenv-rs"
 homepage = "https://github.com/gtfierro/ontoenv-rs"
 description = "A tool for managing ontologies and their dependencies"
```

### Comparing `pyontoenv-0.1.2/pyproject.toml` & `pyontoenv-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 manifest-path = "python/Cargo.toml"
 
 [tool.poetry]
 name = "ontoenv"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python bindings for the OntoEnv Rust library. Manages ontology-based environments for building knowledge graphs."
 license = "bsd-3-clause"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pyontoenv-0.1.2/PKG-INFO` & `pyontoenv-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyontoenv
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Command line tool to manage ontologies and their imports in a local environment
 Home-Page: https://github.com/gtfierro/ontoenv-rs
 Author: Gabe Fierro <gtfierro@mines.edu>
 Author-email: Gabe Fierro <gtfierro@mines.edu>
```


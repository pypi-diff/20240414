# Comparing `tmp/adls_acl-0.0.4.tar.gz` & `tmp/adls_acl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adls_acl-0.0.4.tar", last modified: Sun Apr  7 23:37:02 2024, max compression
+gzip compressed data, was "adls_acl-0.0.5.tar", last modified: Sat Apr 13 23:56:24 2024, max compression
```

## Comparing `adls_acl-0.0.4.tar` & `adls_acl-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:37:02.563668 adls_acl-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-07 23:36:55.000000 adls_acl-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 23:36:55.000000 adls_acl-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-07 23:37:02.563668 adls_acl-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-04-07 23:36:55.000000 adls_acl-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-07 23:36:55.000000 adls_acl-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 23:37:02.563668 adls_acl-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-07 23:36:55.000000 adls_acl-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:37:02.559668 adls_acl-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:37:02.563668 adls_acl-0.0.4/src/adls_acl/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 23:36:55.000000 adls_acl-0.0.4/src/adls_acl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-07 23:36:55.000000 adls_acl-0.0.4/src/adls_acl/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-07 23:36:55.000000 adls_acl-0.0.4/src/adls_acl/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-07 23:36:55.000000 adls_acl-0.0.4/src/adls_acl/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-07 23:36:55.000000 adls_acl-0.0.4/src/adls_acl/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-07 23:36:55.000000 adls_acl-0.0.4/src/adls_acl/orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:37:02.563668 adls_acl-0.0.4/src/adls_acl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-07 23:37:02.000000 adls_acl-0.0.4/src/adls_acl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-07 23:37:02.000000 adls_acl-0.0.4/src/adls_acl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:37:02.000000 adls_acl-0.0.4/src/adls_acl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-07 23:37:02.000000 adls_acl-0.0.4/src/adls_acl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-07 23:37:02.000000 adls_acl-0.0.4/src/adls_acl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 23:37:02.000000 adls_acl-0.0.4/src/adls_acl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:37:02.563668 adls_acl-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-07 23:36:55.000000 adls_acl-0.0.4/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-07 23:36:55.000000 adls_acl-0.0.4/tests/test_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:56:24.867834 adls_acl-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-13 23:56:19.000000 adls_acl-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 23:56:19.000000 adls_acl-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-13 23:56:24.867834 adls_acl-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-13 23:56:19.000000 adls_acl-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-13 23:56:19.000000 adls_acl-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 23:56:24.867834 adls_acl-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-13 23:56:19.000000 adls_acl-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:56:24.863834 adls_acl-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:56:24.863834 adls_acl-0.0.5/src/adls_acl/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 23:56:19.000000 adls_acl-0.0.5/src/adls_acl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-13 23:56:19.000000 adls_acl-0.0.5/src/adls_acl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-13 23:56:19.000000 adls_acl-0.0.5/src/adls_acl/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-13 23:56:19.000000 adls_acl-0.0.5/src/adls_acl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-13 23:56:19.000000 adls_acl-0.0.5/src/adls_acl/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-13 23:56:19.000000 adls_acl-0.0.5/src/adls_acl/orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:56:24.867834 adls_acl-0.0.5/src/adls_acl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-13 23:56:24.000000 adls_acl-0.0.5/src/adls_acl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-13 23:56:24.000000 adls_acl-0.0.5/src/adls_acl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 23:56:24.000000 adls_acl-0.0.5/src/adls_acl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 23:56:24.000000 adls_acl-0.0.5/src/adls_acl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-13 23:56:24.000000 adls_acl-0.0.5/src/adls_acl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 23:56:24.000000 adls_acl-0.0.5/src/adls_acl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 23:56:24.867834 adls_acl-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-13 23:56:19.000000 adls_acl-0.0.5/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-13 23:56:19.000000 adls_acl-0.0.5/tests/test_orchestrator.py
```

### Comparing `adls_acl-0.0.4/LICENSE` & `adls_acl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.4/PKG-INFO` & `adls_acl-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adls_acl
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).
 Home-page: https://github.com/karolusz/adls-acl
 Author: Karol Luszczek
 Author-email: karol.luszczek@reinsight.se
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -67,14 +67,15 @@
 Options:
   --debug          Enable debug messages.
   --silent         Suppress logs to stdout.
   --log-file TEXT  Redirect logs to a file.
   --help           Show this message and exit.
 
 Commands:
+  get-acl  Read the current fs and acls on dirs.
   set-acl  Read and set direcotry structure and ACLs from a YAML file.
 ```
 
 #### `set-acl` command
 ```
 Usage: adls-acl set-acl [OPTIONS] FILE
 
@@ -84,24 +85,44 @@
   --help  Show this message and exit.
 ```
 
 To set acls from an input file `test.yml` the shell command would look like:
 ```bash
 adls-acl set-acl test.yml
 ```
+
+#### `get-acl` command
+```
+Usage: adls-acl get-acl [OPTIONS] ACCOUNT_NAME OUTFILE
+
+  Read the current fs and acls on dirs.
+
+Options:
+  --omit-special        Omit special ACLs when reading the account.
+  --help                Show this message and exit.
+```
+
+This will print the current filesystem of an account (directories only, no files) and their ACLs to a file on a path pass as `OUTFILE` argument.
+[Special ACLs](#special-acls) can be omitted with a flag `--omit-special`
+
+To read ACLs of a ADLS storage account named `testaccount` to file `dump.yml`:
+```bash
+adls-acl get-acl testaccount dump.yml
+```
+
 ### Input file
 
 The YAML schema reference for the input files. Each input file represents a desired directory structure and ACLs for a single Azure Storage account. 
 
 ##### Input File Example
 Example of an input file for a fictitious storage account. All elements of the schema are explained in the following sections.
 
 ```yaml
 account: testaccount
-containers: 
+containers:
   - name: testcontainer1 
     acls:
       - oid: "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
         type: "user"
         acl: r-x
       - oid: "yyyyyyyy-yyyy-yyyy-yyyy-yyyyyyyyyyyy"
         type: "user"
```

### Comparing `adls_acl-0.0.4/README.md` & `adls_acl-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 Options:
   --debug          Enable debug messages.
   --silent         Suppress logs to stdout.
   --log-file TEXT  Redirect logs to a file.
   --help           Show this message and exit.
 
 Commands:
+  get-acl  Read the current fs and acls on dirs.
   set-acl  Read and set direcotry structure and ACLs from a YAML file.
 ```
 
 #### `set-acl` command
 ```
 Usage: adls-acl set-acl [OPTIONS] FILE
 
@@ -57,24 +58,44 @@
   --help  Show this message and exit.
 ```
 
 To set acls from an input file `test.yml` the shell command would look like:
 ```bash
 adls-acl set-acl test.yml
 ```
+
+#### `get-acl` command
+```
+Usage: adls-acl get-acl [OPTIONS] ACCOUNT_NAME OUTFILE
+
+  Read the current fs and acls on dirs.
+
+Options:
+  --omit-special        Omit special ACLs when reading the account.
+  --help                Show this message and exit.
+```
+
+This will print the current filesystem of an account (directories only, no files) and their ACLs to a file on a path pass as `OUTFILE` argument.
+[Special ACLs](#special-acls) can be omitted with a flag `--omit-special`
+
+To read ACLs of a ADLS storage account named `testaccount` to file `dump.yml`:
+```bash
+adls-acl get-acl testaccount dump.yml
+```
+
 ### Input file
 
 The YAML schema reference for the input files. Each input file represents a desired directory structure and ACLs for a single Azure Storage account. 
 
 ##### Input File Example
 Example of an input file for a fictitious storage account. All elements of the schema are explained in the following sections.
 
 ```yaml
 account: testaccount
-containers: 
+containers:
   - name: testcontainer1 
     acls:
       - oid: "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
         type: "user"
         acl: r-x
       - oid: "yyyyyyyy-yyyy-yyyy-yyyy-yyyyyyyyyyyy"
         type: "user"
```

### Comparing `adls_acl-0.0.4/pyproject.toml` & `adls_acl-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.0.4"
+current_version = "0.0.5"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `adls_acl-0.0.4/setup.py` & `adls_acl-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 readme = open("README.md", encoding="utf-8").read()
 
 setup(
     name="adls_acl",
-    version="0.0.4",
+    version="0.0.5",
     url="https://github.com/karolusz/adls-acl",
     author="Karol Luszczek",
     author_email="karol.luszczek@reinsight.se",
     description="A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `adls_acl-0.0.4/src/adls_acl/cli.py` & `adls_acl-0.0.5/src/adls_acl/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 # References:
 # https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-acl-python#update-acls-recursively
 #
 #
 # https://learn.microsoft.com/en-us/azure/storage/blobs/data-lake-storage-access-control#permissions-inheritance
 # default permissions have been set on the parent items before the child items have been created.
 #
-import click, logging, sys
-from enum import Enum
+import click, logging, yaml
 from .logger import configure_logger
 from .orchestrator import Orchestrator
 from .input_parser import config_from_yaml
 from .nodes import container_config_to_tree
 
 root_logger = logging.getLogger()  # Root Logger
 
@@ -22,20 +21,41 @@
 @click.option("--log-file", "log_file", default=None, help="Redirect logs to a file.")
 def cli(debug, silent, log_file):
     global root_logger
     root_logger = configure_logger(root_logger, debug, silent, log_file)
 
 
 @cli.command()
-@click.argument("file", type=click.File(mode="r", encoding="utf-8", lazy=True))
+@click.argument(
+    "file",
+    type=click.File(mode="r", encoding="utf-8", lazy=True),
+)
 def set_acl(file):
     """Read and set direcotry structure and ACLs from a YAML file."""
     config_str = file.read()
     acls_config = config_from_yaml(config_str)
 
     for container in acls_config["containers"]:
         tree_root = container_config_to_tree(container)
         Orchestrator(tree_root, acls_config["account"]).process_tree()
 
 
+@cli.command()
+@click.argument("account_name", type=str)
+@click.argument(
+    "outfile",
+    type=click.File("w", encoding="utf-8", lazy=True),
+)
+@click.option(
+    "--omit-special",
+    "omit_special",
+    is_flag=True,
+    help="Omit special ACLs when reading the account.",
+)
+def get_acl(account_name, outfile, omit_special):
+    """Read the current fs and acls on dirs."""
+    data = Orchestrator(None, account_name).read_account(omit_special=omit_special)
+    yaml.dump(data, outfile, sort_keys=False, indent=2)
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `adls_acl-0.0.4/src/adls_acl/input_parser.py` & `adls_acl-0.0.5/src/adls_acl/input_parser.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.4/src/adls_acl/logger.py` & `adls_acl-0.0.5/src/adls_acl/logger.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.4/src/adls_acl/nodes.py` & `adls_acl-0.0.5/src/adls_acl/nodes.py`

 * *Files 22% similar despite different names*

```diff
@@ -66,40 +66,80 @@
         """Check if it is ACL for other"""
         return True if (self.p_type == "other") else False
 
     def is_default(self):
         """Check if ACL is default"""
         return True if (self.scope == "default") else False
 
+    def is_special(self):
+        """check if any of: mask, other, owner, owner_group"""
+        return (
+            True
+            if any(
+                [
+                    self.is_owner(),
+                    self.is_owner_group(),
+                    self.is_mask(),
+                    self.is_other(),
+                ]
+            )
+            else False
+        )
+
+    def to_yaml(self):
+        """Returns a dict reprentaion"""
+        data = {
+            "oid": self.oid,
+            "type": self.p_type,
+            "acl": self.permissions,
+        }
+        if self.scope is not None:
+            data["scope"] = self.scope
+
+        return data
+
 
 class Node:
     def __init__(self, name: str, parent=None):
         self.name = name
         self.children = []
         self.parent = parent
         self.acls = set()
 
     def __str__(self):
         """Print node nicely"""
         s = f"Path to node: {self.path}"
+
         s += f"\nAcls from input:"
         for acl in self.acls:
             s += f"\n\t{str(acl)}"
 
         return s
 
     @property
-    def path(self):
+    def path_in_file_system(self):
         """Get the path from root of the container to the Node"""
-        if self.parent is not None and not isinstance(self.parent, RootNode):
+        if self.parent is not None and self.parent.parent is not None:
+            return f"{self.parent.path_in_file_system}/{self.name}"
+        else:
+            return self.name
+
+    @property
+    def path(self):
+        """Get the path from root (including the root name)"""
+        if self.parent is not None:
             return f"{self.parent.path}/{self.name}"
         else:
             return f"{self.name}"
 
     @property
+    def is_root(self):
+        return True if self.parent == None else False
+
+    @property
     def parent(self):
         return self._parent
 
     @parent.setter
     def parent(self, value: Self):
         """Sets a parent node. Also registers the child @parent"""
         if value is not None:
@@ -121,44 +161,79 @@
         if not isinstance(acl, Acl):
             raise TypeError(f"Acl must be of type, {type(Acl)}")
         self.acls.update((acl,))
 
     def add_child(self, child: Acl):
         self.children.append(child)
 
+    def to_yaml(self):
+        """Returns a dict reprentaion"""
+        data = {"name": self.name, "acls": [acl.to_yaml() for acl in self.acls]}
+        if len(self.children) > 0:
+            data["folders"] = [child.to_yaml() for child in self.children]
 
-class RootNode(Node):
-    def __init__(self, name: str, parent=None):
-        super().__init__(name, parent)
+        return data
 
 
 def _add_folder_nodes(parent_node: Node, folder: Dict):
     node = Node(folder["name"], parent=parent_node)
     for acl in folder["acls"]:
         node.add_acl(Acl.from_dict(acl))
 
     if "folders" in folder:
         for subfolder in folder["folders"]:
-            _add_folder_nodes(node, subfolder)
+            _ = _add_folder_nodes(node, subfolder)
 
+    return node  # The root node will be returend to the original caller
 
-def container_config_to_tree(container_config) -> RootNode:
-    """Returns a Tree from JSON configuration"""
-    root_node = RootNode(container_config["name"])
-    for acl in container_config["acls"]:
-        root_node.add_acl(Acl.from_dict(acl))
 
-    for folder in container_config["folders"]:
-        _add_folder_nodes(root_node, folder)
+def find_node_by_name(root_node, full_name: str) -> Node:
+    """Return the node by its name (path in the filesystem: from container node)"""
+    """ Should i just have a Tree class instead with index by name for nodes?"""
+    # Names are path from contianer root: dir1/dir2/dir3
 
-    return root_node
+    path_arr = full_name.split("/")
+    # if the name of the node is only 1-level and the search is on the root level
+    # return root node immediatley
+    if path_arr[0] == "" and root_node.is_root:
+        return root_node
 
+    current_dir = path_arr[0]
+    path_reminder = ("/").join(path_arr[1:])
+    node = None
 
-def bfs(root: RootNode):
+    for child_node in root_node.children:
+        if child_node.name == current_dir:
+            node = child_node
+            break
+
+    if len(path_reminder) > 0 and node is not None:
+        node = find_node_by_name(node, full_name=path_reminder)
+
+    return node
+
+
+def container_config_to_tree(container_config) -> Node:
+    """Returns a Tree from JSON configuration"""
+    return _add_folder_nodes(None, container_config)
+
+
+def bfs(root: Node):
     """Breadth-first traversal of the tree"""
     queue = [root]
 
     while queue:
-        node = queue.pop()
+        node = queue.pop(0)
         for child_node in node.children:
             queue.append(child_node)
         yield node
+
+
+def dfs(root: Node):
+    """Depth-frist traversal of the tree"""
+    stack = [root]
+
+    while stack:
+        node = stack.pop()
+        for child_node in node.children:
+            stack.append(child_node)
+        yield node
```

### Comparing `adls_acl-0.0.4/src/adls_acl/orchestrator.py` & `adls_acl-0.0.5/src/adls_acl/orchestrator.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,32 +2,68 @@
 from azure.storage.filedatalake import (
     DataLakeServiceClient,
     DataLakeDirectoryClient,
 )
 from azure.identity import DefaultAzureCredential, AzureCliCredential
 from azure.core.exceptions import ResourceExistsError
 from abc import ABC, abstractmethod
-from typing import Set
+from typing import Set, Dict
 
-from .nodes import RootNode, Node, bfs, Acl
+from .nodes import Node, bfs, Acl, find_node_by_name
 
 log = logging.getLogger(__name__)
 
 
 class Orchestrator:
-    def __init__(self, root: RootNode, account_name: str):
+    def __init__(self, root: Node, account_name: str):
         self.root = root
         self.sc = _get_service_client_token_credential(account_name)
+        self.account_name = account_name
 
     def process_tree(self):
         for node in bfs(self.root):
             processor = processor_selector(node)
             dc = processor.get_dir_client(node, self.sc)
             processor.set_acls(node, dc)
 
+    def read_account(self, omit_special: bool = False) -> Dict:
+        data = {}
+        data["account"] = self.account_name
+        data["containers"] = []
+        for container in self.sc.list_file_systems():
+            fc = self.sc.get_file_system_client(container)
+            dc = fc._get_root_directory_client()
+
+            root_node = Node(name=fc.file_system_name)
+
+            for acl in dc.get_access_control()["acl"].split(","):
+                acl = Acl.from_str(acl)
+                if omit_special and acl.is_special():
+                    pass
+                else:
+                    root_node.add_acl(acl)
+
+            path_list = fc.get_paths(recursive=True)
+            for path in filter(lambda x: x.is_directory == True, path_list):
+                dc = fc.get_directory_client(path.name)
+                parent_name = ("/").join(path.name.split("/")[:-1])
+                parent_node = find_node_by_name(root_node, parent_name)
+                node_name = path.name.split("/")[-1]
+                node = Node(name=node_name, parent=parent_node)
+                for acl in dc.get_access_control()["acl"].split(","):
+                    acl = Acl.from_str(acl)
+                    if omit_special and acl.is_special():
+                        pass
+                    else:
+                        node.add_acl(acl)
+
+            data["containers"].append(root_node.to_yaml())
+
+            return data
+
 
 class ClientWithACLSupport(ABC):
     @abstractmethod
     def get_access_control(): ...
 
     @abstractmethod
     def set_access_control(): ...
@@ -99,28 +135,28 @@
     def update_acls(): ...
 
 
 class ProcessorRoot(Processor):
     def __init__(self):
         pass
 
-    def get_dir_client(self, node: RootNode, client: DataLakeServiceClient):
+    def get_dir_client(self, node: Node, client: DataLakeServiceClient):
         """Creates a container if it doesn't exist and returns a file clietn
         to its root directory."""
         log.info("PROCESSING NODE ===========")
         log.info(node)
-        if not isinstance(node, RootNode):
-            raise TypeError(f"Node of type RootNode was expected")
+        if node.is_root == False:
+            raise ValueError(f"Node is not the root!")
 
         try:
-            file_client = client.create_file_system(node.name)
+            fs_client = client.create_file_system(node.name)
         except ResourceExistsError:
-            file_client = client.get_file_system_client(file_system=node.name)
+            fs_client = client.get_file_system_client(file_system=node.name)
 
-        return file_client._get_root_directory_client()
+        return fs_client._get_root_directory_client()
 
     def set_acls(self, node: Node, client: DataLakeDirectoryClient):
         super().set_acls(node, client)
         client.close()
 
     def update_acls():
         pass
@@ -133,24 +169,24 @@
     def get_dir_client(self, node: Node, client: DataLakeServiceClient):
         """Creates a directory, if it doesn't exist and returns a directory
         client."""
         log.info("PROCESSING NODE ===========")
         log.info(node)
 
         folder_client = client.get_file_system_client(file_system=node.get_root().name)
-        dir_client = folder_client.get_directory_client(node.path)
+        dir_client = folder_client.get_directory_client(node.path_in_file_system)
         dir_client.create_directory()
 
         return dir_client
 
     def set_acls(self, node: Node, client: DataLakeDirectoryClient):
         super().set_acls(node, client)
 
     def update_acls():
         pass
 
 
 def processor_selector(node):
-    if isinstance(node, RootNode):
+    if node.is_root:
         return ProcessorRoot()
-    elif isinstance(node, Node):
+    else:
         return ProcessorDir()
```

### Comparing `adls_acl-0.0.4/src/adls_acl.egg-info/PKG-INFO` & `adls_acl-0.0.5/src/adls_acl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adls_acl
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).
 Home-page: https://github.com/karolusz/adls-acl
 Author: Karol Luszczek
 Author-email: karol.luszczek@reinsight.se
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -67,14 +67,15 @@
 Options:
   --debug          Enable debug messages.
   --silent         Suppress logs to stdout.
   --log-file TEXT  Redirect logs to a file.
   --help           Show this message and exit.
 
 Commands:
+  get-acl  Read the current fs and acls on dirs.
   set-acl  Read and set direcotry structure and ACLs from a YAML file.
 ```
 
 #### `set-acl` command
 ```
 Usage: adls-acl set-acl [OPTIONS] FILE
 
@@ -84,24 +85,44 @@
   --help  Show this message and exit.
 ```
 
 To set acls from an input file `test.yml` the shell command would look like:
 ```bash
 adls-acl set-acl test.yml
 ```
+
+#### `get-acl` command
+```
+Usage: adls-acl get-acl [OPTIONS] ACCOUNT_NAME OUTFILE
+
+  Read the current fs and acls on dirs.
+
+Options:
+  --omit-special        Omit special ACLs when reading the account.
+  --help                Show this message and exit.
+```
+
+This will print the current filesystem of an account (directories only, no files) and their ACLs to a file on a path pass as `OUTFILE` argument.
+[Special ACLs](#special-acls) can be omitted with a flag `--omit-special`
+
+To read ACLs of a ADLS storage account named `testaccount` to file `dump.yml`:
+```bash
+adls-acl get-acl testaccount dump.yml
+```
+
 ### Input file
 
 The YAML schema reference for the input files. Each input file represents a desired directory structure and ACLs for a single Azure Storage account. 
 
 ##### Input File Example
 Example of an input file for a fictitious storage account. All elements of the schema are explained in the following sections.
 
 ```yaml
 account: testaccount
-containers: 
+containers:
   - name: testcontainer1 
     acls:
       - oid: "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
         type: "user"
         acl: r-x
       - oid: "yyyyyyyy-yyyy-yyyy-yyyy-yyyyyyyyyyyy"
         type: "user"
```

### Comparing `adls_acl-0.0.4/tests/test_nodes.py` & `adls_acl-0.0.5/tests/test_nodes.py`

 * *Files 22% similar despite different names*

```diff
@@ -53,24 +53,47 @@
     """Counts the elements in a generator"""
     return sum(1 for _ in iter)
 
 
 def test_container_config_to_tree(container_dict):
     root = _dict_to_tree(container_dict)
 
-    assert isinstance(root, nodes.RootNode)
     assert len(root.children) == 1
     assert root.name == "test_container"
     assert all([isinstance(x, nodes.Acl) for x in root.children[0].acls])
 
 
-def test_bfs(container_dict):
-    root = _dict_to_tree(container_dict)
-    count = _counter(nodes.bfs(root))
-    assert count == 3
+class TestTraversal:
+    @pytest.fixture(scope="class")
+    def tree(self):
+        root = nodes.Node("root")
+        sub_node1 = nodes.Node("subn1", root)
+        sub_node2 = nodes.Node("subn2", root)
+        _ = nodes.Node("subn3", sub_node1)
+        _ = nodes.Node("subn4", sub_node2)
+
+        return root
+
+    def test_bfs(self, tree):
+        assert [x.name for x in nodes.bfs(tree)] == [
+            "root",
+            "subn1",
+            "subn2",
+            "subn3",
+            "subn4",
+        ]
+
+    def test_dfs(self, tree):
+        assert [x.name for x in nodes.dfs(tree)] == [
+            "root",
+            "subn2",
+            "subn4",
+            "subn1",
+            "subn3",
+        ]
 
 
 class TestNode:
     @pytest.fixture(scope="class")
     def rootnode(self, container_dict):
         """Get the rootnode of the test tree"""
         return _dict_to_tree(container_dict)
@@ -83,17 +106,22 @@
             node = node.children[0]
 
         return node
 
     def test_path_on_root_node(self, rootnode):
         assert rootnode.path == "test_container"
 
+    def test_path_in_fs_on_root_node(self, rootnode):
+        assert rootnode.path_in_file_system == "test_container"
+
     def test_path_on_leaf_node(self, leafnode):
-        print(leafnode.path)
-        assert leafnode.path == "test_folder/test_subfolder_one"
+        assert leafnode.path == "test_container/test_folder/test_subfolder_one"
+
+    def test_path_in_fs_on_leaf_node(self, leafnode):
+        assert leafnode.path_in_file_system == "test_folder/test_subfolder_one"
 
     def test_get_root(self, rootnode, leafnode):
         assert leafnode.get_root() == rootnode
 
     def test_add_child(self, leafnode):
         parent = copy.deepcopy(leafnode)
         child = copy.deepcopy(leafnode)
@@ -196,22 +224,26 @@
 
         assert acl.is_default()
 
     def test_is_owner(self, acl_str_owner):
         acl = nodes.Acl.from_str(acl_str_owner)
 
         assert acl.is_owner()
+        assert acl.is_special()
 
     def test_is_owner_group(self, acl_str_owner_group):
         acl = nodes.Acl.from_str(acl_str_owner_group)
 
         assert acl.is_owner_group()
+        assert acl.is_special()
 
     def test_is_mask(self, acl_str_mask):
         acl = nodes.Acl.from_str(acl_str_mask)
 
         assert acl.is_mask()
+        assert acl.is_special()
 
     def test_is_other(self, acl_str_other):
         acl = nodes.Acl.from_str(acl_str_other)
 
         assert acl.is_other()
+        assert acl.is_special()
```

### Comparing `adls_acl-0.0.4/tests/test_orchestrator.py` & `adls_acl-0.0.5/tests/test_orchestrator.py`

 * *Files identical despite different names*


# Comparing `tmp/pve_cli-0.4.1.tar.gz` & `tmp/pve_cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pve_cli-0.4.1.tar", max compression
+gzip compressed data, was "pve_cli-0.5.0.tar", last modified: Sun Apr 14 20:43:10 2024, max compression
```

## Comparing `pve_cli-0.4.1.tar` & `pve_cli-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0    16725 2023-12-25 02:44:02.622926 pve_cli-0.4.1/LICENSE
--rw-r--r--   0        0        0      594 2023-12-25 02:44:02.626926 pve_cli-0.4.1/README.md
--rw-r--r--   0        0        0      198 2023-12-25 02:44:02.626926 pve_cli-0.4.1/pve_cli/__init__.py
--rw-r--r--   0        0        0     3727 2024-02-05 19:02:35.494526 pve_cli-0.4.1/pve_cli/guest_cmd.py
--rw-r--r--   0        0        0     1880 2024-01-21 23:14:01.996698 pve_cli-0.4.1/pve_cli/main.py
--rw-r--r--   0        0        0     5646 2023-12-25 02:44:02.634926 pve_cli-0.4.1/pve_cli/nodes_cmd.py
--rw-r--r--   0        0        0      233 2023-12-25 02:44:02.634926 pve_cli-0.4.1/pve_cli/proxmox/__init__.py
--rw-r--r--   0        0        0     3849 2024-02-22 15:55:23.646926 pve_cli-0.4.1/pve_cli/proxmox/api.py
--rw-r--r--   0        0        0      449 2023-12-25 02:44:02.638926 pve_cli-0.4.1/pve_cli/proxmox/exceptions.py
--rw-r--r--   0        0        0       96 2023-12-25 02:44:02.638926 pve_cli-0.4.1/pve_cli/proxmox/types.py
--rw-r--r--   0        0        0        0 2024-02-26 02:54:23.682469 pve_cli-0.4.1/pve_cli/util/__init__.py
--rw-r--r--   0        0        0      910 2024-01-21 23:14:01.996698 pve_cli-0.4.1/pve_cli/util/callbacks.py
--rw-r--r--   0        0        0      129 2023-12-25 02:44:02.638926 pve_cli-0.4.1/pve_cli/util/exceptions.py
--rw-r--r--   0        0        0     1574 2023-12-26 03:06:30.801607 pve_cli-0.4.1/pve_cli/util/validators.py
--rw-r--r--   0        0        0     1935 2024-02-26 02:09:37.038606 pve_cli-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 pve_cli-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-12-25 02:44:02.838927 pve_cli-0.5.0/LICENSE
+-rw-r--r--   0        0        0      757 2024-04-14 20:34:42.634837 pve_cli-0.5.0/README.md
+-rw-r--r--   0        0        0      198 2023-12-25 02:44:02.838927 pve_cli-0.5.0/pve_cli/__init__.py
+-rw-r--r--   0        0        0     3727 2024-02-05 19:02:35.874529 pve_cli-0.5.0/pve_cli/guest_cmd.py
+-rw-r--r--   0        0        0     1880 2024-01-21 23:14:01.404696 pve_cli-0.5.0/pve_cli/main.py
+-rw-r--r--   0        0        0     6808 2024-04-14 20:34:42.638837 pve_cli-0.5.0/pve_cli/nodes_cmd.py
+-rw-r--r--   0        0        0      233 2023-12-25 02:44:02.842927 pve_cli-0.5.0/pve_cli/proxmox/__init__.py
+-rw-r--r--   0        0        0     3849 2024-02-22 15:55:23.490925 pve_cli-0.5.0/pve_cli/proxmox/api.py
+-rw-r--r--   0        0        0      449 2023-12-25 02:44:02.842927 pve_cli-0.5.0/pve_cli/proxmox/exceptions.py
+-rw-r--r--   0        0        0       96 2023-12-25 02:44:02.842927 pve_cli-0.5.0/pve_cli/proxmox/types.py
+-rw-r--r--   0        0        0        0 2024-04-14 20:42:52.680254 pve_cli-0.5.0/pve_cli/util/__init__.py
+-rw-r--r--   0        0        0      910 2024-01-21 23:14:01.408696 pve_cli-0.5.0/pve_cli/util/callbacks.py
+-rw-r--r--   0        0        0      129 2023-12-25 02:44:02.846927 pve_cli-0.5.0/pve_cli/util/exceptions.py
+-rw-r--r--   0        0        0     1574 2023-12-26 03:06:31.021608 pve_cli-0.5.0/pve_cli/util/validators.py
+-rw-r--r--   0        0        0     2298 2024-04-14 20:43:10.176358 pve_cli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 20:42:52.684254 pve_cli-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     1159 2023-12-26 03:06:31.021608 pve_cli-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      974 2023-12-26 03:06:31.025608 pve_cli-0.5.0/tests/test_main.py
+-rw-r--r--   0        0        0     2505 2023-12-25 02:44:02.850927 pve_cli-0.5.0/tests/test_validators.py
+-rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 pve_cli-0.5.0/PKG-INFO
```

### Comparing `pve_cli-0.4.1/LICENSE` & `pve_cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.1/README.md` & `pve_cli-0.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,8 +11,15 @@
 * Linux (Unix): `~/.config/pve-cli/config.toml`
 * MacOS: `~/Library/Application Support/pve-cli/config.toml`
 * Windows: `C:\Users\<user>\AppData\Local\pve-cli\config.toml`
 
 This leverages the [`get_app_dir`](https://click.palletsprojects.com/en/8.1.x/api/#click.get_app_dir) method
 from [`click`](https://click.palletsprojects.com).
 
+## Required PVE Permissions
 
+For full functionallity following permissions are required:
+* `Sys.Audit`
+* `Sys.PowerMgmt`
+* `VM.Audit`
+* `VM.Migrate`
+* `VM.Monitor`
```

### Comparing `pve_cli-0.4.1/pve_cli/guest_cmd.py` & `pve_cli-0.5.0/pve_cli/guest_cmd.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.1/pve_cli/main.py` & `pve_cli-0.5.0/pve_cli/main.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.1/pve_cli/nodes_cmd.py` & `pve_cli-0.5.0/pve_cli/nodes_cmd.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,102 +10,104 @@
 from rich.progress import Progress, SpinnerColumn, TextColumn, TimeElapsedColumn
 from rich.table import Column, Table
 
 from .proxmox import Proxmox
 
 nodes_cli = typer.Typer()
 
-spinner_col = SpinnerColumn(style='bold white', finished_text='[blue bold]⠿')
+spinner_col = SpinnerColumn(style='bold white')
 text_col = TextColumn('[progress.description]{task.description}')
 
 
 @nodes_cli.callback()
 def nodes_callback(
-        ctx: typer.Context
+    ctx: typer.Context,
+    parallel: Annotated[int, typer.Option('--parallel', '-p', show_default=True)] = 4,
 ):
     proxmox_api = ctx.obj['proxmox_api']
     nodes = proxmox_api.list_nodes()
     ctx.obj['nodes'] = nodes
+    ctx.obj['parallel_migrations'] = parallel
 
 
 @nodes_cli.command('dump-vm-mapping')
 def dump_vms(
-        ctx: typer.Context,
-        outfile: Annotated[typer.FileTextWrite, typer.Argument(help='JSON output filepath')],
+    ctx: typer.Context,
+    outfile: Annotated[typer.FileTextWrite, typer.Argument(help='JSON output filepath')],
 ):
     proxmox_api = ctx.obj['proxmox_api']
     vms = proxmox_api.list_vms()
 
     result = {vm['vmid']: vm['node'] for vm in vms}
     json.dump(result, outfile, indent=2)
 
 
 @nodes_cli.command('restore-vm-mapping')
 def restore_mapping(
-        ctx: typer.Context,
-        infile: Annotated[typer.FileText, typer.Argument(help='JSON input file (created with dump-vms')]
+    ctx: typer.Context,
+    infile: Annotated[typer.FileText, typer.Argument(help='JSON input file (created with dump-vms')]
 ):
     proxmox_api = ctx.obj['proxmox_api']
     vms = proxmox_api.list_vms()
     nodes = ctx.obj['nodes']
+    parallel_migrations = ctx.obj['parallel_migrations']
 
     mapping = json.load(infile)
 
     migration_vms = {node['node']: [] for node in nodes}  # type: dict[str, list[dict]]
     for vm in vms:
         try:
             wanted_node = mapping[str(vm['vmid'])]
         except KeyError:
             continue
 
         if wanted_node == vm['node']:
-            rprint(f'[green]✅ VM {vm["name"]} ({vm["vmid"]}) is on node {wanted_node}')
+            rprint(spinner_col.finished_text, f'[green]✅ VM {vm["name"]} ({vm["vmid"]}) is on node {wanted_node}')
         else:
             migration_vms[wanted_node].append(vm)
 
     for dest_node, vms_to_migrate in migration_vms.items():
         if vms_to_migrate:
-            migrate_vms(proxmox_api, dest_node, vms_to_migrate)
+            migrate_vms(proxmox_api, dest_node, vms_to_migrate, parallel_migrations)
 
 
 @nodes_cli.command('cluster-reboot')
 def reboot_cluster(
-        ctx: typer.Context
+    ctx: typer.Context
 ):
     proxmox_api = ctx.obj['proxmox_api']
     nodes = ctx.obj['nodes']
+    parallel_migrations = ctx.obj['parallel_migrations']
     vms = proxmox_api.list_vms()
 
     for i in range(len(nodes)):
         node = nodes[i]['node']
         tmp_node = nodes[i - 1]['node']
 
         node_running_vms = [vm for vm in vms if vm['status'] == 'running' and vm['node'] == node]
 
-        migrate_vms(proxmox_api, tmp_node, node_running_vms)
+        migrate_vms(proxmox_api, tmp_node, node_running_vms, parallel_migrations)
 
         with Progress(spinner_col, TimeElapsedColumn(), text_col) as progress:
-            task_id = progress.add_task(description=f'[white]Rebooting {node}...',
-                                        total=1)
+            task_id = progress.add_task(description=f'[white]Rebooting {node}...', total=1)
             proxmox_api.reboot_node(node)
             # wait for node to go offline
             while proxmox_api.get_node(node)['status'] == 'online':
-                time.sleep(5)
+                time.sleep(10)  # it is not necessary to check this to often, check node status every 10 seconds should be fine
             # wait for node to come online
             while proxmox_api.get_node(node)['status'] != 'online':
-                time.sleep(5)
-            progress.update(task_id, completed=1, refresh=True,
-                            description=f'[blue]Done: Rebooted {node}')
+                time.sleep(10)  # it is not necessary to check this to often, check node status every 10 seconds should be fine
+            progress.update(task_id, completed=1, refresh=True, description=f'[blue]Done: Rebooted {node}')
 
-        migrate_vms(proxmox_api, node, node_running_vms)
+        migrate_vms(proxmox_api, node, node_running_vms, parallel_migrations)
 
 
 @nodes_cli.command('list')
 def list_(
-        ctx: typer.Context
+    ctx: typer.Context
 ):
     cluster = ctx.obj['cluster']
     nodes = ctx.obj['nodes']
 
     table = Table(title=f'Nodes in cluster {cluster}')
     table.add_column('Node')
     table.add_column('Status', justify='center')
@@ -138,27 +140,41 @@
     percent = int(round(usage * 100, 0))
     field = Table.grid(Column(no_wrap=True, max_width=max_width - 5),
                        Column(no_wrap=True, min_width=5, justify='right'))
     field.add_row(Bar(size=1.0, begin=0.0, end=usage), f'{percent}%')
     return field
 
 
-def migrate_vms(api: Proxmox, dest_node: str, vm_list: list):
+def check_migration_status(running_tasks_list: list, running_tasks: dict, api: Proxmox, progress: Progress, dest_node: str):
+    for upid in running_tasks_list:
+        vm, source_node, task_id = running_tasks[upid]
+        status = api.get_task_status(source_node, upid)
+        if status['status'] == 'stopped':
+            progress.update(task_id, completed=1, refresh=True,
+                            description=f'[blue]✅ Migrated {vm["name"]} ({vm["vmid"]}) from {source_node} to {dest_node}')
+            running_tasks_list.remove(upid)
+
+
+def migrate_vms(api: Proxmox, dest_node: str, vm_list: list, parallel_migrations: int = 4):
     running_tasks = {}
+    running_tasks_list: list[str] = []
+    if parallel_migrations == 0:
+        parallel_migrations = len(vm_list)
+
     with Progress(spinner_col, text_col) as progress:
-        for vm in vm_list:
-            source_node, upid = api.migrate_vm(vm['vmid'], dest_node)
-            task_id = progress.add_task(
-                description=f'[white]🚚 Migrating {vm["name"]} ({vm["vmid"]}) from {source_node} to {dest_node}...',
-                total=1)
-            running_tasks[upid] = (vm, source_node, task_id)
+        while vm_list:
+            while len(running_tasks_list) < parallel_migrations and vm_list:
+                vm = vm_list.pop()
+                source_node, upid = api.migrate_vm(vm['vmid'], dest_node)
+                task_id = progress.add_task(
+                    description=f'[white]🚚 Migrating {vm["name"]} ({vm["vmid"]}) from {source_node} to {dest_node}...',
+                    total=1
+                )
+                running_tasks[upid] = (vm, source_node, task_id)
+                running_tasks_list.append(upid)
+
+            time.sleep(3)  # it is not necessary to check this to often, check migration status every 3 seconds should be fine
+            check_migration_status(running_tasks_list, running_tasks, api, progress, dest_node)
 
-        running_tasks_list = list(running_tasks)
         while running_tasks_list:
-            for upid in running_tasks_list:
-                vm, source_node, task_id = running_tasks[upid]
-                status = api.get_task_status(source_node, upid)
-                if status['status'] == 'stopped':
-                    progress.update(task_id, completed=1, refresh=True,
-                                    description=f'[blue]✅ Migrated {vm["name"]} ({vm["vmid"]}) '
-                                                f'from {source_node} to {dest_node}')
-                    running_tasks_list.remove(upid)
+            time.sleep(3)  # it is not necessary to check this to often, check migration status every 3 seconds should be fine
+            check_migration_status(running_tasks_list, running_tasks, api, progress, dest_node)
```

### Comparing `pve_cli-0.4.1/pve_cli/proxmox/api.py` & `pve_cli-0.5.0/pve_cli/proxmox/api.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.1/pve_cli/util/callbacks.py` & `pve_cli-0.5.0/pve_cli/util/callbacks.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.1/pve_cli/util/validators.py` & `pve_cli-0.5.0/pve_cli/util/validators.py`

 * *Files identical despite different names*


# Comparing `tmp/pyiaacsync-0.7.tar.gz` & `tmp/pyiaacsync-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiaacsync-0.7.tar", last modified: Mon Jul 31 12:30:46 2023, max compression
+gzip compressed data, was "pyiaacsync-0.8.tar", last modified: Sun Apr 14 00:15:19 2024, max compression
```

## Comparing `pyiaacsync-0.7.tar` & `pyiaacsync-0.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-07-31 12:30:46.000000 pyiaacsync-0.7/
--rw-r--r--   0 manasbellani   (501) wheel        (0)     6189 2023-07-31 12:30:46.000000 pyiaacsync-0.7/PKG-INFO
--rw-r--r--   0 manasbellani   (501) wheel        (0)     5062 2023-07-23 03:54:05.000000 pyiaacsync-0.7/README.md
-drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync/
--rw-r--r--   0 manasbellani   (501) wheel        (0)        0 2023-03-17 07:03:20.000000 pyiaacsync-0.7/pyiaacsync/__init__.py
--rw-r--r--   0 manasbellani   (501) wheel        (0)    16485 2023-07-31 12:17:17.000000 pyiaacsync-0.7/pyiaacsync/pyiaacsync.py
-drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync.egg-info/
--rw-r--r--   0 manasbellani   (501) wheel        (0)     6189 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync.egg-info/PKG-INFO
--rw-r--r--   0 manasbellani   (501) wheel        (0)      235 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync.egg-info/SOURCES.txt
--rw-r--r--   0 manasbellani   (501) wheel        (0)        1 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync.egg-info/dependency_links.txt
--rw-r--r--   0 manasbellani   (501) wheel        (0)        7 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync.egg-info/requires.txt
--rw-r--r--   0 manasbellani   (501) wheel        (0)       11 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync.egg-info/top_level.txt
--rw-r--r--   0 manasbellani   (501) wheel        (0)       38 2023-07-31 12:30:46.000000 pyiaacsync-0.7/setup.cfg
--rw-r--r--   0 manasbellani   (501) wheel        (0)      864 2023-07-31 12:20:26.000000 pyiaacsync-0.7/setup.py
+drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2024-04-14 00:15:19.895373 pyiaacsync-0.8/
+-rw-r--r--   0 manasbellani   (501) wheel        (0)     1070 2022-12-25 12:08:19.000000 pyiaacsync-0.8/LICENSE
+-rw-r--r--   0 manasbellani   (501) wheel        (0)     5745 2024-04-14 00:15:19.894595 pyiaacsync-0.8/PKG-INFO
+-rw-r--r--   0 manasbellani   (501) wheel        (0)     5502 2024-04-14 00:13:38.000000 pyiaacsync-0.8/README.md
+drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2024-04-14 00:15:19.887652 pyiaacsync-0.8/pyiaacsync/
+-rw-r--r--   0 manasbellani   (501) wheel        (0)        0 2023-03-17 07:03:20.000000 pyiaacsync-0.8/pyiaacsync/__init__.py
+-rw-r--r--   0 manasbellani   (501) wheel        (0)    18914 2024-04-14 00:02:09.000000 pyiaacsync-0.8/pyiaacsync/pyiaacsync.py
+drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2024-04-14 00:15:19.893820 pyiaacsync-0.8/pyiaacsync.egg-info/
+-rw-r--r--   0 manasbellani   (501) wheel        (0)     5745 2024-04-14 00:15:19.000000 pyiaacsync-0.8/pyiaacsync.egg-info/PKG-INFO
+-rw-r--r--   0 manasbellani   (501) wheel        (0)      243 2024-04-14 00:15:19.000000 pyiaacsync-0.8/pyiaacsync.egg-info/SOURCES.txt
+-rw-r--r--   0 manasbellani   (501) wheel        (0)        1 2024-04-14 00:15:19.000000 pyiaacsync-0.8/pyiaacsync.egg-info/dependency_links.txt
+-rw-r--r--   0 manasbellani   (501) wheel        (0)        7 2024-04-14 00:15:19.000000 pyiaacsync-0.8/pyiaacsync.egg-info/requires.txt
+-rw-r--r--   0 manasbellani   (501) wheel        (0)       11 2024-04-14 00:15:19.000000 pyiaacsync-0.8/pyiaacsync.egg-info/top_level.txt
+-rw-r--r--   0 manasbellani   (501) wheel        (0)       38 2024-04-14 00:15:19.895560 pyiaacsync-0.8/setup.cfg
+-rw-r--r--   0 manasbellani   (501) wheel        (0)      865 2024-04-14 00:07:56.000000 pyiaacsync-0.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyiaacsync-0.7/README.md` & `pyiaacsync-0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,18 @@
     random_args = {}
     ## uncomment line below to demonstrate how the random arguments can work
     #random_args = {'message': 'hello world'}
 ```
 
 *Note*: An additional example has been added in folder called `example-fileasset-with-update` where the `fileassetwupd.py` is a python file which additionally includes the `update` method in the `FileAssetWithUpdate` class. The commands listed below also apply to files in this folder.
 
+*Note*: By default, pyiaacsync will immediately stop syncing assets if there are unexpected errors. This can be over-ridden by setting `true` to `continue_sync_on_error` and specifying an error handler `callback_on_sync_error` which will execute the error handler and continue the processing of remaining assets after executing `callback_on_sync_error` method. An example of this is included in `example-fileasset-with-update`.
+
+*Assumption*: Note that all sync, delete, create, update actions are currently performed once only from pyiaacsync. Any retries must be built in the asset python file
+
 ### Actions
 
 #### init
 The first steps is to execute `init` which will create a new state file `out-teststate.yaml`:
 ```
 python3 example.py -a init
 ```
@@ -82,14 +86,15 @@
 ```
 python3 example.py -a validate_configs
 ```
 
 #### sync
 
 To sync the assets based on the spec/configs folder continuously - this will create the files as per the configs in the folder.
+
 Any changes made to the files the next time will be reset.
 ```
 python3 example.py -a sync
 ```
 
 To sync the assets once only:
 ```
@@ -101,10 +106,7 @@
 To delete all existing assets (in this case, all files) and remove the assets from the state file:
 ```
 python3 example.py -a delete_assets
 ```
 
 ## TODO
 - Add unit testing
-- Fix the comments for create asset
-- Fix the bug in deleteasset
-- Add an assumption: Assuming that the API works ok - every action performed once (no retry)
```

### Comparing `pyiaacsync-0.7/pyiaacsync/pyiaacsync.py` & `pyiaacsync-0.8/pyiaacsync/pyiaacsync.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 class IaacSync:
     """Class used for deploying and syncing IAAC assets defined in an IAAC Sync folder (`iaac_sync_folder`) (e.g. a folder managed via git 
     for version control) that contains various configs describing how to create assets using the `asset` functions
     """
     def __init__(self, iaac_sync_folder, state_file, asset, conf_file_extensions=CONFIG_FILE_EXTENSIONS, 
             init=False, init_force=False, init_state_file=None, delete_all_only=False, validate_configs_only=False,
-            delete_if_asset_not_updated=True, **args):
+            delete_if_asset_not_updated=True, continue_sync_on_error=False, callback_on_sync_error=None, **args):
         """Function to sync spec configs defined in IAAC Sync folder 
 
         Args:
             iaac_sync_folder (str): The IAAC Sync folder path which contains the spec for asset to create
             state_file (str): The path of the state which will be used for syncing the assets
             asset (object): A class that represents the asset to sync. The asset is an class which defines the validate, check, 
                 create, delete methods
@@ -53,21 +53,27 @@
             init (bool, optional): Initialize the state file only. Defaults to False.
             init_state_file (str, optional): An optional initial state file to use when performing initialize. Defaults to None.
             init_force (bool, optional): Force initialization even if init file exists. Defaults to False.
             delete_all_only (bool, optional): Delete all the assets that have been created and clean the state file. Defaults to `False`.
             validate_configs_only (bool, optional): Whether to only validate the configs (not execute any syncing). Defaults to False.
             delete_if_asset_not_updated (bool, optional): If True, then asset is not updated successful, then delete the asset to be 
                 re-created. Otherwise, create the asset again
+            continue_sync_on_error (bool): Whether or not to continue sync on error. If set to True, then `callback_on_sync_error` is called 
+                with error class and message as the argument
+            callback_on_sync_error (func): Function of format `def callback_on_sync_error(err_class, err_msg)` which has error class and 
+                error message as arguments
             args (dict): Any additional optional args which would get passed to the methods defined in the asset class
         """
         self.iaac_sync_folder = iaac_sync_folder
         self.state_file = state_file
         self.asset = asset
         self.conf_file_extensions = conf_file_extensions
         self.delete_if_asset_not_updated = delete_if_asset_not_updated
+        self.continue_sync_on_error = continue_sync_on_error
+        self.callback_on_sync_error = callback_on_sync_error
         self.state = {}
         if init:
             self.init_state(init_state_file, init_force)
         elif delete_all_only:
             self.__delete_assets(**args)
         elif validate_configs_only:
             self.__validate_configs(**args)
@@ -124,18 +130,27 @@
             args (dict): Any additional optional args which would get passed to the methods defined in the asset class
         """
         if self.read_state():
             try:
                 if self.state:
                     state_config_paths = list(self.state.keys())
                     for config_path in state_config_paths:
-                        asset_id = self.state[config_path].get('asset_id', None)
-                        if self.asset.delete(asset_id, **args):
-                            # Remove the asset tracking from the state since it is no longer being tracked in git
-                            del self.state[config_path]
+                        try:
+                            asset_id = self.state[config_path].get('asset_id', None)
+                            if self.asset.delete(asset_id, **args):
+                                # Remove the asset tracking from the state since it is no longer being tracked in git
+                                del self.state[config_path]
+                        except Exception as e:
+                            # Execute callback if set by the user, otherwise raise this error to next parent
+                            # exception
+                            if self.continue_sync_on_error:
+                                self.write_state()
+                                self.callback_on_sync_error(e.__class__, str(e))
+                            else:
+                                raise
             except Exception as e:
                 # Ensure that the current state is written back irrespective of exception that occurs
                 self.write_state()
                 # Re-raise the error
                 raise
                 
             self.write_state()
@@ -184,117 +199,136 @@
                 # Loop through each config fie in the IAAC Sync folder
                 for dir_path, _, files in os.walk(self.iaac_sync_folder):
 
                     for f in files:
                         
                         # Work only with the conf files
                         if any([f.endswith(ext) for ext in self.conf_file_extensions]):
-                            
-                            config_path = os.path.join(dir_path, f)
-
-                            # Keep track of ALL the asset config files
-                            all_config_files.append(config_path)
+                            try:
+                                config_path = os.path.join(dir_path, f)
 
-                            # Calculate the hash for config which will be checked to see if they have changed
-                            config_hash = self.__calculate_hash(config_path)
-                            state_conf = self.state.get(config_path, None)
-                            
-                            # Get the hash of existing assets. If it doesn't exist then 
-                            state_hash = ''
-                            asset_id = ''
-                            if state_conf:
-                                state_hash = state_conf['hash']
-                                asset_id = state_conf['asset_id']
-                            else:
-                                self.state[config_path] = {
-                                    'asset_id': '',
-                                    'hash': '',
-                                }
+                                # Keep track of ALL the asset config files
+                                all_config_files.append(config_path)
 
-                            # Read the config from file
-                            config = ''
-                            try:
-                                with open(config_path, "r") as f:
-                                    config = yaml.safe_load(f)
-                            except Exception as e:
-                                self.write_state()
-                                raise ConfigFileInvalidSyntax(f"Config file: {config_path} syntax invalid. Error: {e.__class__}, {e}")
+                                # Calculate the hash for config which will be checked to see if they have changed
+                                config_hash = self.__calculate_hash(config_path)
+                                state_conf = self.state.get(config_path, None)
+                                
+                                # Get the hash of existing assets. If it doesn't exist then 
+                                state_hash = ''
+                                asset_id = ''
+                                if state_conf:
+                                    state_hash = state_conf['hash']
+                                    asset_id = state_conf['asset_id']
+                                else:
+                                    self.state[config_path] = {
+                                        'asset_id': '',
+                                        'hash': '',
+                                    }
+
+                                # Read the config from file
+                                config = ''
+                                try:
+                                    with open(config_path, "r") as f:
+                                        config = yaml.safe_load(f)
+                                except Exception as e:
+                                    self.write_state()
+                                    raise ConfigFileInvalidSyntax(f"Config file: {config_path} syntax invalid. Error: {e.__class__}, {e}")
+
+                                # Validate whether the config is correctly provided before syncing
+                                if config:
+                                    if self.asset.validate(config, **args):
+                                        
+                                        # Checking if the asset that currently exists matches the config in 'git'
+                                        is_asset_in_sync = True
+                                        if asset_id:
+                                            is_asset_in_sync = self.asset.check(asset_id, config, **args)
 
-                            # Validate whether the config is correctly provided before syncing
-                            if config:
-                                if self.asset.validate(config, **args):
-                                    
-                                    # Checking if the asset that currently exists matches the config in 'git'
-                                    is_asset_in_sync = True
-                                    if asset_id:
-                                        is_asset_in_sync = self.asset.check(asset_id, config, **args)
+                                        # If the spec file has changed OR is brand new, then re-create the asset (delete, then create)
+                                        if (not state_hash) or (state_hash != config_hash) or not is_asset_in_sync:
 
-                                    # If the spec file has changed OR is brand new, then re-create the asset (delete, then create)
-                                    if (not state_hash) or (state_hash != config_hash) or not is_asset_in_sync:
+                                            # Recreate the asset by first attempting to delete it
+                                            if asset_id:
 
-                                        # Recreate the asset by first attempting to delete it
-                                        if asset_id:
+                                                # Check if there is an update function in the asset, if yes, then call it
+                                                if hasattr(self.asset, 'update') and callable(self.asset.update):
+                                                    if self.asset.update(asset_id, config, **args):
+                                                        # Call the update function, and ensure that the same asset ID is returned
+                                                        # if asset ID not returned then there was an error
+                                                        self.state[config_path]['hash'] = config_hash
+                                                        self.state[config_path]['asset_id'] = asset_id
+                                                    else:
+                                                        if self.delete_if_asset_not_updated:
+                                                            if self.asset.delete(asset_id, **args):
+                                                                # Asset ID deleted
+                                                                asset_id = ''
+                                                                if config_path in self.state:
+                                                                    # Update the state file that asset has been deleted
+                                                                    del self.state[config_path]
+                                                            else:
+                                                                raise AssetNotDeletedException(f"Asset with config in file {config_path} could not be deleted")
+                                                        else:
+                                                            raise AssetNotUpdatedException(f"Asset with config in file {config_path} could not be updated")
 
-                                            # Check if there is an update function in the asset, if yes, then call it
-                                            if hasattr(self.asset, 'update') and callable(self.asset.update):
-                                                if self.asset.update(asset_id, config, **args):
-                                                    # Call the update function, and ensure that the same asset ID is returned
-                                                    # if asset ID not returned then there was an error
-                                                    self.state[config_path]['hash'] = config_hash
-                                                    self.state[config_path]['asset_id'] = asset_id
                                                 else:
-                                                    if self.delete_if_asset_not_updated:
-                                                        if self.asset.delete(asset_id, **args):
-                                                            # Asset ID deleted
-                                                            asset_id = ''
-                                                            if config_path in self.state:
-                                                                # Update the state file that asset has been deleted
-                                                                del self.state[config_path]
-                                                        else:
-                                                            raise AssetNotDeletedException(f"Asset with config in file {config_path} could not be deleted")
+                                                    if self.asset.delete(asset_id, **args):
+                                                        # Asset ID deleted
+                                                        asset_id = ''
+                                                        if config_path in self.state:
+                                                            # Update the state file that asset has been deleted
+                                                            del self.state[config_path]
                                                     else:
-                                                        raise AssetNotUpdatedException(f"Asset with config in file {config_path} could not be updated")
+                                                        raise AssetNotDeletedException(f"Asset with config in file {config_path} could not be deleted")
+                                            
+                                            # Try to create the asset again now, if it is deleted
+                                            if not asset_id:
+                                                asset_id = self.asset.create(config, **args)
+                                                if asset_id:
+                                                    if config_path not in self.state:
+                                                        self.state[config_path] = {}
+                                                    # Update the state file with the hash and the new asset ID created
+                                                    self.state[config_path]['hash'] = config_hash
+                                                    self.state[config_path]['asset_id'] = asset_id
 
-                                            else:
-                                                if self.asset.delete(asset_id, **args):
-                                                    # Asset ID deleted
-                                                    asset_id = ''
-                                                    if config_path in self.state:
-                                                        # Update the state file that asset has been deleted
-                                                        del self.state[config_path]
-                                                else:
-                                                    raise AssetNotDeletedException(f"Asset with config in file {config_path} could not be deleted")
-                                        
-                                        # Try to create the asset again now, if it is deleted
-                                        if not asset_id:
-                                            asset_id = self.asset.create(config, **args)
-                                            if asset_id:
-                                                if config_path not in self.state:
-                                                    self.state[config_path] = {}
-                                                # Update the state file with the hash and the new asset ID created
-                                                self.state[config_path]['hash'] = config_hash
-                                                self.state[config_path]['asset_id'] = asset_id
+                                                if not asset_id:
+                                                    raise AssetNotCreatedException(f"Asset with config in file {config_path} could not be created")
+                            except Exception as e:
+                                # Execute callback if set by the user, otherwise raise this error to next parent
+                                # exception
+                                if self.continue_sync_on_error:
+                                    self.write_state()
+                                    self.callback_on_sync_error(e.__class__, str(e))
+                                else:
+                                    raise
 
-                                            if not asset_id:
-                                                raise AssetNotCreatedException(f"Asset with config in file {config_path} could not be created")
                 
                 # Delete any assets which are not in the config spec (git)
                 if self.state:
 
                     # Read all the config spec keys and loop through them
                     state_config_paths = list(self.state.keys())
                     for config_path in state_config_paths:
+                        try:
+                            # Check if any are not in the config specs
+                            if config_path not in all_config_files:
+                                
+                                asset_id = self.state[config_path].get('asset_id', None)
+                                if asset_id:
+                                    if self.asset.delete(asset_id, **args):
+                                        # Remove the asset tracking from the state since it is no longer being tracked in git
+                                        del self.state[config_path]
+                        except Exception as e:
+                            # Execute callback if set by the user, otherwise raise this error to next parent
+                            # exception
+                            if self.continue_sync_on_error:
+                                self.write_state()
+                                self.callback_on_sync_error(e.__class__, str(e))
+                            else:
+                                raise
 
-                        # Check if any are not in the config specs
-                        if config_path not in all_config_files:
-                            asset_id = self.state[config_path].get('asset_id', None)
-                            if asset_id:
-                                if self.asset.delete(asset_id, **args):
-                                    # Remove the asset tracking from the state since it is no longer being tracked in git
-                                    del self.state[config_path]
             except Exception as e:
                 self.write_state()
                 raise
 
             self.write_state()
 
         else:
```

### Comparing `pyiaacsync-0.7/setup.py` & `pyiaacsync-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Read the description from the markdown file
 with open('README.md', 'r') as f:
     description = f.read()
 
 setup(
     name="pyiaacsync",
-    version="0.7",
+    version="0.8",
     packages=find_packages(),
     install_requires=requirements,
     description=project_description,
     long_description=description,
     long_description_content_type="text/markdown",
     url=get_git_remote_url()
-)
+)
```


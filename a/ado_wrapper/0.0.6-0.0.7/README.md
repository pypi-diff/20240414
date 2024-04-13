# Comparing `tmp/ado_wrapper-0.0.6.tar.gz` & `tmp/ado_wrapper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-0.0.6.tar", max compression
+gzip compressed data, was "ado_wrapper-0.0.7.tar", max compression
```

## Comparing `ado_wrapper-0.0.6.tar` & `ado_wrapper-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.6/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-0.0.6/README.md
--rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.6/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6446 2024-04-08 17:57:20.745729 ado_wrapper-0.0.6/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2123 2024-04-10 11:16:39.930064 ado_wrapper-0.0.6/ado_wrapper/client.py
--rw-r--r--   0        0        0    25667 2024-04-11 13:43:04.075027 ado_wrapper-0.0.6/ado_wrapper/dumps.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.6/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-0.0.6/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.6/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-0.0.6/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1805 2024-04-09 15:28:42.531252 ado_wrapper-0.0.6/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0     1342 2024-04-10 19:18:54.311903 ado_wrapper-0.0.6/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0      659 2024-04-08 18:01:44.152197 ado_wrapper-0.0.6/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     4650 2024-04-09 09:35:29.826115 ado_wrapper-0.0.6/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    13517 2024-04-09 20:21:18.486611 ado_wrapper-0.0.6/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6637 2024-04-09 18:43:12.632598 ado_wrapper-0.0.6/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     3477 2024-04-09 18:30:16.745942 ado_wrapper-0.0.6/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-0.0.6/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    14800 2024-04-09 18:53:28.574098 ado_wrapper-0.0.6/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12781 2024-04-09 20:19:59.831154 ado_wrapper-0.0.6/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    15647 2024-04-12 10:04:22.381132 ado_wrapper-0.0.6/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     6014 2024-04-10 18:05:31.126571 ado_wrapper-0.0.6/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4622 2024-04-09 18:43:22.061540 ado_wrapper-0.0.6/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8370 2024-04-11 10:38:27.069961 ado_wrapper-0.0.6/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4934 2024-04-09 18:30:55.561929 ado_wrapper-0.0.6/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     8415 2024-04-10 18:17:52.653711 ado_wrapper-0.0.6/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8158 2024-04-10 17:53:40.392730 ado_wrapper-0.0.6/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4257 2024-04-08 17:51:22.897215 ado_wrapper-0.0.6/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2098 2024-04-12 10:04:57.932187 ado_wrapper-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.7/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-0.0.7/README.md
+-rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.7/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6504 2024-04-13 22:19:56.681692 ado_wrapper-0.0.7/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2123 2024-04-10 11:16:39.930064 ado_wrapper-0.0.7/ado_wrapper/client.py
+-rw-r--r--   0        0        0    25667 2024-04-11 13:43:04.075027 ado_wrapper-0.0.7/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.7/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-0.0.7/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.7/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-0.0.7/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-12 10:52:50.915024 ado_wrapper-0.0.7/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0     1342 2024-04-10 19:18:54.311903 ado_wrapper-0.0.7/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0      659 2024-04-08 18:01:44.152197 ado_wrapper-0.0.7/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     4650 2024-04-09 09:35:29.826115 ado_wrapper-0.0.7/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    13517 2024-04-09 20:21:18.486611 ado_wrapper-0.0.7/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6637 2024-04-09 18:43:12.632598 ado_wrapper-0.0.7/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     3477 2024-04-09 18:30:16.745942 ado_wrapper-0.0.7/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    13519 2024-04-13 22:29:12.944703 ado_wrapper-0.0.7/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-0.0.7/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    14800 2024-04-09 18:53:28.574098 ado_wrapper-0.0.7/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12781 2024-04-09 20:19:59.831154 ado_wrapper-0.0.7/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10304 2024-04-13 22:19:35.024746 ado_wrapper-0.0.7/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     6014 2024-04-10 18:05:31.126571 ado_wrapper-0.0.7/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4622 2024-04-09 18:43:22.061540 ado_wrapper-0.0.7/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8350 2024-04-13 18:18:13.167779 ado_wrapper-0.0.7/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4934 2024-04-09 18:30:55.561929 ado_wrapper-0.0.7/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     8499 2024-04-12 10:53:35.658831 ado_wrapper-0.0.7/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8158 2024-04-10 17:53:40.392730 ado_wrapper-0.0.7/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4257 2024-04-08 17:51:22.897215 ado_wrapper-0.0.7/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2191 2024-04-13 22:29:36.283420 ado_wrapper-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-0.0.7/PKG-INFO
```

### Comparing `ado_wrapper-0.0.6/LICENSE` & `ado_wrapper-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/README.md` & `ado_wrapper-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/__main__.py` & `ado_wrapper-0.0.7/ado_wrapper/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 
 from ado_wrapper.client import AdoClient
 from ado_wrapper.utils import get_internal_field_names, get_resource_variables, ResourceType
 
 
-def main() -> None:
+def main() -> None:  # pylint: disable=too-many-branches, too-many-statements
     ALL_RESOURCES = get_resource_variables()
 
     parser = argparse.ArgumentParser(
         prog="AdoWrapper", description="A tool to manage Azure DevOps resources and interface with the ADO API", usage=""
     )
 
     parser.add_argument("--ado-org", dest="ado_org", required=False)
```

### Comparing `ado_wrapper-0.0.6/ado_wrapper/client.py` & `ado_wrapper-0.0.7/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/dumps.py` & `ado_wrapper-0.0.7/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-0.0.7/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-0.0.7/ado_wrapper/plan_resources/plan_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,13 @@
         ado_client.state_manager.add_resource_to_state("Plan" + class_.__name__, extract_id(resource_object), resource_object.to_json())  # type: ignore[arg-type, union-attr]
         return plan_resource.create(ado_client, url, payload)  # type: ignore[return-value]
 
     @staticmethod
     def update(
         class_: "StateManagedResource", ado_client: "AdoClient", url: str, attribute_name: str, attribute_value: Any, params: dict[str, Any]
     ) -> None:
-        plan_resource = PlannedStateManagedResource.get_plan_resource(class_.__name__)  # type: ignore[attr-defined]
+        pass
+        # plan_resource = PlannedStateManagedResource.get_plan_resource(class_.__name__)  # type: ignore[attr-defined]
         # resource_object = plan_resource.get_by_id(ado_client, extract_id(url))
         # resource_object.update(ado_client, url, attribute_name, attribute_value, params)
 
         # ado_client.state_manager.add_resource_to_state("Plan" + class_.__name__, extract_id(resource_object), resource_object.to_json())
```

### Comparing `ado_wrapper-0.0.6/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-0.0.7/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/__init__.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/branches.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/builds.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/builds.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/commits.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/groups.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/projects.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/releases.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/repo.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/merge_policies.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,279 +1,206 @@
 from __future__ import annotations
 
-import io
-import zipfile
 from dataclasses import dataclass, field
+from datetime import datetime
 from typing import Any, Literal, TYPE_CHECKING
 
 import requests
 
 from ado_wrapper.state_managed_abc import StateManagedResource
-from ado_wrapper.resources.pull_requests import PullRequest, PullRequestStatus
-from ado_wrapper.resources.commits import Commit
-from ado_wrapper.utils import ResourceNotFound, UnknownError
+from ado_wrapper.resources.users import Reviewer
+from ado_wrapper.utils import from_ado_date_string
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
-RepoEditableAttribute = Literal["name", "default_branch", "is_disabled"]
 WhenChangesArePushed = Literal["require_revote_on_each_iteration", "require_revote_on_last_iteration", "reset_votes_on_source_push", "reset_rejections_on_source_push", "do_nothing"]
+name_mapping = {
+    "requireVoteOnEachIteration": "require_revote_on_each_iteration",
+    "requireVoteOnLastIteration": "require_revote_on_last_iteration",
+    "resetOnSourcePush": "reset_votes_on_source_push",
+    "resetRejectionsOnSourcePush": "reset_rejections_on_source_push",
+    "do_nothing": "do_nothing"
+}
 
-# ====================================================================
+def _get_type_id(ado_client: AdoClient, action_type: str) -> str:
+    """Used internally to get a specific update request ID"""
+    request = requests.get(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/policy/types?api-version=6.0", auth=ado_client.auth)
+    # print([(x["displayName"], x["id"]) for x in request.json()["value"]])
+    return [x for x in request.json()["value"] if x["displayName"] == action_type][0]["id"]  # type: ignore[no-any-return]
 
 
 @dataclass
-class Repo(StateManagedResource):
-    """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/repositories?view=azure-devops-rest-7.1"""
-
-    repo_id: str = field(metadata={"is_id_field": True})
-    name: str = field(metadata={"editable": True})
-    default_branch: str = field(default="main", repr=False, metadata={"editable": True, "internal_name": "defaultBranch"})
-    is_disabled: bool = field(default=False, repr=False, metadata={"editable": True, "internal_name": "isDisabled"})
-    # WARNING, disabling a repo means it's not able to be deleted, proceed with caution.
-
-    def __str__(self) -> str:
-        return f"Repo(name={self.name}, id={self.repo_id})"
-
-    @classmethod
-    def from_request_payload(cls, data: dict[str, str]) -> "Repo":
-        return cls(
-            data["id"], data["name"], data.get("defaultBranch", "main").removeprefix("refs/heads/"), bool(data.get("isDisabled", False))
-        )
-
-    @classmethod
-    def get_by_id(cls, ado_client: AdoClient, repo_id: str) -> "Repo":
-        return super().get_by_url(
-            ado_client,
-            f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}?api-version=7.1",
-        )  # type: ignore[return-value]
-
-    @classmethod
-    def create(cls, ado_client: AdoClient, name: str, include_readme: bool = True) -> "Repo":  # type: ignore[override]
-        repo: Repo = super().create(
-            ado_client,
-            f"/{ado_client.ado_project}/_apis/git/repositories?api-version=7.1",
-            {"name": name},
-        )  # type: ignore[assignment]
-        if include_readme:
-            Commit.add_initial_readme(ado_client, repo.repo_id)
-        return repo
-
-    def update(self, ado_client: AdoClient, attribute_name: RepoEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
-        return super().update(
-            ado_client, "patch",
-            f"/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}?api-version=7.1",
-            attribute_name, attribute_value, {},  # fmt: skip
-        )
-
-    @classmethod
-    def delete_by_id(cls, ado_client: AdoClient, repo_id: str) -> None:  # type: ignore[override]
-        # TODO: This never checks if it's disabled, so might error
-        for pull_request in Repo.get_all_pull_requests(ado_client, repo_id, "all"):
-            ado_client.state_manager.remove_resource_from_state("PullRequest", pull_request.pull_request_id)
-        return super().delete_by_id(
-            ado_client,
-            f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}?api-version=7.1",
-            repo_id,
-        )
-
-    @classmethod
-    def get_all(cls, ado_client: AdoClient) -> list["Repo"]:  # type: ignore[override]
-        return super().get_all(
-            ado_client,
-            f"/{ado_client.ado_project}/_apis/git/repositories?api-version=7.1",
-        )  # type: ignore[return-value]
-
-    # ============ End of requirement set by all state managed resources ================== #
-    # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
-    # =============== Start of additional methods included with class ===================== #
+class MergePolicyDefaultReviewer(StateManagedResource):
+    policy_id: str = field(metadata={"is_id_field": True})
+    required_reviewer_id: list[str]
+    is_required: bool
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, repo_name: str) -> "Repo | None":  # type: ignore[return]
-        """Warning, this function must fetch `all` repos to work, be cautious when calling it in a loop."""
-        for repo in cls.get_all(ado_client):
-            if repo.name == repo_name:
-                return repo
-
-    def get_file(self, ado_client: AdoClient, file_path: str, branch_name: str = "main") -> str:
-        request = requests.get(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?path={file_path}&versionType={'Branch'}&version={branch_name}&api-version=7.1",
-            auth=ado_client.auth,
-        )
-        if request.status_code == 404:
-            raise ResourceNotFound(f"File {file_path} not found in repo {self.repo_id}")
-        if request.status_code != 200:
-            raise UnknownError(f"Error getting file {file_path} from repo {self.repo_id}: {request.text}")
-        return request.text  # This is the file content
-
-    def get_contents(self, ado_client: AdoClient, file_types: list[str] | None = None, branch_name: str = "main") -> dict[str, str]:
-        """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/items/get?view=azure-devops-rest-7.1&tabs=HTTP
-        This function downloads the contents of a repo, and returns a dictionary of the files and their contents
-        The file_types parameter is a list of file types to filter for, e.g. ["json", "yaml"]"""
-        try:
-            request = requests.get(
-                f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?recursionLevel={'Full'}&download={True}&$format={'Zip'}&versionDescriptor.version={branch_name}&api-version=7.1",
-                auth=ado_client.auth,
-            )
-        except requests.exceptions.ConnectionError:
-            print(f"=== Connection error, failed to download {self.repo_id}")
-            return {}
-        if request.status_code != 200:
-            print(f"Error getting repo contents for {self.name} ({self.repo_id}):", request.text)
-            return {}
-        # ============ We do this because ADO ===================
-        bytes_io = io.BytesIO()
-        for chunk in request.iter_content(chunk_size=128):
-            bytes_io.write(chunk)
-
-        files = {}
-        try:
-            with zipfile.ZipFile(bytes_io) as zip_ref:
-                # For each file, read the bytes and convert to string
-                for file_name in [x for x in zip_ref.namelist() if file_types is None or x.split(".")[-1] in file_types]:
-                    try:
-                        files[file_name] = zip_ref.read(file_name).decode()  # fmt: skip
-                    except UnicodeDecodeError:
-                        print(f"Error decoding file: {file_name} in {self.name}")
-        except zipfile.BadZipFile as e:
-            print(f"{self.name} ({self.repo_id}) couldn't be unzipped:", e)
-
-        bytes_io.close()
-        # =========== That's all I have to say ==================
-        return files
-
-    def create_pull_request(self, ado_client: AdoClient, branch_name: str, pull_request_title: str, pull_request_description: str) -> "PullRequest":  # fmt: skip
-        """Helper function which redirects to the PullRequest class to make a PR"""
-        return PullRequest.create(ado_client, self.repo_id, branch_name, pull_request_title, pull_request_description)
+    def from_request_payload(cls, data: dict[str, Any]) -> StateManagedResource:
+        return cls(data["id"], data["settings"]["requiredReviewerIds"][0], data["isBlocking"])
 
     @staticmethod
-    def get_all_pull_requests(ado_client: AdoClient, repo_id: str, status: PullRequestStatus = "all") -> list["PullRequest"]:
-        return PullRequest.get_all_by_repo_id(ado_client, repo_id, status)
-
-    def delete(self, ado_client: AdoClient) -> None:
-        if self.is_disabled:
-            self.update(ado_client, "is_disabled", False)
-        self.delete_by_id(ado_client, self.repo_id)
-
-    @staticmethod
-    def get_content_static(
-        ado_client: AdoClient, repo_id: str, file_types: list[str] | None = None, branch_name: str = "main"
-    ) -> dict[str, str]:
-        repo = Repo.get_by_id(ado_client, repo_id)
-        return repo.get_contents(ado_client, file_types, branch_name)
-
-    @staticmethod
-    def get_branch_policy(ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> "RepoBranchPolicies | None":
-        return RepoBranchPolicies.get_by_repo_id(ado_client, repo_id, branch_name)
+    def get_default_reviewers(ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list[Reviewer]:
+        payload = {"contributionIds": ["ms.vss-code-web.branch-policies-data-provider"],
+                   "dataProviderContext": {"properties": {"projectId": ado_client.ado_project_id, "repositoryId": repo_id, "refName": f"refs/heads/{branch_name}"}}}
+        request = requests.post("https://dev.azure.com/VFCloudEngineering/_apis/Contribution/HierarchyQuery?api-version=7.1-preview.1",
+                               json=payload, auth=ado_client.auth).json()
+        if request is None:
+            return []
+        all_reviewers = [Reviewer(x["displayName"], x["uniqueName"], x["id"], 0, False) for x in request["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["identities"]]
+        for policy_group in request["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["policyGroups"].values():
+            if policy_group["currentScopePolicies"] is None:
+                continue
+            is_required = policy_group["currentScopePolicies"][0]["isBlocking"]
+            if is_required and "requiredReviewerIds" in policy_group["currentScopePolicies"][0]["settings"]:
+                reviewers = policy_group["currentScopePolicies"][0]["settings"]["requiredReviewerIds"]
+                for reviewer_id in reviewers:
+                    [x for x in all_reviewers if x.member_id == reviewer_id][0].is_required = True
+        return all_reviewers
+
+    @classmethod
+    def add_default_reviewer(cls, ado_client: AdoClient, repo_id: str, reviewer_id: str, is_required: bool, branch_name: str = "main") -> None:
+        if reviewer_id in [x.member_id for x in cls.get_default_reviewers(ado_client, repo_id, branch_name)]:
+            raise ValueError("Reviewer already exists! To update, please remove the reviewer first.")
+        payload = {
+            "type": {"id": _get_type_id(ado_client, "Required reviewers")}, "isBlocking": is_required, "isEnabled": True,
+            "settings": {
+                "requiredReviewerIds": [reviewer_id],
+                "scope":[{"repositoryId": repo_id, "refName": f"refs/heads/{branch_name}", "matchKind": "Exact"}]
+            }}
+        request = requests.post(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/configurations?api-version=7.1",
+                                json=payload, headers={"Accept": "application/json;api-version=7.1"}, auth=ado_client.auth)
+        assert request.status_code == 200, f"Error setting branch policy: {request.text}"
 
     @staticmethod
-    def set_branch_policy(ado_client: AdoClient, policy_id: str | None, repo_id: str, minimum_approver_count: int,
-                          creator_vote_counts: bool, prohibit_last_pushers_vote: bool, allow_completion_with_rejects: bool,
-                          when_new_changes_are_pushed: WhenChangesArePushed, branch_name: str = "main") -> "RepoBranchPolicies | None":
-        return RepoBranchPolicies.set_branch_policy(ado_client, policy_id, repo_id, minimum_approver_count, creator_vote_counts,
-                                                    prohibit_last_pushers_vote, allow_completion_with_rejects, when_new_changes_are_pushed,
-                                                    branch_name)
-
-# ====================================================================
+    def remove_default_reviewer(ado_client: AdoClient, repo_id: str, reviewer_id: str, branch_name: str = "main") -> None:
+        policies = MergePolicies.get_default_reviewers_by_repo_id(ado_client, repo_id, branch_name)
+        policy_id = [x for x in policies if x.required_reviewer_id == reviewer_id][0].policy_id if policies is not None else None  # type: ignore[comparison-overlap]
+        if not policy_id:
+            return
+        request = requests.delete(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/configurations/{policy_id}?api-version=7.1", auth=ado_client.auth)
+        assert request.status_code == 204, "Error removing required reviewer"
 
 
 @dataclass
-class BuildRepository:
-    build_repository_id: str = field(metadata={"is_id_field": True})
-    name: str | None = None
-    type: str = "TfsGit"
-    clean: bool | None = None
-    checkout_submodules: bool = field(default=False, metadata={"internal_name": "checkoutSubmodules"})
-
-    @classmethod
-    def from_request_payload(cls, data: dict[str, str | bool]) -> "BuildRepository":
-        return cls(data["id"], data.get("name"), data.get("type", "TfsGit"), data.get("clean"), data.get("checkoutSubmodules", False))  # type: ignore[arg-type]
-
-    @classmethod
-    def from_json(cls, data: dict[str, str | bool]) -> "BuildRepository":
-        return cls(data["id"], data.get("name"), data.get("type", "TfsGit"), data.get("clean"), data.get("checkoutSubmodules", False))  # type: ignore[arg-type]
-
-    def to_json(self) -> dict[str, str | bool | None]:
-        return {
-            "id": self.build_repository_id, "name": self.name, "type": self.type,
-            "clean": self.clean, "checkoutSubmodules": self.checkout_submodules,  # fmt: skip
-        }
-
-
-name_mapping = {
-    "requireVoteOnEachIteration": "require_revote_on_each_iteration",
-    "requireVoteOnLastIteration": "require_revote_on_last_iteration",
-    "resetOnSourcePush": "reset_votes_on_source_push",
-    "resetRejectionsOnSourcePush": "reset_rejections_on_source_push",
-    "do_nothing": "do_nothing"
-}
-
-@dataclass
-class RepoBranchPolicies(StateManagedResource):
+class MergeBranchPolicy(StateManagedResource):
     policy_id: str = field(metadata={"is_id_field": True})
-    policy_group_uuid: str
-    repo_id: str
-    branch_name: str
+    policy_group_uuid: str = field(repr=False)
+    repo_id: str = field(repr=False)
+    branch_name: str = field(repr=False)
     minimum_approver_count: int
     creator_vote_counts: bool
     prohibit_last_pushers_vote: bool
     allow_completion_with_rejects: bool
     when_new_changes_are_pushed: WhenChangesArePushed
+    created_date: datetime = field(repr=False)
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, Any]) -> "RepoBranchPolicies | None":  # type: ignore[override]
-        policy_groups = data["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["policyGroups"]
-        if not policy_groups:
-            return None
-        first_policy_group = list(policy_groups.values())[0]
-        if first_policy_group is None or first_policy_group["currentScopePolicies"] is None:
-            return None
-        settings = first_policy_group["currentScopePolicies"][0]["settings"]
-        policy_group_id = list(policy_groups.keys())[0]
-        when_new_changes_are_pushed = name_mapping[([x for x in ("requireVoteOnEachIteration", "requireVoteOnLastIteration", "resetOnSourcePush", "resetRejectionsOnSourcePush") if settings.get(x, False)] or ["do_nothing"])[0]]  # Any or "do_nothing"
+    def from_request_payload(cls, policy_group_id: str, policy: dict[str, Any]) -> "MergeBranchPolicy":  # type: ignore[override]
+        settings = policy["settings"]
+        when_new_changes_are_pushed = name_mapping[([x for x in ("requireVoteOnEachIteration", "requireVoteOnLastIteration", "resetOnSourcePush", "resetRejectionsOnSourcePush") if settings.get(x, False)] or ["do_nothing"])[0]]  # Any or "do_nothing"  # fmt: skip
         return cls(
-            first_policy_group["currentScopePolicies"][0]["id"], policy_group_id, settings["scope"][0]["refName"].removeprefix("refs/heads/"), settings["scope"][0]["repositoryId"],
+            policy["id"], policy_group_id, settings["scope"][0]["refName"].removeprefix("refs/heads/"), settings["scope"][0]["repositoryId"],
             settings["minimumApproverCount"], settings["creatorVoteCounts"], settings["blockLastPusherVote"], settings["allowDownvotes"],
-            when_new_changes_are_pushed  # type: ignore[arg-type]
+            when_new_changes_are_pushed, from_ado_date_string(policy["createdDate"])   # type: ignore[arg-type]  # fmt: skip
         )
 
     @classmethod
-    def get_by_repo_id(cls, ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> "RepoBranchPolicies | None":
-        """Unofficial API, may break at any time."""
-        headers = {"Accept": "application/json;api-version=7.0-preview.1;excludeUrls=true;enumsAsNumbers=true;msDateFormat=true;noArrayWrap=true"}
-        payload = {"contributionIds": ["ms.vss-code-web.branch-policies-data-provider"], "dataProviderContext": {"properties": {"repositoryId": repo_id, "refName": f"refs/heads/{branch_name}", "sourcePage": {"routeValues": {"project": ado_client.ado_project, "adminPivot": "repositories", "controller": "ContributedPage"," action": "Execute"}}}}}
-        request = requests.post(f"https://dev.azure.com/{ado_client.ado_org}/_apis/Contribution/HierarchyQuery", headers=headers, json=payload, auth=ado_client.auth).json()
-        return cls.from_request_payload(request)
+    def get_branch_policy(cls, ado_client: AdoClient, repo_id: str, branch_name: str) -> "MergeBranchPolicy":
+        """Unofficial API, may break at any time. Gets the latest merge requirements for a pull request."""
+        return MergePolicies.get_all_branch_policies_by_repo_id(ado_client, repo_id)[0]  # type: ignore[index]
 
     @staticmethod
-    def _get_type_id(ado_client: AdoClient) -> str:
-        request = requests.get(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/policy/types?api-version=6.0", auth=ado_client.auth)
-        return [x for x in request.json()["value"] if x["displayName"] == "Minimum number of reviewers"][0]["id"]  # type: ignore[no-any-return]
-
-    @classmethod
-    def set_branch_policy(cls, ado_client: AdoClient, policy_id: str | None, repo_id: str, minimum_approver_count: int,
+    def set_branch_policy(ado_client: AdoClient, repo_id: str, minimum_approver_count: int,
                           creator_vote_counts: bool, prohibit_last_pushers_vote: bool, allow_completion_with_rejects: bool,
-                          when_new_changes_are_pushed: WhenChangesArePushed, branch_name: str = "main") -> None:
-        """Unofficial API, may break at any time. Sets the perms for a branch, can also be used as a "create" function."""
+                          when_new_changes_are_pushed: WhenChangesArePushed, branch_name: str = "main") -> None:  # fmt: skip
+        """Unofficial API, may break at any time. Sets the perms for a pull request, can also be used as a "update" function."""
+        existing_policy = MergePolicies.get_all_by_repo_id(ado_client, repo_id, branch_name)
+        latest_policy_id = existing_policy[0].policy_id if existing_policy is not None else None
         payload = {
             "settings": {
                 "minimumApproverCount": minimum_approver_count,
                 "creatorVoteCounts":    creator_vote_counts,
                 "blockLastPusherVote":  prohibit_last_pushers_vote,
                 "allowDownvotes":       allow_completion_with_rejects,
                 "requireVoteOnEachIteration":  when_new_changes_are_pushed == "require_revote_on_each_iteration",
                 "requireVoteOnLastIteration":  when_new_changes_are_pushed == "require_revote_on_last_iteration",
                 "resetOnSourcePush":           when_new_changes_are_pushed == "reset_votes_on_source_push",
                 "resetRejectionsOnSourcePush": when_new_changes_are_pushed == "reset_rejections_on_source_push",
-                "scope": [{"refName": f"refs/heads/{branch_name}", "matchKind": "Exact", "repositoryId": repo_id}],
+                "scope": [{"refName": f"refs/heads/{branch_name}", "repositoryId": repo_id, "matchKind": "Exact"}],
             },
             "isEnabled": True, "isBlocking": True,
-            "type": {"id": cls._get_type_id(ado_client)},
+            "type": {"id": _get_type_id(ado_client, "Minimum number of reviewers")},
         }
-        request_method = "POST" if policy_id is None else "PUT"
-        request = requests.request(request_method, f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/Configurations/{policy_id or ''}".rstrip("/"),
+        request_method = "POST" if latest_policy_id is None else "PUT"
+        request = requests.request(request_method, f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/Configurations/{latest_policy_id or ''}".rstrip("/"),
                                    json=payload, headers={"Accept": "application/json;api-version=7.1"}, auth=ado_client.auth)
         assert request.status_code == 200, f"Error setting branch policy: {request.text}"
-        # return cls.from_request_payload(request.json())
 
 
-RepoBranchPolicies.create = RepoBranchPolicies.set_branch_policy  # type: ignore[assignment]
+@dataclass
+class MergePolicies(StateManagedResource):
+    @classmethod
+    def from_request_payload(cls, data: dict[str, Any]) -> list["MergePolicyDefaultReviewer | MergeBranchPolicy"] | None:  # type: ignore[override]
+        """Used internally to get a list of all policies."""
+        policy_groups: dict[str, Any] = data["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["policyGroups"] or {}  # fmt: skip
+        all_policies = []
+        for policy_group_id, policy_group in policy_groups.items():
+            if policy_group["currentScopePolicies"] is None:
+                continue
+            for policy in policy_group["currentScopePolicies"]:
+                settings = policy["settings"]
+                if "cep-account-main" in settings:
+                    continue
+                if "requiredReviewerIds" in settings:
+                    all_policies.append(MergePolicyDefaultReviewer.from_request_payload(policy))
+                else:
+                    all_policies.append(MergeBranchPolicy.from_request_payload(policy_group_id, policy))
+        return all_policies or None  # type: ignore[return-value]
+
+    @classmethod
+    def get_all_by_repo_id(cls, ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list["MergePolicyDefaultReviewer | MergeBranchPolicy"] | None:  # fmt: skip
+        payload = {"contributionIds": ["ms.vss-code-web.branch-policies-data-provider"], "dataProviderContext": {"properties": {
+            "repositoryId": repo_id, "refName": f"refs/heads/{branch_name}", "sourcePage": {"routeValues": {"project": ado_client.ado_project}}}}}  # fmt: skip
+        request = requests.post(f"https://dev.azure.com/{ado_client.ado_org}/_apis/Contribution/HierarchyQuery?api-version=7.0-preview.1",
+                                json=payload, auth=ado_client.auth).json()  # fmt: skip
+        return cls.from_request_payload(request)
+
+    @classmethod
+    def get_all_branch_policies_by_repo_id(cls, ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list[MergeBranchPolicy] | None:  # fmt: skip
+        policies = cls.get_all_by_repo_id(ado_client, repo_id, branch_name)
+        return (
+            sorted([x for x in policies if isinstance(x, MergeBranchPolicy)], key=lambda x: x.created_date, reverse=True)
+            if policies is not None else None
+        )  # fmt: skip
+
+    @classmethod
+    def get_default_reviewers_by_repo_id(cls, ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list[MergePolicyDefaultReviewer] | None:  # fmt: skip
+        policies = cls.get_all_by_repo_id(ado_client, repo_id, branch_name)
+        return [x for x in policies if isinstance(x, MergePolicyDefaultReviewer)] if policies is not None else None
+
+    # ================== Default Reviewers ================== #
+    @staticmethod
+    def add_default_reviewer(ado_client: AdoClient, repo_id: str, reviewer_id: str, is_required: bool, branch_name: str = "main") -> None:
+        return MergePolicyDefaultReviewer.add_default_reviewer(ado_client, repo_id, reviewer_id, is_required, branch_name)
+
+    @staticmethod
+    def get_default_reviewers(ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list[Reviewer]:
+        return MergePolicyDefaultReviewer.get_default_reviewers(ado_client, repo_id, branch_name)
+
+    @staticmethod
+    def remove_default_reviewer(ado_client: AdoClient, repo_id: str, reviewer_id: str, branch_name: str = "main") -> None:
+        return MergePolicyDefaultReviewer.remove_default_reviewer(ado_client, repo_id, reviewer_id, branch_name)
+
+    # ================== Branch Policies ================== #
+    @staticmethod
+    def set_branch_policy(ado_client: AdoClient, repo_id: str, minimum_approver_count: int,
+                          creator_vote_counts: bool, prohibit_last_pushers_vote: bool, allow_completion_with_rejects: bool,
+                          when_new_changes_are_pushed: WhenChangesArePushed, branch_name: str = "main") -> None:
+        return MergeBranchPolicy.set_branch_policy(ado_client, repo_id, minimum_approver_count, creator_vote_counts,
+                                                   prohibit_last_pushers_vote, allow_completion_with_rejects,
+                                                   when_new_changes_are_pushed, branch_name)  # fmt: skip
+
+    @staticmethod
+    def get_branch_policy(ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> MergeBranchPolicy:
+        return MergeBranchPolicy.get_branch_policy(ado_client, repo_id, branch_name)
```

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/teams.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/users.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,16 +158,16 @@
 
 
 class Reviewer(Member):
     """Identical to Member, but with additional attributes `vote` and `is_required` for PR reviews."""
 
     def __init__(self, name: str, email: str, reviewer_id: str, vote: VoteOptions, is_required: bool) -> None:
         super().__init__(name, email, reviewer_id)
-        self.vote = vote  # Static
-        self.is_required = is_required  # Static
+        self.vote = vote
+        self.is_required = is_required
 
     def __str__(self) -> str:
         return f'{self.name} ({self.email}) voted {VOTE_ID_TO_TYPE[self.vote]}, and was {"required" if self.is_required else "optional"}'
 
     def __repr__(self) -> str:
         return f"Reviewer(name={self.name}, email={self.email}, id={self.member_id}, vote={self.vote}, is_required={self.is_required})"
```

### Comparing `ado_wrapper-0.0.6/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-0.0.7/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/state_managed_abc.py` & `ado_wrapper-0.0.7/ado_wrapper/state_managed_abc.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             if request.status_code == 404:
                 print("[ADO_WRAPPER] Resource not found, probably already deleted, removing from state")
             else:
                 raise DeletionFailed(f"[ADO_WRAPPER] Error deleting {cls.__name__} ({resource_id}): {request.json()['message']}")
         ado_client.state_manager.remove_resource_from_state(cls.__name__, resource_id)  # type: ignore[arg-type]
 
     def delete(self, ado_client: "AdoClient") -> None:
-        return self.delete_by_id(ado_client, extract_id(self))  # type: ignore[call-arg]
+        return self.delete_by_id(ado_client, extract_id(self))  # type: ignore[call-arg]  # pylint: disable=no-value-for-parameter
 
     def update(self, ado_client: "AdoClient", update_action: Literal["put", "patch"], url: str,  # pylint: disable=too-many-arguments
                attribute_name: str, attribute_value: Any, params: dict[str, Any]) -> None:  # fmt: skip
         """The params should be a dictionary which will be combined with the internal name and value of the attribute to be updated."""
         interal_names = get_internal_field_names(self.__class__)
         if attribute_name not in get_internal_field_names(self.__class__):
             raise ValueError(f"The attribute `{attribute_name}` is not editable!  Editable attributes are: {list(interal_names.keys())}")
@@ -141,15 +141,15 @@
         return [cls.from_request_payload(resource) for resource in request.json()["value"]]
 
     @classmethod
     def get_by_abstract_filter(
         cls, ado_client: "AdoClient", func: Callable[["StateManagedResource"], bool]
     ) -> "StateManagedResource | None":
         """Used internally for getting resources by a filter function. The function should return True if the resource is the one you want."""
-        resources = cls.get_all(ado_client)  # type: ignore[call-arg]
+        resources = cls.get_all(ado_client)  # type: ignore[call-arg]  # pylint: disable=no-value-for-parameter
         for resource in resources:
             if func(resource):
                 return resource
         return None
 
     def set_lifecycle_policy(self, ado_client: "AdoClient", policy: Literal["prevent_destroy", "ignore_changes"]) -> None:
         self.life_cycle_policy = policy  # TODO
```

### Comparing `ado_wrapper-0.0.6/ado_wrapper/state_manager.py` & `ado_wrapper-0.0.7/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/ado_wrapper/utils.py` & `ado_wrapper-0.0.7/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.6/pyproject.toml` & `ado_wrapper-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "0.0.6"
+version = "0.0.7"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
 
@@ -26,33 +26,34 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 plugins = ["pydantic.mypy"]
-exclude = ['.venv', '.vscode', '.pytest_cache', '.mypy_cache', '.git', '__pycache__', 'script.py']
+exclude = ['.vscode', '.pytest_cache', '.mypy_cache', '.git', '__pycache__', 'script.py']
 strict = true
 
 [tool.pylint.main]
-ignore = [".venv"]
+ignore = [".venv", ".vscode", ".pytest_cache", ".mypy_cache", ".git", "__pycache__", "script.py"]
 recursive = true
 
 [tool.pylint.messages_control]
 max-line-length = 140
 disable = [
     "missing-module-docstring",
     "missing-class-docstring",
     "missing-function-docstring",
     "missing-timeout",
 
     "too-few-public-methods",
     "too-many-instance-attributes",
     "too-many-arguments",
 
+    "unused-argument",
     "fixme",
     "arguments-differ",
     "arguments-renamed",
     "invalid-name",
     "too-many-locals",
     "line-too-long",
     "broad-exception-caught",
```

### Comparing `ado_wrapper-0.0.6/PKG-INFO` & `ado_wrapper-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 0.0.6
+Version: 0.0.7
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


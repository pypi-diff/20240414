# Comparing `tmp/ado_wrapper-0.0.7.tar.gz` & `tmp/ado_wrapper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-0.0.7.tar", max compression
+gzip compressed data, was "ado_wrapper-0.0.8.tar", max compression
```

## Comparing `ado_wrapper-0.0.7.tar` & `ado_wrapper-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.7/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-0.0.7/README.md
--rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.7/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6504 2024-04-13 22:19:56.681692 ado_wrapper-0.0.7/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2123 2024-04-10 11:16:39.930064 ado_wrapper-0.0.7/ado_wrapper/client.py
--rw-r--r--   0        0        0    25667 2024-04-11 13:43:04.075027 ado_wrapper-0.0.7/ado_wrapper/dumps.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.7/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-0.0.7/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.7/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-0.0.7/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-12 10:52:50.915024 ado_wrapper-0.0.7/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0     1342 2024-04-10 19:18:54.311903 ado_wrapper-0.0.7/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0      659 2024-04-08 18:01:44.152197 ado_wrapper-0.0.7/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     4650 2024-04-09 09:35:29.826115 ado_wrapper-0.0.7/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    13517 2024-04-09 20:21:18.486611 ado_wrapper-0.0.7/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6637 2024-04-09 18:43:12.632598 ado_wrapper-0.0.7/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     3477 2024-04-09 18:30:16.745942 ado_wrapper-0.0.7/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    13519 2024-04-13 22:29:12.944703 ado_wrapper-0.0.7/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-0.0.7/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    14800 2024-04-09 18:53:28.574098 ado_wrapper-0.0.7/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12781 2024-04-09 20:19:59.831154 ado_wrapper-0.0.7/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10304 2024-04-13 22:19:35.024746 ado_wrapper-0.0.7/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     6014 2024-04-10 18:05:31.126571 ado_wrapper-0.0.7/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4622 2024-04-09 18:43:22.061540 ado_wrapper-0.0.7/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8350 2024-04-13 18:18:13.167779 ado_wrapper-0.0.7/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4934 2024-04-09 18:30:55.561929 ado_wrapper-0.0.7/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     8499 2024-04-12 10:53:35.658831 ado_wrapper-0.0.7/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8158 2024-04-10 17:53:40.392730 ado_wrapper-0.0.7/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4257 2024-04-08 17:51:22.897215 ado_wrapper-0.0.7/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2191 2024-04-13 22:29:36.283420 ado_wrapper-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.8/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-0.0.8/README.md
+-rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.8/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6504 2024-04-13 22:32:43.045229 ado_wrapper-0.0.8/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2163 2024-04-14 11:00:28.638164 ado_wrapper-0.0.8/ado_wrapper/client.py
+-rw-r--r--   0        0        0    25667 2024-04-11 13:43:04.075027 ado_wrapper-0.0.8/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.8/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-0.0.8/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.8/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-0.0.8/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-12 10:52:50.915024 ado_wrapper-0.0.8/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0     1342 2024-04-10 19:18:54.311903 ado_wrapper-0.0.8/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0      659 2024-04-08 18:01:44.152197 ado_wrapper-0.0.8/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     4650 2024-04-09 09:35:29.826115 ado_wrapper-0.0.8/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    13458 2024-04-14 10:58:44.110259 ado_wrapper-0.0.8/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6583 2024-04-14 10:58:41.445364 ado_wrapper-0.0.8/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     3432 2024-04-14 10:58:38.698564 ado_wrapper-0.0.8/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    14440 2024-04-14 11:02:49.747626 ado_wrapper-0.0.8/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-0.0.8/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    14600 2024-04-14 10:58:31.073500 ado_wrapper-0.0.8/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12740 2024-04-14 10:58:27.795680 ado_wrapper-0.0.8/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10304 2024-04-14 11:02:04.259069 ado_wrapper-0.0.8/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     5972 2024-04-14 10:59:00.916715 ado_wrapper-0.0.8/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4569 2024-04-14 10:59:03.753536 ado_wrapper-0.0.8/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8313 2024-04-14 09:38:20.128931 ado_wrapper-0.0.8/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4877 2024-04-14 10:59:52.033985 ado_wrapper-0.0.8/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     8422 2024-04-14 11:01:12.740028 ado_wrapper-0.0.8/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8158 2024-04-10 17:53:40.392730 ado_wrapper-0.0.8/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4257 2024-04-08 17:51:22.897215 ado_wrapper-0.0.8/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2213 2024-04-14 11:05:21.074143 ado_wrapper-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-0.0.8/PKG-INFO
```

### Comparing `ado_wrapper-0.0.7/LICENSE` & `ado_wrapper-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.7/README.md` & `ado_wrapper-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.7/ado_wrapper/__main__.py` & `ado_wrapper-0.0.8/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.7/ado_wrapper/client.py` & `ado_wrapper-0.0.8/ado_wrapper/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,22 +14,25 @@
         state_file_name: str | None = "main.state", bypass_initialisation: bool = False,
         action: Literal["plan", "apply"] = "apply"  # fmt: skip
     ) -> None:
         """Takes an email, PAT, org, project, and state file name. The state file name is optional, and if not provided,
         state will not be stored in "main.state" """
         self.ado_email = ado_email
         self.ado_pat = ado_pat
-        self.auth = HTTPBasicAuth(ado_email, ado_pat)
         self.ado_org = ado_org
         self.ado_project = ado_project
+
         self.plan_mode = action == "plan"
 
+        self.session = requests.Session()
+        self.session.auth = HTTPBasicAuth(ado_email, ado_pat)
+
         if not bypass_initialisation:
             # Verify Token is working (helps with setup for first time users):
-            request = requests.get(f"https://dev.azure.com/{self.ado_org}/_apis/projects?api-version=7.1", auth=self.auth)
+            request = self.session.get(f"https://dev.azure.com/{self.ado_org}/_apis/projects?api-version=7.1")
             if request.status_code != 200:
                 raise AuthenticationError(f"Failed to authenticate with ADO: {request.text}")
 
             from ado_wrapper.resources.projects import Project  # Stop circular import
             from ado_wrapper.resources.users import AdoUser  # Stop circular import
 
             self.ado_project_id = Project.get_by_name(self, self.ado_project).project_id  # type: ignore[union-attr]
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/dumps.py` & `ado_wrapper-0.0.8/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.7/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-0.0.8/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.7/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-0.0.8/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.7/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-0.0.8/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/__init__.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/branches.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/builds.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/builds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from datetime import datetime
 from dataclasses import dataclass, field
 from typing import Any, Literal, TYPE_CHECKING
 import time
 
-import requests
-
 from ado_wrapper.utils import from_ado_date_string
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member
 from ado_wrapper.resources.repo import BuildRepository
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
@@ -85,15 +83,15 @@
     def create(  # type: ignore[override]
         cls, ado_client: "AdoClient", definition_id: str, source_branch: str = "refs/heads/main", permit_use_of_var_groups: bool = False,  # fmt: skip
     ) -> "Build":
         """`permit_var_groups` defines whether the variable group will be automatically allowed for the build or need manual approval."""
         # if permit_use_of_var_groups:
         #     rint(f"Variable Groups: {BuildDefinition.get_by_id(ado_client, definition_id).variable_groups}")
         #     for var_group_id in BuildDefinition.get_by_id(ado_client, definition_id).variable_groups:
-        #         request = requests.patch(f"https://dev.azure.com/{ado_client.ado_org}/{definition_id}/_apis/pipelines/pipelinePermissions/variablegroup/{var_group_id}")  # fmt: skip
+        #         request = ado_client.session.patch(f"https://dev.azure.com/{ado_client.ado_org}/{definition_id}/_apis/pipelines/pipelinePermissions/variablegroup/{var_group_id}")  # fmt: skip
         #         rint(request.text, request.status_code)
         #         assert request.status_code <= 204
         return super().create(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/builds?definitionId={definition_id}&api-version=7.1",
             {"reason": "An automated build created with the ado_wrapper Python library", "sourceBranch": source_branch},
         )  # type: ignore[return-value]
@@ -139,26 +137,24 @@
             if (datetime.now() - start_time).seconds > max_timeout_seconds:
                 raise TimeoutError(f"The build did not complete within {max_timeout_seconds} seconds ({max_timeout_seconds//60} minutes)")
             time.sleep(3)
         return build
 
     @staticmethod
     def delete_all_leases(ado_client: "AdoClient", build_id: str) -> None:
-        leases_request = requests.get(
+        leases_request = ado_client.session.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/builds/{build_id}/leases?api-version=7.1",
-            auth=ado_client.auth,
         )
         if leases_request.status_code != 200:
             print(f"Could not delete leases, {leases_request.status_code}")
             return
         leases = leases_request.json()["value"]
         for lease in leases:
-            lease_response = requests.delete(
+            lease_response = ado_client.session.delete(
                 f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/build/retention/leases?ids={lease['leaseId']}&api-version=6.1",
-                auth=ado_client.auth,
             )
             assert lease_response.status_code <= 204
 
 
 # ========================================================================================================
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/commits.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/commits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from datetime import datetime
 from dataclasses import dataclass, field
 from typing import Literal, Any, TYPE_CHECKING
 
-import requests
-
 from ado_wrapper.utils import from_ado_date_string, InvalidPermissionsError
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
@@ -81,15 +79,15 @@
             from_branch_name.startswith("refs/heads/") or to_branch_name.startswith("refs/heads/")
         ), "Branch names should not start with 'refs/heads/'"
         if not updates:
             raise ValueError("No updates provided! It's not possible to create a commit without updates.")
         latest_commit = cls.get_latest_by_repo(ado_client, repo_id, from_branch_name)
         latest_commit_id = None if latest_commit is None else latest_commit.commit_id
         data = get_commit_body_template(latest_commit_id, updates, to_branch_name, change_type, commit_message)
-        request = requests.post(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pushes?api-version=7.1", json=data, auth=ado_client.auth)  # fmt: skip
+        request = ado_client.session.post(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pushes?api-version=7.1", json=data)  # fmt: skip
         if request.status_code == 400:
             raise ValueError("The commit was not created successfully, the file(s) you're trying to add might already exist there.")
         if request.status_code == 403:
             raise InvalidPermissionsError("You do not have permission to create a commit in this repo (possibly due to main branch protections)")  # fmt: skip
         if not request.json().get("commits"):
             raise ValueError("The commit was not created successfully.\nError:", request.json())
         return cls.from_request_payload(request.json()["commits"][-1])
@@ -122,12 +120,12 @@
         default_commit_body["commits"] = [{
             "comment": "Add README.md",
             "changes": [{
                 "changeType": 1, "item": {"path": "/README.md"},
                 "newContentTemplate": {"name": "README.md", "type": "readme"}
             }],
         }]  # fmt: skip
-        request = requests.post(
+        request = ado_client.session.post(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pushes?api-version=7.1",
-            json=default_commit_body, auth=ado_client.auth,  # fmt: skip
+            json=default_commit_body,
         )
         return cls.from_request_payload(request.json()["commits"][0])
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/groups.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from dataclasses import dataclass, field
 
-# import requests
-
 from ado_wrapper.state_managed_abc import StateManagedResource
 
 # from ado_wrapper.resources.users import GroupMember
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
@@ -59,17 +57,16 @@
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_by_name(cls, ado_client: AdoClient, group_name: str) -> "Group | None":
         return cls.get_by_abstract_filter(ado_client, lambda group: group.name == group_name)  # type: ignore[return-value, attr-defined]
 
     # def get_members(self, ado_client: AdoClient) -> list["GroupMember"]:
-    #     request = requests.get(
+    #     request = ado_client.session.get(
     #         f"https://dev.azure.com/{ado_client.ado_org}/_apis/projects/{ado_client.ado_project}/groups/{self.group_id}/members?api-version=7.1-preview.2",
-    #         auth=ado_client.auth,
     #     ).json()
     #     rint(request)
     #     # return [GroupMember.from_request_payload(member) for member in request]
 
     @classmethod
     def get_all_by_member(cls, ado_client: AdoClient, member_descriptor_id: str) -> list["Group"]:
         raise NotImplementedError
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/merge_policies.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Any, Literal, TYPE_CHECKING
 
-import requests
-
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Reviewer
 from ado_wrapper.utils import from_ado_date_string
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
@@ -20,16 +18,16 @@
     "resetOnSourcePush": "reset_votes_on_source_push",
     "resetRejectionsOnSourcePush": "reset_rejections_on_source_push",
     "do_nothing": "do_nothing"
 }
 
 def _get_type_id(ado_client: AdoClient, action_type: str) -> str:
     """Used internally to get a specific update request ID"""
-    request = requests.get(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/policy/types?api-version=6.0", auth=ado_client.auth)
-    # print([(x["displayName"], x["id"]) for x in request.json()["value"]])
+    request = ado_client.session.get(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/policy/types?api-version=6.0")
+    # rint([(x["displayName"], x["id"]) for x in request.json()["value"]])
     return [x for x in request.json()["value"] if x["displayName"] == action_type][0]["id"]  # type: ignore[no-any-return]
 
 
 @dataclass
 class MergePolicyDefaultReviewer(StateManagedResource):
     policy_id: str = field(metadata={"is_id_field": True})
     required_reviewer_id: list[str]
@@ -39,16 +37,16 @@
     def from_request_payload(cls, data: dict[str, Any]) -> StateManagedResource:
         return cls(data["id"], data["settings"]["requiredReviewerIds"][0], data["isBlocking"])
 
     @staticmethod
     def get_default_reviewers(ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list[Reviewer]:
         payload = {"contributionIds": ["ms.vss-code-web.branch-policies-data-provider"],
                    "dataProviderContext": {"properties": {"projectId": ado_client.ado_project_id, "repositoryId": repo_id, "refName": f"refs/heads/{branch_name}"}}}
-        request = requests.post("https://dev.azure.com/VFCloudEngineering/_apis/Contribution/HierarchyQuery?api-version=7.1-preview.1",
-                               json=payload, auth=ado_client.auth).json()
+        request = ado_client.session.post("https://dev.azure.com/VFCloudEngineering/_apis/Contribution/HierarchyQuery?api-version=7.1-preview.1",
+                                          json=payload).json()
         if request is None:
             return []
         all_reviewers = [Reviewer(x["displayName"], x["uniqueName"], x["id"], 0, False) for x in request["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["identities"]]
         for policy_group in request["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["policyGroups"].values():
             if policy_group["currentScopePolicies"] is None:
                 continue
             is_required = policy_group["currentScopePolicies"][0]["isBlocking"]
@@ -62,126 +60,140 @@
     def add_default_reviewer(cls, ado_client: AdoClient, repo_id: str, reviewer_id: str, is_required: bool, branch_name: str = "main") -> None:
         if reviewer_id in [x.member_id for x in cls.get_default_reviewers(ado_client, repo_id, branch_name)]:
             raise ValueError("Reviewer already exists! To update, please remove the reviewer first.")
         payload = {
             "type": {"id": _get_type_id(ado_client, "Required reviewers")}, "isBlocking": is_required, "isEnabled": True,
             "settings": {
                 "requiredReviewerIds": [reviewer_id],
-                "scope":[{"repositoryId": repo_id, "refName": f"refs/heads/{branch_name}", "matchKind": "Exact"}]
+                "scope": [{"repositoryId": repo_id, "refName": f"refs/heads/{branch_name}", "matchKind": "Exact"}]
             }}
-        request = requests.post(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/configurations?api-version=7.1",
-                                json=payload, headers={"Accept": "application/json;api-version=7.1"}, auth=ado_client.auth)
+        request = ado_client.session.post(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/configurations?api-version=7.1",
+                                json=payload, headers={"Accept": "application/json;api-version=7.1"})
         assert request.status_code == 200, f"Error setting branch policy: {request.text}"
 
     @staticmethod
     def remove_default_reviewer(ado_client: AdoClient, repo_id: str, reviewer_id: str, branch_name: str = "main") -> None:
         policies = MergePolicies.get_default_reviewers_by_repo_id(ado_client, repo_id, branch_name)
         policy_id = [x for x in policies if x.required_reviewer_id == reviewer_id][0].policy_id if policies is not None else None  # type: ignore[comparison-overlap]
         if not policy_id:
             return
-        request = requests.delete(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/configurations/{policy_id}?api-version=7.1", auth=ado_client.auth)
+        request = ado_client.session.delete(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/configurations/{policy_id}?api-version=7.1")
         assert request.status_code == 204, "Error removing required reviewer"
 
 
 @dataclass
 class MergeBranchPolicy(StateManagedResource):
     policy_id: str = field(metadata={"is_id_field": True})
-    policy_group_uuid: str = field(repr=False)
     repo_id: str = field(repr=False)
-    branch_name: str = field(repr=False)
+    branch_name: str | None = field(repr=False)
     minimum_approver_count: int
     creator_vote_counts: bool
     prohibit_last_pushers_vote: bool
     allow_completion_with_rejects: bool
     when_new_changes_are_pushed: WhenChangesArePushed
     created_date: datetime = field(repr=False)
+    is_inherited: bool = field(default=False, repr=False)
 
     @classmethod
-    def from_request_payload(cls, policy_group_id: str, policy: dict[str, Any]) -> "MergeBranchPolicy":  # type: ignore[override]
-        settings = policy["settings"]
+    def from_request_payload(cls, data: dict[str, Any], is_inherited: bool) -> "MergeBranchPolicy":  # type: ignore[override]
+        settings = data["settings"]
         when_new_changes_are_pushed = name_mapping[([x for x in ("requireVoteOnEachIteration", "requireVoteOnLastIteration", "resetOnSourcePush", "resetRejectionsOnSourcePush") if settings.get(x, False)] or ["do_nothing"])[0]]  # Any or "do_nothing"  # fmt: skip
+        branch_name: str | None = settings["scope"][0]["refName"]
         return cls(
-            policy["id"], policy_group_id, settings["scope"][0]["refName"].removeprefix("refs/heads/"), settings["scope"][0]["repositoryId"],
+            data["id"], settings["scope"][0]["repositoryId"], (branch_name.removeprefix("refs/heads/") if branch_name else None),
             settings["minimumApproverCount"], settings["creatorVoteCounts"], settings["blockLastPusherVote"], settings["allowDownvotes"],
-            when_new_changes_are_pushed, from_ado_date_string(policy["createdDate"])   # type: ignore[arg-type]  # fmt: skip
+            when_new_changes_are_pushed, from_ado_date_string(data["createdDate"]),  # type: ignore[arg-type]
+            is_inherited     # fmt: skip
         )
 
     @classmethod
     def get_branch_policy(cls, ado_client: AdoClient, repo_id: str, branch_name: str) -> "MergeBranchPolicy":
-        """Unofficial API, may break at any time. Gets the latest merge requirements for a pull request."""
-        return MergePolicies.get_all_branch_policies_by_repo_id(ado_client, repo_id)[0]  # type: ignore[index]
+        """Gets the latest merge requirements for a pull request."""
+        return MergePolicies.get_all_branch_policies_by_repo_id(ado_client, repo_id, branch_name)[0]  # type: ignore[index]
 
     @staticmethod
     def set_branch_policy(ado_client: AdoClient, repo_id: str, minimum_approver_count: int,
                           creator_vote_counts: bool, prohibit_last_pushers_vote: bool, allow_completion_with_rejects: bool,
                           when_new_changes_are_pushed: WhenChangesArePushed, branch_name: str = "main") -> None:  # fmt: skip
-        """Unofficial API, may break at any time. Sets the perms for a pull request, can also be used as a "update" function."""
+        """Sets the perms for a pull request, can also be used as a "update" function."""
         existing_policy = MergePolicies.get_all_by_repo_id(ado_client, repo_id, branch_name)
-        latest_policy_id = existing_policy[0].policy_id if existing_policy is not None else None
+        latest_policy_id = existing_policy[0].policy_id if existing_policy is not None else None  # pylint: disable=unsubscriptable-object
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
                 "scope": [{"refName": f"refs/heads/{branch_name}", "repositoryId": repo_id, "matchKind": "Exact"}],
             },
-            "isEnabled": True, "isBlocking": True,
             "type": {"id": _get_type_id(ado_client, "Minimum number of reviewers")},
+            "isEnabled": True, "isBlocking": True,
         }
         request_method = "POST" if latest_policy_id is None else "PUT"
-        request = requests.request(request_method, f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/Configurations/{latest_policy_id or ''}".rstrip("/"),
-                                   json=payload, headers={"Accept": "application/json;api-version=7.1"}, auth=ado_client.auth)
+        request = ado_client.session.request(request_method, f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/policy/Configurations/{latest_policy_id or ''}".rstrip("/"),
+                                   json=payload, headers={"Accept": "application/json;api-version=7.1"})
         assert request.status_code == 200, f"Error setting branch policy: {request.text}"
 
 
 @dataclass
 class MergePolicies(StateManagedResource):
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> list["MergePolicyDefaultReviewer | MergeBranchPolicy"] | None:  # type: ignore[override]
         """Used internally to get a list of all policies."""
         policy_groups: dict[str, Any] = data["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["policyGroups"] or {}  # fmt: skip
         all_policies = []
-        for policy_group_id, policy_group in policy_groups.items():
-            if policy_group["currentScopePolicies"] is None:
-                continue
-            for policy in policy_group["currentScopePolicies"]:
+        for policy_group in policy_groups.values():
+            for policy in policy_group["currentScopePolicies"] or []:  # If it's None, don't loop
                 settings = policy["settings"]
-                if "cep-account-main" in settings:
+                # Limit merge types
+                if any(x in settings for x in ("allowSquash", "allowNoFastForward", "allowRebase", "allowRebaseMerge")):
+                    continue
+                # Build Validation {'buildDefinitionId': 4, 'queueOnSourceUpdateOnly': True, 'manualQueueOnly': False, 'displayName': None, 'validDuration': 720.0
+                if "buildDefinitionId" in settings:
                     continue
+                # Automatically included reviewers
                 if "requiredReviewerIds" in settings:
                     all_policies.append(MergePolicyDefaultReviewer.from_request_payload(policy))
+                elif "minimumApproverCount" in settings:
+                    new_policy = MergeBranchPolicy.from_request_payload(policy, False)
+                    # if "inheritedPolicies" in policy_group:
+                    #     new_policy.inherited_policies = [MergeBranchPolicy.from_request_payload(x) for x in policy_group["inheritedPolicies"]]
+                    all_policies.append(new_policy)
                 else:
-                    all_policies.append(MergeBranchPolicy.from_request_payload(policy_group_id, policy))
+                    print("Unknown policy type: ", policy)
+
+            # for inherited_policy in policy_group["inheritedPolicies"] or []:
+            #     all_policies.append(MergeBranchPolicy.from_request_payload(inherited_policy, True))
+
         return all_policies or None  # type: ignore[return-value]
 
     @classmethod
     def get_all_by_repo_id(cls, ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list["MergePolicyDefaultReviewer | MergeBranchPolicy"] | None:  # fmt: skip
         payload = {"contributionIds": ["ms.vss-code-web.branch-policies-data-provider"], "dataProviderContext": {"properties": {
             "repositoryId": repo_id, "refName": f"refs/heads/{branch_name}", "sourcePage": {"routeValues": {"project": ado_client.ado_project}}}}}  # fmt: skip
-        request = requests.post(f"https://dev.azure.com/{ado_client.ado_org}/_apis/Contribution/HierarchyQuery?api-version=7.0-preview.1",
-                                json=payload, auth=ado_client.auth).json()  # fmt: skip
+        request = ado_client.session.post(f"https://dev.azure.com/{ado_client.ado_org}/_apis/Contribution/HierarchyQuery?api-version=7.0-preview.1",
+                                json=payload).json()
         return cls.from_request_payload(request)
 
     @classmethod
     def get_all_branch_policies_by_repo_id(cls, ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list[MergeBranchPolicy] | None:  # fmt: skip
         policies = cls.get_all_by_repo_id(ado_client, repo_id, branch_name)
         return (
-            sorted([x for x in policies if isinstance(x, MergeBranchPolicy)], key=lambda x: x.created_date, reverse=True)
+            sorted([x for x in policies if isinstance(x, MergeBranchPolicy)], key=lambda x: x.created_date, reverse=True)  # pylint: disable=not-an-iterable
             if policies is not None else None
         )  # fmt: skip
 
     @classmethod
     def get_default_reviewers_by_repo_id(cls, ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> list[MergePolicyDefaultReviewer] | None:  # fmt: skip
         policies = cls.get_all_by_repo_id(ado_client, repo_id, branch_name)
-        return [x for x in policies if isinstance(x, MergePolicyDefaultReviewer)] if policies is not None else None
+        return [x for x in policies if isinstance(x, MergePolicyDefaultReviewer)] if policies is not None else None  # pylint: disable=not-an-iterable
 
     # ================== Default Reviewers ================== #
     @staticmethod
     def add_default_reviewer(ado_client: AdoClient, repo_id: str, reviewer_id: str, is_required: bool, branch_name: str = "main") -> None:
         return MergePolicyDefaultReviewer.add_default_reviewer(ado_client, repo_id, reviewer_id, is_required, branch_name)
 
     @staticmethod
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/projects.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/pull_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any, Literal, TYPE_CHECKING
 from dataclasses import dataclass, field
 
-import requests
-
 from ado_wrapper.utils import from_ado_date_string, ResourceNotFound
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member, Reviewer
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
     from ado_wrapper.resources.repo import Repo
@@ -65,17 +63,17 @@
         pull_request_description: str, is_draft: bool = False
     ) -> "PullRequest":  # fmt: skip
         """Takes a list of reviewer ids, a branch to pull into main, and an option to start as draft"""
         # https://stackoverflow.com/questions/64655138/add-reviewers-to-azure-devops-pull-request-in-api-call   <- Why we can't allow reviewers from the get go
         # , "reviewers": [{"id": reviewer_id for reviewer_id in reviewer_ids}]
         payload = {"sourceRefName": f"refs/heads/{from_branch_name}", "targetRefName": "refs/heads/main", "title": pull_request_title,
                    "description": pull_request_description, "isDraft": is_draft}  # fmt: skip
-        request = requests.post(
+        request = ado_client.session.post(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullrequests?api-version=7.1",
-            json=payload, auth=ado_client.auth,  # fmt: skip
+            json=payload,
         ).json()
         if request.get("message", "").startswith("TF401398"):
             raise ValueError("The branch you are trying to create a pull request from does not exist.")
         obj = cls.from_request_payload(request)
         ado_client.state_manager.add_resource_to_state(cls.__name__, obj.pull_request_id, obj.to_json())  # type: ignore[arg-type]
         return obj
 
@@ -106,39 +104,37 @@
 
     def add_reviewer(self, ado_client: AdoClient, reviewer_id: str) -> None:
         return self.add_reviewer_static(ado_client, self.repo.repo_id, self.pull_request_id, reviewer_id)
 
     @staticmethod
     def add_reviewer_static(ado_client: AdoClient, repo_id: str, pull_request_id: str, reviewer_id: str) -> None:
         """Copy of the add_reviewer method, but static, i.e. if you have the repo id and pr id, you don't need to fetch them again"""
-        request = requests.put(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullRequests/{pull_request_id}/reviewers/{reviewer_id}?api-version=7.1",
-                                json={"vote": "0", "isRequired": "true"}, auth=ado_client.auth)  # fmt: skip
+        request = ado_client.session.put(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullRequests/{pull_request_id}/reviewers/{reviewer_id}?api-version=7.1",
+                                json={"vote": "0", "isRequired": "true"},)
         assert request.status_code < 300
 
     def close(self, ado_client: AdoClient) -> None:
         self.update(ado_client, "merge_status", "abandoned")
 
     def mark_as_draft(self, ado_client: AdoClient) -> None:
         return self.update(ado_client, "is_draft", True)
 
     def unmark_as_draft(self, ado_client: AdoClient) -> None:
         return self.update(ado_client, "is_draft", True)
 
     def get_reviewers(self, ado_client: AdoClient) -> list[Member]:
-        request = requests.get(
+        request = ado_client.session.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo.repo_id}/pullRequests/{self.pull_request_id}/reviewers?api-version=7.1",
-            auth=ado_client.auth,
         ).json()
         return [Member.from_request_payload(reviewer) for reviewer in request["value"]]
 
     @classmethod
     def get_all_by_repo_id(cls, ado_client: AdoClient, repo_id: str, status: PullRequestStatus = "all") -> list[PullRequest]:
-        pull_requests = requests.get(
+        pull_requests = ado_client.session.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pullrequests?searchCriteria.status={status}&api-version=7.1",
-            auth=ado_client.auth,
         ).json()
         try:
             return [PullRequest.from_request_payload(pr) for pr in pull_requests["value"]]
         except KeyError:
             if pull_requests.get("message", "").startswith("TF401019"):
                 print(f"Repo `{pull_requests['message'].split('identifier')[1].split(' ')[0]}` was disabled, or you had no access.")
                 return []
@@ -149,40 +145,37 @@
         return [pr for pr in cls.get_all(ado_client, status) if pr.author.email == author_email]
 
     @classmethod
     def get_my_pull_requests(cls, ado_client: AdoClient) -> list[PullRequest]:
         """This is super tempremental, I have to do a bunch of splits, it's not official so might not work, the statuses are also numerical."""
         import json
 
-        request = requests.get(f"https://dev.azure.com/{ado_client.ado_org}/_pulls", auth=ado_client.auth)
+        request = ado_client.session.get(f"https://dev.azure.com/{ado_client.ado_org}/_pulls")
         raw_data = (
             request.text.split("application/json")[1].split('pullRequests"')[1].split("queries")[0].removeprefix(":").removesuffix(',"')
         )
         return [cls.from_request_payload(pr) for pr in json.loads(raw_data).values()]
 
     def get_comment_threads(self, ado_client: AdoClient, ignore_system_messages: bool = True) -> list[PullRequestCommentThread]:
-        request = requests.get(
+        request = ado_client.session.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo.repo_id}/pullRequests/{self.pull_request_id}/threads?api-version=7.1",
-            auth=ado_client.auth,
         ).json()["value"]
         comments = [PullRequestCommentThread.from_request_payload(data) for data in request]
         if ignore_system_messages:
             comments = [comment for comment in comments if comment.comments[0].comment_type != "system"]
         return comments
 
     def get_comments(self, ado_client: AdoClient, ignore_system_messages: bool = True) -> list[PullRequestComment]:
         """Gets a list of comments on a pull request, optionally ignoring system messages."""
         return [comment for thread in self.get_comment_threads(ado_client, ignore_system_messages) for comment in thread.comments]
 
     def post_comment(self, ado_client: AdoClient, content: str) -> PullRequestComment:
-        payload = {"comments": [{"commentType": 1, "content": content}], "status": "1"}
-        request = requests.post(
+        request = ado_client.session.post(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo.repo_id}/pullRequests/{self.pull_request_id}/threads?api-version=7.1",
-            json=payload,
-            auth=ado_client.auth,
+            json={"comments": [{"commentType": 1, "content": content}], "status": "1"},
         ).json()
         return PullRequestComment.from_request_payload(request["comments"][0])
 
 
 @dataclass
 class PullRequestCommentThread(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/pull-request-thread-comments/list?view=azure-devops-rest-7.1
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/releases.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/releases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from datetime import datetime
 from dataclasses import dataclass, field
 from typing import Any, Literal, TYPE_CHECKING
 
-import requests
-
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.utils import from_ado_date_string
 from ado_wrapper.resources.users import Member
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
@@ -222,17 +220,16 @@
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_all_releases_for_definition(cls, ado_client: "AdoClient", definition_id: str) -> "list[Release]":
-        response = requests.get(
+        response = ado_client.session.get(
             f"https://vsrm.dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/release/releases?api-version=7.1&definitionId={definition_id}",
-            auth=ado_client.auth,
         ).json()
         return [Release.from_request_payload(release) for release in response["value"]]
 
     @classmethod
     def get_all(cls, ado_client: "AdoClient") -> "list[ReleaseDefinition]":  # type: ignore[override]
         return super().get_all(
             ado_client,
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/repo.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from typing import Any, Literal, TYPE_CHECKING
 
 import requests
 
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.pull_requests import PullRequest, PullRequestStatus
 from ado_wrapper.resources.commits import Commit
-from ado_wrapper.resources.merge_policies import MergePolicies, MergeBranchPolicy
+from ado_wrapper.resources.merge_policies import MergePolicies
 from ado_wrapper.utils import ResourceNotFound, UnknownError
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
+    from ado_wrapper.resources.merge_policies import MergeBranchPolicy
 
 RepoEditableAttribute = Literal["name", "default_branch", "is_disabled"]
 WhenChangesArePushed = Literal["require_revote_on_each_iteration", "require_revote_on_last_iteration", "reset_votes_on_source_push", "reset_rejections_on_source_push", "do_nothing"]
 # ====================================================================
 
 
 @dataclass
@@ -91,32 +92,30 @@
     def get_by_name(cls, ado_client: AdoClient, repo_name: str) -> "Repo | None":  # type: ignore[return]
         """Warning, this function must fetch `all` repos to work, be cautious when calling it in a loop."""
         for repo in cls.get_all(ado_client):
             if repo.name == repo_name:
                 return repo
 
     def get_file(self, ado_client: AdoClient, file_path: str, branch_name: str = "main") -> str:
-        request = requests.get(
+        request = ado_client.session.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?path={file_path}&versionType={'Branch'}&version={branch_name}&api-version=7.1",
-            auth=ado_client.auth,
         )
         if request.status_code == 404:
             raise ResourceNotFound(f"File {file_path} not found in repo {self.repo_id}")
         if request.status_code != 200:
             raise UnknownError(f"Error getting file {file_path} from repo {self.repo_id}: {request.text}")
         return request.text  # This is the file content
 
     def get_contents(self, ado_client: AdoClient, file_types: list[str] | None = None, branch_name: str = "main") -> dict[str, str]:
         """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/items/get?view=azure-devops-rest-7.1&tabs=HTTP
         This function downloads the contents of a repo, and returns a dictionary of the files and their contents
         The file_types parameter is a list of file types to filter for, e.g. ["json", "yaml"]"""
         try:
-            request = requests.get(
+            request = ado_client.session.get(
                 f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?recursionLevel={'Full'}&download={True}&$format={'Zip'}&versionDescriptor.version={branch_name}&api-version=7.1",
-                auth=ado_client.auth,
             )
         except requests.exceptions.ConnectionError:
             print(f"=== Connection error, failed to download {self.repo_id}")
             return {}
         if request.status_code != 200:
             print(f"Error getting repo contents for {self.name} ({self.repo_id}):", request.text)
             return {}
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/service_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Any, Literal, TYPE_CHECKING
 
-import requests
-
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import Member
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 ServiceEndpointEditableAttribute = Literal["name"]
@@ -119,11 +117,11 @@
         https://learn.microsoft.com/en-us/rest/api/azure/devops/approvalsandchecks/pipeline-permissions/update-pipeline-permisions-for-resources?view=azure-devops-rest-7.1
         """
         PAYLOAD = {
             "resource": {"id": self.service_endpoint_id, "type": "endpoint", "name": ""},
             "pipelines": [] if pipeline_id == "all" else [{"id": pipeline_id}],
             "allPipelines": {"authorized": True, "authorizedBy": "null", "authorizedOn": "null"},
         }
-        return requests.patch(  # type: ignore[no-any-return]
+        return ado_client.session.patch(  # type: ignore[no-any-return]
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/pipelines/pipelinePermissions/endpoint/{self.service_endpoint_id}?api-version=7.1",
-            json=PAYLOAD, auth=ado_client.auth,  # fmt: skip
+            json=PAYLOAD,
         ).json()
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/teams.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/teams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from dataclasses import dataclass, field
 
-import requests
-
 from ado_wrapper.state_managed_abc import StateManagedResource
 from ado_wrapper.resources.users import TeamMember
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 
@@ -37,15 +35,15 @@
         )  # type: ignore[assignment]
         resource.team_members = resource.get_members(ado_client)
         return resource
 
     @classmethod
     def create(cls, ado_client: AdoClient, name: str, description: str) -> "Team":  # type: ignore[override]
         raise NotImplementedError
-        # request = requests.post(f"/_apis/teams?api-version=7.1", json={"name": name, "description": description}, auth=ado_client.auth).json()
+        # request = ado_client.session.post(f"/_apis/teams?api-version=7.1", json={"name": name, "description": description}).json()
         # return cls.from_request_payload(request)
 
     def update(self, ado_client: AdoClient, attribute_name: str, attribute_value: str) -> None:  # type: ignore[override]
         raise NotImplementedError
 
     @classmethod
     def delete_by_id(cls, ado_client: AdoClient, team_id: str) -> None:  # type: ignore[override]
@@ -63,17 +61,16 @@
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_by_name(cls, ado_client: AdoClient, team_name: str) -> "Team | None":
         return cls.get_by_abstract_filter(ado_client, lambda team: team.name == team_name)  # type: ignore[return-value, attr-defined]
 
     def get_members(self, ado_client: AdoClient) -> list["TeamMember"]:
-        request = requests.get(
+        request = ado_client.session.get(
             f"https://dev.azure.com/{ado_client.ado_org}/_apis/projects/{ado_client.ado_project}/teams/{self.team_id}/members?api-version=7.1-preview.2",
-            auth=ado_client.auth,
         ).json()
         if "value" not in request and request.get("message", "").startswith("The team with id "):  # If the team doesn't exist anymore.
             return []
         team_members = [TeamMember.from_request_payload(member) for member in request["value"]]
         self.team_members = team_members
         return team_members
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/users.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
     def get_by_email(cls, ado_client: AdoClient, member_email: str) -> "AdoUser":
         user: AdoUser = cls.get_by_abstract_filter(ado_client, lambda user: user.email == member_email)  # type: ignore[attr-defined, assignment]
-        if not user:
+        if user is None:
             raise ValueError(f"Member with email {member_email} not found")
         return user
 
     @classmethod
     def get_by_name(cls, ado_client: AdoClient, member_name: str) -> "AdoUser | None":
         return cls.get_by_abstract_filter(ado_client, lambda user: user.display_name == member_name)  # type: ignore[return-value, attr-defined]
 
@@ -86,20 +86,17 @@
 # ======================================================================================================= #
 
 
 @dataclass
 class Member(StateManagedResource):
     """A stripped down member class which is often returned by the API, for example in build requests."""
 
-    name: str  # Static
-    email: str  # Static
-    member_id: str  # Static
-
-    def __str__(self) -> str:
-        return f"{self.name} ({self.email})"
+    name: str
+    email: str
+    member_id: str = field(metadata={"is_id_field": True}, repr=False)
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "Member":
         # displayName, uniqueName/mailAddress, id/originId
         # This gets returned slightly differently from different APIs
         return cls(data["displayName"], data.get("uniqueName") or data.get("mailAddress", "UNKNOWN"),  # type: ignore[arg-type]
                    data.get("id") or data["originId"])  # fmt: skip
@@ -129,15 +126,15 @@
         super().__init__(name, email, member_id)
         self.is_team_admin = is_team_admin  # Static
 
     def __str__(self) -> str:
         return f"{super().__str__()}" + (" (Team Admin)" if self.is_team_admin else "")
 
     def __repr__(self) -> str:
-        return f"{super().__str__()[:-1]}, team_admin={self.is_team_admin})"
+        return f"{super().__str__().removesuffix(')')}, team_admin={self.is_team_admin})"
 
     @classmethod
     def from_json(cls, data: dict[str, Any]) -> "TeamMember":
         return cls(data["name"], data["email"], data["id"], data["is_team_admin"])
 
     def to_json(self) -> dict[str, Any]:
         return {
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-0.0.8/ado_wrapper/resources/variable_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,14 @@
     description: str  # = field(metadata={"editable": True})  # Bug in the api means this is not editable (it never returns or sets description)
     variables: dict[str, str] = field(metadata={"editable": True})
     created_on: datetime
     created_by: Member
     modified_by: Member
     modified_on: datetime | None = None
 
-    def __str__(self) -> str:
-        return repr(self)
-
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "VariableGroup":
         created_by = Member.from_request_payload(data["createdBy"])
         modified_by = Member.from_request_payload(data["modifiedBy"])
         return cls(str(data["id"]), data["name"], data.get("description", ""),
                    {key: value["value"] if isinstance(value, dict) else value for key, value in data["variables"].items()},
                    from_ado_date_string(data["createdOn"]), created_by, modified_by, from_ado_date_string(data.get("modifiedOn")))  # fmt: skip
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/state_managed_abc.py` & `ado_wrapper-0.0.8/ado_wrapper/state_managed_abc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from typing import Any, TYPE_CHECKING, Literal, Callable
 from dataclasses import dataclass, fields
 from datetime import datetime
 
-import requests
-
 from ado_wrapper.utils import (
     get_resource_variables, extract_id, get_internal_field_names,
     ResourceAlreadyExists, DeletionFailed, ResourceNotFound, UpdateFailed,  # fmt: skip
 )
 from ado_wrapper.plan_resources.plan_resource import PlannedStateManagedResource
 
 if TYPE_CHECKING:
@@ -64,15 +62,15 @@
     def get_by_id(cls, ado_client: "AdoClient", resource_id: str) -> "StateManagedResource":
         raise NotImplementedError
 
     @classmethod
     def get_by_url(cls, ado_client: "AdoClient", url: str) -> "StateManagedResource":
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}{url}"
-        request = requests.get(url, auth=ado_client.auth)
+        request = ado_client.session.get(url)
         if request.status_code == 404:
             raise ResourceNotFound(f"No {cls.__name__} found with that identifier!")
         if request.status_code >= 300:
             raise ValueError(f"Error getting {cls.__name__} by id: {request.text}")
         if "value" in request.json():
             return cls.from_request_payload(request.json()["value"][0])
         return cls.from_request_payload(request.json())
@@ -81,29 +79,29 @@
     def create(
         cls, ado_client: "AdoClient", url: str, payload: dict[str, Any] | None = None
     ) -> "StateManagedResource | PlannedStateManagedResource":
         if ado_client.plan_mode:
             return PlannedStateManagedResource.create(cls, ado_client, url, payload)
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}" + url
-        request = requests.post(url, json=payload or {}, auth=ado_client.auth)  # Create a brand new dict
+        request = ado_client.session.post(url, json=payload or {})  # Create a brand new dict
         if request.status_code == 401:
             raise PermissionError(f"You do not have permission to create this {cls.__name__}!")
         if request.status_code == 409:
             raise ResourceAlreadyExists(f"The {cls.__name__} with that identifier already exist!")
         resource = cls.from_request_payload(request.json())
         ado_client.state_manager.add_resource_to_state(cls.__name__, extract_id(resource), resource.to_json())  # type: ignore[arg-type]
         return resource
 
     @classmethod
     def delete_by_id(cls, ado_client: "AdoClient", url: str, resource_id: str) -> None:
         """Deletes an object by its id. The id is passed so it can be removed from state"""
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}{url}"
-        request = requests.delete(url, auth=ado_client.auth)
+        request = ado_client.session.delete(url)
         if request.status_code != 204:
             if request.status_code == 404:
                 print("[ADO_WRAPPER] Resource not found, probably already deleted, removing from state")
             else:
                 raise DeletionFailed(f"[ADO_WRAPPER] Error deleting {cls.__name__} ({resource_id}): {request.json()['message']}")
         ado_client.state_manager.remove_resource_from_state(cls.__name__, resource_id)  # type: ignore[arg-type]
 
@@ -119,27 +117,27 @@
         params |= {interal_names[attribute_name]: attribute_value}
 
         if ado_client.plan_mode:
             return PlannedStateManagedResource.update(self, ado_client, url, attribute_name, attribute_value, params)
 
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}{url}"
-        request = requests.request(update_action, url, json=params, auth=ado_client.auth)
+        request = ado_client.session.request(update_action, url, json=params)
         if request.status_code != 200:
             raise UpdateFailed(
                 f"Failed to update {self.__class__.__name__} with id {extract_id(self)} and attribute {attribute_name} to {attribute_value}. \nReason:\n{request.text}"
             )
         setattr(self, attribute_name, attribute_value)
         ado_client.state_manager.update_resource_in_state(self.__class__.__name__, extract_id(self), self.to_json())  # type: ignore[arg-type]
 
     @classmethod
     def get_all(cls, ado_client: "AdoClient", url: str) -> list["StateManagedResource"]:
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}{url}"
-        request = requests.get(url, auth=ado_client.auth)
+        request = ado_client.session.get(url)
         if request.status_code >= 300:
             raise ValueError(f"Error getting all {cls.__name__}: {request.text}")
         return [cls.from_request_payload(resource) for resource in request.json()["value"]]
 
     @classmethod
     def get_by_abstract_filter(
         cls, ado_client: "AdoClient", func: Callable[["StateManagedResource"], bool]
```

### Comparing `ado_wrapper-0.0.7/ado_wrapper/state_manager.py` & `ado_wrapper-0.0.8/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.7/ado_wrapper/utils.py` & `ado_wrapper-0.0.8/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.7/pyproject.toml` & `ado_wrapper-0.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "0.0.7"
+version = "0.0.8"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
 
@@ -45,14 +45,15 @@
     "missing-function-docstring",
     "missing-timeout",
 
     "too-few-public-methods",
     "too-many-instance-attributes",
     "too-many-arguments",
 
+    "duplicate-code",
     "unused-argument",
     "fixme",
     "arguments-differ",
     "arguments-renamed",
     "invalid-name",
     "too-many-locals",
     "line-too-long",
```

### Comparing `ado_wrapper-0.0.7/PKG-INFO` & `ado_wrapper-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 0.0.7
+Version: 0.0.8
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


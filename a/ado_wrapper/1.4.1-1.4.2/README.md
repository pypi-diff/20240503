# Comparing `tmp/ado_wrapper-1.4.1.tar.gz` & `tmp/ado_wrapper-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.4.1.tar", max compression
+gzip compressed data, was "ado_wrapper-1.4.2.tar", max compression
```

## Comparing `ado_wrapper-1.4.1.tar` & `ado_wrapper-1.4.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.4.1/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.4.1/README.md
--rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.4.1/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.4.1/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2187 2024-04-21 14:56:46.791867 ado_wrapper-1.4.1/ado_wrapper/client.py
--rw-r--r--   0        0        0    25691 2024-04-21 11:28:27.535399 ado_wrapper-1.4.1/ado_wrapper/dumps.py
--rw-r--r--   0        0        0     3378 2024-05-02 10:50:48.977836 ado_wrapper-1.4.1/ado_wrapper/generate_docs.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.4.1/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.4.1/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.4.1/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.4.1/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.4.1/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.4.1/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0     1026 2024-04-29 12:13:21.212309 ado_wrapper-1.4.1/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.4.1/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.4.1/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    14817 2024-05-02 10:36:23.066153 ado_wrapper-1.4.1/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6583 2024-04-21 14:56:46.795412 ado_wrapper-1.4.1/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.4.1/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3308 2024-04-21 14:56:46.796388 ado_wrapper-1.4.1/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    15274 2024-04-29 10:16:27.641099 ado_wrapper-1.4.1/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.4.1/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    13959 2024-04-21 14:56:46.797627 ado_wrapper-1.4.1/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.4.1/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10226 2024-04-22 10:44:14.335216 ado_wrapper-1.4.1/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.4.1/ado_wrapper/resources/searches.py
--rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.4.1/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.4.1/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8295 2024-04-21 14:56:46.799706 ado_wrapper-1.4.1/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.4.1/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     9380 2024-04-23 09:03:14.872165 ado_wrapper-1.4.1/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     7881 2024-04-23 11:05:52.742242 ado_wrapper-1.4.1/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4782 2024-04-23 08:38:52.967534 ado_wrapper-1.4.1/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2760 2024-05-02 10:50:36.784127 ado_wrapper-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.4.2/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.4.2/README.md
+-rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.4.2/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.4.2/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2187 2024-04-21 14:56:46.791867 ado_wrapper-1.4.2/ado_wrapper/client.py
+-rw-r--r--   0        0        0    25691 2024-04-21 11:28:27.535399 ado_wrapper-1.4.2/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0     3378 2024-05-02 10:50:48.977836 ado_wrapper-1.4.2/ado_wrapper/generate_docs.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.4.2/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.4.2/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.4.2/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.4.2/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.4.2/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.4.2/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0     1082 2024-05-02 12:12:40.876620 ado_wrapper-1.4.2/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3710 2024-05-02 12:34:44.409220 ado_wrapper-1.4.2/ado_wrapper/resources/agent_pools.py
+-rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.4.2/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.4.2/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    14817 2024-05-02 10:36:23.066153 ado_wrapper-1.4.2/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.4.2/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.4.2/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3308 2024-04-21 14:56:46.796388 ado_wrapper-1.4.2/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    15274 2024-04-29 10:16:27.641099 ado_wrapper-1.4.2/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.4.2/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    13959 2024-04-21 14:56:46.797627 ado_wrapper-1.4.2/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.4.2/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10226 2024-04-22 10:44:14.335216 ado_wrapper-1.4.2/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.4.2/ado_wrapper/resources/searches.py
+-rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.4.2/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.4.2/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8295 2024-04-21 14:56:46.799706 ado_wrapper-1.4.2/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.4.2/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     9380 2024-04-23 09:03:14.872165 ado_wrapper-1.4.2/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     7881 2024-04-23 11:05:52.742242 ado_wrapper-1.4.2/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4806 2024-05-02 12:13:10.282768 ado_wrapper-1.4.2/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2760 2024-05-03 16:39:50.466961 ado_wrapper-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.4.2/PKG-INFO
```

### Comparing `ado_wrapper-1.4.1/LICENSE` & `ado_wrapper-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/README.md` & `ado_wrapper-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/__main__.py` & `ado_wrapper-1.4.2/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/client.py` & `ado_wrapper-1.4.2/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/dumps.py` & `ado_wrapper-1.4.2/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/generate_docs.py` & `ado_wrapper-1.4.2/ado_wrapper/generate_docs.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.4.2/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.4.2/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.4.2/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ado_wrapper.resources.agent_pools import AgentPool
 from ado_wrapper.resources.annotated_tags import AnnotatedTag
 from ado_wrapper.resources.branches import Branch
 from ado_wrapper.resources.builds import Build, BuildDefinition
 from ado_wrapper.resources.commits import Commit
 from ado_wrapper.resources.environment import Environment, PipelineAuthorisation
 from ado_wrapper.resources.groups import Group
 from ado_wrapper.resources.merge_policies import (
```

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/annotated_tags.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/branches.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/builds.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/builds.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/commits.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/commits.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     message: str
 
     def __str__(self) -> str:
         return f"{self.commit_id} by {self.author!s} on {self.date}\n{self.message}"
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "Commit":
-        member = Member(data["author"]["name"], data["author"]["email"], "UNKNOWN")
+        member = Member(data["author"]["name"], data["author"].get("email", "BOT USER"), "UNKNOWN")
         return cls(data["commitId"], member, from_ado_date_string(data["author"]["date"]), data["comment"])
 
     @classmethod
     def get_by_id(cls, ado_client: "AdoClient", repo_id: str, commit_id: str) -> "Commit":  # type: ignore[override]
         return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/commits/{commit_id}?api-version=7.1",
@@ -79,15 +79,18 @@
             from_branch_name.startswith("refs/heads/") or to_branch_name.startswith("refs/heads/")
         ), "Branch names should not start with 'refs/heads/'"
         if not updates:
             raise ValueError("No updates provided! It's not possible to create a commit without updates.")
         latest_commit = cls.get_latest_by_repo(ado_client, repo_id, from_branch_name)
         latest_commit_id = None if latest_commit is None else latest_commit.commit_id
         data = get_commit_body_template(latest_commit_id, updates, to_branch_name, change_type, commit_message)
-        request = ado_client.session.post(f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pushes?api-version=7.1", json=data)  # fmt: skip
+        request = ado_client.session.post(
+            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{repo_id}/pushes?api-version=7.1",
+            json=data,
+        )
         if request.status_code == 400:
             raise ValueError("The commit was not created successfully, the file(s) you're trying to add might already exist there.")
         if request.status_code == 403:
             raise InvalidPermissionsError("You do not have permission to create a commit in this repo (possibly due to main branch protections)")  # fmt: skip
         if not request.json().get("commits"):
             raise ValueError("The commit was not created successfully.\nError:", request.json())
         return cls.from_request_payload(request.json()["commits"][-1])
```

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/environment.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/environment.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/groups.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/merge_policies.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/projects.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/releases.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/repo.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/searches.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/searches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/teams.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/users.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/users.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.4.2/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.4.2/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/state_manager.py` & `ado_wrapper-1.4.2/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.4.1/ado_wrapper/utils.py` & `ado_wrapper-1.4.2/ado_wrapper/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,20 +131,20 @@
             "The client has not been initialised. Please disable `bypass_initialisation` in AdoClient before using this function."
         )
 
 
 def get_resource_variables() -> dict[str, type["StateManagedResource"]]:  # We do this to avoid circular imports
     """This returns a mapping of resource name (str) to the class type of the resource. This is used to dynamically create instances of resources."""
     from ado_wrapper.resources import (  # type: ignore[attr-defined]  # pylint: disable=possibly-unused-variable
-        AnnotatedTag, Branch, Build, BuildDefinition, Commit, Environment, Group, MergePolicies, MergeBranchPolicy,
+        AgentPool, AnnotatedTag, Branch, Build, BuildDefinition, Commit, Environment, Group, MergePolicies, MergeBranchPolicy,
         MergePolicyDefaultReviewer, Project, PullRequest, Release, ReleaseDefinition, Repo, BuildRepository, Team,
         AdoUser, Member, ServiceEndpoint, Reviewer, VariableGroup,  # fmt: skip
     )
 
     return locals()
 
 
 ResourceType = Literal[
-    "AnnotatedTag", "Branch", "Build", "BuildDefinition", "Commit", "Environment", "Group", "MergePolicies", "MergeBranchPolicy",
+    "AgentPool", "AnnotatedTag", "Branch", "Build", "BuildDefinition", "Commit", "Environment", "Group", "MergePolicies", "MergeBranchPolicy",
     "MergePolicyDefaultReviewer", "Project", "PullRequest", "Release", "ReleaseDefinition",
     "Repo", "Team", "AdoUser", "Member", "ServiceEndpoint", "Reviewer", "VariableGroup"  # fmt: skip
 ]
```

### Comparing `ado_wrapper-1.4.1/pyproject.toml` & `ado_wrapper-1.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "1.4.1"
+version = "1.4.2"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-1.4.1/PKG-INFO` & `ado_wrapper-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.4.1
+Version: 1.4.2
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


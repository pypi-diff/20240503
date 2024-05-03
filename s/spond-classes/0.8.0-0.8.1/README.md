# Comparing `tmp/spond_classes-0.8.0.tar.gz` & `tmp/spond_classes-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spond_classes-0.8.0.tar", max compression
+gzip compressed data, was "spond_classes-0.8.1.tar", max compression
```

## Comparing `spond_classes-0.8.0.tar` & `spond_classes-0.8.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1084 2023-11-25 18:32:05.774061 spond_classes-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0    35823 2023-11-25 14:36:46.887184 spond_classes-0.8.0/LICENSE
--rw-r--r--   0        0        0     2642 2023-11-25 18:21:02.894208 spond_classes-0.8.0/README.md
--rw-r--r--   0        0        0     1423 2023-11-25 18:32:05.774061 spond_classes-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      376 2023-11-25 14:36:46.897184 spond_classes-0.8.0/spond_classes/__init__.py
--rw-r--r--   0        0        0     3266 2023-11-25 17:42:47.704712 spond_classes-0.8.0/spond_classes/event.py
--rw-r--r--   0        0        0     5368 2023-11-25 14:36:46.897184 spond_classes-0.8.0/spond_classes/group.py
--rw-r--r--   0        0        0     3451 2023-11-25 18:32:05.764061 spond_classes-0.8.0/spond_classes/member.py
--rw-r--r--   0        0        0        0 2023-11-25 14:36:46.897184 spond_classes-0.8.0/spond_classes/py.typed
--rw-r--r--   0        0        0     1455 2023-11-25 14:36:46.897184 spond_classes-0.8.0/spond_classes/role.py
--rw-r--r--   0        0        0     1451 2023-11-25 14:36:46.907184 spond_classes-0.8.0/spond_classes/subgroup.py
--rw-r--r--   0        0        0     3500 1970-01-01 00:00:00.000000 spond_classes-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1742 2024-05-03 18:25:13.871587 spond_classes-0.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0    35823 2023-12-24 18:39:51.814809 spond_classes-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1633 2024-05-03 18:25:13.869583 spond_classes-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2762 2024-05-03 18:25:14.842922 spond_classes-0.8.1/README.md
+-rw-r--r--   0        0        0      336 2024-03-31 18:32:28.304420 spond_classes-0.8.1/spond_classes/__init__.py
+-rw-r--r--   0        0        0     3298 2024-05-03 18:18:33.548165 spond_classes-0.8.1/spond_classes/event.py
+-rw-r--r--   0        0        0     5186 2024-05-03 18:18:33.549165 spond_classes-0.8.1/spond_classes/group.py
+-rw-r--r--   0        0        0     3331 2024-05-03 18:18:33.549165 spond_classes-0.8.1/spond_classes/member.py
+-rw-r--r--   0        0        0        0 2023-12-24 18:39:51.816809 spond_classes-0.8.1/spond_classes/py.typed
+-rw-r--r--   0        0        0     1492 2024-05-03 18:18:33.549165 spond_classes-0.8.1/spond_classes/role.py
+-rw-r--r--   0        0        0     1476 2024-05-03 18:18:33.550165 spond_classes-0.8.1/spond_classes/subgroup.py
+-rw-r--r--   0        0        0     3499 1970-01-01 00:00:00.000000 spond_classes-0.8.1/PKG-INFO
```

### Comparing `spond_classes-0.8.0/LICENSE` & `spond_classes-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spond_classes-0.8.0/README.md` & `spond_classes-0.8.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,122 +1,121 @@
-# Spond-classes
-
-## About
-
-[Spond](https://spond.com/welcome) is a team/group-oriented events system.
-
-The unofficial Python [`spond` library package](https://github.com/Olen/Spond/) gets
-data from the Spond API and returns `dict` objects.
-
-This unofficial Python `spond-classes` package parses those `dict` objects to create
-class instances, i.e. provides an object abstraction layer.
-
-Experimental, very partial, read-only implementation.
-
-## Install
-
-Install from PyPI, e.g:
-`
-pip install spond-classes
-`
-Or if you're using Poetry:
-`
-poetry add spond-classes
-`
-
-## Key features
-
-* Create `Group` class instance from the dict returned by the corresponding `spond`
-  method:
-
-```
-spond_classes.Group.from_dict()
-```
-
-* Then access class instance attributes and methods:
-
-```
-Group.uid: str
-Group.name: str
-Group.members: List[Member]
-Group.member_by_id() -> Member
-Group.roles: List[SpondRoles]
-Group.role_by_id() -> Role
-Group.subgroups: List[Subgroup]
-Group.subgroup_by_id() -> Subgroup
-```
-
-* Also provides access to child `Member`, `Role`, `Subgroup` instances:
-
-```
-Member.uid: str
-Member.created_time: datetime
-Member.first_name: str
-Member.last_name: str
-Member.full_name: str
-Member.phone_number: str
-Member.profile_uid: str
-Member.roles: List[Role]
-Member.subgroups: List[Subgroup]
-
-Role.uid: str
-Role.members: List[Member]
-Role.name: str
-
-Subgroup.uid: str
-Subgroup.members: List[Member]
-Subgroup.name: str
-```
-
-* Create `Event` class instance from the dict returned by the corresponding `Spond`
-  method:
-
-```
-spond_classes.Event.from_dict()
-```
-
-* Then access attributes:
-
-```
-Event.uid: str
-Event.heading: str
-Event.start_time: datetime
-Event.accepted_uids: list
-Event.declined_uids: list
-Event.unanswered_uids: list
-Event.waiting_list_uids: list
-Event.unconfirmed_uids: list
-```
-
-It's also possible to create `Member.from_dict()`, `Role.from_dict()`,
-`Subgroup.from_dict()`.
-
-## Example code
-
-Adapting the example code in [`Spond`](https://github.com/Olen/Spond/) README:
-
-```
-import asyncio
-from spond import spond
-import spond_classes
-
-username = 'my@mail.invalid'
-password = 'Pa55worD'
-group_id = 'C9DC791FFE63D7914D6952BE10D97B46'  # fake
-
-async def main():
-    s = spond.Spond(username=username, password=password)
-    group_data = await s.get_group(group_id)
-    await s.clientsession.close()
-
-    # Now we can create a class instance ...
-    group = spond_classes.Group.from_dict(group_data)
-
-    # ... use class properties instead of dict keys ...
-    print(group.name)
-
-    # ... and access child instances and their properties
-    for member in group.members:
-        print(member.full_name)
-
-asyncio.run(main())
-```
+# Spond-classes
+
+## About
+
+[Spond](https://spond.com/welcome) is a team/group-oriented events system.
+
+The unofficial Python [`spond` library package](https://github.com/Olen/Spond/) gets
+data from the Spond API and returns `dict` objects.
+
+This unofficial Python `spond-classes` package parses those `dict` objects to create
+class instances, i.e. provides an object abstraction layer.
+
+Experimental, very partial, read-only implementation.
+
+## Install
+
+Install from PyPI, e.g:
+`
+pip install spond-classes
+`
+Or if you're using Poetry:
+`
+poetry add spond-classes
+`
+
+## Example code
+
+Adapting the example code in [`Spond`](https://github.com/Olen/Spond/) README:
+
+```
+import asyncio
+from spond import spond
+import spond_classes
+
+username = 'my@mail.invalid'
+password = 'Pa55worD'
+group_id = 'C9DC791FFE63D7914D6952BE10D97B46'  # fake
+
+async def main():
+    s = spond.Spond(username=username, password=password)
+    group_data = await s.get_group(group_id)
+    await s.clientsession.close()
+
+    # Now we can create a class instance ...
+    group = spond_classes.Group.from_dict(group_data)
+
+    # ... use class properties instead of dict keys ...
+    print(group.name)
+
+    # ... and access child instances and their properties
+    for member in group.members:
+        print(member.full_name)
+
+asyncio.run(main())
+```
+## Key features
+
+* Create `Group` class instance from the dict returned by the corresponding `spond`
+  method:
+
+```
+spond_classes.Group.from_dict()
+```
+
+* Then access class instance attributes and methods:
+
+```
+Group.uid: str
+Group.name: str
+Group.members: List[Member]
+Group.member_by_id() -> Member
+Group.roles: List[SpondRoles]
+Group.role_by_id() -> Role
+Group.subgroups: List[Subgroup]
+Group.subgroup_by_id() -> Subgroup
+```
+
+* Also provides access to child `Member`, `Role`, `Subgroup` instances:
+
+```
+Member.uid: str
+Member.created_time: datetime
+Member.first_name: str
+Member.last_name: str
+Member.full_name: str
+Member.phone_number: str
+Member.profile_uid: str
+Member.roles: List[Role]
+Member.subgroups: List[Subgroup]
+
+Role.uid: str
+Role.members: List[Member]
+Role.name: str
+
+Subgroup.uid: str
+Subgroup.members: List[Member]
+Subgroup.name: str
+```
+
+* Create `Event` class instance from the dict returned by the corresponding `Spond`
+  method:
+
+```
+spond_classes.Event.from_dict()
+```
+
+* Then access attributes:
+
+```
+Event.uid: str
+Event.heading: str
+Event.start_time: datetime
+Event.accepted_uids: list
+Event.declined_uids: list
+Event.unanswered_uids: list
+Event.waiting_list_uids: list
+Event.unconfirmed_uids: list
+```
+
+It's also possible to create `Member.from_dict()`, `Role.from_dict()`,
+`Subgroup.from_dict()`.
```

### Comparing `spond_classes-0.8.0/pyproject.toml` & `spond_classes-0.8.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,59 @@
-[tool.poetry]
-name = "spond-classes"
-version = "0.8.0"
-description = "Experimental Python class abstraction layer for `spond` package."
-authors = ["elliot-100 <3186037+elliot-100@users.noreply.github.com>"]
-readme = "README.md"
-homepage = "https://github.com/elliot-100/Spond-classes"
-repository = "https://github.com/elliot-100/Spond-classes"
-packages = [{include = "spond_classes"}]
-include = ["CHANGELOG.md"]
-license = "GPL 3.0"
-
-[tool.poetry.dependencies]
-python = "^3.8"
-python-dateutil = "^2.8.2"
-spond = "^0.99.1"
-
-[tool.poetry.group.dev.dependencies]
-black = "^23.11.0"
-isort = "^5.11.4"
-pre-commit = "^3.1.1"
-ruff = "^0.1.6"
-
-[tool.poetry.group.test.dependencies]
-mypy = "^1.7.1"
-pytest = "^7.4.3"
-types-python-dateutil = "^2.8.19.14"
-
-[tool.black]
-line-length = 88
-target-version = ['py38']
-
-[tool.isort]
-profile = "black"
-
-[tool.mypy]
-warn_unused_configs = true
-strict = true
-disallow_any_generics = false
-
-[tool.ruff]
-# Enable rulesets:
-# flake8-ANNotations, flake8-COMmas, pyDocstyle, pycodestylE, pyFlakes,
-# flake8-Future-Annotations, flake8-bandit (S)
-select = ["ANN", "COM", "D", "E", "F", "FA", "S"]
-
-# Ignore rules:
-#  Missing type annotation for `self` in method
-ignore = ["ANN101"]
-
-[tool.ruff.per-file-ignores]
-# Use of `assert` detected
-"**/{tests}/*" = ["S101"]
-
-[tool.ruff.pydocstyle]
-convention = "numpy"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "spond-classes"
+version = "0.8.1"
+description = "Experimental Python class abstraction layer for `spond` package."
+authors = ["elliot-100 <3186037+elliot-100@users.noreply.github.com>"]
+readme = "README.md"
+homepage = "https://github.com/elliot-100/Spond-classes"
+repository = "https://github.com/elliot-100/Spond-classes"
+packages = [{include = "spond_classes"}]
+include = ["CHANGELOG.md"]
+license = "GPL 3.0"
+
+[tool.poetry.dependencies]
+python = "^3.8"
+python-dateutil = "^2.8.2"
+spond = "^0.99.1"
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^3.1.1"
+ruff = "^0.4.2"
+
+[tool.poetry.group.test.dependencies]
+mypy = "^1.8.0"
+pytest = "^8.1.1"
+types-python-dateutil = "^2.8.19.14"
+
+[tool.mypy]
+warn_unused_configs = true
+strict = true
+disallow_any_generics = false
+
+[tool.ruff.lint]
+select = ["ALL"]
+
+# Ignore rules that conflict with Ruff formatter:
+#   COM812 Trailing comma missing
+
+# Ignore other rules:
+#   ANN101 Missing type annotation for `self` in method
+#   ANN102 Missing type annotation for `cls` in classmethod
+#   D205 1 blank line required between summary line and description
+
+ignore = ["COM812", "ANN101", "ANN102", "D205"]
+
+[tool.ruff.lint.per-file-ignores]
+# Ignore rules that aren't relevant in tests:
+#   S101 Use of assert detected
+"**/{tests}/*" = ["S101"]
+
+# Ignore rules that conflict with Mypy
+#   PLC0414 Import alias does not rename original package
+"__init__.py" = ["PLC0414"]
+
+[tool.ruff.lint.pydocstyle]
+convention = "numpy"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `spond_classes-0.8.0/spond_classes/event.py` & `spond_classes-0.8.1/spond_classes/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Event class."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING
 
 from dateutil import parser
+from typing_extensions import Self
 
 if TYPE_CHECKING:
     from datetime import datetime
 
 
 @dataclass
 class Event:
@@ -49,16 +51,23 @@
     # Populated by `Event.from_dict()`, as they rely on full Event data:
     accepted_uids: list = field(default_factory=list, repr=False)
     declined_uids: list = field(default_factory=list, repr=False)
     unanswered_uids: list = field(default_factory=list, repr=False)
     waiting_list_uids: list = field(default_factory=list, repr=False)
     unconfirmed_uids: list = field(default_factory=list, repr=False)
 
-    @staticmethod
-    def from_dict(event_data: dict) -> Event:
+    def __str__(self) -> str:
+        """Return simple human-readable description.
+
+        Date is included because heading is unlikely to be unique.
+        """
+        return f"Event '{self.heading}' on {self.start_time.date()}"
+
+    @classmethod
+    def from_dict(cls, event_data: dict) -> Self:
         """Create an Event object from relevant dict.
 
         Parameters
         ----------
         event_data
             Dict representing the event, as returned by `spond.get_event()`.
         """
@@ -71,24 +80,17 @@
             raise TypeError
         accepted_uids = event_data["responses"].get("acceptedIds", [])
         declined_uids = event_data["responses"].get("declinedIds", [])
         unanswered_uids = event_data["responses"].get("unansweredIds", [])
         waiting_list_uids = event_data["responses"].get("waitinglistIds", [])
         unconfirmed_uids = event_data["responses"].get("unconfirmedIds", [])
 
-        return Event(
+        return cls(
             uid,
             heading,
             start_time,
             accepted_uids,
             declined_uids,
             unanswered_uids,
             waiting_list_uids,
             unconfirmed_uids,
         )
-
-    def __str__(self: Event) -> str:
-        """Return simple human-readable description.
-
-        Date is included because heading is unlikely to be unique.
-        """
-        return f"Event '{self.heading}' on {self.start_time.date()}"
```

### Comparing `spond_classes-0.8.0/spond_classes/group.py` & `spond_classes-0.8.1/spond_classes/group.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Group class."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 
+from typing_extensions import Self
+
 from .member import Member
 from .role import Role
 from .subgroup import Subgroup
 
 
 @dataclass
 class Group:
@@ -44,114 +47,108 @@
     name: str
 
     # Populated by `Group.from_dict()`, as they rely on full Group data:
     members: list[Member] = field(default_factory=list, repr=False)
     roles: list[Role] = field(default_factory=list, repr=False)
     subgroups: list[Subgroup] = field(default_factory=list, repr=False)
 
-    def __str__(self: Group) -> str:
+    def __str__(self) -> str:
         """Return simple human-readable description."""
         return f"Group '{self.name}'"
 
-    @staticmethod
-    def core_from_dict(group_data: dict) -> Group:
+    @classmethod
+    def core_from_dict(cls, group_data: dict) -> Self:
         """Create a minimal Group object (required attributes only) from relevant dict.
 
         Parameters
         ----------
         group_data
             Dict representing the group, as returned by `spond.get_group()`.
         """
         if not isinstance(group_data, dict):
             raise TypeError
         uid = group_data["id"]
         name = group_data["name"]
-        return Group(uid, name)
+        return cls(uid, name)
 
-    @staticmethod
-    def from_dict(group_data: dict) -> Group:
+    @classmethod
+    def from_dict(cls, group_data: dict) -> Self:
         """Create a full-featured Group object and child objects from relevant dict.
 
         Parameters
         ----------
         group_data
             Dict representing the group, as returned by `spond.get_group()`.
         """
-        group = Group.core_from_dict(group_data)
+        group = cls.core_from_dict(group_data)
 
-        # create child SpondMembers
-        group.members = [
-            Member.from_dict(member_data)
-            for member_data in group_data.get("members", [])
-        ]
-        # create child SpondSubgroups
-        group.subgroups = [
-            Subgroup.from_dict(subgroup_data)
-            for subgroup_data in group_data.get("subGroups", [])
-        ]
-        # create child SpondRoles
-        group.roles = [Role.from_dict(role) for role in group_data.get("roles", [])]
+        group.members = Group._create_children(group_data, "members", Member)
+        group.subgroups = Group._create_children(group_data, "subGroups", Subgroup)
+        group.roles = Group._create_children(group_data, "roles", Role)
 
         for member_data in group_data.get("members", []):
             member_data_id = member_data.get("id")
+            member = group.member_by_id(member_data_id)
 
             for subgroup_data_id in member_data.get("subGroups", []):
-                # populate child SpondMembers' subgroup attributes
-                group.member_by_id(member_data_id).subgroups.append(
-                    group.subgroup_by_id(subgroup_data_id),
-                )
-                # populate child SpondSubgroups' members attribute
-                group.subgroup_by_id(subgroup_data_id).members.append(
-                    group.member_by_id(member_data_id),
-                )
+                subgroup = group.subgroup_by_id(subgroup_data_id)
+                # populate group.members.member.subgroups.subgroup
+                member.subgroups.append(subgroup)
+                # populate group.subgroups.subgroup.members.member
+                subgroup.members.append(member)
 
             for role_data_id in member_data.get("roles", []):
-                # populate child SpondMembers' roles attribute
-                group.member_by_id(member_data_id).roles.append(
-                    group.role_by_id(role_data_id),
-                )
-
-                # populate child SpondRoles' members attribute
-                group.role_by_id(role_data_id).members.append(
-                    group.member_by_id(member_data_id),
-                )
+                role = group.role_by_id(role_data_id)
+                # populate group.members.member.roles.role
+                member.roles.append(role)
+                # populate group.roles.role.members.member
+                role.members.append(member)
 
         return group
 
-    def subgroup_by_id(self: Group, subgroup_uid: str) -> Subgroup:
+    def subgroup_by_id(self, subgroup_uid: str) -> Subgroup:
         """Return the child Subgroup with matching id, or an error.
 
         Parameters
         ----------
         subgroup_uid
             ID of the subgroup.
         """
         for subgroup in self.subgroups:
             if subgroup.uid == subgroup_uid:
                 return subgroup
         raise IndexError
 
-    def member_by_id(self: Group, member_uid: str) -> Member:
+    def member_by_id(self, member_uid: str) -> Member:
         """Return the child Member with matching id, or an error.
 
         Parameters
         ----------
         member_uid
             ID of the member.
         """
         for member in self.members:
             if member.uid == member_uid:
                 return member
         raise IndexError
 
-    def role_by_id(self: Group, role_uid: str) -> Role:
+    def role_by_id(self, role_uid: str) -> Role:
         """Return the child Role with matching id, or an error.
 
         Parameters
         ----------
         role_uid
             ID of the role.
         """
         for role in self.roles:
             if role.uid == role_uid:
                 return role
         raise IndexError
+
+    @staticmethod
+    def _create_children(
+        group_data: dict,
+        key: str,
+        child_cls: type[Member | Role | Subgroup],
+    ) -> list:
+        """Create child objects."""
+        return [child_cls.from_dict(item) for item in group_data.get(key, [])]
```

### Comparing `spond_classes-0.8.0/spond_classes/member.py` & `spond_classes-0.8.1/spond_classes/member.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,122 +1,114 @@
-"""Member class."""
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING
-
-from dateutil import parser
-
-if TYPE_CHECKING:
-    from datetime import datetime
-
-    from .role import Role
-    from .subgroup import Subgroup
-
-
-@dataclass
-class Member:
-    """Represents a member in the Spond system.
-
-    A Member is an individual's record within a Group.
-
-    A Member belongs to one Group.
-    A Member has zero, one or more Roles.
-    NB: relationship to Events isn't yet implemented.
-
-    Attributes
-    ----------
-    uid : str
-        id of the Member.
-        'id' in API, but 'id' is a reserved term and the `spond` package uses `uid`.
-    created_time : datetime
-        Derived from 'createdTime' in API, but returns a datetime instead of a string.
-    email : str
-        'email' in API.
-    first_name : str
-        'firstName' in API.
-    last_name : str
-        'lastName' in API.
-    phone_number : str
-        'phoneNumber' in API.
-    profile_uid : str
-        `profile` -> `id` in API.
-    roles : list[Role]
-        The Member's Roles.
-        'roles' in API.
-    subgroups : list[Subgroup]
-        The Member's Subgroups.
-        Derived from 'subGroups' in API.
-    full_name : str
-        The Member's full name.
-        Provided for convenience.
-    """
-
-    # Populated by implicit Member.__init__().
-    uid: str
-    created_time: datetime
-    email: str | None
-    first_name: str
-    last_name: str
-    phone_number: str | None
-    profile_uid: str | None
-
-    # Populated by `Group.from_dict()`, as they rely on full Group data:
-    roles: list[Role] = field(default_factory=list)
-    subgroups: list[Subgroup] = field(default_factory=list)
-
-    def __repr__(self: Member) -> str:
-        """Return string representation."""
-        return (
-            f"Member(uid='{self.uid}', first_name='{self.first_name}', "
-            f"last_name='{self.last_name}')"
-        )
-
-    def __str__(self: Member) -> str:
-        """Return simple human-readable description.
-
-        Last few chars of uid are included because full name is unlikely to be unique.
-        """
-        return (
-            f"Member '{self.first_name} {self.last_name}' "
-            f"(uid ends '...{self.uid[-3:]}')"
-        )
-
-    @property
-    def full_name(self: Member) -> str:
-        """Return the member's full name."""
-        return f"{self.first_name} {self.last_name}"
-
-    @staticmethod
-    def from_dict(member_data: dict) -> Member:
-        """Create a Member object from relevant dict.
-
-        Parameters
-        ----------
-        member_data
-            Dict representing the member, as returned by `spond.get_person()`.
-        """
-        if not isinstance(member_data, dict):
-            raise TypeError
-        uid = member_data["id"]
-        created_time = parser.isoparse(member_data["createdTime"])
-        first_name = member_data["firstName"]
-        last_name = member_data["lastName"]
-
-        # Handle data that may be missing/private
-        email = member_data.get("email")
-        phone_number = member_data.get("phoneNumber")
-        profile = member_data.get("profile")
-        if profile:
-            profile_uid = profile["id"]
-        else:
-            profile_uid = None
-
-        return Member(
-            uid,
-            created_time,
-            email,
-            first_name,
-            last_name,
-            phone_number,
-            profile_uid,
-        )
+"""Member class."""
+
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING
+
+from dateutil import parser
+from typing_extensions import Self
+
+if TYPE_CHECKING:
+    from datetime import datetime
+
+    from .role import Role
+    from .subgroup import Subgroup
+
+
+@dataclass
+class Member:
+    """Represents a member in the Spond system.
+
+    A Member is an individual's record within a Group.
+
+    A Member belongs to one Group.
+    A Member has zero, one or more Roles.
+    NB: relationship to Events isn't yet implemented.
+
+    Attributes
+    ----------
+    uid : str
+        id of the Member.
+        'id' in API, but 'id' is a reserved term and the `spond` package uses `uid`.
+    created_time : datetime
+        Derived from 'createdTime' in API, but returns a datetime instead of a string.
+    email : str
+        'email' in API.
+    first_name : str
+        'firstName' in API.
+    last_name : str
+        'lastName' in API.
+    phone_number : str
+        'phoneNumber' in API.
+    profile_uid : str
+        `profile` -> `id` in API.
+    roles : list[Role]
+        The Member's Roles.
+        'roles' in API.
+    subgroups : list[Subgroup]
+        The Member's Subgroups.
+        Derived from 'subGroups' in API.
+    full_name : str
+        The Member's full name.
+        Provided for convenience.
+    """
+
+    # Populated by implicit Member.__init__().
+    uid: str
+    created_time: datetime
+    email: str | None
+    first_name: str
+    last_name: str
+    phone_number: str | None
+    profile_uid: str | None
+
+    # Populated by `Group.from_dict()`, as they rely on full Group data:
+    roles: list[Role] = field(default_factory=list, repr=False)
+    subgroups: list[Subgroup] = field(default_factory=list, repr=False)
+
+    def __str__(self) -> str:
+        """Return simple human-readable description.
+
+        Last few chars of uid are included because full name is unlikely to be unique.
+        """
+        return (
+            f"Member '{self.first_name} {self.last_name}' "
+            f"(uid ends '...{self.uid[-3:]}')"
+        )
+
+    @property
+    def full_name(self) -> str:
+        """Return the member's full name."""
+        return f"{self.first_name} {self.last_name}"
+
+    @classmethod
+    def from_dict(cls, member_data: dict) -> Self:
+        """Create a Member object from relevant dict.
+
+        Parameters
+        ----------
+        member_data
+            Dict representing the member, as returned by `spond.get_person()`.
+        """
+        if not isinstance(member_data, dict):
+            raise TypeError
+        uid = member_data["id"]
+        created_time = parser.isoparse(member_data["createdTime"])
+        first_name = member_data["firstName"]
+        last_name = member_data["lastName"]
+
+        # Handle data that may be missing/private
+        email = member_data.get("email")
+        phone_number = member_data.get("phoneNumber")
+        profile = member_data.get("profile")
+        profile_uid = profile["id"] if profile else None
+
+        return cls(
+            uid,
+            created_time,
+            email,
+            first_name,
+            last_name,
+            phone_number,
+            profile_uid,
+        )
```

### Comparing `spond_classes-0.8.0/spond_classes/role.py` & `spond_classes-0.8.1/spond_classes/role.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Role class."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING
 
+from typing_extensions import Self
+
 if TYPE_CHECKING:
     from .member import Member
 
 
 @dataclass
 class Role:
     """Represents a role in the Spond system.
@@ -30,29 +33,29 @@
     # Required params, populated by implicit Role.__init__().
     uid: str
     name: str
 
     # Populated by `Group.from_dict()`, as they rely on full Group data:
     members: list[Member] = field(default_factory=list, repr=False)
 
-    @staticmethod
-    def from_dict(role_data: dict) -> Role:
+    def __str__(self) -> str:
+        """Return simple human-readable description."""
+        return f"Role '{self.name}'"
+
+    @classmethod
+    def from_dict(cls, role_data: dict) -> Self:
         """Create a Role object from relevant dict.
 
         Parameters
         ----------
         role_data
             Dict representing the role.
         """
         if not isinstance(role_data, dict):
             raise TypeError
         uid = role_data["id"]
         name = role_data["name"]
 
-        return Role(
+        return cls(
             uid,
             name,
         )
-
-    def __str__(self: Role) -> str:
-        """Return simple human-readable description."""
-        return f"Role '{self.name}'"
```

### Comparing `spond_classes-0.8.0/spond_classes/subgroup.py` & `spond_classes-0.8.1/spond_classes/subgroup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Subgroup class."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING
 
+from typing_extensions import Self
+
 if TYPE_CHECKING:
     from .member import Member
 
 
 @dataclass
 class Subgroup:
     """Subgroup.
@@ -30,25 +33,25 @@
     # Required params, populated by implicit Subgroup.__init__().
     uid: str
     name: str
 
     # Populated by `Group.from_dict()`, as they rely on full Group data:
     members: list[Member] = field(default_factory=list, repr=False)
 
-    def __str__(self: Subgroup) -> str:
+    def __str__(self) -> str:
         """Return simple human-readable description."""
         return f"Subgroup '{self.name}'"
 
-    @staticmethod
-    def from_dict(subgroup_data: dict) -> Subgroup:
+    @classmethod
+    def from_dict(cls, subgroup_data: dict) -> Self:
         """Create a Subgroup object from relevant dict.
 
         Parameters
         ----------
         subgroup_data
             Dict representing the subgroup.
         """
         if not isinstance(subgroup_data, dict):
             raise TypeError
         uid = subgroup_data["id"]
         name = subgroup_data["name"]
-        return Subgroup(uid, name)
+        return cls(uid, name)
```

### Comparing `spond_classes-0.8.0/PKG-INFO` & `spond_classes-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spond-classes
-Version: 0.8.0
+Version: 0.8.1
 Summary: Experimental Python class abstraction layer for `spond` package.
 Home-page: https://github.com/elliot-100/Spond-classes
 License: GPL 3.0
 Author: elliot-100
 Author-email: 3186037+elliot-100@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -40,14 +40,44 @@
 pip install spond-classes
 `
 Or if you're using Poetry:
 `
 poetry add spond-classes
 `
 
+## Example code
+
+Adapting the example code in [`Spond`](https://github.com/Olen/Spond/) README:
+
+```
+import asyncio
+from spond import spond
+import spond_classes
+
+username = 'my@mail.invalid'
+password = 'Pa55worD'
+group_id = 'C9DC791FFE63D7914D6952BE10D97B46'  # fake
+
+async def main():
+    s = spond.Spond(username=username, password=password)
+    group_data = await s.get_group(group_id)
+    await s.clientsession.close()
+
+    # Now we can create a class instance ...
+    group = spond_classes.Group.from_dict(group_data)
+
+    # ... use class properties instead of dict keys ...
+    print(group.name)
+
+    # ... and access child instances and their properties
+    for member in group.members:
+        print(member.full_name)
+
+asyncio.run(main())
+```
 ## Key features
 
 * Create `Group` class instance from the dict returned by the corresponding `spond`
   method:
 
 ```
 spond_classes.Group.from_dict()
@@ -107,38 +137,7 @@
 Event.waiting_list_uids: list
 Event.unconfirmed_uids: list
 ```
 
 It's also possible to create `Member.from_dict()`, `Role.from_dict()`,
 `Subgroup.from_dict()`.
 
-## Example code
-
-Adapting the example code in [`Spond`](https://github.com/Olen/Spond/) README:
-
-```
-import asyncio
-from spond import spond
-import spond_classes
-
-username = 'my@mail.invalid'
-password = 'Pa55worD'
-group_id = 'C9DC791FFE63D7914D6952BE10D97B46'  # fake
-
-async def main():
-    s = spond.Spond(username=username, password=password)
-    group_data = await s.get_group(group_id)
-    await s.clientsession.close()
-
-    # Now we can create a class instance ...
-    group = spond_classes.Group.from_dict(group_data)
-
-    # ... use class properties instead of dict keys ...
-    print(group.name)
-
-    # ... and access child instances and their properties
-    for member in group.members:
-        print(member.full_name)
-
-asyncio.run(main())
-```
-
```


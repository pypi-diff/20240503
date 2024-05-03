# Comparing `tmp/django_monkey_patches-3.0.3.tar.gz` & `tmp/django_monkey_patches-4.0.0.tar.gz`

## Comparing `django_monkey_patches-3.0.3.tar` & `django_monkey_patches-4.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/README_printable.md
--rwxr-xr-x   0        0        0     2439 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/build_and_checks.sh
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/wget_sha512.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/__init__.py
--rw-r--r--   0        0        0    39101 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__base_cache__make_cache_key.py
--rw-r--r--   0        0        0    15669 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__orm__prefetch.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_set.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_set__get.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_set__get_or_create.py
--rw-r--r--   0        0        0    37322 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_wrapper.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django__test_case__tear_down.py
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django_rest_framework__field__get_request.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/PKG-INFO
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/requires.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/top_level.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/COPYING.LESSER
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/README.md
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/pyproject.toml
--rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 django_monkey_patches-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/README_printable.md
+-rwxr-xr-x   0        0        0     2439 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/build_and_checks.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/wget_sha512.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches/__init__.py
+-rw-r--r--   0        0        0    39101 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches/django__base_cache__make_cache_key.py
+-rw-r--r--   0        0        0    15669 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches/django__orm__prefetch.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches/django__query_set.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches/django__query_set__get.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches/django__query_set__get_or_create.py
+-rw-r--r--   0        0        0    42015 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches/django__query_wrapper.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches/django__test_case__tear_down.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches/django_rest_framework__field__get_request.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
+-rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches.egg-info/requires.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/src/django_monkey_patches.egg-info/top_level.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/COPYING.LESSER
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/README.md
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 django_monkey_patches-4.0.0/PKG-INFO
```

### Comparing `django_monkey_patches-3.0.3/README_printable.md` & `django_monkey_patches-4.0.0/README_printable.md`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/build_and_checks.sh` & `django_monkey_patches-4.0.0/build_and_checks.sh`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/wget_sha512.sh` & `django_monkey_patches-4.0.0/wget_sha512.sh`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py` & `django_monkey_patches-4.0.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches/django__base_cache__make_cache_key.py` & `django_monkey_patches-4.0.0/src/django_monkey_patches/django__base_cache__make_cache_key.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches/django__orm__prefetch.py` & `django_monkey_patches-4.0.0/src/django_monkey_patches/django__orm__prefetch.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py` & `django_monkey_patches-4.0.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_set.py` & `django_monkey_patches-4.0.0/src/django_monkey_patches/django__query_set.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_set__get.py` & `django_monkey_patches-4.0.0/src/django_monkey_patches/django__query_set__get.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_set__get_or_create.py` & `django_monkey_patches-4.0.0/src/django_monkey_patches/django__query_set__get_or_create.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches/django__query_wrapper.py` & `django_monkey_patches-4.0.0/src/django_monkey_patches/django__query_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -513,80 +513,143 @@
     if you don't want compatibility problems later.
     """
     return connection.django_monkey_patches_stash_stack.get(
         get_reference_pid()
     )
 
 
-def is_globally_init():
+def is_globally_init(connection):
     """
     Since Django connections are shared between processes
     in many cases,
     tell if these connections already have the dicts linked
     to this patch.
     """
-    return hasattr(connections, "django_monkey_patches_dict")
+    return hasattr(connection, "django_monkey_patches_dict")
 
 
-def is_locally_init():
+def is_locally_init(connection):
     """
     Since Django connections are shared between processes
     in many cases,
     tell if these connections already have the dicts linked
     to this patch.
     And test if these dicts have values for the current reference_pid.
     """
     return (
-        is_globally_init()
-        and connections.django_monkey_patches_dict.get(
+        is_globally_init(connection)
+        and connection.django_monkey_patches_dict.get(
             get_reference_pid()
         )
         is not None
     )
 
 
-def init_connections_extra_data(
+def init_connection_extra_data(
+    connection,
     get_extra_data_template_callback,
     manager=None,
     empty_stash_stack=False,
 ):
     """
-    You should call this function or a custom one
-    before using the custom query wrapper.
+    An inner function to init one connection.
     """
-    if not is_globally_init():
-        connections.django_monkey_patches_reference_pids = {}
-        connections.django_monkey_patches_dict = {}
-        connections.django_monkey_patches_stash_stack = {}
-        for connection_key in connections:
-            connection = connections[connection_key]
+    if not is_globally_init(connection):
+        if connection is connections:
             connection.django_monkey_patches_reference_pids = {}
-            connection.django_monkey_patches_dict = {}
-            connection.django_monkey_patches_stash_stack = {}
+        connection.django_monkey_patches_dict = {}
+        connection.django_monkey_patches_stash_stack = {}
 
-    connections.django_monkey_patches_dict[get_reference_pid()] = (
+    connection.django_monkey_patches_dict[get_reference_pid()] = (
         get_extra_data_template_callback()
     )
-    if empty_stash_stack or get_connection_stack(connections) is None:
-        connections.django_monkey_patches_stash_stack[
+    if empty_stash_stack or get_connection_stack(connection) is None:
+        connection.django_monkey_patches_stash_stack[
             get_reference_pid()
         ] = get_managed_list(manager)
 
+
+# pylint: disable-next=too-many-arguments
+def init_connection_extra_data_v1(
+    connection,
+    manager=None,
+    empty_stash_stack=False,
+    query_fields=None,
+    min_seconds_threshold=0,
+    max_seconds_threshold=float("inf"),
+    filter_callback=None,
+    insertion_callback=None,
+    subsets_extra_data=None,
+    allocated_subsets_extra_data=None,
+    allocated_subsets_key_callback=None,
+    allocated_subsets_init_callback=None,
+    top_down_post_processing_callback=None,
+    bottom_up_post_processing_callback=None,
+):
+    """
+    A simple default function providing the
+    get_extra_data_template_callback argument
+    to init_connection_extra_data().
+    """
+
+    def lambda_get_extra_data_template_for_set_of_queries_v1():
+        return get_extra_data_template_for_set_of_queries_v1(
+            query_fields=query_fields,
+            min_seconds_threshold=min_seconds_threshold,
+            max_seconds_threshold=max_seconds_threshold,
+            filter_callback=filter_callback,
+            insertion_callback=insertion_callback,
+            subsets_extra_data=subsets_extra_data,
+            allocated_subsets_extra_data=allocated_subsets_extra_data,
+            allocated_subsets_key_callback=(
+                allocated_subsets_key_callback
+            ),
+            allocated_subsets_init_callback=(
+                allocated_subsets_init_callback
+            ),
+            top_down_post_processing_callback=(
+                top_down_post_processing_callback
+            ),
+            bottom_up_post_processing_callback=(
+                bottom_up_post_processing_callback
+            ),
+            manager=manager,
+        )
+
+    init_connection_extra_data(
+        connection,
+        lambda_get_extra_data_template_for_set_of_queries_v1,
+        manager=manager,
+        empty_stash_stack=empty_stash_stack,
+    )
+
+
+def init_connections_extra_data(
+    get_extra_data_template_callback,
+    manager=None,
+    empty_stash_stack=False,
+):
+    """
+    You should call this function or a custom one
+    before using the custom query wrapper.
+    """
+    init_connection_extra_data(
+        connections,
+        get_extra_data_template_callback,
+        manager=manager,
+        empty_stash_stack=empty_stash_stack,
+    )
     for connection_key in connections:
         connection = connections[connection_key]
-        connection.django_monkey_patches_dict[get_reference_pid()] = (
-            get_extra_data_template_callback()
+        init_connection_extra_data(
+            connection,
+            get_extra_data_template_callback,
+            manager=manager,
+            empty_stash_stack=empty_stash_stack,
         )
-        if (
-            empty_stash_stack
-            or get_connection_stack(connection) is None
-        ):
-            connection.django_monkey_patches_stash_stack[
-                get_reference_pid()
-            ] = get_managed_list(manager)
 
 
 # pylint: disable-next=too-many-arguments
 def init_connections_extra_data_v1(
     manager=None,
     empty_stash_stack=False,
     query_fields=None,
@@ -864,43 +927,120 @@
     for connection_key in connections_to_wrap:
         connection = connections[connection_key]
         exit_stack.enter_context(
             connection.execute_wrapper(custom_query_wrapper)
         )
 
 
-def stash_extra_data_dicts(reinit_after_stash=None):
+def stash_extra_data_dict(
+    connection,
+    reinit_after_stash=None,
+    init_if_non_locally_init=False,
+):
     """
-    Stash current django_monkey_patches_dicts
-    in django_monkey_patches_stash_stacks.
+    Stash connection django_monkey_patches_dict
+    in django_monkey_patches_stash_stack.
     """
-    connections.django_monkey_patches_stash_stack[
+    if not is_locally_init(connection) and init_if_non_locally_init:
+        reinit_after_stash(connection)
+        return
+    connection.django_monkey_patches_stash_stack[
         get_reference_pid()
     ].append(
-        connections.django_monkey_patches_dict[get_reference_pid()]
+        connection.django_monkey_patches_dict[get_reference_pid()]
     )
 
     if reinit_after_stash is None:
-        connections.django_monkey_patches_dict[
-            get_reference_pid()
-        ] = None
+        connection.django_monkey_patches_dict[get_reference_pid()] = (
+            None
+        )
+    else:
+        reinit_after_stash(connection)
+
+
+# pylint: disable-next=too-many-arguments
+def stash_extra_data_dict_and_reinit_v1(
+    connection,
+    manager=None,
+    query_fields=None,
+    min_seconds_threshold=0,
+    max_seconds_threshold=float("inf"),
+    filter_callback=None,
+    insertion_callback=None,
+    subsets_extra_data=None,
+    allocated_subsets_extra_data=None,
+    allocated_subsets_key_callback=None,
+    allocated_subsets_init_callback=None,
+    top_down_post_processing_callback=None,
+    bottom_up_post_processing_callback=None,
+    init_if_non_locally_init=False,
+):
+    """
+    Stash connection django_monkey_patches_dict
+    in django_monkey_patches_stash_stack,
+    and apply a reinit using default init function.
+    """
+
+    def lambda_init_connection_extra_data_v1(connection_):
+        init_connection_extra_data_v1(
+            connection_,
+            manager=manager,
+            empty_stash_stack=False,
+            query_fields=query_fields,
+            min_seconds_threshold=min_seconds_threshold,
+            max_seconds_threshold=max_seconds_threshold,
+            filter_callback=filter_callback,
+            insertion_callback=insertion_callback,
+            subsets_extra_data=subsets_extra_data,
+            allocated_subsets_extra_data=allocated_subsets_extra_data,
+            allocated_subsets_key_callback=(
+                allocated_subsets_key_callback
+            ),
+            allocated_subsets_init_callback=(
+                allocated_subsets_init_callback
+            ),
+            top_down_post_processing_callback=(
+                top_down_post_processing_callback
+            ),
+            bottom_up_post_processing_callback=(
+                bottom_up_post_processing_callback
+            ),
+        )
+
+    stash_extra_data_dict(
+        connection,
+        reinit_after_stash=lambda_init_connection_extra_data_v1,
+        init_if_non_locally_init=init_if_non_locally_init,
+    )
+
+
+def stash_extra_data_dicts(
+    # These two arguments should be mutually exclusive.
+    local_reinit_after_stash=None,
+    global_reinit_after_stash=None,
+    init_if_non_locally_init=False,
+):
+    """
+    Stash current django_monkey_patches_dicts
+    in django_monkey_patches_stash_stacks.
+    """
+    stash_extra_data_dict(
+        connections,
+        reinit_after_stash=local_reinit_after_stash,
+        init_if_non_locally_init=init_if_non_locally_init,
+    )
     for connection_key in connections:
         connection = connections[connection_key]
-        connection.django_monkey_patches_stash_stack[
-            get_reference_pid()
-        ].append(
-            connection.django_monkey_patches_dict[get_reference_pid()]
+        stash_extra_data_dict(
+            connection,
+            reinit_after_stash=local_reinit_after_stash,
+            init_if_non_locally_init=init_if_non_locally_init,
         )
-        if reinit_after_stash is None:
-            connection.django_monkey_patches_dict[
-                get_reference_pid()
-            ] = None
-
-    if reinit_after_stash:
-        reinit_after_stash()
+    if global_reinit_after_stash:
+        global_reinit_after_stash()
 
 
 # pylint: disable-next=too-many-arguments
 def stash_extra_data_dicts_and_reinit_v1(
     manager=None,
     query_fields=None,
     min_seconds_threshold=0,
@@ -909,23 +1049,25 @@
     insertion_callback=None,
     subsets_extra_data=None,
     allocated_subsets_extra_data=None,
     allocated_subsets_key_callback=None,
     allocated_subsets_init_callback=None,
     top_down_post_processing_callback=None,
     bottom_up_post_processing_callback=None,
+    init_if_non_locally_init=False,
 ):
     """
     Stash current django_monkey_patches_dicts
     in django_monkey_patches_stash_stacks,
     and apply a reinit using default init functions.
     """
 
-    def lambda_init_connections_extra_data_v1():
-        init_connections_extra_data_v1(
+    def lambda_init_connection_extra_data_v1(connection):
+        init_connection_extra_data_v1(
+            connection,
             manager=manager,
             empty_stash_stack=False,
             query_fields=query_fields,
             min_seconds_threshold=min_seconds_threshold,
             max_seconds_threshold=max_seconds_threshold,
             filter_callback=filter_callback,
             insertion_callback=insertion_callback,
@@ -942,34 +1084,46 @@
             ),
             bottom_up_post_processing_callback=(
                 bottom_up_post_processing_callback
             ),
         )
 
     stash_extra_data_dicts(
-        reinit_after_stash=lambda_init_connections_extra_data_v1
+        local_reinit_after_stash=lambda_init_connection_extra_data_v1,
+        init_if_non_locally_init=init_if_non_locally_init,
     )
 
 
-def pop_extra_data_dicts():
+def pop_extra_data_dict(connection, ignore_empty_stack=False):
+    """
+    Pop last dict in django_monkey_patches_stash_stack
+    to django_monkey_patches_dict of connection.
+    """
+    stash_stack = get_connection_stack(connection)
+    if ignore_empty_stack and len(stash_stack) == 0:
+        return
+    connection.django_monkey_patches_dict[get_reference_pid()] = (
+        stash_stack.pop()
+    )
+
+
+def pop_extra_data_dicts(ignore_empty_stack=False):
     """
     Pop last dicts in django_monkey_patches_stash_stacks
     to django_monkey_patches_dicts.
     """
-    connections.django_monkey_patches_dict[get_reference_pid()] = (
-        connections.django_monkey_patches_stash_stack[
-            get_reference_pid()
-        ].pop()
+    pop_extra_data_dict(
+        connections,
+        ignore_empty_stack=ignore_empty_stack,
     )
     for connection_key in connections:
         connection = connections[connection_key]
-        connection.django_monkey_patches_dict[get_reference_pid()] = (
-            connection.django_monkey_patches_stash_stack[
-                get_reference_pid()
-            ].pop()
+        pop_extra_data_dict(
+            connection,
+            ignore_empty_stack=ignore_empty_stack,
         )
 
 
 def apply_patch_rq_v1():
     """
     A function to apply a patch to rq needed to follow pids between
     parent and child processes in Django-rq.
```

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches/django__test_case__tear_down.py` & `django_monkey_patches-4.0.0/src/django_monkey_patches/django__test_case__tear_down.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches/django_rest_framework__field__get_request.py` & `django_monkey_patches-4.0.0/src/django_monkey_patches/django_rest_framework__field__get_request.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py` & `django_monkey_patches-4.0.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/PKG-INFO` & `django_monkey_patches-4.0.0/src/django_monkey_patches.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/src/django_monkey_patches.egg-info/SOURCES.txt` & `django_monkey_patches-4.0.0/src/django_monkey_patches.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/COPYING` & `django_monkey_patches-4.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/COPYING.LESSER` & `django_monkey_patches-4.0.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/README.md` & `django_monkey_patches-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-3.0.3/pyproject.toml` & `django_monkey_patches-4.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-monkey-patches"
-version = "3.0.3"
+version = "4.0.0"
 description = """\
 Add monkey-patches to correct and enhance your favorite framework\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
```

### Comparing `django_monkey_patches-3.0.3/PKG-INFO` & `django_monkey_patches-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-monkey-patches
-Version: 3.0.3
+Version: 4.0.0
 Summary: Add monkey-patches to correct and enhance your favorite framework
 Project-URL: Homepage, https://github.com/LLyaudet/django-monkey-patches
 Project-URL: Bug Tracker, https://github.com/LLyaudet/django-monkey-patches/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 Maintainer-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```


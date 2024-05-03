# Comparing `tmp/taskflows-0.4.1-py3-none-any.whl.zip` & `tmp/taskflows-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 23718 bytes, number of entries: 16
+Zip file size: 23801 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx       87 b- defN 24-Feb-15 20:59 taskflows/__init__.py
--rw-rw-r--  2.0 unx     9552 b- defN 24-Apr-29 20:43 taskflows/admin.py
--rw-rw-r--  2.0 unx     3723 b- defN 24-Apr-29 18:43 taskflows/db.py
+-rw-rw-r--  2.0 unx    10110 b- defN 24-May-02 17:22 taskflows/admin.py
+-rw-rw-r--  2.0 unx     3444 b- defN 24-May-01 00:36 taskflows/db.py
 -rw-rw-r--  2.0 unx     8937 b- defN 24-Mar-05 14:35 taskflows/tasks.py
 -rw-rw-r--  2.0 unx      564 b- defN 24-Feb-12 20:43 taskflows/utils.py
--rwxrwxr-x  2.0 unx      570 b- defN 24-Apr-29 19:55 taskflows/service/__init__.py
+-rwxrwxr-x  2.0 unx      587 b- defN 24-May-02 17:22 taskflows/service/__init__.py
 -rwxrwxr-x  2.0 unx     1286 b- defN 24-Feb-29 14:30 taskflows/service/commands.py
 -rwxrwxr-x  2.0 unx     1586 b- defN 24-Feb-12 20:43 taskflows/service/constraints.py
 -rw-rw-r--  2.0 unx    18204 b- defN 24-Apr-22 18:48 taskflows/service/docker.py
 -rwxrwxr-x  2.0 unx     2234 b- defN 24-Feb-12 20:43 taskflows/service/schedule.py
 -rwxrwxr-x  2.0 unx    18155 b- defN 24-Apr-29 23:57 taskflows/service/service.py
--rw-rw-r--  2.0 unx     4093 b- defN 24-Apr-30 00:40 taskflows-0.4.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-30 00:40 taskflows-0.4.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx      111 b- defN 24-Apr-30 00:40 taskflows-0.4.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 24-Apr-30 00:40 taskflows-0.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1293 b- defN 24-Apr-30 00:40 taskflows-0.4.1.dist-info/RECORD
-16 files, 70497 bytes uncompressed, 21596 bytes compressed:  69.4%
+-rw-rw-r--  2.0 unx     4093 b- defN 24-May-03 14:25 taskflows-0.4.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-03 14:25 taskflows-0.4.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      111 b- defN 24-May-03 14:25 taskflows-0.4.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 24-May-03 14:25 taskflows-0.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1294 b- defN 24-May-03 14:25 taskflows-0.4.3.dist-info/RECORD
+16 files, 70794 bytes uncompressed, 21679 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: taskflows/service/schedule.py
 Comment: 
 
 Filename: taskflows/service/service.py
 Comment: 
 
-Filename: taskflows-0.4.1.dist-info/METADATA
+Filename: taskflows-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: taskflows-0.4.1.dist-info/WHEEL
+Filename: taskflows-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: taskflows-0.4.1.dist-info/entry_points.txt
+Filename: taskflows-0.4.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: taskflows-0.4.1.dist-info/top_level.txt
+Filename: taskflows-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: taskflows-0.4.1.dist-info/RECORD
+Filename: taskflows-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## taskflows/admin.py

```diff
@@ -11,14 +11,15 @@
 from dynamic_imports import import_module
 from rich import box
 from rich.console import Console
 from rich.table import Table
 
 from .db import task_flows_db
 from .service import (
+    systemd_dir,
     Service,
     disable_service,
     enable_service,
     get_service_files,
     get_timer_files,
     remove_service,
     restart_service,
@@ -82,15 +83,15 @@
     pprint(proc.stdout.decode().split("\n"))
     # manager.GetUnitFileState(service)
 
 
 @cli.command(name="list")
 def list_services():
     """List services."""
-    services = [f.name for f in get_service_files()]
+    services = [f.stem.replace(_SYSTEMD_FILE_PREFIX,"") for f in get_service_files()]
     if services:
         click.echo(pformat(services))
     else:
         click.echo(click.style("No services found.", fg="yellow"))
 
 
 @cli.command()
@@ -279,14 +280,30 @@
     Args:
         service (str): Name or name pattern of service(s) to remove.
     """
     remove_service(service)
     click.echo(click.style("Done!", fg="green"))
 
 
+@cli.command
+@click.argument("service", required=False)
+def show(service: str):
+    services = []
+    if service:
+        if not service.startswith(_SYSTEMD_FILE_PREFIX):
+            service = _SYSTEMD_FILE_PREFIX+service
+        if not service.endswith('.service'):
+            service += '.service'
+        services = [service]
+    else:
+        services = list(systemd_dir.glob('*.service'))
+    services = "\n\n".join([s.read_text() for s in services])
+    click.echo(click.style(services, fg="cyan"))
+
+
 def table_column_colors():
     colors_gen = cycle(["orange3", "green", "cyan", "magenta", "dodger_blue1", "red"])
 
     @lru_cache
     def column_color(col_name: str) -> str:
         return next(colors_gen)
```

## taskflows/db.py

```diff
@@ -14,40 +14,33 @@
     return TaskflowsDB()
 
 
 class TaskflowsDB:
     def __init__(self) -> None:
         db_url = os.getenv("TASKFLOWS_DB_URL")
         if not db_url:
-            db_dir = "/var/lib/taskflows"
-            try:
-                Path(db_dir).mkdir(exist_ok=True)
-            except PermissionError:
-                db_dir = os.path.expanduser("~/.taskflows")
-                Path(db_dir).mkdir(exist_ok=True)
+            db_dir = os.path.expanduser("~/.taskflows")
             db_url = f"sqlite:///{db_dir}/taskflows.sqlite"
             dialect = "sqlite"
         else:
             dialect = re.search(r"^[a-z]+", db_url).group()
             if dialect == "sqlite":
                 db_dir = Path(db_url.replace("sqlite:///", "")).parent
-                logger.info("Checking database directory exists %s", db_dir)
-                db_dir.mkdir(parents=True, exist_ok=True)
+        Path(db_dir).mkdir(parents=True, exist_ok=True)
         schema_name = os.getenv("TASKFLOWS_DB_SCHEMA")
         if dialect == "sqlite":
             if schema_name:
                 logger.warning(
                     "Schemas are not supported by SQLite. Will not use provided schema: %s",
                     schema_name,
                 )
             schema_name = None
             from sqlalchemy.dialects.sqlite import JSON, insert
         elif dialect == "postgresql":
             from sqlalchemy.dialects.postgresql import JSON, insert
-
             if not schema_name:
                 schema_name = "taskflows"
         else:
             raise ValueError(f"Unsupported database dialect: {dialect}")
         logger.info("Using database: %s", db_url)
         sa_meta = sa.MetaData(schema=schema_name)
         engine = sa.create_engine(db_url)
```

## taskflows/service/__init__.py

```diff
@@ -7,14 +7,15 @@
     Memory,
     MemoryPressure,
     SystemLoadConstraint,
 )
 from .docker import ContainerLimits, DockerContainer, DockerImage, Ulimit, Volume
 from .schedule import Calendar, Periodic, Schedule
 from .service import (
+    systemd_dir,
     Service,
     disable_service,
     enable_service,
     get_service_files,
     get_timer_files,
     remove_service,
     restart_service,
```

## Comparing `taskflows-0.4.1.dist-info/METADATA` & `taskflows-0.4.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskflows
-Version: 0.4.1
+Version: 0.4.3
 Summary: Python task management, scheduling, alerts.
 Author-email: Dan Kelleher <kelleherjdan@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

## Comparing `taskflows-0.4.1.dist-info/RECORD` & `taskflows-0.4.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 taskflows/__init__.py,sha256=oW-FCpGdoTfDXFNZ7hlNV2lzLUzQoKSPTP2TfvDIPPk,87
-taskflows/admin.py,sha256=AakqlB954gWaZ8vJC3haLvf43oV3HZbulWUe8N8meII,9552
-taskflows/db.py,sha256=vrdCXikZJe6kNYHt--WywYtvY5epEiv216_JXoRrccY,3723
+taskflows/admin.py,sha256=1errDFcld0SB3Um1KIHKjRPYhYP_ZXoTcrCczZE9Uko,10110
+taskflows/db.py,sha256=aOoWhuy1__7YobfP0bB1x-sTFEjoSM06Kdw1m6--GWc,3444
 taskflows/tasks.py,sha256=aXQxLu6_JItg5iqQpZDDYLaJKIvbI5B17_rLWQGWJFk,8937
 taskflows/utils.py,sha256=TahZKvotnW_us79SXYkjrjXoa464MwHFe6uo5SR0XuI,564
-taskflows/service/__init__.py,sha256=A6HD1mdzY1YMvXwKDzqrMJFsSxeg781UsoxDRW7N24o,570
+taskflows/service/__init__.py,sha256=Epl-nKhfYN7Qn69PBBH8mvxXgYVJBywvIAcIFUK8Su8,587
 taskflows/service/commands.py,sha256=t_ITtM5l5_Dtpx70p6uKBaWGixGkNZCYm13zXBlQkQw,1286
 taskflows/service/constraints.py,sha256=2N5eSAJjUg2twxmVjs3GWaqmppc-DW0dZ5MlMRqcmNw,1586
 taskflows/service/docker.py,sha256=w2VFWPCcAd5hLqkOamfdJuPagT_qeB4tBqVoFnGw5Rc,18204
 taskflows/service/schedule.py,sha256=84B5phVhjSoj-UTtmqHmVwKTHYVjjfuryYW3p4yuJco,2234
 taskflows/service/service.py,sha256=_tKef13I2Ge3qPF3WgJprVFAaxDxnPciCC6fMPuo2iY,18155
-taskflows-0.4.1.dist-info/METADATA,sha256=1EoLOzkJSOvnqCi3_6BtMY_8ezWcmAOwu9CEsJPnbcg,4093
-taskflows-0.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-taskflows-0.4.1.dist-info/entry_points.txt,sha256=84ElXyA0XQ3cRfNIL-woPCmCkGk9-OV4YarSW0i-88Y,111
-taskflows-0.4.1.dist-info/top_level.txt,sha256=CipuamG5azL_xisU7bxm8aEd18vy0JSHVWx4WzswtqQ,10
-taskflows-0.4.1.dist-info/RECORD,,
+taskflows-0.4.3.dist-info/METADATA,sha256=c44Ca9B-QAZjeC741_0-L7Zqduff0b8oENKKvfQpUmU,4093
+taskflows-0.4.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+taskflows-0.4.3.dist-info/entry_points.txt,sha256=84ElXyA0XQ3cRfNIL-woPCmCkGk9-OV4YarSW0i-88Y,111
+taskflows-0.4.3.dist-info/top_level.txt,sha256=CipuamG5azL_xisU7bxm8aEd18vy0JSHVWx4WzswtqQ,10
+taskflows-0.4.3.dist-info/RECORD,,
```


# Comparing `tmp/ultima_scraper_db-0.3.4.tar.gz` & `tmp/ultima_scraper_db-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_db-0.3.4.tar", max compression
+gzip compressed data, was "ultima_scraper_db-0.3.5.tar", max compression
```

## Comparing `ultima_scraper_db-0.3.4.tar` & `ultima_scraper_db-0.3.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35149 2023-07-12 18:49:43.683779 ultima_scraper_db-0.3.4/LICENSE
--rw-r--r--   0        0        0        0 2023-07-12 18:49:43.683779 ultima_scraper_db-0.3.4/README.md
--rw-r--r--   0        0        0      769 2024-02-13 04:08:42.529873 ultima_scraper_db-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        1 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.4/ultima_scraper_db/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/__init__.py
--rw-r--r--   0        0        0      172 2023-11-17 08:19:59.260044 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/rest_api.py
--rw-r--r--   0        0        0     5856 2024-01-21 05:59:43.924738 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/__init__.py
--rw-r--r--   0        0        0       58 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/alembic/README
--rw-r--r--   0        0        0     2702 2023-08-06 09:24:11.959103 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/alembic/env.py
--rw-r--r--   0        0        0      510 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/alembic/script.py.mako
--rw-r--r--   0        0        0     1367 2024-02-13 00:37:33.667968 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/alembic/versions/358d71fc1759_.py
--rw-r--r--   0        0        0    46084 2023-12-30 16:44:57.006348 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/alembic/versions/ac840f4e3061_.py
--rw-r--r--   0        0        0     3380 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/alembic.ini
--rw-r--r--   0        0        0        0 2023-08-02 08:54:09.083135 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/api/__init__.py
--rw-r--r--   0        0        0      268 2023-08-16 13:40:22.806271 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/api/app.py
--rw-r--r--   0        0        0      860 2024-01-21 06:44:32.497635 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/api/client.py
--rw-r--r--   0        0        0        0 2023-08-02 08:55:13.084330 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/api/routers/__init__.py
--rw-r--r--   0        0        0     5567 2024-02-11 01:31:28.018687 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/api/routers/jobs.py
--rw-r--r--   0        0        0     2009 2024-01-21 07:46:20.883469 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/api/routers/users.py
--rw-r--r--   0        0        0     3417 2024-01-21 06:42:39.948237 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/database_api.py
--rw-r--r--   0        0        0      406 2023-11-29 01:58:04.294758 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/filters.py
--rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/schemas/__init__.py
--rw-r--r--   0        0        0     1883 2023-08-16 20:12:22.325190 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/schemas/management.py
--rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/schemas/templates/__init__.py
--rw-r--r--   0        0        0    40783 2024-02-13 03:14:00.361098 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/schemas/templates/site.py
--rw-r--r--   0        0        0    53468 2024-02-13 02:54:32.723334 ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/site_api.py
--rw-r--r--   0        0        0     6412 2023-11-17 13:06:54.782943 ultima_scraper_db-0.3.4/ultima_scraper_db/helpers.py
--rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.4/ultima_scraper_db/managers/__init__.py
--rw-r--r--   0        0        0     9967 2023-12-10 12:50:39.067918 ultima_scraper_db-0.3.4/ultima_scraper_db/managers/database_manager.py
--rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.4/ultima_scraper_db/py.typed
--rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 ultima_scraper_db-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-12 18:49:43.683779 ultima_scraper_db-0.3.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-12 18:49:43.683779 ultima_scraper_db-0.3.5/README.md
+-rw-r--r--   0        0        0      761 2024-05-03 05:23:39.479346 ultima_scraper_db-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.5/ultima_scraper_db/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/__init__.py
+-rw-r--r--   0        0        0      172 2023-11-17 08:19:59.260044 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/rest_api.py
+-rw-r--r--   0        0        0     5856 2024-01-21 05:59:43.924738 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/alembic/README
+-rw-r--r--   0        0        0     2702 2023-08-06 09:24:11.959103 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/alembic/env.py
+-rw-r--r--   0        0        0      510 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/alembic/script.py.mako
+-rw-r--r--   0        0        0     1367 2024-02-13 00:37:33.667968 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/alembic/versions/358d71fc1759_.py
+-rw-r--r--   0        0        0    46084 2023-12-30 16:44:57.006348 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/alembic/versions/ac840f4e3061_.py
+-rw-r--r--   0        0        0     3380 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/alembic.ini
+-rw-r--r--   0        0        0        0 2023-08-02 08:54:09.083135 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/api/__init__.py
+-rw-r--r--   0        0        0      268 2023-08-16 13:40:22.806271 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/api/app.py
+-rw-r--r--   0        0        0      860 2024-01-21 06:44:32.497635 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/api/client.py
+-rw-r--r--   0        0        0        0 2023-08-02 08:55:13.084330 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/api/routers/__init__.py
+-rw-r--r--   0        0        0     5567 2024-02-11 01:31:28.018687 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/api/routers/jobs.py
+-rw-r--r--   0        0        0     2034 2024-03-22 11:09:15.696777 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/api/routers/users.py
+-rw-r--r--   0        0        0     3417 2024-01-21 06:42:39.948237 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/database_api.py
+-rw-r--r--   0        0        0      406 2023-11-29 01:58:04.294758 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/filters.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/schemas/__init__.py
+-rw-r--r--   0        0        0     1883 2023-08-16 20:12:22.325190 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/schemas/management.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/schemas/templates/__init__.py
+-rw-r--r--   0        0        0    41719 2024-04-25 13:08:39.409108 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/schemas/templates/site.py
+-rw-r--r--   0        0        0    53654 2024-03-09 03:53:29.083155 ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/site_api.py
+-rw-r--r--   0        0        0     6412 2023-11-17 13:06:54.782943 ultima_scraper_db-0.3.5/ultima_scraper_db/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.5/ultima_scraper_db/managers/__init__.py
+-rw-r--r--   0        0        0    10378 2024-03-22 10:54:22.620488 ultima_scraper_db-0.3.5/ultima_scraper_db/managers/database_manager.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:49:43.687112 ultima_scraper_db-0.3.5/ultima_scraper_db/py.typed
+-rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 ultima_scraper_db-0.3.5/PKG-INFO
```

### Comparing `ultima_scraper_db-0.3.4/LICENSE` & `ultima_scraper_db-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.3.4/pyproject.toml` & `ultima_scraper_db-0.3.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 [tool.poetry]
 name = "ultima-scraper-db"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
-authors = [
-    "UltimaHoarder <1285176+UltimaHoarder@users.noreply.github.com>",
-]
+authors = ["UltimaHoarder <1285176+UltimaHoarder@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "ultima_scraper_db" }]
 include = ["ultima_scraper_db/py.typed"]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
-sqlalchemy = {extras = ["asyncio"], version = "^2.0.16"}
+python = ">=3.10,<4"
+sqlalchemy = { extras = ["asyncio"], version = "^2.0.16" }
 asyncpg = "^0.27.0"
 psycopg = "^3.1.9"
 ultima-scraper-api = "^2.0.0"
 ultima-scraper-collection = "^2.0.0"
 sqlalchemy-utils = "^0.41.1"
 alembic = "^1.11.1"
 sshtunnel = "^0.4.0"
-fastapi = "^0.104.1"
-uvicorn = {extras = ["standard"], version = "^0.24.0"}
+fastapi = "^0.100"
+uvicorn = { extras = ["standard"], version = "^0.24.0" }
 fastapi-pagination = "^0.12.6"
 inflection = "^0.5.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/__init__.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/alembic/env.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/alembic/versions/358d71fc1759_.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/alembic/versions/358d71fc1759_.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/alembic/versions/ac840f4e3061_.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/alembic/versions/ac840f4e3061_.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/alembic.ini` & `ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/api/client.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/api/client.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/api/routers/jobs.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/api/routers/jobs.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/api/routers/users.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/api/routers/users.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from fastapi import APIRouter, Depends, HTTPException, Request, Response
 from pydantic import BaseModel
 from sqlalchemy import or_, orm, select
 from sqlalchemy.orm import contains_eager, lazyload, sessionmaker
-
 from ultima_scraper_db.databases.ultima_archive.api.client import UAClient
 from ultima_scraper_db.databases.ultima_archive.schemas.templates.site import UserModel
 
 restricted = (
     lazyload(UserModel.user_auths_info),
     orm.defer(UserModel.performer),
     orm.defer(UserModel.favorite),
@@ -49,16 +48,17 @@
                 or_(UserModel.active.is_(True), UserModel.downloaded_at.is_not(None))
             )
             .offset(offset)
             .limit(limit)
             .order_by(UserModel.id)
             .options(*restricted)
         )
-        users = await site_api.get_session().scalars(stmt)
-        return users.all()
+        results = await site_api.get_session().scalars(stmt)
+        users = results.all()
+        return users
 
 
 @router.get("/{identifier}")
 async def read(site_name: str, identifier: int | str):
     database_api = UAClient.database_api
 
     site_api = database_api.get_site_api(site_name)
```

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/database_api.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/database_api.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/schemas/management.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/schemas/management.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/schemas/templates/site.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/schemas/templates/site.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,25 @@
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 from ultima_scraper_api.apis.fansly.classes.extras import (
     AuthDetails as FanslyAuthDetails,
 )
 from ultima_scraper_api.apis.onlyfans.classes.extras import (
     AuthDetails as OnlyFansAuthDetails,
 )
-
 from ultima_scraper_db.databases.ultima_archive import (
     CustomFuncs,
     DefaultContentTypes,
     SiteTemplate,
 )
 from ultima_scraper_db.helpers import TIMESTAMPTZ, selectin_relationship
 
 if TYPE_CHECKING:
     from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
         ContentMetadata,
     )
-
     from ultima_scraper_db.databases.ultima_archive.schemas.management import SiteModel
     from ultima_scraper_db.databases.ultima_archive.site_api import ContentManager
 
 
 standard_unique_constraints = (
     UniqueConstraint(
         "story_id",
@@ -165,21 +163,39 @@
                     SubscriptionModel.downloaded_at.is_not(None),
                 )
             )
             .order_by(SubscriptionModel.downloaded_at.desc())
         )
         return await session.scalar(stmt)
 
+    async def update_username(self, username: str):
+        u_username = f"u{self.id}"
+        final_aliases = [
+            x for x in self.aliases if x.id is not None and x.username != u_username
+        ]
+        if username == u_username:
+            if self.aliases:
+                aliases_sorted_by_id = [x for x in self.aliases if x.id is None]
+                aliases_sorted_by_id.extend(
+                    sorted(final_aliases, key=lambda x: x.id, reverse=True)
+                )
+                if not aliases_sorted_by_id:
+                    return
+                username = aliases_sorted_by_id[0].username
+        if self.username != username:
+            old_username = self.username
+            self.username = username
+            await self.add_alias(old_username)
+
     async def add_alias(self, username: str):
         if self.username != username:
-            alias = await self.find_aliases(self.username)
+            alias = await self.find_aliases(username)
             if not alias:
-                alias = UserAliasModel(username=self.username)
+                alias = UserAliasModel(username=username)
                 self.aliases.append(alias)
-            self.username = username
             return alias
 
     async def find_aliases(self, username: str):
         await self.awaitable_attrs.aliases
         for alias in self.aliases:
             if alias.username == username:
                 return alias
@@ -516,14 +532,19 @@
         back_populates="media",
     )
 
     content_media_assos: Mapped[list[ContentMediaAssoModel]] = relationship(
         back_populates="media"
     )
 
+    async def get_contents(self):
+        await self.awaitable_attrs.content_media_assos
+        db_contents = [await x.get_content() for x in self.content_media_assos]
+        return db_contents
+
     async def find_content(self, api_type: str):
         content_type = api_type if api_type != "Stories" else "Story"
         await self.awaitable_attrs.content_media_assos
         for content_media_asso in self.content_media_assos:
             try:
                 key = content_media_asso.get_key(content_type)
                 assert key
```

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/databases/ultima_archive/site_api.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/databases/ultima_archive/site_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -670,16 +670,21 @@
             for text_item in text_list:
                 text_item = text_item.strip()
                 stmt = stmt.where(MessageModel.text.icontains(text_item))
         stmt = stmt.options(joinedload(MessageModel.user))
         found_contents = await self.get_session().scalars(stmt)
         return found_contents.all()
 
-    async def get_media(self, media_id: int):
-        stmt = select(MediaModel).where(MediaModel.id == media_id)
+    async def get_media(self, media_id: int | None = None, url: str | None = None):
+        found_media = None
+        stmt = select(MediaModel)
+        if media_id:
+            stmt = stmt.where(MediaModel.id == media_id)
+        if url:
+            stmt = stmt.where(MediaModel.url.contains(url))
         found_media = await self.get_session().scalar(stmt)
         if found_media:
             await found_media.awaitable_attrs.filepaths
         return found_media
 
     async def get_medias(self, user_id: int, media_ids: list[int] | None = None):
         stmt = (
```

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/helpers.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/helpers.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_db-0.3.4/ultima_scraper_db/managers/database_manager.py` & `ultima_scraper_db-0.3.5/ultima_scraper_db/managers/database_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,14 +245,24 @@
                     alembic_cfg = self.alembica.config
                     _upgraded = await conn.run_sync(run_upgrade, alembic_cfg)
                     break
             except Exception as e:
                 print(e)
                 breakpoint()
 
+    async def run_downgrade(self, version: str) -> None:
+        def downgrade(connection: Connection, cfg: Config):
+            cfg.attributes["connection"] = connection
+            command.downgrade(alembic_cfg, version)
+
+        async with self.engine.connect() as conn:
+            assert self.alembica
+            alembic_cfg = self.alembica.config
+            await conn.run_sync(downgrade, alembic_cfg)
+
 
 class DatabaseManager:
     def __init__(self) -> None:
         self.databases: dict[str, Database] = {}
 
     def create_database(
         self,
```

### Comparing `ultima_scraper_db-0.3.4/PKG-INFO` & `ultima_scraper_db-0.3.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-db
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Author: UltimaHoarder
 Author-email: 1285176+UltimaHoarder@users.noreply.github.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (>=1.11.1,<2.0.0)
 Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
-Requires-Dist: fastapi (>=0.104.1,<0.105.0)
+Requires-Dist: fastapi (>=0.100,<0.101)
 Requires-Dist: fastapi-pagination (>=0.12.6,<0.13.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: psycopg (>=3.1.9,<4.0.0)
 Requires-Dist: sqlalchemy-utils (>=0.41.1,<0.42.0)
 Requires-Dist: sqlalchemy[asyncio] (>=2.0.16,<3.0.0)
 Requires-Dist: sshtunnel (>=0.4.0,<0.5.0)
 Requires-Dist: ultima-scraper-api (>=2.0.0,<3.0.0)
```


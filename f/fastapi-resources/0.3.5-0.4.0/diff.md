# Comparing `tmp/fastapi_resources-0.3.5.tar.gz` & `tmp/fastapi_resources-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_resources-0.3.5.tar", max compression
+gzip compressed data, was "fastapi_resources-0.4.0.tar", max compression
```

## Comparing `fastapi_resources-0.3.5.tar` & `fastapi_resources-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0        0 2022-10-05 19:53:19.150339 fastapi_resources-0.3.5/fastapi_resources/__init__.py
--rw-r--r--   0        0        0       24 2022-10-12 22:22:41.674354 fastapi_resources-0.3.5/fastapi_resources/resources/__init__.py
--rw-r--r--   0        0        0     3424 2023-01-04 21:54:31.127181 fastapi_resources-0.3.5/fastapi_resources/resources/base_resource.py
--rw-r--r--   0        0        0       25 2022-10-12 22:22:32.063966 fastapi_resources-0.3.5/fastapi_resources/resources/sqlmodel/__init__.py
--rw-r--r--   0        0        0    10046 2023-01-06 22:31:50.686739 fastapi_resources-0.3.5/fastapi_resources/resources/sqlmodel/base.py
--rw-r--r--   0        0        0       36 2022-10-13 20:31:29.502194 fastapi_resources-0.3.5/fastapi_resources/resources/sqlmodel/exceptions.py
--rw-r--r--   0        0        0     6902 2023-01-06 20:42:38.810731 fastapi_resources-0.3.5/fastapi_resources/resources/sqlmodel/mixins.py
--rw-r--r--   0        0        0      582 2023-01-06 19:52:01.912652 fastapi_resources-0.3.5/fastapi_resources/resources/sqlmodel/paginators.py
--rw-r--r--   0        0        0      745 2022-10-13 19:16:01.780931 fastapi_resources-0.3.5/fastapi_resources/resources/sqlmodel/resources.py
--rw-r--r--   0        0        0     2352 2023-01-04 22:45:54.021176 fastapi_resources-0.3.5/fastapi_resources/resources/sqlmodel/types.py
--rw-r--r--   0        0        0     1808 2023-01-04 20:57:27.498669 fastapi_resources-0.3.5/fastapi_resources/resources/types.py
--rw-r--r--   0        0        0       91 2022-10-05 19:53:19.151384 fastapi_resources-0.3.5/fastapi_resources/routers/__init__.py
--rw-r--r--   0        0        0    11590 2023-03-16 17:43:41.041072 fastapi_resources-0.3.5/fastapi_resources/routers/base_router.py
--rw-r--r--   0        0        0      859 2023-01-04 21:47:54.786676 fastapi_resources-0.3.5/fastapi_resources/routers/decorators.py
--rw-r--r--   0        0        0       51 2022-10-12 22:33:19.044947 fastapi_resources-0.3.5/fastapi_resources/routers/json_api_router/__init__.py
--rw-r--r--   0        0        0    17503 2023-03-16 17:44:03.111528 fastapi_resources-0.3.5/fastapi_resources/routers/json_api_router/json_api_router.py
--rw-r--r--   0        0        0     2578 2023-01-04 22:20:34.640894 fastapi_resources-0.3.5/fastapi_resources/routers/json_api_router/types.py
--rw-r--r--   0        0        0        0 2022-10-05 19:53:19.152483 fastapi_resources-0.3.5/fastapi_resources/types.py
--rw-r--r--   0        0        0      609 2023-03-16 17:46:47.094968 fastapi_resources-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 fastapi_resources-0.3.5/setup.py
--rw-r--r--   0        0        0      383 1970-01-01 00:00:00.000000 fastapi_resources-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-05 19:53:19.150339 fastapi_resources-0.4.0/fastapi_resources/__init__.py
+-rw-r--r--   0        0        0       26 2023-07-09 18:36:12.306946 fastapi_resources-0.4.0/fastapi_resources/resources/__init__.py
+-rw-r--r--   0        0        0     3426 2023-07-09 20:12:25.173070 fastapi_resources-0.4.0/fastapi_resources/resources/base_resource.py
+-rw-r--r--   0        0        0       25 2022-10-12 22:22:32.063966 fastapi_resources-0.4.0/fastapi_resources/resources/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     9932 2023-07-10 03:48:15.896523 fastapi_resources-0.4.0/fastapi_resources/resources/sqlalchemy/base.py
+-rw-r--r--   0        0        0       36 2022-10-13 20:31:29.502194 fastapi_resources-0.4.0/fastapi_resources/resources/sqlalchemy/exceptions.py
+-rw-r--r--   0        0        0     6955 2023-07-09 19:11:08.139363 fastapi_resources-0.4.0/fastapi_resources/resources/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0      553 2023-07-09 19:16:18.892879 fastapi_resources-0.4.0/fastapi_resources/resources/sqlalchemy/paginators.py
+-rw-r--r--   0        0        0      777 2023-07-09 19:16:11.998943 fastapi_resources-0.4.0/fastapi_resources/resources/sqlalchemy/resources.py
+-rw-r--r--   0        0        0     2405 2023-07-09 19:15:42.380538 fastapi_resources-0.4.0/fastapi_resources/resources/sqlalchemy/types.py
+-rw-r--r--   0        0        0     1808 2023-01-04 20:57:27.498669 fastapi_resources-0.4.0/fastapi_resources/resources/types.py
+-rw-r--r--   0        0        0       91 2022-10-05 19:53:19.151384 fastapi_resources-0.4.0/fastapi_resources/routers/__init__.py
+-rw-r--r--   0        0        0    11622 2023-07-10 03:48:20.095838 fastapi_resources-0.4.0/fastapi_resources/routers/base_router.py
+-rw-r--r--   0        0        0      859 2023-01-04 21:47:54.786676 fastapi_resources-0.4.0/fastapi_resources/routers/decorators.py
+-rw-r--r--   0        0        0       51 2022-10-12 22:33:19.044947 fastapi_resources-0.4.0/fastapi_resources/routers/json_api_router/__init__.py
+-rw-r--r--   0        0        0    17591 2023-07-10 03:43:15.272658 fastapi_resources-0.4.0/fastapi_resources/routers/json_api_router/json_api_router.py
+-rw-r--r--   0        0        0     2452 2023-07-10 02:53:21.921955 fastapi_resources-0.4.0/fastapi_resources/routers/json_api_router/types.py
+-rw-r--r--   0        0        0        0 2022-10-05 19:53:19.152483 fastapi_resources-0.4.0/fastapi_resources/types.py
+-rw-r--r--   0        0        0      651 2023-07-10 17:31:01.101926 fastapi_resources-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 fastapi_resources-0.4.0/PKG-INFO
```

### Comparing `fastapi_resources-0.3.5/fastapi_resources/resources/base_resource.py` & `fastapi_resources-0.4.0/fastapi_resources/resources/base_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,11 +103,11 @@
 
     @classmethod
     def get_relationships(cls) -> Relationships:
         return {}
 
     @classmethod
     def get_attributes(cls) -> set[str]:
-        return set(cls.Db.__fields__.keys())
+        return set(cls.Db.model_fields.keys())
 
     def get_related(self, obj: BaseModel, inclusion: list[str]) -> list[SelectedObj]:
         raise NotImplementedError()
```

### Comparing `fastapi_resources-0.3.5/fastapi_resources/resources/sqlmodel/base.py` & `fastapi_resources-0.4.0/fastapi_resources/resources/sqlalchemy/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 import copy
 from typing import Any, ClassVar, Generic, Optional, Type
 
-from fastapi import HTTPException
-from sqlalchemy.orm import MANYTOONE
-from sqlalchemy.orm import exc as sa_exceptions
-from sqlalchemy.orm import joinedload
-from sqlmodel import Session, SQLModel, func, select, text, update
-from sqlmodel.sql.expression import SelectOfScalar
+from sqlalchemy import exc as sa_exceptions
+from sqlalchemy import func, inspect, select
+from sqlalchemy.orm import MANYTOONE, DeclarativeBase, Session, joinedload
 
 from fastapi_resources.resources import base_resource
-from fastapi_resources.resources.sqlmodel.exceptions import NotFound
+from fastapi_resources.resources.sqlalchemy.exceptions import NotFound
 
 from . import types
 
 
 def get_relationships_from_schema(
-    schema: Type[SQLModel],
+    schema: Type[DeclarativeBase],
     schema_cache: Optional[
         dict[
-            tuple[Optional[str], Type[SQLModel]],
+            tuple[Optional[str], Type[DeclarativeBase]],
             types.SchemaWithRelationships,
         ]
     ] = None,
     immediate_parent_backpopulated_field: Optional[str] = None,
     parent_key: Optional[str] = None,
 ):
     schema_cache = schema_cache or {}
 
-    relationship_fields = schema.__sqlmodel_relationships__.keys()
     relationships = {}
 
     parent_schema_with_relationships = types.SchemaWithRelationships(
         schema=schema,
         relationships=relationships,
     )
 
     # Just a sanity check. This function should never be called for a relationship
     # that already exists.
     assert (parent_key, schema) not in schema_cache
 
     schema_cache[(parent_key, schema)] = parent_schema_with_relationships
 
-    for field in relationship_fields:
-        sqlalchemy_relationship = getattr(schema, field).property
+    for field, sqlalchemy_relationship in inspect(schema).relationships.items():
         related_schema = sqlalchemy_relationship.mapper.class_
         many = sqlalchemy_relationship.uselist
 
         # Used to uniquely identify the related schema relative to a parent
         new_parent_key = f"{schema}.{field}"
 
         # TODO: Handle MANYTOMANY
@@ -56,29 +51,30 @@
             if direction == MANYTOONE
             else sqlalchemy_relationship.remote_side
         )[0].name
 
         # If this branch already contains the schema with the same parent,
         # we can reuse the relationship to avoid a cycle.
         if relationship_info := schema_cache.get((new_parent_key, related_schema)):
-            relationships[field] = types.SQLModelRelationshipInfo(
+            relationships[field] = types.SQLAlchemyRelationshipInfo(
                 schema_with_relationships=relationship_info,
                 many=many,
                 field=field,
                 direction=direction,
                 update_field=update_field,
             )
             continue
 
         # For any relationship, the child will have a backpopulated reference
         # to the parent; we want to exclude that from available relationships
         if field == immediate_parent_backpopulated_field:
             continue
 
-        backpopulated_field = schema.__sqlmodel_relationships__[field].back_populates
+        # TODO: Can we cache the relationships when added to the registry?
+        backpopulated_field = inspect(schema).relationships[field].back_populates
 
         get_relationships_from_schema(
             schema=related_schema,
             schema_cache=schema_cache,
             immediate_parent_backpopulated_field=backpopulated_field,
             parent_key=new_parent_key,
         )
@@ -87,40 +83,40 @@
         # will have been created. But we want to use it without having
         # to return the object, so we just grab it from cache. A cleaner
         # solution is to overload the signature based on whether
         # `parent_field` is passed in,
         schema_with_relationship = schema_cache.get((new_parent_key, related_schema))
         assert schema_with_relationship
 
-        relationships[field] = types.SQLModelRelationshipInfo(
+        relationships[field] = types.SQLAlchemyRelationshipInfo(
             schema_with_relationships=schema_with_relationship,
             many=many,
             field=field,
             direction=direction,
             update_field=update_field,
         )
 
     return relationships
 
 
-class BaseSQLResource(
+class BaseSQLAlchemyResource(
     base_resource.Resource[types.TDb],
-    types.SQLResourceProtocol[types.TDb],
+    types.SQLAlchemyResourceProtocol[types.TDb],
     Generic[types.TDb],
 ):
-    registry: dict[Type[SQLModel], type["BaseSQLResource"]] = {}
+    registry: dict[Type[DeclarativeBase], type["BaseSQLAlchemyResource"]] = {}
 
     Paginator: ClassVar[Optional[Type[types.PaginatorProtocol]]]
     paginator: Optional[types.PaginatorProtocol]
 
     id_field: Optional[str] = None
 
     def __init_subclass__(cls) -> None:
         if Db := getattr(cls, "Db", None):
-            BaseSQLResource.registry[Db] = cls
+            BaseSQLAlchemyResource.registry[Db] = cls
 
         return super().__init_subclass__()
 
     def __init__(
         self,
         session: Session = None,
         inclusions: Optional[types.Inclusions] = None,
@@ -152,32 +148,33 @@
         TODO: Have the relationship point to the resource, rather than the schema. Use
             the registry to lookup the related resource.
 
         Used to:
           - Validate a given inclusion resolves to a relationship (done in the base class)
           - To retrieve all the objects along an inclusion with their schemas
         """
-        read_fields = set(cls.Read.__fields__.keys())
-        read_fields.update(cls.Read.__sqlmodel_relationships__.keys())
+        read_fields = set(getattr(cls.Read, "__relationships__", set()))
+
         relationships = get_relationships_from_schema(schema=cls.Db)
 
         return {
             name: info for name, info in relationships.items() if name in read_fields
         }
 
     @classmethod
     def get_attributes(cls) -> set[str]:
         attributes = set()
+        relationships = cls.get_relationships()
 
         # These are the fields according to the pydantic model
-        fields = cls.Read.schema().get("properties", {})
+        fields = cls.Read.model_fields
         for field in fields:
             # If the field refers to a foreign key field we skip it as it'll be
             # included in get_relationships.
-            if getattr(cls.Db, field).expressions[0].foreign_keys:
+            if field in relationships:
                 continue
 
             attributes.add(field)
 
         return attributes
 
     # TODO: Update to a type from sqlalchemy when we require 2.0
@@ -242,15 +239,15 @@
         id: int | str,
     ) -> types.TDb:
         select = self.get_select()
 
         id_field = getattr(self.Db, self.id_field or "id")
 
         try:
-            return self.session.exec(select.where(id_field == id)).unique().one()
+            return self.session.scalars(select.where(id_field == id)).unique().one()
         except sa_exceptions.NoResultFound:
             raise NotFound(f"{self.name} not found")
 
     def get_related(
         self,
         obj: types.TDb,
         inclusion: list[str],
@@ -271,15 +268,15 @@
 
             selected_objs = (
                 selected_objs if isinstance(selected_objs, list) else [selected_objs]
             )
 
             selected_objs = [
                 types.SelectedObj(
-                    obj=selected_obj, resource=BaseSQLResource.registry[schema]
+                    obj=selected_obj, resource=BaseSQLAlchemyResource.registry[schema]
                 )
                 for selected_obj in selected_objs
             ]
 
             if next_inclusion:
                 selected_objs = [
                     *selected_objs,
```

### Comparing `fastapi_resources-0.3.5/fastapi_resources/resources/sqlmodel/mixins.py` & `fastapi_resources-0.4.0/fastapi_resources/resources/sqlalchemy/mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Optional
 
+from sqlalchemy import select, update
 from sqlalchemy.orm import MANYTOONE, ONETOMANY
-from sqlmodel import select, update
 
-from fastapi_resources.resources.sqlmodel import types
-from fastapi_resources.resources.sqlmodel.exceptions import NotFound
+from fastapi_resources.resources.sqlalchemy import types
+from fastapi_resources.resources.sqlalchemy.exceptions import NotFound
 
 
 class CreateResourceMixin:
     def create(
-        self: types.SQLResourceProtocol[types.TDb],
+        self: types.SQLAlchemyResourceProtocol[types.TDb],
         attributes: dict,
         relationships: Optional[dict[str, str | int | list[str | int]]] = None,
         **kwargs,
     ):
         row = self.Db(**attributes)
 
         for key, value in kwargs.items():
@@ -35,15 +35,15 @@
                 related_ids if isinstance(related_ids, list) else [related_ids]
             )
 
             # Do a select to check we have permission
             related_resource = RelatedResource(context=self.context)
 
             if related_where := related_resource.get_where():
-                results = self.session.exec(
+                results = self.session.scalars(
                     select(related_db_model).where(
                         related_db_model.id.in_(new_related_ids), *related_where
                     )
                 ).all()
 
                 if len(results) != len(new_related_ids):
                     raise NotFound()
@@ -88,15 +88,15 @@
             self.session.refresh(row)
 
         return row
 
 
 class UpdateResourceMixin:
     def update(
-        self: types.SQLResourceProtocol[types.TDb],
+        self: types.SQLAlchemyResourceProtocol[types.TDb],
         *,
         id: int | str,
         attributes: dict,
         relationships: Optional[dict[str, str | int | list[str | int]]] = None,
         **kwargs,
     ):
         row = self.get_object(id=id)
@@ -119,15 +119,15 @@
                     related_ids if isinstance(related_ids, list) else [related_ids]
                 )
 
                 # Do a select to check we have permission
                 related_resource = RelatedResource(context=self.context)
 
                 if related_where := related_resource.get_where():
-                    results = self.session.exec(
+                    results = self.session.scalars(
                         select(related_db_model).where(
                             related_db_model.id.in_(new_related_ids), *related_where
                         )
                     ).all()
 
                     if len(results) != len(new_related_ids):
                         raise NotFound(f"{related_resource.name} not found")
@@ -163,41 +163,41 @@
         self.session.commit()
         self.session.refresh(row)
 
         return row
 
 
 class ListResourceMixin:
-    def list(self: types.SQLResourceProtocol[types.TDb]):
+    def list(self: types.SQLAlchemyResourceProtocol[types.TDb]):
         select = self.get_select()
 
         paginator = getattr(self, "paginator", None)
 
         if paginator:
             select = paginator.paginate_select(select)
 
-        rows = self.session.exec(select).unique().all()
-        count = self.session.exec(self.get_count_select()).one()
+        rows = self.session.scalars(select).unique().all()
+        count = self.session.scalars(self.get_count_select()).one()
 
         next = None
 
         if paginator:
             next = paginator.get_next(count=count)
 
         return rows, next, count
 
 
 class RetrieveResourceMixin:
-    def retrieve(self: types.SQLResourceProtocol[types.TDb], *, id: int | str):
+    def retrieve(self: types.SQLAlchemyResourceProtocol[types.TDb], *, id: int | str):
         row = self.get_object(id=id)
 
         return row
 
 
 class DeleteResourceMixin:
-    def delete(self: types.SQLResourceProtocol[types.TDb], *, id: int | str):
+    def delete(self: types.SQLAlchemyResourceProtocol[types.TDb], *, id: int | str):
         row = self.get_object(id=id)
 
         self.session.delete(row)
         self.session.commit()
 
         return {"ok": True}
```

### Comparing `fastapi_resources-0.3.5/fastapi_resources/resources/sqlmodel/paginators.py` & `fastapi_resources-0.4.0/fastapi_resources/resources/sqlalchemy/paginators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Optional
 
-from sqlmodel.sql.expression import SelectOfScalar
+from sqlalchemy import Select
 
 
 class LimitOffsetPaginator:
     def __init__(self, cursor: Optional[str] = None, limit: Optional[int] = None):
         self.page = int(cursor) if cursor else 1
         self.limit = limit or 20
 
-    def paginate_select(self, select: SelectOfScalar):
+    def paginate_select(self, select: Select):
         return select.limit(self.limit).offset((self.page - 1) * self.limit)
 
     def get_next(self, count: int):
         current_max = self.page * self.limit
 
         if count > current_max:
             return str(self.page + 1)
```

### Comparing `fastapi_resources-0.3.5/fastapi_resources/resources/sqlmodel/resources.py` & `fastapi_resources-0.4.0/fastapi_resources/resources/sqlalchemy/resources.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from typing import Generic
 
 from . import base, mixins, types
 
 __all__ = [
     "ListCreateResource",
     "ListCreateUpdateResource",
-    "SQLModelResource",
+    "SQLAlchemyResource",
 ]
 
 
 class ListCreateResource(
-    mixins.CreateResourceMixin, mixins.ListResourceMixin, base.BaseSQLResource
+    mixins.CreateResourceMixin, mixins.ListResourceMixin, base.BaseSQLAlchemyResource
 ):
     pass
 
 
 class ListCreateUpdateResource(
     mixins.ListResourceMixin,
     mixins.CreateResourceMixin,
     mixins.UpdateResourceMixin,
-    base.BaseSQLResource,
+    base.BaseSQLAlchemyResource,
 ):
     pass
 
 
-class SQLModelResource(
+class SQLAlchemyResource(
     mixins.RetrieveResourceMixin,
     mixins.ListResourceMixin,
     mixins.CreateResourceMixin,
     mixins.UpdateResourceMixin,
     mixins.DeleteResourceMixin,
-    base.BaseSQLResource[types.TDb],
-    types.SQLResourceProtocol[types.TDb],
+    base.BaseSQLAlchemyResource[types.TDb],
+    types.SQLAlchemyResourceProtocol[types.TDb],
     Generic[types.TDb],
 ):
     pass
```

### Comparing `fastapi_resources-0.3.5/fastapi_resources/resources/types.py` & `fastapi_resources-0.4.0/fastapi_resources/resources/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.3.5/fastapi_resources/routers/base_router.py` & `fastapi_resources-0.4.0/fastapi_resources/routers/base_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     runtime_checkable,
 )
 
 from fastapi import APIRouter, BackgroundTasks, HTTPException, Request, Response
 from fastapi.routing import APIRoute
 from pydantic import BaseModel
 
-from fastapi_resources.resources.sqlmodel.exceptions import NotFound
+from fastapi_resources.resources.sqlalchemy.exceptions import NotFound
 from fastapi_resources.resources.types import ResourceProtocol
 from fastapi_resources.routers import decorators
 
 
 class TCreatePayload(BaseModel):
     pass
 
@@ -281,15 +281,16 @@
 
     async def _retrieve(self, *, id: Union[int, str], request: Request):
         resource = self.get_resource(request=request)
         if not resource.retrieve:
             raise NotImplementedError("Resource.retrieve not implemented")
 
         row = resource.retrieve(id=id)
-        return self.build_response(rows=row, resource=resource, request=request)
+        res = self.build_response(rows=row, resource=resource, request=request)
+        return res
 
     async def _list(self, *, request: Request):
         resource = self.get_resource(request=request)
         if not resource.list:
             raise NotImplementedError("Resource.list not implemented")
 
         # Next and count are ignored in the base router
@@ -305,15 +306,15 @@
         create: TCreatePayload,
         request: Request,
         background_tasks: BackgroundTasks,
     ):
         resource = self.get_resource(request=request)
 
         attributes, relationships = self.parse_update(
-            resource=resource, update=create.dict(exclude_unset=True)
+            resource=resource, update=create.model_dump(exclude_unset=True)
         )
 
         row = self.perform_create(
             request=request,
             resource=resource,
             attributes=attributes,
             relationships=relationships,
@@ -338,15 +339,15 @@
         update: TUpdatePayload,
         request: Request,
         background_tasks: BackgroundTasks,
     ):
         resource = self.get_resource(request=request)
 
         attributes, relationships = self.parse_update(
-            resource=resource, update=update.dict(exclude_unset=True)
+            resource=resource, update=update.model_dump(exclude_unset=True)
         )
         row = self.perform_update(
             request=request,
             resource=resource,
             attributes=attributes,
             relationships=relationships,
             id=id,
```

### Comparing `fastapi_resources-0.3.5/fastapi_resources/routers/decorators.py` & `fastapi_resources-0.4.0/fastapi_resources/routers/decorators.py`

 * *Files identical despite different names*

### Comparing `fastapi_resources-0.3.5/fastapi_resources/routers/json_api_router/json_api_router.py` & `fastapi_resources-0.4.0/fastapi_resources/routers/json_api_router/json_api_router.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from typing import Callable, List, Literal, Optional, Type, TypeVar, Union
 
 from fastapi import BackgroundTasks, HTTPException, Query, Request, Response
 from fastapi.exceptions import RequestValidationError
 from fastapi.responses import JSONResponse
 from pydantic import create_model
-from pydantic.main import BaseModel, ModelMetaclass
+from pydantic.main import BaseModel
 
 from fastapi_resources.resources.types import (
     Inclusions,
     RelationshipInfo,
     Relationships,
     ResourceProtocol,
 )
 from fastapi_resources.routers import base_router
 
 from . import types
 
-include_query = Query(None, regex=r"^([\w\.]+)(,[\w\.]+)*$")
+include_query = Query(None, pattern=r"^([\w\.]+)(,[\w\.]+)*$")
 
 
 TResource = TypeVar("TResource", bound=ResourceProtocol)
 
 
 def get_schemas_from_relationships(
-    relationships: Relationships, visited: Optional[set[type[types.Object]]] = None
-) -> list[tuple[str, ModelMetaclass]]:
-    schemas: list[tuple[str, ModelMetaclass]] = []
+    relationships: Relationships, visited: Optional[set[Type[BaseModel]]] = None
+) -> list[tuple[str, type[BaseModel]]]:
+    schemas: list[tuple[str, Type[BaseModel]]] = []
 
     visited = visited or set()
     for relationship_info in relationships.values():
         schema = relationship_info.schema_with_relationships.schema
         if schema in visited:
             continue
 
@@ -42,16 +42,15 @@
 
     return schemas
 
 
 def get_relationships_model_for_model(
     method: str, resource_class: type[TResource], model: type[BaseModel]
 ):
-    allowed_fields = set(model.__fields__.keys())
-    allowed_fields.update(model.__sqlmodel_relationships__.keys())
+    allowed_fields = set(getattr(model, "__relationships__", set()))
 
     RelationshipLinkages = {
         relationship_name: (
             Optional[
                 create_model(
                     f"{model.__name__}__{method}__Relationships{relationship_name}",
                     __base__=(
@@ -84,19 +83,22 @@
 
     return Relationships
 
 
 def get_attributes_model_for_model(
     method: str, model: type[BaseModel], resource_class: type[TResource]
 ):
-    Attributes = create_model(f"{model.__name__}__{method}__Attributes", __base__=model)
-
-    # Remove the ID
-    if "id" in Attributes.__fields__:
-        del Attributes.__fields__["id"]
+    base_model_fields = {
+        name: (field.annotation, field)
+        for name, field in model.model_fields.items()
+        if name != "id"
+    }
+    Attributes = create_model(
+        f"{model.__name__}__{method}__Attributes", **base_model_fields
+    )
 
     return Attributes
 
 
 def get_model_for_resource_class(
     method: str, model: type[BaseModel], resource_class: type[TResource]
 ):
@@ -372,34 +374,37 @@
             relationships[relationship_name] = relationship_object
 
         # If the relationship is to-one, then we can include `data`
         # But for to-many, we only include it if it's in inclusions.
         return relationships
 
     def build_resource_object(self, obj: types.Object, resource: TResource):
+        pydantic_object = resource.Read.model_validate(
+            obj, from_attributes=True, strict=False
+        )
+
         valid_attributes = resource.get_attributes()
-        pydantic_object = resource.Read.from_orm(obj)
 
         # ID is a special case, so can ignored
         if "id" in valid_attributes:
             valid_attributes.remove("id")
 
         # Filter out relationships attributes
         attributes = {
             key: value
-            for key, value in pydantic_object.dict().items()
+            for key, value in pydantic_object.model_dump().items()
             if key in valid_attributes
         }
 
         resource_object = types.JAResourceObject(
-            id=pydantic_object.id,
+            id=str(pydantic_object.id),
             type=resource.name,
             attributes=attributes,
             links=self.build_resource_object_links(
-                id=pydantic_object.id, resource=resource
+                id=str(pydantic_object.id), resource=resource
             ),
             relationships=self.build_resource_object_relationships(
                 obj=obj, resource=resource
             ),
         )
 
         return resource_object
```

### Comparing `fastapi_resources-0.3.5/fastapi_resources/routers/json_api_router/types.py` & `fastapi_resources-0.4.0/fastapi_resources/routers/json_api_router/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Generic, List, Optional, TypeVar, Union
 
 from pydantic import BaseModel
-from pydantic.generics import GenericModel
 
 
 class Object(BaseModel):
     id: str
 
 
 TRead = TypeVar("TRead", bound=Object)
@@ -23,78 +22,76 @@
     pass
 
 
 class JALinks(BaseModel):
     """A links-object"""
 
     self: Optional[str] = ""
-    # Will be used when relationship endpoints are implemented
-    related: Optional[str] = ""
 
 
 class JALinksWithPagination(JALinks):
     next: Optional[str] = None
 
 
 TLinks = TypeVar("TLinks", bound=Union[JALinks, JALinksWithPagination])
 
 
-class JAResourceIdentifierObject(GenericModel, Generic[TType]):
+class JAResourceIdentifierObject(BaseModel, Generic[TType]):
     type: TType
     id: str
 
 
-class JARelationshipsObjectSingle(GenericModel, Generic[TType]):
-    links: Optional[JALinks]
+class JARelationshipsObjectSingle(BaseModel, Generic[TType]):
+    links: Optional[JALinks] = None
     data: Optional[JAResourceIdentifierObject[TType]] = None
 
 
-class JARelationshipsObjectMany(GenericModel, Generic[TType]):
-    links: Optional[JALinks]
+class JARelationshipsObjectMany(BaseModel, Generic[TType]):
+    links: Optional[JALinks] = None
     data: list[JAResourceIdentifierObject[TType]]
 
 
-class JAResourceObject(GenericModel, Generic[TAttributes, TRelationships, TName]):
+class JAResourceObject(BaseModel, Generic[TAttributes, TRelationships, TName]):
     id: str
     type: TName
     attributes: TAttributes
     links: JALinks
     relationships: TRelationships
 
 
-class JAUpdateObject(GenericModel, Generic[TAttributes, TRelationships, TName]):
+class JAUpdateObject(BaseModel, Generic[TAttributes, TRelationships, TName]):
     id: str
     type: TName
-    attributes: Optional[TAttributes]
-    relationships: Optional[TRelationships]
+    attributes: Optional[TAttributes] = None
+    relationships: Optional[TRelationships] = None
 
 
-class JAUpdateRequest(GenericModel, Generic[TAttributes, TRelationships, TName]):
+class JAUpdateRequest(BaseModel, Generic[TAttributes, TRelationships, TName]):
     data: JAUpdateObject[TAttributes, TRelationships, TName]
 
 
-class JACreateObject(GenericModel, Generic[TAttributes, TRelationships, TName]):
+class JACreateObject(BaseModel, Generic[TAttributes, TRelationships, TName]):
     type: TName
-    attributes: Optional[TAttributes]
-    relationships: Optional[TRelationships]
+    attributes: Optional[TAttributes] = None
+    relationships: Optional[TRelationships] = None
 
 
-class JACreateRequest(GenericModel, Generic[TAttributes, TRelationships, TName]):
+class JACreateRequest(BaseModel, Generic[TAttributes, TRelationships, TName]):
     data: JACreateObject[TAttributes, TRelationships, TName]
 
 
 class JAResponseSingle(
-    GenericModel, Generic[TAttributes, TRelationships, TName, TIncluded]
+    BaseModel, Generic[TAttributes, TRelationships, TName, TIncluded]
 ):
     data: JAResourceObject[TAttributes, TRelationships, TName]
     included: TIncluded
     links: JALinks
 
 
 class JAResponseList(
-    GenericModel,
+    BaseModel,
     Generic[TAttributes, TRelationships, TName, TIncluded, TMeta, TLinks],
 ):
     data: List[JAResourceObject[TAttributes, TRelationships, TName]]
     included: TIncluded
     links: TLinks
     meta: TMeta
```

### Comparing `fastapi_resources-0.3.5/pyproject.toml` & `fastapi_resources-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [tool.poetry]
 name = "fastapi-resources"
-version = "0.3.5"
+version = "0.4.0"
 description = ""
 authors = ["Ben Davis <ben@bencdavis.com>"]
 packages = [
     { include = "fastapi_resources" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-fastapi = "^0.85.0"
-sqlmodel = "^0.0.8"
+fastapi = "^0.100.0"
+sqlalchemy = "^2.0.18"
+pydantic = "^2.0.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 requests = "^2.26.0"
 pytest-clarity = "^1.0.1"
 pytest-watcher = "^0.2.1"
 debugpy = "^1.6.2"
 
 [tool.poetry.group.dev.dependencies]
 dirty-equals = "^0.5.0"
 uvicorn = {extras = ["standard"], version = "^0.15.0"}
+httpx = "^0.24.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```


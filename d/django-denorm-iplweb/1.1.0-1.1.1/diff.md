# Comparing `tmp/django_denorm_iplweb-1.1.0-py3-none-any.whl.zip` & `tmp/django_denorm_iplweb-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 38886 bytes, number of entries: 44
+Zip file size: 39398 bytes, number of entries: 45
 -rw-r--r--  2.0 unx      736 b- defN 21-Sep-29 11:15 denorm/__init__.py
 -rw-r--r--  2.0 unx      493 b- defN 21-Oct-12 09:41 denorm/apps.py
 -rw-r--r--  2.0 unx      692 b- defN 21-Oct-12 09:41 denorm/contextmanagers.py
--rw-r--r--  2.0 unx    30292 b- defN 22-May-07 21:34 denorm/denorms.py
+-rw-r--r--  2.0 unx    30285 b- defN 23-Jul-10 01:18 denorm/denorms.py
 -rw-r--r--  2.0 unx    27369 b- defN 21-Oct-12 09:41 denorm/dependencies.py
--rw-r--r--  2.0 unx    10889 b- defN 21-Oct-12 09:41 denorm/fields.py
+-rw-r--r--  2.0 unx    10953 b- defN 23-Jul-10 01:36 denorm/fields.py
 -rw-r--r--  2.0 unx     2056 b- defN 21-Oct-12 09:41 denorm/helpers.py
 -rw-r--r--  2.0 unx     1074 b- defN 21-Oct-12 09:41 denorm/middleware.py
 -rw-r--r--  2.0 unx     5950 b- defN 22-Jul-07 21:53 denorm/models.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Oct-12 09:41 denorm/conf/__init__.py
 -rw-r--r--  2.0 unx      294 b- defN 21-Oct-12 12:24 denorm/conf/settings.py
 -rw-r--r--  2.0 unx      874 b- defN 21-Oct-12 09:41 denorm/db/__init__.py
 -rw-r--r--  2.0 unx     9463 b- defN 21-Oct-12 09:41 denorm/db/base.py
@@ -32,15 +32,16 @@
 -rw-r--r--  2.0 unx     1191 b- defN 21-Oct-12 09:41 denorm/migrations/0006_auto_20211003_0346.py
 -rw-r--r--  2.0 unx      399 b- defN 21-Oct-12 09:41 denorm/migrations/0007_auto_created_on_now.py
 -rw-r--r--  2.0 unx      407 b- defN 21-Oct-12 09:41 denorm/migrations/0008_alter_dirtyinstance_object_id.py
 -rw-r--r--  2.0 unx      414 b- defN 21-Oct-12 09:41 denorm/migrations/0009_alter_dirtyinstance_object_id.py
 -rw-r--r--  2.0 unx      417 b- defN 21-Oct-12 09:41 denorm/migrations/0010_alter_dirtyinstance_object_id.py
 -rw-r--r--  2.0 unx      414 b- defN 21-Oct-12 09:41 denorm/migrations/0011_alter_dirtyinstance_object_id.py
 -rw-r--r--  2.0 unx      417 b- defN 21-Oct-12 09:41 denorm/migrations/0012_alter_dirtyinstance_object_id.py
+-rw-r--r--  2.0 unx      431 b- defN 23-Jul-10 01:11 denorm/migrations/0013_alter_dirtyinstance_success.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-29 11:15 denorm/migrations/__init__.py
--rw-r--r--  2.0 unx      276 b- defN 22-Jul-07 21:55 django_denorm_iplweb-1.1.0.dist-info/AUTHORS.txt
--rw-r--r--  2.0 unx     2985 b- defN 22-Jul-07 21:55 django_denorm_iplweb-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      666 b- defN 22-Jul-07 21:55 django_denorm_iplweb-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-07 21:55 django_denorm_iplweb-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 22-Jul-07 21:55 django_denorm_iplweb-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4036 b- defN 22-Jul-07 21:55 django_denorm_iplweb-1.1.0.dist-info/RECORD
-44 files, 123085 bytes uncompressed, 32278 bytes compressed:  73.8%
+-rw-r--r--  2.0 unx      276 b- defN 23-Jul-10 07:22 django_denorm_iplweb-1.1.1.dist-info/AUTHORS.txt
+-rw-r--r--  2.0 unx     2985 b- defN 23-Jul-10 07:22 django_denorm_iplweb-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      630 b- defN 23-Jul-10 07:22 django_denorm_iplweb-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 07:22 django_denorm_iplweb-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-10 07:22 django_denorm_iplweb-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4145 b- defN 23-Jul-10 07:22 django_denorm_iplweb-1.1.1.dist-info/RECORD
+45 files, 123646 bytes uncompressed, 32608 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -105,29 +105,32 @@
 
 Filename: denorm/migrations/0011_alter_dirtyinstance_object_id.py
 Comment: 
 
 Filename: denorm/migrations/0012_alter_dirtyinstance_object_id.py
 Comment: 
 
+Filename: denorm/migrations/0013_alter_dirtyinstance_success.py
+Comment: 
+
 Filename: denorm/migrations/__init__.py
 Comment: 
 
-Filename: django_denorm_iplweb-1.1.0.dist-info/AUTHORS.txt
+Filename: django_denorm_iplweb-1.1.1.dist-info/AUTHORS.txt
 Comment: 
 
-Filename: django_denorm_iplweb-1.1.0.dist-info/LICENSE
+Filename: django_denorm_iplweb-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: django_denorm_iplweb-1.1.0.dist-info/METADATA
+Filename: django_denorm_iplweb-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: django_denorm_iplweb-1.1.0.dist-info/WHEEL
+Filename: django_denorm_iplweb-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: django_denorm_iplweb-1.1.0.dist-info/top_level.txt
+Filename: django_denorm_iplweb-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: django_denorm_iplweb-1.1.0.dist-info/RECORD
+Filename: django_denorm_iplweb-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## denorm/denorms.py

```diff
@@ -1,16 +1,24 @@
-# -*- coding: utf-8 -*-
 import abc
 import logging
 import traceback
 from itertools import islice
 
 from django.apps import apps
 from django.contrib import contenttypes
 from django.core.exceptions import FieldDoesNotExist
+
+try:
+    from django.core.exceptions import FullResultSet
+except ImportError:
+
+    class FullResultSet(Exception):
+        pass
+
+
 from django.db import OperationalError, connection, connections, transaction
 from django.db.models import ManyToManyField, sql
 from django.db.models.aggregates import Sum
 from django.db.models.manager import Manager
 from django.db.models.query_utils import Q
 from django.db.models.sql.compiler import SQLCompiler
 from django.db.models.sql.datastructures import Join
@@ -81,15 +89,15 @@
             for field in model._meta.fields:
                 if hasattr(field, "denorm"):
                     if not field.denorm.model._meta.swapped:
                         alldenorms.append(field.denorm)
     return alldenorms
 
 
-class Denorm(object):
+class Denorm:
     def __init__(self, skip=None, only=None):
         self.func = None
         self.skip = skip
         self.only = only
 
     def get_quote_name(self, using):
         if using:
@@ -118,16 +126,16 @@
         # only write new values to the DB if they actually changed
         new_value = self.func(instance)
 
         if isinstance(attr, Manager):
             # for a many to many field the decorated
             # function should return a list of either model instances
             # or primary keys
-            old_pks = set([x.pk for x in attr.all()])
-            new_pks = set([])
+            old_pks = {x.pk for x in attr.all()}
+            new_pks = set()
 
             for x in new_value:
                 # we need to compare sets of objects based on pk values,
                 # as django lacks an identity map.
                 if hasattr(x, "pk"):
                     new_pks.add(x.pk)
                 else:
@@ -157,15 +165,15 @@
     as a callback.
     """
 
     def setup(self, **kwargs):
         """
         Calls setup() on all DenormDependency resolvers
         """
-        super(BaseCallbackDenorm, self).setup(**kwargs)
+        super().setup(**kwargs)
 
         for dependency in self.depend:
             dependency.setup(self.model)
 
     def get_triggers(self, using):
         """
         Creates a list of all triggers needed to keep track of changes
@@ -173,15 +181,15 @@
         """
         trigger_list = list()
 
         # Get the triggers of all DenormDependency instances attached
         # to our callback.
         for dependency in self.depend:
             trigger_list += dependency.get_triggers(using=using)
-        ret = trigger_list + super(BaseCallbackDenorm, self).get_triggers(using=using)
+        ret = trigger_list + super().get_triggers(using=using)
         return ret
 
 
 class CallbackDenorm(BaseCallbackDenorm):
     """
     As above, but with extra triggers on self as described below
     """
@@ -230,30 +238,30 @@
                 content_type,
                 using,
                 self.skip,
                 self.only,
             ),
         ]
 
-        return trigger_list + super(CallbackDenorm, self).get_triggers(using=using)
+        return trigger_list + super().get_triggers(using=using)
 
 
 class BaseCacheKeyDenorm(Denorm):
     def __init__(self, depend_on_related, *args, **kwargs):
         self.depend = depend_on_related
-        super(BaseCacheKeyDenorm, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         import random
 
         self.func = lambda o: random.randint(-9223372036854775808, 9223372036854775807)
 
     def setup(self, **kwargs):
         """
         Calls setup() on all DenormDependency resolvers
         """
-        super(BaseCacheKeyDenorm, self).setup(**kwargs)
+        super().setup(**kwargs)
 
         for dependency in self.depend:
             dependency.setup(self.model)
 
     def get_triggers(self, using):
         """
         Creates a list of all triggers needed to keep track of changes
@@ -262,15 +270,15 @@
         trigger_list = list()
 
         # Get the triggers of all DenormDependency instances attached
         # to our callback.
         for dependency in self.depend:
             trigger_list += dependency.get_triggers(using=using)
 
-        return trigger_list + super(BaseCacheKeyDenorm, self).get_triggers(using=using)
+        return trigger_list + super().get_triggers(using=using)
 
 
 class CacheKeyDenorm(BaseCacheKeyDenorm):
     """
     As above, but with extra triggers on self as described below
     """
 
@@ -313,42 +321,42 @@
                 content_type,
                 using,
                 self.skip,
                 self.only,
             ),
         ]
 
-        return trigger_list + super(CacheKeyDenorm, self).get_triggers(using=using)
+        return trigger_list + super().get_triggers(using=using)
 
 
 class TriggerWhereNode(WhereNode):
     def sql_for_columns(self, data, qn, connection, internal_type=None):
         """
         Returns the SQL fragment used for the left-hand side of a column
         constraint (for example, the "T1.foo" portion in the clause
         "WHERE ... T1.foo = 6").
         """
         table_alias, name, db_type = data
         if table_alias:
             if table_alias in ("NEW", "OLD"):
-                lhs = "%s.%s" % (table_alias, qn(name))
+                lhs = f"{table_alias}.{qn(name)}"
             else:
-                lhs = "%s.%s" % (qn(table_alias), qn(name))
+                lhs = f"{qn(table_alias)}.{qn(name)}"
         else:
             lhs = qn(name)
         try:
             response = connection.ops.field_cast_sql(db_type, internal_type) % lhs
         except TypeError:
             response = connection.ops.field_cast_sql(db_type) % lhs
         return response
 
 
 class TriggerFilterQuery(sql.Query):
     def __init__(self, model, trigger_alias, where=TriggerWhereNode):
-        super(TriggerFilterQuery, self).__init__(model, where)
+        super().__init__(model, where)
         self.trigger_alias = trigger_alias
         try:
 
             class JoinField:
                 def get_joining_columns(self):
                     return None
 
@@ -369,15 +377,15 @@
         self.skip = skip
         self.only = only
 
     def setup(self, sender, **kwargs):
         # as we connected to the ``class_prepared`` signal for any sender
         # and we only need to setup once, check if the sender is our model.
         if sender is self.model:
-            super(AggregateDenorm, self).setup(sender=sender, **kwargs)
+            super().setup(sender=sender, **kwargs)
 
         # related managers will only be available after both models are initialized
         # so check if its available already, and get our manager
         if not self.manager and hasattr(self.model, str(self.manager_name)):
             self.manager = getattr(self.model, self.manager_name)
 
     def get_related_where(self, fk_name, using, type):
@@ -495,36 +503,42 @@
                     "reverse_related": qn(fk_name),
                 }
             ]
             dec_where = [action.replace("NEW.", "OLD.") for action in inc_where]
         else:
             pk_name = qn(self.model._meta.pk.get_attname_column()[1])
             fk_name = qn(related_field.attname)
-            inc_where = ["%s = NEW.%s" % (pk_name, fk_name)]
-            dec_where = ["%s = OLD.%s" % (pk_name, fk_name)]
+            inc_where = [f"{pk_name} = NEW.{fk_name}"]
+            dec_where = [f"{pk_name} = OLD.{fk_name}"]
 
         content_type = str(
             contenttypes.models.ContentType.objects.get_for_model(self.model).pk
         )
 
         if hasattr(self.manager, "field"):  # Django>=1.9
             related_model = self.manager.field.model
         else:  # Django>=1.8
             related_model = self.manager.related.related_model
         inc_query = TriggerFilterQuery(related_model, trigger_alias="NEW")
         inc_query.add_q(Q(**self.filter))
         inc_query.add_q(~Q(**self.exclude))
         qn = SQLCompiler(inc_query, cconnection, using)
-        inc_filter_where, _ = inc_query.where.as_sql(qn, cconnection)
+        try:
+            inc_filter_where, _ = inc_query.where.as_sql(qn, cconnection)
+        except FullResultSet:
+            inc_filter_where, _ = ("", "")
 
         dec_query = TriggerFilterQuery(related_model, trigger_alias="OLD")
         dec_query.add_q(Q(**self.filter))
         dec_query.add_q(~Q(**self.exclude))
         qn = SQLCompiler(dec_query, cconnection, using)
-        dec_filter_where, where_params = dec_query.where.as_sql(qn, cconnection)
+        try:
+            dec_filter_where, where_params = dec_query.where.as_sql(qn, cconnection)
+        except FullResultSet:
+            dec_filter_where, where_params = ("", "")
 
         if inc_filter_where:
             inc_where.append(inc_filter_where)
         if dec_filter_where:
             dec_where.append(dec_filter_where)
             # create the triggers for the incremental updates
         increment = triggers.TriggerActionUpdate(
@@ -590,15 +604,15 @@
 
 class SumDenorm(AggregateDenorm):
     """
     Handles denormalization of a sum field by doing incrementally updates.
     """
 
     def __init__(self, skip=None, field=None):
-        super(SumDenorm, self).__init__(skip)
+        super().__init__(skip)
         # in case we want to set the value without relying on the
         # correctness of the incremental updates we create a function that
         # calculates it from scratch.
         self.sum_field = field
         self.func = lambda obj: (
             getattr(obj, self.manager_name)
             .filter(**self.filter)
@@ -607,20 +621,20 @@
             .values()[0]
             or 0
         )
 
     def get_increment_value(self, using):
         qn = self.get_quote_name(using)
 
-        return "%s + NEW.%s" % (qn(self.fieldname), qn(self.sum_field))
+        return f"{qn(self.fieldname)} + NEW.{qn(self.sum_field)}"
 
     def get_decrement_value(self, using):
         qn = self.get_quote_name(using)
 
-        return "%s - OLD.%s" % (qn(self.fieldname), qn(self.sum_field))
+        return f"{qn(self.fieldname)} - OLD.{qn(self.sum_field)}"
 
     def get_related_increment_value(self, using):
         qn = self.get_quote_name(using)
 
         related_query = Query(self.manager.related.model)
         related_query.add_extra(
             None,
@@ -639,15 +653,15 @@
         )
         related_query.add_fields([self.fieldname])
         related_query.clear_ordering(force_empty=True)
         related_query.default_cols = False
         related_filter_where, related_where_params = related_query.get_compiler(
             using=using
         ).as_sql()
-        return "%s + (%s)" % (qn(self.fieldname), related_filter_where)
+        return f"{qn(self.fieldname)} + ({related_filter_where})"
 
     def get_related_decrement_value(self, using):
         qn = self.get_quote_name(using)
 
         related_query = Query(self.manager.related.model)
         related_query.add_extra(
             None,
@@ -666,25 +680,25 @@
         )
         related_query.add_fields([self.fieldname])
         related_query.clear_ordering(force_empty=True)
         related_query.default_cols = False
         related_filter_where, related_where_params = related_query.get_compiler(
             using=using
         ).as_sql()
-        return "%s - (%s)" % (qn(self.fieldname), related_filter_where)
+        return f"{qn(self.fieldname)} - ({related_filter_where})"
 
 
 class CountDenorm(AggregateDenorm):
     """
     Handles the denormalization of a count field by doing incrementally
     updates.
     """
 
     def __init__(self, skip=None, only=None):
-        super(CountDenorm, self).__init__(skip=skip, only=only)
+        super().__init__(skip=skip, only=only)
         # in case we want to set the value without relying on the
         # correctness of the incremental updates we create a function that
         # calculates it from scratch.
         self.func = (
             lambda obj: getattr(obj, self.manager_name)
             .filter(**self.filter)
             .exclude(**self.exclude)
@@ -734,30 +748,30 @@
     """
 
     alldenorms = get_alldenorms()
     models = {}
     for denorm in alldenorms:
         current_app_label = denorm.model._meta.app_label
         current_model_name = denorm.model._meta.model.__name__
-        current_app_model = "%s.%s" % (current_app_label, current_model_name)
+        current_app_model = f"{current_app_label}.{current_model_name}"
         if model_name is None or model_name.lower() in (
             current_app_label.lower(),
             current_model_name.lower(),
             current_app_model.lower(),
         ):
             if field_name is None or field_name == denorm.fieldname:
                 models.setdefault(denorm.model, []).append(denorm)
 
     i = 0
     for model, denorms in models.items():
         if verbose:
             for denorm in denorms:
                 msg = (
                     "making dirty instances",
-                    "%s/%s" % (i + 1, len(alldenorms)),
+                    f"{i + 1}/{len(alldenorms)}",
                     denorm.fieldname,
                     "in",
                     denorm.model,
                 )
                 logger.info(msg)
                 i += 1
 
@@ -822,15 +836,14 @@
 
     while True:
         cnt += 1
         if cnt == 2 and run_once:
             break
 
         with transaction.atomic():
-
             items_to_process = DirtyInstance.objects.process_next()
             for ctype_id, obj_id in skip_those_ids:
                 # print(f"PID {os.getpid()} skipping {ctype_id, obj_id}")
                 items_to_process = items_to_process.exclude(
                     Q(content_type_id=ctype_id, object_id=obj_id)
                 )
 
@@ -849,15 +862,15 @@
                 dirty_instance.find_similar()
                 .select_for_update(of=("self",), skip_locked=True)
                 .values_list("func_name", flat=True)
             )
 
             if INTERACTIVE:
                 DirtyInstance.objects.dump()
-                breakpoint()
+                breakpoint()  # noqa
 
             try:
                 obj = dirty_instance.content_object_for_update()
             except OperationalError:
                 # This is locked, add tho the list of skipped items
                 elem = (dirty_instance.content_type_id, dirty_instance.object_id)
                 skip_those_ids.append(elem)
```

## denorm/fields.py

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from django.conf import settings
 from django.db import connection, models
 
 from . import denorms
 
 
 def denormalized(DBField, *args, **kwargs):
@@ -60,14 +59,19 @@
             models.signals.post_save.connect(denorms.many_to_many_post_save, sender=cls)
             DBField.contribute_to_class(self, cls, name, *args, **kwargs)
 
         def pre_save(self, model_instance, add):
             """
             Updates the value of the denormalized field before it gets saved.
             """
+            # if not model_instance.pk:
+            #     # Object is not yet created, there is no PK. We are unable to query for
+            #     # the _sets of linked objects or so. We need to return the reasonable default
+            #     return getattr(self, "default")
+
             value = self.denorm.func(model_instance)
 
             if hasattr(self, "remote_field") and self.remote_field:  # Django>=1.10
                 related_field_model = self.remote_field.model
             elif hasattr(self, "related_field"):  # Django>1.5
                 related_field_model = self.related_field.model
             elif hasattr(self, "related"):
@@ -83,15 +87,15 @@
                 setattr(model_instance, self.name, value)
                 return getattr(model_instance, self.attname)
             else:
                 setattr(model_instance, self.attname, value)
                 return value
 
         def deconstruct(self):
-            name, path, args, kwargs = super(DenormDBField, self).deconstruct()
+            name, path, args, kwargs = super().deconstruct()
             super_name, super_path, super_args, super_kwargs = DBField(
                 *args, **kwargs
             ).deconstruct()
             return name, super_path, args, kwargs
 
     def deco(func):
         dbfield = DenormDBField(func, *args, **kwargs)
@@ -136,21 +140,21 @@
         self.denorm = self.get_denorm(skip)
         self.denorm.manager_name = manager_name
         self.denorm.filter = qs_filter
         self.denorm.exclude = qs_exclude
         self.kwargs = kwargs
         kwargs["default"] = 0
         kwargs["editable"] = False
-        super(AggregateField, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def contribute_to_class(self, cls, name, *args, **kwargs):
         self.denorm.model = cls
         self.denorm.fieldname = name
         models.signals.class_prepared.connect(self.denorm.setup)
-        super(AggregateField, self).contribute_to_class(cls, name, *args, **kwargs)
+        super().contribute_to_class(cls, name, *args, **kwargs)
 
     def pre_save(self, model_instance, add):
         """
         Makes sure we never overwrite the count with an outdated value.
         This is necessary because if the count was changed by
         a trigger after this model instance was created, the value
         we would write has not been updated.
@@ -165,15 +169,15 @@
                 flat=True,
             )[0]
 
         setattr(model_instance, self.attname, value)
         return value
 
     def deconstruct(self):
-        name, path, args, kwargs = super(AggregateField, self).deconstruct()
+        name, path, args, kwargs = super().deconstruct()
         del kwargs["editable"]
         args = [self.denorm.manager_name] + args
         return name, path, args, kwargs
 
 
 class CountField(AggregateField):
     """
@@ -198,15 +202,15 @@
         >>> adult_user_count = CountField('user_set', filter={'age__gt':18})
 
         Any additional arguments are passed on to the contructor of
         PositiveIntegerField.
         """
 
         kwargs["editable"] = False
-        super(CountField, self).__init__(manager_name, **kwargs)
+        super().__init__(manager_name, **kwargs)
 
     def get_denorm(self, skip):
         return denorms.CountDenorm(skip)
 
 
 class SumField(AggregateField):
     """
@@ -216,15 +220,15 @@
     are added and removed.
 
     """
 
     def __init__(self, manager_name=None, field=None, **kwargs):
         self.field = field
         kwargs["editable"] = False
-        super(SumField, self).__init__(manager_name, **kwargs)
+        super().__init__(manager_name, **kwargs)
 
     def get_denorm(self, skip):
         return denorms.SumDenorm(skip, self.field)
 
 
 class CacheKeyField(models.BigIntegerField):
     """
@@ -240,15 +244,15 @@
         All arguments are passed on to the contructor of
         BigIntegerField.
         """
         self.dependencies = []
         kwargs["default"] = 0
         kwargs["editable"] = False
         self.kwargs = kwargs
-        super(CacheKeyField, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def depend_on_related(self, *args, **kwargs):
         """
         Add dependency information to the CacheKeyField.
         Accepts the same arguments like the *denorm.depend_on_related* decorator
         """
         from .dependencies import CacheKeyDependOnRelated
@@ -258,23 +262,23 @@
     def contribute_to_class(self, cls, name, *args, **kwargs):
         for depend in self.dependencies:
             depend.fieldname = name
         self.denorm = denorms.BaseCacheKeyDenorm(depend_on_related=self.dependencies)
         self.denorm.model = cls
         self.denorm.fieldname = name
         models.signals.class_prepared.connect(self.denorm.setup)
-        super(CacheKeyField, self).contribute_to_class(cls, name, *args, **kwargs)
+        super().contribute_to_class(cls, name, *args, **kwargs)
 
     def pre_save(self, model_instance, add):
         value = self.denorm.func(model_instance)
         setattr(model_instance, self.attname, value)
         return value
 
 
-class CacheWrapper(object):
+class CacheWrapper:
     def __init__(self, field):
         self.field = field
 
     def __set__(self, obj, value):
         key = "CachedField_%s" % value
         cached = self.field.cache.get(key)
         if not cached:
@@ -283,21 +287,21 @@
         obj.__dict__[self.field.name] = cached
 
 
 class CachedField(CacheKeyField):
     def __init__(self, func=None, cache=None, *args, **kwargs):
         self.func = func
         self.cache = cache
-        super(CachedField, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         if func and cache:
             for c, a, kw in self.func.depend:
                 self.depend_on_related(*a, **kw)
 
     def contribute_to_class(self, cls, name, *args, **kwargs):
-        super(CachedField, self).contribute_to_class(cls, name, *args, **kwargs)
+        super().contribute_to_class(cls, name, *args, **kwargs)
         setattr(cls, self.name, CacheWrapper(self))
 
 
 def cached(cache, *args, **kwargs):
     def deco(func):
         dbfield = CachedField(func, cache, *args, **kwargs)
         return dbfield
```

## Comparing `django_denorm_iplweb-1.1.0.dist-info/LICENSE` & `django_denorm_iplweb-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_denorm_iplweb-1.1.0.dist-info/RECORD` & `django_denorm_iplweb-1.1.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 denorm/__init__.py,sha256=H0y0FvNC1Zmky1WYjKheaqbXbbtGiC9adm-RpB8Yj8w,736
 denorm/apps.py,sha256=ZmCj4mq_usD-hjC0kTBVkGO_Fv3crecABuXS3ZPThXc,493
 denorm/contextmanagers.py,sha256=XeFZofso7Xsy10w1qbti7bJywCtR1ZJVBw16yPuvzpc,692
-denorm/denorms.py,sha256=Ja3PJPXiuZPHmZ7voJIP72b0k0U5dXEXRCm9VgV2OC8,30292
+denorm/denorms.py,sha256=4ZGk3FT8JuF2MrlihtVUkbEesj-4oWb9YDnF8tOpQLs,30285
 denorm/dependencies.py,sha256=7s4LO2pI7e3qlnkeAWsocTGL1f1lKkYhA2cgSJx4mHU,27369
-denorm/fields.py,sha256=u5ZJPA8lJr8gs2uOyKJCNOXlcC8aDA4me-d2tYD5IoU,10889
+denorm/fields.py,sha256=mN3VwWU9ZZstlnx3rnop6NyVdI6kXx3cWDFXcVRFkYc,10953
 denorm/helpers.py,sha256=cuFVS6pDe0gl5OwsIAGmW0VD9eUYzba5xHZwU6cOY8Y,2056
 denorm/middleware.py,sha256=r_35wmvBEHr3GmM4OJrgUSb0fdc9RIvwF4qTzRon5L0,1074
 denorm/models.py,sha256=5_3zmYErdnP8PS3l3SSHRn1BZYcu5qvauck_CJlbT3s,5950
 denorm/conf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 denorm/conf/settings.py,sha256=O75imSGKT5ctPYuw-nTPVDaDPx08iB8wCaXfPWOqtZQ,294
 denorm/db/__init__.py,sha256=ynGcKhgCdtyccEBPQVIwd3XXzDYh_72fCmc79hxf1Ug,874
 denorm/db/base.py,sha256=URVZ4sbuc4TGc_Xm5MtuQhhOOf3mXNNEyUPjLYQegBY,9463
@@ -31,14 +31,15 @@
 denorm/migrations/0006_auto_20211003_0346.py,sha256=KSwX6uUDeN0tDkYSBcMLIl2xtsifdPQ5-07H6SmQhY0,1191
 denorm/migrations/0007_auto_created_on_now.py,sha256=sPu8V8oDasYCumIYyMYJs7rp55hoI3iFzMkdkSuic8U,399
 denorm/migrations/0008_alter_dirtyinstance_object_id.py,sha256=qxgrJooqAEQKPRP_tzMKUDdJteFI-GyrPDl-zT7J6ww,407
 denorm/migrations/0009_alter_dirtyinstance_object_id.py,sha256=jdYI3oHo4Yh3L3fMIAghivJEk3bAaj3m9ReBULHNxfU,414
 denorm/migrations/0010_alter_dirtyinstance_object_id.py,sha256=nQL73hJpb7Cx0YIwWjU9Usdgii7yVolIFZfDr3eSQPc,417
 denorm/migrations/0011_alter_dirtyinstance_object_id.py,sha256=4rICVDeX95YstHOHdXMH-pVzBDvHNfilkJj_wHBjIf4,414
 denorm/migrations/0012_alter_dirtyinstance_object_id.py,sha256=uuhWnIEUW1wfEn2i-5uaf46ihWRdadIJOhf0v8j4ruk,417
+denorm/migrations/0013_alter_dirtyinstance_success.py,sha256=FpEPlUiv9YTOQI5l2RoJIvmhnMmqk0Sd407nOFg8Ips,431
 denorm/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-django_denorm_iplweb-1.1.0.dist-info/AUTHORS.txt,sha256=0mfucpnny18ulrwLGWX9PxS_Ib47TdrtxwZ7-QBGV9w,276
-django_denorm_iplweb-1.1.0.dist-info/LICENSE,sha256=8D3QJ8oIaQh8iLVkRy5EmMyY8wHxWrWStrNAi-ozdCY,2985
-django_denorm_iplweb-1.1.0.dist-info/METADATA,sha256=-PYrJ89nA28P9Ma5pakCwI4nM1-CyEAmiCiaABljUcQ,666
-django_denorm_iplweb-1.1.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-django_denorm_iplweb-1.1.0.dist-info/top_level.txt,sha256=RRQDTfZo5bzkzBIqg8FL7cIeXoQC8b6T2w2X8kA92vE,7
-django_denorm_iplweb-1.1.0.dist-info/RECORD,,
+django_denorm_iplweb-1.1.1.dist-info/AUTHORS.txt,sha256=0mfucpnny18ulrwLGWX9PxS_Ib47TdrtxwZ7-QBGV9w,276
+django_denorm_iplweb-1.1.1.dist-info/LICENSE,sha256=8D3QJ8oIaQh8iLVkRy5EmMyY8wHxWrWStrNAi-ozdCY,2985
+django_denorm_iplweb-1.1.1.dist-info/METADATA,sha256=aiHPxDrTAm9aruxr1vW59x3GaHTwaqXmiGNHC5zf0LM,630
+django_denorm_iplweb-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+django_denorm_iplweb-1.1.1.dist-info/top_level.txt,sha256=RRQDTfZo5bzkzBIqg8FL7cIeXoQC8b6T2w2X8kA92vE,7
+django_denorm_iplweb-1.1.1.dist-info/RECORD,,
```


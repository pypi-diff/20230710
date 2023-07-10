# Comparing `tmp/strawberry_django_auth-0.374.6.tar.gz` & `tmp/strawberry_django_auth-0.375.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_auth-0.374.6.tar", max compression
+gzip compressed data, was "strawberry_django_auth-0.375.0.tar", max compression
```

## Comparing `strawberry_django_auth-0.374.6.tar` & `strawberry_django_auth-0.375.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1075 2023-05-29 13:00:19.957047 strawberry_django_auth-0.374.6/LICENSE
--rw-r--r--   0        0        0     3820 2023-05-29 13:00:19.957047 strawberry_django_auth-0.374.6/README.md
--rw-r--r--   0        0        0       24 2023-05-29 13:00:20.001048 strawberry_django_auth-0.374.6/gqlauth/__init__.py
--rw-r--r--   0        0        0      168 2023-05-29 13:00:20.001048 strawberry_django_auth-0.374.6/gqlauth/admin.py
--rw-r--r--   0        0        0      215 2023-05-29 13:00:20.001048 strawberry_django_auth-0.374.6/gqlauth/apps.py
--rw-r--r--   0        0        0        0 2023-05-29 13:00:20.001048 strawberry_django_auth-0.374.6/gqlauth/captcha/__init__.py
--rw-r--r--   0        0        0     1267 2023-05-29 13:00:20.001048 strawberry_django_auth-0.374.6/gqlauth/captcha/captcha_factorty.py
--rw-r--r--   0        0        0     6602 2023-05-29 13:00:20.001048 strawberry_django_auth-0.374.6/gqlauth/captcha/create.py
--rw-r--r--   0        0        0    16724 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/captcha/fonts/Nehama.ttf
--rw-r--r--   0        0        0   221328 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/captcha/fonts/OpenSans-Semibold.ttf
--rw-r--r--   0        0        0    45448 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/captcha/fonts/pltwide.ttf
--rwxr-xr-x   0        0        0    22768 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/captcha/fonts/stam.ttf
--rw-r--r--   0        0        0     3248 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/captcha/models.py
--rw-r--r--   0        0        0      448 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/captcha/types_.py
--rw-r--r--   0        0        0        0 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/core/__init__.py
--rw-r--r--   0        0        0     1995 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/core/constants.py
--rw-r--r--   0        0        0      724 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/core/directives.py
--rw-r--r--   0        0        0     1093 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/core/exceptions.py
--rw-r--r--   0        0        0      231 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/core/interfaces.py
--rw-r--r--   0        0        0     4559 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/core/middlewares.py
--rw-r--r--   0        0        0     1453 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/core/mixins.py
--rw-r--r--   0        0        0     1516 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/core/scalars.py
--rw-r--r--   0        0        0      857 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/core/types_.py
--rw-r--r--   0        0        0     3979 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/core/utils.py
--rw-r--r--   0        0        0        0 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/jwt/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/jwt/tools.py
--rw-r--r--   0        0        0     7498 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/jwt/types_.py
--rw-r--r--   0        0        0     2969 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/migrations/0001_initial.py
--rw-r--r--   0        0        0      355 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/migrations/0002_alter_userstatus_options.py
--rw-r--r--   0        0        0      301 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/migrations/0003_delete_captcha.py
--rw-r--r--   0        0        0     1062 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/migrations/0004_captcha.py
--rw-r--r--   0        0        0        0 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/migrations/__init__.py
--rw-r--r--   0        0        0     7328 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/models.py
--rw-r--r--   0        0        0        0 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/py.typed
--rw-r--r--   0        0        0      649 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/settings.py
--rw-r--r--   0        0        0     9830 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/settings_type.py
--rw-r--r--   0        0        0      171 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/templates/email/activation_email.html
--rw-r--r--   0        0        0       41 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/templates/email/activation_subject.txt
--rw-r--r--   0        0        0   176202 2023-05-29 13:00:20.005048 strawberry_django_auth-0.374.6/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg
--rw-r--r--   0        0        0   100933 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg
--rw-r--r--   0        0        0      162 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/templates/email/password_reset_email.html
--rw-r--r--   0        0        0       39 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/templates/email/password_reset_subject.txt
--rw-r--r--   0        0        0      160 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/templates/email/password_set_email.html
--rw-r--r--   0        0        0       37 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/templates/email/password_set_subject.txt
--rw-r--r--   0        0        0        0 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/user/__init__.py
--rw-r--r--   0        0        0     2177 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/user/arg_mutations.py
--rw-r--r--   0        0        0     1628 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/user/forms.py
--rw-r--r--   0        0        0     1281 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/user/helpers.py
--rw-r--r--   0        0        0     1104 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/user/queries.py
--rw-r--r--   0        0        0     2277 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/user/relay.py
--rw-r--r--   0        0        0    19509 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/user/resolvers.py
--rw-r--r--   0        0        0      450 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/user/signals.py
--rw-r--r--   0        0        0     2005 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/user/types_.py
--rw-r--r--   0        0        0      119 2023-05-29 13:00:20.009048 strawberry_django_auth-0.374.6/gqlauth/user/views.py
--rw-r--r--   0        0        0     3209 2023-05-29 13:00:35.761299 strawberry_django_auth-0.374.6/pyproject.toml
--rw-r--r--   0        0        0     5138 1970-01-01 00:00:00.000000 strawberry_django_auth-0.374.6/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-10 04:00:36.059143 strawberry_django_auth-0.375.0/LICENSE
+-rw-r--r--   0        0        0     3820 2023-07-10 04:00:36.059143 strawberry_django_auth-0.375.0/README.md
+-rw-r--r--   0        0        0       24 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/admin.py
+-rw-r--r--   0        0        0      215 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/apps.py
+-rw-r--r--   0        0        0        0 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/__init__.py
+-rw-r--r--   0        0        0     1267 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/captcha_factorty.py
+-rw-r--r--   0        0        0     6618 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/create.py
+-rw-r--r--   0        0        0    16724 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/Nehama.ttf
+-rw-r--r--   0        0        0   221328 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/OpenSans-Semibold.ttf
+-rw-r--r--   0        0        0    45448 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/pltwide.ttf
+-rwxr-xr-x   0        0        0    22768 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/stam.ttf
+-rw-r--r--   0        0        0     3248 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/models.py
+-rw-r--r--   0        0        0      448 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/captcha/types_.py
+-rw-r--r--   0        0        0        0 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/__init__.py
+-rw-r--r--   0        0        0     1995 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/constants.py
+-rw-r--r--   0        0        0      910 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/directives.py
+-rw-r--r--   0        0        0     1093 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/exceptions.py
+-rw-r--r--   0        0        0      231 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/interfaces.py
+-rw-r--r--   0        0        0     4662 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/middlewares.py
+-rw-r--r--   0        0        0     1453 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/mixins.py
+-rw-r--r--   0        0        0     1516 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/scalars.py
+-rw-r--r--   0        0        0      857 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/types_.py
+-rw-r--r--   0        0        0     4063 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/jwt/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/jwt/tools.py
+-rw-r--r--   0        0        0     7498 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/jwt/types_.py
+-rw-r--r--   0        0        0     2969 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/migrations/0001_initial.py
+-rw-r--r--   0        0        0      355 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/migrations/0002_alter_userstatus_options.py
+-rw-r--r--   0        0        0      301 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/migrations/0003_delete_captcha.py
+-rw-r--r--   0        0        0     1062 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/migrations/0004_captcha.py
+-rw-r--r--   0        0        0        0 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/migrations/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/models.py
+-rw-r--r--   0        0        0        0 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/py.typed
+-rw-r--r--   0        0        0      649 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/settings.py
+-rw-r--r--   0        0        0     9825 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/settings_type.py
+-rw-r--r--   0        0        0      171 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/templates/email/activation_email.html
+-rw-r--r--   0        0        0       41 2023-07-10 04:00:36.115147 strawberry_django_auth-0.375.0/gqlauth/templates/email/activation_subject.txt
+-rw-r--r--   0        0        0   176202 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg
+-rw-r--r--   0        0        0   100933 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg
+-rw-r--r--   0        0        0      162 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/templates/email/password_reset_email.html
+-rw-r--r--   0        0        0       39 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/templates/email/password_reset_subject.txt
+-rw-r--r--   0        0        0      160 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/templates/email/password_set_email.html
+-rw-r--r--   0        0        0       37 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/templates/email/password_set_subject.txt
+-rw-r--r--   0        0        0        0 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/__init__.py
+-rw-r--r--   0        0        0     2177 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/arg_mutations.py
+-rw-r--r--   0        0        0     1628 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/forms.py
+-rw-r--r--   0        0        0     1281 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/helpers.py
+-rw-r--r--   0        0        0     1111 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/queries.py
+-rw-r--r--   0        0        0     2277 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/relay.py
+-rw-r--r--   0        0        0    19506 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/resolvers.py
+-rw-r--r--   0        0        0      450 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/signals.py
+-rw-r--r--   0        0        0     2005 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/types_.py
+-rw-r--r--   0        0        0      119 2023-07-10 04:00:36.119147 strawberry_django_auth-0.375.0/gqlauth/user/views.py
+-rw-r--r--   0        0        0     3205 2023-07-10 04:00:56.620680 strawberry_django_auth-0.375.0/pyproject.toml
+-rw-r--r--   0        0        0     5134 1970-01-01 00:00:00.000000 strawberry_django_auth-0.375.0/PKG-INFO
```

### Comparing `strawberry_django_auth-0.374.6/LICENSE` & `strawberry_django_auth-0.375.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/README.md` & `strawberry_django_auth-0.375.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/captcha/captcha_factorty.py` & `strawberry_django_auth-0.375.0/gqlauth/captcha/captcha_factorty.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/captcha/create.py` & `strawberry_django_auth-0.375.0/gqlauth/captcha/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,16 @@
         return image
 
     def create_captcha_image(self, chars, color, background):
         """Create the CAPTCHA image itself.
 
         :param chars: text to be generated.
         :param color: color of the text.
-        :param background: color of the background.
-        The color should be a tuple of 3 numbers, such as (0, 255, 255).
+        :param background: color of the background.         The color
+                should be a tuple of 3 numbers, such as (0, 255, 255).
         """
         image = Image.new("RGB", (self._width, self._height), background)
         draw = Draw(image)
 
         def _draw_character(c):
             # if hebrew
             direction = "ltr"
```

### Comparing `strawberry_django_auth-0.374.6/gqlauth/captcha/fonts/Nehama.ttf` & `strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/Nehama.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/captcha/fonts/OpenSans-Semibold.ttf` & `strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/OpenSans-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/captcha/fonts/pltwide.ttf` & `strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/pltwide.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/captcha/fonts/stam.ttf` & `strawberry_django_auth-0.375.0/gqlauth/captcha/fonts/stam.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/captcha/models.py` & `strawberry_django_auth-0.375.0/gqlauth/captcha/models.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/core/constants.py` & `strawberry_django_auth-0.375.0/gqlauth/core/constants.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/core/directives.py` & `strawberry_django_auth-0.375.0/gqlauth/core/directives.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 import dataclasses
-from typing import Any, final
+from typing import Any, Callable, final
 
 import strawberry
 from strawberry.schema_directive import Location
-from strawberry_django_plus.permissions import ConditionDirective
+from strawberry.types import Info
+from strawberry_django.permissions import DjangoNoPermission, DjangoPermissionExtension
 
 from gqlauth.core.utils import UserProto
 
 
 @strawberry.schema_directive(
     locations=[Location.FIELD_DEFINITION],
     description="Checks whether a user is verified",
 )
 @final
-class IsVerified(ConditionDirective):
+class IsVerified(DjangoPermissionExtension):
     """Mark a field as only resolvable by authenticated users."""
 
     message: strawberry.Private[str] = dataclasses.field(default="User is not authenticated.")
 
-    def check_condition(self, root: Any, info, user: UserProto, **kwargs) -> bool:  # type: ignore
-        return user.is_authenticated and user.status.verified
+    def resolve_for_user(
+        self,
+        resolver: Callable,
+        user: UserProto,
+        *,
+        info: Info,
+        source: Any,
+    ):
+        if user.is_authenticated and user.status.verified:
+            return resolver()
+        raise DjangoNoPermission
```

### Comparing `strawberry_django_auth-0.374.6/gqlauth/core/exceptions.py` & `strawberry_django_auth-0.375.0/gqlauth/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/core/middlewares.py` & `strawberry_django_auth-0.375.0/gqlauth/core/middlewares.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,13 +122,15 @@
         res = super().subscribe(*args, **kwargs)
         return res
 
     @staticmethod
     def _inject_user_and_errors(kwargs: dict) -> UserOrError:
         context = kwargs.get("context_value")
         # channels compat
-        if ws := getattr(context, "ws", None):
-            user_or_error: UserOrError = ws.scope[USER_OR_ERROR_KEY]
+        if isinstance(context, dict):
+            request = context["request"]
+            user_or_error: UserOrError = request.scope[USER_OR_ERROR_KEY]
+            request.user = user_or_error.user  # type: ignore
         else:
             user_or_error: UserOrError = getattr(context.request, USER_OR_ERROR_KEY)  # type: ignore
-        context.request.user = user_or_error.user  # type: ignore
+            context.request.user = user_or_error.user  # type: ignore
         return user_or_error
```

### Comparing `strawberry_django_auth-0.374.6/gqlauth/core/mixins.py` & `strawberry_django_auth-0.375.0/gqlauth/core/mixins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from abc import ABC
 from typing import Type
 
+import strawberry_django
 from django.contrib.auth import get_user_model
 from strawberry.types import Info
-from strawberry_django_plus import gql
 
 from gqlauth.core.utils import hide_args_kwargs, inject_arguments
 from gqlauth.user.resolvers import BaseMixin
 
 UserModel = get_user_model()
 
 
 class ArgMixin(BaseMixin, ABC):
     def __init_subclass__(cls: Type[BaseMixin], **kwargs):
         input_type = cls.resolve_mutation.__annotations__["input_"]
         return_type = cls.resolve_mutation.__annotations__["return"]
 
-        @gql.django.field(description=cls.__doc__)
+        @strawberry_django.field(description=cls.__doc__)
         @inject_arguments(input_type.__annotations__)
         @hide_args_kwargs
         def field(info: Info, **kwargs) -> return_type:  # type: ignore
             cls.verification_check(info)
             return cls.resolve_mutation(info, input_type(**kwargs))  # type: ignore
 
         cls.field = field  # type: ignore
 
 
 class RelayMixin(BaseMixin, ABC):
     def __init_subclass__(cls: Type[BaseMixin], **kwargs):
         input_type = cls.resolve_mutation.__annotations__["input_"]
         return_type = cls.resolve_mutation.__annotations__["return"]
 
-        @gql.django.field(description=cls.__doc__)
+        @strawberry_django.field(description=cls.__doc__)
         @hide_args_kwargs
         def field(info: Info, input: input_type) -> return_type:  # type: ignore
             cls.verification_check(info)
             return cls.resolve_mutation(info, input)  # type: ignore
 
         cls.field = field  # type: ignore
```

### Comparing `strawberry_django_auth-0.374.6/gqlauth/core/scalars.py` & `strawberry_django_auth-0.375.0/gqlauth/core/scalars.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/core/types_.py` & `strawberry_django_auth-0.375.0/gqlauth/core/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/core/utils.py` & `strawberry_django_auth-0.375.0/gqlauth/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,18 @@
         return {to_camel_case(k): camelize(v) for k, v in data.items()}
     if isiterable(data) and not isinstance(data, str):
         return [camelize(d) for d in data]
     return data
 
 
 def get_user(info: Info) -> USER_UNION:
-    return info.context.request.user  # type: ignore
+    try:
+        return info.context.request.user  # type: ignore
+    except AttributeError:
+        return info.context["request"].user
 
 
 def cast_to_status_user(user: USER_UNION) -> UserProto:
     user.status  # type: ignore  # raise attribute error
     return user  # type: ignore
```

### Comparing `strawberry_django_auth-0.374.6/gqlauth/jwt/types_.py` & `strawberry_django_auth-0.375.0/gqlauth/jwt/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/migrations/0001_initial.py` & `strawberry_django_auth-0.375.0/gqlauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/migrations/0004_captcha.py` & `strawberry_django_auth-0.375.0/gqlauth/migrations/0004_captcha.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/models.py` & `strawberry_django_auth-0.375.0/gqlauth/models.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/settings.py` & `strawberry_django_auth-0.375.0/gqlauth/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/settings_type.py` & `strawberry_django_auth-0.375.0/gqlauth/settings_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,16 +246,15 @@
     """
     JWT_DECODE_HANDLER: Callable[[str], "TokenType"] = decode_jwt
 
     JWT_TOKEN_FINDER: Callable[[Union["HttpRequest", dict]], Optional[str]] = token_finder
     """A hook called by `GqlAuthRootField` to find the token. Accepts the
     request object (might be channels scope dict or django request object)
 
-     **remember to strip the "JWT " prefix
-    if you override this.**
+    **remember to strip the "JWT " prefix if you override this.**
     """
     JWT_EXPIRATION_DELTA: timedelta = timedelta(minutes=5)
     """Timedelta added to `utcnow()` to set the expiration time.
 
     When this ends you will have to create a new token by logging in or
     using the refresh token.
     """
```

### Comparing `strawberry_django_auth-0.374.6/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg` & `strawberry_django_auth-0.375.0/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg` & `strawberry_django_auth-0.375.0/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/user/arg_mutations.py` & `strawberry_django_auth-0.375.0/gqlauth/user/arg_mutations.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/user/forms.py` & `strawberry_django_auth-0.375.0/gqlauth/user/forms.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/user/helpers.py` & `strawberry_django_auth-0.375.0/gqlauth/user/helpers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/user/queries.py` & `strawberry_django_auth-0.375.0/gqlauth/user/queries.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 import strawberry
+import strawberry_django
 from django.contrib.auth import get_user_model
 from strawberry.schema_directive import Location
 from strawberry.types import Info
-from strawberry_django_plus import gql
 
 from gqlauth.core.types_ import GQLAuthError, GQLAuthErrors
 from gqlauth.core.utils import get_user
 
 # project
 from .types_ import UserFilter, UserType
 
@@ -16,22 +16,22 @@
 
 
 @strawberry.schema_directive(locations=[Location.FIELD_DEFINITION])
 class Sample:
     message: str = "fdsafdsafdsfa"
 
 
-@gql.django.type(model=USER_MODEL, filters=UserFilter)
+@strawberry_django.type(model=USER_MODEL, filters=UserFilter)
 class UserQueries:
-    @gql.django.field(description="Returns the current user if he is not anonymous.")
+    @strawberry_django.field(description="Returns the current user if he is not anonymous.")
     def public_user(self, info: Info) -> Optional[UserType]:
         user = get_user(info)
         if not user.is_anonymous:
             return user  # type: ignore
         return None
 
-    @gql.django.field()
+    @strawberry_django.field()
     def me(self, info: Info) -> UserType:
         user = get_user(info)
         if not user.is_authenticated:
             raise GQLAuthError(code=GQLAuthErrors.UNAUTHENTICATED)
         return user  # type: ignore
```

### Comparing `strawberry_django_auth-0.374.6/gqlauth/user/relay.py` & `strawberry_django_auth-0.375.0/gqlauth/user/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/gqlauth/user/resolvers.py` & `strawberry_django_auth-0.375.0/gqlauth/user/resolvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import contextlib
 from dataclasses import asdict
 from smtplib import SMTPException
 from typing import Callable, cast
 from uuid import UUID
 
 import strawberry
+import strawberry_django
 from django.contrib.auth import get_user_model
 from django.contrib.auth.forms import PasswordChangeForm, SetPasswordForm
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.signing import BadSignature, SignatureExpired
 from django.db import transaction
 from strawberry.field import StrawberryField
 from strawberry.types import Info
-from strawberry_django_plus import gql
 
 from gqlauth.core.constants import Messages, TokenAction
 from gqlauth.core.exceptions import (
     PasswordAlreadySetError,
     TokenScopeError,
     UserAlreadyVerified,
     UserNotVerified,
@@ -84,15 +84,15 @@
         captcha. And uuid representing the captcha id in the database. When you
         will try to log in or register You will need submit that uuid With the
         user input.
 
         **The captcha will be invoked when the timeout expires**.
         """
 
-        @gql.django.field(description=__doc__)
+        @strawberry_django.field(description=__doc__)
         def field(self) -> CaptchaType:
             return CaptchaModel.create_captcha()
 
 
 class RegisterMixin(BaseMixin):
     """Register user with fields defined in the settings. If the email field of
     the user model is part of the registration fields (default), check if there
@@ -493,16 +493,17 @@
 
 class RefreshTokenMixin(BaseMixin):
     """### refreshToken to generate a new login token:
 
     *Use this only if `JWT_LONG_RUNNING_REFRESH_TOKEN` is True*
 
     using the refresh-token you already got during authorization, and
-    obtain a brand-new token (and possibly a new refresh token if you revoked the previous).
-    This is an alternative to log in when your token expired.
+    obtain a brand-new token (and possibly a new refresh token if you
+    revoked the previous). This is an alternative to log in when your
+    token expired.
     """
 
     @strawberry.input(
         description="If `revoke_refresh_token` is true,"
         " revokes to refresh token an creates a new one."
     )
     class RefreshTokenInput:
```

### Comparing `strawberry_django_auth-0.374.6/gqlauth/user/types_.py` & `strawberry_django_auth-0.375.0/gqlauth/user/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.6/pyproject.toml` & `strawberry_django_auth-0.375.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-auth"
-version = "0.374.6"
+version = "0.375.0"
 description = "Graphql authentication system with Strawberry for Django."
 license = "MIT"
 authors = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 readme = "README.md"
 classifiers = [
     'Environment :: Web Environment',
@@ -23,17 +23,17 @@
     { include = "gqlauth" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 Django = ">=3.2,<4.3"
 PyJWT = ">=2.6.0,<3.0"
-strawberry-django-plus = ">=1.25.2,<3.0.0"
 pillow = {version = "^9.5.0", extras = ["captcha"]}
 django-stubs = {extras = ["compatible-mypy"], version = "^4.2.0"}
+strawberry-graphql-django = ">=0.10.5"
 
 [tool.poetry.extras]
 captcha = ["pillow"]
 
 [tool.poetry.dev-dependencies]
 coverage = "^7.2"
 pytest = "^7.2"
```

### Comparing `strawberry_django_auth-0.374.6/PKG-INFO` & `strawberry_django_auth-0.375.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-auth
-Version: 0.374.6
+Version: 0.375.0
 Summary: Graphql authentication system with Strawberry for Django.
 License: MIT
 Author: Nir.J Benlulu
 Author-email: nrbnlulu@gmail.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: captcha
 Requires-Dist: Django (>=3.2,<4.3)
 Requires-Dist: PyJWT (>=2.6.0,<3.0)
 Requires-Dist: django-stubs[compatible-mypy] (>=4.2.0,<5.0.0)
 Requires-Dist: pillow[captcha] (>=9.5.0,<10.0.0) ; extra == "captcha"
-Requires-Dist: strawberry-django-plus (>=1.25.2,<3.0.0)
+Requires-Dist: strawberry-graphql-django (>=0.10.5)
 Project-URL: Documentation, https://nrbnlulu.github.io/strawberry-django-auth/
 Project-URL: Homepage, https://github.com/nrbnlulu/strawberry-django-auth
 Description-Content-Type: text/markdown
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/nrbnlulu/strawberry-django-auth/tests.yml?label=Tests&style=for-the-badge)](https://github.com/nrbnlulu/strawberry-django-auth/actions/workflows/tests.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/nrbnlulu/strawberry-django-auth?style=for-the-badge)](https://app.codecov.io/gh/nrbnlulu/strawberry-django-auth)
 [![Pypi](https://img.shields.io/pypi/v/strawberry-django-auth.svg?style=for-the-badge&logo=appveyor)](https://pypi.org/project/strawberry-django-auth/)
```


# Comparing `tmp/wideo-0.1.1.tar.gz` & `tmp/wideo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wideo-0.1.1.tar", max compression
+gzip compressed data, was "wideo-0.2.0.tar", max compression
```

## Comparing `wideo-0.1.1.tar` & `wideo-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,43 @@
--rw-r--r--   0        0        0      674 2023-06-28 13:25:29.295087 wideo-0.1.1/README.md
--rw-r--r--   0        0        0      469 2023-06-28 13:25:29.303088 wideo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1584 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/__init__.py
--rw-r--r--   0        0        0      674 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/admin_urls.py
--rw-r--r--   0        0        0      174 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/apps.py
--rw-r--r--   0        0        0      376 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/blocks.py
--rw-r--r--   0        0        0       55 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/exceptions.py
--rw-r--r--   0        0        0     1670 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/ffmpeg.py
--rw-r--r--   0        0        0      329 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/fields.py
--rw-r--r--   0        0        0      849 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/forms.py
--rw-r--r--   0        0        0     9737 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/migrations/__init__.py
--rw-r--r--   0        0        0     4851 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/models.py
--rw-r--r--   0        0        0      777 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/permissions.py
--rw-r--r--   0        0        0      899 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/signals.py
--rw-r--r--   0        0        0     1301 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/storage.py
--rw-r--r--   0        0        0      269 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/tasks.py
--rw-r--r--   0        0        0      179 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/blocks/video.html
--rw-r--r--   0        0        0     2299 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/forms/file.html
--rw-r--r--   0        0        0      190 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/forms/file_edit.html
--rw-r--r--   0        0        0      179 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/icons/video.svg
--rw-r--r--   0        0        0      457 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/preview/plyr_styles.html
--rw-r--r--   0        0        0     1757 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/preview/video_source.html
--rw-r--r--   0        0        0      124 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/video.html
--rw-r--r--   0        0        0     3303 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/videos/add.html
--rw-r--r--   0        0        0     1621 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/videos/confirm_delete.html
--rw-r--r--   0        0        0     2690 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/videos/edit.html
--rw-r--r--   0        0        0     4455 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/videos/index.html
--rw-r--r--   0        0        0     2586 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/videos/results.html
--rw-r--r--   0        0        0        0 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/templates/wideo/videos/results_video.html
--rw-r--r--   0        0        0    14465 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/views.py
--rw-r--r--   0        0        0      612 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/wagtail_hooks.py
--rw-r--r--   0        0        0      126 2023-06-28 13:25:29.303088 wideo-0.1.1/src/wideo/widgets.py
--rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 wideo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      674 2023-07-10 13:18:51.111670 wideo-0.2.0/README.md
+-rw-r--r--   0        0        0      469 2023-07-10 13:18:51.115670 wideo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1584 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/__init__.py
+-rw-r--r--   0        0        0      767 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/admin_urls.py
+-rw-r--r--   0        0        0      174 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/apps.py
+-rw-r--r--   0        0        0      376 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/blocks.py
+-rw-r--r--   0        0        0     2494 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/codecs.py
+-rw-r--r--   0        0        0       92 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/exceptions.py
+-rw-r--r--   0        0        0     7167 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/ffmpeg.py
+-rw-r--r--   0        0        0      329 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/fields.py
+-rw-r--r--   0        0        0      334 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/forms.py
+-rw-r--r--   0        0        0        0 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/management/commands/__init__.py
+-rw-r--r--   0        0        0      321 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/management/commands/delete_orphan_uploaded_videos.py
+-rw-r--r--   0        0        0      557 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/management/commands/encode_videos.py
+-rw-r--r--   0        0        0     9737 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/migrations/0001_initial.py
+-rw-r--r--   0        0        0      676 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/migrations/0002_lock.py
+-rw-r--r--   0        0        0     2955 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/migrations/0003_uploadedvideochunk.py
+-rw-r--r--   0        0        0        0 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/migrations/__init__.py
+-rw-r--r--   0        0        0     6373 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/models.py
+-rw-r--r--   0        0        0      777 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/permissions.py
+-rw-r--r--   0        0        0     1544 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/signals.py
+-rw-r--r--   0        0        0     1301 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/storage.py
+-rw-r--r--   0        0        0      636 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/tasks.py
+-rw-r--r--   0        0        0      179 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/blocks/video.html
+-rw-r--r--   0        0        0     3771 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/forms/file.html
+-rw-r--r--   0        0        0      190 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/forms/file_edit.html
+-rw-r--r--   0        0        0      179 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/icons/video.svg
+-rw-r--r--   0        0        0      457 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/preview/plyr_styles.html
+-rw-r--r--   0        0        0     1757 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/preview/video_source.html
+-rw-r--r--   0        0        0      124 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/video.html
+-rw-r--r--   0        0        0     3303 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/videos/add.html
+-rw-r--r--   0        0        0     1621 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/videos/confirm_delete.html
+-rw-r--r--   0        0        0     2690 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/videos/edit.html
+-rw-r--r--   0        0        0     4455 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/videos/index.html
+-rw-r--r--   0        0        0     2586 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/videos/results.html
+-rw-r--r--   0        0        0        0 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templates/wideo/videos/results_video.html
+-rw-r--r--   0        0        0        0 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templatetags/__init__.py
+-rw-r--r--   0        0        0      231 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/templatetags/settings.py
+-rw-r--r--   0        0        0    14570 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/views.py
+-rw-r--r--   0        0        0      612 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/wagtail_hooks.py
+-rw-r--r--   0        0        0      126 2023-07-10 13:18:51.119670 wideo-0.2.0/src/wideo/widgets.py
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 wideo-0.2.0/PKG-INFO
```

### Comparing `wideo-0.1.1/README.md` & `wideo-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wideo-0.1.1/src/wideo/__init__.py` & `wideo-0.2.0/src/wideo/__init__.py`

 * *Files identical despite different names*

### Comparing `wideo-0.1.1/src/wideo/admin_urls.py` & `wideo-0.2.0/src/wideo/admin_urls.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         "results/",
         wideo.views.ListingResultsView.as_view(),
         name="listing_results",
     ),
     path("add/", wideo.views.add, name="add"),
     path("<int:video_id>/", wideo.views.edit, name="edit"),
     path("<int:video_id>/delete/", wideo.views.delete, name="delete"),
-    path("upload/", wideo.views.upload_file, name="upload"),
+    path("upload/prepare/", wideo.views.upload_prepare, name="upload-prepare"),
+    path("upload/chunk/", wideo.views.upload_chunk, name="upload-chunk"),
     path(
         "get_uploaded_video_render/<int:uploaded_video_id>/",
         wideo.views.get_uploaded_video_render,
         name="get-uploaded-video-render",
     ),
 ]
```

### Comparing `wideo-0.1.1/src/wideo/migrations/0001_initial.py` & `wideo-0.2.0/src/wideo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wideo-0.1.1/src/wideo/models.py` & `wideo-0.2.0/src/wideo/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,49 @@
+import functools
+from datetime import timedelta
+from typing import Any, Callable
+
 from django.conf import settings
 from django.db import models
+from django.db.transaction import atomic
+from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
 from taggit.managers import TaggableManager
 from wagtail.models import CollectionMember
 from wagtail.search import index
 from wagtail.snippets.models import register_snippet
 
-from . import get_render_model
+from . import get_render_model, get_video_model
 from .storage import upload_to
 
 
+def delete_orphan_uploaded_videos():
+    """
+    Delete all the instances of UploadedVideo that are not related to any Video
+    anymore (result of changing the video file while editing a Video).
+    """
+    used_ids = get_video_model().objects.values("upload_id")
+    UploadedVideo.objects.exclude(id__in=used_ids).filter(
+        created_at__lt=now() - timedelta(days=1)
+    ).delete()
+
+
+def lock(name: str) -> Callable:
+    def decorator(func: Callable) -> Callable:
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs) -> Any:
+            with atomic():
+                Lock.objects.select_for_update().get_or_create(name=name)
+                return func(*args, **kwargs)
+
+        return wrapper
+
+    return decorator
+
+
 class TimestampedModel(models.Model):
     class Meta:
         abstract = True
 
     created_at = models.DateTimeField(
         verbose_name=_("created at"), auto_now_add=True, db_index=True
     )
@@ -77,17 +107,38 @@
     )
     frame_count = models.IntegerField(
         verbose_name=_("original frame count"),
         help_text=_("Number of frames in the video"),
     )
 
 
-class UploadedVideo(TimestampedModel, UserUpload, RemoteVideoFile):
-    def __str__(self) -> str:
-        return str(self.file)
+class UploadedVideo(TimestampedModel, UserUpload):
+    pass
+
+
+class UploadedVideoChunk(models.Model):
+    class Meta:
+        unique_together = ("video", "index")
+
+    video = models.ForeignKey(
+        to=UploadedVideo,
+        on_delete=models.CASCADE,
+        related_name="chunks",
+        verbose_name=_("video"),
+        help_text=_("The video the chunk is part of"),
+    )
+    index = models.IntegerField(
+        verbose_name=_("index"),
+        help_text=_("The position of the chunk in the uploaded video"),
+    )
+    file = models.FileField(
+        upload_to=upload_to,
+        verbose_name=_("file"),
+        help_text=_("The uploaded chunk"),
+    )
 
 
 class AbstractVideo(index.Indexed, CollectionMember, TimestampedModel, UserUpload):
     class Meta:
         abstract = True
 
     class ProcessStatus(models.TextChoices):
@@ -170,7 +221,11 @@
 class Render(AbstractRender):
     video = models.ForeignKey(
         to=Video,
         on_delete=models.CASCADE,
         verbose_name=_("video"),
         help_text=_("The video that was rendered"),
     )
+
+
+class Lock(models.Model):
+    name = models.TextField(unique=True)
```

### Comparing `wideo-0.1.1/src/wideo/permissions.py` & `wideo-0.2.0/src/wideo/permissions.py`

 * *Files identical despite different names*

### Comparing `wideo-0.1.1/src/wideo/storage.py` & `wideo-0.2.0/src/wideo/storage.py`

 * *Files identical despite different names*

### Comparing `wideo-0.1.1/src/wideo/templates/wideo/preview/video_source.html` & `wideo-0.2.0/src/wideo/templates/wideo/preview/video_source.html`

 * *Files identical despite different names*

### Comparing `wideo-0.1.1/src/wideo/templates/wideo/videos/add.html` & `wideo-0.2.0/src/wideo/templates/wideo/videos/add.html`

 * *Files identical despite different names*

### Comparing `wideo-0.1.1/src/wideo/templates/wideo/videos/confirm_delete.html` & `wideo-0.2.0/src/wideo/templates/wideo/videos/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wideo-0.1.1/src/wideo/templates/wideo/videos/edit.html` & `wideo-0.2.0/src/wideo/templates/wideo/videos/edit.html`

 * *Files identical despite different names*

### Comparing `wideo-0.1.1/src/wideo/templates/wideo/videos/index.html` & `wideo-0.2.0/src/wideo/templates/wideo/videos/index.html`

 * *Files identical despite different names*

### Comparing `wideo-0.1.1/src/wideo/templates/wideo/videos/results.html` & `wideo-0.2.0/src/wideo/templates/wideo/videos/results.html`

 * *Files identical despite different names*

### Comparing `wideo-0.1.1/src/wideo/views.py` & `wideo-0.2.0/src/wideo/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 
 from django.conf import settings
 from django.core.exceptions import PermissionDenied
 from django.core.paginator import Paginator
-from django.http import HttpRequest, HttpResponse, QueryDict
+from django.db.transaction import atomic
+from django.http import HttpRequest, HttpResponse
+from django.http.multipartparser import MultiPartParser
 from django.shortcuts import get_object_or_404, redirect
 from django.template.response import TemplateResponse
 from django.urls import NoReverseMatch, reverse
 from django.utils.decorators import method_decorator
 from django.utils.http import urlencode
 from django.utils.translation import gettext as _
 from django.utils.translation import gettext_lazy, ngettext
@@ -19,17 +21,16 @@
 from wagtail.admin.models import popular_tags_for_model
 from wagtail.admin.utils import get_valid_next_url_from_request
 from wagtail.admin.views import generic
 from wagtail.models import Collection
 from wagtail.search.backends import get_search_backend
 
 from . import get_render_model, get_video_model
-from .ffmpeg import get_video_info
-from .forms import BaseVideoForm, UploadedVideoForm, VideoForm
-from .models import UploadedVideo
+from .forms import BaseVideoForm, VideoForm
+from .models import UploadedVideo, UploadedVideoChunk
 from .permissions import permission_policy
 
 permission_checker = PermissionPolicyChecker(permission_policy)
 
 INDEX_PAGE_SIZE = getattr(settings, "WIDEO_INDEX_PAGE_SIZE", 30)
 USAGE_PAGE_SIZE = getattr(settings, "WIDEO_USAGE_PAGE_SIZE", 20)
 
@@ -342,37 +343,36 @@
         {
             "video": video,
             "next": next_url,
         },
     )
 
 
-def upload_file(request: HttpRequest) -> HttpResponse:
+@atomic
+def upload_prepare(request: HttpRequest) -> HttpResponse:
     if request.method != "POST":
         return HttpResponse(status=status.HTTP_405_METHOD_NOT_ALLOWED)
 
-    video_info = get_video_info(request.FILES["file"])
-    form = UploadedVideoForm(
-        {
-            **request.POST,
-            "mime": video_info["mime"],
-            "duration": video_info["duration"],
-            "width": video_info["width"],
-            "height": video_info["height"],
-            "frames_per_second": video_info["avg_frame_rate"],
-            "frame_count": video_info["nb_frames"],
-        },
-        request.FILES,
-    )
+    upload = UploadedVideo.objects.create()
+    return HttpResponse(status=status.HTTP_201_CREATED, content=upload.id)
+
 
-    if not form.is_valid():
-        return HttpResponse(status=status.HTTP_400_BAD_REQUEST, content=form.errors)
+@atomic
+def upload_chunk(request: HttpRequest) -> HttpResponse:
+    if request.method != "PUT":
+        return HttpResponse(status=status.HTTP_405_METHOD_NOT_ALLOWED)
 
-    instance = form.save()
-    return HttpResponse(status=status.HTTP_201_CREATED, content=instance.id)
+    data, files = MultiPartParser(
+        request.META, request, request.upload_handlers
+    ).parse()
+    upload = get_object_or_404(UploadedVideo, id=data["upload_id"])
+    UploadedVideoChunk.objects.update_or_create(
+        video=upload, index=data["index"], defaults={"file": files["blob"]}
+    )
+    return HttpResponse(status=status.HTTP_200_OK)
 
 
 def get_uploaded_video_render(
     request: HttpRequest, uploaded_video_id: int
 ) -> HttpResponse:
     """
     Given an UploadedVideo by its ID, return its information as if it was a
@@ -385,25 +385,26 @@
     still want to get the information of the video to display a preview in that
     add/edit template, so we get its information as if we were getting a unique
     Render so that we can use it with a video library.
     """
     if request.method != "GET":
         return HttpResponse(status=status.HTTP_405_METHOD_NOT_ALLOWED)
 
-    video = get_object_or_404(UploadedVideo, id=uploaded_video_id)
-
     data = {
         "type": "video",
         "title": "Video preview",
         "sources": [
             {
-                "src": video.file.url,
-                "type": video.mime,
-                "size": 720,
+                "src": render.file.url,
+                "type": render.mime,
+                "size": render.height,
             }
+            for render in get_render_model().objects.filter(
+                video__upload_id=uploaded_video_id
+            )
         ],
         #     poster: '/path/to/poster.jpg',
         #     previewThumbnails: {
         #         src: '/path/to/thumbnails.vtt',
         #     },
         #     tracks: [
         #         {
```

### Comparing `wideo-0.1.1/src/wideo/wagtail_hooks.py` & `wideo-0.2.0/src/wideo/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wideo-0.1.1/PKG-INFO` & `wideo-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wideo
-Version: 0.1.1
+Version: 0.2.0
 Summary: Add video goodness to your Wagtail website
 License: WTFPL
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


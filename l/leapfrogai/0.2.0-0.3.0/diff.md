# Comparing `tmp/leapfrogai-0.2.0.tar.gz` & `tmp/leapfrogai-0.3.0.tar.gz`

## Comparing `leapfrogai-0.2.0.tar` & `leapfrogai-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/Dockerfile
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/LICENSE
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/serve.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/audio/audio_pb2.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/audio/audio_pb2.pyi
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/audio/audio_pb2_grpc.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/embeddings/embeddings_pb2.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/embeddings/embeddings_pb2.pyi
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/embeddings/embeddings_pb2_grpc.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/generate/generate_pb2.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/generate/generate_pb2.pyi
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/generate/generate_pb2_grpc.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/name/name_pb2.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/name/name_pb2.pyi
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/name/name_pb2_grpc.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/LICENSE
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/leapfrogai/README.md
--rw-r--r--   0        0        0    19113 2020-02-02 00:00:00.000000 leapfrogai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/api/backends/leapfrogai/config.go
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/api/backends/leapfrogai/leapfrog.go
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/Dockerfile
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/LICENSE
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/__init__.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/serve.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/audio/audio_pb2.py
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/audio/audio_pb2.pyi
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/audio/audio_pb2_grpc.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/chat/chat_pb2.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/chat/chat_pb2.pyi
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/chat/chat_pb2_grpc.py
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/completion/completion_pb2.py
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/completion/completion_pb2.pyi
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/completion/completion_pb2_grpc.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/embeddings/embeddings_pb2.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/embeddings/embeddings_pb2.pyi
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/embeddings/embeddings_pb2_grpc.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/name/name_pb2.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/name/name_pb2.pyi
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/name/name_pb2_grpc.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/leapfrogai/README.md
+-rw-r--r--   0        0        0    19113 2020-02-02 00:00:00.000000 leapfrogai-0.3.0/PKG-INFO
```

### Comparing `leapfrogai-0.2.0/leapfrogai/Dockerfile` & `leapfrogai-0.3.0/leapfrogai/Dockerfile`

 * *Files identical despite different names*

### Comparing `leapfrogai-0.2.0/leapfrogai/LICENSE` & `leapfrogai-0.3.0/leapfrogai/LICENSE`

 * *Files identical despite different names*

### Comparing `leapfrogai-0.2.0/leapfrogai/serve.py` & `leapfrogai-0.3.0/leapfrogai/serve.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 from concurrent import futures
 
 import grpc
 
 from .audio import audio_pb2_grpc
+from .chat import chat_pb2_grpc
 from .embeddings import embeddings_pb2_grpc
-from .generate import generate_pb2_grpc
+from .completion import completion_pb2_grpc
 from .name import name_pb2_grpc
 
 
 def serve(o):
     # Create a gRPC server
-    server = grpc.server(futures.ThreadPoolExecutor(max_workers=1))
+    server = grpc.server(futures.ThreadPoolExecutor(max_workers=3))
+
+    if hasattr(o, "ChatComplete"):
+        chat_pb2_grpc.add_ChatCompletionServiceServicer_to_server(o, server)
+
+    if hasattr(o, "ChatCompleteStream"):
+        chat_pb2_grpc.add_ChatCompletionStreamServiceServicer_to_server(o, server)
+
+    if hasattr(o, "LLMConfig"):
+        completion_pb2_grpc.add_LLMConfigServiceServicer_to_server(o, server)
 
     if hasattr(o, "Complete"):
-        generate_pb2_grpc.add_CompletionServiceServicer_to_server(o, server)
+        completion_pb2_grpc.add_CompletionServiceServicer_to_server(o, server)
+
+    if hasattr(o, "CompleteStream"):
+        completion_pb2_grpc.add_CompletionStreamServiceServicer_to_server(o, server)
 
     if hasattr(o, "CreateEmbedding"):
         embeddings_pb2_grpc.add_EmbeddingsServiceServicer_to_server(o, server)
 
     if hasattr(o, "Name"):
         name_pb2_grpc.add_NameServiceServicer_to_server(o, server)
 
     if hasattr(o, "Transcribe") and hasattr(o, "Translate"):
         audio_pb2_grpc.add_AudioServicer_to_server(o, server)
 
     # Listen on port 50051
     print("Starting server. Listening on port 50051.")
     server.add_insecure_port("[::]:50051")
     server.start()
-    server.wait_for_termination()
 
-    # Keep thread alive
-    try:
-        while True:
-            pass
-    except KeyboardInterrupt:
-        server.stop(0)
+    # block the thread until the server terminates...without using async to await the completion
+    # of all requests, this is the best we can do to gracefully wait while the server responds to requests
+    server.wait_for_termination()
```

### Comparing `leapfrogai-0.2.0/leapfrogai/audio/audio_pb2.py` & `leapfrogai-0.3.0/leapfrogai/audio/audio_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: audio/audio.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x61udio/audio.proto\x12\x05\x61udio\"\xc4\x01\n\rAudioMetadata\x12\x0e\n\x06prompt\x18\x01 \x01(\t\x12\x13\n\x0btemperature\x18\x02 \x01(\x02\x12\x15\n\rinputlanguage\x18\x03 \x01(\t\x12\x30\n\x06\x66ormat\x18\x04 \x01(\x0e\x32 .audio.AudioMetadata.AudioFormat\"E\n\x0b\x41udioFormat\x12\x08\n\x04JSON\x10\x00\x12\x08\n\x04TEXT\x10\x01\x12\x07\n\x03SRT\x10\x02\x12\x10\n\x0cVERBOSE_JSON\x10\x03\x12\x07\n\x03VTT\x10\x04\"Y\n\x0c\x41udioRequest\x12(\n\x08metadata\x18\x01 \x01(\x0b\x32\x14.audio.AudioMetadataH\x00\x12\x14\n\nchunk_data\x18\x02 \x01(\x0cH\x00\x42\t\n\x07request\"\xe1\x02\n\rAudioResponse\x12\x1e\n\x04task\x18\x01 \x01(\x0e\x32\x10.audio.AudioTask\x12\x10\n\x08language\x18\x02 \x01(\t\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12.\n\x08segments\x18\x04 \x03(\x0b\x32\x1c.audio.AudioResponse.Segment\x12\x0c\n\x04text\x18\x05 \x01(\t\x1a\xcd\x01\n\x07Segment\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04seek\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x01\x12\x0b\n\x03\x65nd\x18\x04 \x01(\x01\x12\x0c\n\x04text\x18\x05 \x01(\t\x12\x0e\n\x06tokens\x18\x06 \x03(\x05\x12\x13\n\x0btemperature\x18\x07 \x01(\x01\x12\x13\n\x0b\x61vg_logprob\x18\x08 \x01(\x01\x12\x19\n\x11\x63ompression_ratio\x18\t \x01(\x01\x12\x16\n\x0eno_speech_prob\x18\n \x01(\x01\x12\x11\n\ttransient\x18\x0b \x01(\x08**\n\tAudioTask\x12\x0e\n\nTRANSCRIBE\x10\x00\x12\r\n\tTRANSLATE\x10\x01\x32|\n\x05\x41udio\x12\x38\n\tTranslate\x12\x13.audio.AudioRequest\x1a\x14.audio.AudioResponse(\x01\x12\x39\n\nTranscribe\x12\x13.audio.AudioRequest\x1a\x14.audio.AudioResponse(\x01\x42\x38Z6github.com/defenseunicorns/leapfrogai/pkg/client/audiob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'audio.audio_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'audio.audio_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z6github.com/defenseunicorns/leapfrogai/pkg/client/audio'
-  _AUDIOTASK._serialized_start=674
-  _AUDIOTASK._serialized_end=716
-  _AUDIOMETADATA._serialized_start=29
-  _AUDIOMETADATA._serialized_end=225
-  _AUDIOMETADATA_AUDIOFORMAT._serialized_start=156
-  _AUDIOMETADATA_AUDIOFORMAT._serialized_end=225
-  _AUDIOREQUEST._serialized_start=227
-  _AUDIOREQUEST._serialized_end=316
-  _AUDIORESPONSE._serialized_start=319
-  _AUDIORESPONSE._serialized_end=672
-  _AUDIORESPONSE_SEGMENT._serialized_start=467
-  _AUDIORESPONSE_SEGMENT._serialized_end=672
-  _AUDIO._serialized_start=718
-  _AUDIO._serialized_end=842
+  _globals['_AUDIOTASK']._serialized_start=674
+  _globals['_AUDIOTASK']._serialized_end=716
+  _globals['_AUDIOMETADATA']._serialized_start=29
+  _globals['_AUDIOMETADATA']._serialized_end=225
+  _globals['_AUDIOMETADATA_AUDIOFORMAT']._serialized_start=156
+  _globals['_AUDIOMETADATA_AUDIOFORMAT']._serialized_end=225
+  _globals['_AUDIOREQUEST']._serialized_start=227
+  _globals['_AUDIOREQUEST']._serialized_end=316
+  _globals['_AUDIORESPONSE']._serialized_start=319
+  _globals['_AUDIORESPONSE']._serialized_end=672
+  _globals['_AUDIORESPONSE_SEGMENT']._serialized_start=467
+  _globals['_AUDIORESPONSE_SEGMENT']._serialized_end=672
+  _globals['_AUDIO']._serialized_start=718
+  _globals['_AUDIO']._serialized_end=842
 # @@protoc_insertion_point(module_scope)
```

### Comparing `leapfrogai-0.2.0/leapfrogai/audio/audio_pb2.pyi` & `leapfrogai-0.3.0/leapfrogai/audio/audio_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,85 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
+
+class AudioTask(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    TRANSCRIBE: _ClassVar[AudioTask]
+    TRANSLATE: _ClassVar[AudioTask]
 TRANSCRIBE: AudioTask
 TRANSLATE: AudioTask
 
 class AudioMetadata(_message.Message):
-    __slots__ = ["format", "inputlanguage", "prompt", "temperature"]
+    __slots__ = ["prompt", "temperature", "inputlanguage", "format"]
     class AudioFormat(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    FORMAT_FIELD_NUMBER: _ClassVar[int]
-    INPUTLANGUAGE_FIELD_NUMBER: _ClassVar[int]
+        JSON: _ClassVar[AudioMetadata.AudioFormat]
+        TEXT: _ClassVar[AudioMetadata.AudioFormat]
+        SRT: _ClassVar[AudioMetadata.AudioFormat]
+        VERBOSE_JSON: _ClassVar[AudioMetadata.AudioFormat]
+        VTT: _ClassVar[AudioMetadata.AudioFormat]
     JSON: AudioMetadata.AudioFormat
-    PROMPT_FIELD_NUMBER: _ClassVar[int]
-    SRT: AudioMetadata.AudioFormat
-    TEMPERATURE_FIELD_NUMBER: _ClassVar[int]
     TEXT: AudioMetadata.AudioFormat
+    SRT: AudioMetadata.AudioFormat
     VERBOSE_JSON: AudioMetadata.AudioFormat
     VTT: AudioMetadata.AudioFormat
-    format: AudioMetadata.AudioFormat
-    inputlanguage: str
+    PROMPT_FIELD_NUMBER: _ClassVar[int]
+    TEMPERATURE_FIELD_NUMBER: _ClassVar[int]
+    INPUTLANGUAGE_FIELD_NUMBER: _ClassVar[int]
+    FORMAT_FIELD_NUMBER: _ClassVar[int]
     prompt: str
     temperature: float
+    inputlanguage: str
+    format: AudioMetadata.AudioFormat
     def __init__(self, prompt: _Optional[str] = ..., temperature: _Optional[float] = ..., inputlanguage: _Optional[str] = ..., format: _Optional[_Union[AudioMetadata.AudioFormat, str]] = ...) -> None: ...
 
 class AudioRequest(_message.Message):
-    __slots__ = ["chunk_data", "metadata"]
-    CHUNK_DATA_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["metadata", "chunk_data"]
     METADATA_FIELD_NUMBER: _ClassVar[int]
-    chunk_data: bytes
+    CHUNK_DATA_FIELD_NUMBER: _ClassVar[int]
     metadata: AudioMetadata
+    chunk_data: bytes
     def __init__(self, metadata: _Optional[_Union[AudioMetadata, _Mapping]] = ..., chunk_data: _Optional[bytes] = ...) -> None: ...
 
 class AudioResponse(_message.Message):
-    __slots__ = ["duration", "language", "segments", "task", "text"]
+    __slots__ = ["task", "language", "duration", "segments", "text"]
     class Segment(_message.Message):
-        __slots__ = ["avg_logprob", "compression_ratio", "end", "id", "no_speech_prob", "seek", "start", "temperature", "text", "tokens", "transient"]
-        AVG_LOGPROB_FIELD_NUMBER: _ClassVar[int]
-        COMPRESSION_RATIO_FIELD_NUMBER: _ClassVar[int]
-        END_FIELD_NUMBER: _ClassVar[int]
+        __slots__ = ["id", "seek", "start", "end", "text", "tokens", "temperature", "avg_logprob", "compression_ratio", "no_speech_prob", "transient"]
         ID_FIELD_NUMBER: _ClassVar[int]
-        NO_SPEECH_PROB_FIELD_NUMBER: _ClassVar[int]
         SEEK_FIELD_NUMBER: _ClassVar[int]
         START_FIELD_NUMBER: _ClassVar[int]
-        TEMPERATURE_FIELD_NUMBER: _ClassVar[int]
+        END_FIELD_NUMBER: _ClassVar[int]
         TEXT_FIELD_NUMBER: _ClassVar[int]
         TOKENS_FIELD_NUMBER: _ClassVar[int]
+        TEMPERATURE_FIELD_NUMBER: _ClassVar[int]
+        AVG_LOGPROB_FIELD_NUMBER: _ClassVar[int]
+        COMPRESSION_RATIO_FIELD_NUMBER: _ClassVar[int]
+        NO_SPEECH_PROB_FIELD_NUMBER: _ClassVar[int]
         TRANSIENT_FIELD_NUMBER: _ClassVar[int]
-        avg_logprob: float
-        compression_ratio: float
-        end: float
         id: int
-        no_speech_prob: float
         seek: int
         start: float
-        temperature: float
+        end: float
         text: str
         tokens: _containers.RepeatedScalarFieldContainer[int]
+        temperature: float
+        avg_logprob: float
+        compression_ratio: float
+        no_speech_prob: float
         transient: bool
         def __init__(self, id: _Optional[int] = ..., seek: _Optional[int] = ..., start: _Optional[float] = ..., end: _Optional[float] = ..., text: _Optional[str] = ..., tokens: _Optional[_Iterable[int]] = ..., temperature: _Optional[float] = ..., avg_logprob: _Optional[float] = ..., compression_ratio: _Optional[float] = ..., no_speech_prob: _Optional[float] = ..., transient: bool = ...) -> None: ...
-    DURATION_FIELD_NUMBER: _ClassVar[int]
+    TASK_FIELD_NUMBER: _ClassVar[int]
     LANGUAGE_FIELD_NUMBER: _ClassVar[int]
+    DURATION_FIELD_NUMBER: _ClassVar[int]
     SEGMENTS_FIELD_NUMBER: _ClassVar[int]
-    TASK_FIELD_NUMBER: _ClassVar[int]
     TEXT_FIELD_NUMBER: _ClassVar[int]
-    duration: float
+    task: AudioTask
     language: str
+    duration: float
     segments: _containers.RepeatedCompositeFieldContainer[AudioResponse.Segment]
-    task: AudioTask
     text: str
     def __init__(self, task: _Optional[_Union[AudioTask, str]] = ..., language: _Optional[str] = ..., duration: _Optional[float] = ..., segments: _Optional[_Iterable[_Union[AudioResponse.Segment, _Mapping]]] = ..., text: _Optional[str] = ...) -> None: ...
-
-class AudioTask(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
```

### Comparing `leapfrogai-0.2.0/leapfrogai/audio/audio_pb2_grpc.py` & `leapfrogai-0.3.0/leapfrogai/audio/audio_pb2_grpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,89 +11,114 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Translate = channel.stream_unary(
-                '/audio.Audio/Translate',
-                request_serializer=audio_dot_audio__pb2.AudioRequest.SerializeToString,
-                response_deserializer=audio_dot_audio__pb2.AudioResponse.FromString,
-                )
+            "/audio.Audio/Translate",
+            request_serializer=audio_dot_audio__pb2.AudioRequest.SerializeToString,
+            response_deserializer=audio_dot_audio__pb2.AudioResponse.FromString,
+        )
         self.Transcribe = channel.stream_unary(
-                '/audio.Audio/Transcribe',
-                request_serializer=audio_dot_audio__pb2.AudioRequest.SerializeToString,
-                response_deserializer=audio_dot_audio__pb2.AudioResponse.FromString,
-                )
+            "/audio.Audio/Transcribe",
+            request_serializer=audio_dot_audio__pb2.AudioRequest.SerializeToString,
+            response_deserializer=audio_dot_audio__pb2.AudioResponse.FromString,
+        )
 
 
 class AudioServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Translate(self, request_iterator, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
 
     def Transcribe(self, request_iterator, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
 
 
 def add_AudioServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'Translate': grpc.stream_unary_rpc_method_handler(
-                    servicer.Translate,
-                    request_deserializer=audio_dot_audio__pb2.AudioRequest.FromString,
-                    response_serializer=audio_dot_audio__pb2.AudioResponse.SerializeToString,
-            ),
-            'Transcribe': grpc.stream_unary_rpc_method_handler(
-                    servicer.Transcribe,
-                    request_deserializer=audio_dot_audio__pb2.AudioRequest.FromString,
-                    response_serializer=audio_dot_audio__pb2.AudioResponse.SerializeToString,
-            ),
+        "Translate": grpc.stream_unary_rpc_method_handler(
+            servicer.Translate,
+            request_deserializer=audio_dot_audio__pb2.AudioRequest.FromString,
+            response_serializer=audio_dot_audio__pb2.AudioResponse.SerializeToString,
+        ),
+        "Transcribe": grpc.stream_unary_rpc_method_handler(
+            servicer.Transcribe,
+            request_deserializer=audio_dot_audio__pb2.AudioRequest.FromString,
+            response_serializer=audio_dot_audio__pb2.AudioResponse.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'audio.Audio', rpc_method_handlers)
+        "audio.Audio", rpc_method_handlers
+    )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
- # This class is part of an EXPERIMENTAL API.
+# This class is part of an EXPERIMENTAL API.
 class Audio(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def Translate(request_iterator,
+    def Translate(
+        request_iterator,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.stream_unary(
+            request_iterator,
             target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.stream_unary(request_iterator, target, '/audio.Audio/Translate',
+            "/audio.Audio/Translate",
             audio_dot_audio__pb2.AudioRequest.SerializeToString,
             audio_dot_audio__pb2.AudioResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
 
     @staticmethod
-    def Transcribe(request_iterator,
+    def Transcribe(
+        request_iterator,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.stream_unary(
+            request_iterator,
             target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.stream_unary(request_iterator, target, '/audio.Audio/Transcribe',
+            "/audio.Audio/Transcribe",
             audio_dot_audio__pb2.AudioRequest.SerializeToString,
             audio_dot_audio__pb2.AudioResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
```

### Comparing `leapfrogai-0.2.0/leapfrogai/embeddings/embeddings_pb2.py` & `leapfrogai-0.3.0/leapfrogai/embeddings/embeddings_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: embeddings/embeddings.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x65mbeddings/embeddings.proto\x12\tembedding\"\"\n\x10\x45mbeddingRequest\x12\x0e\n\x06inputs\x18\x01 \x03(\t\"\x1e\n\tEmbedding\x12\x11\n\tembedding\x18\x01 \x03(\x02\"=\n\x11\x45mbeddingResponse\x12(\n\nembeddings\x18\x01 \x03(\x0b\x32\x14.embedding.Embedding2a\n\x11\x45mbeddingsService\x12L\n\x0f\x43reateEmbedding\x12\x1b.embedding.EmbeddingRequest\x1a\x1c.embedding.EmbeddingResponseB<Z:github.com/defenseunicorns/leapfrogai/pkg/client/embeddingb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x65mbeddings/embeddings.proto\x12\nembeddings\"\"\n\x10\x45mbeddingRequest\x12\x0e\n\x06inputs\x18\x01 \x03(\t\"\x1e\n\tEmbedding\x12\x11\n\tembedding\x18\x01 \x03(\x02\">\n\x11\x45mbeddingResponse\x12)\n\nembeddings\x18\x01 \x03(\x0b\x32\x15.embeddings.Embedding2c\n\x11\x45mbeddingsService\x12N\n\x0f\x43reateEmbedding\x12\x1c.embeddings.EmbeddingRequest\x1a\x1d.embeddings.EmbeddingResponseB=Z;github.com/defenseunicorns/leapfrogai/pkg/client/embeddingsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'embeddings.embeddings_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'embeddings.embeddings_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z:github.com/defenseunicorns/leapfrogai/pkg/client/embedding'
-  _EMBEDDINGREQUEST._serialized_start=42
-  _EMBEDDINGREQUEST._serialized_end=76
-  _EMBEDDING._serialized_start=78
-  _EMBEDDING._serialized_end=108
-  _EMBEDDINGRESPONSE._serialized_start=110
-  _EMBEDDINGRESPONSE._serialized_end=171
-  _EMBEDDINGSSERVICE._serialized_start=173
-  _EMBEDDINGSSERVICE._serialized_end=270
+  DESCRIPTOR._serialized_options = b'Z;github.com/defenseunicorns/leapfrogai/pkg/client/embeddings'
+  _globals['_EMBEDDINGREQUEST']._serialized_start=43
+  _globals['_EMBEDDINGREQUEST']._serialized_end=77
+  _globals['_EMBEDDING']._serialized_start=79
+  _globals['_EMBEDDING']._serialized_end=109
+  _globals['_EMBEDDINGRESPONSE']._serialized_start=111
+  _globals['_EMBEDDINGRESPONSE']._serialized_end=173
+  _globals['_EMBEDDINGSSERVICE']._serialized_start=175
+  _globals['_EMBEDDINGSSERVICE']._serialized_end=274
 # @@protoc_insertion_point(module_scope)
```

### Comparing `leapfrogai-0.2.0/leapfrogai/embeddings/embeddings_pb2.pyi` & `leapfrogai-0.3.0/leapfrogai/embeddings/embeddings_pb2.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Embedding(_message.Message):
-    __slots__ = ["embedding"]
-    EMBEDDING_FIELD_NUMBER: _ClassVar[int]
-    embedding: _containers.RepeatedScalarFieldContainer[float]
-    def __init__(self, embedding: _Optional[_Iterable[float]] = ...) -> None: ...
-
 class EmbeddingRequest(_message.Message):
     __slots__ = ["inputs"]
     INPUTS_FIELD_NUMBER: _ClassVar[int]
     inputs: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, inputs: _Optional[_Iterable[str]] = ...) -> None: ...
 
+class Embedding(_message.Message):
+    __slots__ = ["embedding"]
+    EMBEDDING_FIELD_NUMBER: _ClassVar[int]
+    embedding: _containers.RepeatedScalarFieldContainer[float]
+    def __init__(self, embedding: _Optional[_Iterable[float]] = ...) -> None: ...
+
 class EmbeddingResponse(_message.Message):
     __slots__ = ["embeddings"]
     EMBEDDINGS_FIELD_NUMBER: _ClassVar[int]
     embeddings: _containers.RepeatedCompositeFieldContainer[Embedding]
     def __init__(self, embeddings: _Optional[_Iterable[_Union[Embedding, _Mapping]]] = ...) -> None: ...
```

### Comparing `leapfrogai-0.2.0/leapfrogai/embeddings/embeddings_pb2_grpc.py` & `leapfrogai-0.3.0/leapfrogai/embeddings/embeddings_pb2_grpc.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,56 +11,69 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.CreateEmbedding = channel.unary_unary(
-                '/embedding.EmbeddingsService/CreateEmbedding',
-                request_serializer=embeddings_dot_embeddings__pb2.EmbeddingRequest.SerializeToString,
-                response_deserializer=embeddings_dot_embeddings__pb2.EmbeddingResponse.FromString,
-                )
+            "/embeddings.EmbeddingsService/CreateEmbedding",
+            request_serializer=embeddings_dot_embeddings__pb2.EmbeddingRequest.SerializeToString,
+            response_deserializer=embeddings_dot_embeddings__pb2.EmbeddingResponse.FromString,
+        )
 
 
 class EmbeddingsServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def CreateEmbedding(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
 
 
 def add_EmbeddingsServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'CreateEmbedding': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateEmbedding,
-                    request_deserializer=embeddings_dot_embeddings__pb2.EmbeddingRequest.FromString,
-                    response_serializer=embeddings_dot_embeddings__pb2.EmbeddingResponse.SerializeToString,
-            ),
+        "CreateEmbedding": grpc.unary_unary_rpc_method_handler(
+            servicer.CreateEmbedding,
+            request_deserializer=embeddings_dot_embeddings__pb2.EmbeddingRequest.FromString,
+            response_serializer=embeddings_dot_embeddings__pb2.EmbeddingResponse.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'embedding.EmbeddingsService', rpc_method_handlers)
+        "embeddings.EmbeddingsService", rpc_method_handlers
+    )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
- # This class is part of an EXPERIMENTAL API.
+# This class is part of an EXPERIMENTAL API.
 class EmbeddingsService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def CreateEmbedding(request,
+    def CreateEmbedding(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
             target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/embedding.EmbeddingsService/CreateEmbedding',
+            "/embeddings.EmbeddingsService/CreateEmbedding",
             embeddings_dot_embeddings__pb2.EmbeddingRequest.SerializeToString,
             embeddings_dot_embeddings__pb2.EmbeddingResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
```

### Comparing `leapfrogai-0.2.0/leapfrogai/generate/generate_pb2.pyi` & `leapfrogai-0.3.0/leapfrogai/chat/chat_pb2.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,109 @@
 from google.protobuf.internal import containers as _containers
+from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class CompletionRequest(_message.Message):
-    __slots__ = ["best_of", "echo", "frequence_penalty", "logit_bias", "logprobs", "max_tokens", "presence_penalty", "prompt", "stop", "stream", "suffix", "temperature", "top_p"]
+class ChatRole(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+    USER: _ClassVar[ChatRole]
+    SYSTEM: _ClassVar[ChatRole]
+    FUNCTION: _ClassVar[ChatRole]
+    ASSISTANT: _ClassVar[ChatRole]
+USER: ChatRole
+SYSTEM: ChatRole
+FUNCTION: ChatRole
+ASSISTANT: ChatRole
+
+class ChatItem(_message.Message):
+    __slots__ = ["role", "content"]
+    ROLE_FIELD_NUMBER: _ClassVar[int]
+    CONTENT_FIELD_NUMBER: _ClassVar[int]
+    role: ChatRole
+    content: str
+    def __init__(self, role: _Optional[_Union[ChatRole, str]] = ..., content: _Optional[str] = ...) -> None: ...
+
+class ChatCompletionRequest(_message.Message):
+    __slots__ = ["chat_items", "max_new_tokens", "temperature", "top_k", "top_p", "do_sample", "n", "stop", "repetition_penalty", "presence_penalty", "frequency_penalty", "best_of", "logit_bias", "return_full_text", "truncate", "typical_p", "watermark", "seed", "user"]
     class LogitBiasEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: int
         def __init__(self, key: _Optional[str] = ..., value: _Optional[int] = ...) -> None: ...
-    BEST_OF_FIELD_NUMBER: _ClassVar[int]
-    ECHO_FIELD_NUMBER: _ClassVar[int]
-    FREQUENCE_PENALTY_FIELD_NUMBER: _ClassVar[int]
-    LOGIT_BIAS_FIELD_NUMBER: _ClassVar[int]
-    LOGPROBS_FIELD_NUMBER: _ClassVar[int]
-    MAX_TOKENS_FIELD_NUMBER: _ClassVar[int]
-    PRESENCE_PENALTY_FIELD_NUMBER: _ClassVar[int]
-    PROMPT_FIELD_NUMBER: _ClassVar[int]
-    STOP_FIELD_NUMBER: _ClassVar[int]
-    STREAM_FIELD_NUMBER: _ClassVar[int]
-    SUFFIX_FIELD_NUMBER: _ClassVar[int]
+    CHAT_ITEMS_FIELD_NUMBER: _ClassVar[int]
+    MAX_NEW_TOKENS_FIELD_NUMBER: _ClassVar[int]
     TEMPERATURE_FIELD_NUMBER: _ClassVar[int]
+    TOP_K_FIELD_NUMBER: _ClassVar[int]
     TOP_P_FIELD_NUMBER: _ClassVar[int]
-    best_of: int
-    echo: bool
-    frequence_penalty: float
-    logit_bias: _containers.ScalarMap[str, int]
-    logprobs: int
-    max_tokens: int
-    presence_penalty: float
-    prompt: str
-    stop: _containers.RepeatedScalarFieldContainer[str]
-    stream: bool
-    suffix: str
+    DO_SAMPLE_FIELD_NUMBER: _ClassVar[int]
+    N_FIELD_NUMBER: _ClassVar[int]
+    STOP_FIELD_NUMBER: _ClassVar[int]
+    REPETITION_PENALTY_FIELD_NUMBER: _ClassVar[int]
+    PRESENCE_PENALTY_FIELD_NUMBER: _ClassVar[int]
+    FREQUENCY_PENALTY_FIELD_NUMBER: _ClassVar[int]
+    BEST_OF_FIELD_NUMBER: _ClassVar[int]
+    LOGIT_BIAS_FIELD_NUMBER: _ClassVar[int]
+    RETURN_FULL_TEXT_FIELD_NUMBER: _ClassVar[int]
+    TRUNCATE_FIELD_NUMBER: _ClassVar[int]
+    TYPICAL_P_FIELD_NUMBER: _ClassVar[int]
+    WATERMARK_FIELD_NUMBER: _ClassVar[int]
+    SEED_FIELD_NUMBER: _ClassVar[int]
+    USER_FIELD_NUMBER: _ClassVar[int]
+    chat_items: _containers.RepeatedCompositeFieldContainer[ChatItem]
+    max_new_tokens: int
     temperature: float
+    top_k: float
     top_p: float
-    def __init__(self, prompt: _Optional[str] = ..., suffix: _Optional[str] = ..., max_tokens: _Optional[int] = ..., temperature: _Optional[float] = ..., top_p: _Optional[float] = ..., stream: bool = ..., logprobs: _Optional[int] = ..., echo: bool = ..., stop: _Optional[_Iterable[str]] = ..., presence_penalty: _Optional[float] = ..., frequence_penalty: _Optional[float] = ..., best_of: _Optional[int] = ..., logit_bias: _Optional[_Mapping[str, int]] = ...) -> None: ...
+    do_sample: bool
+    n: int
+    stop: _containers.RepeatedScalarFieldContainer[str]
+    repetition_penalty: float
+    presence_penalty: float
+    frequency_penalty: float
+    best_of: str
+    logit_bias: _containers.ScalarMap[str, int]
+    return_full_text: bool
+    truncate: int
+    typical_p: float
+    watermark: bool
+    seed: int
+    user: str
+    def __init__(self, chat_items: _Optional[_Iterable[_Union[ChatItem, _Mapping]]] = ..., max_new_tokens: _Optional[int] = ..., temperature: _Optional[float] = ..., top_k: _Optional[float] = ..., top_p: _Optional[float] = ..., do_sample: bool = ..., n: _Optional[int] = ..., stop: _Optional[_Iterable[str]] = ..., repetition_penalty: _Optional[float] = ..., presence_penalty: _Optional[float] = ..., frequency_penalty: _Optional[float] = ..., best_of: _Optional[str] = ..., logit_bias: _Optional[_Mapping[str, int]] = ..., return_full_text: bool = ..., truncate: _Optional[int] = ..., typical_p: _Optional[float] = ..., watermark: bool = ..., seed: _Optional[int] = ..., user: _Optional[str] = ...) -> None: ...
 
-class CompletionResponse(_message.Message):
-    __slots__ = ["completion", "finish_reason"]
-    COMPLETION_FIELD_NUMBER: _ClassVar[int]
+class ChatCompletionChoice(_message.Message):
+    __slots__ = ["index", "chat_item", "finish_reason"]
+    INDEX_FIELD_NUMBER: _ClassVar[int]
+    CHAT_ITEM_FIELD_NUMBER: _ClassVar[int]
     FINISH_REASON_FIELD_NUMBER: _ClassVar[int]
-    completion: str
+    index: int
+    chat_item: ChatItem
     finish_reason: str
-    def __init__(self, completion: _Optional[str] = ..., finish_reason: _Optional[str] = ...) -> None: ...
+    def __init__(self, index: _Optional[int] = ..., chat_item: _Optional[_Union[ChatItem, _Mapping]] = ..., finish_reason: _Optional[str] = ...) -> None: ...
+
+class Usage(_message.Message):
+    __slots__ = ["prompt_tokens", "completion_tokens", "total_tokens"]
+    PROMPT_TOKENS_FIELD_NUMBER: _ClassVar[int]
+    COMPLETION_TOKENS_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_TOKENS_FIELD_NUMBER: _ClassVar[int]
+    prompt_tokens: int
+    completion_tokens: int
+    total_tokens: int
+    def __init__(self, prompt_tokens: _Optional[int] = ..., completion_tokens: _Optional[int] = ..., total_tokens: _Optional[int] = ...) -> None: ...
+
+class ChatCompletionResponse(_message.Message):
+    __slots__ = ["id", "object", "created", "choices", "usage"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    OBJECT_FIELD_NUMBER: _ClassVar[int]
+    CREATED_FIELD_NUMBER: _ClassVar[int]
+    CHOICES_FIELD_NUMBER: _ClassVar[int]
+    USAGE_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    object: str
+    created: int
+    choices: _containers.RepeatedCompositeFieldContainer[ChatCompletionChoice]
+    usage: Usage
+    def __init__(self, id: _Optional[str] = ..., object: _Optional[str] = ..., created: _Optional[int] = ..., choices: _Optional[_Iterable[_Union[ChatCompletionChoice, _Mapping]]] = ..., usage: _Optional[_Union[Usage, _Mapping]] = ...) -> None: ...
```

### Comparing `leapfrogai-0.2.0/leapfrogai/name/name_pb2.py` & `leapfrogai-0.3.0/leapfrogai/name/name_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: name/name.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fname/name.proto\x12\x04name\x1a\x1bgoogle/protobuf/empty.proto\"\x1c\n\x0cNameResponse\x12\x0c\n\x04name\x18\x01 \x01(\t2A\n\x0bNameService\x12\x32\n\x04Name\x12\x16.google.protobuf.Empty\x1a\x12.name.NameResponseB7Z5github.com/defenseunicorns/leapfrogai/pkg/client/nameb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'name.name_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'name.name_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z5github.com/defenseunicorns/leapfrogai/pkg/client/name'
-  _NAMERESPONSE._serialized_start=54
-  _NAMERESPONSE._serialized_end=82
-  _NAMESERVICE._serialized_start=84
-  _NAMESERVICE._serialized_end=149
+  _globals['_NAMERESPONSE']._serialized_start=54
+  _globals['_NAMERESPONSE']._serialized_end=82
+  _globals['_NAMESERVICE']._serialized_start=84
+  _globals['_NAMESERVICE']._serialized_end=149
 # @@protoc_insertion_point(module_scope)
```

### Comparing `leapfrogai-0.2.0/leapfrogai/name/name_pb2_grpc.py` & `leapfrogai-0.3.0/leapfrogai/name/name_pb2_grpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,56 +12,69 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Name = channel.unary_unary(
-                '/name.NameService/Name',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=name_dot_name__pb2.NameResponse.FromString,
-                )
+            "/name.NameService/Name",
+            request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            response_deserializer=name_dot_name__pb2.NameResponse.FromString,
+        )
 
 
 class NameServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Name(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
 
 
 def add_NameServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'Name': grpc.unary_unary_rpc_method_handler(
-                    servicer.Name,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=name_dot_name__pb2.NameResponse.SerializeToString,
-            ),
+        "Name": grpc.unary_unary_rpc_method_handler(
+            servicer.Name,
+            request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            response_serializer=name_dot_name__pb2.NameResponse.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'name.NameService', rpc_method_handlers)
+        "name.NameService", rpc_method_handlers
+    )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
- # This class is part of an EXPERIMENTAL API.
+# This class is part of an EXPERIMENTAL API.
 class NameService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def Name(request,
+    def Name(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
             target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/name.NameService/Name',
+            "/name.NameService/Name",
             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             name_dot_name__pb2.NameResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
```

### Comparing `leapfrogai-0.2.0/LICENSE` & `leapfrogai-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `leapfrogai-0.2.0/pyproject.toml` & `leapfrogai-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "leapfrogai"
-version = "0.2.0"
+version = "0.3.0"
 
 description = "A tool for building gRPC-based model backends for LeapfrogAI"
 authors = [
     { name = "LeapfrogAI Authors", email = "ai@defenseunicorns.com" },
     { name = "Gerred Dillon", email = "gerred@defenseunicorns.com" },
     { name = "Tom Runyon", email = "tom@defenseunicorns.com" },
 ]
```

### Comparing `leapfrogai-0.2.0/leapfrogai/README.md` & `leapfrogai-0.3.0/leapfrogai/README.md`

 * *Files identical despite different names*

### Comparing `leapfrogai-0.2.0/PKG-INFO` & `leapfrogai-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leapfrogai
-Version: 0.2.0
+Version: 0.3.0
 Summary: A tool for building gRPC-based model backends for LeapfrogAI
 Author-email: LeapfrogAI Authors <ai@defenseunicorns.com>, Gerred Dillon <gerred@defenseunicorns.com>, Tom Runyon <tom@defenseunicorns.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```


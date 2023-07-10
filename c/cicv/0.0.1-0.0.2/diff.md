# Comparing `tmp/cicv-0.0.1.tar.gz` & `tmp/cicv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cicv-0.0.1.tar", last modified: Thu Jun 29 10:27:17 2023, max compression
+gzip compressed data, was "cicv-0.0.2.tar", last modified: Mon Jul 10 09:18:07 2023, max compression
```

## Comparing `cicv-0.0.1.tar` & `cicv-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-29 10:27:17.458518 cicv-0.0.1/
--rw-rw-r--   0 max       (1000) max       (1000)     1086 2023-06-27 05:10:12.000000 cicv-0.0.1/LICENSE
--rw-rw-r--   0 max       (1000) max       (1000)      159 2023-06-29 10:27:17.458518 cicv-0.0.1/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     1093 2023-06-29 10:24:03.000000 cicv-0.0.1/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-29 10:27:17.458518 cicv-0.0.1/cicv/
--rw-rw-r--   0 max       (1000) max       (1000)       76 2023-06-29 10:02:11.000000 cicv-0.0.1/cicv/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)      628 2023-06-29 09:27:20.000000 cicv-0.0.1/cicv/config.py
--rw-rw-r--   0 max       (1000) max       (1000)    19743 2023-06-29 10:21:10.000000 cicv-0.0.1/cicv/source.py
--rw-rw-r--   0 max       (1000) max       (1000)     4133 2023-06-29 10:01:58.000000 cicv-0.0.1/cicv/utils.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-06-29 10:27:17.458518 cicv-0.0.1/cicv.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)      159 2023-06-29 10:27:17.000000 cicv-0.0.1/cicv.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      226 2023-06-29 10:27:17.000000 cicv-0.0.1/cicv.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2023-06-29 10:27:17.000000 cicv-0.0.1/cicv.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)       14 2023-06-29 10:27:17.000000 cicv-0.0.1/cicv.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)        5 2023-06-29 10:27:17.000000 cicv-0.0.1/cicv.egg-info/top_level.txt
--rw-rw-r--   0 max       (1000) max       (1000)       38 2023-06-29 10:27:17.458518 cicv-0.0.1/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)      319 2023-06-29 10:22:14.000000 cicv-0.0.1/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-07-10 09:18:07.426361 cicv-0.0.2/
+-rw-rw-r--   0 max       (1000) max       (1000)     1086 2023-06-27 05:10:12.000000 cicv-0.0.2/LICENSE
+-rw-rw-r--   0 max       (1000) max       (1000)      182 2023-07-10 09:18:07.426361 cicv-0.0.2/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      608 2023-06-30 08:33:53.000000 cicv-0.0.2/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-07-10 09:18:07.422361 cicv-0.0.2/cicv/
+-rw-rw-r--   0 max       (1000) max       (1000)       65 2023-06-30 09:43:16.000000 cicv-0.0.2/cicv/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      628 2023-06-29 09:27:20.000000 cicv-0.0.2/cicv/config.py
+-rw-rw-r--   0 max       (1000) max       (1000)    19678 2023-07-10 09:06:22.000000 cicv-0.0.2/cicv/source.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4122 2023-06-30 09:43:20.000000 cicv-0.0.2/cicv/utils.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-07-10 09:18:07.426361 cicv-0.0.2/cicv.egg-info/
+-rw-rw-r--   0 max       (1000) max       (1000)      182 2023-07-10 09:18:07.000000 cicv-0.0.2/cicv.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      245 2023-07-10 09:18:07.000000 cicv-0.0.2/cicv.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2023-07-10 09:18:07.000000 cicv-0.0.2/cicv.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       24 2023-07-10 09:18:07.000000 cicv-0.0.2/cicv.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        5 2023-07-10 09:18:07.000000 cicv-0.0.2/cicv.egg-info/top_level.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2023-07-10 09:18:07.426361 cicv-0.0.2/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)      303 2023-07-10 09:17:44.000000 cicv-0.0.2/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-07-10 09:18:07.426361 cicv-0.0.2/test/
+-rw-rw-r--   0 max       (1000) max       (1000)     2913 2023-06-29 10:30:33.000000 cicv-0.0.2/test/test-usage.py
```

### Comparing `cicv-0.0.1/LICENSE` & `cicv-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cicv-0.0.1/cicv/config.py` & `cicv-0.0.2/cicv/config.py`

 * *Files identical despite different names*

### Comparing `cicv-0.0.1/cicv/source.py` & `cicv-0.0.2/cicv/source.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,25 +29,22 @@
     CAM
 )
 
 # --------------------------------------------------
 # Basic Wrapper
 class Wrapper(abc.ABC):
 
-    # @abc.abstractclassmethod
-    # def _read_frame(self):
-    #     raise NotImplementedError
-
+    @abc.abstractclassmethod
     def read(self) -> np.ndarray:
         """Read frame via opencv.
 
         Returns:
             np.ndarray: frame buffer
         """
-        raise self._read_frame()
+        pass
 
     @abc.abstractclassmethod
     def get_type(self) -> str:
         """Get the type of the current object.
 
         Returns:
             str: _description_
@@ -58,44 +55,51 @@
     def get_fps(self):
         raise NotImplementedError
 
     @abc.abstractclassmethod
     def release(self):
         raise NotImplementedError
 
+    def _init_time_params(self):
+        self.timeout = 1/self.get_fps()
+        self.t_prev = time.time()
+        self.t_bias = 1e-5
+    
+    def _wait_time(self):
+        # NOTE: Sleep Directly for correct FPS 
+        t_process = ( self.timeout - (time.time() - self.t_prev ) )
+        if t_process > 0:
+            time.sleep( t_process )
+        self.t_prev = time.time()
+
 # --------------------------------------------------
 # Source Wrapper Object
 
 class ImageWrapper(Wrapper):
     
     def __init__(self, path:str) -> None:
         
         # Checking
         check_file_exists(file_path=path)
         check_input_ext(input=path, sup_ext=IMAGE.exts)
 
         # Parameters
         self.path = path
         self.frame = check_image_buffer(cv2.imread(path))
-
-        # Wait Time
-        self.timeout = 1/self.get_fps()
-        self.t_prev = time.time()
+        
+        # Time Parameters
+        self._init_time_params()
 
     def read(self):
-        # NOTE: Sleep Directly for correct FPS 
-        t_process = ( self.timeout - (time.time() - self.t_prev) )
-        if t_process > 0:
-            time.sleep( t_process )
 
         # Copy
         _frame = copy.deepcopy(self.frame)
 
-        # Update t_prev
-        self.t_prev = time.time()
+        # Wait for correct fps
+        self._wait_time()
 
         return _frame 
     
     def get_type(self):
         return IMAGE.__name__
 
     def get_fps(self):
@@ -134,26 +138,34 @@
             # collect image path and buffer
             self.img_paths.append(img_path)
             self.img_buffers.append(img_buf)
         
         # Log
         logging.info('Found {} images in {}'.format(len(self.img_paths), self.path))
 
+        # Time Parameters
+        self._init_time_params()
+
     def read(self):
 
         self.img_nums += 1
-        if self.img_nums < self.get_fps():
-            return self.img_buffers[self.img_id]
 
         self.img_id += 1
         if self.img_id > len(self.img_paths)-1:
             self.img_id = 0
 
         self.img_nums = 0
-        return self.img_buffers[self.img_id]
+
+        # Copy
+        _frame = copy.deepcopy(self.img_buffers[self.img_id])
+
+        # Wait for correct fps
+        self._wait_time()
+
+        return _frame
 
     def get_type(self):
         return DIR.__name__
     
     def release(self):
         self.img_paths, self.img_buffers = [], []
 
@@ -167,57 +179,48 @@
         check_input_ext(path, VIDEO_EXTS)
 
         # Init
         self.path = path
         self.cap = cv2.VideoCapture()
         self.set_cap()
 
-        # Wait Time Helper
-        self.timebias = 1e-5
-        self.timeout = 1/self.get_fps() - self.timebias
-        self.t_prev = time.time()
+        self._init_time_params()
         
     def set_cap(self):
         status = self.cap.open(self.path)
         if not status:
             raise VideoOpenError(f"Can not open the {self.get_type} from {self.path}")
 
     def reset_cap(self):
         logging.debug('Reset Source')
         self.cap.set(cv2.CAP_PROP_POS_FRAMES, 0)
 
     def read(self):
 
-        # NOTE: Sleep Directly for correct FPS 
-        t_process = ( self.timeout - (time.time() - self.t_prev) )
-        if t_process > 0:
-            time.sleep( t_process - self.timebias )
-        
         # Read Video Capture
         status, frame = self.cap.read()
 
         if not status:
             self.reset_cap()
             status, frame = self.cap.read()
             if not status:
                 raise VideoOpenError(f"VideoWrapper is broken, can't get the frame from {self.path}")
         
-        # Update t_prev
-        self.t_prev = time.time()
+        self._wait_time()
         
         return frame
     
     def get_fps(self):
         try:
             return self.cap.get(cv2.CAP_PROP_FPS)
         except Exception as e:
             raise RuntimeError('Can not get FPS value')
 
     def get_type(self):
-        return VIDEO
+        return VIDEO.__name__
 
     def get_delay_time(self):
         return self.frame_delay
 
     def release(self):
         self.cap.release()
 
@@ -267,28 +270,27 @@
         
         if not status:
             self.reset_cap()
             
         return frame
 
     def get_type(self):
-        return RTSP
+        return RTSP.__name__
 
 class UsbCameraWrapper(VideoWrapper):
     
     def __init__(self, path, resolution, fps) -> None:
 
         self.path = path
         
         self.cap = cv2.VideoCapture()
-        self.fps = 30 if fps is None else fps
+        self.fps = RTSP.fps if fps is None else fps
         self.resolution = resolution
         self.set_cap(self.resolution, self.fps)
 
-
     def set_cap(self, resolution, fps):
         """ Setup camera 
         - Args
             - resolution: A tuple with width and height, e.g.( <width>, <height> )
             - fps: The fps 
         """
         if not isinstance(self.path, int) and self.path.isdigit():
@@ -310,15 +312,15 @@
             if fps:
                 self.cap.set(cv2.CAP_PROP_FPS, fps)
             
         except ValueError:
             raise InvalidInput("Can not find the camera {}".format(self.path))
 
     def get_type(self):
-        return CAM
+        return CAM.__name__
 
     def reset_cap(self):
         self.set_cap(self.resolution, self.fps)
         logging.debug('Reset Camera')
         time.sleep(1/30)
 
     def read(self):
@@ -328,14 +330,17 @@
             self.reset_cap()    
             status, frame = self.cap.read()
             
             if not status:
                 raise UsbCamOpenError("Can not capture frame, please make sure the camera is available")
         
         return frame
+    
+    def get_fps(self):
+        return self.fps
 
 # --------------------------------------------------
 # Entrance
 
 def get_source_object(input:str, camera_resolution:Tuple[int, int]=(1280, 720), fps:int=30) -> Wrapper:
     """Trying to instance the source object
 
@@ -344,39 +349,40 @@
         camera_resolution (Tuple[int, int], optional): setup camera resolution ( width, height ) if need. Defaults to (1280, 720).
         fps (int, optional): setup fps if need. Defaults to 30.
 
     Raises:
         errors: the latest exception
 
     Returns:
-        Wrapper: return a iVIT Source Wrapper
+        Wrapper: return a CICV Source Wrapper
     """
     errors = []
     for reader in (ImageWrapper, DirImageWrapper, VideoWrapper, RtspWrapper):
         try:
             return reader(input)
         except (InvalidInput, OpenError) as e:
             errors.append(e)
 
     try:
         return UsbCameraWrapper(input, camera_resolution, fps)
     except (InvalidInput, OpenError) as e:
-        errors.append(e)
+        if len(errors)==0:
+            errors.append(e)
     
     # if not errors[OpenError]:
     #     logging.error(*errors[InvalidInput])#, file=sys.stderr, sep='\n')
     # else:
     #     logging.error(*errors[OpenError])#, file=sys.stderr, sep='\n')
 
     raise errors[-1]
 
 class Source(object):
 
     def __init__(self, input:str, resolution:Tuple[int, int]=None, fps:int=None) -> None:
-        """iVIT Source Object
+        """CICV Source Object
         
         Args:
             input (str): the input data, supported image path, image folder, 
             video path, rtsp uri and usb camera
             resolution (Tuple[int, int], optional): A tuple value with width and height, 
             you will get target size of the frame after setting up. Defaults to None.
             fps (int, optional): This option is only for camera. Defaults to None.
@@ -387,15 +393,15 @@
         # Init
         self.frame = self.src.read()
         self.height, self.width = self.frame.shape[:2]
         self._print_info()
 
     def _print_info(self):
         print(
-            "[ iVIT Source Information ]\n",
+            "[ CICV Source Information ]\n",
             f"\t- Name      : {self.input}\n",
             f"\t- Type      : {self.src.get_type()}\n",
             f"\t- Shape     : {self.width}, {self.height} ( W, H )\n",
             f"\t- FPS       : {self.src.get_fps()}\n"
         )
 
     def read(self) -> np.ndarray:
@@ -446,15 +452,15 @@
     def release(self) -> None:
         """Release source object """
         return self.src.release()
 
 class SourceV2(object):
 
     def __init__(self, input:str, resolution:Tuple[int, int]=None, fps:int=None, start:bool=False) -> None:
-        """iVIT Source Object ( Async )
+        """CICV Source Object ( Async )
 
         Args:
             input (str): the input data, supported image path, image folder, video path, rtsp uri and usb camera.
             resolution (Tuple[int, int], optional): A tuple value with width and height, you will get target size of the frame after setting up. Defaults to None.
             fps (int, optional): This option is only for camera. Defaults to None.
             start (bool, optional): Start the source piepline after instance. Defaults to False.
 
@@ -486,15 +492,15 @@
         self._print_info()
         
         self.t = self._create_thread()  # Create Thread and start ( if need )
         if start: self.start()
 
     def _print_info(self):
         print(
-            "[ iVIT Source Information ]\n",
+            "[ CICV Source Information ]\n",
             f"\t- Name      : {self.input}\n",
             f"\t- Type      : {self.src.get_type()}\n",
             f"\t- Shape     : {self.width}, {self.height} ( W, H )\n",
             f"\t- FPS       : {self.src.get_fps()}\n",
             f"\t- WARNUP    : {self.t_warnup}s\n"
         )
 
@@ -671,15 +677,15 @@
         """
         return ( self.height, self.width )
 
     def read(self) -> Tuple[bool, np.ndarray ]:
         """ Get source status and current frame """
 
         if not self.is_ready:
-            raise RuntimeError('iVIT Source has not start yet.')
+            raise RuntimeError('CICV Source has not start yet.')
 
         # Check current frame and previous frame
         if self.pre_frame_id == self.cur_frame_id:    
             return (False, self.frame)
         
         self.pre_frame_id = self.cur_frame_id
         self.t_update = time.time()
```

### Comparing `cicv-0.0.1/cicv/utils.py` & `cicv-0.0.2/cicv/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     raise InvalidInput(f"Can not find the folder ({folder_path})")
 
 def check_image_buffer(frame:np.ndarray) -> np.ndarray:
     if frame is None:
         raise ImageOpenError("Get empty image")
     return frame
 
-def put_highlighted_text(
+def draw_text(
         frame:np.ndarray, 
         message:str, 
         position:tuple=(40,40), 
         font_face=cv2.FONT_HERSHEY_SIMPLEX, 
         font_scale=1, 
         color=(0, 255, 0), 
         thickness=2) -> None:
```


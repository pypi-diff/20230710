# Comparing `tmp/streamlitopencvplayer-1.3.2.tar.gz` & `tmp/streamlitopencvplayer-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.3.2.tar", last modified: Mon Jul 10 16:11:53 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.3.3.tar", last modified: Mon Jul 10 16:23:08 2023, max compression
```

## Comparing `streamlitopencvplayer-1.3.2.tar` & `streamlitopencvplayer-1.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 16:11:53.885432 streamlitopencvplayer-1.3.2/
--rw-rw-rw-   0        0        0      419 2023-07-10 16:11:53.883966 streamlitopencvplayer-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 16:11:53.886432 streamlitopencvplayer-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-10 16:08:26.000000 streamlitopencvplayer-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 16:11:53.852768 streamlitopencvplayer-1.3.2/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.3.2/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     6989 2023-07-10 11:36:37.000000 streamlitopencvplayer-1.3.2/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-10 16:11:53.871347 streamlitopencvplayer-1.3.2/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-10 16:11:53.000000 streamlitopencvplayer-1.3.2/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-10 16:11:53.000000 streamlitopencvplayer-1.3.2/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 16:11:53.000000 streamlitopencvplayer-1.3.2/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-10 16:11:53.000000 streamlitopencvplayer-1.3.2/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-10 16:11:53.879400 streamlitopencvplayer-1.3.2/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.3.2/test/__init__.py
--rw-rw-rw-   0        0        0     2170 2023-07-04 20:30:14.000000 streamlitopencvplayer-1.3.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-10 16:23:08.463556 streamlitopencvplayer-1.3.3/
+-rw-rw-rw-   0        0        0      419 2023-07-10 16:23:08.462555 streamlitopencvplayer-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 16:23:08.464555 streamlitopencvplayer-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-10 16:18:16.000000 streamlitopencvplayer-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 16:23:08.432174 streamlitopencvplayer-1.3.3/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.3.3/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     6770 2023-07-10 16:23:02.000000 streamlitopencvplayer-1.3.3/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-10 16:23:08.449896 streamlitopencvplayer-1.3.3/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-10 16:23:07.000000 streamlitopencvplayer-1.3.3/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-10 16:23:08.000000 streamlitopencvplayer-1.3.3/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 16:23:07.000000 streamlitopencvplayer-1.3.3/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-10 16:23:07.000000 streamlitopencvplayer-1.3.3/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 16:23:08.457554 streamlitopencvplayer-1.3.3/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.3.3/test/__init__.py
+-rw-rw-rw-   0        0        0     2170 2023-07-04 20:30:14.000000 streamlitopencvplayer-1.3.3/test/test.py
```

### Comparing `streamlitopencvplayer-1.3.2/README.md` & `streamlitopencvplayer-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.3.2/setup.py` & `streamlitopencvplayer-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.2' 
+VERSION = '1.3.3' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.3.2/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.3.3/streamlitopencvplayer/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,24 +44,20 @@
         #print(st.session_state['name_vid_sel'])
         alerts = []
         data = []
 
         for x in range(len(list_ts)):
                 time_alert = float(list_ts[x])-float(
                     st.session_state['name_vid_sel'].partition('_')[0])
-                print(time_alert)
                 alerts.append(int((time_alert)*fps))
                 
                 data.append(list_data[x])
     i = 0
-    #print("-----------")
-    #print(alerts)
-    #print(data[0][1][0][2])
 
-    draw_detections = st.checkbox("Draw detections")
+    draw_detections = st.checkbox("Draw detections",value=True)
     resume = False
     column1, column2, column3 = st.columns([1, 2, 1])
     with column1:
         # zone to display images
         stframe = st.empty()
     with column3:
         # Alerts
@@ -115,39 +111,37 @@
                 st.session_state['frames'].append(frames)
             else:
                 break
         st.session_state['cap'].release()
     # back to the first frame if the video is finished
     if st.session_state['counter'] == len(st.session_state['frames']):
         st.session_state['counter'] = 0
-    print(len(data))
+    #print(len(data))
     stframe.image(st.session_state['frames']
                   [st.session_state['counter']], caption='', width=450)
     if not resume:
         while st.session_state['counter'] < len(st.session_state['frames']):         
                 for i in range(len(data)):
-                    #st.write("counter ",st.session_state['counter'])
-                    #st.write("fps",alerts[i])
                     if draw_detections:
                         if st.session_state['counter'] == int(alerts[i]):
                             # draw all detections on the frame
                             for j in range(len(data[i])):
                                 output = cv2.rectangle(st.session_state['frames'][st.session_state['counter']], (data[i][j][0][0], data[i][j][0][1]), (
                                     data[i][j][0][2], data[i][j][0][3]), color=(128, 0, 0), thickness=2)
                                 output = cv2.putText(
                                     st.session_state['frames'][st.session_state['counter']], data[i][j][3], (data[i][j][0][0], data[i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
                             # update image zone with detections
                             stframe.image(output, caption='', width=500)
-                            time.sleep(0.08)
+                            time.sleep(0.05)
                             # the detection is drawn, to the next one
                             st.session_state['counter'] += 1
 
                 stframe.image(
                     st.session_state['frames'][st.session_state['counter']], caption='', width=500)
-                time.sleep(0.08)
+                time.sleep(0.05)
                 st.session_state['counter'] += 1
                     
 
                 if pause:
                     resume = True
                     break
                 if plus:
```

### Comparing `streamlitopencvplayer-1.3.2/test/test.py` & `streamlitopencvplayer-1.3.3/test/test.py`

 * *Files identical despite different names*


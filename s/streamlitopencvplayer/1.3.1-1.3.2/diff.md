# Comparing `tmp/streamlitopencvplayer-1.3.1.tar.gz` & `tmp/streamlitopencvplayer-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.3.1.tar", last modified: Tue Jul  4 20:12:45 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.3.2.tar", last modified: Mon Jul 10 16:11:53 2023, max compression
```

## Comparing `streamlitopencvplayer-1.3.1.tar` & `streamlitopencvplayer-1.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 20:12:45.019362 streamlitopencvplayer-1.3.1/
--rw-rw-rw-   0        0        0      419 2023-07-04 20:12:45.017645 streamlitopencvplayer-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 20:12:45.020357 streamlitopencvplayer-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-04 20:12:41.000000 streamlitopencvplayer-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:12:44.989369 streamlitopencvplayer-1.3.1/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.3.1/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     6612 2023-07-04 20:12:29.000000 streamlitopencvplayer-1.3.1/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:12:45.006953 streamlitopencvplayer-1.3.1/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-04 20:12:44.000000 streamlitopencvplayer-1.3.1/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-04 20:12:44.000000 streamlitopencvplayer-1.3.1/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 20:12:44.000000 streamlitopencvplayer-1.3.1/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-04 20:12:44.000000 streamlitopencvplayer-1.3.1/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-04 20:12:45.013344 streamlitopencvplayer-1.3.1/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.3.1/test/__init__.py
--rw-rw-rw-   0        0        0     1690 2023-07-04 19:05:23.000000 streamlitopencvplayer-1.3.1/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-10 16:11:53.885432 streamlitopencvplayer-1.3.2/
+-rw-rw-rw-   0        0        0      419 2023-07-10 16:11:53.883966 streamlitopencvplayer-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-10 16:11:53.886432 streamlitopencvplayer-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-10 16:08:26.000000 streamlitopencvplayer-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 16:11:53.852768 streamlitopencvplayer-1.3.2/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.3.2/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     6989 2023-07-10 11:36:37.000000 streamlitopencvplayer-1.3.2/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-10 16:11:53.871347 streamlitopencvplayer-1.3.2/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-10 16:11:53.000000 streamlitopencvplayer-1.3.2/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-10 16:11:53.000000 streamlitopencvplayer-1.3.2/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 16:11:53.000000 streamlitopencvplayer-1.3.2/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-10 16:11:53.000000 streamlitopencvplayer-1.3.2/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 16:11:53.879400 streamlitopencvplayer-1.3.2/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.3.2/test/__init__.py
+-rw-rw-rw-   0        0        0     2170 2023-07-04 20:30:14.000000 streamlitopencvplayer-1.3.2/test/test.py
```

### Comparing `streamlitopencvplayer-1.3.1/README.md` & `streamlitopencvplayer-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.3.1/setup.py` & `streamlitopencvplayer-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.1' 
+VERSION = '1.3.2' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.3.1/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.3.2/streamlitopencvplayer/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,23 @@
     st.session_state['frames'] = []
 if 'alerts' not in st.session_state:
     st.session_state['alerts'] = []
 if 'data' not in st.session_state:
     st.session_state['data'] = []
 if 'alerts_list' not in st.session_state:
     st.session_state['alerts_list'] = []
+if 'name_vid_sel' not in st.session_state:
+    st.session_state['name_vid_sel'] = "1687441603.4032989_1687441609.4032989"
 
 
 # Function to display video in the Streamlit app
 
 def display_video(video_path, json_file):
     # Open the video file
-    st.write(video_path)
+    
     st.session_state['cap'] = cv2.VideoCapture(video_path)
     fps = st.session_state['cap'].get(cv2.CAP_PROP_FPS)
     # Opening JSON file and returns JSON object as a dictionnary
     if json_file is not None:
         response = urllib.request.urlopen(json_file)
         fileReader = json.loads(response.read())
         list_ts = []
@@ -42,15 +44,17 @@
         #print(st.session_state['name_vid_sel'])
         alerts = []
         data = []
 
         for x in range(len(list_ts)):
                 time_alert = float(list_ts[x])-float(
                     st.session_state['name_vid_sel'].partition('_')[0])
+                print(time_alert)
                 alerts.append(int((time_alert)*fps))
+                
                 data.append(list_data[x])
     i = 0
     #print("-----------")
     #print(alerts)
     #print(data[0][1][0][2])
 
     draw_detections = st.checkbox("Draw detections")
@@ -111,32 +115,35 @@
                 st.session_state['frames'].append(frames)
             else:
                 break
         st.session_state['cap'].release()
     # back to the first frame if the video is finished
     if st.session_state['counter'] == len(st.session_state['frames']):
         st.session_state['counter'] = 0
-
+    print(len(data))
     stframe.image(st.session_state['frames']
                   [st.session_state['counter']], caption='', width=450)
     if not resume:
         while st.session_state['counter'] < len(st.session_state['frames']):         
                 for i in range(len(data)):
-                    if st.session_state['counter'] == int(alerts[i]*fps) and draw_detections:
-                        # draw all detections on the frame
-                        for j in range(len(data[i])):
-                            output = cv2.rectangle(st.session_state['frames'][st.session_state['counter']], (data[i][j][0][0], data[i][j][0][1]), (
-                                data[i][j][0][2], data[i][j][0][3]), color=(128, 0, 0), thickness=2)
-                            output = cv2.putText(
-                                st.session_state['frames'][st.session_state['counter']], data[i][j][3], (data[i][j][0][0], data[i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
-                        # update image zone with detections
-                        stframe.image(output, caption='', width=500)
-                        time.sleep(0.08)
-                        # the detection is drawn, to the next one
-                        st.session_state['counter'] += 1
+                    #st.write("counter ",st.session_state['counter'])
+                    #st.write("fps",alerts[i])
+                    if draw_detections:
+                        if st.session_state['counter'] == int(alerts[i]):
+                            # draw all detections on the frame
+                            for j in range(len(data[i])):
+                                output = cv2.rectangle(st.session_state['frames'][st.session_state['counter']], (data[i][j][0][0], data[i][j][0][1]), (
+                                    data[i][j][0][2], data[i][j][0][3]), color=(128, 0, 0), thickness=2)
+                                output = cv2.putText(
+                                    st.session_state['frames'][st.session_state['counter']], data[i][j][3], (data[i][j][0][0], data[i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
+                            # update image zone with detections
+                            stframe.image(output, caption='', width=500)
+                            time.sleep(0.08)
+                            # the detection is drawn, to the next one
+                            st.session_state['counter'] += 1
 
                 stframe.image(
                     st.session_state['frames'][st.session_state['counter']], caption='', width=500)
                 time.sleep(0.08)
                 st.session_state['counter'] += 1
                     
 
@@ -162,17 +169,16 @@
         container_2.empty()
         pause = container_2.button('▶')
         resume = False
 
 def main():
 
 
-    video_path = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441603.4032989_1687441609.4032989.webm?sp=r&st=2023-07-04T15:19:38Z&se=2023-07-06T23:19:38Z&spr=https&sv=2022-11-02&sr=b&sig=beK2pXlTRKEEPSEQ31sZjkpc%2FPtQU1vpDLUN4gvX2xQ%3D"
-    down_json = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441611.4008365.json?se=2023-07-05T19%3A17%3A04Z&sp=r&sv=2021-08-06&sr=b&sig=1IkIpRp%2BVh3DkTKIVjFbvwk0nAApzGi9LiwZTrsq6AA%3D"
-    
+    video_path = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441603.4032989_1687441609.4032989.webm?se=2023-07-11T11%3A34%3A13Z&sp=r&sv=2021-08-06&sr=b&sig=GW3M0UHASHtfWJ9wbHV5v7oDbreSv5F6ApGIRW6Ypz8%3D"
+    down_json = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441603.4032989_1687441609.4032989_global.json?sv=2021-10-04&st=2023-07-10T11%3A21%3A13Z&se=2023-07-18T11%3A21%3A00Z&sr=b&sp=r&sig=NvwsYEALxwRizyL2eOAsPxQbCV7SpywLVepv6S%2FNUiQ%3D"
     if video_path is not None:
         display_video(video_path, down_json)
 
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `streamlitopencvplayer-1.3.1/test/test.py` & `streamlitopencvplayer-1.3.2/test/test.py`

 * *Files 17% similar despite different names*

```diff
@@ -56,7 +56,12 @@
         "-J",
         help="Enter the json file path",
     )
     args = parser.parse_args()
     opencvplayer = opencvplayer(
         args.video_path, args.json_file)
     opencvplayer.main()
+
+'''
+    video_path = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441603.4032989_1687441609.4032989.webm?sp=r&st=2023-07-04T15:19:38Z&se=2023-07-06T23:19:38Z&spr=https&sv=2022-11-02&sr=b&sig=beK2pXlTRKEEPSEQ31sZjkpc%2FPtQU1vpDLUN4gvX2xQ%3D"
+    down_json = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441603.4032989_1687441609.4032989_global.json?se=2023-07-05T20%3A24%3A12Z&sp=r&sv=2021-08-06&sr=b&sig=q0O120LhDaxSl63TIYOCcsKUeZDQ2ANwGV1rZT0bkPU%3D"
+'''
```


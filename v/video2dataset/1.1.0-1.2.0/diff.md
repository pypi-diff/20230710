# Comparing `tmp/video2dataset-1.1.0.tar.gz` & `tmp/video2dataset-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video2dataset-1.1.0.tar", last modified: Wed Mar 22 23:57:13 2023, max compression
+gzip compressed data, was "video2dataset-1.2.0.tar", last modified: Mon Jul 10 10:46:05 2023, max compression
```

## Comparing `video2dataset-1.1.0.tar` & `video2dataset-1.2.0.tar`

### file list

```diff
@@ -1,41 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 23:57:13.803610 video2dataset-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-22 23:57:01.000000 video2dataset-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-03-22 23:57:13.803610 video2dataset-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-03-22 23:57:01.000000 video2dataset-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 23:57:13.803610 video2dataset-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-22 23:57:01.000000 video2dataset-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 23:57:13.799610 video2dataset-1.1.0/video2dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/data_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/data_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 23:57:13.803610 video2dataset-1.1.0/video2dataset/dataloader/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/dataloader/custom_wds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/dataloader/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/dataloader/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/dataloader/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/dataloader/video_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/distributor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/input_sharder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/output_sharder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 23:57:13.803610 video2dataset-1.1.0/video2dataset/subsamplers/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/subsamplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/subsamplers/audio_rate_subsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/subsamplers/clipping_subsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/subsamplers/cut_detection_subsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/subsamplers/frame_subsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/subsamplers/noop_subsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/subsamplers/resolution_subsampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 23:57:13.803610 video2dataset-1.1.0/video2dataset/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/workers/download_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-03-22 23:57:01.000000 video2dataset-1.1.0/video2dataset/workers/subset_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 23:57:13.799610 video2dataset-1.1.0/video2dataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-03-22 23:57:13.000000 video2dataset-1.1.0/video2dataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-22 23:57:13.000000 video2dataset-1.1.0/video2dataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 23:57:13.000000 video2dataset-1.1.0/video2dataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-22 23:57:13.000000 video2dataset-1.1.0/video2dataset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-22 23:57:13.000000 video2dataset-1.1.0/video2dataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-22 23:57:13.000000 video2dataset-1.1.0/video2dataset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:05.413330 video2dataset-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-10 10:45:51.000000 video2dataset-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18150 2023-07-10 10:46:05.413330 video2dataset-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-07-10 10:45:51.000000 video2dataset-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:46:05.413330 video2dataset-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-10 10:45:51.000000 video2dataset-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:05.409330 video2dataset-1.2.0/video2dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:05.413330 video2dataset-1.2.0/video2dataset/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/data_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:05.413330 video2dataset-1.2.0/video2dataset/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/dataloader/audio_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/dataloader/custom_wds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/dataloader/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/dataloader/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/dataloader/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/dataloader/video_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/distributor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/input_sharder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/output_sharder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/slurm_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:05.413330 video2dataset-1.2.0/video2dataset/subsamplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/subsamplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/subsamplers/audio_rate_subsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/subsamplers/caption_subsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/subsamplers/clipping_subsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/subsamplers/cut_detection_subsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/subsamplers/ffprobe_subsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/subsamplers/frame_subsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/subsamplers/noop_subsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/subsamplers/optical_flow_subsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/subsamplers/resolution_subsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/subsamplers/subsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/subsamplers/whisper_subsampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:05.413330 video2dataset-1.2.0/video2dataset/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/workers/caption_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/workers/download_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/workers/optical_flow_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/workers/subset_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-10 10:45:51.000000 video2dataset-1.2.0/video2dataset/workers/whisper_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:46:05.413330 video2dataset-1.2.0/video2dataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18150 2023-07-10 10:46:05.000000 video2dataset-1.2.0/video2dataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-10 10:46:05.000000 video2dataset-1.2.0/video2dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:46:05.000000 video2dataset-1.2.0/video2dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 10:46:05.000000 video2dataset-1.2.0/video2dataset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-10 10:46:05.000000 video2dataset-1.2.0/video2dataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 10:46:05.000000 video2dataset-1.2.0/video2dataset.egg-info/top_level.txt
```

### Comparing `video2dataset-1.1.0/LICENSE` & `video2dataset-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `video2dataset-1.1.0/PKG-INFO` & `video2dataset-1.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,231 +1,252 @@
-Metadata-Version: 2.1
-Name: video2dataset
-Version: 1.1.0
-Summary: Easily create large video dataset from video urls
-Home-page: https://github.com/iejMac/video2dataset
-Author: Maciej Kilian
-Author-email: kilianmaciej6@gmail.com
-License: MIT
-Description: # video2dataset
-        [![pypi](https://img.shields.io/pypi/v/video2dataset.svg)](https://pypi.python.org/pypi/video2dataset)
-        
-        Easily create large video dataset from video urls
-        
-        ![Video2dataset design overview](video2dataset_overview.png)]
-        
-        Checkout the [design doc](https://docs.google.com/document/d/1_TD2KQLkEegszq4Eip568fc6cWnh9h0Jqj4Lc88t9Y0/edit#)
-        
-        ## Install
-        
-        pip install video2dataset
-        
-        ## Examples
-        
-        
-        ## Usage
-        
-        First get some video url list. For example:
-        ```
-        echo 'https://www.youtube.com/watch?v=0WfKzVqdQqo' >> myvidlist.txt
-        ```
-        
-        Then, run the tool:
-        
-        ```
-        video2dataset --url_list=myvidlist.txt --output_folder=output_folder
-        ```
-        
-        The tool will then automatically download the urls and store them with that format:
-        * output_folder
-            * 00000
-                * 000000000.mp4
-                * 000000001.mp4
-                * 000000002.mp4
-        
-        or as this format if choosing webdataset:
-        * output_folder
-            * 00000.tar containing:
-                * 000000000.mp4
-                * 000000001.mp4
-                * 000000002.mp4
-        
-        with each number being the position in the list. The subfolders avoids having too many files in a single folder.
-        
-        If **captions** are provided, they will be saved as 0.txt, 1.txt, ...
-        
-        This can then easily be fed into machine learning training or any other use case.
-        
-        Also .json files named 0.json, 1.json,... are saved with these keys:
-        * url
-        * caption
-        * key of the form 000010005 : the first 5 digits are the shard id, the last 4 are the index in the shard
-        * status : whether the download succeeded
-        * error_message
-        
-        Also a .parquet file will be saved with the same name as the subfolder/tar files containing these same metadata.
-        It can be used to analyze the results efficiently.
-        
-        .json files will also be saved with the same name suffixed by _stats, they contain stats collected during downloading (download time, number of success, ...)
-        
-        
-        ## API
-        
-        This module exposes a single function `download` which takes the same arguments as the command line tool:
-        
-        * **url_list** A file with the list of url of images to download. It can be a folder of such files. (*required*)
-        * **output_folder** The path to the output folder. (default *"images"*)
-        * **processes_count** The number of processes used for downloading the pictures. This is important to be high for performance. (default *1*)
-        * **encode_formats** Dict of (modality, format) pairs specifying what file format each modality should be saved as. This determines which modalities will be written in the output dataset f.e. if we only specify audio only audio wil be saved (default *{"video": "mp4"}*)
-        * **output_format** decides how to save pictures (default *files*)
-          * **files** saves as a set of subfolder containing pictures
-          * **webdataset** saves as tars containing pictures
-          * **parquet** saves as parquet containing pictures as bytes
-          * **tfrecord** saves as tfrecord containing pictures as bytes
-          * **dummy** does not save. Useful for benchmarks
-        * **input_format** decides how to load the urls (default *txt*)
-          * **txt** loads the urls as a text file of url, one per line
-          * **csv** loads the urls and optional caption as a csv
-          * **tsv** loads the urls and optional caption as a tsv
-          * **tsv.gz** loads the urls and optional caption as a compressed (gzip) tsv.gz
-          * **json** loads the urls and optional caption as a json
-          * **parquet** loads the urls and optional caption as a parquet
-        * **url_col** the name of the url column for parquet and csv (default *url*)
-        * **caption_col** the name of the caption column for parquet and csv (default *None*)
-        * **clip_col** the name of the column with a list of timespans for each clip (defualt *None*)
-        * **save_additional_columns** list of additional columns to take from the csv/parquet files and save in metadata files (default *None*)
-        * **number_sample_per_shard** the number of sample that will be downloaded in one shard (default *10000*)
-        * **timeout** maximum time (in seconds) to wait when trying to download an image (default *10*)
-        * **video_size** size of video frames (default *360*)
-        * **resize_mode** what resizing transformations to apply to video resolution (default *None*)
-          * **scale** scale video keeping aspect ratios (currently always picks video height)
-          * **crop** center crop to video_size x video_size
-          * **pad** center pad to video_size x video_size
-        * **video_fps** what FPS to resample the video to. If < 0 then video FPS remains unchanged (default *-1*)
-        * **audio_rate** audio sampling rate, by default (-1) it is left unchanged from the downloaded video (default *-1*)
-        * **enable_wandb** whether to enable wandb logging (default *False*)
-        * **wandb_project** name of W&B project used (default *video2dataset*)
-        * **oom_shard_count** the order of magnitude of the number of shards, used only to decide what zero padding to use to name the shard files (default *5*)
-        * **distributor** choose how to distribute the downloading (default *multiprocessing*)
-          * **multiprocessing** use a multiprocessing pool to spawn processes
-          * **pyspark** use a pyspark session to create workers on a spark cluster (see details below)
-        * **subjob_size** the number of shards to download in each subjob supporting it, a subjob can be a pyspark job for example (default *1000*)
-        * **incremental_mode** Can be "incremental" or "overwrite". For "incremental", video2dataset will download all the shards that were not downloaded, for "overwrite" video2dataset will delete recursively the output folder then start from zero (default *incremental*)
-        * **tmp_dir** name of temporary directory in your file system (default */tmp*)
-        * **yt_metadata_args** dict of YouTube metadata arguments (default *None*, more info below)
-        * **detect_cuts** whether or not to detect jump-cuts in each video and store as metadata (default *False*)
-        * **cut_detection_mode** Can be either "longest" or "all" -- "longest" will select the longest contiguous (i.e. no jump-cuts) section of video, and "all" will select all contiguous sections of video to store in metadata (default *"longest"*)
-        * **cut_framerates** a list of additional framerates to detect jump cuts at. If None, jump cuts will only be detected at the original framerate of the video (default *None*)
-        * **cuts_are_clips** whether or not to turn each contiguous section of each input video into a distinct ouput video (default *False*)
-        * **stage** which stage of processing to execute in betweeen downloading + cheap subsampling and costly subsampling (default *"download"*)
-        
-        ## Downloading YouTube Metadata
-        
-        If we want to download a large amount of YouTube videos with video2dataset we can specify some parameters and also extract useful metadata as well. For directions on how to do so please see this [example](https://github.com/iejMac/video2dataset/blob/main/examples/yt_metadata.md).
-        
-        ## Incremental mode
-        
-        If a first download got interrupted for any reason, you can run again with --incremental "incremental" (this is the default) and using the same output folder , the same number_sample_per_shard and the same input urls, and video2dataset will complete the download.
-        
-        ## Output format choice
-        
-        video2dataset support several formats. There are trade off for which to choose:
-        * files: this is the simplest one, images are simply saved as files. It's good for up to 1M samples on a local file system. Beyond that performance issues appear very fast. Handling more than a million files in standard filesystem does not work well.
-        * webdataset: webdataset format saves samples in tar files, thanks to [webdataset](https://webdataset.github.io/webdataset/) library, this makes it possible to load the resulting dataset fast in both pytorch, tensorflow and jax. Choose this for most use cases. It works well for any filesystem
-        * parquet: parquet is a columnar format that allows fast filtering. It's particularly easy to read it using pyarrow and pyspark. Choose this if the rest of your data ecosystem is based on pyspark. [petastorm](https://github.com/uber/petastorm) can be used to read the data but it's not as easy to use as webdataset
-        * tfrecord: tfrecord is a protobuf based format. It's particularly easy to use from tensorflow and using [tf data](https://www.tensorflow.org/guide/data). Use this if you plan to use the dataset only in the tensorflow ecosystem. The tensorflow writer does not use fsspec and as a consequence supports only a limited amount of filesystem, including local, hdfs, s3 and gcs. It is also less efficient than the webdataset writer when writing to other filesystems than local, losing some 30% performance.
-        
-        ## File system support
-        
-        Thanks to [fsspec](https://filesystem-spec.readthedocs.io/en/latest/), video2dataset supports reading and writing files in [many file systems](https://github.com/fsspec/filesystem_spec/blob/6233f315548b512ec379323f762b70764efeb92c/fsspec/registry.py#L87).
-        To use it, simply use the prefix of your filesystem before the path. For example `hdfs://`, `s3://`, `http://`, or `gcs://`.
-        Some of these file systems require installing an additional package (for example s3fs for s3, gcsfs for gcs).
-        See fsspec doc for all the details.
-        
-        If you need specific configuration for your filesystem, you may handle this problem by using the [fsspec configuration system](https://filesystem-spec.readthedocs.io/en/latest/features.html#configuration) that makes it possible to create a file such as `.config/fsspec/s3.json` and have information in it such as:
-        ```
-        {
-          "s3": {
-            "client_kwargs": {
-                    "endpoint_url": "https://some_endpoint",
-                    "aws_access_key_id": "your_user",
-                   "aws_secret_access_key": "your_password"
-            }
-          }
-        }
-        ```
-        Which may be necessary if using s3 compatible file systems such as [minio](https://min.io/). That kind of configuration also work for all other fsspec-supported file systems.
-        
-        ## Distribution modes
-        
-        video2dataset supports several distributors.
-        * multiprocessing which spawns a process pool and use these local processes for downloading
-        * pyspark which spawns workers in a spark pool to do the downloading
-        
-        multiprocessing is a good option for downloading on one machine, and as such it is the default.
-        Pyspark lets video2dataset use many nodes, which makes it as fast as the number of machines.
-        It can be particularly useful if downloading datasets with more than a billion image. Here's an [example](https://github.com/iejMac/video2dataset/blob/main/examples/distributed_spark.md)
-        for how we used pyspark distributed mode to download 40M videos with metadata.
-        
-        ### pyspark configuration
-        
-        In order to use video2dataset with pyspark, you will need to do this:
-        1. `pip install pyspark`
-        2. use the `--distributor pyspark` option
-        3. tweak the `--subjob_size 1000` option: this is the number of images to download in each subjob. Increasing it will mean a longer time of preparation to put the feather files in the temporary dir, a shorter time will mean sending less shards at a time to the pyspark job.
-        
-        By default a local spark session will be created.
-        You may want to create a custom spark session depending on your specific spark cluster.
-        
-        
-        ## For development
-        
-        Either locally, or in [gitpod](https://gitpod.io/#https://github.com/iejMac/video2dataset) (do `export PIP_USER=false` there)
-        
-        Setup a virtualenv:
-        
-        ```
-        python3 -m venv .env
-        source .env/bin/activate
-        pip install -e .
-        ```
-        
-        to run tests:
-        ```
-        pip install -r requirements-test.txt
-        ```
-        then 
-        ```
-        make lint
-        make test
-        ```
-        
-        You can use `make black` to reformat the code
-        
-        `python -m pytest -x -s -v tests -k "dummy"` to run a specific test
-        
-        ## Benchmarks
-        
-        ## Special Contributors:
-        
-        * [ChatGPT](https://chat.openai.com) - FrameSubsampler implementation
-        
-        ## Citation
-        ```
-        @misc{beaumont-2023-video2dataset,
-          author = {Romain Beaumont, Maciej Kilian},
-          title = {video2dataset: Easily turn large sets of video urls to a video dataset},
-          year = {2023},
-          publisher = {GitHub},
-          journal = {GitHub repository},
-          howpublished = {\url{https://github.com/iejMac/video2dataset}}
-        }
-        ```
-        
-Keywords: machine learning
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
+# video2dataset
+[![pypi](https://img.shields.io/pypi/v/video2dataset.svg)](https://pypi.python.org/pypi/video2dataset)
+
+Easily create large video dataset from video urls. Can download and package 10M videos in 12h on a single 16 core machine.
+
+![video2dataset design overview](docs/video2dataset_overview.png)
+
+## Install
+
+```
+pip install video2dataset
+```
+
+Or from source via
+
+```
+git clone https://github.com/iejMac/video2dataset
+cd video2dataset
+pip install -e .
+```
+
+## Usage
+
+First get some video urls and metadata. For example lets save this small animal video dataset to a csv file called `videos.csv`
+```
+url,caption
+https://www.youtube.com/watch?v=od_PmtmMDV0,Driving to the banana store
+https://www.youtube.com/watch?v=8FhGOV7fs64,Polar bear eating
+https://www.youtube.com/watch?v=TReCLbmhlMs,Cat scared of printer
+```
+
+Then, run the tool:
+
+```
+video2dataset --url_list="videos.csv" --url_col="url" --caption_col="caption" --output_folder="dataset"
+```
+If you go into the output folder you should see a nice small video dataset stored with all relevant metadata.
+
+## Examples
+
+Here are some more concrete examples of video2dataset usage.
+
+#### WebVid download
+
+The WebVid dataset is a high quality video-text of 10M stock videos. It can be easily downloaded and stored using [one video2dataset command](https://github.com/iejMac/video2dataset/blob/main/examples/download_webvid.sh), to perform the same on the train split (much larger) you just need to swap out the csv file and update the distribution params to something more beefy. Here's an [example config](https://github.com/iejMac/video2dataset/blob/main/examples/default_slurm.yaml) that adjusts the default config for slurm distribution (so we can use many nodes to download it quickly).
+
+#### Re-processing
+
+video2dataset is designed such that you can chain together runs to re-process your downloaded data since `webdataset` is a valid `input_format`. Here's an example - with the WebVid data you downloaded in the previous example you can also run [this script](https://github.com/iejMac/video2dataset/blob/main/examples/optical_flow_webvid.sh) which will compute the optical flow for each video and store it in metadata shards (shards which only have the optical flow metadata in them). You can also run [this script](https://github.com/iejMac/video2dataset/blob/main/examples/downsample_webvid.sh) which will take those videos and perform resizing, fps downsampling, cut detection, and clipping and also store that in a new dataset. We make sure that the content in shards with the same IDs is the same across re-processing runs. Furthermore, if clipping is not performed shard IDs *and* sample IDs are exactly the same since clipping is the only transformation that changes the sample IDs i.e. if sample `000` is clipped into 3 clips they will be split into `000_000`, `000_001`, `000_002`.
+
+#### Dataloading
+
+Once you download some chunk of WebVid (or any video dataset) you can load it using our dataloader like in [this example](https://github.com/iejMac/video2dataset/blob/main/examples/dataloader_example.py). Try it out.
+
+#### Large processing job examples
+
+Whenever we do a large dataset processing job we document them in [dataset examples](https://github.com/iejMac/video2dataset/tree/main/dataset_examples) as many existing datasets are unique and might require special procesing or the authors just don't specify the best ways of getting the data. Thanks to this we can all share the most efficient ways of processing large video/audio datasets!
+
+## Output format
+
+The tool will automatically download the urls and store them with the format:
+
+* output_folder
+    * 00000{.ext if output_format != files, can be tar, parquet, tfrecord, etc.}
+        * 000000000.mp4
+        * 000000001.mp4
+        * 000000002.mp4
+
+with each number being the position in the input table or the input sample ID. The subfolders avoid having too many files in a single folder. If **captions** are provided, they will be saved as 0.txt, 1.txt, etc. (matching the ID of the sample they belong to). This can then easily be fed into machine learning training or any other use case.
+
+Also .json files named 0.json, 1.json,... are saved with these keys:
+* url
+* caption
+* key of the form 000010005: the first 5 digits are the shard id, the last 4 are the index in the shard
+* additionally gathered metadata (either specified from input table or collected during downloading/processing)
+* status: whether the download succeeded
+* error_message
+
+Also a .parquet file will be saved with the same name as the subfolder/tar files containing these same metadata.
+It can be used to analyze the results efficiently.
+
+.json files will also be saved with the same name suffixed by _stats, they contain stats collected during downloading (download time, number of success, ...)
+
+### Output format choice
+
+video2dataset support several formats. There are trade off for which to choose:
+* files: this is the simplest one, videos are simply saved as files. It's good for up to 1M samples on a local file system. Beyond that performance issues appear very fast. Handling more than a million files in standard filesystem does not work well.
+* webdataset: webdataset format saves samples in tar files, thanks to [webdataset](https://webdataset.github.io/webdataset/) library, this makes it possible to load the resulting dataset fast in both pytorch, tensorflow and jax. Choose this for most use cases. It works well for any filesystem
+* parquet: parquet is a columnar format that allows fast filtering. It's particularly easy to read it using pyarrow and pyspark. Choose this if the rest of your data ecosystem is based on pyspark. [petastorm](https://github.com/uber/petastorm) can be used to read the data but it's not as easy to use as webdataset
+* tfrecord: tfrecord is a protobuf based format. It's particularly easy to use from tensorflow and using [tf data](https://www.tensorflow.org/guide/data). Use this if you plan to use the dataset only in the tensorflow ecosystem. The tensorflow writer does not use fsspec and as a consequence supports only a limited amount of filesystem, including local, hdfs, s3 and gcs. It is also less efficient than the webdataset writer when writing to other filesystems than local, losing some 30% performance.
+
+
+## API
+
+The module exposes a single function `video2dataset` which takes the same arguments as the command line tool:
+
+```
+url_list: list of input urls - can be any of the supported input formats
+    (csv, parquet, braceexpand tar paths etc.)
+output_folder: Desired location of output dataset (default = "dataset")
+output_format: Format of output dataset, can be (default = "files")
+    - files, samples saved in subdirectory for each shard (useful for debugging)
+    - webdataset, samples saved in tars (useful for efficient loading)
+    - parquet, sampels saved in parquet (as bytes)
+    - tfrecord, samples saved in tfrecord (as bytes)
+    - dummy, does not save (useful for benchmarks)
+input_format: Format of the input, can be (default = "csv")
+    - txt, text file with a url in each line
+    - csv, csv file with urls, (and captions + metadata)
+    - tsv, tsv - || -
+    - tsv.gz, - || - but compressed gzip
+    - json, loads urls and metadata as json
+    - parquet, loads urls and metadata as parquet
+    - webdataset, usually braceexpand format of mutliple paths to tars to re-process
+encode_formats: Dict that specifies what extension each modality should use (default = "{'video': 'mp4'}")
+    f.e. {"video": "mp4", "audio": "m4a"}
+stage: String that tells video2dataset what stage of processing is being performed. Can be (default = 'download')
+    WARNING: To be depracated soon (this information should be deduced based on config)
+    - download, when input is some tabular format and data must be downloaded first
+    - subset, tar files are already written and we would like to re-process (input_format == "webdataset")
+    - optical_flow, tar files are written and we woudl like to compute optical_flow and save to md shards
+url_col: Column in input (if has columns) that contains the url (default = "url")
+caption_col: Column in input (if has columns) that contains captions (to be written as txt) (default = None)
+clip_col: Column in input (if has columns) that contains timeframes of clips for how to split video (default = None)
+save_additional_columns: List of column names to save to json component of a sample (defualt = None)
+enable_wandb: Whether or not to log info to wandb (default = False)
+wandb_project: Name of wandb project to log runs to (default = "video2dataset")
+incremental_mode: Decides how to handle restarting, Can be (default = "incremental")
+    - incremental, checks which shards are done and skips those
+    - overwrite, deletes and reprocesses shards as it goes
+max_shard_retry: Maximum amount of attempts to retry a failed shard (default = 1)
+tmp_dir: Path to temporary directory on your file system (default = "/tmp")
+config: Path to your config of choice or the config itself (more info on configs in API doc) (default = "default")
+```
+
+These arguments give coarse control over input/output "shape" of the dataset. For finer control of subsamplers, distribution, reading, and storage see the more detailed [API.md](https://github.com/iejMac/video2dataset/blob/main/API.md) doc.
+
+## Downloading YouTube Metadata
+
+If we want to download a large amount of YouTube videos with video2dataset we can specify some parameters and also extract useful metadata as well. For directions on how to do so please see this [example](https://github.com/iejMac/video2dataset/blob/main/examples/yt_metadata.md).
+
+## Incremental mode
+
+If a first download got interrupted for any reason, you can run again with --incremental "incremental" (this is the default) and using the same output folder , the same number_sample_per_shard and the same input urls, and video2dataset will complete the download.
+
+## File system support
+
+Thanks to [fsspec](https://filesystem-spec.readthedocs.io/en/latest/), video2dataset supports reading and writing files in [many file systems](https://github.com/fsspec/filesystem_spec/blob/6233f315548b512ec379323f762b70764efeb92c/fsspec/registry.py#L87).
+To use it, simply use the prefix of your filesystem before the path. For example `hdfs://`, `s3://`, `http://`, or `gcs://`.
+Some of these file systems require installing an additional package (for example s3fs for s3, gcsfs for gcs).
+See fsspec doc for all the details.
+
+If you need specific configuration for your filesystem, you may handle this problem by using the [fsspec configuration system](https://filesystem-spec.readthedocs.io/en/latest/features.html#configuration) that makes it possible to create a file such as `.config/fsspec/s3.json` and have information in it such as:
+```
+{
+  "s3": {
+    "client_kwargs": {
+            "endpoint_url": "https://some_endpoint",
+            "aws_access_key_id": "your_user",
+            "aws_secret_access_key": "your_password"
+    }
+  }
+}
+```
+Which may be necessary if using s3 compatible file systems such as [minio](https://min.io/). That kind of configuration also work for all other fsspec-supported file systems.
+
+## Distribution modes
+
+video2dataset supports several distributors.
+* multiprocessing which spawns a process pool and use these local processes for downloading
+* pyspark which spawns workers in a spark pool to do the downloading
+* slurm which starts separate worker nodes
+
+multiprocessing is a good option for downloading on one machine, and as such it is the default.
+Pyspark lets video2dataset use many nodes, which makes it as fast as the number of machines.
+It can be particularly useful if downloading datasets with more than a billion image. Here's an [example](https://github.com/iejMac/video2dataset/blob/main/examples/distributed_spark.md)
+for how we used pyspark distributed mode to download 40M videos with metadata. If you have access to a slurm cluster it is more comfortable to use than pyspark but not everyone does.
+
+### pyspark configuration
+
+In order to use video2dataset with pyspark, you will need to do this:
+1. `pip install pyspark`
+2. set `distributor: pyspark` in your config
+3. tweak the `subjob_size: 1000` option in your config. This is the number of videos to download in each subjob. Increasing it will mean a longer time of preparation to put the feather files in the temporary dir, a shorter time will mean sending less shards at a time to the pyspark job.
+
+By default a local spark session will be created.
+You may want to create a custom spark session depending on your specific spark cluster.
+
+## Benchmarks
+
+As stated at the top of the README - video2dataset is capable of downloading 10M videos in 12h. For more details on end2end performance please see specific runs in [dataset examples](https://github.com/iejMac/video2dataset/tree/main/dataset_examples) as there are nuances to video (how long it is, where it comes from etc.). For example it takes considerably longer to pul videos from youtube than just mp4 links (compare [WebVid.md](https://github.com/iejMac/video2dataset/tree/main/dataset_examples/WebVid.md) to [VideoCC.md](https://github.com/iejMac/video2dataset/tree/main/dataset_examples/VideoCC.md)). Each example should have a "Performance" statement at the bottom which should contain info about download/processing performance (video/s, Mb/s) along with a cost estimate on popular cloud infrastructure.
+
+For information about video2dataset subsampler speed please check out the [benchmark suite](https://github.com/iejMac/video2dataset/tree/main/benchmark) which contains code that produces performance numbers for subsamplers, over a grid of parameters, on a given architecture. It also contains a json file with some results we produced. This can be used to estimate costs of big runs and also to optimize the subsamplers. NOTE: cost can drastically vary based on chosen subsampler configuration.
+
+## Integration with Weights & Biases
+
+If you pass the `--enable_wandb=True` parameter then performance metrics will be logged to [Weights & Biases](https://wandb.com/)
+
+![W&B metrics](docs/wandb_logs.png)
+
+In addition, most frequent errors are logged for easier debugging
+
+![W&B status](docs/wandb_status.png)
+
+Other features are available:
+
+* logging of environment configuration (OS, python version, CPU count, Hostname, etc)
+* monitoring of hardware resources (GPU/CPU, RAM, Disk, Networking, etc)
+* custom graphs and reports
+* comparison of runs (convenient when optimizing parameters such as number of threads/cpus)
+
+When running the script for the first time, you can decide to either associate your metrics to your account or log them anonymously.
+
+You can also log in (or create an account) before by running `wandb login`.	
+
+## For development
+
+Either locally, or in [gitpod](https://gitpod.io/#https://github.com/iejMac/video2dataset) (do `export PIP_USER=false` there)
+
+Setup a virtualenv:
+
+```
+python3 -m venv .env
+source .env/bin/activate
+pip install -e .
+```
+
+to run tests:
+```
+pip install -r requirements-test.txt
+```
+then 
+```
+make lint
+make test
+```
+
+You can use `make black` to reformat the code
+
+`python -m pytest -x -s -v tests -k "dummy"` to run a specific test
+
+## Citation
+```
+@misc{beaumont-2023-video2dataset,
+  author = {Romain Beaumont, Maciej Kilian},
+  title = {video2dataset: Easily turn large sets of video urls to a video dataset},
+  year = {2023},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/iejMac/video2dataset}}
+}
+```
```

### Comparing `video2dataset-1.1.0/setup.py` & `video2dataset-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     REQUIREMENTS = _read_reqs("requirements.txt")
 
     setup(
         name="video2dataset",
         packages=find_packages(),
         include_package_data=True,
-        version="1.1.0",
+        version="1.2.0",
         license="MIT",
         description="Easily create large video dataset from video urls",
         long_description=long_description,
         long_description_content_type="text/markdown",
         entry_points={"console_scripts": ["video2dataset=video2dataset.main:main"]},
         author="Maciej Kilian",
         author_email="kilianmaciej6@gmail.com",
```

### Comparing `video2dataset-1.1.0/video2dataset/data_reader.py` & `video2dataset-1.2.0/video2dataset/data_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         'get_info': True
     }
 
     writesubtitles:    Whether to write subtitles
     writeautomaticsub: Write the automatically generated subtitles to a file
     subtitleslangs:    List of languages of the subtitles to download.
     get_info: whether to add info (title, description, tags etc) to the output.
-
     """
 
     write_subs = yt_metadata_args.get("writesubtitles", None)
 
     yt_metadata_args["skip_download"] = True
     yt_metadata_args["ignoreerrors"] = True
     yt_metadata_args["quiet"] = True
@@ -96,15 +95,15 @@
             info_dict = None
 
         yt_meta_dict = {"info": info_dict, "subtitles": sub_dict}
 
         return yt_meta_dict
 
 
-def get_web_file_info(url):
+def get_file_info(url):
     """returns info about the url (currently extension and modality)"""
     # TODO: make this nicer
     video_extensions = ["mp4", "webm", "mov", "avi", "mkv"]
     audio_extensions = ["mp3", "wav", "m4a"]
     for ext in video_extensions:
         if url.endswith(f".{ext}"):
             return ext, "video"
@@ -120,19 +119,27 @@
     def __init__(self, timeout, tmp_dir, encode_formats):
         self.timeout = timeout
         self.tmp_dir = tmp_dir
         self.encode_formats = encode_formats
 
     def __call__(self, url):
         modality_paths = {}
-        resp = requests.get(url, stream=True, timeout=self.timeout)
-        ext, modality = get_web_file_info(url)
+
+        ext, modality = get_file_info(url)
+        if not os.path.isfile(url):
+            resp = requests.get(url, stream=True, timeout=self.timeout)
+            byts = resp.content
+        else:  # local files (don't want to delete)
+            with open(url, "rb") as f:
+                byts = f.read()
+
         modality_path = f"{self.tmp_dir}/{str(uuid.uuid4())}.{ext}"
         with open(modality_path, "wb") as f:
-            f.write(resp.content)
+            f.write(byts)
+
         modality_paths[modality] = modality_path
 
         if modality == "video" and self.encode_formats.get("audio", None):
             audio_format = self.encode_formats["audio"]
             audio_path = video2audio(modality_paths["video"], audio_format, self.tmp_dir)
             if audio_path is not None:
                 modality_paths["audio"] = audio_path
@@ -142,91 +149,122 @@
                 os.remove(modality_path)
                 modality_path.pop(modality)
 
         return modality_paths, None
 
 
 class YtDlpDownloader:
-    """Downloader class for yt-dlp links"""
+    """Downloader class for yt-dlp links
+
+    yt_args:
+        download_size: preferred height of video to download. Will try to download smallest video >=download_size
+        download_audio_rate: same as size but with audio
+        yt_metadata_args: see get_yt_metadata function docstring
+    """
 
     # TODO: maybe we just include height and width in the metadata_args
-    def __init__(self, tmp_dir, metadata_args, video_size, audio_rate, encode_formats):
+    def __init__(self, yt_args, tmp_dir, encode_formats):
+        self.metadata_args = yt_args.get("yt_metadata_args", {})
+        self.video_size = yt_args.get("download_size", 360)
+        self.audio_rate = yt_args.get("download_audio_rate", 44100)
         self.tmp_dir = tmp_dir
-        self.metadata_args = metadata_args
-        self.video_size = video_size
-        self.audio_rate = audio_rate
         self.encode_formats = encode_formats
 
+        # TODO: figure out when to do this
+        # was relevant with HD videos for loading with decord
+        self.specify_codec = False
+
     def __call__(self, url):
         modality_paths = {}
 
-        # video_format_string = f"bv*[height<={self.video_size}][ext=mp4]/b[height<={self.video_size}][ext=mp4] / wv/w[ext=mp4]"
         video_format_string = (
-            f"wv*[height>={self.video_size}][ext=mp4]/w[height>={self.video_size}][ext=mp4] / bv/b[ext=mp4]"
+            f"wv*[height>={self.video_size}][ext=mp4]{'[codec=avc1]' if self.specify_codec else ''}/"
+            f"w[height>={self.video_size}][ext=mp4]{'[codec=avc1]' if self.specify_codec else ''}/"
+            f"bv/b[ext=mp4]{'[codec=avc1]' if self.specify_codec else ''}"
         )
         audio_fmt_string = (
             f"wa[asr>={self.audio_rate}][ext=m4a] / ba[ext=m4a]" if self.audio_rate > 0 else "ba[ext=m4a]"
         )
 
         if self.encode_formats.get("audio", None):
             audio_path_m4a = f"{self.tmp_dir}/{str(uuid.uuid4())}.m4a"
             ydl_opts = {
                 "outtmpl": audio_path_m4a,
                 "format": audio_fmt_string,
                 "quiet": True,
             }
-            with yt_dlp.YoutubeDL(ydl_opts) as ydl:
-                ydl.download(url)
 
-            # TODO: look into this, don't think we can just do this
-            # TODO: just figure out a way to download the preferred extension using yt-dlp
-            # audio_path = audio_path_m4a.replace(".m4a", f".{self.encode_formats['audio']}")
-            audio_path = audio_path_m4a
-            modality_paths["audio"] = audio_path
+            err = None
+            try:
+                with yt_dlp.YoutubeDL(ydl_opts) as ydl:
+                    ydl.download(url)
+            except Exception as e:  # pylint: disable=(broad-except)
+                err = str(e)
+                os.remove(audio_path_m4a)
+
+            if err is None:
+                # TODO: look into this, don't think we can just do this
+                # TODO: just figure out a way to download the preferred extension using yt-dlp
+                # audio_path = audio_path_m4a.replace(".m4a", f".{self.encode_formats['audio']}")
+                audio_path = audio_path_m4a
+                modality_paths["audio"] = audio_path
 
         if self.encode_formats.get("video", None):
             video_path = f"{self.tmp_dir}/{str(uuid.uuid4())}.mp4"
-            modality_paths["video"] = video_path
             ydl_opts = {
                 "outtmpl": video_path,
                 "format": video_format_string,
                 "quiet": True,
             }
 
-            with yt_dlp.YoutubeDL(ydl_opts) as ydl:
-                ydl.download(url)
+            err = None
+            try:
+                with yt_dlp.YoutubeDL(ydl_opts) as ydl:
+                    ydl.download(url)
+            except Exception as e:  # pylint: disable=(broad-except)
+                err = str(e)
+                os.remove(video_path)
 
-        if self.metadata_args:
-            yt_meta_dict = get_yt_meta(url, self.metadata_args)
-        else:
+            if err is None:
+                modality_paths["video"] = video_path
+
+        err = None
+        try:
+            if self.metadata_args:
+                yt_meta_dict = get_yt_meta(url, self.metadata_args)
+            else:
+                yt_meta_dict = {}
+        except Exception as e:  # pylint: disable=(broad-except)
+            err = str(e)
             yt_meta_dict = {}
+
         return modality_paths, yt_meta_dict, None
 
 
 class VideoDataReader:
     """Video data reader provide data for a video"""
 
-    def __init__(self, video_size, audio_rate, dl_timeout, tmp_dir, yt_meta_args, encode_formats) -> None:
-        self.webfile_downloader = WebFileDownloader(dl_timeout, tmp_dir, encode_formats)
-        self.yt_downloader = YtDlpDownloader(tmp_dir, yt_meta_args, video_size, audio_rate, encode_formats)
+    def __init__(self, encode_formats, tmp_dir, reading_config):
+        self.webfile_downloader = WebFileDownloader(reading_config["timeout"], tmp_dir, encode_formats)
+        self.yt_downloader = YtDlpDownloader(reading_config["yt_args"], tmp_dir, encode_formats)
 
     def __call__(self, row):
         key, url = row
 
         meta_dict = None
-        # TODO: make nice function to detect what type of link we're dealing with
-        if get_web_file_info(url):  # web file that can be directly downloaded
-            modality_paths, error_message = self.webfile_downloader(url)
-        elif "youtube" in url:  # youtube link
-            try:
+        try:
+            # TODO: make nice function to detect what type of link we're dealing with
+            if get_file_info(url):  # web file that can be directly downloaded
+                modality_paths, error_message = self.webfile_downloader(url)
+            elif "youtube" in url:  # youtube link
                 modality_paths, meta_dict, error_message = self.yt_downloader(url)
-            except Exception as e:  # pylint: disable=(broad-except)
-                modality_paths, meta_dict, error_message = {}, None, str(e)
-        else:
-            modality_paths, error_message = {}, "Warning: Unsupported URL type"
+            else:
+                modality_paths, error_message = {}, "Warning: Unsupported URL type"
+        except Exception as e:  # pylint: disable=(broad-except)
+            modality_paths, meta_dict, error_message = {}, None, str(e)
 
         streams = {}
         for modality, modality_path in modality_paths.items():
             with open(modality_path, "rb") as modality_file:
                 streams[modality] = modality_file.read()
             os.remove(modality_path)
```

### Comparing `video2dataset-1.1.0/video2dataset/data_writer.py` & `video2dataset-1.2.0/video2dataset/data_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,23 @@
             self.parquet_writer = None
             self.output_fd.close()
 
 
 class ParquetSampleWriter:
     """ParquetSampleWriter is a video+caption writer to parquet"""
 
-    def __init__(self, shard_id, output_folder, save_caption, oom_shard_count, schema, encode_formats):
+    def __init__(
+        self,
+        shard_id,
+        output_folder,
+        save_caption,
+        oom_shard_count,
+        schema,
+        encode_formats,
+    ):
         self.oom_shard_count = oom_shard_count
         for fmt in encode_formats.values():
             schema = schema.append(pa.field(fmt, pa.binary()))
         shard_name = (
             shard_id
             if isinstance(shard_id, str)
             else "{shard_id:0{oom_shard_count}d}".format(  # pylint: disable=consider-using-f-string
@@ -72,30 +80,39 @@
         self.save_caption = save_caption
         self.encode_formats = encode_formats
 
     def write(self, streams, key, caption, meta):
         """Keep sample in memory then write to disk when close() is called"""
         sample = {"key": key}
         for modality, stream in streams.items():
-            sample[self.encode_formats[modality]] = stream
+            ext = self.encode_formats[modality] if modality in self.encode_formats else modality
+            sample[ext] = stream
 
         if self.save_caption:
             sample["txt"] = str(caption) if caption is not None else ""
         sample.update(meta)
 
         self.buffered_parquet_writer.write(sample)
 
     def close(self):
         self.buffered_parquet_writer.close()
 
 
 class WebDatasetSampleWriter:
     """WebDatasetSampleWriter is a video+caption writer to webdataset"""
 
-    def __init__(self, shard_id, output_folder, save_caption, oom_shard_count, schema, encode_formats):
+    def __init__(
+        self,
+        shard_id,
+        output_folder,
+        save_caption,
+        oom_shard_count,
+        schema,
+        encode_formats,
+    ):
         self.oom_shard_count = oom_shard_count
         shard_name = (
             shard_id
             if isinstance(shard_id, str)
             else "{shard_id:0{oom_shard_count}d}".format(  # pylint: disable=consider-using-f-string
                 shard_id=shard_id, oom_shard_count=oom_shard_count
             )
@@ -108,15 +125,16 @@
         self.buffered_parquet_writer = BufferedParquetWriter(output_folder + "/" + shard_name + ".parquet", schema, 100)
         self.encode_formats = encode_formats
 
     def write(self, streams, key, caption, meta):
         """write sample to tars"""
         sample = {"__key__": key}
         for modality, stream in streams.items():
-            sample[self.encode_formats[modality]] = stream
+            ext = self.encode_formats[modality] if modality in self.encode_formats else modality
+            sample[ext] = stream
 
         if self.save_caption:
             sample["txt"] = str(caption) if caption is not None else ""
         # some meta data may not be JSON serializable
         for k, v in meta.items():
             if isinstance(v, np.ndarray):
                 meta[k] = v.tolist()
@@ -130,19 +148,29 @@
         self.tarwriter.close()
         self.tar_fd.close()
 
 
 class TFRecordSampleWriter:
     """TFRecordSampleWriter is a video+caption writer to TFRecord"""
 
-    def __init__(self, shard_id, output_folder, save_caption, oom_shard_count, schema, encode_formats):
+    def __init__(
+        self,
+        shard_id,
+        output_folder,
+        save_caption,
+        oom_shard_count,
+        schema,
+        encode_formats,
+    ):
         try:
             os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
             import tensorflow_io as _  # pylint: disable=import-outside-toplevel
-            from tensorflow.python.lib.io.tf_record import TFRecordWriter  # pylint: disable=import-outside-toplevel
+            from tensorflow.python.lib.io.tf_record import (  # pylint: disable=import-outside-toplevel
+                TFRecordWriter,
+            )  # pylint: disable=import-outside-toplevel
             from tensorflow.python.training.training import (  # pylint: disable=import-outside-toplevel
                 BytesList,
                 Example,
                 Feature,
                 Features,
                 FloatList,
                 Int64List,
@@ -174,15 +202,16 @@
         self.buffered_parquet_writer = BufferedParquetWriter(output_folder + "/" + shard_name + ".parquet", schema, 100)
         self.encode_formats = encode_formats
 
     def write(self, streams, key, caption, meta):
         """Write a sample using tfrecord writer"""
         sample = {"key": self._bytes_feature(key.encode())}
         for modality, stream in streams.items():
-            sample[self.encode_formats[modality]] = self._bytes_feature(stream)
+            ext = self.encode_formats[modality] if modality in self.encode_formats else modality
+            sample[ext] = self._bytes_feature(stream)
 
         if self.save_caption:
             sample["txt"] = self._bytes_feature(str(caption) if caption is not None else "")
         for k, v in meta.items():
             sample[k] = self._feature(v)
 
         tf_example = self._Example(features=self._Features(feature=sample))
@@ -233,15 +262,23 @@
                     value[i] = bytes_feature.encode()
             return self._Feature(bytes_list=self._BytesList(value=value))
 
 
 class FilesSampleWriter:
     """FilesSampleWriter is a caption+video writer to files"""
 
-    def __init__(self, shard_id, output_folder, save_caption, oom_shard_count, schema, encode_formats):
+    def __init__(
+        self,
+        shard_id,
+        output_folder,
+        save_caption,
+        oom_shard_count,
+        schema,
+        encode_formats,
+    ):
         self.oom_shard_count = oom_shard_count
         shard_name = (
             shard_id
             if isinstance(shard_id, str)
             else "{shard_id:0{oom_shard_count}d}".format(  # pylint: disable=consider-using-f-string
                 shard_id=shard_id, oom_shard_count=oom_shard_count
             )
@@ -253,15 +290,16 @@
         self.save_caption = save_caption
         self.buffered_parquet_writer = BufferedParquetWriter(output_folder + "/" + shard_name + ".parquet", schema, 100)
         self.encode_formats = encode_formats
 
     def write(self, streams, key, caption, meta):
         """Write sample to disk"""
         for modality, stream in streams.items():
-            filename = f"{self.subfolder}/{key}.{self.encode_formats[modality]}"
+            ext = self.encode_formats[modality] if modality in self.encode_formats else modality
+            filename = f"{self.subfolder}/{key}.{ext}"
             with self.fs.open(filename, "wb") as f:
                 f.write(stream)
 
         if self.save_caption:
             caption = str(caption) if caption is not None else ""
             caption_filename = f"{self.subfolder}/{key}.txt"
             with self.fs.open(caption_filename, "w") as f:
@@ -281,15 +319,23 @@
     def close(self):
         self.buffered_parquet_writer.close()
 
 
 class DummySampleWriter:
     """Does not write"""
 
-    def __init__(self, shard_id, output_folder, save_caption, oom_shard_count, schema, encode_formats):
+    def __init__(
+        self,
+        shard_id,
+        output_folder,
+        save_caption,
+        oom_shard_count,
+        schema,
+        encode_formats,
+    ):
         pass
 
     def write(self, streams, key, caption, meta):
         pass
 
     def close(self):
         pass
```

### Comparing `video2dataset-1.1.0/video2dataset/dataloader/filters.py` & `video2dataset-1.2.0/video2dataset/dataloader/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """WebDataset filters"""
 from langdetect import detect_langs, DetectorFactory  # pylint: disable=unused-import
+from typing import List, Union, Dict
 
 from webdataset.autodecode import decoders  # pylint: disable=unused-import
 
 
 class LanguageFilter:
     """Filters the dataset based on the language"""
 
@@ -27,20 +28,25 @@
                 valid = False
         return valid
 
 
 class KeyFilter:
     """Filters the dataset based on the key"""
 
-    def __init__(self, video_key="mp4"):
-        self.video_key = video_key
+    def __init__(self, enforce_keys=None):
+        self.enforce_keys = enforce_keys
+        if enforce_keys is None:
+            self.enforce_keys = ["mp4", "txt"]
 
     def __call__(self, sample):
         try:
-            return self.video_key in sample and "txt" in sample
+            for key in self.enforce_keys:
+                if key not in sample:
+                    return False
+            return True
         except Exception as _:  # pylint: disable=broad-except
             return False
 
 
 class AestheticsFilter:
     """Filters the dataset based on aesthethics"""
 
@@ -72,7 +78,27 @@
             try:
                 valid = sample["json"]["punsafe"] < self.p_unsafe_threshold
             except Exception:  # pylint: disable=broad-except
                 if "punsafe" not in sample["json"]:
                     raise
                 valid = False
         return valid
+
+
+class UnusedKeyFilter:
+    """Removes keys specified keys which are not used during loading and by that speeds up sampling"""
+
+    def __init__(self, keys: Union[str, List[str], None] = None) -> None:
+        if keys is None:
+            self.unused_keys = set()
+        elif isinstance(keys, str):
+            self.unused_keys = {keys}
+        else:
+            self.unused_keys = set(keys)
+
+    def __call__(self, x: Dict) -> Dict:
+        if not self.unused_keys:
+            return x
+        for key in self.unused_keys.intersection(x.keys()):
+            del x[key]
+
+        return x
```

### Comparing `video2dataset-1.1.0/video2dataset/dataloader/transform.py` & `video2dataset-1.2.0/video2dataset/dataloader/transform.py`

 * *Files 16% similar despite different names*

```diff
@@ -67,16 +67,18 @@
             print("Video size not large enough, consider reducing size")
             print(e)
             raise e
 
         reference = [y, x]
         return reference
 
-    def _get_resize_size(self, frame, orig_h, orig_w):
+    # def _get_resize_size(self, frame, orig_h, orig_w):
+    def _get_resize_size(self, frame):
         """gets resize size"""
+        orig_h, orig_w = frame.shape[:2]
         if self.resize_size is not None:
             if isinstance(self.resize_size, int):
                 f = self.resize_size / min((orig_h, orig_w))
                 resize_size = [int(round(orig_h * f)), int(round(orig_w * f))]
             else:
                 resize_size = self.resize_size
             h, w = resize_size
@@ -106,36 +108,46 @@
 
         if self.key not in data:
             raise KeyError(f"Specified key {self.key} not in data")
 
         vidkey = self.key
         frames = data[vidkey]
 
+        if isinstance(frames, int):
+            raise TypeError(f"Frames is int: {frames}")
+
         # for videos: take height and width of first frames since the same for all frames anyways,
         # if resize size is integer, then this is used as the new size of the smaller size
-        orig_h = data[self.height_key][0].item()
-        orig_w = data[self.width_key][0].item()
+        # orig_h = data[self.height_key][0].item()
+        # orig_w = data[self.width_key][0].item()
 
-        resize_size, (h, w) = self._get_resize_size(frames[0], orig_h, orig_w)
+        # resize_size, (h, w) = self._get_resize_size(frames[0], orig_h, orig_w)
+        resize_size, (h, w) = self._get_resize_size(frames[0])
         reference = self._get_reference_frame(resize_size, h, w)
 
         for frame in frames:
 
             if resize_size is not None:
-                frame = cv2.resize(frame, tuple(reversed(resize_size)), interpolation=cv2.INTER_LANCZOS4)
+                frame = cv2.resize(
+                    frame,
+                    tuple(reversed(resize_size)),
+                    interpolation=cv2.INTER_LANCZOS4,
+                )
 
             if self.crop_size is not None:
                 x_ = reference[1] - int(round(self.crop_size[1] / 2))
                 y_ = reference[0] - int(round(self.crop_size[0] / 2))
 
-                frame = frame[int(y_) : int(y_) + self.crop_size[0], int(x_) : int(x_) + self.crop_size[1]]
+                frame = frame[
+                    int(y_) : int(y_) + self.crop_size[0],
+                    int(x_) : int(x_) + self.crop_size[1],
+                ]
 
             # TODO: maybe lets add other options for normalization
             # will need for VideoCLIP built on top of CLIP
-            frame = frame.astype(float) / 127.5 - 1.0
 
             frame = torch.from_numpy(frame)
             result.append(frame)
 
         data[vidkey] = torch.stack(result).to(torch.float16)
         return data
 
@@ -146,10 +158,23 @@
     def __init__(self, cuts_key, video_key="mp4"):
         self.cuts_key = cuts_key
         self.video_key = video_key
 
     def __call__(self, sample):
         assert self.cuts_key in sample, f'no field with key "{self.cuts_key}" in sample, but this is required.'
         assert self.video_key in sample, f'no field with key "{self.video_key}" in sample, but this is required.'
-        sample[self.video_key] = {self.video_key: sample[self.video_key], self.cuts_key: sample[self.cuts_key]}
+        sample[self.video_key] = {
+            self.video_key: sample[self.video_key],
+            self.cuts_key: sample[self.cuts_key],
+        }
         del sample[self.cuts_key]
         return sample
+
+
+class CustomTransforms:
+    def __init__(self, key_transform_dict):
+        self.key_transform_dict = key_transform_dict
+
+    def __call__(self, sample):
+        for key, transform in self.key_transform_dict.items():
+            sample[key] = transform(sample[key])
+        return sample
```

### Comparing `video2dataset-1.1.0/video2dataset/dataloader/video_decode.py` & `video2dataset-1.2.0/video2dataset/dataloader/video_decode.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Video Decoders"""
 import os
 import re
 import numpy as np
 import torch
+import torch.nn.functional as F
 import decord
 import tempfile
 from typing import Iterable
 
 from webdataset.autodecode import decoders
 
 
@@ -36,24 +37,40 @@
     def __call__(self, *args, **kwargs):
         raise NotImplementedError(f"{self.__class__.__name__} is abstract")
 
 
 class VideoDecorder(AbstractVideoDecoder):
     """Basic video decoder that uses decord"""
 
-    def __init__(self, n_frames=None, fps=None, num_threads=4, tmpdir="/scratch/", min_fps=1, max_fps=32):
+    def __init__(
+        self,
+        n_frames=None,
+        uniformly_sample=None,
+        fps=None,
+        num_threads=4,
+        tmpdir="/tmp/",
+        min_fps=1,
+        max_fps=32,
+        return_bytes=False,
+        pad_frames=False,
+    ):
         super().__init__()
         self.n_frames = n_frames
+        self.pad_frames = pad_frames
         if fps is not None and not isinstance(fps, Iterable):
             fps = [
                 fps,
             ]
+        if uniformly_sample:
+            assert fps is None, "fps not compatible with uniformly_sample..."
+        self.uniformly_sample = uniformly_sample
         self.fps = fps
         self.min_fps = min_fps
         self.max_fps = max_fps
+        self.return_bytes = return_bytes
         # for frame rate conditioning
         if self.fps == "sample":
             # this means we sample fps in every iteration
             self.fs_ids = {fr: i for i, fr in enumerate(range(self.min_fps, self.max_fps + 1))}
         elif isinstance(self.fps, list):
             self.fs_ids = {fr: i for i, fr in enumerate(self.fps)}
         else:
@@ -69,49 +86,55 @@
         elif isinstance(self.fps, list):
             infostring1 = ",".join([str(f) for f in self.fps])
         else:
             infostring1 = "native"
         info = (
             f'Decoding video clips of length {self.n_frames} with "decord".'
             + f" Subsampling clips to {infostring1} fps {infostring2}"
+            + self.pad_frames * "Padding videos that are too short"
         )
 
         print(info)
 
         self.tmpdir = tmpdir
         print(f"Setting {self.tmpdir} as temporary directory for the decoder")
 
     def get_frames(self, reader, n_frames, stride, **kwargs):  # pylint: disable=arguments-differ
-        if n_frames * stride > len(reader) - 1:
-            raise ValueError("video clip not long enough for decoding")
-
+        if n_frames * stride > len(reader):
+            if not self.pad_frames:
+                raise ValueError("video clip not long enough for decoding")
+            n_frames = len(reader)
         # sample frame start and choose scene
-        frame_start = self.prng.choice(int(len(reader)) - int(n_frames * stride), 1).item()
+        if n_frames == len(reader) or n_frames == len(reader) // stride:
+            frame_start = 0
+        else:
+            frame_start = self.prng.choice(int(len(reader)) - int(n_frames * stride), 1).item()
         # only decode the frames which are actually needed
         frames = reader.get_batch(np.arange(frame_start, frame_start + n_frames * stride, stride).tolist())
 
-        return frames, frame_start
+        # TODO: maybe its useful to inform the user which frmaes are padded
+        # can just output first_pad_index or a mask or something
+        pad_start = len(frames)
+        if self.pad_frames and frames.shape[0] < self.n_frames:
+            frames = F.pad(frames, (0, 0) * 3 + (0, self.n_frames - frames.shape[0]))
+
+        return frames, frame_start, pad_start
 
     def __call__(self, key, data, scene_list=None):  # pylint: disable=arguments-differ
         extension = re.sub(r".*[.]", "", key)
         if extension not in "mp4 ogv mjpeg avi mov h264 mpg webm wmv".split():
             return None
 
         additional_info = {}
         with tempfile.TemporaryDirectory(dir=self.tmpdir) as dirname:
             fname = os.path.join(dirname, f"file.{extension}")
             with open(fname, "wb") as stream:
                 stream.write(data)
             reader = decord.VideoReader(fname, num_threads=self.num_threads)
 
-        if self.n_frames is None:
-            n_frames = len(reader)
-        else:
-            n_frames = self.n_frames
-
         native_fps = int(np.round(reader.get_avg_fps()))
         if isinstance(self.fps, list):
             fps_choices = list(filter(lambda x: x <= native_fps, self.fps))
             if not fps_choices:
                 return None
             chosen_fps = self.prng.choice(list(fps_choices), 1).item()
 
@@ -122,28 +145,46 @@
             additional_info.update({"fps_id": 0})
             chosen_fps = self.prng.choice(np.arange(self.min_fps, max_fps + 1), 1).item()
         else:
             chosen_fps = native_fps
 
         fs_id = self.fs_ids[chosen_fps] if self.fs_ids else 0
         stride = int(np.round(native_fps / chosen_fps))
-        additional_info.update({"fps_id": torch.Tensor([fs_id] * n_frames).long()})
+        if self.n_frames is None:
+            n_frames = len(reader) // stride
+        else:
+            n_frames = self.n_frames
 
-        frames, start_frame = self.get_frames(reader, n_frames, stride, scene_list=scene_list)
+        if self.uniformly_sample:
+            additional_info.update({"fps_id": torch.Tensor([fs_id] * self.n_frames).long()})
+            t = len(reader)
+            indices = np.linspace(0, t - 1, self.n_frames)
+            indices = np.clip(indices, 0, t - 1).astype(int)
+            frames, start_frame, pad_start = reader.get_batch(indices), indices[0], len(indices)
+        else:
+            additional_info.update({"fps_id": torch.Tensor([fs_id] * n_frames).long()})
+            frames, start_frame, pad_start = self.get_frames(reader, n_frames, stride, scene_list=scene_list)
         frames = frames.float().numpy()
 
         additional_info["original_height"] = torch.full((frames.shape[0],), fill_value=frames.shape[1]).long()
         additional_info["original_width"] = torch.full((frames.shape[0],), fill_value=frames.shape[2]).long()
 
+        pad_masks = torch.zeros((frames.shape[0],))
+        pad_masks[:pad_start] = 1.0
+        additional_info["pad_masks"] = pad_masks
+
         if self.n_frames is not None and frames.shape[0] < self.n_frames:
             raise ValueError("Decoded video not long enough, skipping")
 
         # return compatible with torchvisioin API
         additional_info.update({"native_fps": chosen_fps if chosen_fps is not None else native_fps})
         additional_info.update({"start_frame": start_frame})
+
+        if self.return_bytes:
+            additional_info.update({"video_bytes": data})
         out = (list(frames), additional_info)
         return out
 
 
 class VideoDecorderWithCutDetection(VideoDecorder):
     """Video decoder that uses decord with cut detection"""
 
@@ -163,15 +204,14 @@
 
         cut_list = decoders[self.cuts_key](data[self.cuts_key])
         data = data[extension]
 
         return super().__call__(key, data, scene_list=cut_list)
 
     def get_frames(self, reader, n_frames, stride, scene_list):  # pylint: disable=arguments-differ
-
         min_len = n_frames * stride
         # filter out subclips shorther than minimal required length
         scene_list = list(filter(lambda x: x[1] - x[0] > min_len, scene_list))
         if len(scene_list) == 0:
             raise ValueError("video clips not long enough for decoding")
 
         clip_id = self.prng.choice(len(scene_list), 1).item()
```

### Comparing `video2dataset-1.1.0/video2dataset/input_sharder.py` & `video2dataset-1.2.0/video2dataset/input_sharder.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,22 +32,24 @@
         url_col,
         caption_col,
         clip_col,
         save_additional_columns,
         number_sample_per_shard,
         done_shards,
         tmp_path,
+        sampler=lambda x: x,
     ) -> None:
         self.input_format = input_format
         self.url_col = url_col
         self.caption_col = caption_col
         self.clip_col = clip_col
         self.save_additional_columns = save_additional_columns
         self.number_sample_per_shard = number_sample_per_shard
         self.done_shards = done_shards
+        self.shard_sampler = sampler
 
         fs, url_path = fsspec.core.url_to_fs(url_list)
         self.fs = fs
         self.tmp_path = tmp_path
 
         if fs.isdir(url_path):
             self.input_files = sorted(fs.glob(url_path + "/*." + input_format))
@@ -109,14 +111,18 @@
 
         number_shards = math.ceil(df.num_rows / self.number_sample_per_shard)
         shards_to_write = [
             (start_shard_id + shard_id, shard_id)
             for shard_id in range(number_shards)
             if start_shard_id + shard_id not in self.done_shards
         ]
+
+        shards_to_write = self.shard_sampler(shards_to_write)
+        number_shards = len(shards_to_write)
+
         if len(shards_to_write) == 0:
             return [], number_shards
 
         def write_shard(t):
             full_shard_id, shard_id = t
             begin_shard = shard_id * self.number_sample_per_shard
             end_shard = min(number_samples, (1 + shard_id) * self.number_sample_per_shard)
```

### Comparing `video2dataset-1.1.0/video2dataset/logger.py` & `video2dataset-1.2.0/video2dataset/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,22 @@
         self.success = 0
         self.failed_to_download = 0
         self.failed_to_subsample = 0
         self.bytes_downloaded = 0
         self.enable_wandb = enable_wandb
 
     def __call__(
-        self, count, success, failed_to_download, failed_to_subsample, bytes_downloaded, start_time, end_time
+        self,
+        count,
+        success,
+        failed_to_download,
+        failed_to_subsample,
+        bytes_downloaded,
+        start_time,
+        end_time,
     ):  # pylint: disable=arguments-differ
         self.count += count
         self.success += success
         self.failed_to_download += failed_to_download
         self.failed_to_subsample += failed_to_subsample
         self.bytes_downloaded += bytes_downloaded
         self.start_time = min(start_time, self.start_time)
@@ -112,15 +119,22 @@
             self.failed_to_subsample,
             self.bytes_downloaded,
             self.start_time,
             self.end_time,
         )
 
     def do_log(
-        self, count, success, failed_to_download, failed_to_subsample, bytes_downloaded, start_time, end_time
+        self,
+        count,
+        success,
+        failed_to_download,
+        failed_to_subsample,
+        bytes_downloaded,
+        start_time,
+        end_time,
     ):  # pylint: disable=arguments-differ
         duration = end_time - start_time
         vid_per_sec = count / duration
         bytes_per_sec = 1.0 * bytes_downloaded / duration
         success_ratio = 1.0 * success / count
         failed_to_download_ratio = 1.0 * failed_to_download / count
         failed_to_subsample_ratio = 1.0 * failed_to_subsample / count
@@ -209,15 +223,22 @@
 
 
 # https://docs.python.org/3/library/multiprocessing.html
 # logger process that reads stats files regularly, aggregates and send to wandb / print to terminal
 class LoggerProcess(multiprocessing.context.SpawnProcess):
     """Logger process that reads stats files regularly, aggregates and send to wandb / print to terminal"""
 
-    def __init__(self, output_folder, enable_wandb, wandb_project, config_parameters, log_interval=5):
+    def __init__(
+        self,
+        output_folder,
+        enable_wandb,
+        wandb_project,
+        config_parameters,
+        log_interval=5,
+    ):
         super().__init__()
         self.log_interval = log_interval
         self.enable_wandb = enable_wandb
         self.output_folder = output_folder
         self.stats_files = set()
         self.wandb_project = wandb_project
         self.done_shards = set()
@@ -227,15 +248,19 @@
 
     def run(self):
         """Run logger process"""
 
         fs, output_path = fsspec.core.url_to_fs(self.output_folder, use_listings_cache=False)
 
         if self.enable_wandb:
-            self.current_run = wandb.init(project=self.wandb_project, config=self.config_parameters, anonymous="allow")
+            self.current_run = wandb.init(
+                project=self.wandb_project,
+                config=self.config_parameters,
+                anonymous="allow",
+            )
         else:
             self.current_run = None
         self.total_speed_logger = SpeedLogger("total", enable_wandb=self.enable_wandb)
         self.status_table_logger = StatusTableLogger(enable_wandb=self.enable_wandb)
         last_check = 0
         total_status_dict = CappedCounter()
         while True:
```

### Comparing `video2dataset-1.1.0/video2dataset/output_sharder.py` & `video2dataset-1.2.0/video2dataset/output_sharder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 """Reader is module to read the url list and return shards"""
 import braceexpand
+import fsspec
 
 
 class OutputSharder:
     """
     The reader class reads a shard list and returns shards
 
     It provides an iter method
     It provides attributes:
     - shard_list: a list of shards to read
     - input_format: the format of the input dataset
     - done_shards: a set of already done shards
     - group_shards: the number of shards to group together
     """
 
-    def __init__(
-        self,
-        shard_list,
-        input_format,
-        done_shards,
-    ) -> None:
-
+    def __init__(self, shard_list, input_format, done_shards, sampler=lambda x: x) -> None:
         self.input_format = input_format
         self.done_shards = done_shards
-        self.shard_list = list(braceexpand.braceexpand(shard_list))
+        fs, url_path = fsspec.core.url_to_fs(shard_list)
+
+        if fs.isdir(url_path):
+            self.shard_list = sorted(fs.glob(url_path + "/*.tar"))
+            if "s3://" in shard_list:
+                self.shard_list = ["s3://" + s for s in self.shard_list]
+            if len(self.shard_list) == 0:
+                raise Exception(f"No file found at path {url_path} with extension {input_format}")
+        else:
+            self.shard_list = list(braceexpand.braceexpand(shard_list))
+
+        num_shards = len(self.shard_list)
+        print(f"Found a total of {num_shards} shards!")
 
         if self.input_format == "webdataset":
             self.shard_ids = [s.split("/")[-1][: -len(".tar")] for s in self.shard_list]
         elif self.input_format == "files":
             self.shard_ids = [s.split("/")[-1] for s in self.shard_list]
 
-        self.shards = [
-            (s, s_id) for s_id, s in zip(self.shard_ids, self.shard_list) if int(s_id) not in self.done_shards
-        ]
+        self.shards = sampler(
+            [(s_id, s) for s_id, s in zip(self.shard_ids, self.shard_list) if int(s_id) not in self.done_shards]
+        )
+
+        num_shards = len(self.shards)
+        print(f"Processing a total of {num_shards} shards!")
 
     def __iter__(self):
         """
         Iterate over shards, yield shards of size group_shards size
         Each shard is a tuple (shard_id, shard)
         """
-        for s, s_id in self.shards:
+        for s_id, s in self.shards:
             yield (s, s_id)
```

### Comparing `video2dataset-1.1.0/video2dataset/subsamplers/audio_rate_subsampler.py` & `video2dataset-1.2.0/video2dataset/subsamplers/audio_rate_subsampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,12 +28,12 @@
                 ext = self.encode_formats["audio"]
                 try:
                     # TODO: for now assuming m4a, change this
                     ffmpeg_args = {"ar": str(self.sample_rate), "f": ext}
                     _ = ffmpeg.input(f"{tmpdir}/input.m4a")
                     _ = _.output(f"{tmpdir}/output.{ext}", **ffmpeg_args).run(capture_stdout=True, quiet=True)
                 except Exception as err:  # pylint: disable=broad-except
-                    return [], str(err)
+                    return [], None, str(err)
 
                 with open(f"{tmpdir}/output.{ext}", "rb") as f:
                     subsampled_bytes.append(f.read())
-        return subsampled_bytes, None
+        return subsampled_bytes, None, None
```

### Comparing `video2dataset-1.1.0/video2dataset/subsamplers/cut_detection_subsampler.py` & `video2dataset-1.2.0/video2dataset/subsamplers/resolution_subsampler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,49 @@
 """
-cut detection subsampler detects cuts in a video
+resolution subsampler adjusts the resolution of the videos to some constant value
 """
-import numpy as np
-from scenedetect import AdaptiveDetector, SceneManager, open_video
 import os
+import ffmpeg
 import tempfile
 
+from .subsampler import Subsampler
 
-def get_scenes_from_scene_manager(scene_manager, cut_detection_mode):
-    """
-    Returns a list of cuts from a scene manager given a cut detection mode
-    """
-    scene_list = scene_manager.get_scene_list(start_in_scene=True)
-    scene = []
-
-    for clip in scene_list:
-        scene.append([clip[0].get_frames(), clip[1].get_frames()])
-
-    if cut_detection_mode == "longest":  # we have multiple cuts, pick the longest
-        longest_clip = np.argmax([clip[1] - clip[0] for clip in scene])
-        scene = [scene[longest_clip]]
 
-    return scene
-
-
-class CutDetectionSubsampler:
+class ResolutionSubsampler(Subsampler):
     """
-    Detects cuts in input videos and returns contiguous segments in a video as metadata.
+    Adjusts the resolution of the videos to the specified height and width.
 
-    expects:
-    - cut_detection_mode to be either "longest" to pick the longest cut or "all" to pick all cuts
-    - framerates to be None (for original fps only) or a list of target framerates to detect cuts in
+    Args:
+        video_size (int): Target resolution of the videos.
+        resize_mode (list[str]): List of resize modes to apply. Possible options are:
+            scale: scale video keeping aspect ratios (currently always picks video height)
+            crop: center crop to video_size x video_size
+            pad: center pad to video_size x video_size
     """
 
-    def __init__(self, cut_detection_mode="all", framerates=None):
-        self.framerates = framerates
-        self.cut_detection_mode = cut_detection_mode
+    def __init__(self, video_size, resize_mode):
+        self.video_size = video_size
+        self.resize_mode = resize_mode
 
-    def __call__(self, streams):
+    def __call__(self, streams, metadata=None):
         video_bytes = streams["video"]
-
-        with tempfile.TemporaryDirectory() as tmpdir:
-            video_path = os.path.join(tmpdir, "input.mp4")
-            with open(video_path, "wb") as f:
-                f.write(video_bytes)
-
-            video = open_video(video_path)
-
-            detector = AdaptiveDetector()
-            scene_manager = SceneManager()
-            scene_manager.add_detector(detector)
-
-            cuts = {}
-            original_fps = video.frame_rate
-            cuts["original_fps"] = original_fps
-
-            scene_manager.detect_scenes(video=video)
-            cuts["cuts_original_fps"] = get_scenes_from_scene_manager(scene_manager, self.cut_detection_mode)
-            if self.framerates is not None:
-                for target_fps in self.framerates:
-                    video.reset()
-
-                    scene_manager = SceneManager()
-                    detector = AdaptiveDetector()
-                    scene_manager.add_detector(detector)
-                    frame_skip = max(
-                        int(original_fps // target_fps) - 1, 0
-                    )  # if we take 1 frame and skip N frames we're sampling 1/N+1 % of the video
-                    # so if we desire to sample 1/N of the video, we need to subtract one when doing frame skipping
-
-                    scene_manager.detect_scenes(video=video, frame_skip=frame_skip)
-                    cuts[f"cuts_{target_fps}"] = get_scenes_from_scene_manager(scene_manager, self.cut_detection_mode)
-                    scene_manager.clear()
-
-        return cuts
+        subsampled_bytes = []
+        for vid_bytes in video_bytes:
+            with tempfile.TemporaryDirectory() as tmpdir:
+                with open(os.path.join(tmpdir, "input.mp4"), "wb") as f:
+                    f.write(vid_bytes)
+                try:
+                    _ = ffmpeg.input(f"{tmpdir}/input.mp4")
+                    if "scale" in self.resize_mode:
+                        _ = _.filter("scale", -2, self.video_size)
+                    if "crop" in self.resize_mode:
+                        _ = _.filter("crop", w=self.video_size, h=self.video_size)
+                    if "pad" in self.resize_mode:
+                        _ = _.filter("pad", w=self.video_size, h=self.video_size)
+                    _ = _.output(f"{tmpdir}/output.mp4", reset_timestamps=1).run(capture_stdout=True, quiet=True)
+                except Exception as err:  # pylint: disable=broad-except
+                    return [], None, str(err)
+
+                with open(f"{tmpdir}/output.mp4", "rb") as f:
+                    subsampled_bytes.append(f.read())
+        streams["video"] = subsampled_bytes
+        return streams, None, None
```

### Comparing `video2dataset-1.1.0/video2dataset/workers/download_worker.py` & `video2dataset-1.2.0/video2dataset/workers/download_worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from video2dataset.data_reader import VideoDataReader
 from video2dataset.logger import CappedCounter
 from video2dataset.logger import write_stats
 from video2dataset.subsamplers import (
     ClippingSubsampler,
     CutDetectionSubsampler,
     FrameSubsampler,
+    FFProbeSubsampler,
     NoOpSubsampler,
     ResolutionSubsampler,
     AudioRateSubsampler,
 )
 
 
 def compute_key(key, shard_id, oom_sample_per_shard, oom_shard_count):
@@ -39,63 +40,61 @@
 
     def __init__(
         self,
         sample_writer_class,
         save_caption,
         output_folder,
         column_list,
-        thread_count,
-        timeout,
-        number_sample_per_shard,
-        oom_shard_count,
-        video_size,
-        resize_mode,
-        video_fps,
-        audio_rate,
         tmp_dir,
-        yt_metadata_args,
-        captions_are_subtitles,
-        detect_cuts,
-        cut_detection_mode,
-        cuts_are_clips,
         encode_formats,
-        cut_framerates,
-        oom_clip_count=5,
+        config,
     ) -> None:
         self.sample_writer_class = sample_writer_class
         self.save_caption = save_caption
         self.output_folder = output_folder
         self.column_list = column_list
-        self.number_sample_per_shard = number_sample_per_shard
-        self.oom_shard_count = oom_shard_count
-        self.thread_count = thread_count
-        self.captions_are_subtitles = captions_are_subtitles
-
         self.encode_formats = encode_formats
+        self.config = config
+
+        self.data_reader = VideoDataReader(encode_formats, tmp_dir, config["reading"])
 
-        self.data_reader = VideoDataReader(video_size, audio_rate, timeout, tmp_dir, yt_metadata_args, encode_formats)
+        self.clipping_subsampler = ClippingSubsampler(
+            5,  # oom_clip_count
+            encode_formats,
+            **self.config["subsampling"].get("ClippingSubsampler", {"args": {}})["args"],
+        )
+        need_keyframes = self.clipping_subsampler.precision == "keyframe_adjusted"
+
+        self.ffprobe_subsampler = None
+        if "FFProbeSubsampler" in self.config["subsampling"] or need_keyframes:
+            self.ffprobe_subsampler = FFProbeSubsampler(
+                **self.config["subsampling"].get("FFProbeSubsampler", {"args": {}})["args"]
+            )
+            self.ffprobe_subsampler.extract_keyframes |= need_keyframes
+
+        self.cut_detector = None
+        self.cuts_are_clips = False
+        if "CutDetectionSubsampler" in self.config["subsampling"]:
+            if "args" in self.config["subsampling"]["CutDetectionSubsampler"]:
+                self.cut_detector = CutDetectionSubsampler(
+                    **self.config["subsampling"]["CutDetectionSubsampler"]["args"]
+                )
+            self.cuts_are_clips = self.config["subsampling"]["CutDetectionSubsampler"].get("cuts_are_clips", False)
 
-        self.clipping_subsampler = ClippingSubsampler(oom_clip_count, encode_formats)
-        self.cut_detection_mode = cut_detection_mode
-        self.cut_framerates = cut_framerates
-        self.detect_cuts = detect_cuts
-        if detect_cuts:
-            self.cut_detector = CutDetectionSubsampler(cut_detection_mode=cut_detection_mode, framerates=cut_framerates)
-        self.cuts_are_clips = cuts_are_clips
         self.noop_subsampler = NoOpSubsampler()
 
         video_subsamplers: List[Any] = []
-        if resize_mode is not None:
-            video_subsamplers.append(ResolutionSubsampler(video_size, resize_mode))
-        if video_fps > 0:
-            video_subsamplers.append(FrameSubsampler(video_fps))
+        if "ResolutionSubsampler" in self.config["subsampling"]:
+            video_subsamplers.append(ResolutionSubsampler(**self.config["subsampling"]["ResolutionSubsampler"]["args"]))
+        if "FrameSubsampler" in self.config["subsampling"]:
+            video_subsamplers.append(FrameSubsampler(**self.config["subsampling"]["FrameSubsampler"]["args"]))
 
         audio_subsamplers: List[Any] = []
-        if audio_rate > 0:
-            audio_subsamplers.append(AudioRateSubsampler(audio_rate, encode_formats))
+        if "AudioRateSubsampler" in self.config["subsampling"]:
+            video_subsamplers.append(AudioRateSubsampler(**self.config["subsampling"]["AudioRateSubsampler"]["args"]))
 
         self.subsamplers = {"video": video_subsamplers, "audio": audio_subsamplers}
 
     def __call__(
         self,
         row,
     ):
@@ -131,151 +130,165 @@
         del pydict
         del df
 
         status_dict = CappedCounter()
 
         count = len(shard_to_dl)
         successes = 0
-        failed_to_download = 0
-        failed_to_subsample = 0
+        failed = {
+            "failed_to_download": 0,
+            "failed_to_subsample": 0,
+        }
         bytes_downloaded = 0
         url_indice = self.column_list.index("url")
         caption_indice = self.column_list.index("caption") if "caption" in self.column_list else None
         key_url_list = [(key, x[url_indice]) for key, x in shard_to_dl]
 
-        semaphore = Semaphore(self.thread_count)
+        semaphore = Semaphore(self.config["distribution"]["thread_count"])
 
         def data_generator():
             for e in key_url_list:
                 semaphore.acquire()  # pylint: disable=(consider-using-with)
                 yield e
 
         loader = data_generator()
 
         # give schema to writer
         sample_writer = self.sample_writer_class(
-            shard_id, self.output_folder, self.save_caption, self.oom_shard_count, schema, self.encode_formats
+            shard_id,
+            self.output_folder,
+            self.save_caption,
+            self.config["storage"]["oom_shard_count"],
+            schema,
+            self.encode_formats,
         )
-        oom_sample_per_shard = math.ceil(math.log10(self.number_sample_per_shard))
+        oom_sample_per_shard = math.ceil(math.log10(self.config["storage"]["number_sample_per_shard"]))
 
-        with ThreadPool(self.thread_count) as thread_pool:
+        with ThreadPool(self.config["distribution"]["thread_count"]) as thread_pool:
             for key, streams, yt_meta_dict, error_message in thread_pool.imap_unordered(
                 self.data_reader,  # pylint: disable=(unnecessary-lambda)
                 loader,
             ):
                 try:
                     _, sample_data = shard_to_dl[key]
-                    str_key = compute_key(key, shard_id, oom_sample_per_shard, self.oom_shard_count)
+                    str_key = compute_key(
+                        key, shard_id, oom_sample_per_shard, self.config["storage"]["oom_shard_count"]
+                    )
                     meta = {
                         **{self.column_list[i]: sample_data[i] for i in range(len(self.column_list))},
                         "key": str_key,
                         "status": None,
                         "error_message": error_message,
                         "yt_meta_dict": yt_meta_dict,
                     }
 
                     if error_message is not None:
+                        print(error_message)
                         if "[youtube]" in error_message:  # video-specific error, remove videoID
                             error_message = "ERROR: [youtube]:" + error_message.split(":")[-1]
-                        failed_to_download += 1
-                        status = "failed_to_download"
-                        status_dict.increment(error_message)
-                        meta["status"] = status
-                        sample_writer.write(
-                            {},
-                            str_key,
-                            sample_data[caption_indice] if caption_indice is not None else None,
-                            meta,
-                        )
-                        semaphore.release()
-                        continue
+                        raise Exception("failed_to_download")
 
                     for stream in streams.values():
                         bytes_downloaded += len(stream)
+                    for mod in streams:
+                        streams[mod] = [streams[mod]]
 
-                    metas = [meta]
+                    if self.ffprobe_subsampler is not None:
+                        streams, meta, error_message = self.ffprobe_subsampler(streams, meta)
+                        if error_message is not None:
+                            raise Exception("failed_to_subsample")
 
-                    if self.captions_are_subtitles:  # create clips
+                    if self.config["storage"]["captions_are_subtitles"]:  # create clips
                         subtitles = meta["yt_meta_dict"]["subtitles"]
                         meta["clips"] = [[line_dict["start"], line_dict["end"]] for line_dict in subtitles]
-                        meta["lines"] = [" ".join(line_dict["lines"]) for line_dict in subtitles]
+                    elif self.cut_detector is not None:  # apply cut detection to get clips
+                        streams, cuts, error_message = self.cut_detector(streams)
+
+                        if error_message is not None:
+                            raise Exception("failed_to_subsample")
 
-                    elif self.detect_cuts:  # apply cut detection to get clips
-                        meta["cuts"] = self.cut_detector(streams)
+                        meta["cuts"] = cuts
 
-                        if self.cuts_are_clips:
-                            cuts = (np.array(meta["cuts"]["cuts_original_fps"]) / meta["cuts"]["original_fps"]).tolist()
-                            meta["clips"] = cuts
+                    if self.cuts_are_clips:
+                        cuts = meta["cuts"]["cuts_original_fps"]
+                        native_fps = meta["cuts"]["original_fps"]
+                        meta["clips"] = (np.array(cuts) / native_fps).tolist()
 
                     # 1 video -> many videos (either clipping or noop which does identity broadcasting)
                     broadcast_subsampler = (
                         self.clipping_subsampler
-                        if ("clips" in self.column_list or self.captions_are_subtitles)
+                        if (
+                            "clips" in self.column_list
+                            or self.config["storage"]["captions_are_subtitles"]
+                            or self.cuts_are_clips
+                        )
                         else self.noop_subsampler
                     )
                     subsampled_streams, metas, error_message = broadcast_subsampler(streams, meta)
 
                     for modality in subsampled_streams:
                         for modality_subsampler in self.subsamplers[modality]:
-                            subsampled_modality, error_message = modality_subsampler(subsampled_streams[modality])
-                            subsampled_streams[modality] = subsampled_modality
+                            subsampled_streams, metas, error_message = modality_subsampler(subsampled_streams, metas)
 
                     if error_message is not None:
-                        failed_to_subsample += 1
-                        status = "failed_to_subsample"
-                        status_dict.increment(error_message)
-                        meta["status"] = status
                         meta["clips"] = []
-                        meta["error_message"] = error_message
-                        sample_writer.write(
-                            {},
-                            str_key,
-                            sample_data[caption_indice] if caption_indice is not None else None,
-                            meta,
-                        )
-                        semaphore.release()
-                        continue
+                        raise Exception("failed_to_subsample")
 
                     successes += 1
                     status = "success"
                     status_dict.increment(status)
                     subsampled_streams_list = [
                         dict(zip(subsampled_streams, s)) for s in zip(*subsampled_streams.values())
                     ]
                     for subsampled_streams, meta in zip(subsampled_streams_list, metas):
                         meta["status"] = status
 
-                        text_caption = (sample_data[caption_indice] if caption_indice is not None else None,)
-                        if self.captions_are_subtitles:
-                            text_caption = meta["yt_meta_dict"].pop("subtitles")
+                        text_caption = sample_data[caption_indice] if caption_indice is not None else None
+                        if self.config["storage"]["captions_are_subtitles"]:
+                            text_caption = meta.get("clip_subtitles")[0]["lines"][0]
 
                         sample_writer.write(
                             subsampled_streams,
                             meta["key"],
                             text_caption,
                             meta,
                         )
                 except Exception as err:  # pylint: disable=broad-except
-                    traceback.print_exc()
-                    print(f"Sample {key} failed to download: {err}")
+                    status = str(err)
+                    if status.startswith("failed_to_"):
+                        failed[status] += 1
+                        status_dict.increment(error_message)
+                        meta["status"] = status
+                        meta["error_message"] = error_message
+                        sample_writer.write(
+                            {},
+                            str_key,
+                            sample_data[caption_indice] if caption_indice is not None else None,
+                            meta,
+                        )
+                        semaphore.release()
+                    else:
+                        traceback.print_exc()
+                        print(f"Sample {key} failed to download: {err}")
+
                 semaphore.release()
 
             sample_writer.close()
             thread_pool.terminate()
             thread_pool.join()
             del thread_pool
 
         end_time = time.time()
         write_stats(
             self.output_folder,
             shard_id,
             count,
             successes,
-            failed_to_download,
-            failed_to_subsample,
+            failed["failed_to_download"],
+            failed["failed_to_subsample"],
             bytes_downloaded,
             start_time,
             end_time,
             status_dict,
-            self.oom_shard_count,
+            self.config["storage"]["oom_shard_count"],
         )
         fs.rm(shard_path)
```

### Comparing `video2dataset-1.1.0/video2dataset.egg-info/SOURCES.txt` & `video2dataset-1.2.0/video2dataset.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,40 @@
 video2dataset/data_reader.py
 video2dataset/data_writer.py
 video2dataset/distributor.py
 video2dataset/input_sharder.py
 video2dataset/logger.py
 video2dataset/main.py
 video2dataset/output_sharder.py
+video2dataset/slurm_executor.py
 video2dataset.egg-info/PKG-INFO
 video2dataset.egg-info/SOURCES.txt
 video2dataset.egg-info/dependency_links.txt
 video2dataset.egg-info/entry_points.txt
 video2dataset.egg-info/requires.txt
 video2dataset.egg-info/top_level.txt
+video2dataset/configs/__init__.py
 video2dataset/dataloader/__init__.py
+video2dataset/dataloader/audio_decode.py
 video2dataset/dataloader/custom_wds.py
 video2dataset/dataloader/dataloader.py
 video2dataset/dataloader/filters.py
 video2dataset/dataloader/transform.py
 video2dataset/dataloader/video_decode.py
 video2dataset/subsamplers/__init__.py
 video2dataset/subsamplers/audio_rate_subsampler.py
+video2dataset/subsamplers/caption_subsampler.py
 video2dataset/subsamplers/clipping_subsampler.py
 video2dataset/subsamplers/cut_detection_subsampler.py
+video2dataset/subsamplers/ffprobe_subsampler.py
 video2dataset/subsamplers/frame_subsampler.py
 video2dataset/subsamplers/noop_subsampler.py
+video2dataset/subsamplers/optical_flow_subsampler.py
 video2dataset/subsamplers/resolution_subsampler.py
+video2dataset/subsamplers/subsampler.py
+video2dataset/subsamplers/whisper_subsampler.py
 video2dataset/workers/__init__.py
+video2dataset/workers/caption_worker.py
 video2dataset/workers/download_worker.py
-video2dataset/workers/subset_worker.py
+video2dataset/workers/optical_flow_worker.py
+video2dataset/workers/subset_worker.py
+video2dataset/workers/whisper_worker.py
```


# Comparing `tmp/gnssrefl-1.4.1.tar.gz` & `tmp/gnssrefl-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-1.4.1.tar", last modified: Fri Jul  7 10:32:58 2023, max compression
+gzip compressed data, was "gnssrefl-1.4.2.tar", last modified: Mon Jul 10 09:17:36 2023, max compression
```

## Comparing `gnssrefl-1.4.1.tar` & `gnssrefl-1.4.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:32:58.251297 gnssrefl-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 10:32:43.000000 gnssrefl-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 10:32:43.000000 gnssrefl-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-07 10:32:58.247297 gnssrefl-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-07 10:32:43.000000 gnssrefl-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:32:58.227297 gnssrefl-1.4.1/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:32:58.227297 gnssrefl-1.4.1/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/decipher_argt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/filesizes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16210 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gnssir.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gnssir_input.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33744 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gnssir_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (123)   182915 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/make_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    28009 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/nmea2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/nyquist_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/nyquist_libs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34342 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19612 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/quickLook_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16994 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/quickLook_function2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/quickPhase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/quicklib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50791 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rinex3_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/smoosh_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    60672 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/vwc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/vwc_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    32905 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/xnmeasnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:32:58.227297 gnssrefl-1.4.1/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-07 10:32:58.000000 gnssrefl-1.4.1/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-07 10:32:58.000000 gnssrefl-1.4.1/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:32:58.000000 gnssrefl-1.4.1/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-07 10:32:58.000000 gnssrefl-1.4.1/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 10:32:58.000000 gnssrefl-1.4.1/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 10:32:58.000000 gnssrefl-1.4.1/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:32:58.251297 gnssrefl-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:32:58.247297 gnssrefl-1.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:36.384845 gnssrefl-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-10 09:17:36.384845 gnssrefl-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:36.364844 gnssrefl-1.4.2/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:36.364844 gnssrefl-1.4.2/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/decipher_argt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/filesizes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16210 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gnssir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13093 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gnssir_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33744 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gnssir_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (123)   183016 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/make_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28009 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/nmea2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/nyquist_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/nyquist_libs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34342 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19612 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/quickLook_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16994 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/quickLook_function2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/quickPhase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/quicklib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50791 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rinex3_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/smoosh_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60672 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/vwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/vwc_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32905 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/xnmeasnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:36.364844 gnssrefl-1.4.2/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-10 09:17:36.000000 gnssrefl-1.4.2/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-10 09:17:36.000000 gnssrefl-1.4.2/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:17:36.000000 gnssrefl-1.4.2/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-10 09:17:36.000000 gnssrefl-1.4.2/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 09:17:36.000000 gnssrefl-1.4.2/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 09:17:36.000000 gnssrefl-1.4.2/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:17:36.384845 gnssrefl-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:17:36.384845 gnssrefl-1.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-10 09:17:20.000000 gnssrefl-1.4.2/test/test_rinex2snr.py
```

### Comparing `gnssrefl-1.4.1/LICENSE` & `gnssrefl-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/PKG-INFO` & `gnssrefl-1.4.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.4.1
+Version: 1.4.2
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.4.1** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.2** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
+July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
+While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
+using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
+I will be removing all versions (1.3.16 up to 1.4.1) from pypi that have this bug. If you were 
+using the newarcs option in the last month, you need to rerun gnssir and any 
+downstream codes (subdaily, daily_avg etc). This bug has 
+no impact on the data translation codes (rinex2snr, nmea2snr).  
+
+How do you find out which version are you running? Type <code>pip list | grep gnssrefl</code>
 
 Our documentation is available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
 
 [Youtube videos for beginners](https://www.youtube.com/channel/UCC1NW5oS7liG7C8NBK148Bg).
 
@@ -33,15 +42,15 @@
 NASA (NNX12AK21G and NNX13AF43G). <code>gnssrefl</code> was initially developed 
 as a fun post-retirement project, followed by support from NASA (80NSSC20K1731).
 
 As of August 31, 2023, we will be an independent (unfunded) software package. Please help us maintain/improve this code. 
 
 Kristine M. Larson
 
-July 2, 2023
+July 7, 2023
 
 <HR>
```

### Comparing `gnssrefl-1.4.1/gnssrefl/EGM96.py` & `gnssrefl-1.4.2/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/check_rinex_file.py` & `gnssrefl-1.4.2/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/computemp1mp2.py` & `gnssrefl-1.4.2/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/daily_avg.py` & `gnssrefl-1.4.2/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/daily_avg_cl.py` & `gnssrefl-1.4.2/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-1.4.2/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/decipher_argt.py` & `gnssrefl-1.4.2/gnssrefl/decipher_argt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/download_ioc.py` & `gnssrefl-1.4.2/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/download_noaa.py` & `gnssrefl-1.4.2/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/download_orbits.py` & `gnssrefl-1.4.2/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/download_psmsl.py` & `gnssrefl-1.4.2/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/download_rinex.py` & `gnssrefl-1.4.2/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/download_teqc.py` & `gnssrefl-1.4.2/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/download_tides.py` & `gnssrefl-1.4.2/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/download_unr.py` & `gnssrefl-1.4.2/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/download_wsv.py` & `gnssrefl-1.4.2/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/filesizes.py` & `gnssrefl-1.4.2/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/gnssir.py` & `gnssrefl-1.4.2/gnssrefl/gnssir.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/gnssir_cl.py` & `gnssrefl-1.4.2/gnssrefl/gnssir_cl.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     extension : string, optional
         extension for result file, useful for testing strategies. default is empty string
     compress : boolean, optional
         xz compress SNR files after use. default is False.
     screenstats : bool, optional
         whether to print stats to the screen or not. default is True.
     delTmax : int, optional
-        maximum satellite arc length in minutes. Set in make_json_input
+        maximum satellite arc length in minutes. found in the json
     e1 : float, optional
         use to override the minimum elevation angle.
     e2 : float, optional
         use to override the maximum elevation angle.
     mmdd : boolean, optional
         adds columns in results for month, day, hour, and minute. default is False.
     gzip : boolean, optional
@@ -169,14 +169,15 @@
     exitS = g.check_inputs(station, year, doy, snr)
 
     if exitS:
         sys.exit()
 
     lsp = guts.read_json_file(station, extension)
     # now check the overrides to the json instructions
+    print(lsp)
 
     if newarcs:
         if 'azval2' not in lsp:
             print('An azval2 variable was not found in your json. Fix your json ')
             print('and/or use gnssir_input to make a new one. Exiting')
             sys.exit()
```

### Comparing `gnssrefl-1.4.1/gnssrefl/gnssir_input.py` & `gnssrefl-1.4.2/gnssrefl/gnssir_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,28 @@
     parser.add_argument("-e2", default=None, type=float, help="Upper limit elevation angle (deg), default 25")
     parser.add_argument("-h1", default=None, type=float, help="Lower limit reflector height (m), default 0.5")
     parser.add_argument("-h2", default=None, type=float, help="Upper limit reflector height (m), default 8")
     parser.add_argument("-nr1",default=None, type=float, help="Lower limit RH used for noise region in QC(m)")
     parser.add_argument("-nr2",default=None, type=float, help="Upper limit RH used for noise region in QC(m)")
     parser.add_argument("-peak2noise", default=None, type=float, help="peak to noise ratio used for QC")
     parser.add_argument("-ampl", default=None, type=float, help="Required spectral peak amplitude for QC")
-    parser.add_argument("-allfreq", default=None, type=str, help="Set to True to include all GNSS")
+    parser.add_argument("-allfreq", default=None, type=str, help="Include all GNSS")
     parser.add_argument("-l1", default=None, type=str, help="Only use GPS L1")
     parser.add_argument("-l2c", default=None, type=str, help="Only use GPS L2C")
     parser.add_argument("-xyz", default=None, type=str, help="True if using Cartesian coordinates")
     parser.add_argument("-refraction", default=None, type=str, help="Set to False to turn off refraction correction")
     parser.add_argument("-extension", type=str, help="Provide extension name so you can try different strategies")
     parser.add_argument("-ediff", default=None, type=str, help="Allowed min/max elevation diff from obs min/max elev angle (degrees) default is 2")
     parser.add_argument("-delTmax", default=None, type=float, help="max arc length (min) default is 75. Shorten for tides.")
-    parser.add_argument('-frlist', nargs="*",type=int,  help="User defined frequencies using our nomenclature.")
-    parser.add_argument('-azlist2', nargs="*",type=float,  help="list of azimuth regions, default 0-360") 
-    parser.add_argument('-ellist', nargs="*",type=float,  help="List of elevation angles to allow more complex analysis scenarios-advanced users only!") 
+    parser.add_argument("-frlist", nargs="*",type=int,  help="User defined frequencies using our nomenclature.")
+    parser.add_argument("-azlist2", nargs="*",type=float,  default=None,help="list of azimuth regions, default 0-360") 
+    parser.add_argument("-ellist", nargs="*",type=float,  default=None,help="List of elevation angles to allow more complex analysis scenarios-advanced users only!") 
+
+    #print(parser.parse_args())
+
 
 
     args = parser.parse_args().__dict__
 
     # convert all expected boolean inputs from strings to booleans
     boolean_args = ['allfreq', 'l1', 'l2c', 'xyz', 'refraction']
     args = str2bool(args, boolean_args)
@@ -309,12 +312,13 @@
     print('writing out to:', outputfile)
     with open(outputfile, 'w+') as outfile:
         json.dump(lsp, outfile, indent=4)
 
 
 def main():
     args = parse_arguments()
+    print(args)
     make_gnssir_input(**args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gnssrefl-1.4.1/gnssrefl/gnssir_v2.py` & `gnssrefl-1.4.2/gnssrefl/gnssir_v2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/gnsssnr.f` & `gnssrefl-1.4.2/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/gnsssnrbigger.f` & `gnssrefl-1.4.2/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/gps.py` & `gnssrefl-1.4.2/gnssrefl/gps.py`

 * *Files 0% similar despite different names*

```diff
@@ -5222,14 +5222,18 @@
     lat = 0; lon = 0; ht = 0
     if len(station) != 4:
         print('The station name must be four characters long')
         return lat, lon, ht
 
     not_in_database = False
     xdir = os.environ['REFL_CODE']
+    fdir = xdir + '/Files'
+    if not os.path.isdir(fdir):
+        subprocess.call(['mkdir', fdir])
+
     nfile1 = 'gnssrefl/station_pos.db'
     nfile1_exist = os.path.isfile(nfile1)
     nfile2 = xdir + '/Files/station_pos.db'
     nfile2_exist = os.path.isfile(nfile2)
 
     if (nfile1_exist) or (nfile2_exist):
         iii = 0
```

### Comparing `gnssrefl-1.4.1/gnssrefl/gpssnr.f` & `gnssrefl-1.4.2/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/gpsweek.py` & `gnssrefl-1.4.2/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/gpt_1wA.pickle` & `gnssrefl-1.4.2/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/highrate.py` & `gnssrefl-1.4.2/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/installexe_cl.py` & `gnssrefl-1.4.2/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/invsnr_cl.py` & `gnssrefl-1.4.2/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/invsnr_input.py` & `gnssrefl-1.4.2/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/karnak_libraries.py` & `gnssrefl-1.4.2/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/kelly.py` & `gnssrefl-1.4.2/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/llh2xyz.py` & `gnssrefl-1.4.2/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/make_json_input.py` & `gnssrefl-1.4.2/gnssrefl/make_json_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/nmea2snr.py` & `gnssrefl-1.4.2/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/nmea2snr_cl.py` & `gnssrefl-1.4.2/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/nyquist_cl.py` & `gnssrefl-1.4.2/gnssrefl/nyquist_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/nyquist_libs.py` & `gnssrefl-1.4.2/gnssrefl/nyquist_libs.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/phase_functions.py` & `gnssrefl-1.4.2/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/prn2gps.py` & `gnssrefl-1.4.2/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/query_unr.py` & `gnssrefl-1.4.2/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/quickLook_cl.py` & `gnssrefl-1.4.2/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/quickLook_function.py` & `gnssrefl-1.4.2/gnssrefl/quickLook_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/quickLook_function2.py` & `gnssrefl-1.4.2/gnssrefl/quickLook_function2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/quickPhase.py` & `gnssrefl-1.4.2/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/quicklib.py` & `gnssrefl-1.4.2/gnssrefl/quicklib.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/quickplt.py` & `gnssrefl-1.4.2/gnssrefl/quickplt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/read_snr_files.py` & `gnssrefl-1.4.2/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/refl_zones.py` & `gnssrefl-1.4.2/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/refl_zones_cl.py` & `gnssrefl-1.4.2/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/refraction.py` & `gnssrefl-1.4.2/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/rh_plot.py` & `gnssrefl-1.4.2/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/rinex2snr.py` & `gnssrefl-1.4.2/gnssrefl/rinex2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/rinex2snr_cl.py` & `gnssrefl-1.4.2/gnssrefl/rinex2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/rinex3_rinex2.py` & `gnssrefl-1.4.2/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/rinex3_snr.py` & `gnssrefl-1.4.2/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/rinpy.py` & `gnssrefl-1.4.2/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-1.4.2/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/smoosh.py` & `gnssrefl-1.4.2/gnssrefl/smoosh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/smoosh_snr.py` & `gnssrefl-1.4.2/gnssrefl/smoosh_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/snow_functions.py` & `gnssrefl-1.4.2/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/snowdepth_cl.py` & `gnssrefl-1.4.2/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/spline_functions.py` & `gnssrefl-1.4.2/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/subdaily.py` & `gnssrefl-1.4.2/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/subdaily_cl.py` & `gnssrefl-1.4.2/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/utils.py` & `gnssrefl-1.4.2/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/veg_multiyr.py` & `gnssrefl-1.4.2/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/vwc.py` & `gnssrefl-1.4.2/gnssrefl/vwc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/vwc_cl.py` & `gnssrefl-1.4.2/gnssrefl/vwc_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/vwc_input.py` & `gnssrefl-1.4.2/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/xnmeasnr.f` & `gnssrefl-1.4.2/gnssrefl/xnmeasnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/xyz2llh.py` & `gnssrefl-1.4.2/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/ydoy.py` & `gnssrefl-1.4.2/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl/ymd.py` & `gnssrefl-1.4.2/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-1.4.2/gnssrefl.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.4.1
+Version: 1.4.2
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.4.1** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.2** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
+July 7, 2023: The newarcs option had a bug in it: the refraction correction was not being applied.
+While the refraction correction is not very important for some applications (snow, soil moisture), using it sometimes and not
+using it other times IS NOT GOOD.  You will see a bias in time series when you switched. This bug is fixed as of version 1.4.1
+I will be removing all versions (1.3.16 up to 1.4.1) from pypi that have this bug. If you were 
+using the newarcs option in the last month, you need to rerun gnssir and any 
+downstream codes (subdaily, daily_avg etc). This bug has 
+no impact on the data translation codes (rinex2snr, nmea2snr).  
+
+How do you find out which version are you running? Type <code>pip list | grep gnssrefl</code>
 
 Our documentation is available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
 
 [Youtube videos for beginners](https://www.youtube.com/channel/UCC1NW5oS7liG7C8NBK148Bg).
 
@@ -33,15 +42,15 @@
 NASA (NNX12AK21G and NNX13AF43G). <code>gnssrefl</code> was initially developed 
 as a fun post-retirement project, followed by support from NASA (80NSSC20K1731).
 
 As of August 31, 2023, we will be an independent (unfunded) software package. Please help us maintain/improve this code. 
 
 Kristine M. Larson
 
-July 2, 2023
+July 7, 2023
 
 <HR>
```

### Comparing `gnssrefl-1.4.1/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-1.4.2/gnssrefl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-1.4.2/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/pyproject.toml` & `gnssrefl-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.4.1/setup.py` & `gnssrefl-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["numpy","wget","scipy","matplotlib","requests","progress","astropy","simplekml","earthscope-sdk"]
 setup(
     name="gnssrefl",
-    version="1.4.1",
+    version="1.4.2",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-1.4.1/test/test_gps.py` & `gnssrefl-1.4.2/test/test_gps.py`

 * *Files identical despite different names*


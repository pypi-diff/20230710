# Comparing `tmp/ScopeSim-0.5.6.tar.gz` & `tmp/ScopeSim-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScopeSim-0.5.6.tar", last modified: Mon Mar 13 15:33:43 2023, max compression
+gzip compressed data, was "ScopeSim-0.6.0.tar", last modified: Mon Jul 10 14:44:14 2023, max compression
```

## Comparing `ScopeSim-0.5.6.tar` & `ScopeSim-0.6.0.tar`

### file list

```diff
@@ -1,224 +1,228 @@
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.753482 ScopeSim-0.5.6/
--rw-r--r--   0 hugo      (1000) users      (998)      393 2020-11-02 12:28:44.000000 ScopeSim-0.5.6/LICENCE
--rw-r--r--   0 hugo      (1000) users      (998)      330 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/MANIFEST.in
--rw-r--r--   0 hugo      (1000) users      (998)     3403 2023-03-13 15:33:43.753482 ScopeSim-0.5.6/PKG-INFO
--rw-r--r--   0 hugo      (1000) users      (998)     2826 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/README.md
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.645481 ScopeSim-0.5.6/ScopeSim.egg-info/
--rw-r--r--   0 hugo      (1000) users      (998)     3403 2023-03-13 15:33:43.000000 ScopeSim-0.5.6/ScopeSim.egg-info/PKG-INFO
--rw-r--r--   0 hugo      (1000) users      (998)     7124 2023-03-13 15:33:43.000000 ScopeSim-0.5.6/ScopeSim.egg-info/SOURCES.txt
--rw-r--r--   0 hugo      (1000) users      (998)        1 2023-03-13 15:33:43.000000 ScopeSim-0.5.6/ScopeSim.egg-info/dependency_links.txt
--rw-r--r--   0 hugo      (1000) users      (998)      165 2023-03-13 15:33:43.000000 ScopeSim-0.5.6/ScopeSim.egg-info/requires.txt
--rw-r--r--   0 hugo      (1000) users      (998)       14 2023-03-13 15:33:43.000000 ScopeSim-0.5.6/ScopeSim.egg-info/top_level.txt
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.633482 ScopeSim-0.5.6/docs/
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.649482 ScopeSim-0.5.6/docs/source/
--rw-r--r--   0 hugo      (1000) users      (998)        0 2020-11-02 12:28:44.000000 ScopeSim-0.5.6/docs/source/__init__.py
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.649482 ScopeSim-0.5.6/docs/source/_ext/
--rw-r--r--   0 hugo      (1000) users      (998)        0 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/docs/source/_ext/__init__.py
--rw-r--r--   0 hugo      (1000) users      (998)     1244 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/docs/source/_ext/scopesim_sphinx_ext.py
--rw-r--r--   0 hugo      (1000) users      (998)       72 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/docs/source/_ext/test_scopesim_sphinx_ext.py
--rw-r--r--   0 hugo      (1000) users      (998)     7970 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/docs/source/conf.py
--rw-r--r--   0 hugo      (1000) users      (998)     5180 2023-03-10 18:54:26.000000 ScopeSim-0.5.6/docs/source/getting_started.py
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.653482 ScopeSim-0.5.6/scopesim/
--rw-r--r--   0 hugo      (1000) users      (998)     3337 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/__init__.py
--rw-r--r--   0 hugo      (1000) users      (998)     2635 2020-11-02 12:28:44.000000 ScopeSim-0.5.6/scopesim/base_classes.py
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.657482 ScopeSim-0.5.6/scopesim/commands/
--rw-r--r--   0 hugo      (1000) users      (998)       40 2020-11-02 12:28:44.000000 ScopeSim-0.5.6/scopesim/commands/__init__.py
--rw-r--r--   0 hugo      (1000) users      (998)    13462 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/commands/user_commands.py
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.637482 ScopeSim-0.5.6/scopesim/data/
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.637482 ScopeSim-0.5.6/scopesim/data/svo/
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.657482 ScopeSim-0.5.6/scopesim/data/svo/2MASS/
--rw-r--r--   0 hugo      (1000) users      (998)    11859 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/2MASS/2MASS.H
--rw-r--r--   0 hugo      (1000) users      (998)    16464 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/2MASS/2MASS.J
--rw-r--r--   0 hugo      (1000) users      (998)    13556 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/2MASS/2MASS.Ks
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.693482 ScopeSim-0.5.6/scopesim/data/svo/GTC/
--rw-r--r--   0 hugo      (1000) users      (998)    71472 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS
--rw-r--r--   0 hugo      (1000) users      (998)    13131 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F643
--rw-r--r--   0 hugo      (1000) users      (998)    12702 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F643_filter
--rw-r--r--   0 hugo      (1000) users      (998)    11853 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F648
--rw-r--r--   0 hugo      (1000) users      (998)    11482 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F648_filter
--rw-r--r--   0 hugo      (1000) users      (998)    15666 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F657
--rw-r--r--   0 hugo      (1000) users      (998)    15055 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F657_filter
--rw-r--r--   0 hugo      (1000) users      (998)    11944 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F666
--rw-r--r--   0 hugo      (1000) users      (998)    11576 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F666_filter
--rw-r--r--   0 hugo      (1000) users      (998)    12648 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F680
--rw-r--r--   0 hugo      (1000) users      (998)    12233 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F680_filter
--rw-r--r--   0 hugo      (1000) users      (998)    13110 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F694
--rw-r--r--   0 hugo      (1000) users      (998)    12702 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F694_filter
--rw-r--r--   0 hugo      (1000) users      (998)    13189 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F709
--rw-r--r--   0 hugo      (1000) users      (998)    12795 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F709_filter
--rw-r--r--   0 hugo      (1000) users      (998)    12973 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F723
--rw-r--r--   0 hugo      (1000) users      (998)    12621 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F723_filter
--rw-r--r--   0 hugo      (1000) users      (998)    12980 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F738
--rw-r--r--   0 hugo      (1000) users      (998)    12608 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F738_filter
--rw-r--r--   0 hugo      (1000) users      (998)    13449 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F754
--rw-r--r--   0 hugo      (1000) users      (998)    13067 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F754_filter
--rw-r--r--   0 hugo      (1000) users      (998)    15422 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F770
--rw-r--r--   0 hugo      (1000) users      (998)    14863 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F770_filter
--rw-r--r--   0 hugo      (1000) users      (998)    16672 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F785
--rw-r--r--   0 hugo      (1000) users      (998)    15992 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F785_filter
--rw-r--r--   0 hugo      (1000) users      (998)    16103 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F802
--rw-r--r--   0 hugo      (1000) users      (998)    15429 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F802_filter
--rw-r--r--   0 hugo      (1000) users      (998)    17153 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F819
--rw-r--r--   0 hugo      (1000) users      (998)    16369 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F819_filter
--rw-r--r--   0 hugo      (1000) users      (998)    14863 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F838
--rw-r--r--   0 hugo      (1000) users      (998)    14207 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F838_filter
--rw-r--r--   0 hugo      (1000) users      (998)    14996 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F858
--rw-r--r--   0 hugo      (1000) users      (998)    14311 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F858_filter
--rw-r--r--   0 hugo      (1000) users      (998)    15495 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F878
--rw-r--r--   0 hugo      (1000) users      (998)    14782 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F878_filter
--rw-r--r--   0 hugo      (1000) users      (998)    14587 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F893
--rw-r--r--   0 hugo      (1000) users      (998)    13934 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F893_filter
--rw-r--r--   0 hugo      (1000) users      (998)    13465 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F902
--rw-r--r--   0 hugo      (1000) users      (998)    12902 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F902_filter
--rw-r--r--   0 hugo      (1000) users      (998)    13871 2023-03-13 15:33:22.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F911
--rw-r--r--   0 hugo      (1000) users      (998)    13278 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F911_filter
--rw-r--r--   0 hugo      (1000) users      (998)    13056 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F919
--rw-r--r--   0 hugo      (1000) users      (998)    12515 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F919_filter
--rw-r--r--   0 hugo      (1000) users      (998)    12853 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F924
--rw-r--r--   0 hugo      (1000) users      (998)    12328 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F924_filter
--rw-r--r--   0 hugo      (1000) users      (998)    12852 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F927
--rw-r--r--   0 hugo      (1000) users      (998)    12339 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F927_filter
--rw-r--r--   0 hugo      (1000) users      (998)    12756 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F932
--rw-r--r--   0 hugo      (1000) users      (998)    12244 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F932_filter
--rw-r--r--   0 hugo      (1000) users      (998)    12758 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F936
--rw-r--r--   0 hugo      (1000) users      (998)    12244 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F936_filter
--rw-r--r--   0 hugo      (1000) users      (998)    12764 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F940
--rw-r--r--   0 hugo      (1000) users      (998)    12234 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F940_filter
--rw-r--r--   0 hugo      (1000) users      (998)    25885 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.sdss_g_filter
--rw-r--r--   0 hugo      (1000) users      (998)    26728 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.sdss_i_filter
--rw-r--r--   0 hugo      (1000) users      (998)    27457 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.sdss_r_filter
--rw-r--r--   0 hugo      (1000) users      (998)    33965 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.sdss_z_filter
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.693482 ScopeSim-0.5.6/scopesim/data/svo/Gemini/
--rw-r--r--   0 hugo      (1000) users      (998)    95207 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/Gemini/NIRI.Lprime-G0207w
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.693482 ScopeSim-0.5.6/scopesim/data/svo/Generic/
--rw-r--r--   0 hugo      (1000) users      (998)     8344 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/Generic/Bessell.V
--rw-r--r--   0 hugo      (1000) users      (998)     8631 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/Generic/Johnson.I
--rw-r--r--   0 hugo      (1000) users      (998)     9112 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/Generic/Johnson.J
--rw-r--r--   0 hugo      (1000) users      (998)     9240 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/Generic/Johnson_UBVRIJHKL.N
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.693482 ScopeSim-0.5.6/scopesim/data/svo/HST/
--rw-r--r--   0 hugo      (1000) users      (998)    58531 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/HST/WFC3_IR.F160W
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.705482 ScopeSim-0.5.6/scopesim/data/svo/JWST/
--rw-r--r--   0 hugo      (1000) users      (998)    20594 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI
--rw-r--r--   0 hugo      (1000) users      (998)    48045 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1000W
--rw-r--r--   0 hugo      (1000) users      (998)    25066 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1065C
--rw-r--r--   0 hugo      (1000) users      (998)    36354 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1130W
--rw-r--r--   0 hugo      (1000) users      (998)    25357 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1140C
--rw-r--r--   0 hugo      (1000) users      (998)    59537 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1280W
--rw-r--r--   0 hugo      (1000) users      (998)    77628 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1500W
--rw-r--r--   0 hugo      (1000) users      (998)    25578 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1550C
--rw-r--r--   0 hugo      (1000) users      (998)    96583 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1800W
--rw-r--r--   0 hugo      (1000) users      (998)   133082 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F2100W
--rw-r--r--   0 hugo      (1000) users      (998)    25578 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F2300C
--rw-r--r--   0 hugo      (1000) users      (998)   135422 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F2550W
--rw-r--r--   0 hugo      (1000) users      (998)    35473 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F560W
--rw-r--r--   0 hugo      (1000) users      (998)    52930 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F770W
--rw-r--r--   0 hugo      (1000) users      (998)    13045 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/JWST/NIRCam.F164N
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.705482 ScopeSim-0.5.6/scopesim/data/svo/None/
--rw-r--r--   0 hugo      (1000) users      (998)      272 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/None/None.None
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.705482 ScopeSim-0.5.6/scopesim/data/svo/Paranal/
--rw-r--r--   0 hugo      (1000) users      (998)    33154 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/Paranal/HAWKI.BrGamma
--rw-r--r--   0 hugo      (1000) users      (998)    24618 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/Paranal/HAWKI.H
--rw-r--r--   0 hugo      (1000) users      (998)    16731 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/Paranal/HAWKI.J
--rw-r--r--   0 hugo      (1000) users      (998)    28804 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/Paranal/HAWKI.Ks
--rw-r--r--   0 hugo      (1000) users      (998)     9107 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/Paranal/NACO.Ks
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.709482 ScopeSim-0.5.6/scopesim/data/svo/SLOAN/
--rw-r--r--   0 hugo      (1000) users      (998)   181368 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/SLOAN/SDSS.rprime_filter
--rw-r--r--   0 hugo      (1000) users      (998)    19736 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/SLOAN/SDSS.z
--rw-r--r--   0 hugo      (1000) users      (998)   501297 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/data/svo/SLOAN/SDSS.zprime_filter
--rw-r--r--   0 hugo      (1000) users      (998)     2256 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/defaults.yaml
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.709482 ScopeSim-0.5.6/scopesim/detector/
--rw-r--r--   0 hugo      (1000) users      (998)       72 2020-11-02 12:28:44.000000 ScopeSim-0.5.6/scopesim/detector/__init__.py
--rw-r--r--   0 hugo      (1000) users      (998)     1443 2022-03-23 13:25:17.000000 ScopeSim-0.5.6/scopesim/detector/detector.py
--rw-r--r--   0 hugo      (1000) users      (998)     4246 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/detector/detector_array.py
--rw-r--r--   0 hugo      (1000) users      (998)    20469 2020-11-02 12:28:44.000000 ScopeSim-0.5.6/scopesim/detector/nghxrg.py
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.725482 ScopeSim-0.5.6/scopesim/effects/
--rw-r--r--   0 hugo      (1000) users      (998)      448 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/effects/__init__.py
--rw-r--r--   0 hugo      (1000) users      (998)    20315 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/effects/apertures.py
--rw-r--r--   0 hugo      (1000) users      (998)     5919 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/effects/data_container.py
--rw-r--r--   0 hugo      (1000) users      (998)    11652 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/effects/detector_list.py
--rw-r--r--   0 hugo      (1000) users      (998)    10785 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/effects/effects.py
--rw-r--r--   0 hugo      (1000) users      (998)     3908 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/effects/effects_utils.py
--rw-r--r--   0 hugo      (1000) users      (998)    21263 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/effects/electronic.py
--rw-r--r--   0 hugo      (1000) users      (998)    21776 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/effects/fits_headers.py
--rw-r--r--   0 hugo      (1000) users      (998)    18629 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/effects/metis_lms_trace_list.py
--rw-r--r--   0 hugo      (1000) users      (998)     3181 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/effects/obs_strategies.py
--rw-r--r--   0 hugo      (1000) users      (998)     9531 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/effects/psf_utils.py
--rw-r--r--   0 hugo      (1000) users      (998)    30998 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/effects/psfs.py
--rw-r--r--   0 hugo      (1000) users      (998)      951 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/effects/rotation.py
--rw-r--r--   0 hugo      (1000) users      (998)    12926 2022-03-23 13:25:17.000000 ScopeSim-0.5.6/scopesim/effects/shifts.py
--rw-r--r--   0 hugo      (1000) users      (998)    13701 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/effects/spectral_trace_list.py
--rw-r--r--   0 hugo      (1000) users      (998)    32717 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/effects/spectral_trace_list_utils.py
--rw-r--r--   0 hugo      (1000) users      (998)     6338 2021-04-19 10:58:26.000000 ScopeSim-0.5.6/scopesim/effects/surface_list.py
--rw-r--r--   0 hugo      (1000) users      (998)     7614 2022-03-23 13:25:17.000000 ScopeSim-0.5.6/scopesim/effects/surface_list_OLD.py
--rw-r--r--   0 hugo      (1000) users      (998)    31437 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/effects/ter_curves.py
--rw-r--r--   0 hugo      (1000) users      (998)    13457 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/effects/ter_curves_utils.py
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.733482 ScopeSim-0.5.6/scopesim/optics/
--rw-r--r--   0 hugo      (1000) users      (998)     9457 2022-03-23 13:25:17.000000 ScopeSim-0.5.6/scopesim/optics/OLD_fov.py
--rw-r--r--   0 hugo      (1000) users      (998)     4440 2022-03-23 13:25:17.000000 ScopeSim-0.5.6/scopesim/optics/OLD_fov_manager.py
--rw-r--r--   0 hugo      (1000) users      (998)      425 2020-11-02 12:28:44.000000 ScopeSim-0.5.6/scopesim/optics/__init__.py
--rw-r--r--   0 hugo      (1000) users      (998)    26313 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/optics/fov.py
--rw-r--r--   0 hugo      (1000) users      (998)    14727 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/optics/fov_manager.py
--rw-r--r--   0 hugo      (1000) users      (998)    14508 2021-04-19 10:58:26.000000 ScopeSim-0.5.6/scopesim/optics/fov_manager_utils.py
--rw-r--r--   0 hugo      (1000) users      (998)    15466 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/optics/fov_utils.py
--rw-r--r--   0 hugo      (1000) users      (998)     4592 2022-03-23 13:25:17.000000 ScopeSim-0.5.6/scopesim/optics/image_plane.py
--rw-r--r--   0 hugo      (1000) users      (998)    26272 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/optics/image_plane_utils.py
--rw-r--r--   0 hugo      (1000) users      (998)     2808 2020-11-02 12:28:44.000000 ScopeSim-0.5.6/scopesim/optics/monochromatic_trace_curve.py
--rw-r--r--   0 hugo      (1000) users      (998)     8764 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/optics/optical_element.py
--rw-r--r--   0 hugo      (1000) users      (998)    19449 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/optics/optical_train.py
--rw-r--r--   0 hugo      (1000) users      (998)    11579 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/optics/optics_manager.py
--rw-r--r--   0 hugo      (1000) users      (998)     3001 2020-11-02 12:28:44.000000 ScopeSim-0.5.6/scopesim/optics/radiometry.py
--rw-r--r--   0 hugo      (1000) users      (998)     5262 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/optics/radiometry_utils.py
--rw-r--r--   0 hugo      (1000) users      (998)        0 2020-11-02 12:28:44.000000 ScopeSim-0.5.6/scopesim/optics/spectrograph.py
--rw-r--r--   0 hugo      (1000) users      (998)     9714 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/optics/surface.py
--rw-r--r--   0 hugo      (1000) users      (998)     4021 2022-03-23 13:25:17.000000 ScopeSim-0.5.6/scopesim/optics/surface_utils.py
--rw-r--r--   0 hugo      (1000) users      (998)      775 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/rc.py
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.737482 ScopeSim-0.5.6/scopesim/reports/
--rw-r--r--   0 hugo      (1000) users      (998)        0 2020-11-02 12:28:44.000000 ScopeSim-0.5.6/scopesim/reports/__init__.py
--rw-r--r--   0 hugo      (1000) users      (998)      550 2022-03-23 13:25:17.000000 ScopeSim-0.5.6/scopesim/reports/report_generator.py
--rw-r--r--   0 hugo      (1000) users      (998)    10668 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/reports/rst_utils.py
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.737482 ScopeSim-0.5.6/scopesim/server/
--rw-r--r--   0 hugo      (1000) users      (998)     4932 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/server/OLD_database.py
--rw-r--r--   0 hugo      (1000) users      (998)      168 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/server/__init__.py
--rw-r--r--   0 hugo      (1000) users      (998)    15352 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/server/database.py
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.741482 ScopeSim-0.5.6/scopesim/source/
--rw-r--r--   0 hugo      (1000) users      (998)       60 2022-03-23 13:25:17.000000 ScopeSim-0.5.6/scopesim/source/__init__.py
--rw-r--r--   0 hugo      (1000) users      (998)    23705 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/source/source.py
--rw-r--r--   0 hugo      (1000) users      (998)     8894 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/source/source_templates.py
--rw-r--r--   0 hugo      (1000) users      (998)     7937 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/source/source_utils.py
--rw-r--r--   0 hugo      (1000) users      (998)     3689 2022-03-23 13:25:17.000000 ScopeSim-0.5.6/scopesim/system_dict.py
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.637482 ScopeSim-0.5.6/scopesim/tests/
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.741482 ScopeSim-0.5.6/scopesim/tests/mocks/
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.749482 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/
--rw-r--r--   0 hugo      (1000) users      (998)    63184 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/ATMO_default_NIR_IMG.dat
--rw-r--r--   0 hugo      (1000) users      (998)      255 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/FITS_extra_keywords.yaml
--rw-r--r--   0 hugo      (1000) users      (998)      341 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/INS_common_optics.dat
--rw-r--r--   0 hugo      (1000) users      (998)      390 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/INS_ifu_apertures.dat
--rw-r--r--   0 hugo      (1000) users      (998)   109440 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/INS_ifu_traces.fits
--rw-r--r--   0 hugo      (1000) users      (998)    69120 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/INS_lss_traces.fits
--rw-r--r--   0 hugo      (1000) users      (998)       75 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/INS_unity_refl.dat
--rw-r--r--   0 hugo      (1000) users      (998)       77 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/INS_unity_trans.dat
--rw-r--r--   0 hugo      (1000) users      (998)      613 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/YAML_atmosphere.yaml
--rw-r--r--   0 hugo      (1000) users      (998)     1414 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/YAML_basic_instrument.yaml
--rw-r--r--   0 hugo      (1000) users      (998)     2165 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/YAML_detector.yaml
--rw-r--r--   0 hugo      (1000) users      (998)      517 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/YAML_mode_ifu.yaml
--rw-r--r--   0 hugo      (1000) users      (998)      528 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/YAML_mode_spectroscopy.yaml
--rw-r--r--   0 hugo      (1000) users      (998)      561 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/YAML_telescope.yaml
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.749482 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/code/
--rw-r--r--   0 hugo      (1000) users      (998)     4077 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/code/make_spectral_trace.py
--rw-r--r--   0 hugo      (1000) users      (998)     1381 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/default.yaml
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.753482 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/filters/
--rw-r--r--   0 hugo      (1000) users      (998)     6330 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/filters/TC_filter_BrGamma.dat
--rw-r--r--   0 hugo      (1000) users      (998)    18524 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/filters/TC_filter_CH4.dat
--rw-r--r--   0 hugo      (1000) users      (998)     4406 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/filters/TC_filter_H.dat
--rw-r--r--   0 hugo      (1000) users      (998)     2663 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/filters/TC_filter_J.dat
--rw-r--r--   0 hugo      (1000) users      (998)     5331 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/filters/TC_filter_Ks.dat
--rw-r--r--   0 hugo      (1000) users      (998)       77 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/filters/TC_filter_open.dat
-drwxr-xr-x   0 hugo      (1000) users      (998)        0 2023-03-13 15:33:43.753482 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/slits/
--rw-r--r--   0 hugo      (1000) users      (998)      158 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/slits/SLIT_narrow.dat
--rw-r--r--   0 hugo      (1000) users      (998)      142 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/slits/SLIT_wide.dat
--rw-r--r--   0 hugo      (1000) users      (998)     1318 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/scopesim/tests/mocks/load_basic_instrument.py
--rw-r--r--   0 hugo      (1000) users      (998)    28940 2023-03-10 20:29:22.000000 ScopeSim-0.5.6/scopesim/utils.py
--rw-r--r--   0 hugo      (1000) users      (998)   276480 2020-11-02 12:28:44.000000 ScopeSim-0.5.6/scopesim/vega.fits
--rw-r--r--   0 hugo      (1000) users      (998)     4355 2023-03-13 15:33:23.000000 ScopeSim-0.5.6/scopesim/version.py
--rw-r--r--   0 hugo      (1000) users      (998)       38 2023-03-13 15:33:43.753482 ScopeSim-0.5.6/setup.cfg
--rw-r--r--   0 hugo      (1000) users      (998)     2500 2023-03-08 18:06:27.000000 ScopeSim-0.5.6/setup.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.476015 ScopeSim-0.6.0/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    35149 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/LICENSE
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      330 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/MANIFEST.in
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     2279 2023-07-10 14:44:14.476015 ScopeSim-0.6.0/PKG-INFO
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1299 2023-07-10 14:00:47.000000 ScopeSim-0.6.0/README.md
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.452014 ScopeSim-0.6.0/ScopeSim.egg-info/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     2279 2023-07-10 14:44:14.000000 ScopeSim-0.6.0/ScopeSim.egg-info/PKG-INFO
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     7260 2023-07-10 14:44:14.000000 ScopeSim-0.6.0/ScopeSim.egg-info/SOURCES.txt
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)        1 2023-07-10 14:44:14.000000 ScopeSim-0.6.0/ScopeSim.egg-info/dependency_links.txt
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      434 2023-07-10 14:44:14.000000 ScopeSim-0.6.0/ScopeSim.egg-info/requires.txt
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       28 2023-07-10 14:44:14.000000 ScopeSim-0.6.0/ScopeSim.egg-info/top_level.txt
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.452014 ScopeSim-0.6.0/docs/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)        0 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/docs/__init__.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.452014 ScopeSim-0.6.0/docs/source/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)        0 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/docs/source/__init__.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.452014 ScopeSim-0.6.0/docs/source/_ext/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)        0 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/docs/source/_ext/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1244 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/docs/source/_ext/scopesim_sphinx_ext.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       72 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/docs/source/_ext/test_scopesim_sphinx_ext.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     7970 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/docs/source/conf.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1904 2023-07-10 14:00:47.000000 ScopeSim-0.6.0/pyproject.toml
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.452014 ScopeSim-0.6.0/scopesim/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     3287 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     2548 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/base_classes.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.452014 ScopeSim-0.6.0/scopesim/commands/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       40 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/commands/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    15036 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/commands/user_commands.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.448014 ScopeSim-0.6.0/scopesim/data/
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.448014 ScopeSim-0.6.0/scopesim/data/svo/
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.452014 ScopeSim-0.6.0/scopesim/data/svo/2MASS/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    11859 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/2MASS/2MASS.H
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    16464 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/2MASS/2MASS.J
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13556 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/2MASS/2MASS.Ks
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.460014 ScopeSim-0.6.0/scopesim/data/svo/GTC/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    71472 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13131 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F643
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12702 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F643_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    11853 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F648
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    11482 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F648_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    15666 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F657
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    15055 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F657_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    11944 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F666
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    11576 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F666_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12648 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F680
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12233 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F680_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13110 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F694
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12702 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F694_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13189 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F709
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12795 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F709_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12973 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F723
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12621 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F723_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12980 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F738
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12608 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F738_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13449 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F754
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13067 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F754_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    15422 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F770
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    14863 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F770_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    16672 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F785
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    15992 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F785_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    16103 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F802
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    15429 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F802_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    17153 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F819
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    16369 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F819_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    14863 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F838
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    14207 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F838_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    14996 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F858
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    14311 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F858_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    15495 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F878
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    14782 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F878_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    14587 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F893
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13934 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F893_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13465 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F902
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12902 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F902_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13871 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F911
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13278 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F911_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13056 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F919
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12515 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F919_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12853 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F924
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12328 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F924_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12852 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F927
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12339 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F927_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12756 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F932
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12244 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F932_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12758 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F936
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12244 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F936_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12764 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F940
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12234 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F940_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    25885 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.sdss_g_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    26728 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.sdss_i_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    27457 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.sdss_r_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    33965 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.sdss_z_filter
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.460014 ScopeSim-0.6.0/scopesim/data/svo/Gemini/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    95207 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/Gemini/NIRI.Lprime-G0207w
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.460014 ScopeSim-0.6.0/scopesim/data/svo/Generic/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     8344 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/Generic/Bessell.V
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     8631 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/Generic/Johnson.I
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     9112 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/Generic/Johnson.J
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     9240 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/Generic/Johnson_UBVRIJHKL.N
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.460014 ScopeSim-0.6.0/scopesim/data/svo/HST/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    58531 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/HST/WFC3_IR.F160W
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.464015 ScopeSim-0.6.0/scopesim/data/svo/JWST/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    20594 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    48045 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1000W
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    25066 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1065C
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    36354 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1130W
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    25357 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1140C
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    59537 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1280W
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    77628 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1500W
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    25578 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1550C
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    96583 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1800W
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)   133082 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F2100W
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    25578 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F2300C
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)   135422 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F2550W
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    35473 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F560W
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    52930 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F770W
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13045 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/JWST/NIRCam.F164N
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.464015 ScopeSim-0.6.0/scopesim/data/svo/None/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      272 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/None/None.None
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.464015 ScopeSim-0.6.0/scopesim/data/svo/Paranal/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    33154 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/Paranal/HAWKI.BrGamma
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    24618 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/Paranal/HAWKI.H
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    16731 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/Paranal/HAWKI.J
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    28804 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/Paranal/HAWKI.Ks
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     9107 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/Paranal/NACO.Ks
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.464015 ScopeSim-0.6.0/scopesim/data/svo/SLOAN/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)   181368 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/SLOAN/SDSS.rprime_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    19736 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/SLOAN/SDSS.z
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)   501297 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/data/svo/SLOAN/SDSS.zprime_filter
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     2256 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/defaults.yaml
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.464015 ScopeSim-0.6.0/scopesim/detector/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       72 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/detector/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1443 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/detector/detector.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     4246 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/detector/detector_array.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    20469 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/detector/nghxrg.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.468015 ScopeSim-0.6.0/scopesim/effects/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      483 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    20300 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/apertures.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     5831 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/data_container.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    11603 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/detector_list.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    10443 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/effects/effects.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     3900 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/effects_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    21263 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/electronic.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    21587 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/fits_headers.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    18732 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/effects/metis_lms_trace_list.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     3181 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/effects/obs_strategies.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     9485 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/psf_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    30944 2023-07-10 11:34:12.000000 ScopeSim-0.6.0/scopesim/effects/psfs.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      979 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/rotation.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    12874 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/shifts.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     4347 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/spectral_efficiency.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    17403 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/effects/spectral_trace_list.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    36728 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/effects/spectral_trace_list_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     6185 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/surface_list.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     7614 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/effects/surface_list_OLD.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    32077 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/ter_curves.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    13313 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/effects/ter_curves_utils.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.468015 ScopeSim-0.6.0/scopesim/optics/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     9457 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/optics/OLD_fov.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     4440 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/optics/OLD_fov_manager.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      425 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/optics/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    26506 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/optics/fov.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    15597 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/optics/fov_manager.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    14430 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/optics/fov_manager_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    15669 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/optics/fov_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     4582 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/optics/image_plane.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    26192 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/optics/image_plane_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     2808 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/optics/monochromatic_trace_curve.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     9022 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/optics/optical_element.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    19505 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/optics/optical_train.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    11965 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/optics/optics_manager.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     3046 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/optics/radiometry.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     5223 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/optics/radiometry_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)        0 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/optics/spectrograph.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     9819 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/optics/surface.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     3971 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/optics/surface_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      747 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/rc.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.468015 ScopeSim-0.6.0/scopesim/reports/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)        0 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/reports/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      550 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/reports/report_generator.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    10591 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/reports/rst_utils.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.472015 ScopeSim-0.6.0/scopesim/server/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     5079 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/server/OLD_database.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      204 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/server/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    17459 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/server/database.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     2682 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/server/download_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     5110 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/server/example_data_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     4447 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/server/github_utils.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.472015 ScopeSim-0.6.0/scopesim/source/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       60 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/source/__init__.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    23757 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/source/source.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     8982 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/source/source_templates.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     7887 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/source/source_utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     5320 2023-07-10 13:56:39.000000 ScopeSim-0.6.0/scopesim/system_dict.py
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.448014 ScopeSim-0.6.0/scopesim/tests/
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.472015 ScopeSim-0.6.0/scopesim/tests/mocks/
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.472015 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    63184 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/ATMO_default_NIR_IMG.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      255 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/FITS_extra_keywords.yaml
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      341 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/INS_common_optics.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      390 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/INS_ifu_apertures.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)   109440 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/INS_ifu_traces.fits
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    69120 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/INS_lss_traces.fits
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       75 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/INS_unity_refl.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       77 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/INS_unity_trans.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      613 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/YAML_atmosphere.yaml
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1414 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/YAML_basic_instrument.yaml
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     2165 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/YAML_detector.yaml
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      517 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/YAML_mode_ifu.yaml
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      528 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/YAML_mode_spectroscopy.yaml
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      561 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/YAML_telescope.yaml
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.472015 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/code/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     4077 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/code/make_spectral_trace.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1381 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/default.yaml
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.472015 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/filters/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     6330 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/filters/TC_filter_BrGamma.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    18524 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/filters/TC_filter_CH4.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     4406 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/filters/TC_filter_H.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     2663 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/filters/TC_filter_J.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     5331 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/filters/TC_filter_Ks.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       77 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/filters/TC_filter_open.dat
+drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2023-07-10 14:44:14.476015 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/slits/
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      158 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/slits/SLIT_narrow.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)      142 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/slits/SLIT_wide.dat
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     1318 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/tests/mocks/load_basic_instrument.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)    27183 2023-07-10 09:28:17.000000 ScopeSim-0.6.0/scopesim/utils.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)   276480 2023-07-10 09:22:12.000000 ScopeSim-0.6.0/scopesim/vega.fits
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)     4730 2023-07-10 14:10:43.000000 ScopeSim-0.6.0/scopesim/version.py
+-rw-rw-r--   0 hugo      (1000) hugo      (1000)       38 2023-07-10 14:44:14.476015 ScopeSim-0.6.0/setup.cfg
```

### Comparing `ScopeSim-0.5.6/ScopeSim.egg-info/SOURCES.txt` & `ScopeSim-0.6.0/ScopeSim.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-LICENCE
+LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
 ScopeSim.egg-info/PKG-INFO
 ScopeSim.egg-info/SOURCES.txt
 ScopeSim.egg-info/dependency_links.txt
 ScopeSim.egg-info/requires.txt
 ScopeSim.egg-info/top_level.txt
+docs/__init__.py
 docs/source/__init__.py
 docs/source/conf.py
-docs/source/getting_started.py
 docs/source/_ext/__init__.py
 docs/source/_ext/scopesim_sphinx_ext.py
 docs/source/_ext/test_scopesim_sphinx_ext.py
 scopesim/__init__.py
 scopesim/base_classes.py
 scopesim/defaults.yaml
 scopesim/rc.py
@@ -127,14 +127,15 @@
 scopesim/effects/fits_headers.py
 scopesim/effects/metis_lms_trace_list.py
 scopesim/effects/obs_strategies.py
 scopesim/effects/psf_utils.py
 scopesim/effects/psfs.py
 scopesim/effects/rotation.py
 scopesim/effects/shifts.py
+scopesim/effects/spectral_efficiency.py
 scopesim/effects/spectral_trace_list.py
 scopesim/effects/spectral_trace_list_utils.py
 scopesim/effects/surface_list.py
 scopesim/effects/surface_list_OLD.py
 scopesim/effects/ter_curves.py
 scopesim/effects/ter_curves_utils.py
 scopesim/optics/OLD_fov.py
@@ -157,14 +158,17 @@
 scopesim/optics/surface_utils.py
 scopesim/reports/__init__.py
 scopesim/reports/report_generator.py
 scopesim/reports/rst_utils.py
 scopesim/server/OLD_database.py
 scopesim/server/__init__.py
 scopesim/server/database.py
+scopesim/server/download_utils.py
+scopesim/server/example_data_utils.py
+scopesim/server/github_utils.py
 scopesim/source/__init__.py
 scopesim/source/source.py
 scopesim/source/source_templates.py
 scopesim/source/source_utils.py
 scopesim/tests/mocks/load_basic_instrument.py
 scopesim/tests/mocks/basic_instrument/ATMO_default_NIR_IMG.dat
 scopesim/tests/mocks/basic_instrument/FITS_extra_keywords.yaml
```

### Comparing `ScopeSim-0.5.6/docs/source/_ext/scopesim_sphinx_ext.py` & `ScopeSim-0.6.0/docs/source/_ext/scopesim_sphinx_ext.py`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/docs/source/conf.py` & `ScopeSim-0.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/__init__.py` & `ScopeSim-0.6.0/scopesim/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 ################################################################################
 #                            TURN OFF WARNINGS                                 #
 ################################################################################
 import sys
 import logging
 import warnings
 import yaml
+from importlib import metadata
 from astropy.utils.exceptions import AstropyWarning
 
 warnings.simplefilter('ignore', UserWarning)
 warnings.simplefilter('ignore', FutureWarning)
 warnings.simplefilter('ignore', RuntimeWarning)     # warnings for the developer
 warnings.simplefilter('ignore', category=AstropyWarning)
 yaml.warnings({'YAMLLoadWarning': False})
@@ -71,11 +72,8 @@
 
 from .tests.mocks.load_basic_instrument import load_example_optical_train
 
 ################################################################################
 #                          VERSION INFORMATION                                 #
 ################################################################################
 
-try:
-    from .version import version as __version__
-except ImportError:
-    __version__ = "Version number is not available"
+__version__ = metadata.version(__package__)
```

### Comparing `ScopeSim-0.5.6/scopesim/base_classes.py` & `ScopeSim-0.6.0/scopesim/base_classes.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,28 +38,28 @@
         if isinstance(obj, Header):
             comments = {key: obj.comments[key] for key in obj
                         if obj.comments[key] != ""}
             self.comments.update(comments)
             self.dic.update(dict(obj))
 
         if isinstance(obj, dict):
-            if any([isinstance(obj[key], (tuple, list)) for key in obj]):
+            if any(isinstance(obj[key], (tuple, list)) for key in obj):
                 for key in obj:
                     if isinstance(obj[key], (tuple, list)):
                         self.comments[key] = obj[key][1]
                         self.dic[key] = obj[key][0]
                     else:
                         self.dic[key] = obj[key]
             else:
                 self.dic.update(obj)
 
     def as_header(self):
         hdr = Header(self.dic)
-        for key in self.comments:
-            hdr.comments[key] = self.comments[key]
+        for key, value in self.comments.items():
+            hdr.comments[key] = value
 
         return hdr
 
     def __setitem__(self, key, value):
         if isinstance(value, (tuple, list)):
             value, comment = value
             self.comments[key] = comment
@@ -76,32 +76,28 @@
         return self.dic.__iter__()
 
     def __contains__(self, item):
         return self.dic.__contains__(item)
 
     def __repr__(self):
         msgs = ""
-        for key in self.dic:
+        for key, value in self.dic.items():
             cmt_msg = ""
             if key in self.comments:
-                cmt_msg = " / {}".format(self.comments[key])
-
-            msg = "{} = {}".format(key.upper().ljust(9),
-                                   str(self.dic[key]).rjust(16))
-            msgs += msg + cmt_msg + "\n"
-
+                cmt_msg = " / {self.comments[key]}"
+            msgs += f"{key.upper():<9} = {value!s:>16}{cmt_msg}\n"
         return msgs
 
     def items(self):
         items_dict = []
-        for key in self.dic:
+        for key, value in self.dic.items():
             if key in self.comments:
-                items_dict += [(key, (self.dic[key], self.comments[key]))]
+                items_dict.append((key, (value, self.comments[key])))
             else:
-                items_dict += [(key, self.dic[key])]
+                items_dict.append((key, value))
         return items_dict
 
     def keys(self):
         return self.dic.__iter__()
 
     def values(self):
         """Like :meth:`dict.values`."""
```

### Comparing `ScopeSim-0.5.6/scopesim/commands/user_commands.py` & `ScopeSim-0.6.0/scopesim/commands/user_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import logging
 import copy
+from pathlib import Path
 
 import numpy as np
 import yaml
 import requests
 
 from .. import rc
 from ..utils import find_file
@@ -176,27 +177,27 @@
                     yaml_file = find_file(yaml_input)
                     if yaml_file is not None:
                         yaml_dict = load_yaml_dicts(yaml_file)
                         self.update(yamls=yaml_dict)
                         if yaml_input == "default.yaml":
                             self.default_yamls = yaml_dict
                     else:
-                        logging.warning("{} could not be found".format(yaml_input))
+                        logging.warning("%s could not be found", yaml_input)
 
                 elif isinstance(yaml_input, dict):
                     self.cmds.update(yaml_input)
-                    self.yaml_dicts += [yaml_input]
+                    self.yaml_dicts.append(yaml_input)
 
                     for key in ["packages", "yamls", "mode_yamls"]:
                         if key in yaml_input:
                             self.update(**{key: yaml_input[key]})
 
                 else:
                     raise ValueError("yaml_dicts must be a filename or a "
-                                     "dictionary: {}".format(yaml_input))
+                                     f"dictionary: {yaml_input}")
 
         if "mode_yamls" in kwargs:
             # Convert the yaml list of modes to a dict object
             self.modes_dict = {my["name"]: my for my in kwargs["mode_yamls"]}
             if "modes" in self.cmds["!OBS"]:
                 if not isinstance(self.cmds["!OBS.modes"], list):
                     self.cmds["!OBS.modes"] = [self.cmds["!OBS.modes"]]
@@ -225,30 +226,29 @@
         if not isinstance(modes, list):
             modes = [modes]
         for defyam in self.default_yamls:
             if "properties" in defyam and "modes" in defyam["properties"]:
                 defyam["properties"]["modes"] = []
                 for mode in modes:
                     if mode in self.modes_dict:
-                        defyam["properties"]["modes"] += [mode]
+                        defyam["properties"]["modes"].append(mode)
                     else:
-                        raise ValueError("mode '{}' was not recognised"
-                                         "".format(mode))
+                        raise ValueError(f"mode '{mode}' was not recognised")
 
         self.__init__(yamls=self.default_yamls)
 
     def list_modes(self):
         if isinstance(self.modes_dict, dict):
             modes = {}
             for mode_name in self.modes_dict:
                 dic = self.modes_dict[mode_name]
                 desc = dic["description"] if "description" in dic else "<None>"
                 modes[mode_name] = desc
 
-            msg = "\n".join(["{}: {}".format(key, modes[key]) for key in modes])
+            msg = "\n".join([f"{key}: {value}" for key, value in modes.items()])
         else:
             msg = "No modes found"
         return msg
 
     @property
     def modes(self):
         print(self.list_modes())
@@ -259,57 +259,102 @@
     def __getitem__(self, item):
         return self.cmds.__getitem__(item)
 
     def __contains__(self, item):
         return self.cmds.__contains__(item)
 
     def __repr__(self):
-        return self.cmds.__repr__()
+        return f"{self.__class__.__name__}(**{self.kwargs!r})"
 
 
 def check_for_updates(package_name):
     """
     Asks IRDB server if there are newer versions of the instrument package
     """
     response = {}
 
     # tracking **exclusively** your IP address for our internal stats
     if rc.__currsys__["!SIM.reports.ip_tracking"] and \
             "TRAVIS" not in os.environ:
         front_matter = rc.__currsys__["!SIM.file.server_base_url"]
-        back_matter = "api.php?package_name={}".format(package_name)
+        back_matter = f"api.php?package_name={package_name}"
         try:
             response = requests.get(url=front_matter+back_matter).json()
         except:
-            print("Offline. Cannot check for updates for {}"
-                  "".format(package_name))
+            print(f"Offline. Cannot check for updates for {package_name}")
     return response
 
 
+def patch_fake_symlinks(path: Path):
+    """Fixes broken symlinks in path.
+
+    The irdb has some symlinks in it, which work fine under linux, but not
+    always under windows, see https://stackoverflow.com/a/11664406 .
+
+    "This makes symlinks created and committed e.g. under Linux appear as
+    plain text files that contain the link text under Windows"
+
+    It is therefore necessary to assume that these can be regular files.
+
+    E.g. when Path.cwd() is
+    WindowsPath('C:/Users/hugo/hugo/repos/irdb/MICADO/docs/example_notebooks')
+    and path is WindowsPath('inst_pkgs/MICADO')
+    then this function should return
+    WindowsPath('C:/Users/hugo/hugo/repos/irdb/MICADO')
+    """
+    path = path.resolve()
+    if path.exists() and path.is_dir():
+        # A normal directory.
+        return path
+    if path.exists() and path.is_file():
+        # Could be a regular file, or a broken symlink.
+        size = path.stat().st_size
+        if size > 250 or size == 0:
+            # A symlink is probably not longer than 250 characters.
+            return path
+        line = open(path).readline()
+        if len(line) != size:
+            # There is more content in the file, so probably not a link.
+            return path
+        pline = Path(line)
+        if pline.exists():
+            # The file contains exactly a path that exists. So it is
+            # probably a link.
+            return pline.resolve()
+    if path.exists():
+        # The path exists, but is not a file or directory. Just return it.
+        return path
+    # The path does not exist.
+    parent = path.parent
+    pathup = patch_fake_symlinks(parent)
+    assert pathup != parent, ValueError("Cannot find path")
+    return patch_fake_symlinks(pathup / path.name)
+
+
 def add_packages_to_rc_search(local_path, package_list):
     """
     Adds the paths of a list of locally saved packages to the search path list
 
     Parameters
     ----------
     local_path : str
         Where the pacakges are located. Generally given by the value in
         scopesim.rc.__config__["!SIM.file.local_packages_path"]
 
     package_list : list
         A list of the package names to add
 
     """
-
+    plocal_path = patch_fake_symlinks(Path(local_path))
     for pkg in package_list:
-        pkg_dir = os.path.abspath(os.path.join(local_path, pkg))
-        if not os.path.exists(pkg_dir):
+        pkg_dir = plocal_path / pkg
+        if not pkg_dir.exists():
             # todo: keep here, but add test for this by downloading test_package
             # raise ValueError("Package could not be found: {}".format(pkg_dir))
-            logging.warning("Package could not be found: {}".format(pkg_dir))
+            logging.warning("Package could not be found: %s", pkg_dir)
 
         if pkg_dir in rc.__search_path__:
             # if package is already in search_path, move it to the first place
             ii = np.where(np.array(rc.__search_path__) == pkg_dir)[0][0]
             rc.__search_path__.pop(ii)
 
         rc.__search_path__ = [pkg_dir] + rc.__search_path__
@@ -367,23 +412,21 @@
     Returns
     -------
     main_pkgs, ext_pkgs : lists
         If action="return": Lists containing the names of locally saved packages
 
     """
 
-    local_path = os.path.abspath(rc.__config__["!SIM.file.local_packages_path"])
-    pkgs = [d for d in os.listdir(local_path) if
-            os.path.isdir(os.path.join(local_path, d))]
-
-    main_pkgs = [pkg for pkg in pkgs if
-                 os.path.exists(os.path.join(local_path, pkg, "default.yaml"))]
-    ext_pkgs = [pkg for pkg in pkgs if not
-                os.path.exists(os.path.join(local_path, pkg, "default.yaml"))]
+    local_path = Path(rc.__config__["!SIM.file.local_packages_path"]).absolute()
+    pkgs = [d for d in local_path.iterdir() if d.is_dir()]
+
+    main_pkgs = [pkg for pkg in pkgs if (pkg/"default.yaml").exists()]
+    ext_pkgs = [pkg for pkg in pkgs if not (pkg/"default.yaml").exists()]
 
     if action == "display":
-        msg = "\nLocal package directory:\n  {}\n" \
-              "Full packages [can be used with 'use_instrument=...']\n  {}\n" \
-              "Support packages\n  {}".format(local_path, main_pkgs, ext_pkgs)
+        msg = (f"\nLocal package directory:\n  {local_path}\n"
+               "Full packages [can be used with 'use_instrument=...']\n"
+               f"{main_pkgs}\n"
+               f"Support packages\n  {ext_pkgs}")
         print(msg)
     else:
         return main_pkgs, ext_pkgs
```

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/2MASS/2MASS.H` & `ScopeSim-0.6.0/scopesim/data/svo/2MASS/2MASS.H`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/2MASS/2MASS.J` & `ScopeSim-0.6.0/scopesim/data/svo/2MASS/2MASS.J`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/2MASS/2MASS.Ks` & `ScopeSim-0.6.0/scopesim/data/svo/2MASS/2MASS.Ks`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F643` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F643`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F643_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F643_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F648` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F648`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F648_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F648_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F657` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F657`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F657_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F657_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F666` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F666`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F666_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F666_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F680` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F680`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F680_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F680_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F694` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F694`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F694_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F694_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F709` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F709`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F709_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F709_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F723` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F723`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F723_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F723_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F738` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F738`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F738_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F738_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F754` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F754`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F754_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F754_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F770` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F770`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F770_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F770_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F785` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F785`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F785_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F785_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F802` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F802`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F802_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F802_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F819` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F819`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F819_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F819_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F838` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F838`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F838_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F838_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F858` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F858`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F858_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F858_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F878` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F878`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F878_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F878_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F893` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F893`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F893_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F893_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F902` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F902`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F902_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F902_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F911` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F911`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F911_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F911_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F919` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F919`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F919_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F919_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F924` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F924`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F924_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F924_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F927` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F927`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F927_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F927_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F932` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F932`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F932_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F932_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F936` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F936`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F936_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F936_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F940` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F940`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.F940_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.F940_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.sdss_g_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.sdss_g_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.sdss_i_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.sdss_i_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.sdss_r_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.sdss_r_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/GTC/OSIRIS.sdss_z_filter` & `ScopeSim-0.6.0/scopesim/data/svo/GTC/OSIRIS.sdss_z_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/Gemini/NIRI.Lprime-G0207w` & `ScopeSim-0.6.0/scopesim/data/svo/Gemini/NIRI.Lprime-G0207w`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/Generic/Bessell.V` & `ScopeSim-0.6.0/scopesim/data/svo/Generic/Bessell.V`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/Generic/Johnson.I` & `ScopeSim-0.6.0/scopesim/data/svo/Generic/Johnson.I`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/Generic/Johnson.J` & `ScopeSim-0.6.0/scopesim/data/svo/Generic/Johnson.J`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/Generic/Johnson_UBVRIJHKL.N` & `ScopeSim-0.6.0/scopesim/data/svo/Generic/Johnson_UBVRIJHKL.N`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/HST/WFC3_IR.F160W` & `ScopeSim-0.6.0/scopesim/data/svo/HST/WFC3_IR.F160W`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1000W` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1000W`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1065C` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1065C`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1130W` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1130W`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1140C` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1140C`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1280W` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1280W`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1500W` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1500W`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1550C` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1550C`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F1800W` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F1800W`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F2100W` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F2100W`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F2300C` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F2300C`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F2550W` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F2550W`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F560W` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F560W`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/MIRI.F770W` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/MIRI.F770W`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/JWST/NIRCam.F164N` & `ScopeSim-0.6.0/scopesim/data/svo/JWST/NIRCam.F164N`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/Paranal/HAWKI.BrGamma` & `ScopeSim-0.6.0/scopesim/data/svo/Paranal/HAWKI.BrGamma`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/Paranal/HAWKI.H` & `ScopeSim-0.6.0/scopesim/data/svo/Paranal/HAWKI.H`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/Paranal/HAWKI.J` & `ScopeSim-0.6.0/scopesim/data/svo/Paranal/HAWKI.J`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/Paranal/HAWKI.Ks` & `ScopeSim-0.6.0/scopesim/data/svo/Paranal/HAWKI.Ks`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/Paranal/NACO.Ks` & `ScopeSim-0.6.0/scopesim/data/svo/Paranal/NACO.Ks`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/SLOAN/SDSS.rprime_filter` & `ScopeSim-0.6.0/scopesim/data/svo/SLOAN/SDSS.rprime_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/SLOAN/SDSS.z` & `ScopeSim-0.6.0/scopesim/data/svo/SLOAN/SDSS.z`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/data/svo/SLOAN/SDSS.zprime_filter` & `ScopeSim-0.6.0/scopesim/data/svo/SLOAN/SDSS.zprime_filter`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/defaults.yaml` & `ScopeSim-0.6.0/scopesim/defaults.yaml`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/detector/detector.py` & `ScopeSim-0.6.0/scopesim/detector/detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         self.meta.update(header)
         self.meta.update(kwargs)
 
     def extract_from(self, image_plane, spline_order=1, reset=True):
         if reset:
             self.reset()
         if not isinstance(image_plane, ImagePlaneBase):
-            raise ValueError("image_plane must be an ImagePlane object: {}"
-                             "".format(type(image_plane)))
+            raise ValueError("image_plane must be an ImagePlane object, but is: "
+                             f"{type(image_plane)}")
 
         self._hdu = imp_utils.add_imagehdu_to_imagehdu(image_plane.hdu,
                                                        self.hdu, spline_order,
                                                        wcs_suffix="D")
 
     def reset(self):
         self._hdu.data = np.zeros(self._hdu.data.shape)
```

### Comparing `ScopeSim-0.5.6/scopesim/detector/detector_array.py` & `ScopeSim-0.6.0/scopesim/detector/detector_array.py`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/detector/nghxrg.py` & `ScopeSim-0.6.0/scopesim/detector/nghxrg.py`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/effects/apertures.py` & `ScopeSim-0.6.0/scopesim/effects/apertures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Effects related to field masks, including spectroscopic slits"""
-from os import path as pth
-from copy import deepcopy
+
+from pathlib import Path
 import logging
 import yaml
 
 import numpy as np
-from matplotlib.path import Path
+from matplotlib.path import Path as MPLPath  # rename to avoid conflict with pathlib
 from astropy.io import fits
 from astropy import units as u
 from astropy.table import Table
 
 from .effects import Effect
 from ..optics import image_plane_utils as imp_utils
 from ..base_classes import FOVSetupBase
@@ -333,15 +333,15 @@
                       "shape": row["shape"],
                       "conserve_image": yaml.full_load(str(row["conserve_image"])),
                       "no_mask": self.meta["no_mask"],
                       "pixel_scale": self.meta["pixel_scale"],
                       "x_unit": "arcsec",
                       "y_unit": "arcsec",
                       "angle_unit": "arcsec"}
-            apertures_list += [ApertureMask(array_dict=array_dict, **params)]
+            apertures_list.append(ApertureMask(array_dict=array_dict, **params))
 
         return apertures_list
 
     def plot(self):
         import matplotlib.pyplot as plt
         plt.gcf().clf()
 
@@ -366,16 +366,16 @@
     def __add__(self, other):
         if isinstance(other, ApertureList):
             from astropy.table import vstack
             self.table = vstack([self.table, other.table])
 
             return self
         else:
-            raise ValueError("Secondary argument not of type ApertureList: {}"
-                             "".format(type(other)))
+            raise ValueError("Secondary argument not of type ApertureList: "
+                             f"{type(other) = }")
 
     # def __getitem__(self, item):
     #     return self.get_apertures(item)[0]
 
 
 
 class SlitWheel(Effect):
@@ -429,35 +429,34 @@
                   "path": "",
                   "report_plot_include": False,
                   "report_table_include": True,
                   "report_table_rounding": 4}
         self.meta.update(params)
         self.meta.update(kwargs)
 
-        path = pth.join(self.meta["path"],
-                        from_currsys(self.meta["filename_format"]))
+        path = Path(self.meta["path"], from_currsys(self.meta["filename_format"]))
         self.slits = {}
         for name in from_currsys(self.meta["slit_names"]):
             kwargs["name"] = name
-            self.slits[name] = ApertureMask(filename=path.format(name),
-                                            **kwargs)
+            fname = str(path).format(name)
+            self.slits[name] = ApertureMask(filename=fname, **kwargs)
 
         self.table = self.get_table()
 
     def apply_to(self, obj, **kwargs):
         """Use apply_to of current_slit"""
         return self.current_slit.apply_to(obj, **kwargs)
 
     def fov_grid(self, which="edges", **kwargs):
         return self.current_slit.fov_grid(which=which, **kwargs)
 
     def change_slit(self, slitname=None):
         """Change the current slit"""
         if not slitname or slitname in self.slits.keys():
-            self.meta['current_slit'] = slitname
+            self.meta["current_slit"] = slitname
             self.include = slitname
         else:
             raise ValueError("Unknown slit requested: " + slitname)
 
     def add_slit(self, newslit, name=None):
         """
         Add a slit to the SlitWheel
@@ -479,37 +478,37 @@
         currslit = from_currsys(self.meta["current_slit"])
         if not currslit:
             return False
         return self.slits[currslit]
 
     @property
     def display_name(self):
-        return f'{self.meta["name"]} : ' \
-               f'[{from_currsys(self.meta["current_slit"])}]'
+        return f"{self.meta['name']} : " \
+               f"[{from_currsys(self.meta['current_slit'])}]"
 
 
     def __getattr__(self, item):
         return getattr(self.current_slit, item)
 
     def get_table(self):
         """
         Create a table of slits with centre position, width and length
 
         Width is defined as the extension in the y-direction, length in the
         x-direction. All values are in milliarcsec.
         """
         names = list(self.slits.keys())
         slits = self.slits.values()
-        xmax = np.array([slit.data['x'].max() * u.Unit(slit.meta['x_unit'])
+        xmax = np.array([slit.data["x"].max() * u.Unit(slit.meta["x_unit"])
                          .to(u.mas) for slit in slits])
-        xmin = np.array([slit.data['x'].min() * u.Unit(slit.meta['x_unit'])
+        xmin = np.array([slit.data["x"].min() * u.Unit(slit.meta["x_unit"])
                          .to(u.mas) for slit in slits])
-        ymax = np.array([slit.data['y'].max() * u.Unit(slit.meta['y_unit'])
+        ymax = np.array([slit.data["y"].max() * u.Unit(slit.meta["y_unit"])
                          .to(u.mas) for slit in slits])
-        ymin = np.array([slit.data['y'].min() * u.Unit(slit.meta['y_unit'])
+        ymin = np.array([slit.data["y"].min() * u.Unit(slit.meta["y_unit"])
                          .to(u.mas) for slit in slits])
         xmax = quantify(xmax, u.mas)
         xmin = quantify(xmin, u.mas)
         ymax = quantify(ymax, u.mas)
         ymin = quantify(ymin, u.mas)
 
         lengths = xmax - xmin
@@ -565,15 +564,15 @@
     naxis1 = int(np.ceil((np.max(x) - np.min(x)) / pixel_scale))
     naxis2 = int(np.ceil((np.max(y) - np.min(y)) / pixel_scale))
     xrange = np.linspace(np.min(x), np.max(x), naxis1)
     yrange = np.linspace(np.min(y), np.max(y), naxis2)
     coords = [(xi, yi) for xi in xrange for yi in yrange]
 
     corners = [(xi, yi) for xi, yi in zip(x, y)]
-    path = Path(corners)
+    path = MPLPath(corners)
     # ..todo: known issue - for super thin apertures, the first row is masked
     # rad = 0.005
     rad = 0  # increase this to include slightly more points within the polygon
     mask = path.contains_points(coords, radius=rad).reshape((naxis2, naxis1))
 
     return mask
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/data_container.py` & `ScopeSim-0.6.0/scopesim/effects/data_container.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,25 +110,23 @@
         else:
             self.headers += [None]
 
         self.meta.update(self.table.meta)
         self.meta.update(hdr_dict)
         # self.table.meta.update(hdr_dict)
         self.table.meta.update(self.meta)
-        self.meta["history"] += ["ASCII table read from {}"
-                                 "".format(self.meta["filename"])]
+        self.meta["history"] += [f"ASCII table read from {self.meta['filename']}"]
 
     def _load_fits(self):
         self._file = fits.open(self.meta["filename"])
         for ext in self._file:
             self.headers += [ext.header]
 
         self.meta.update(dict(self._file[0].header))
-        self.meta["history"] += ["Opened handle to FITS file {}"
-                                 "".format(self.meta["filename"])]
+        self.meta["history"] += [f"Opened handle to FITS file {self.meta['filename']}"]
 
     def get_data(self, ext=0, layer=None):
         """
         Returns either a table or a ImageHDU object
 
         .. note:: Use this call for reading in individual FITS extensions.
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/detector_list.py` & `ScopeSim-0.6.0/scopesim/effects/detector_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,30 +114,30 @@
         self.meta.update(params)
         self.meta.update(kwargs)
 
         # for backwards compatibility
         new_colnames = {"xhw": "x_size", "yhw": "y_size", "pixsize": "pixel_size"}
         mult_cols = {"xhw": 2., "yhw": 2., "pixsize": 1.}
         if isinstance(self.table, Table):
-            for col in new_colnames:
+            for col, new_name in new_colnames.items():
                 if col in self.table.colnames:
                     self.table[col] = self.table[col] * mult_cols[col]
-                    self.table.rename_column(col, new_colnames[col])
+                    self.table.rename_column(col, new_name)
         if not "x_size_unit" in self.meta and "xhw_unit" in self.meta:
             self.meta["x_size_unit"] = self.meta["xhw_unit"]
         if not "y_size_unit" in self.meta and "yhw_unit" in self.meta:
             self.meta["y_size_unit"] = self.meta["yhw_unit"]
 
     def apply_to(self, obj, **kwargs):
         if isinstance(obj, FOVSetupBase):
 
             hdr = self.image_plane_header
             x_mm, y_mm = calc_footprint(hdr, "D")
             pixel_size = hdr["CDELT1D"]              # mm
-            pixel_scale = (kwargs.get("pixel_scale", self.meta["pixel_scale"]))   # ["]
+            pixel_scale = kwargs.get("pixel_scale", self.meta["pixel_scale"])   # ["]
             pixel_scale = utils.from_currsys(pixel_scale)
             x_sky = x_mm * pixel_scale / pixel_size  # x["] = x[mm] * ["] / [mm]
             y_sky = y_mm * pixel_scale / pixel_size  # y["] = y[mm] * ["] / [mm]
 
             obj.shrink(axis=["x", "y"], values=([min(x_sky), max(x_sky)],
                                                 [min(y_sky), max(y_sky)]))
             obj.detector_limits = {"xd_min": min(x_mm),
@@ -205,22 +205,21 @@
             tbl = self.table
         elif isinstance(self.meta["active_detectors"], (list, tuple)):
             mask = [det_id in self.meta["active_detectors"]
                     for det_id in self.table["id"]]
             tbl = self.table[mask]
         else:
             raise ValueError("Could not determine which detectors are active: "
-                             "{}, {}, ".format(self.meta["active_detectors"],
-                                               self.table))
+                             f"{self.meta['active_detectors']}, {self.table}, ")
         tbl = utils.from_currsys(tbl)
 
         return tbl
 
     def detector_headers(self, ids=None):
-        if ids is not None and all([isinstance(ii, int) for ii in ids]):
+        if ids is not None and all(isinstance(ii, int) for ii in ids):
             self.meta["active_detectors"] = list(ids)
 
         tbl = utils.from_currsys(self.active_table)
         hdrs = []
         for row in tbl:
             pixel_size = row["pixel_size"]
             xcen, ycen = float(row["x_cen"]), float(row["y_cen"])
@@ -240,19 +239,19 @@
                 hdr["PC1_2"] = sang
                 hdr["PC2_1"] = -sang
                 hdr["PC2_2"] = cang
 
             # hdr["GAIN"] = row["gain"]
             if "id" in row:
                 hdr["DET_ID"] = row["id"]
-                hdr["EXTNAME"] = f'DET_{row["id"]}'
+                hdr["EXTNAME"] = f"DET_{row['id']}"
 
             row_dict = {col: row[col] for col in row.colnames}
             hdr.update(row_dict)
-            hdrs += [hdr]
+            hdrs.append(hdr)
 
         return hdrs
 
     def plot(self):
         import matplotlib.pyplot as plt
         plt.gcf().clf()
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/effects.py` & `ScopeSim-0.6.0/scopesim/effects/effects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import os
-from astropy.table import Table
+from pathlib import Path
 
 from ..effects.data_container import DataContainer
 from .. import base_classes as bc
 from ..utils import from_currsys, write_report
 from ..reports.rst_utils import table_to_rst
-from .. import rc
 
 
 class Effect(DataContainer):
     """
     The base class for representing the effects (artifacts) in an optical system
 
     The ``Effect`` class is conceived to independently apply the changes that
@@ -43,16 +41,16 @@
         self.meta["include"] = True
         self.meta.update(kwargs)
 
     def apply_to(self, obj, **kwargs):
         if not isinstance(obj, (bc.FOVSetupBase, bc.SourceBase,
                                 bc.FieldOfViewBase, bc.ImagePlaneBase,
                                 bc.DetectorBase)):
-            raise ValueError(f"object must one of the following: FOVSetupBase, "
-                             f"Source, FieldOfView, ImagePlane, Detector: "
+            raise ValueError("object must one of the following: FOVSetupBase, "
+                             "Source, FieldOfView, ImagePlane, Detector: "
                              f"{type(obj)}")
 
         return obj
 
     def fov_grid(self, which="", **kwargs):
         """
         Returns the edges needed to generate FieldOfViews for an observation
@@ -112,21 +110,21 @@
     @property
     def display_name(self):
         return self.meta.get("name", self.meta.get("filename", "<empty>"))
 
     @property
     def meta_string(self):
         meta_str = ""
-        max_key_len = max([len(key) for key in self.meta.keys()])
+        max_key_len = max(len(key) for key in self.meta.keys())
+        padlen = max_key_len + 4
         for key in self.meta:
-            if key not in ["comments", "changes", "description", "history",
+            if key not in {"comments", "changes", "description", "history",
                            "report_table_caption", "report_plot_caption",
-                           "table"]:
-                meta_str += "    {} : {}\n".format(key.rjust(max_key_len),
-                                                   self.meta[key])
+                           "table"}:
+                meta_str += f"{key:>{padlen}} : {self.meta[key]}\n"
 
         return meta_str
 
     def report(self, filename=None, output="rst", rst_title_chars="*+",
                **kwargs):
         """
         For Effect objects, generates a report based on the data and meta-data
@@ -219,120 +217,107 @@
                                                     "<no description>"),
                   "class_description": cls_descr,
                   "changes_str": changes_str}
         params.update(self.meta)
         params.update(kwargs)
         params = from_currsys(params)
 
-        rst_str = """
-{}
-{}
-**Included by default**: ``{}``
+        rst_str = f"""
+{str(self)}
+{rst_title_chars[0] * len(str(self))}
+**Included by default**: ``{params["include"]}``
 
-**File Description**: {}
+**File Description**: {params["file_description"]}
 
-**Class Description**: {}
+**Class Description**: {params["class_description"]}
 
 **Changes**:
 
-{}
+{params["changes_str"]}
 
 Data
-{}
-""".format(str(self),
-           rst_title_chars[0] * len(str(self)),
-           params["include"],
-           params["file_description"],
-           params["class_description"],
-           params["changes_str"],
-           rst_title_chars[1] * 4)
+{rst_title_chars[1] * 4}
+"""
 
         if params["report_plot_include"] and hasattr(self, "plot"):
             fig = self.plot()
 
             if fig is not None:
                 path = params["report_image_path"]
                 fname = params["report_plot_filename"]
                 if fname is None:
                     fname = self.meta["name"].lower().replace(" ", "_")
 
                 for fmt in params["report_plot_file_formats"]:
                     fname = ".".join((fname.split(".")[0], fmt))
-                    file_path = os.path.join(path, fname)
+                    file_path = Path(path, fname)
 
                     fig.savefig(fname=file_path)
 
                 # rel_path = os.path.relpath(params["report_image_path"],
                 #                            params["report_rst_path"])
                 # rel_file_path = os.path.join(rel_path, fname)
 
-                rst_str += """
-.. figure:: {}
-    :name: {}
-
-    {}
-""".format(fname,
-           "fig:" + params.get("name", "<unknown Effect>"),
-           params["report_plot_caption"])
+                rst_str += f"""
+.. figure:: {fname}
+    :name: {"fig:" + params.get("name", "<unknown Effect>")}
+
+    {params["report_plot_caption"]}
+"""
 
         if params["report_table_include"]:
-            rst_str += """
+            rst_str += f"""
 .. table::
-    :name: {}
+    :name: {"tbl:" + params.get("name")}
 
-{}
+{table_to_rst(self.table, indent=4, rounding=params["report_table_rounding"])}
 
-{}
-""".format("tbl:" + params.get("name"),
-           table_to_rst(self.table, indent=4,
-                        rounding=params["report_table_rounding"]),
-           params["report_table_caption"])
+{params["report_table_caption"]}
+"""
 
-        rst_str += """
+        rst_str += f"""
 Meta-data
-{}
+{rst_title_chars[1] * 9}
 ::
 
-{}
-""".format(rst_title_chars[1] * 9,
-           self.meta_string)
+{self.meta_string}
+"""
 
         write_report(rst_str, filename, output)
 
         return rst_str
 
     def info(self):
         """
         Prints basic information on the effect, notably the description
         """
-        name = self.meta.get("name", self.meta.get("filename", "<empty>"))
-        text = f'{type(self).__name__}: "{name}"'
+        text = str(self)
 
         desc = self.meta.get("description")
         if desc is not None:
-             text += f"\nDescription: {desc}"
+            text += f"\nDescription: {desc}"
 
         print(text)
 
     def __repr__(self):
-        return f'{type(self).__name__}: "{self.display_name}"'
+        return f"{self.__class__.__name__}(**{self.meta!r})"
 
     def __str__(self):
-        return self.__repr__()
+        return f"{self.__class__.__name__}: \"{self.display_name}\""
 
     def __getitem__(self, item):
-        if isinstance(item, str) and item[0] == "#":
+        if isinstance(item, str) and item.startswith("#"):
             if len(item) > 1:
-                if item[-1] == "!":
+                if item.endswith("!"):
                     key = item[1:-1]
                     if len(key) > 0:
                         value = from_currsys(self.meta[key])
                     else:
                         value = from_currsys(self.meta)
                 else:
                     value = self.meta[item[1:]]
             else:
                 value = self.meta
         else:
             raise ValueError(f"__getitem__ calls must start with '#': {item}")
 
-        return value
+        return value
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/effects_utils.py` & `ScopeSim-0.6.0/scopesim/effects/effects_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def combine_surface_effects(surface_effects):
     surflist_list = [eff for eff in surface_effects
                      if isinstance(eff, efs.SurfaceList)]
     surf_list = [eff for eff in surface_effects
                  if isinstance(eff, (efs.TERCurve, efs.FilterWheel))
                  and not isinstance(eff, efs.SurfaceList)]
 
-    if len(surflist_list) == 0:
+    if not surflist_list:
         surflist_list = [empty_surface_list(name="combined_surface_list")]
 
     new_surflist = copy(surflist_list[0])
     for surflist in surflist_list[1:]:
         new_surflist.add_surface_list(surflist)
 
     # ..todo:: should read position from the list positions in surface_effects
@@ -81,15 +81,15 @@
 
     return effect
 
 
 def is_spectroscope(effects):
     spec_classes = (efs.SpectralTraceList,
                     efs.SpectralTraceListWheel)
-    return any([isinstance(eff, spec_classes) for eff in effects])
+    return any(isinstance(eff, spec_classes) for eff in effects)
 
 
 def empty_surface_list(**kwargs):
     tbl = Table(names=["name", "outer", "inner", "angle",
                        "temperature", "action", "filename"],
                 data=[["test"], [0.], [0.], [0.], [0.], ["none"], ["none"]],
                 meta={"outer_unit": "m", "inner_unit": "m",
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/electronic.py` & `ScopeSim-0.6.0/scopesim/effects/electronic.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,27 +84,27 @@
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         params = {"z_order": [299, 900]}
         self.meta.update(params)
         self.meta.update(kwargs)
 
-        required_keys = ['mode_properties']
+        required_keys = ["mode_properties"]
         utils.check_keys(self.meta, required_keys, action="error")
 
-        self.mode_properties = kwargs['mode_properties']
+        self.mode_properties = kwargs["mode_properties"]
 
     def apply_to(self, obj, **kwargs):
-        mode_name = kwargs.get('detector_readout_mode',
+        mode_name = kwargs.get("detector_readout_mode",
                                from_currsys("!OBS.detector_readout_mode"))
         if isinstance(obj, ImagePlaneBase) and mode_name == "auto":
             mode_name = self.select_mode(obj, **kwargs)
             print("Detector mode set to", mode_name)
 
-        self.meta['detector_readout_mode'] = mode_name
+        self.meta["detector_readout_mode"] = mode_name
         props_dict = self.mode_properties[mode_name]
         rc.__currsys__["!OBS.detector_readout_mode"] = mode_name
         for key, value in props_dict.items():
             rc.__currsys__[key] = value
 
         return obj
 
@@ -177,21 +177,21 @@
         on the `ImagePlane`, mapped to the detector array.
         """
         super().__init__(**kwargs)
         params = {"z_order": [902]}
         self.meta.update(params)
         self.meta.update(kwargs)
 
-        required_keys = ['fill_frac', 'full_well', 'mindit']
+        required_keys = ["fill_frac", "full_well", "mindit"]
         utils.check_keys(self.meta, required_keys, action="error")
 
     def apply_to(self, obj, **kwargs):
         if isinstance(obj, (ImagePlaneBase, DetectorBase)):
             implane_max = np.max(obj.data)
-            exptime = kwargs.get('exptime', from_currsys("!OBS.exptime"))
+            exptime = kwargs.get("exptime", from_currsys("!OBS.exptime"))
             mindit = from_currsys(self.meta["mindit"])
 
             if exptime is None:
                 exptime = from_currsys("!OBS.dit") * from_currsys("!OBS.ndit")
             print(f"Requested exposure time: {exptime:.3f} s")
 
             if exptime < mindit:
@@ -215,16 +215,16 @@
                 print("Warning: The detector will be saturated!")
                 # ..todo: turn into proper warning
 
             print("Exposure parameters:")
             print(f"                DIT: {dit:.3f} s  NDIT: {ndit}")
             print(f"Total exposure time: {dit * ndit:.3f} s")
 
-            rc.__currsys__['!OBS.dit'] = dit
-            rc.__currsys__['!OBS.ndit'] = ndit
+            rc.__currsys__["!OBS.dit"] = dit
+            rc.__currsys__["!OBS.ndit"] = ndit
 
         return obj
 
 
 class SummedExposure(Effect):
     """
     Simulates a summed stack of ``ndit`` exposures
@@ -414,16 +414,16 @@
         if isinstance(obj, DetectorBase):
             if isinstance(from_currsys(self.meta["value"]), dict):
                 dtcr_id = obj.meta[utils.real_colname("id", obj.meta)]
                 dark = from_currsys(self.meta["value"][dtcr_id])
             elif isinstance(from_currsys(self.meta["value"]), float):
                 dark = from_currsys(self.meta["value"])
             else:
-                raise ValueError("<DarkCurrent>.meta['value'] must be either"
-                                 "dict or float: {}".format(self.meta["value"]))
+                raise ValueError("<DarkCurrent>.meta['value'] must be either "
+                                 f"dict or float, but is {self.meta['value']}")
 
             dit = from_currsys(self.meta["dit"])
             ndit = from_currsys(self.meta["ndit"])
 
             obj._hdu.data += dark * dit * ndit
 
         return obj
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/fits_headers.py` & `ScopeSim-0.6.0/scopesim/effects/fits_headers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-import yaml
 from copy import deepcopy
 import datetime
+
+import yaml
 import numpy as np
+
 from astropy.io import fits
 from astropy import units as u
 from astropy.table import Table
+
 from . import Effect
-from ..utils import check_keys, from_currsys, find_file
+from ..utils import from_currsys, find_file
 
 
 class ExtraFitsKeywords(Effect):
     """
     Extra FITS header keywords to be added to the pipeline FITS files
 
     These keywords are ONLY for keywords that should be MANUALLY ADDED to the
@@ -226,34 +229,34 @@
 
         tmp_dicts = []
         if self.meta["filename"] is not None:
             yaml_file = find_file(self.meta["filename"])
             with open(yaml_file) as f:
                 # possible multiple yaml docs in a file
                 # --> returns list even for a single doc
-                tmp_dicts += [dic for dic in yaml.full_load_all(f)]
+                tmp_dicts.extend(dic for dic in yaml.full_load_all(f))
 
         if self.meta["yaml_string"] is not None:
             yml = self.meta["yaml_string"]
-            tmp_dicts += [dic for dic in yaml.full_load_all(yml)]
+            tmp_dicts.extend(dic for dic in yaml.full_load_all(yml))
 
         if self.meta["header_dict"] is not None:
             if not isinstance(self.meta["header_dict"], list):
-                tmp_dicts += [self.meta["header_dict"]]
+                tmp_dicts.append(self.meta["header_dict"])
             else:
-                tmp_dicts += self.meta["header_dict"]
+                tmp_dicts.extend(self.meta["header_dict"])
 
         self.dict_list = []
         for dic in tmp_dicts:
             # format says yaml file contains list of dicts
             if isinstance(dic, list):
-                self.dict_list += dic
+                self.dict_list.extend(dic)
             # catch case where user forgets the list
             elif isinstance(dic, dict):
-                self.dict_list += [dic]
+                self.dict_list.append(dic)
 
     def apply_to(self, hdul, **kwargs):
         """
         Adds extra fits keywords from a yaml file including !,#-stings
 
         Parameters
         ----------
@@ -279,26 +282,26 @@
 
         return hdul
 
 
 def get_relevant_extensions(dic, hdul):
     exts = []
     if dic.get("ext_name") is not None:
-        exts += [i for i, hdu in enumerate(hdul)
-                 if hdu.header["EXTNAME"] == dic["ext_name"]]
+        exts.extend(i for i, hdu in enumerate(hdul)
+                    if hdu.header["EXTNAME"] == dic["ext_name"])
     elif dic.get("ext_number") is not None:
         ext_n = np.array(dic["ext_number"])
-        exts += list(ext_n[ext_n<len(hdul)])
+        exts.extend(ext_n[ext_n<len(hdul)])
     elif dic.get("ext_type") is not None:
         if isinstance(dic["ext_type"], list):
             ext_type_list = dic["ext_type"]
         else:
             ext_type_list = [dic["ext_type"]]
-        cls = tuple([getattr(fits, cls_str) for cls_str in ext_type_list])
-        exts += [i for i, hdu in enumerate(hdul) if isinstance(hdu, cls)]
+        cls = tuple(getattr(fits, cls_str) for cls_str in ext_type_list)
+        exts.extend(i for i, hdu in enumerate(hdul) if isinstance(hdu, cls))
 
     return exts
 
 
 def flatten_dict(dic, base_key="", flat_dict=None,
                  resolve=False, optics_manager=None):
     """
@@ -440,15 +443,15 @@
                     value = eff_meta[key]
                     if key in ["history", "notes", "changes"]:
                         eff_meta.pop(key)
                     if isinstance(value, Table):
                         eff_meta[key] = f"Table object of length: {len(value)}"
 
                 # add effect under the EFFn keyword
-                prefix = self.meta['keyword_prefix']
+                prefix = self.meta["keyword_prefix"]
                 class_name = opt_train[eff_name].__class__.__name__
                 self.dict_list = [{"ext_number": self.meta["ext_number"],
                                    "keywords": {
                                        f"{prefix} EFF{i} class": [class_name, "ScopeSim class name"],
                                        f"{prefix} EFF{i}": eff_meta}
                                    }]
                 super_apply_to = super(EffectsMetaKeywords, self).apply_to
@@ -493,48 +496,46 @@
                   "ext_number": [0],
                   "keyword_prefix": "HIERARCH SIM"}
         self.meta.update(params)
         self.meta.update(kwargs)
 
     def apply_to(self, hdul, **kwargs):
         opt_train = kwargs.get("optical_train")
-        if isinstance(hdul, fits.HDUList) and opt_train is not None:
-            src = opt_train._last_source
-            src_dicts = []
-            if src is not None:
-                prefix = self.meta['keyword_prefix']
-                for i, field in enumerate(src.fields):
-
-                    src_class = field.__class__.__name__
-                    src_dic = deepcopy(src._meta_dicts[i])
-                    if isinstance(field, fits.ImageHDU):
-                        hdr = field.header
-                        for key in hdr:
-                            src_dic = {key: [hdr[key], hdr.comments[key]]}
-
-                    elif isinstance(field, Table):
-                        src_dic.update(field.meta)
-                        src_dic["length"] = len(field)
-                        for j, name in enumerate(field.colnames):
-                            src_dic[f"col{j}_name"] = name
-                            src_dic[f"col{j}_unit"] = str(field[name].unit)
-
-                    self.dict_list = [{"ext_number": self.meta["ext_number"],
-                                       "keywords": {
-                                           f"{prefix} SRC{i} class": src_class,
-                                           f"{prefix} SRC{i}": src_dic}
-                                       }]
-                    super_apply_to = super(SourceDescriptionFitsKeywords, self).apply_to
-                    hdul = super_apply_to(hdul=hdul, optical_train=opt_train)
-
-            # catch the function call
-            for hdu in hdul:
-                for key in hdu.header:
-                    if "function_call" in key:
-                        hdu.header[f"FN{key.split()[1]}"] = hdu.header.pop(key)
+        if not isinstance(hdul, fits.HDUList) or opt_train is None:
+            return hdul
+
+        if (src := opt_train._last_source) is not None:
+            prefix = self.meta["keyword_prefix"]
+            for i, field in enumerate(src.fields):
+                src_class = field.__class__.__name__
+                src_dic = deepcopy(src._meta_dicts[i])
+                if isinstance(field, fits.ImageHDU):
+                    hdr = field.header
+                    for key in hdr:
+                        src_dic = {key: [hdr[key], hdr.comments[key]]}
+
+                elif isinstance(field, Table):
+                    src_dic.update(field.meta)
+                    src_dic["length"] = len(field)
+                    for j, name in enumerate(field.colnames):
+                        src_dic[f"col{j}_name"] = name
+                        src_dic[f"col{j}_unit"] = str(field[name].unit)
+
+                self.dict_list = [{"ext_number": self.meta["ext_number"],
+                                   "keywords": {
+                                       f"{prefix} SRC{i} class": src_class,
+                                       f"{prefix} SRC{i}": src_dic}
+                                   }]
+                hdul = super().apply_to(hdul=hdul, optical_train=opt_train)
+
+        # catch the function call
+        for hdu in hdul:
+            for key in hdu.header:
+                if "function_call" in key:
+                    hdu.header[f"FN{key.split()[1]}"] = hdu.header.pop(key)
 
         return hdul
 
 
 class SimulationConfigFitsKeywords(ExtraFitsKeywords):
     """
     Adds parameters from all config dictionaries to the FITS headers
@@ -580,15 +581,15 @@
         self.meta.update(params)
         self.meta.update(kwargs)
 
     def apply_to(self, hdul, **kwargs):
         opt_train = kwargs.get("optical_train")
         if isinstance(hdul, fits.HDUList) and opt_train is not None:
             cmds = opt_train.cmds.cmds.dic
-            sim_prefix = self.meta['keyword_prefix']
+            sim_prefix = self.meta["keyword_prefix"]
             resolve_prefix = "unresolved_" if not self.meta["resolve"] else ""
             # needed for the super().apply_to method
             self.dict_list = [{"ext_number": self.meta["ext_number"],
                                f"{resolve_prefix}keywords": {
                                    f"{sim_prefix} CONFIG": cmds}
                                }]
             super_apply_to = super(SimulationConfigFitsKeywords, self).apply_to
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/metis_lms_trace_list.py` & `ScopeSim-0.6.0/scopesim/effects/metis_lms_trace_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,83 +33,83 @@
     }
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         #self.params = {"wavelen": "!OBS.wavelen"}
         #self.params.update(kwargs)
 
-        self.wavelen = self.meta['wavelen']
+        self.wavelen = self.meta["wavelen"]
 
         # field of view of the instrument
         # ..todo: get this from aperture list
 
         self.slicelist = self._file["Aperture List"].data
-        #self.view = np.array([self.meta['naxis1'] * self.meta['pixscale'],
-        #                      self.meta['nslice'] * self.meta['slicewidth']])
-        self.view = np.array([self.slicelist['right'].max() -
-                              self.slicelist['left'].min(),
-                              self.slicelist['top'].max() -
-                              self.slicelist['bottom'].min()])
+        #self.view = np.array([self.meta["naxis1"] * self.meta["pixscale"],
+        #                      self.meta["nslice"] * self.meta["slicewidth"]])
+        self.view = np.array([self.slicelist["right"].max() -
+                              self.slicelist["left"].min(),
+                              self.slicelist["top"].max() -
+                              self.slicelist["bottom"].min()])
 
         #for sli, spt in enumerate(self.spectral_traces.values()):
-        #    spt.meta['xmin'] = self.slicelist['left'][sli]
-        #    spt.meta['xmax'] = self.slicelist['right'][sli]
-        #    spt.meta['ymin'] = self.slicelist['bottom'][sli]
-        #    spt.meta['ymax'] = self.slicelist['top'][sli]
+        #    spt.meta["xmin"] = self.slicelist["left"][sli]
+        #    spt.meta["xmax"] = self.slicelist["right"][sli]
+        #    spt.meta["ymin"] = self.slicelist["bottom"][sli]
+        #    spt.meta["ymax"] = self.slicelist["top"][sli]
 
         #if self._file is not None:
         #    print(self._file)
         #    self.make_spectral_traces()
 
     def apply_to(self, obj, **kwargs):
         """
         overrides SpectralTraceList.apply_to()
         """
         if isinstance(obj, FOVSetupBase):
             # Create a single volume that covers the aperture and
             # the maximum wavelength range of LMS
             volumes = [self.spectral_traces[key].fov_grid()
                        for key in self.spectral_traces]
-            wave_min = min([vol["wave_min"] for vol in volumes])
-            wave_max = max([vol["wave_max"] for vol in volumes])
+            wave_min = min(vol["wave_min"] for vol in volumes)
+            wave_max = max(vol["wave_max"] for vol in volumes)
             extracted_vols = obj.extract(axes=["wave"],
                                          edges=([[wave_min, wave_max]]))
             obj.volumes = extracted_vols
 
         if isinstance(obj, FieldOfViewBase):
             # Application to field of view
-            if obj.hdu is not None and obj.hdu.header['NAXIS'] == 3:
+            if obj.hdu is not None and obj.hdu.header["NAXIS"] == 3:
                 obj.cube = obj.hdu
             elif obj.hdu is None and obj.cube is None:
                 obj.cube = obj.make_cube_hdu()
 
             fovcube = obj.cube.data
             n_z, n_y, n_x = fovcube.shape
             fovwcs = WCS(obj.cube.header)
             # Make this linear to avoid jump at RA 0 deg
-            fovwcs.wcs.ctype = ['LINEAR', 'LINEAR', fovwcs.wcs.ctype[2]]
+            fovwcs.wcs.ctype = ["LINEAR", "LINEAR", fovwcs.wcs.ctype[2]]
             fovwcs_spat = fovwcs.sub(2)
-            ny_slice = self.meta['slice_samples'] #
+            ny_slice = self.meta["slice_samples"] #
 
             # Spatial pixel coordinates
             xslice, yslice = np.meshgrid(np.arange(n_x),
                                          np.arange(ny_slice))
 
-            fovimage = np.zeros((obj.detector_header['NAXIS2'],
-                                 obj.detector_header['NAXIS1']),
+            fovimage = np.zeros((obj.detector_header["NAXIS2"],
+                                 obj.detector_header["NAXIS1"]),
                                 dtype=np.float32)
 
 
             for sptid, spt in self.spectral_traces.items():
-                ymin = spt.meta['fov']['y_min']
-                ymax = spt.meta['fov']['y_max']
+                ymin = spt.meta["fov"]["y_min"]
+                ymax = spt.meta["fov"]["y_max"]
 
                 slicewcs = deepcopy(fovwcs)
 
-                slicewcs.wcs.ctype = ['LINEAR', 'LINEAR', slicewcs.wcs.ctype[2]]
+                slicewcs.wcs.ctype = ["LINEAR", "LINEAR", slicewcs.wcs.ctype[2]]
                 slicewcs.wcs.crpix[1] = (ny_slice + 1) / 2
                 slicewcs.wcs.crval[1] = (ymin + ymax) / 2 / 3600
                 slicewcs.wcs.cdelt[1] = (ymax - ymin) / ny_slice / 3600
                 slicewcs_spat = slicewcs.sub(2)
 
                 # World coordinates for the slice
                 xworld, yworld = slicewcs_spat.all_pix2world(xslice,
@@ -121,60 +121,60 @@
                 for islice in range(n_z):
                     ifov = RectBivariateSpline(np.arange(n_y),
                                                np.arange(n_x),
                                                fovcube[islice], kx=1, ky=1)
                     slicecube[islice] = ifov(yfov, xfov, grid=False)
 
                 slicefov = FieldOfView(obj.header,
-                                       [obj.meta['wave_min'], obj.meta['wave_max']])
+                                       [obj.meta["wave_min"], obj.meta["wave_max"]])
                 slicefov.detector_header = obj.detector_header
-                slicefov.meta['xi_min'] = obj.meta['xi_min']
-                slicefov.meta['xi_max'] = obj.meta['xi_max']
-                slicefov.meta['trace_id'] = sptid
+                slicefov.meta["xi_min"] = obj.meta["xi_min"]
+                slicefov.meta["xi_max"] = obj.meta["xi_max"]
+                slicefov.meta["trace_id"] = sptid
                 slicefov.cube = fits.ImageHDU(header=slicewcs.to_header(),
                                               data=slicecube)
                 #slicefov.cube.writeto(f"slicefov_{sptid}.fits", overwrite=True)
                 slicefov.hdu = spt.map_spectra_to_focal_plane(slicefov)
 
-                sxmin = slicefov.hdu.header['XMIN']
-                sxmax = slicefov.hdu.header['XMAX']
-                symin = slicefov.hdu.header['YMIN']
-                symax = slicefov.hdu.header['YMAX']
+                sxmin = slicefov.hdu.header["XMIN"]
+                sxmax = slicefov.hdu.header["XMAX"]
+                symin = slicefov.hdu.header["YMIN"]
+                symax = slicefov.hdu.header["YMAX"]
                 fovimage[symin:symax, sxmin:sxmax] += slicefov.hdu.data
 
             obj.hdu = fits.ImageHDU(data=fovimage, header=obj.detector_header)
 
         return obj
 
     def make_spectral_traces(self):
         """
         Compute the transformations by interpolation
         """
-        #nslice = len(self._file['Aperture List'].data)
+        #nslice = len(self._file["Aperture List"].data)
         # determine echelle order and angle from specified wavelength
         tempres = self._angle_from_lambda()
-        self.meta['order'] = tempres['Ord']
-        self.meta['angle'] = tempres['Angle']
+        self.meta["order"] = tempres["Ord"]
+        self.meta["angle"] = tempres["Angle"]
 
         spec_traces = {}
-        for sli in np.arange(self.meta['nslice']):
+        for sli in np.arange(self.meta["nslice"]):
             slicename = "Slice " + str(sli + 1)
             spec_traces[slicename] = MetisLMSSpectralTrace(
                 self._file,
                 spslice=sli, params=self.meta)
 
         self.spectral_traces = spec_traces
 
     def _angle_from_lambda(self):
         """
         Determine optimal echelle rotation angle for wavelength
         """
-        lam = from_currsys(self.meta['wavelen'])
-        grat_spacing = self.meta['grat_spacing']
-        wcal = self._file['WCAL'].data
+        lam = from_currsys(self.meta["wavelen"])
+        grat_spacing = self.meta["grat_spacing"]
+        wcal = self._file["WCAL"].data
         return echelle_setting(lam, grat_spacing, wcal)
 
 
 class MetisLMSSpectralTrace(SpectralTrace):
     """
     SpectralTrace for the METIS LM spectrograph
     """
@@ -184,71 +184,71 @@
         "slicewidth": 0.0207,  # arcsec
         "pixscale": 0.0082,    # arcsec
         "grat_spacing": 18.2,
         "plate_scale": 0.303,
     }
 
     def __init__(self, hdulist, spslice, params, **kwargs):
-        polyhdu = hdulist['Polynomial coefficients']
+        polyhdu = hdulist["Polynomial coefficients"]
         params.update(kwargs)
-        params['aperture_id'] = spslice
-        params['slice'] = spslice
+        params["aperture_id"] = spslice
+        params["slice"] = spslice
         super().__init__(polyhdu, **params)
 
         self._file = hdulist
-        self.meta['description'] = "Slice " + str(spslice + 1)
-        self.meta['trace_id'] = f"Slice {spslice + 1}"
+        self.meta["description"] = "Slice " + str(spslice + 1)
+        self.meta["trace_id"] = f"Slice {spslice + 1}"
         self.meta.update(params)
         # Provisional:
-        self.meta['fov'] = self.fov_grid()
+        self.meta["fov"] = self.fov_grid()
 
     def fov_grid(self):
         """
         Provide information on the source space volume required by the effect
 
         Returns
         -------
         A dictionary with entries `wave_min` and `wave_max`, `x_min`, `y_min`,
         `x_max`, `y_max`. Spatial limits refer to the sky and are given in
         arcsec.
         """
 
-        aperture = self._file['Aperture list'].data[self.meta['slice']]
-        x_min = aperture['left']
-        x_max = aperture['right']
-        y_min = aperture['bottom']
-        y_max = aperture['top']
-        trace_id = self.meta['trace_id']
+        aperture = self._file["Aperture list"].data[self.meta["slice"]]
+        x_min = aperture["left"]
+        x_max = aperture["right"]
+        y_min = aperture["bottom"]
+        y_max = aperture["top"]
+        trace_id = self.meta["trace_id"]
 
         layout = ioascii.read(find_file("!DET.layout.file_name"))
         det_lims = {}
-        xhw = layout['pixel_size'] * layout['x_size'] / 2
-        yhw = layout['pixel_size'] * layout['y_size'] / 2
-        det_lims['xd_min'] = min(layout['x_cen'] - xhw)
-        det_lims['xd_max'] = max(layout['x_cen'] + xhw)
-        det_lims['yd_min'] = min(layout['y_cen'] - yhw)
-        det_lims['yd_max'] = max(layout['y_cen'] + yhw)
+        xhw = layout["pixel_size"] * layout["x_size"] / 2
+        yhw = layout["pixel_size"] * layout["y_size"] / 2
+        det_lims["xd_min"] = min(layout["x_cen"] - xhw)
+        det_lims["xd_max"] = max(layout["x_cen"] + xhw)
+        det_lims["yd_min"] = min(layout["y_cen"] - yhw)
+        det_lims["yd_max"] = max(layout["y_cen"] + yhw)
         wave_min, wave_max = self.get_waverange(det_lims)
 
         # ..todo: just a hack - xi and x are the same except xi is a quantity
         xi_min = quantify(x_min, u.arcsec)
         xi_max = quantify(x_max, u.arcsec)
 
         return {"x_min": x_min, "x_max": x_max,
                 "y_min": y_min, "y_max": y_max,
                 "xi_min": xi_min, "xi_max": xi_max,
                 "wave_min": wave_min, "wave_max": wave_max,
                 "trace_id": trace_id}
 
     def get_waverange(self, det_mm_lims):
         """Determine wavelength range that spectral trace covers on image plane"""
-        xmin = det_mm_lims['xd_min']
-        xmax = det_mm_lims['xd_max']
+        xmin = det_mm_lims["xd_min"]
+        xmax = det_mm_lims["xd_max"]
 
-        lam0 = from_currsys(self.meta['wavelen'])
+        lam0 = from_currsys(self.meta["wavelen"])
         xi0 = 0.
         ymid = self.xilam2y(xi0, lam0)[0]   # estimate y level of trace
 
         waverange = self.xy2lam(np.array([xmin, xmax]), np.array([ymid, ymid]),
                                 grid=False)
 
         return waverange.min(), waverange.max()
@@ -259,23 +259,23 @@
         The LMS transforms actually operate on phase rather than
         wavelength, hence the necessity of defining pre- and
         posttransforms on the lam variable.
         """
         matrices = self.get_matrices()
         # matrices are transposed to align argument sequence
         # with the name of the functions
-        self.xilam2x = Transform2D(matrices['A'].T,
+        self.xilam2x = Transform2D(matrices["A"].T,
                                    pretransform_x=self.sky2fp,
                                    pretransform_y=self.lam2phase)
-        self.xilam2y = Transform2D(matrices['B'].T,
+        self.xilam2y = Transform2D(matrices["B"].T,
                                    pretransform_x=self.sky2fp,
                                    pretransform_y=self.lam2phase)
-        self.xy2lam = Transform2D(matrices['AI'],
+        self.xy2lam = Transform2D(matrices["AI"],
                                   posttransform=self.phase2lam)
-        self.xy2xi = Transform2D(matrices['BI'],
+        self.xy2xi = Transform2D(matrices["BI"],
                                  posttransform=self.fp2sky)
 
 
     def get_matrices(self):
         """
         Extract matrix from lms_dist_poly.txt
 
@@ -291,37 +291,37 @@
         angle : float
             Grism angle in degrees
 
         Returns
         -------
         dict of four np.arrays of shape (4, 4) each
         """
-        spslice = self.meta['slice']
-        order = self.meta['order']
-        angle = self.meta['angle']
-        matnames = ['A', 'B', 'AI', 'BI']
+        spslice = self.meta["slice"]
+        order = self.meta["order"]
+        angle = self.meta["angle"]
+        matnames = ["A", "B", "AI", "BI"]
         matrices = {}
 
         poly = self.table
         for matid in range(4):
-            select = ((poly['Ord'] == order) *
-                      (poly['Sli'] == spslice) *
-                      (poly['Mat'] == matid))
+            select = ((poly["Ord"] == order) *
+                      (poly["Sli"] == spslice) *
+                      (poly["Mat"] == matid))
             if not np.any(select):
                 raise KeyError("Combination of Order, Slice not found")
 
             subpoly = poly[select]
             thematrix = np.zeros((4, 4))
             for i in range(4):
                 for j in range(4):
-                    sel_ij = (subpoly['Row'] == i) * (subpoly['Col'] == j)
-                    thematrix[i, j] = (subpoly['A11'][sel_ij] * angle**3 +
-                                       subpoly['A12'][sel_ij] * angle**2 +
-                                       subpoly['A21'][sel_ij] * angle +
-                                       subpoly['A22'][sel_ij])
+                    sel_ij = (subpoly["Row"] == i) * (subpoly["Col"] == j)
+                    thematrix[i, j] = (subpoly["A11"][sel_ij] * angle**3 +
+                                       subpoly["A12"][sel_ij] * angle**2 +
+                                       subpoly["A21"][sel_ij] * angle +
+                                       subpoly["A22"][sel_ij])
             matrices[matnames[matid]] = thematrix
 
         return matrices
 
 
     def lam2phase(self, lam):
         """
@@ -334,15 +334,15 @@
         lam : ndarray (float)
             wavelength (um)
 
         Returns
         -------
         Phase : ndarray
         """
-        return self.meta['order'] * lam / (2 * self.meta['grat_spacing'])
+        return self.meta["order"] * lam / (2 * self.meta["grat_spacing"])
 
     def phase2lam(self, phase):
         """
         Convert phase to wavelength
 
         Wavelength is phase * 2 * grat_spacing / order
 
@@ -351,35 +351,37 @@
         phase : ndarray (float)
             phase (dimensionless)
 
         Returns
         -------
         wavelength : ndarray (um)
         """
-        return 2 * self.meta['grat_spacing'] * phase / self.meta['order']
+        return 2 * self.meta["grat_spacing"] * phase / self.meta["order"]
 
     def sky2fp(self, xi):
         """
         Convert position in arcsec to position in FP2
         """
-        return xi / self.meta['plate_scale']
+        return xi / self.meta["plate_scale"]
 
     def fp2sky(self, fp_x):
         """
         Convert position in FP2 to position on sky
         """
-        return fp_x * self.meta['plate_scale']
-
+        return fp_x * self.meta["plate_scale"]
 
     def __repr__(self):
-        msg = '<MetisLMSSpectralTrace> "{}" : {} um : Order {} : Angle {}'\
-            ''.format(self.meta["description"],
-                      from_currsys(self.meta["wavelen"]),
-                      self.meta["order"],
-                      self.meta["angle"])
+        msg = (f"{self.__class__.__name__}({self._file!r}, "
+               f"{self.meta['slice']!r}, {self.meta!r})")
+        return msg
+
+    def __str__(self):
+        msg = (f"<MetisLMSSpectralTrace> \"{self.meta['description']}\" : "
+               f"{from_currsys(self.meta['wavelen'])} um : "
+               f"Order {self.meta['order']} : Angle {self.meta['angle']}")
         return msg
 
 
 def echelle_setting(wavelength, grat_spacing, wcal_def):
     """
     Determine optimal echelle rotation angle for wavelength
 
@@ -406,26 +408,26 @@
     elif isinstance(wcal_def, (fits.TableHDU, fits.BinTableHDU)):
         # Read wcal extension of layout file
         wcal = wcal_def.data
     elif isinstance(wcal_def, Table):
         wcal = wcal_def
     elif isinstance(wcal_def, str):
         try:
-            wcal = fits.getdata(wcal_def, extname='WCAL')
+            wcal = fits.getdata(wcal_def, extname="WCAL")
         except OSError:
             wcal = ioascii.read(wcal_def, comment="^#", format="csv")
     else:
         raise TypeError("wcal_def not in recognised format:", wcal_def)
 
     # Compute angles, determine which order gives angle closest to zero
-    angles = wcal['c0'] * wavelength + wcal['c1']
+    angles = wcal["c0"] * wavelength + wcal["c1"]
     imin = np.argmin(np.abs(angles))
 
     # Extract parameters
-    order = wcal['Ord'][imin]
+    order = wcal["Ord"][imin]
     angle = angles[imin]
 
     # Compute the phase corresponding to the wavelength
     phase = wavelength * order / (2 * grat_spacing)
 
     return {"Ord": order, "Angle": angle, "Phase": phase}
 
@@ -439,21 +441,21 @@
     The effect differs from its parent class `ApertureMask` in the initialisation
     from the `Aperture List` extension of the trace file `!OBS.trace_file`.
     """
     def __init__(self, filename, ext_id="Aperture List", **kwargs):
         filename = find_file(from_currsys(filename))
         ap_hdr = fits.getheader(filename, extname=ext_id)
         ap_list = fits.getdata(filename, extname=ext_id)
-        xmin, xmax = ap_list['left'].min(), ap_list['right'].max()
-        ymin, ymax = ap_list['bottom'].min(), ap_list['top'].max()
+        xmin, xmax = ap_list["left"].min(), ap_list["right"].max()
+        ymin, ymax = ap_list["bottom"].min(), ap_list["top"].max()
         slicer_dict = {"x": [xmin, xmax, xmax, xmin],
                        "y": [ymin, ymin, ymax, ymax]}
         try:
-            kwargs["x_unit"] = ap_hdr['X_UNIT']
-            kwargs["y_unit"] = ap_hdr['Y_UNIT']
+            kwargs["x_unit"] = ap_hdr["X_UNIT"]
+            kwargs["y_unit"] = ap_hdr["Y_UNIT"]
         except KeyError:
             pass
 
         super().__init__(array_dict=slicer_dict, id="LMS slicer",
                          conserve_image=True, **kwargs)
 
 
@@ -471,43 +473,43 @@
         "eff_max": 0.75
     }
 
     def __init__(self, **kwargs):
         self.meta = self._class_params
         self.meta.update(kwargs)
 
-        filename = find_file(self.meta['filename'])
-        wcal = fits.getdata(filename, extname='WCAL')
-        if 'wavelen' in kwargs:
-            wavelen = from_currsys(kwargs['wavelen'])
-            grat_spacing = self.meta['grat_spacing']
+        filename = find_file(self.meta["filename"])
+        wcal = fits.getdata(filename, extname="WCAL")
+        if "wavelen" in kwargs:
+            wavelen = from_currsys(kwargs["wavelen"])
+            grat_spacing = self.meta["grat_spacing"]
             ech = echelle_setting(wavelen, grat_spacing, wcal)
-            self.meta['order'] = ech['Ord']
+            self.meta["order"] = ech["Ord"]
         else:
             wavelen = None
 
         lam, efficiency = self.make_ter_curve(wcal, wavelen)
 
         super().__init__(wavelength=lam,
                          transmission=efficiency,
                          emissivity=np.zeros_like(lam),
                          **self.meta)
 
     def make_ter_curve(self, wcal, wavelen=None):
         """Compute the blaze function for the selected order"""
-        order = self.meta['order']
-        eff_wid = self.meta['eff_wid']
-        eff_max = self.meta['eff_max']
+        order = self.meta["order"]
+        eff_wid = self.meta["eff_wid"]
+        eff_max = self.meta["eff_max"]
 
-        wcal_ord = wcal[wcal['Ord'] == self.meta['order']]
+        wcal_ord = wcal[wcal["Ord"] == self.meta["order"]]
 
         if wavelen is not None:
             lam = np.linspace(wavelen - 0.2, wavelen + 0.2, 1001)
-            angle = wcal_ord['c0'] * lam + wcal_ord['c1']
+            angle = wcal_ord["c0"] * lam + wcal_ord["c1"]
         else:
             angle = np.linspace(7, -7, 10001)
-            lam = wcal_ord['ic0'] * angle + wcal_ord['ic1']
+            lam = wcal_ord["ic0"] * angle + wcal_ord["ic1"]
 
         phase = order * np.pi * np.sin(np.deg2rad(angle)) * eff_wid
         efficiency = eff_max * np.sinc(phase / np.pi)**2
 
         return lam, efficiency
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/obs_strategies.py` & `ScopeSim-0.6.0/scopesim/effects/obs_strategies.py`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/effects/psf_utils.py` & `ScopeSim-0.6.0/scopesim/effects/psf_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,17 +60,17 @@
 
     strehl_map = strehl_hdu.data
 
     nms_spline = RectBivariateSpline(ws, nms, strehl_map, kx=1, ky=1)
     strehls = nms_spline(wavelength, nms)[0]
 
     if strehl > np.max(strehls):
-        raise ValueError("Strehl ratio ({}) is impossible at this wavelength "
-                         "({}). Maximum Strehl possible is {}."
-                         "".format(strehl, wavelength, np.max(strehls)))
+        raise ValueError(f"Strehl ratio ({strehl}) is impossible at this "
+                         f"wavelength ({wavelength}). Maximum Strehl possible "
+                         f"is {np.max(strehls)}.")
 
     if strehls[0] < strehls[-1]:
         nm = np.interp(strehl, strehls, nms)
     else:
         nm = np.interp(strehl, strehls[::-1], nms[::-1])
 
     if plot:
@@ -174,16 +174,15 @@
     Returns
     -------
     wave_set, wave_ext
 
     """
 
     if not isinstance(hdu_list, fits.HDUList):
-        raise ValueError("psf_effect must be a PSF object: {}"
-                         "".format(type(hdu_list)))
+        raise ValueError(f"psf_effect must be a PSF object: {type(hdu_list)}")
 
     tmp = np.array([[ii, hdu.header[wave_key]]
                     for ii, hdu in enumerate(hdu_list)
                     if wave_key in hdu.header and hdu.data is not None])
     wave_ext = tmp[:, 0].astype(int)
     wave_set = tmp[:, 1]
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/psfs.py` & `ScopeSim-0.6.0/scopesim/effects/psfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from copy import deepcopy
 import numpy as np
 from scipy.signal import convolve
 from scipy.interpolate import RectBivariateSpline
 
 from astropy import units as u
 from astropy.io import fits
 from astropy.convolution import Gaussian2DKernel
@@ -135,15 +134,15 @@
 
     def plot(self, obj=None, **kwargs):
         import matplotlib.pyplot as plt
         from matplotlib.colors import LogNorm
         plt.gcf().clf()
 
         kernel = self.get_kernel(obj)
-        plt.imshow(kernel, norm=LogNorm(), origin='lower', **kwargs)
+        plt.imshow(kernel, norm=LogNorm(), origin="lower", **kwargs)
 
         return plt.gcf()
 
 
 
 ################################################################################
 # Analytical PSFs - Vibration, Seeing, NCPAs
@@ -254,16 +253,16 @@
         wave_min, wave_max = utils.from_currsys([self.meta["wave_min"],
                                                  self.meta["wave_max"]])
         waves = np.linspace(wave_min, wave_max, 1001) * u.um
         wfe = self.total_wfe
         strehl = pu.wfe2strehl(wfe=wfe, wave=waves)
 
         plt.plot(waves, strehl)
-        plt.xlabel("Wavelength [{}]".format(waves.unit))
-        plt.ylabel("Strehl Ratio \n[Total WFE = {}]".format(wfe))
+        plt.xlabel(f"Wavelength [{waves.unit}]")
+        plt.ylabel(f"Strehl Ratio \n[Total WFE = {wfe}]")
 
         return plt.gcf()
 
 
 class SeeingPSF(AnalyticalPSF):
     """
     Currently only returns gaussian kernel with a ``fwhm`` [arcsec]
@@ -515,66 +514,66 @@
         pixel_scale = utils.from_currsys("!INST.pixel_scale")
 
         kernel = self.get_kernel(pixel_scale)
         # subplot2grid((n_vert, n_horiz), (from_top, from_left), colspan=1, rowspan=1)
         plt.subplot2grid((2, 2), (0, 0))
         im = kernel
         r_sky = pixel_scale * im.shape[0]
-        plt.imshow(im, norm=LogNorm(), origin='lower',
+        plt.imshow(im, norm=LogNorm(), origin="lower",
                    extent= [-r_sky, r_sky, -r_sky, r_sky], **kwargs)
         plt.ylabel("[arcsec]")
 
         plt.subplot2grid((2, 2), (0, 1))
         x = kernel.shape[1] // 2
         y = kernel.shape[0] // 2
         r = 16
         im = kernel[y-r:y+r, x-r:x+r]
         r_sky = pixel_scale * im.shape[0]
-        plt.imshow(im, norm=LogNorm(), origin='lower',
+        plt.imshow(im, norm=LogNorm(), origin="lower",
                    extent= [-r_sky, r_sky, -r_sky, r_sky], **kwargs)
         plt.ylabel("[arcsec]")
-        plt.gca().yaxis.set_label_position('right')
+        plt.gca().yaxis.set_label_position("right")
 
         plt.subplot2grid((2, 2), (1, 0), colspan=2)
         hdr = self._file[0].header
         data = self._file[0].data
 
         hdr = self._file[0].header
         data = self._file[0].data
 
         wfes = np.arange(hdr["NAXIS1"]) * hdr["CDELT1"] + hdr["CRVAL1"]
         waves = np.arange(hdr["NAXIS2"]) * hdr["CDELT2"] + hdr["CRVAL2"]
         for i in np.arange(len(waves))[::-1]:
             plt.plot(wfes, data[i, :],
-                     label=r"{} $\mu m$".format(round(waves[i], 3)))
+                     label=f"{waves[i]:.3f} " + r"$\mu m$")
 
         plt.xlabel("RMS Wavefront Error [um]")
         plt.ylabel("Strehl Ratio")
         plt.legend()
 
         return plt.gcf()
 
 
 
 ################################################################################
-# Discrete PSFs - MAORY and co PSFs
+# Discrete PSFs - MORFEO and co PSFs
 
 
 class DiscretePSF(PSF):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.meta["z_order"] = [43]
         self.convolution_classes = FieldOfViewBase
         # self.convolution_classes = ImagePlaneBase
 
 
 class FieldConstantPSF(DiscretePSF):
     """A PSF that is constant across the field.
 
-    For spectroscopy, the a wavelength-dependent PSF cube is built, where for each
+    For spectroscopy, a wavelength-dependent PSF cube is built, where for each
     wavelength the reference PSF is scaled proportional to wavelength.
     """
     def __init__(self, **kwargs):
         # sub_pixel_flag and flux_accuracy are taken care of in PSF base class
         super().__init__(**kwargs)
 
         self.required_keys = ["filename"]
@@ -595,15 +594,15 @@
     #   Taken care of by PSF base class
 
     def get_kernel(self, fov):
         """Find nearest wavelength and build PSF kernel from file"""
         ii = pu.nearest_index(fov.wavelength, self._waveset)
         ext = self.kernel_indexes[ii]
         if ext != self.current_layer_id:
-            if fov.hdu.header['NAXIS'] == 3:
+            if fov.hdu.header["NAXIS"] == 3:
                 self.current_layer_id = ext
                 self.make_psf_cube(fov)
             else:
                 self.kernel = self._file[ext].data
                 self.current_layer_id = ext
                 hdr = self._file[ext].header
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/rotation.py` & `ScopeSim-0.6.0/scopesim/effects/rotation.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from ..base_classes import DetectorBase
 
 
 class Rotate90CCD(Effect):
     """
     Rotates CCD by integer multiples of 90 degrees
     rotations kwarg is number of counter-clockwise rotations
+    
+    Author: Dave jones
 
     """
     def __init__(self, **kwargs):
         super(Rotate90CCD, self).__init__(**kwargs)
         params = {"z_order": [809]}
         self.meta.update(params)
         self.meta.update(kwargs)
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/shifts.py` & `ScopeSim-0.6.0/scopesim/effects/shifts.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,15 @@
         return obj
 
     def fov_grid(self, which="shifts", **kwargs):
         if which == "shifts":
             col_names = ["wavelength", "dx", "dy"]
             waves, dx, dy = [self.get_table(**kwargs)[col] for col in col_names]
             return waves, dx, dy
-        else:
-            return None
+        return None
 
     def get_table(self, **kwargs):
         if self.table is None:
             names = ["wavelength", "dx", "dy"]
             waves = from_currsys(["!SIM.spectral.wave_" + key
                                   for key in ("min", "mid", "max")])
             tbl = Table(names=names, data=[waves, [0] * 3, [0] * 3])
@@ -41,16 +40,16 @@
     def plot(self):
         import matplotlib.pyplot as plt
         plt.gcf().clf()
 
         tbl = self.get_table()
         plt.scatter(x=tbl["dx"], y=tbl["dy"], c=tbl["wavelength"])
         plt.colorbar()
-        plt.xlabel("dx [{}]".format(quantify(tbl["dx"], u.arcsec).unit))
-        plt.ylabel("dy [{}]".format(quantify(tbl["dy"], u.arcsec).unit))
+        plt.xlabel(f"dx [{quantify(tbl['dx'], u.arcsec).unit}]")
+        plt.ylabel(f"dy [{quantify(tbl['dy'], u.arcsec).unit}]")
         plt.axvline(0, ls=":")
         plt.axhline(0, ls=":")
         # plt.gca().set_aspect("equal")
 
         return plt.gcf()
 
 
@@ -219,16 +218,15 @@
         kwargs.update(self.meta)
         if "quick_adc" in self.meta:
             ad = AtmosphericDispersion(**self.meta)
             waves, dx, dy = ad.fov_grid()
             dx *= -(1 - self.meta["efficiency"])
             dy *= -(1 - self.meta["efficiency"])
             return waves, dx, dy
-        else:
-            return None
+        return None
 
     def plot(self):
         return None
 
 
 def atmospheric_refraction(lam, z0=60, temp=0, rel_hum=60, pres=750,
                            lat=-24.5, h=3064):
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/spectral_trace_list.py` & `ScopeSim-0.6.0/scopesim/effects/spectral_trace_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """
 Effect for mapping spectral cubes to the detector plane
 
-The Effect is called SpectralTraceList, it applies a list of
-optics.spectral_trace_SpectralTrace objects to a FieldOfView.
+The Effect is called `SpectralTraceList`, it applies a list of
+`spectral_trace_list_utils.SpectralTrace` objects to a `FieldOfView`.
 """
 
-from os import path as pth
+from pathlib import Path
+import logging
+
 import numpy as np
 
 from astropy.io import fits
 from astropy.table import Table
 
 from .effects import Effect
-from .spectral_trace_list_utils import SpectralTrace
-from ..utils import from_currsys, check_keys, interp2
+from .ter_curves import FilterCurve
+from .spectral_trace_list_utils import SpectralTrace, make_image_interpolations
+from ..utils import from_currsys, check_keys
 from ..optics.image_plane_utils import header_from_list_of_xy
 from ..base_classes import FieldOfViewBase, FOVSetupBase
 
 
 class SpectralTraceList(Effect):
     """
     List of spectral trace geometries for the detector plane
@@ -57,25 +60,29 @@
 
     EXT 1 : BinTableHDU : Overview of traces
     ++++++++++++++++++++++++++++++++++++++++
     No special header keywords are required in this extension
 
     Required Table columns:
 
-    - description : str : description of each each trace
+    - description : str : identifier of each trace
     - extension_id : int : which extension is each trace in
     - aperture_id : int : which aperture matches this trace (e.g. MOS / IFU)
     - image_plane_id : int : on which image plane is this trace projected
 
     EXT 2 : BinTableHDU : Individual traces
     +++++++++++++++++++++++++++++++++++++++
-    No special header keywords are required in this extension
+    Required header keywords:
+    - EXTNAME : must be identical to the `description` in EXT 1
 
-    Required Table columns:
+    Recommended header keywords:
+    - DISPDIR : 'x' or 'y' : dispersion axis. If not present, Scopesim tries
+      to determine this automatically; this may be unreliable in some cases.
 
+    Required Table columns:
     - wavelength : float : [um] : wavelength of monochromatic aperture image
     - s : float : [arcsec] : position along aperture perpendicular to trace
     - x : float : [mm] : x position of aperture image on focal plane
     - y : float : [mm] : y position of aperture image on focal plane
 
     """
     _class_params = {"x_colname": "x",
@@ -93,14 +100,15 @@
 
         if "hdulist" in kwargs and isinstance(kwargs["hdulist"], fits.HDUList):
             self._file = kwargs["hdulist"]
 
         params = {"z_order": [70, 270, 670],
                   "pixel_scale": "!INST.pixel_scale",  # [arcsec / pix]}
                   "plate_scale": "!INST.plate_scale",  # [arcsec / mm]
+                  "spectral_bin_width": "!SIM.spectral.spectral_bin_width", # [um]
                   "wave_min": "!SIM.spectral.wave_min",  # [um]
                   "wave_mid": "!SIM.spectral.wave_mid",  # [um]
                   "wave_max": "!SIM.spectral.wave_max",  # [um]
                   "x_colname": "x",
                   "y_colname": "y",
                   "s_colname": "s",
                   "wave_colname": "wavelength",
@@ -180,42 +188,23 @@
             if obj.hdu is not None and obj.hdu.header["NAXIS"] == 3:
                 obj.cube = obj.hdu
             elif obj.hdu is not None and obj.hdu.header["NAXIS"] == 2:
                 # todo: catch the case of obj.hdu.header["NAXIS"] == 2
                 # for MAAT
                 pass
             elif obj.hdu is None and obj.cube is None:
+                logging.info("Making cube")
                 obj.cube = obj.make_cube_hdu()
 
-            # ..todo: obj will be changed to a single one covering the full field of view
-            # covered by the image slicer (28 slices for LMS; for LSS still only a single slit)
-            # We need a loop over spectral_traces that chops up obj into the single-slice fov before
-            # calling map_spectra...
-            trace_id = obj.meta['trace_id']
+            trace_id = obj.meta["trace_id"]
             spt = self.spectral_traces[trace_id]
             obj.hdu = spt.map_spectra_to_focal_plane(obj)
 
         return obj
 
-    def get_waveset(self, pixel_size=None):
-        if pixel_size is None:
-            pixel_size = self.meta["pixel_scale"] / self.meta["plate_scale"]
-
-        wavesets = [spt.get_pixel_wavelength_edges(pixel_size)
-                    for spt in self.spectral_traces]
-
-        return wavesets
-
-    def get_fov_headers(self, sky_header, **kwargs):
-        fov_headers = []
-        for spt in self.spectral_traces:
-            fov_headers += spt.fov_headers(sky_header=sky_header, **kwargs)
-
-        return fov_headers
-
 
     @property
     def footprint(self):
         """Return the footprint of the entire SpectralTraceList"""
         xfoot, yfoot = [], []
         for spt in self.spectral_traces.values():
             xtrace, ytrace = spt.footprint()
@@ -231,14 +220,108 @@
     def image_plane_header(self):
         x, y = self.footprint
         pixel_scale = from_currsys(self.meta["pixel_scale"])
         hdr = header_from_list_of_xy(x, y, pixel_scale, "D")
 
         return hdr
 
+    def rectify_traces(self, hdulist, xi_min=None, xi_max=None, interps=None,
+                       **kwargs):
+        """Create rectified 2D spectra for all traces in the list
+
+        This method creates an HDU list with one extension per spectral
+        trace, i.e. it essentially treats all traces independently.
+        For the case of an IFU where the traces correspond to spatial
+        slices for the same wavelength range, use method `rectify_cube`
+        (not yet implemented).
+
+        Parameters
+        ----------
+        hdulist : str or fits.HDUList
+           The result of scopesim readout()
+        xi_min, xi_max : float [arcsec]
+           Spatial limits of the slit on the sky. This should be taken
+           from the header of the hdulist, but this is not yet provided by
+           scopesim. For the time being, these limits *must* be provided by
+           the user.
+        interps :  list of interpolation functions
+           If provided, there must be one for each image extension in `hdulist`.
+           The functions go from pixels to the images and can be created with,
+           e.g., RectBivariateSpline.
+        """
+        try:
+            inhdul = fits.open(hdulist)
+        except TypeError:
+            inhdul = hdulist
+
+        # Crude attempt to get a useful wavelength range
+        # Problematic because different instruments use different
+        # keywords for the filter... We try to make it work for METIS
+        # and MICADO for the time being.
+        try:
+            filter_name = from_currsys("!OBS.filter_name")
+        except ValueError:
+            filter_name = from_currsys("!OBS.filter_name_fw1")
+
+        filtcurve = FilterCurve(
+            filter_name=filter_name,
+            filename_format=from_currsys("!INST.filter_file_format"))
+        filtwaves = filtcurve.table['wavelength']
+        filtwave = filtwaves[filtcurve.table['transmission'] > 0.01]
+        wave_min, wave_max = min(filtwave), max(filtwave)
+        logging.info("Full wavelength range: %.02f .. %.02f um",
+                     wave_min, wave_max)
+
+        if xi_min is None or xi_max is None:
+            try:
+                xi_min = inhdul[0].header["HIERARCH INS SLIT XIMIN"]
+                xi_max = inhdul[0].header["HIERARCH INS SLIT XIMAX"]
+                logging.info(
+                    "Slit limits taken from header: %.02f .. %.02f arcsec",
+                    xi_min, xi_max)
+            except KeyError:
+                logging.error("""
+                Spatial slit limits (in arcsec) must be provided:
+                - either as method parameters xi_min and xi_max
+                - or as header keywords HIERARCH INS SLIT XIMIN/XIMAX
+                """)
+                return None
+
+
+        bin_width = kwargs.get("bin_width", None)
+
+        if interps is None:
+            logging.info("Computing interpolation functions")
+            interps = make_image_interpolations(hdulist)
+
+        pdu = fits.PrimaryHDU()
+        pdu.header['FILETYPE'] = "Rectified spectra"
+        #pdu.header['INSTRUME'] = inhdul[0].header['HIERARCH ESO OBS INSTRUME']
+        #pdu.header['FILTER'] = from_currsys("!OBS.filter_name_fw1")
+        outhdul = fits.HDUList([pdu])
+
+        for i, trace_id in enumerate(self.spectral_traces):
+            hdu = self[trace_id].rectify(hdulist,
+                                         interps=interps,
+                                         bin_width=bin_width,
+                                         xi_min=xi_min, xi_max=xi_max,
+                                         wave_min=wave_min, wave_max=wave_max)
+            if hdu is not None:   # ..todo: rectify does not do that yet
+                outhdul.append(hdu)
+                outhdul[0].header[f"EXTNAME{i+1}"] = trace_id
+
+        outhdul[0].header.update(inhdul[0].header)
+
+        return outhdul
+
+
+    def rectify_cube(self, hdulist):
+        """Rectify traces and combine into a cube"""
+        raise(NotImplementedError)
+
     def plot(self, wave_min=None, wave_max=None, **kwargs):
         if wave_min is None:
             wave_min = from_currsys("!SIM.spectral.wave_min")
         if wave_max is None:
             wave_max = from_currsys("!SIM.spectral.wave_max")
 
         from matplotlib import pyplot as plt
@@ -250,21 +333,28 @@
             clrs = "rgbcymk" * (1 + len(self.spectral_traces) // 7)
             for spt, c in zip(self.spectral_traces.values(), clrs):
                 spt.plot(wave_min, wave_max, c=c)
 
         return plt.gcf()
 
     def __repr__(self):
-        return "\n".join([spt.__repr__() for spt in self.spectral_traces])
+        # "\n".join([spt.__repr__() for spt in self.spectral_traces])
+        return f"{self.__class__.__name__}(**{self.meta!r})"
 
     def __str__(self):
-        msg = 'SpectralTraceList: "{}" : {} traces' \
-              ''.format(self.meta.get("name"), len(self.spectral_traces))
+        msg = (f"SpectralTraceList: \"{self.meta.get('name')}\" : "
+               f"{len(self.spectral_traces)} traces")
         return msg
 
+    def __getitem__(self, item):
+        return self.spectral_traces[item]
+
+    def __setitem__(self, key, value):
+        self.spectral_traces[key] = value
+
 
 class SpectralTraceListWheel(Effect):
     """
     A Wheel-Effect object for selecting between multiple gratings/grisms
 
     See ``SpectralTraceList`` for the trace file format description.
 
@@ -331,21 +421,20 @@
                   "path": "",
                   "report_plot_include": True,
                   "report_table_include": True,
                   "report_table_rounding": 4}
         self.meta.update(params)
         self.meta.update(kwargs)
 
-        path = pth.join(self.meta["path"],
-                        from_currsys(self.meta["filename_format"]))
+        path = Path(self.meta["path"], from_currsys(self.meta["filename_format"]))
         self.trace_lists = {}
         for name in from_currsys(self.meta["trace_list_names"]):
             kwargs["name"] = name
-            self.trace_lists[name] = SpectralTraceList(filename=path.format(name),
-                                                       **kwargs)
+            fname = str(path).format(name)
+            self.trace_lists[name] = SpectralTraceList(filename=fname, **kwargs)
 
     def apply_to(self, obj, **kwargs):
         """Use apply_to of current trace list"""
         return self.current_trace_list.apply_to(obj, **kwargs)
 
     @property
     def current_trace_list(self):
@@ -354,8 +443,8 @@
         if trace_list_name is not None:
             trace_list_eff = self.trace_lists[trace_list_name]
         return trace_list_eff
 
     @property
     def display_name(self):
         name = self.meta.get("name", self.meta.get("filename", "<untitled>"))
-        return f'{name} : [{from_currsys(self.meta["current_trace_list"])}]'
+        return f"{name} : [{from_currsys(self.meta['current_trace_list'])}]"
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/spectral_trace_list_utils.py` & `ScopeSim-0.6.0/scopesim/effects/spectral_trace_list_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """
+Utility classes and functions for SpectralTraceList
+
 This module contains
-   - the definition of the `SpectralTrace` class.
+   - the definition of the `SpectralTrace` class. The visible effect should
+     always be a `SpectralTraceList`, even if that contains only one
+     `SpectralTrace`.
    - the definition of the `XiLamImage` class
    - utility functions for use with spectral traces
 """
 
 import logging
 
 import numpy as np
 
 from scipy.interpolate import RectBivariateSpline
-from scipy.interpolate import InterpolatedUnivariateSpline
+from scipy.interpolate import interp1d
 from matplotlib import pyplot as plt
 
 from astropy.table import Table
 from astropy.modeling import fitting
 from astropy.io import fits
 from astropy import units as u
 from astropy.wcs import WCS
 from astropy.modeling.models import Polynomial2D
 
-from ..optics import image_plane_utils as imp_utils
-from ..utils import deriv_polynomial2d, power_vector, interp2, check_keys,\
-    from_currsys, quantify
+from ..utils import power_vector, quantify, from_currsys
 
 
 class SpectralTrace:
     """Definition of one spectral trace
 
     A SpectralTrace describes the mapping of spectral slit coordinates
     to the focal plane. The class reads an order layout and fits several
@@ -56,176 +58,160 @@
         # The values need to be here for stand-alone use.
         self.meta = {}
         self.meta.update(self._class_params)
         self.meta.update(kwargs)
 
         if isinstance(trace_tbl, (fits.BinTableHDU, fits.TableHDU)):
             self.table = Table.read(trace_tbl)
-            self.meta["trace_id"] = trace_tbl.header.get('EXTNAME', "<unknown trace id>")
+            self.meta["trace_id"] = trace_tbl.header.get("EXTNAME", "<unknown trace id>")
+            self.dispersion_axis = trace_tbl.header.get("DISPDIR", "unknown")
         elif isinstance(trace_tbl, Table):
             self.table = trace_tbl
+            self.dispersion_axis = "unknown"
         else:
             raise ValueError("trace_tbl must be one of (fits.BinTableHDU, "
-                             "fits.TableHDU, astropy.Table): {}"
-                             "".format(type(trace_tbl)))
-
+                             f"fits.TableHDU, astropy.Table) but is {type(trace_tbl)}")
         self.compute_interpolation_functions()
 
+        # Declaration of other attributes
+        self._xilamimg = None
+        self.dlam_per_pix = None
+
     def fov_grid(self):
         """
         Provide information on the source space volume required by the effect
 
         Returns
         -------
         A dictionary with entries `wave_min` and `wave_max`.
         Spatial limits are determined by the `ApertureMask` effect
         and are not returned here.
         """
-        trace_id = self.meta['trace_id']
-        aperture_id = self.meta['aperture_id']
-        lam_arr = self.table[self.meta['wave_colname']]
+        trace_id = self.meta["trace_id"]
+        aperture_id = self.meta["aperture_id"]
+        lam_arr = self.table[self.meta["wave_colname"]]
 
         wave_max = np.max(lam_arr)
         wave_min = np.min(lam_arr)
 
-        return {'wave_min': wave_min, 'wave_max': wave_max,
-                'trace_id': trace_id, 'aperture_id': aperture_id}
+        return {"wave_min": wave_min, "wave_max": wave_max,
+                "trace_id": trace_id, "aperture_id": aperture_id}
 
     def compute_interpolation_functions(self):
         """
         Compute various interpolation functions between slit and focal plane
+
+        Focal plane coordinates are `x` and `y`, in mm. Slit coordinates are
+        `xi` (spatial coordinate along the slit, in arcsec) and `lam` (wavelength, in um).
         """
-        if self.meta["invalid_value"] is not None:
-            self.table = sanitize_table(
-                self.table,
-                invalid_value=self.meta["invalid_value"],
-                wave_colname=self.meta["wave_colname"],
-                x_colname=self.meta["x_colname"],
-                y_colname=self.meta["y_colname"],
-                spline_order=self.meta["spline_order"],
-                ext_id=self.meta["extension_id"])
-
-        x_arr = self.table[self.meta['x_colname']]
-        y_arr = self.table[self.meta['y_colname']]
-        xi_arr = self.table[self.meta['s_colname']]
-        lam_arr = self.table[self.meta['wave_colname']]
-
-        wi0, wi1 = lam_arr.argmin(), lam_arr.argmax()
-        x_disp_length = np.diff([x_arr[wi0], x_arr[wi1]])
-        y_disp_length = np.diff([y_arr[wi0], y_arr[wi1]])
-        self.dispersion_axis = "x" if x_disp_length > y_disp_length else "y"
+        x_arr = self.table[self.meta["x_colname"]]
+        y_arr = self.table[self.meta["y_colname"]]
+        xi_arr = self.table[self.meta["s_colname"]]
+        lam_arr = self.table[self.meta["wave_colname"]]
 
         self.wave_min = quantify(np.min(lam_arr), u.um).value
         self.wave_max = quantify(np.max(lam_arr), u.um).value
 
         self.xy2xi = Transform2D.fit(x_arr, y_arr, xi_arr)
         self.xy2lam = Transform2D.fit(x_arr, y_arr, lam_arr)
         self.xilam2x = Transform2D.fit(xi_arr, lam_arr, x_arr)
         self.xilam2y = Transform2D.fit(xi_arr, lam_arr, y_arr)
         self._xiy2x = Transform2D.fit(xi_arr, y_arr, x_arr)
         self._xiy2lam = Transform2D.fit(xi_arr, y_arr, lam_arr)
 
+        if self.dispersion_axis == 'unknown':
+            dlam_dx, dlam_dy = self.xy2lam.gradient()
+            wave_mid = 0.5 * (self.wave_min + self.wave_max)
+            xi_mid = np.mean(xi_arr)
+            x_mid = self.xilam2x(xi_mid, wave_mid)
+            y_mid = self.xilam2y(xi_mid, wave_mid)
+            if dlam_dx(x_mid, y_mid) > dlam_dy(x_mid, y_mid):
+                self.dispersion_axis = "x"
+            else:
+                self.dispersion_axis = "y"
+            logging.warning("Dispersion axis determined to be %s",
+                            self.dispersion_axis)
+
+
     def map_spectra_to_focal_plane(self, fov):
         """
         Apply the spectral trace mapping to a spectral cube
 
         The cube is contained in a FieldOfView object, which also has
         world coordinate systems for the Source (sky coordinates and
         wavelengths) and for the focal plane.
         The method returns a section of the fov image along with info on
         where this image lies in the focal plane.
         """
-
+        logging.info("Mapping %s", fov.meta['trace_id'])
         # Initialise the image based on the footprint of the spectral
         # trace and the focal plane WCS
-        wave_min = fov.meta['wave_min'].value       # [um]
-        wave_max = fov.meta['wave_max'].value       # [um]
-        xi_min = fov.meta['xi_min'].value           # [arcsec]
-        xi_max = fov.meta['xi_max'].value           # [arcsec]
+        wave_min = fov.meta["wave_min"].value       # [um]
+        wave_max = fov.meta["wave_max"].value       # [um]
+        xi_min = fov.meta["xi_min"].value           # [arcsec]
+        xi_max = fov.meta["xi_max"].value           # [arcsec]
         xlim_mm, ylim_mm = self.footprint(wave_min=wave_min, wave_max=wave_max,
                                           xi_min=xi_min, xi_max=xi_max)
-        #print("xlim_mm:", xlim_mm, "   ylim_mm:", ylim_mm)
+
         if xlim_mm is None:
-            print("xlim_mm is None")
+            logging.warning("xlim_mm is None")
             return None
 
         fov_header = fov.header
         det_header = fov.detector_header
 
         # WCSD from the FieldOfView - this is the full detector plane
-        fpa_wcs = WCS(fov_header, key='D')
-        naxis1, naxis2 = fov_header['NAXIS1'], fov_header['NAXIS2']
-        pixsize = fov_header['CDELT1D'] * u.Unit(fov_header['CUNIT1D'])
+        pixsize = fov_header["CDELT1D"] * u.Unit(fov_header["CUNIT1D"])
         pixsize = pixsize.to(u.mm).value
-        pixscale = fov_header['CDELT1'] * u.Unit(fov_header['CUNIT1'])
+        pixscale = fov_header["CDELT1"] * u.Unit(fov_header["CUNIT1"])
         pixscale = pixscale.to(u.arcsec).value
 
-        fpa_wcsd = WCS(det_header, key='D')
-        naxis1d, naxis2d = det_header['NAXIS1'], det_header['NAXIS2']
+        fpa_wcsd = WCS(det_header, key="D")
+        naxis1d, naxis2d = det_header["NAXIS1"], det_header["NAXIS2"]
         xlim_px, ylim_px = fpa_wcsd.all_world2pix(xlim_mm, ylim_mm, 0)
         xmin = np.floor(xlim_px.min()).astype(int)
         xmax = np.ceil(xlim_px.max()).astype(int)
         ymin = np.floor(ylim_px.min()).astype(int)
         ymax = np.ceil(ylim_px.max()).astype(int)
 
         ## Check if spectral trace footprint is outside FoV
-        #print(fpa_wcsd)
-        #print(xmin, xmax, ymin, ymax, " <<->> ", naxis1d, naxis2d)
         if xmax < 0 or xmin > naxis1d or ymax < 0 or ymin > naxis2d:
-            logging.warning("Spectral trace footprint is outside FoV")
+            logging.info("Spectral trace %s: footprint is outside FoV",
+                         fov.meta['trace_id'])
             return None
 
         # Only work on parts within the FoV
         xmin = max(xmin, 0)
         xmax = min(xmax, naxis1d)
         ymin = max(ymin, 0)
         ymax = min(ymax, naxis2d)
 
         # Create header for the subimage - I think this only needs the DET one,
         # but we'll do both. The WCSs are initialised from the full fpa WCS and
         # then shifted accordingly.
-        # sub_wcs = WCS(fov_header, key=" ")
-        # sub_wcs.wcs.crpix -= np.array([xmin, ymin])
         det_wcs = WCS(det_header, key="D")
         det_wcs.wcs.crpix -= np.array([xmin, ymin])
 
         sub_naxis1 = xmax - xmin
         sub_naxis2 = ymax - ymin
 
         # initialise the subimage
         image = np.zeros((sub_naxis2, sub_naxis1), dtype=np.float32)
 
         # Adjust the limits of the subimage in millimeters in the focal plane
         # This takes the adjustment to integer pixels into account
         xmin_mm, ymin_mm = fpa_wcsd.all_pix2world(xmin, ymin, 0)
         xmax_mm, ymax_mm = fpa_wcsd.all_pix2world(xmax, ymax, 0)
 
-        # wavelength step per detector pixel at centre of slice
-        # ..todo: - currently using average dlam_per_pix. This should
-        #           be okay if there is not strong anamorphism. Below, we
-        #           compute an image of abs(dlam_per_pix) in the focal plane.
-        #           XiLamImage would need that as an image of xi/lam, which should
-        #           be possible but too much for the time being.
-        #         - The dispersion direction is selected by the direction of the
-        #           gradient of lam(x, y). This works if the lam-axis is well
-        #           aligned with x or y. Needs to be tested for MICADO.
-
-
-        # dlam_by_dx, dlam_by_dy = self.xy2lam.gradient()
-        # if np.abs(dlam_by_dx(0, 0)) > np.abs(dlam_by_dy(0, 0)):
-        if self.dispersion_axis == "x":
-            avg_dlam_per_pix = (wave_max - wave_min) / sub_naxis1
-        else:
-            avg_dlam_per_pix = (wave_max - wave_min) / sub_naxis2
-
+        self._set_dispersion(wave_min, wave_max, pixsize=pixsize)
         try:
-            xilam = XiLamImage(fov, avg_dlam_per_pix)
-            self.xilam = xilam    # ..todo: remove
+            xilam = XiLamImage(fov, self.dlam_per_pix)
+            self._xilamimg = xilam   # ..todo: remove or make available with a debug flag?
         except ValueError:
-            print(" ---> ", self.meta['trace_id'], "gave ValueError")
+            print(f" ---> {self.meta['trace_id']} gave ValueError")
 
         npix_xi, npix_lam = xilam.npix_xi, xilam.npix_lam
         xilam_wcs = xilam.wcs
 
         # focal-plane coordinate images
         ximg_fpa, yimg_fpa = np.meshgrid(np.linspace(xmin_mm, xmax_mm,
                                                      sub_naxis1,
@@ -277,20 +263,139 @@
         img_header = det_wcs.to_header()
         img_header["XMIN"] = xmin
         img_header["XMAX"] = xmax
         img_header["YMIN"] = ymin
         img_header["YMAX"] = ymax
 
         if np.any(image < 0):
-            logging.warning(f"map_spectra_to_focal_plane: {np.sum(image < 0)} negative pixels")
-
+            logging.warning("map_spectra_to_focal_plane: %d negative pixels",
+                            np.sum(image < 0))
 
         image_hdu = fits.ImageHDU(header=img_header, data=image)
         return image_hdu
 
+    def rectify(self, hdulist, interps=None, wcs=None, **kwargs):
+        """Create 2D spectrum for a trace
+
+        Parameters
+        ----------
+        hdulist : HDUList
+           The result of scopesim readout
+        interps : list of interpolation functions
+           If provided, there must be one for each image extension in `hdulist`.
+           The functions go from pixels to the images and can be created with,
+           e.g., RectBivariateSpline.
+        wcs : The WCS describing the rectified XiLamImage. This can be created
+           in a simple way from the fov included in the `OpticalTrain` used in
+           the simulation run producing `hdulist`.
+
+        The WCS can also be set up via the following keywords:
+
+        bin_width : float [um]
+           The spectral bin width. This is best computed automatically from the
+           spectral dispersion of the trace.
+        wave_min, wave_max : float [um]
+           Limits of the wavelength range to extract. The default is the
+           the full range on which the `SpectralTrace` is defined. This may
+           extend significantly beyond the filter window.
+        xi_min, xi_max : float [arcsec]
+           Spatial limits of the slit on the sky. This should be taken from
+           the header of the hdulist, but this is not yet provided by scopesim
+        """
+        logging.info("Rectifying %s", self.trace_id)
+
+        wave_min = kwargs.get("wave_min",
+                              self.wave_min)
+        wave_max = kwargs.get("wave_max",
+                              self.wave_max)
+        if wave_max < self.wave_min or wave_min > self.wave_max:
+            logging.info("   Outside filter range")
+            return None
+        wave_min = max(wave_min, self.wave_min)
+        wave_max = min(wave_max, self.wave_max)
+        logging.info("   %.02f .. %.02f um", wave_min, wave_max)
+
+        # bin_width is taken as the minimum dispersion of the trace
+        bin_width = kwargs.get("bin_width", None)
+        if bin_width is None:
+            self._set_dispersion(wave_min, wave_max)
+            bin_width = np.abs(self.dlam_per_pix.y).min()
+        logging.info("   Bin width %.02g um", bin_width)
+
+        pixscale = from_currsys(self.meta['pixel_scale'])
+
+        # Temporary solution to get slit length
+        xi_min = kwargs.get("xi_min", None)
+        if xi_min is None:
+            try:
+                xi_min = hdulist[0].header["HIERARCH INS SLIT XIMIN"]
+            except KeyError:
+                logging.error("xi_min not found")
+                return None
+        xi_max = kwargs.get("xi_max", None)
+        if xi_max is None:
+            try:
+                xi_max = hdulist[0].header["HIERARCH INS SLIT XIMAX"]
+            except KeyError:
+                logging.error("xi_max not found")
+                return None
+
+        if wcs is None:
+            wcs = WCS(naxis=2)
+            wcs.wcs.ctype = ['WAVE', 'LINEAR']
+            wcs.wcs.cunit = ['um', 'arcsec']
+            wcs.wcs.crpix = [1, 1]
+            wcs.wcs.cdelt = [bin_width, pixscale] # PIXSCALE
+
+        # crval set to wave_min to catch explicitely set value
+        wcs.wcs.crval = [wave_min, xi_min]   # XIMIN
+
+        nlam = int((wave_max - wave_min) / bin_width) + 1
+        nxi = int((xi_max - xi_min) / pixscale) + 1
+
+        # Create interpolation functions if not provided
+        if interps is None:
+            logging.info("Computing image interpolations")
+            interps = make_image_interpolations(hdulist, kx=1, ky=1)
+
+        # Create Xi, Lam images (do I need Iarr and Jarr or can I build Xi, Lam directly?)
+        Iarr, Jarr = np.meshgrid(np.arange(nlam, dtype=np.float32),
+                                 np.arange(nxi, dtype=np.float32))
+        Lam, Xi = wcs.all_pix2world(Iarr, Jarr, 0)
+
+        # Make sure that we do have microns
+        Lam = Lam * u.Unit(wcs.wcs.cunit[0]).to(u.um)
+
+        # Convert Xi, Lam to focal plane units
+        Xarr = self.xilam2x(Xi, Lam)
+        Yarr = self.xilam2y(Xi, Lam)
+
+        rect_spec = np.zeros_like(Xarr, dtype=np.float32)
+
+        ihdu = 0
+        for hdu in hdulist:
+            if not isinstance(hdu, fits.ImageHDU):
+                continue
+
+            wcs_fp = WCS(hdu.header, key="D")
+            n_x = hdu.header['NAXIS1']
+            n_y = hdu.header['NAXIS2']
+            iarr, jarr = wcs_fp.all_world2pix(Xarr, Yarr, 0)
+            mask = (iarr > 0) * (iarr < n_x) * (jarr > 0) * (jarr < n_y)
+            if np.any(mask):
+                specpart = interps[ihdu](jarr, iarr, grid=False)
+                rect_spec += specpart * mask
+
+            ihdu += 1
+
+        header = wcs.to_header()
+        header['EXTNAME'] = self.trace_id
+        return fits.ImageHDU(data=rect_spec, header=header)
+
+
     def footprint(self, wave_min=None, wave_max=None, xi_min=None, xi_max=None):
         """
         Return corners of rectangle enclosing spectral trace
 
         Parameters
         ----------
         wave_min, wave_max : float [um], Quantity
@@ -298,26 +403,24 @@
             If `None`, use the full range that the spectral trace is defined on.
             Float values are interpreted as microns.
         xi_min, xi_max : float [arcsec], Quantity
             Minimum and maximum slit position on the sky.
             If `None`, use the full range that the spectral trace is defined on.
             Float values are interpreted as arcsec.
         """
-        #print(f"footprint: {wave_min}, {wave_max}, {xi_min}, {xi_max}")
-
         ## Define the wavelength range of the footprint. This is a compromise
         ## between the requested range (by method args) and the definition
         ## range of the spectral trace
         ## This is only relevant if the trace is given by a table of reference
         ## points. Otherwise (METIS LMS!) we assume that the range is valid.
-        if ('wave_colname' in self.meta and
-            self.meta['wave_colname'] in self.table.colnames):
+        if ("wave_colname" in self.meta and
+            self.meta["wave_colname"] in self.table.colnames):
             # Here, the parameters are obtained from a table of reference points
-            wave_unit = self.table[self.meta['wave_colname']].unit
-            wave_val = quantify(self.table[self.meta['wave_colname']].data,
+            wave_unit = self.table[self.meta["wave_colname"]].unit
+            wave_val = quantify(self.table[self.meta["wave_colname"]].data,
                                 wave_unit)
 
             if wave_min is None:
                 wave_min = np.min(wave_val)
             if wave_max is None:
                 wave_max = np.max(wave_val)
 
@@ -333,19 +436,19 @@
             wave_min = max(wave_min, np.min(wave_val)).value
             wave_max = min(wave_max, np.max(wave_val)).value
 
             ## Define the slit range of the footprint. This is a compromise
             ## between the requested range (by method args) and the definition
             ## range of the spectral trace
             try:
-                xi_unit = self.table[self.meta['s_colname']].unit
+                xi_unit = self.table[self.meta["s_colname"]].unit
             except KeyError:
                 xi_unit = u.arcsec
 
-            xi_val = quantify(self.table[self.meta['s_colname']].data,
+            xi_val = quantify(self.table[self.meta["s_colname"]].data,
                               xi_unit)
 
             if xi_min is None:
                 xi_min = np.min(xi_val)
             if xi_max is None:
                 xi_max = np.max(xi_val)
 
@@ -379,14 +482,17 @@
                 [y_edge.min(), y_edge.min(), y_edge.max(), y_edge.max()])
 
     def plot(self, wave_min=None, wave_max=None, c="r"):
         """Plot control points of the SpectralTrace"""
 
         # Footprint (rectangle enclosing the trace)
         xlim, ylim  = self.footprint(wave_min=wave_min, wave_max=wave_max)
+        if xlim is None:
+            return
+
         xlim.append(xlim[0])
         ylim.append(ylim[0])
         plt.plot(xlim, ylim)
 
         # Control points
         waves = self.table[self.meta["wave_colname"]]
         if wave_min is None:
@@ -396,107 +502,144 @@
 
         mask = (waves >= wave_min) * (waves <= wave_max)
         if sum(mask) > 2:
             w = waves[mask]
 
             x = self.table[self.meta["x_colname"]][mask]
             y = self.table[self.meta["y_colname"]][mask]
-            plt.plot(x, y, 'o', c=c)
+            plt.plot(x, y, "o", c=c)
 
-            for wave in np.unique(waves):
-                xx = x[waves==wave]
+            for wave in np.unique(w):
+                xx = x[w==wave]
                 xx.sort()
                 dx = xx[-1] - xx[-2]
-                plt.text(x[waves==wave].max() + 0.5 * dx,
-                         y[waves==wave].mean(),
-                         str(wave), va='center', ha='left')
 
+                plt.text(x[w==wave].max() + 0.5 * dx,
+                         y[w==wave].mean(),
+                         str(wave), va='center', ha='left')
 
             plt.gca().set_aspect("equal")
 
+    @property
+    def trace_id(self):
+        """Return the name of the trace"""
+        return self.meta['trace_id']
+
+    def _set_dispersion(self, wave_min, wave_max, pixsize=None):
+        """Computation of dispersion dlam_per_pix along xi=0
+        """
+        #..todo: This may have to be generalised - xi=0 is at the centre
+        #of METIS slits and the short MICADO slit.
+
+        xi = np.array([0] * 1001)
+        lam = np.linspace(wave_min, wave_max, 1001)
+        x_mm = self.xilam2x(xi, lam)
+        y_mm = self.xilam2y(xi, lam)
+        if self.dispersion_axis == "x":
+            dlam_grad = self.xy2lam.gradient()[0]  # dlam_by_dx
+        else:
+            dlam_grad = self.xy2lam.gradient()[1]  # dlam_by_dy
+        pixsize = (from_currsys(self.meta['pixel_scale']) /
+                   from_currsys(self.meta['plate_scale']))
+        self.dlam_per_pix = interp1d(lam,
+                                     dlam_grad(x_mm, y_mm) * pixsize,
+                                     fill_value="extrapolate")
+
     def __repr__(self):
-        msg = '<SpectralTrace> "{}" : [{}, {}]um : Ext {} : Aperture {} : ' \
-              'ImagePlane {}' \
-              ''.format(self.meta["trace_id"],
-                        round(self.wave_min, 4), round(self.wave_max, 4),
-                        self.meta["extension_id"], self.meta["aperture_id"],
-                        self.meta["image_plane_id"])
+        return f"{self.__class__.__name__}({self.table!r}, **{self.meta!r})"
+
+    def __str__(self):
+        msg = (f"<SpectralTrace> \"{self.meta['trace_id']}\" : "
+               f"[{self.wave_min:.4f}, {self.wave_max:.4f}]um : "
+               f"Ext {self.meta['extension_id']} : "
+               f"Aperture {self.meta['aperture_id']} : "
+               f"ImagePlane {self.meta['image_plane_id']}")
         return msg
 
 
 class XiLamImage():
     """
     Class to compute a rectified 2D spectrum
 
     The class produces and holds an image of xi (relative position along
     the spatial slit direction) and wavelength lambda.
+
+    Parameters
+    ----------
+    fov : FieldOfView
+    dlam_per_pix : a 1-D interpolation function from wavelength (in um) to dispersion
+          (in um/pixel); alternatively a number giving an average dispersion
     """
 
     def __init__(self, fov, dlam_per_pix):
         # ..todo: we assume that we always have a cube. We use SpecCADO's
         #         add_cube_layer method
-        cube_wcs = WCS(fov.cube.header, key=' ')
+        cube_wcs = WCS(fov.cube.header, key=" ")
         wcs_lam = cube_wcs.sub([3])
 
-        d_xi = fov.cube.header['CDELT1']
-        d_xi *= u.Unit(fov.cube.header['CUNIT1']).to(u.arcsec)
-        d_eta = fov.cube.header['CDELT2']
-        d_eta *= u.Unit(fov.cube.header['CUNIT2']).to(u.arcsec)
-        d_lam = fov.cube.header['CDELT3']
-        d_lam *= u.Unit(fov.cube.header['CUNIT3']).to(u.um)
+        d_xi = fov.cube.header["CDELT1"]
+        d_xi *= u.Unit(fov.cube.header["CUNIT1"]).to(u.arcsec)
+        d_eta = fov.cube.header["CDELT2"]
+        d_eta *= u.Unit(fov.cube.header["CUNIT2"]).to(u.arcsec)
+        d_lam = fov.cube.header["CDELT3"]
+        d_lam *= u.Unit(fov.cube.header["CUNIT3"]).to(u.um)
 
         # This is based on the cube shape and assumes that the cube's spatial
         # dimensions are set by the slit aperture
         (n_lam, n_eta, n_xi) = fov.cube.data.shape
 
         # arrays of cube coordinates
-        cube_xi = d_xi * np.arange(n_xi) + fov.meta['xi_min'].value
+        cube_xi = d_xi * np.arange(n_xi) + fov.meta["xi_min"].value
         cube_eta = d_eta * (np.arange(n_eta) - (n_eta - 1) / 2)
         cube_lam = wcs_lam.all_pix2world(np.arange(n_lam), 1)[0]
         cube_lam *= u.Unit(wcs_lam.wcs.cunit[0]).to(u.um)
 
         # Initialise the array to hold the xi-lambda image
         self.image = np.zeros((n_xi, n_lam), dtype=np.float32)
         self.lam = cube_lam
+        try:
+            dlam_per_pix_val = dlam_per_pix(np.asarray(self.lam))
+        except TypeError:
+            dlam_per_pix_val = dlam_per_pix
+            logging.warning("Using scalar dlam_per_pix = %.2g",
+                            dlam_per_pix_val)
 
         for i, eta in enumerate(cube_eta):
-            #if abs(eta) > fov.slit_width / 2:   # ..todo: needed?
-            #    continue
+            lam0 = self.lam + dlam_per_pix_val * eta / d_eta
 
-            lam0 = self.lam + dlam_per_pix * eta / d_eta
             # lam0 is the target wavelength. We need to check that this
             # overlaps with the wavelength range covered by the cube
             if lam0.min() < cube_lam.max() and lam0.max() > cube_lam.min():
                 plane = fov.cube.data[:, i, :].T
                 plane_interp = RectBivariateSpline(cube_xi, cube_lam, plane,
                                                    kx=1, ky=1)
                 self.image += plane_interp(cube_xi, lam0)
 
         self.image *= d_eta     # ph/s/um/arcsec2 --> ph/s/um/arcsec
 
         # WCS for the xi-lambda image, i.e. the rectified 2D spectrum
         # Default WCS with xi in arcsec
         self.wcs = WCS(naxis=2)
         self.wcs.wcs.crpix = [1, 1]
-        self.wcs.wcs.crval = [self.lam[0], fov.meta['xi_min'].value]
+        self.wcs.wcs.crval = [self.lam[0], fov.meta["xi_min"].value]
         self.wcs.wcs.pc = [[1, 0], [0, 1]]
         self.wcs.wcs.cdelt = [d_lam, d_xi]
-        self.wcs.wcs.ctype = ['LINEAR', 'LINEAR']
-        self.wcs.wcs.cname = ['WAVELEN', 'SLITPOS']
-        self.wcs.wcs.cunit = ['um', 'arcsec']
+        self.wcs.wcs.ctype = ["LINEAR", "LINEAR"]
+        self.wcs.wcs.cname = ["WAVELEN", "SLITPOS"]
+        self.wcs.wcs.cunit = ["um", "arcsec"]
 
         # Alternative: xi = [0, 1], dimensionless
         self.wcsa = WCS(naxis=2)
         self.wcsa.wcs.crpix = [1, 1]
         self.wcsa.wcs.crval = [self.lam[0], 0]
         self.wcsa.wcs.pc = [[1, 0], [0, 1]]
         self.wcsa.wcs.cdelt = [d_lam, 1./n_xi]
-        self.wcsa.wcs.ctype = ['LINEAR', 'LINEAR']
-        self.wcsa.wcs.cname = ['WAVELEN', 'SLITPOS']
-        self.wcs.wcs.cunit = ['um', '']
+        self.wcsa.wcs.ctype = ["LINEAR", "LINEAR"]
+        self.wcsa.wcs.cname = ["WAVELEN", "SLITPOS"]
+        self.wcs.wcs.cunit = ["um", ""]
 
         self.xi = self.wcs.all_pix2world(self.lam[0], np.arange(n_xi), 0)[1]
         self.npix_xi = n_xi
         self.npix_lam = n_lam
         # ..todo: cubic spline introduces negative values, linear does not.
         #  Alternative might be to cubic-spline interpolate on sqrt(image),
         #  with subsequent squaring of the result. This would require
@@ -558,15 +701,14 @@
 
     def _repackage(self, trafo):
         """Make sure `trafo` is a tuple"""
         if trafo is not None and not isinstance(trafo, tuple):
             trafo = (trafo, {})
         return trafo
 
-
     def __call__(self, x, y, grid=False, **kwargs):
         """
         Apply the polynomial transform
 
         The transformation is a polynomial based on the simple
         monomials x^i y^j. When grid=True, the transform is applied to the grid
         formed by the tensor product of the vectors x and y. When grid=False,
@@ -617,15 +759,15 @@
         if grid:
             result = yvec.T @ temp
         else:
             # Compute the scalar product of each column in yvec with the
             # corresponding column in temp. This gives the diagonal of the
             # expression in the "grid" branch.
             result = (yvec * temp).sum(axis=0)
-            if orig_shape == () or orig_shape is None:
+            if not orig_shape:
                 result = np.float32(result)
             else:
                 result = result.reshape(orig_shape)
 
         # Apply posttransform
         if self.posttransform is not None:
             result = self.posttransform[0](result, **self.posttransform[1])
@@ -662,30 +804,30 @@
     """
     coeffs = dict(zip(fit.param_names, fit.parameters))
     deg = fit.degree
     mat = np.zeros((deg + 1 , deg + 1), dtype=np.float32)
     for i in range(deg + 1):
         for j in range(deg + 1):
             try:
-                mat[j, i] = coeffs['c{}_{}'.format(i, j)]
+                mat[j, i] = coeffs[f"c{i}_{j}"]
             except KeyError:
                 pass
     return mat
 
 # ..todo: should the next three functions be combined and return a dictionary of fits?
 def xilam2xy_fit(layout, params):
     """
     Determine polynomial fits of FPA position
 
     Fits are of degree 4 as a function of slit position and wavelength.
     """
-    xi_arr = layout[params['s_colname']]
-    lam_arr = layout[params['wave_colname']]
-    x_arr = layout[params['x_colname']]
-    y_arr = layout[params['y_colname']]
+    xi_arr = layout[params["s_colname"]]
+    lam_arr = layout[params["wave_colname"]]
+    x_arr = layout[params["x_colname"]]
+    y_arr = layout[params["y_colname"]]
 
     ## Filter the lists: remove any points with x==0
     ## ..todo: this may not be necessary after sanitising the table
     #good = x != 0
     #xi = xi[good]
     #lam = lam[good]
     #x = x[good]
@@ -703,18 +845,18 @@
 def xy2xilam_fit(layout, params):
     """
     Determine polynomial fits of wavelength/slit position
 
     Fits are of degree 4 as a function of focal plane position
     """
 
-    xi_arr = layout[params['s_colname']]
-    lam_arr = layout[params['wave_colname']]
-    x_arr = layout[params['x_colname']]
-    y_arr = layout[params['y_colname']]
+    xi_arr = layout[params["s_colname"]]
+    lam_arr = layout[params["wave_colname"]]
+    x_arr = layout[params["x_colname"]]
+    y_arr = layout[params["y_colname"]]
 
     pinit_xi = Polynomial2D(degree=4)
     pinit_lam = Polynomial2D(degree=4)
     fitter = fitting.LinearLSQFitter()
     xy2xi = fitter(pinit_xi, x_arr, y_arr, xi_arr)
     xy2lam = fitter(pinit_lam, x_arr, y_arr, lam_arr)
 
@@ -726,26 +868,40 @@
 
     Fits are of degree 4 as a function of focal plane position
     """
 
     # These are helper functions to allow fitting of left/right edges
     # for the purpose of checking whether a trace is on a chip or not.
 
-    xi_arr = layout[params['s_colname']]
-    lam_arr = layout[params['wave_colname']]
-    x_arr = layout[params['x_colname']]
-    y_arr = layout[params['y_colname']]
+    xi_arr = layout[params["s_colname"]]
+    lam_arr = layout[params["wave_colname"]]
+    x_arr = layout[params["x_colname"]]
+    y_arr = layout[params["y_colname"]]
 
     pinit_x = Polynomial2D(degree=4)
     pinit_lam = Polynomial2D(degree=4)
     fitter = fitting.LinearLSQFitter()
     xiy2x = fitter(pinit_x, xi_arr, y_arr, x_arr)
     xiy2lam = fitter(pinit_lam, xi_arr, y_arr, lam_arr)
     return xiy2x, xiy2lam
 
+def make_image_interpolations(hdulist, **kwargs):
+    """
+    Create 2D interpolation functions for images
+    """
+    interps = []
+    for hdu in hdulist:
+        if isinstance(hdu, fits.ImageHDU):
+            interps.append(
+                RectBivariateSpline(np.arange(hdu.header['NAXIS1']),
+                                    np.arange(hdu.header['NAXIS2']),
+                                    hdu.data, **kwargs)
+            )
+    return interps
+
 
 # ..todo: Check whether the following functions are actually used
 def rolling_median(x, n):
     """ Calculates the rolling median of a sequence for +/- n entries """
     y = [np.median(x[max(0, i-n):min(len(x), i+n+1)]) for i in range(len(x))]
     return np.array(y)
 
@@ -792,50 +948,7 @@
     dxs = np.diff(coords["x"], axis=1)
     dys = np.diff(coords["y"], axis=1)
     shears = np.array([np.arctan2(dys[i], dxs[i]) for i in range(dxs.shape[0])])
     shears = np.array(list(shears.T) + [shears.T[-1]]).T
     shears = (np.average(shears, axis=0) * rad2deg) - (90 + rotations)
 
     return rotations, shears
-
-
-# def sanitize_table(tbl, invalid_value, wave_colname, x_colname, y_colname,
-#                    spline_order=4, ext_id=None):
-#
-#     y_colnames = [col for col in tbl.colnames if y_colname in col]
-#     x_colnames = [col.replace(y_colname, x_colname) for col in y_colnames]
-#
-#     for x_col, y_col in zip(x_colnames, y_colnames):
-#         wave = tbl[wave_colname].data
-#         x = tbl[x_col].data
-#         y = tbl[y_col].data
-#
-#         valid = (x != invalid_value) * (y != invalid_value)
-#         invalid = np.invert(valid)
-#         if sum(invalid) == 0:
-#             continue
-#
-#         if sum(valid) == 0:
-#             logging.warning("--- Extension {} ---"
-#                             "All points in {} or {} were invalid. \n"
-#                             "THESE COLUMNS HAVE BEEN REMOVED FROM THE TABLE \n"
-#                             "invalid_value = {} \n"
-#                             "wave = {} \nx = {} \ny = {}"
-#                             "".format(ext_id, x_col, y_col, invalid_value,
-#                                       wave, x, y))
-#             tbl.remove_columns([x_col, y_col])
-#             continue
-#
-#         k = spline_order
-#         if wave[-1] > wave[0]:
-#             xnew = InterpolatedUnivariateSpline(wave[valid], x[valid], k=k)
-#             ynew = InterpolatedUnivariateSpline(wave[valid], y[valid], k=k)
-#         else:
-#             xnew = InterpolatedUnivariateSpline(wave[valid][::-1],
-#                                                 x[valid][::-1], k=k)
-#             ynew = InterpolatedUnivariateSpline(wave[valid][::-1],
-#                                                 y[valid][::-1], k=k)
-#
-#         tbl[x_col][invalid] = xnew(wave[invalid])
-#         tbl[y_col][invalid] = ynew(wave[invalid])
-#
-#     return tbl
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/surface_list.py` & `ScopeSim-0.6.0/scopesim/effects/surface_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,36 +21,34 @@
 
         self.surfaces = rad_utils.make_surface_dict_from_table(self.table)
         self._surface = None
         self._throughput = None
         self._emission = None
 
     def fov_grid(self, which="waveset", **kwargs):
+        wave_edges = []
         if which == "waveset":
             self.meta.update(kwargs)
             self.meta = from_currsys(self.meta)
             wave_min = quantify(self.meta["wave_min"], u.um)
             wave_max = quantify(self.meta["wave_max"], u.um)
             # ..todo:: add 1001 to default.yaml somewhere
             wave = np.linspace(wave_min, wave_max, 1001)
             throughput = self.throughput(wave)
             threshold = self.meta["minimum_throughput"]
             valid_waves = np.where(throughput >= threshold)[0]
-            if len(valid_waves) > 0:
-                wave_edges = [min(wave[valid_waves]), max(wave[valid_waves])]
-            else:
-                raise ValueError("No transmission found above the threshold {} "
-                                 "in this wavelength range {}. Did you open "
-                                 "the shutter?"
-                                 "".format(self.meta["minimum_throughput"],
-                                           [self.meta["wave_min"],
-                                            self.meta["wave_max"]]))
-        else:
-            wave_edges = []
 
+            if not len(valid_waves):
+                msg = ("No transmission found above the threshold "
+                       f"{self.meta['minimum_throughput']} in this wavelength "
+                       f"range {[self.meta['wave_min'], self.meta['wave_max']]}."
+                       " Did you open the shutter?")
+                raise ValueError(msg)
+
+            wave_edges = [min(wave[valid_waves]), max(wave[valid_waves])]
         return wave_edges
 
     @property
     def throughput(self):
         if self._throughput is None:
             self._throughput = self.get_throughput()
         return self._throughput
@@ -74,25 +72,26 @@
         return self._surface
 
     @surface.setter
     def surface(self, item):
         self._surface = item
 
     def get_throughput(self, start=0, end=None, rows=None):
-        """ Copied directly from radiometry_table """
+        """Copied directly from radiometry_table."""
 
         if self.table is None:
             return None
-        end = len(self.table) if end is None else end
-        end = end + len(self.table) if end < 0 else end
-        rows = np.arange(start, end) if rows is None else rows
-
-        thru = rad_utils.combine_throughputs(self.table, self.surfaces, rows)
+        if end is None:
+            end = len(self.table)
+        if end < 0:
+            end += len(self.table)
+        if rows is None:
+            rows = np.arange(start, end)
 
-        return thru
+        return rad_utils.combine_throughputs(self.table, self.surfaces, rows)
 
     def get_emission(self, etendue, start=0, end=None, rows=None,
                      use_area=False):
         # ..todo:: work out what this use_area flag means!
 
         if self.table is None:
             return None
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/surface_list_OLD.py` & `ScopeSim-0.6.0/scopesim/effects/surface_list_OLD.py`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/effects/ter_curves.py` & `ScopeSim-0.6.0/scopesim/effects/ter_curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-'''Transmission, emissivity, reflection curves'''
-import numpy as np
-from astropy import units as u
-from os import path as pth
+"""Transmission, emissivity, reflection curves"""
 import logging
+from pathlib import Path
 
+import numpy as np
+import skycalc_ipy
+from astropy import units as u
 from astropy.io import fits
 from astropy.table import Table
-from astropy import units as u
-
-from synphot import SourceSpectrum
-from synphot.units import PHOTLAM
-import skycalc_ipy
 
+from .effects import Effect
+from .ter_curves_utils import add_edge_zeros
 from .ter_curves_utils import combine_two_spectra, apply_throughput_to_cube
 from .ter_curves_utils import download_svo_filter, download_svo_filter_list
-from .ter_curves_utils import add_edge_zeros
-from .effects import Effect
+from ..base_classes import SourceBase, FOVSetupBase
 from ..optics.surface import SpectralSurface
-from ..source.source_utils import make_imagehdu_from_table
 from ..source.source import Source
-from ..base_classes import SourceBase, FOVSetupBase
 from ..utils import from_currsys, quantify, check_keys, find_file
 
 
 class TERCurve(Effect):
     """
     Transmission, Emissivity, Reflection Curve
 
     Must contain a wavelength column, and one or more of the following:
     ``transmission``, ``emissivity``, ``reflection``.
-    Additionally in the header there
+    Additionally, in the header there
     should be the following keywords: wavelength_unit
 
     kwargs that can be passed::
 
         "rescale_emission" : { "filter_name": str, "value": float, "unit": str}
 
     Examples
@@ -46,15 +41,15 @@
             array_dict:
                 wavelength: [0.3, 3.0]
                 transmission: [0.9, 0.9]
                 emission: [1, 1]
             wavelength_unit: um
             emission_unit: ph s-1 m-2 um-1
             rescale_emission:
-                filter_name: "Paranal/HAWKI.Ks"
+                filter_name: "Paranal/HAWK.Ks"
                 value: 15.5
                 unit: ABmag
 
     Indirectly inside a YAML file::
 
         name: some_curve
         class TERCurve
@@ -88,21 +83,24 @@
         self.surface.meta.update(self.meta)
         self._background_source = None
 
         data = self.get_data()
         if self.meta["ignore_wings"]:
             data = add_edge_zeros(data, "wavelength")
         if data is not None:
+            # Assert that get_data() did not give us an image.
+            assert isinstance(data, Table), "TER Curves must be tables."
             self.surface.table = data
             self.surface.table.meta.update(self.meta)
 
     # ####### added in new branch
 
     def apply_to(self, obj, **kwargs):
         if isinstance(obj, SourceBase):
+            assert isinstance(obj, Source), "Only Source supported."
             self.meta = from_currsys(self.meta)
             wave_min = quantify(self.meta["wave_min"], u.um).to(u.AA)
             wave_max = quantify(self.meta["wave_max"], u.um).to(u.AA)
 
             thru = self.throughput
 
             # apply transmission to source spectra
@@ -115,14 +113,16 @@
                 obj.cube_fields[icube] = apply_throughput_to_cube(cube, thru)
 
             # add the effect background to the source background field
             if self.background_source is not None:
                 obj.append(self.background_source)
 
         if isinstance(obj, FOVSetupBase):
+            from ..optics.fov_manager import FovVolumeList
+            assert isinstance(obj, FovVolumeList), "Only FovVolumeList supported."
             wave = self.surface.throughput.waveset
             thru = self.surface.throughput(wave)
             valid_waves = np.argwhere(thru > 0)
             wave_min = wave[max(0, valid_waves[0][0] - 1)]
             wave_max = wave[min(len(wave) - 1, valid_waves[-1][0] + 1)]
 
             obj.shrink("wave", [wave_min.to(u.um).value,
@@ -139,17 +139,25 @@
         return self.surface.throughput
 
     @property
     def background_source(self):
         if self._background_source is None:
             # add a single pixel ImageHDU for the extended background with a
             # size of 1 degree
-            bg_cell_width = from_currsys(self.meta["bg_cell_width"])
+            # bg_cell_width = from_currsys(self.meta["bg_cell_width"])
+
             flux = self.emission
             bg_hdu = fits.ImageHDU()
+            # TODO: The make_imagehdu_from_table below has been replaced with
+            #       the empty ImageHDU above in fbca416. That change might,
+            #       have been fine (or not?), but now there is no use anywhere
+            #       in the code of make_imagehdu_from_table or bg_cell_width,
+            #       so maybe these need to be removed?
+            # bg_hdu = make_imagehdu_from_table([0], [0], [1], bg_cell_width * u.arcsec)
+
             bg_hdu.header.update({"BG_SRC": True,
                                   "BG_SURF": self.display_name,
                                   "CUNIT1": "ARCSEC",
                                   "CUNIT2": "ARCSEC",
                                   "CDELT1": 0,
                                   "CDELT2": 0,
                                   "BUNIT": "PHOTLAM arcsec-2",
@@ -166,14 +174,16 @@
 
         Parameters
         ----------
         which : str
             "x" plots throughput. "t","e","r" plot trans/emission/refl
         wavelength : list, np.ndarray
         ax : matplotlib.Axis
+        new_figure : start a new figure (or add to the existing one)
+        label : the label to use (ignored)
         kwargs
 
         Returns
         -------
 
         """
         import matplotlib.pyplot as plt
@@ -209,18 +219,18 @@
                 y = surf.reflection(wave)
             else:
                 y = surf.throughput(wave)
 
             plt.plot(wave, y, **plot_kwargs)
 
             wave_unit = self.meta.get("wavelength_unit")
-            plt.xlabel("Wavelength [{}]".format(wave_unit))
+            plt.xlabel(f"Wavelength [{wave_unit}]")
             y_str = {"t": "Transmission", "e": "Emission",
                      "r": "Reflectivity", "x": "Throughput"}
-            plt.ylabel("{} [{}]".format(y_str[ter], y.unit))
+            plt.ylabel(f"{y_str[ter]} [{y.unit}]")
 
         return plt.gcf()
 
 
 class AtmosphericTERCurve(TERCurve):
     def __init__(self, **kwargs):
         super(AtmosphericTERCurve, self).__init__(**kwargs)
@@ -263,16 +273,19 @@
         """
         super(SkycalcTERCurve, self).__init__(**kwargs)
         self.meta["z_order"] = [112, 512]
         self.meta["use_local_skycalc_file"] = False
         self.meta.update(kwargs)
 
         self.skycalc_table = None
+        self.skycalc_conn = None
 
         if self.include is True:
+            # Only query the database if the effect is actually included.
+            # Sets skycalc_conn and skycalc_table.
             self.load_skycalc_table()
 
     @property
     def include(self):
         return from_currsys(self.meta["include"])
 
     @include.setter
@@ -325,15 +338,15 @@
         conn_kwargs = {key: self.meta[key] for key in self.meta
                        if key in self.skycalc_conn.defaults}
         conn_kwargs = from_currsys(conn_kwargs)
         self.skycalc_conn.values.update(conn_kwargs)
 
         try:
             tbl = self.skycalc_conn.get_sky_spectrum(return_type="table")
-        except:
+        except ConnectionError:
             msg = "Could not connect to skycalc server"
             logging.exception(msg)
             raise ValueError(msg)
 
         return tbl
 
 
@@ -372,16 +385,15 @@
             if "filter_name" in kwargs and "filename_format" in kwargs:
                 filt_name = from_currsys(kwargs["filter_name"])
                 file_format = from_currsys(kwargs["filename_format"])
                 kwargs["filename"] = file_format.format(filt_name)
             else:
                 raise ValueError("FilterCurve must be passed one of (`filename`"
                                  " `array_dict`, `table`) or both "
-                                 "(`filter_name`, `filename_format`):"
-                                 "{}".format(kwargs))
+                                 f"(`filter_name`, `filename_format`): {kwargs}")
 
         super(FilterCurve, self).__init__(**kwargs)
         if self.table is None:
             raise ValueError("Could not initialise filter. Either filename not "
                              "found, or array are not compatible")
 
         params = {"minimum_throughput": "!SIM.spectral.minimum_throughput",
@@ -422,26 +434,28 @@
             wave_edges = []
 
         return wave_edges
 
     @property
     def fwhm(self):
         wave = self.surface.wavelength
+        # noinspection PyProtectedMember
         thru = self.surface._get_ter_property("transmission", fmt="array")
         mask = thru >= 0.5
         if any(mask):
             dwave = wave[mask][-1] - wave[mask][0]
         else:
             dwave = 0 * wave.unit
 
         return dwave
 
     @property
     def centre(self):
         wave = self.surface.wavelength
+        # noinspection PyProtectedMember
         thru = self.surface._get_ter_property("transmission", fmt="array")
         num = np.trapz(thru * wave**2, x=wave)
         den = np.trapz(thru * wave, x=wave)
 
         return num / den
 
     @property
@@ -536,17 +550,15 @@
         check_keys(kwargs, required_keys, action="error")
         filt_str = "{}/{}.{}".format(kwargs["observatory"],
                                      kwargs["instrument"],
                                      kwargs["filter_name"])
         kwargs["name"] = kwargs["filter_name"]
         kwargs["svo_id"] = filt_str
 
-        raise_error = kwargs.get("error_on_wrong_name", True)
-        tbl = download_svo_filter(filt_str, return_style="table",
-                                  error_on_wrong_name=raise_error)
+        tbl = download_svo_filter(filt_str, return_style="table")
         super(SpanishVOFilterCurve, self).__init__(table=tbl, **kwargs)
 
 
 class FilterWheel(Effect):
     """
     This wheel holds a selection of predefined filters.
 
@@ -573,38 +585,36 @@
                   "path": "",
                   "report_plot_include": True,
                   "report_table_include": True,
                   "report_table_rounding": 4}
         self.meta.update(params)
         self.meta.update(kwargs)
 
-        path = pth.join(self.meta["path"],
-                        from_currsys(self.meta["filename_format"]))
+        path = Path(self.meta["path"], from_currsys(self.meta["filename_format"]))
         self.filters = {}
         for name in from_currsys(self.meta["filter_names"]):
             kwargs["name"] = name
-            self.filters[name] = FilterCurve(filename=path.format(name),
+            self.filters[name] = FilterCurve(filename=str(path).format(name),
                                              **kwargs)
 
         self.table = self.get_table()
 
-
     def apply_to(self, obj, **kwargs):
         """Use apply_to of current filter"""
         return self.current_filter.apply_to(obj, **kwargs)
 
     def fov_grid(self, which="waveset", **kwargs):
         return self.current_filter.fov_grid(which=which, **kwargs)
 
     def change_filter(self, filtername=None):
         """Change the current filter"""
         if filtername in self.filters.keys():
-            self.meta['current_filter'] = filtername
+            self.meta["current_filter"] = filtername
         else:
-            raise ValueError("Unknown filter requested: " + filtername)
+            raise ValueError(f"Unknown filter requested: {filtername}")
 
     def add_filter(self, newfilter, name=None):
         """
         Add a filter to the FilterWheel
 
         Parameters
         ==========
@@ -623,16 +633,16 @@
         filt_name = from_currsys(self.meta["current_filter"])
         if filt_name is not None:
             filter_eff = self.filters[filt_name]
         return filter_eff
 
     @property
     def display_name(self):
-        return f'{self.meta["name"]} : ' \
-               f'[{from_currsys(self.meta["current_filter"])}]'
+        return (f"{self.meta['name']} : "
+                f"[{from_currsys(self.meta['current_filter'])}]")
 
     def __getattr__(self, item):
         return getattr(self.current_filter, item)
 
     def plot(self, which="x", wavelength=None, **kwargs):
         """
 
@@ -648,18 +658,18 @@
 
         """
         import matplotlib.pyplot as plt
         plt.figure(figsize=(10, 5))
 
         for ii, ter in enumerate(which):
             ax = plt.subplot(len(which), 1, ii+1)
-            for name in self.filters:
-                self.filters[name].plot(which=ter, wavelength=wavelength,
-                                        ax=ax, new_figure=False,
-                                        plot_kwargs={"label": name}, **kwargs)
+            for name, _filter in self.filters.items():
+                _filter.plot(which=ter, wavelength=wavelength, ax=ax,
+                             new_figure=False, plot_kwargs={"label": name},
+                             **kwargs)
 
         # plt.semilogy()
         plt.legend()
 
         return plt.gcf()
 
     def get_table(self):
@@ -681,18 +691,18 @@
     A selection of top-hat filter curves as defined in the input lists
 
     Parameters
     ----------
     filter_names: list of string
 
     transmissions: list of floats
-        [0..1] Peak transmissions inside the cuttoff limits
+        [0..1] Peak transmissions inside the cutoff limits
 
     wing_transmissions: list of floats
-        [0..1] Wing transmissions outside the cuttoff limits
+        [0..1] Wing transmissions outside the cutoff limits
 
     blue_cutoffs: list of floats
         [um]
 
     red_cutoffs: list of floats
         [um]
 
@@ -747,15 +757,15 @@
     """
     A FilterWheel that loads all the filters from the Spanish VO service
 
     .. warning::
        This use ``astropy.download_file(..., cache=True)``.
 
     The filter transmission curves probably won't change, but if you notice
-    discrepancies, try clearing the astopy cache::
+    discrepancies, try clearing the astropy cache::
 
         >> from astropy.utils.data import clear_download_cache
         >> clear_download_cache()
 
     Parameters
     ----------
     observatory : str
@@ -799,15 +809,15 @@
                   "include_str": None,         # passed to
                   "exclude_str": None,
                   }
         self.meta.update(params)
         self.meta.update(kwargs)
 
         obs, inst = self.meta["observatory"], self.meta["instrument"]
-        inc, exc =  self.meta["include_str"], self.meta["exclude_str"]
+        inc, exc = self.meta["include_str"], self.meta["exclude_str"]
         filter_names = download_svo_filter_list(obs, inst, short_names=True,
                                                 include=inc, exclude=exc)
 
         self.meta["filter_names"] = filter_names
         self.filters = {name: SpanishVOFilterCurve(observatory=obs,
                                                    instrument=inst,
                                                    filter_name=name)
@@ -828,29 +838,25 @@
     characterised by "grey" transmissivity.
     The emissivity is set to zero, assuming that the mask is cold.
     """
     def __init__(self, transmission, **kwargs):
         self.params = {"wave_min": "!SIM.spectral.wave_min",
                        "wave_max": "!SIM.spectral.wave_max"}
         self.params.update(kwargs)
-        self.make_ter_curve(transmission)
-
-    def update_transmission(self, transmission, **kwargs):
-        self.params.update(kwargs)
-        self.make_ter_curve(transmission)
-
-    def make_ter_curve(self, transmission):
         wave_min = from_currsys(self.params["wave_min"]) * u.um
         wave_max = from_currsys(self.params["wave_max"]) * u.um
         transmission = from_currsys(transmission)
 
         super().__init__(wavelength=[wave_min, wave_max],
                          transmission=[transmission, transmission],
                          emissivity=[0., 0.], **self.params)
 
+    def update_transmission(self, transmission, **kwargs):
+        self.__init__(transmission, **kwargs)
+
 
 class ADCWheel(Effect):
     """
     This wheel holds a selection of predefined atmospheric dispersion
     correctors.
 
     Example
@@ -874,54 +880,53 @@
                   "path": "",
                   "report_plot_include": False,
                   "report_table_include": True,
                   "report_table_rounding": 4}
         self.meta.update(params)
         self.meta.update(kwargs)
 
-        path = pth.join(self.meta["path"],
-                        from_currsys(self.meta["filename_format"]))
+        path = Path(self.meta["path"], from_currsys(self.meta["filename_format"]))
         self.adcs = {}
         for name in from_currsys(self.meta["adc_names"]):
             kwargs["name"] = name
-            self.adcs[name] = TERCurve(filename=path.format(name),
+            self.adcs[name] = TERCurve(filename=str(path).format(name),
                                        **kwargs)
 
         self.table = self.get_table()
 
     def apply_to(self, obj, **kwargs):
         """Use apply_to of current adc"""
         return self.current_adc.apply_to(obj, **kwargs)
 
     def change_adc(self, adcname=None):
         """Change the current ADC"""
         if not adcname or adcname in self.adcs.keys():
-            self.meta['current_adc'] = adcname
+            self.meta["current_adc"] = adcname
             self.include = adcname
         else:
-            raise ValueError("Unknown ADC requested: " + adcname)
+            raise ValueError(f"Unknown ADC requested: {adcname}")
 
     @property
     def current_adc(self):
         """Return the currently used ADC"""
-        curradc = from_currsys(self.meta['current_adc'])
+        curradc = from_currsys(self.meta["current_adc"])
         if not curradc:
             return False
         return self.adcs[curradc]
 
     @property
     def display_name(self):
-        return f'{self.meta["name"]} : ' \
-               f'[{from_currsys(self.meta["current_adc"])}]'
+        return (f"{self.meta['name']} : "
+                f"[{from_currsys(self.meta['current_adc'])}]")
 
     def __getattr__(self, item):
         return getattr(self.current_adc, item)
 
     def get_table(self):
-        """Create a table of ADCs with maximimum througput"""
+        """Create a table of ADCs with maximum throughput"""
         names = list(self.adcs.keys())
         adcs = self.adcs.values()
-        tmax = np.array([adc.data['transmission'].max() for adc in adcs])
+        tmax = np.array([adc.data["transmission"].max() for adc in adcs])
 
         tbl = Table(names=["name", "max_transmission"],
                     data=[names, tmax])
         return tbl
```

### Comparing `ScopeSim-0.5.6/scopesim/effects/ter_curves_utils.py` & `ScopeSim-0.6.0/scopesim/effects/ter_curves_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from pathlib import Path
 
 import numpy as np
 from astropy import units as u
 from astropy.table import Table
 from astropy.utils.data import download_file
 from astropy.io import ascii as ioascii
@@ -40,29 +39,29 @@
                    "PaBeta": "Gemini/NIRI.PaBeta-G0221",
                    "BrGamma": "Gemini/NIRI.BrG-G0218",
                    }
 
 PATH_HERE = Path(__file__).parent
 PATH_SVO_DATA = PATH_HERE.parent / "data" / "svo"
 
+
 def get_filter_effective_wavelength(filter_name):
     if isinstance(filter_name, str):
         filter_name = from_currsys(filter_name)
         wave, trans = download_svo_filter(FILTER_DEFAULTS[filter_name],
                                           return_style="quantity")
         eff_wave = np.sum(wave * trans) / np.sum(trans)      # convert from Angstrom
         eff_wave = eff_wave.to(u.um)
     else:
         eff_wave = filter_name
 
     return eff_wave
 
 
-def download_svo_filter(filter_name, return_style="synphot",
-                        error_on_wrong_name=True):
+def download_svo_filter(filter_name, return_style="synphot"):
     """
     Query the SVO service for the true transmittance for a given filter
 
     Copied 1 to 1 from tynt by Brett Morris
 
     Parameters
     ----------
@@ -74,56 +73,48 @@
         Defines the format the data is returned
         - synphot: synphot.SpectralElement
         - table: astropy.table.Table
         - quantity: astropy.unit.Quantity [wave, trans]
         - array: np.ndarray [wave, trans], where wave is in Angstrom
         - vo_table : astropy.table.Table - original output from SVO service
 
-    error_on_wrong_name : bool
-        Default True. Raises an exception if filter_name is as incorrect SVO ID
-
     Returns
     -------
     filt_curve : See return_style
         Astronomical filter object.
 
     """
+    # The SVO is only accessible over http, not over https.
+    # noinspection HttpUrlsUsage
     url = f"http://svo2.cab.inta-csic.es/theory/fps3/fps.php?ID={filter_name}"
     path = find_file(
         filter_name,
         path=[PATH_SVO_DATA],
         silent=True,
     )
     if not path:
         path = download_file(url, cache=True)
 
-    try:
-        tbl = Table.read(path, format='votable')
-        wave = u.Quantity(tbl['Wavelength'].data.data, u.Angstrom, copy=False)
-        trans = tbl['Transmission'].data.data
-    except:
-        if error_on_wrong_name:
-            raise ValueError(f"{filter_name} is an incorrect SVO identiier")
-        else:
-            logging.warning(f"'{filter_name}' was not found in the SVO. "
-                            f"Defaulting to a unity transmission curve.")
-            wave = [3e3, 3e5] << u.Angstrom
-            trans = np.array([1., 1.])
+    tbl = Table.read(path, format='votable')
+    wave = u.Quantity(tbl['Wavelength'].data.data, u.Angstrom, copy=False)
+    trans = tbl['Transmission'].data.data
 
     if return_style == "synphot":
         filt = SpectralElement(Empirical1D, points=wave, lookup_table=trans)
     elif return_style == "table":
         filt = Table(data=[wave, trans], names=["wavelength", "transmission"])
         filt.meta["wavelength_unit"] = "Angstrom"
     elif return_style == "quantity":
         filt = [wave, trans]
     elif return_style == "array":
         filt = [wave.value, trans]
     elif return_style == "vo_table":
         filt = tbl
+    else:
+        raise ValueError("return_style %s unknown.", return_style)
 
     return filt
 
 
 def download_svo_filter_list(observatory, instrument, short_names=False,
                              include=None, exclude=None):
     """
@@ -150,15 +141,17 @@
 
     Returns
     -------
     names : list
         A list of filter names
 
     """
-    base_url = f"http://svo2.cab.inta-csic.es/theory/fps3/fps.php?"
+    # The SVO is only accessible over http, not over https.
+    # noinspection HttpUrlsUsage
+    base_url = "http://svo2.cab.inta-csic.es/theory/fps3/fps.php?"
     url = base_url + f"Facility={observatory}&Instrument={instrument}"
     fn = f"{observatory}/{instrument}"
     path = find_file(
         fn,
         path=[PATH_SVO_DATA],
         silent=True,
     )
@@ -189,27 +182,29 @@
         filt = SpectralElement(Empirical1D, points=wave,
                                lookup_table=tbl["transmission"])
     elif filter_name in FILTER_DEFAULTS:
         filt = download_svo_filter(FILTER_DEFAULTS[filter_name])
     else:
         try:
             filt = download_svo_filter(filter_name)
-        except:
+        except ConnectionError:
             filt = None
 
     return filt
 
 
 def get_zero_mag_spectrum(system_name="AB"):
     if system_name.lower() in ["vega"]:
         spec = vega_spectrum()
     elif system_name.lower() in ["ab"]:
         spec = ab_spectrum()
     elif system_name.lower() in ["st", "hst"]:
         spec = st_spectrum()
+    else:
+        raise ValueError("system_name %s is unknown", system_name)
 
     return spec
 
 
 def zero_mag_flux(filter_name, photometric_system, return_filter=False):
     """
     Returns the zero magnitude photon flux for a filter
@@ -320,14 +315,15 @@
 
     real_flux = Observation(spectrum, filt).effstim(flux_unit=PHOTLAM)
     scale_factor = ref_flux / real_flux
     spectrum *= scale_factor.value
 
     return spectrum
 
+
 def apply_throughput_to_cube(cube, thru):
     """
     Apply throughput curve to a spectroscopic cube
 
     Parameters
     ----------
     cube : ImageHDU
@@ -342,14 +338,15 @@
     """
     wcs = WCS(cube.header).spectral
     wave_cube = wcs.all_pix2world(np.arange(cube.data.shape[0]), 0)[0]
     wave_cube = (wave_cube * u.Unit(wcs.wcs.cunit[0])).to(u.AA)
     cube.data *= thru(wave_cube).value[:, None, None]
     return cube
 
+
 def combine_two_spectra(spec_a, spec_b, action, wave_min, wave_max):
     """
     Combines transmission and/or emission spectrum with a common waverange
 
     Spec_A is the source spectrum
     Spec_B is either the transmission or emission that should be applied
 
@@ -372,24 +369,26 @@
     else:
         wave_val = spec_a.waveset.value
     mask = (wave_val > wave_min.value) * (wave_val < wave_max.value)
 
     wave = ([wave_min.value] + list(wave_val[mask]) + [wave_max.value]) * u.AA
     if "mult" in action.lower():
         spec_c = spec_a(wave) * spec_b(wave)
-        ## Diagnostic plots - not for general use
+        # Diagnostic plots - not for general use
         # from matplotlib import pyplot as plt
         # plt.plot(wave, spec_a(wave), label="spec_a")
         # plt.plot(wave, spec_b(wave), label="spec_b")
         # plt.plot(wave, spec_c, label="spec_c")
         # plt.xlim(2.9e4, 4.2e4)
         # plt.legend()
         # plt.show()
     elif "add" in action.lower():
         spec_c = spec_a(wave) + spec_b(wave)
+    else:
+        raise ValueError(f"action {action} unknown")
 
     new_source = SourceSpectrum(Empirical1D, points=wave, lookup_table=spec_c)
     new_source.meta.update(spec_b.meta)
     new_source.meta.update(spec_a.meta)
 
     return new_source
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/OLD_fov.py` & `ScopeSim-0.6.0/scopesim/optics/OLD_fov.py`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/optics/OLD_fov_manager.py` & `ScopeSim-0.6.0/scopesim/optics/OLD_fov_manager.py`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/optics/fov.py` & `ScopeSim-0.6.0/scopesim/optics/fov.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
         self._wavelength = None
         self._volume = None
 
     @property
     def pixel_area(self):
         if self.meta["pixel_area"] is None:
             hdr = self.header
-            pixarea = (hdr['CDELT1'] * u.Unit(hdr['CUNIT1']) *
-                       hdr['CDELT2'] * u.Unit(hdr['CUNIT2'])).to(u.arcsec ** 2)
+            pixarea = (hdr["CDELT1"] * u.Unit(hdr["CUNIT1"]) *
+                       hdr["CDELT2"] * u.Unit(hdr["CUNIT2"])).to(u.arcsec ** 2)
             self.meta["pixel_area"] = pixarea.value     # [arcsec]
 
         return self.meta["pixel_area"]
 
     def extract_from(self, src):
         """ ..assumption: Bandpass has been applied
 
@@ -293,18 +293,18 @@
                                          header=self.header)
 
         # 2. Find Cube fields
         for field in self.cube_fields:
             # cube_fields come in with units of photlam/arcsec2, need to convert to ph/s
             # We need to the voxel volume (spectral and solid angle) for that.
             # ..todo: implement branch for use_photlam is True
-            spectral_bin_width = (field.header['CDELT3'] *
-                                  u.Unit(field.header['CUNIT3'])).to(u.Angstrom)
-            pixarea = (field.header['CDELT1'] * u.Unit(field.header['CUNIT1']) *
-                       field.header['CDELT2'] * u.Unit(field.header['CUNIT2'])).to(u.arcsec**2)
+            spectral_bin_width = (field.header["CDELT3"] *
+                                  u.Unit(field.header["CUNIT3"])).to(u.Angstrom)
+            pixarea = (field.header["CDELT1"] * u.Unit(field.header["CUNIT1"]) *
+                       field.header["CDELT2"] * u.Unit(field.header["CUNIT2"])).to(u.arcsec**2)
 
             # First collapse to image, then convert units
             image = np.sum(field.data, axis=0) * PHOTLAM/u.arcsec**2
             image = (image * pixarea * area * spectral_bin_width).to(u.ph/u.s)
 
             tmp_hdu = fits.ImageHDU(data=image, header=field.header)
             canvas_image_hdu = imp_utils.add_imagehdu_to_imagehdu(
@@ -461,18 +461,18 @@
             field_interp = interp1d(field_waveset.to(u.um).value,
                                     field.data, axis=0, kind="linear",
                                     bounds_error=False, fill_value=0)
 
             field_data = field_interp(fov_waveset.value)
 
             # Pixel scale conversion
-            field_pixarea = (field.header['CDELT1']
-                             * field.header['CDELT2']
-                             * u.Unit(field.header['CUNIT1'])
-                             * u.Unit(field.header['CUNIT2'])).to(u.arcsec**2)
+            field_pixarea = (field.header["CDELT1"]
+                             * field.header["CDELT2"]
+                             * u.Unit(field.header["CUNIT1"])
+                             * u.Unit(field.header["CUNIT2"])).to(u.arcsec**2)
             field_pixarea = field_pixarea.value
             field_data *= field_pixarea / self.pixel_area
             field_hdu = fits.ImageHDU(data=field_data, header=field.header)
             canvas_cube_hdu = imp_utils.add_imagehdu_to_imagehdu(
                 field_hdu,
                 canvas_cube_hdu,
                 spline_order=spline_order)
@@ -481,16 +481,16 @@
         for field in self.image_fields:
             # Cube should be in PHOTLAM arcsec-2 for SpectralTrace mapping
             # Assumption is that ImageHDUs have units of PHOTLAM arcsec-2
             # ImageHDUs have photons/second/pixel.
             # ..todo: Add a catch to get ImageHDU with BUNITs
             canvas_image_hdu = fits.ImageHDU(data=np.zeros((naxis2, naxis1)),
                                              header=self.header)
-            pixarea = (field.header['CDELT1'] * u.Unit(field.header['CUNIT1']) *
-                       field.header['CDELT2'] * u.Unit(field.header['CUNIT2'])).to(u.arcsec**2)
+            pixarea = (field.header["CDELT1"] * u.Unit(field.header["CUNIT1"]) *
+                       field.header["CDELT2"] * u.Unit(field.header["CUNIT2"])).to(u.arcsec**2)
 
             field.data = field.data / self.pixel_area
             canvas_image_hdu = imp_utils.add_imagehdu_to_imagehdu(field,
                                                     canvas_image_hdu,
                                                     spline_order=spline_order)
             spec = specs[field.header["SPEC_REF"]]
             field_cube = canvas_image_hdu.data[None, :, :] * spec[:, None, None]  # 2D * 1D -> 3D
@@ -641,18 +641,22 @@
     @property
     def background_fields(self):
         return [field for field in self.fields
                 if isinstance(field, fits.ImageHDU)
                 and field.header.get("BG_SRC", False) is True]
 
     def __repr__(self):
-        msg = "FOV id: {}, with dimensions ({}, {})\n" \
-              "".format(self.meta["id"], self.header["NAXIS1"],
-                        self.header["NAXIS2"])
-        msg += "Sky centre: ({}, {})\n" \
-               "".format(self.header["CRVAL1"], self.header["CRVAL2"])
-        msg += "Image centre: ({}, {})\n" \
-               "".format(self.header["CRVAL1D"], self.header["CRVAL2D"])
-        msg += "Wavelength range: ({}, {})um\n" \
-               "".format(self.meta["wave_min"], self.meta["wave_max"])
+        waverange = [self.meta["wave_min"].value, self.meta["wave_max"].value]
+        msg = (f"{self.__class__.__name__}({self.header!r}, {waverange!r}, "
+               f"{self.detector_header!r}, **{self.meta!r})")
+        return msg
 
+    def __str__(self):
+        msg = (f"FOV id: {self.meta['id']}, with dimensions "
+               f"({self.header['NAXIS1']}, {self.header['NAXIS2']})\n"
+               f"Sky centre: ({self.header['CRVAL1']}, "
+               f"{self.header['CRVAL2']})\n"
+               f"Image centre: ({self.header['CRVAL1D']}, "
+               f"{self.header['CRVAL2D']})\n"
+               f"Wavelength range: ({self.meta['wave_min']}, "
+               f"{self.meta['wave_max']})um\n")
         return msg
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/fov_manager.py` & `ScopeSim-0.6.0/scopesim/optics/fov_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,20 +38,21 @@
 # Imaging dependent on:
 # - Detector array borders
 # - PSF wavelength granularity
 # - Atmospheric dispersion
 #
 # """
 
-from copy import deepcopy, copy
+from copy import deepcopy
 import numpy as np
-from astropy.table import Table
+from typing import TextIO
+from io import StringIO
+
 from astropy import units as u
 
-from . import fov_manager_utils as fmu
 from . import image_plane_utils as ipu
 from ..effects import DetectorList
 from ..effects import effects_utils as eu
 from ..utils import from_currsys
 
 from .fov import FieldOfView
 from ..base_classes import FOVSetupBase
@@ -156,16 +157,16 @@
             # useful for spectroscopy mode where slit dimensions is not the same
             # as detector dimensions
             # ..todo: Make sure this changes for multiple image planes
             if from_currsys(self.meta["decouple_sky_det_hdrs"]) is True:
                 det_eff = eu.get_all_effects(self.effects, DetectorList)[0]
                 dethdr = det_eff.image_plane_header
 
-            fovs += [FieldOfView(skyhdr, waverange, detector_header=dethdr,
-                                 **vol["meta"])]
+            fovs.append(FieldOfView(skyhdr, waverange, detector_header=dethdr,
+                                    **vol["meta"]))
 
         return fovs
 
     @property
     def fovs(self):
         if from_currsys(self.meta["preload_fovs"]) is False:
             self._fovs_list = self.generate_fovs_list()
@@ -187,15 +188,17 @@
     wave : [um]
         On-sky wavelengths
     xd, yd : [mm]
         Detector plane coordinates relative to centre of ImagePlane
 
     """
 
-    def __init__(self, initial_volume={}):
+    def __init__(self, initial_volume=None):
+        if initial_volume is None:
+            initial_volume = {}
 
         self.volumes = [{"wave_min": 0.3,
                          "wave_max": 30,
                          "x_min": -1800,
                          "x_max": 1800,
                          "y_min": -1800,
                          "y_max": 1800,
@@ -286,23 +289,23 @@
         else:
             to_pop = []
 
             if values[0] is not None:
                 for i, vol in enumerate(self.volumes):
                     if aperture_id in (vol["meta"]["aperture_id"], None):
                         if vol[f"{axis}_max"] <= values[0]:
-                            to_pop += [i]
+                            to_pop.append(i)
                         elif vol[f"{axis}_min"] < values[0]:
                             vol[f"{axis}_min"] = values[0]
 
             if values[1] is not None:
                 for i, vol in enumerate(self.volumes):
                     if aperture_id in (vol["meta"]["aperture_id"], None):
                         if vol[f"{axis}_min"] >= values[1]:
-                            to_pop += [i]
+                            to_pop.append(i)
                         if vol[f"{axis}_max"] > values[1]:
                             vol[f"{axis}_max"] = values[1]
 
             for i in sorted(to_pop)[::-1]:
                 self.volumes.pop(i)
 
     def extract(self, axes, edges, aperture_id=None):
@@ -352,34 +355,57 @@
                        edge[1] >= old_vol[f"{axis}_min"]:
                         new_vol[f"{axis}_min"] = max(edge[0], old_vol[f"{axis}_min"])
                         new_vol[f"{axis}_max"] = min(edge[1], old_vol[f"{axis}_max"])
                     else:
                         add_flag = False
 
                 if add_flag is True:
-                    new_vols += [new_vol]
+                    new_vols.append(new_vol)
 
         return new_vols
 
     def __len__(self):
         return len(self.volumes)
 
-    def __getitem__(self, item):
-        return self.volumes[item]
+    def __iter__(self):
+        return iter(self.volumes)
+
+    def __getitem__(self, key):
+        return self.volumes[key]
 
     def __setitem__(self, key, value):
         self.volumes[item] = value
 
-    def __repr__(self):
-        text = f"FovVolumeList with [{len(self.volumes)}] volumes:\n"
-        for i, vol in enumerate(self.volumes):
-            mini_text = ", ".join([f"{key}: {val}" for key, val in vol.items()])
-            text += f"  [{i}] {mini_text} \n"
+    def __delitem__(self, key):
+        del self.volumes[key]
 
-        return text
+    def write_string(self, stream: TextIO) -> None:
+        """Write formatted string representation to I/O stream"""
+        n_vol = len(self.volumes)
+        stream.write(f"FovVolumeList with {n_vol} volumes:")
+        max_digits = len(str(n_vol))
+
+        for i_vol, vol in enumerate(self.volumes):
+            pre = "\n└─" if i_vol == n_vol - 1 else "\n├─"
+            stream.write(f"{pre}[{i_vol:>{max_digits}}]:")
+
+            pre = "\n  " if i_vol == n_vol - 1 else "\n│ "
+            n_key = len(vol)
+            for i_key, (key, val) in enumerate(vol.items()):
+                subpre = "└─" if i_key == n_key - 1 else "├─"
+                stream.write(f"{pre}{subpre}{key}: {val}")
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.volumes[0]})"
+
+    def __str__(self) -> str:
+        with StringIO() as str_stream:
+            self.write_string(str_stream)
+            output = str_stream.getvalue()
+        return output
 
     def __iadd__(self, other):
         if isinstance(other, list):
             self.volumes += other
         else:
             raise ValueError(f"Can only add lists of volumes: {other}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/fov_manager_utils.py` & `ScopeSim-0.6.0/scopesim/optics/fov_manager_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,16 +101,15 @@
                       for filt in filters]
     if len(wave_bin_edges) > 0:
         kwargs["wave_min"] = np.max([w[0].value for w in wave_bin_edges])
         kwargs["wave_max"] = np.min([w[1].value for w in wave_bin_edges])
     wave_bin_edges = [[kwargs["wave_min"], kwargs["wave_max"]]]
 
     if kwargs["wave_min"] > kwargs["wave_max"]:
-        raise ValueError("Filter wavelength ranges do not overlap: {}"
-                         "".format(wave_bin_edges))
+        raise ValueError(f"Filter wavelength ranges do not overlap: {wave_bin_edges}")
 
     # ..todo: add in Atmospheric dispersion and ADC here
     for effect_class in [efs.PSF]:
         effects = get_all_effects(effects_list, effect_class)
         for eff in effects:
             waveset = eff.fov_grid(which="waveset", **kwargs)
             if waveset is not None:
@@ -169,15 +168,15 @@
         if len(detector_arrays) > 0:
             aperture_effects += [detarr.fov_grid(which="edges",
                                                  pixel_scale=pixel_scale)
                                  for detarr in detector_arrays]
         else:
             raise ValueError("No ApertureMask or DetectorList was provided. At "
                              "least one must be passed to make an ImagePlane: "
-                             "{}".format(effects))
+                             f"{effects}")
 
     # get aperture headers from fov_grid()
     # - for-loop catches mutliple headers from ApertureList.fov_grid()
     hdrs = []
     for ap_eff in aperture_effects:
         # ..todo:: add this functionality to ApertureList effect
         hdr = ap_eff.fov_grid(which="edges", pixel_scale=pixel_scale)
@@ -243,16 +242,15 @@
     if len(shifts["wavelengths"]) > 0:
         mask = (shift_waves > np.min(waveset)) * (shift_waves < np.max(waveset))
         waveset = combine_wavesets([waveset, shift_waves[mask]])
 
     counter = 0
     fovs = []
 
-    print("Preparing {} FieldOfViews".format((len(waveset)-1)*len(headers)),
-          flush=True)
+    print(f"Preparing {(len(waveset)-1)*len(headers)} FieldOfViews", flush=True)
 
     for ii in range(len(waveset) - 1):
         for hdr in headers:
             # add any pre-instrument shifts to the FOV sky coords
             wave_mid = 0.5 * (waveset[ii] + waveset[ii+1])
             x_shift = np.interp(wave_mid, shift_waves, shift_dx)
             y_shift = np.interp(wave_mid, shift_waves, shift_dy)
@@ -298,16 +296,16 @@
     elif len(spec_trace_effects) > 0:
         implane_hdr = spec_trace_effects[0].image_plane_header
     else:
         raise ValueError("Missing a way to determine the image plane size")
 
     # ..todo: deal with multiple trace lists
     if len(spec_trace_effects) != 1:
-        raise ValueError("More than one SpectralTraceList was found: {}"
-                         "".format(spec_trace_effects))
+        raise ValueError("More than one SpectralTraceList was found: "
+                         f"{spec_trace_effects}")
     spec_trace = spec_trace_effects[0]
 
     sky_hdrs = []
     for ap_eff in aperture_effects:
         # if ApertureList, a list of ApertureMask headers is returned
         # If ApertureMask, a single header is returned
         hdr = ap_eff.fov_grid(which="edges", pixel_scale=kwargs["pixel_scale"])
@@ -330,15 +328,15 @@
 
 def get_spectroscopy_fovs(headers, shifts, effects=[], **kwargs):
 
     shift_waves = shifts["wavelengths"]     # in [um]
     shift_dx = shifts["x_shifts"]           # in [deg]
     shift_dy = shifts["y_shifts"]
 
-    print("Preparing {} FieldOfViews".format(len(headers)), flush=True)
+    print(f"Preparing {len(headers)} FieldOfViews", flush=True)
 
     apertures = get_all_effects(effects, (efs.ApertureList, efs.ApertureMask))
     masks = [ap.fov_grid(which="masks") for ap in apertures]
     mask_dict = {}
     for mask in masks:
         if isinstance(mask, dict):
             mask_dict.update(mask)
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/fov_utils.py` & `ScopeSim-0.6.0/scopesim/optics/fov_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,15 @@
                                                u.arcsec).to(u.deg).value)
             s = wcs_suffix
             cdelt = utils.quantify(fov_header["CDELT1" + s], u.deg).value
             field_header = imp_utils.header_from_list_of_xy(x, y, cdelt, s)
         elif isinstance(field, (fits.ImageHDU, fits.PrimaryHDU)):
             field_header = field.header
         else:
-            logging.warning("Input was neither Table nor ImageHDU: {}"
-                          "".format(field))
+            logging.warning("Input was neither Table nor ImageHDU: %s", field)
             return False
 
         ext_xsky, ext_ysky = imp_utils.calc_footprint(field_header, wcs_suffix)
         fov_xsky, fov_ysky = imp_utils.calc_footprint(fov_header, wcs_suffix)
 
         is_inside_fov = min(ext_xsky) < max(fov_xsky) and \
                         max(ext_xsky) > min(fov_xsky) and \
@@ -226,16 +225,16 @@
 
     """
     if isinstance(field, Table):
         field_new = extract_area_from_table(field, fov_volume)
     elif isinstance(field, fits.ImageHDU):
         field_new = extract_area_from_imagehdu(field, fov_volume)
     else:
-        raise ValueError("field must be either Table or ImageHDU: {}"
-                         "".format(type(field)))
+        raise ValueError("field must be either Table or ImageHDU, but is "
+                         f"{type(field)}")
 
     return field_new
 
 
 def extract_area_from_table(table, fov_volume):
     """
     Extracts the entries of a Table that fits inside the fov_volume
@@ -270,36 +269,40 @@
 def extract_area_from_imagehdu(imagehdu, fov_volume):
     """
     Extracts the part of a ImageHDU that fits inside the fov_volume
 
     Parameters
     ----------
     imagehdu : fits.ImageHDU
-        The field ImageHDU, either an image of a wavelength [um] cube
+        The field ImageHDU, either an image or a cube with wavelength [um]
     fov_volume : dict
         Contains {"xs": [xmin, xmax], "ys": [ymin, ymax],
                   "waves": [wave_min, wave_max],
                   "xy_unit": "deg" or "mm", "wave_unit": "um"}
 
     Returns
     -------
     new_imagehdu : fits.ImageHDU
 
     """
     hdr = imagehdu.header
     new_hdr = {}
-
+    naxis1, naxis2 = hdr["NAXIS1"], hdr["NAXIS2"]
     x_hdu, y_hdu = imp_utils.calc_footprint(imagehdu)  # field edges in "deg"
     x_fov, y_fov = fov_volume["xs"], fov_volume["ys"]
 
     x0s, x1s = max(min(x_hdu), min(x_fov)), min(max(x_hdu), max(x_fov))
     y0s, y1s = max(min(y_hdu), min(y_fov)), min(max(y_hdu), max(y_fov))
 
     xp, yp = imp_utils.val2pix(hdr, np.array([x0s, x1s]), np.array([y0s, y1s]))
-    (x0p, x1p), (y0p, y1p) = np.round(xp).astype(int), np.round(yp).astype(int)
+    x0p = max(0, np.floor(xp[0]).astype(int))
+    x1p = min(naxis1, np.ceil(xp[1]).astype(int))
+    y0p = max(0, np.floor(yp[0]).astype(int))
+    y1p = min(naxis2, np.ceil(yp[1]).astype(int))
+    # (x0p, x1p), (y0p, y1p) = np.round(xp).astype(int), np.round(yp).astype(int)
     if x0p == x1p:
         x1p += 1
     if y0p == y1p:
         y1p += 1
 
     new_hdr = imp_utils.header_from_list_of_xy([x0s, x1s], [y0s, y1s],
                                                pixel_scale=hdr["CDELT1"])
@@ -322,15 +325,15 @@
         wunit = u.Unit(hdr.get("CUNIT3", "AA"))
         fov_waves = utils.quantify(fov_volume["waves"], u.um).to(wunit).value
         mask = ((hdu_waves > fov_waves[0] - 0.5 * wdel) *
                 (hdu_waves <= fov_waves[1] + 0.5 * wdel))  # need to go [+/-] half a bin
 
         # OC [2021-12-14] if fov range is not covered by the source return nothing
         if not np.any(mask):
-            print("FOV {} um - {} um: not covered by Source".format(fov_waves[0], fov_waves[1]))
+            print(f"FOV {fov_waves[0]} um - {fov_waves[1]} um: not covered by Source")
             return None
 
         i0p, i1p = np.where(mask)[0][0], np.where(mask)[0][-1]
         f0 = (abs(hdu_waves[i0p] - fov_waves[0] + 0.5 * wdel) % wdel) / wdel    # blue edge
         f1 = (abs(hdu_waves[i1p] - fov_waves[1] - 0.5 * wdel) % wdel) / wdel    # red edge
         data = imagehdu.data[i0p:i1p+1, y0p:y1p, x0p:x1p]
         data[0, :, :] *= f0
@@ -389,21 +392,21 @@
                          f"{type(spectrum)}")
 
     wave_min, wave_max = utils.quantify(waverange, u.um).to(u.AA).value
     spec_waveset = spectrum.waveset.to(u.AA).value
     mask = (spec_waveset > wave_min) * (spec_waveset < wave_max)
 
     if sum(mask) == 0:
-        logging.info(f"Waverange does not overlap with Spectrum waveset: "
-                      f"{[wave_min, wave_max]} <> {spec_waveset} "
-                      f"for spectrum {spectrum}")
+        logging.info(("Waverange does not overlap with Spectrum waveset: "
+                      "%s <> %s for spectrum %s"),
+                     [wave_min, wave_max], spec_waveset, spectrum)
     if wave_min < min(spec_waveset) or wave_max > max(spec_waveset):
-        logging.info(f"Waverange only partially overlaps with Spectrum waveset: "
-                      f"{[wave_min, wave_max]} <> {spec_waveset} "
-                      f"for spectrum {spectrum}")
+        logging.info(("Waverange only partially overlaps with Spectrum waveset: "
+                      "%s <> %s for spectrum %s"),
+                     [wave_min, wave_max], spec_waveset, spectrum)
 
     wave = np.r_[wave_min, spec_waveset[mask], wave_max]
     flux = spectrum(wave)
 
     new_spectrum = SourceSpectrum(Empirical1D, points=wave, lookup_table=flux)
     new_spectrum.meta.update(spectrum.meta)
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/image_plane.py` & `ScopeSim-0.6.0/scopesim/optics/image_plane.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,18 +46,18 @@
     def __init__(self, header, **kwargs):
 
         max_seg_size = rc.__config__["!SIM.computing.max_segment_size"]
         self.meta = {"SIM_MAX_SEGMENT_SIZE" : max_seg_size}
         self.meta.update(kwargs)
         self.id = header["IMGPLANE"] if "IMGPLANE" in header else 0
 
-        if not any([utils.has_needed_keywords(header, s)
-                    for s in ["", "D", "S"]]):
-            raise ValueError("header must have a valid image-plane WCS: {}"
-                             "".format(dict(header)))
+        if not any(utils.has_needed_keywords(header, s)
+                   for s in ["", "D", "S"]):
+            raise ValueError(f"header must have a valid image-plane WCS: "
+                             f"{dict(header)}")
 
         image = np.zeros((header["NAXIS2"]+1, header["NAXIS1"]+1))
         self.hdu = fits.ImageHDU(data=image, header=header)
 
     def add(self, hdus_or_tables, sub_pixel=None, spline_order=None, wcs_suffix=""):
         """
         Add a projection of an image or table files to the canvas
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/image_plane_utils.py` & `ScopeSim-0.6.0/scopesim/optics/image_plane_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,37 +28,37 @@
     Returns
     -------
     header : fits.Header
         A Header containing a WCS and NAXISn values to build an ImageHDU
 
     """
 
-    size_warning = "Header dimension are {} large: {}. Any image made from " \
-                   "this header will use more that >{} in memory"
+    size_warning = ("Header dimension are {adverb} large: {num_pix}. Any image "
+                    "made from this header will use more that >{size} in memory")
 
     headers = [ht.header for ht in hdu_or_table_list
                if isinstance(ht, fits.ImageHDU)]
-    if sum([isinstance(ht, Table) for ht in hdu_or_table_list]) > 0:
+    if any(isinstance(ht, Table) for ht in hdu_or_table_list):
         tbls = [ht for ht in hdu_or_table_list if isinstance(ht, Table)]
         tbl_hdr = _make_bounding_header_for_tables(tbls,
                                                    pixel_scale=pixel_scale)
-        headers += [tbl_hdr]
+        headers.append(tbl_hdr)
 
-    if len(headers) > 0:
-        hdr = _make_bounding_header_from_imagehdus(headers,
-                                                   pixel_scale=pixel_scale)
-        num_pix = hdr["NAXIS1"] * hdr["NAXIS2"]
-        if num_pix > 2 ** 25:  # 2 * 4096**2
-            logging.warning(size_warning.format("", num_pix, "256 MB"))
-        elif num_pix > 2 ** 28:
-            raise MemoryError(size_warning.format("too", num_pix, "8 GB"))
-    else:
+    if not headers:
         logging.warning("No tables or ImageHDUs were passed")
-        hdr = None
+        return None
 
+    hdr = _make_bounding_header_from_imagehdus(headers, pixel_scale=pixel_scale)
+    num_pix = hdr["NAXIS1"] * hdr["NAXIS2"]
+    if num_pix > 2 ** 28:
+        raise MemoryError(size_warning.format(adverb="too", num_pix=num_pix,
+                                              size="8 GB"))
+    if num_pix > 2 ** 25:  # 2 * 4096**2
+        logging.warning(size_warning.format(adverb="", num_pix=num_pix,
+                                            size="256 MB"))
     return hdr
 
 
 def _make_bounding_header_from_imagehdus(imagehdus, pixel_scale=1*u.arcsec):
     """
     Returns a Header with WCS and NAXISn keywords bounding all input ImageHDUs
 
@@ -235,16 +235,15 @@
     -------
     canvas_hdu : fits.ImageHDU
 
     """
 
     s = wcs_suffix
     if not utils.has_needed_keywords(canvas_hdu.header, s):
-        raise ValueError("canvas_hdu must include an appropriate WCS: {}"
-                         "".format(s))
+        raise ValueError(f"canvas_hdu must include an appropriate WCS: {s}")
 
     f = utils.quantity_from_table("flux", table, default_unit=u.Unit("ph s-1"))
     if s == "D":
         x = utils.quantity_from_table("x_mm", table, default_unit=u.mm).to(u.mm)
         y = utils.quantity_from_table("y_mm", table, default_unit=u.mm).to(u.mm)
     else:
         arcsec = u.arcsec
@@ -267,28 +266,26 @@
         canvas_hdu = _add_intpixel_sources_to_canvas(canvas_hdu, xpix, ypix, f,
                                                      mask)
 
     return canvas_hdu
 
 
 def _add_intpixel_sources_to_canvas(canvas_hdu, xpix, ypix, flux, mask):
-    canvas_hdu.header["comment"] = "Adding {} int-pixel files" \
-                                   "".format(len(flux))
+    canvas_hdu.header["comment"] = f"Adding {len(flux)} int-pixel files"
     xpix = xpix.astype(int)
     ypix = ypix.astype(int)
     for ii in range(len(xpix)):
         if mask[ii]:
             canvas_hdu.data[ypix[ii], xpix[ii]] += flux[ii].value
 
     return canvas_hdu
 
 
 def _add_subpixel_sources_to_canvas(canvas_hdu, xpix, ypix, flux, mask):
-    canvas_hdu.header["comment"] = "Adding {} sub-pixel files" \
-                                   "".format(len(flux))
+    canvas_hdu.header["comment"] = f"Adding {len(flux)} sub-pixel files"
     canvas_shape = canvas_hdu.data.shape
     for ii in range(len(xpix)):
         if mask[ii]:
             xx, yy, fracs = sub_pixel_fractions(xpix[ii], ypix[ii])
             for x, y, frac in zip(xx, yy, fracs):
                 if y < canvas_shape[0] and x < canvas_shape[1]:
                     canvas_hdu.data[y, x] += frac * flux[ii].value
@@ -493,16 +490,16 @@
 
         for ii in range(max(1, len(wcs_suffix))):
             si = wcs_suffix[ii] if len(wcs_suffix) > 0 else ""
             imagehdu.header["CRPIX1"+si] *= zoom1
             imagehdu.header["CRPIX2"+si] *= zoom2
             imagehdu.header["CDELT1"+si] = pixel_scale
             imagehdu.header["CDELT2"+si] = pixel_scale
-            imagehdu.header["CUNIT1"+si] = "mm" if si == 'D' else "deg"
-            imagehdu.header["CUNIT2"+si] = "mm" if si == 'D' else "deg"
+            imagehdu.header["CUNIT1"+si] = "mm" if si == "D" else "deg"
+            imagehdu.header["CUNIT2"+si] = "mm" if si == "D" else "deg"
 
     return imagehdu
 
 
 def reorient_imagehdu(imagehdu, wcs_suffix="", conserve_flux=True,
                       spline_order=1):
     """
@@ -552,18 +549,18 @@
         imagehdu.data = new_im
         hdr["CRPIX1"+s] = hdr["NAXIS1"] / 2.
         hdr["CRPIX2"+s] = hdr["NAXIS2"] / 2.
         for card in ["PC1_1"+s, "PC1_2"+s, "PC2_1"+s, "PC2_2"+s]:
             hdr.remove(card)
         imagehdu.header = hdr
 
-    elif any(["PC1_1" in key for key in imagehdu.header]):
-        logging.warning("PC Keywords were found, but not used due to different "
-                      "wcs_suffix given: {} \n {}"
-                      "".format(wcs_suffix, dict(imagehdu.header)))
+    elif any("PC1_1" in key for key in imagehdu.header):
+        logging.warning(("PC Keywords were found, but not used due to different "
+                         "wcs_suffix given: %s \n %s"),
+                        wcs_suffix, dict(imagehdu.header))
 
     return imagehdu
 
 
 def affine_map(input, matrix=None, rotation_angle=0, shear_angle=0,
                scale_factor=None, reshape=True, spline_order=3):
     """
@@ -846,10 +843,10 @@
             x1_sky = x0_sky + (x1_pix - x0_pix) * x_delt
             y1_sky = y0_sky + (y1_pix - y0_pix) * y_delt
             x2_sky = x1_sky + x_delt * min(chunk_size, naxis1 - x1_pix)
             y2_sky = y1_sky + y_delt * min(chunk_size, naxis2 - y1_pix)
 
             hdr_sky = header_from_list_of_xy([x1_sky, x2_sky], [y1_sky, y2_sky],
                                              pixel_scale=x_delt, wcs_suffix=s)
-            hdr_list += [hdr_sky]
+            hdr_list.append(hdr_sky)
 
     return hdr_list
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/monochromatic_trace_curve.py` & `ScopeSim-0.6.0/scopesim/optics/monochromatic_trace_curve.py`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/optics/optical_element.py` & `ScopeSim-0.6.0/scopesim/optics/optical_element.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 from inspect import isclass
+from typing import TextIO
+from io import StringIO
 
 from astropy.table import Table
 
 from .. import effects as efs
 from ..effects.effects_utils import make_effect, get_all_effects
 from ..utils import write_report
 from ..reports.rst_utils import table_to_rst
@@ -60,34 +62,33 @@
         self.meta = {"name": "<empty>"}
         self.meta.update(kwargs)
         self.properties = {}
         self.effects = []
 
         if isinstance(yaml_dict, dict):
             self.meta.update({key: yaml_dict[key] for key in yaml_dict
-                              if key not in ["properties", "effects"]})
+                              if key not in {"properties", "effects"}})
             if "properties" in yaml_dict:
                 self.properties = yaml_dict["properties"]
             if "name" in yaml_dict:
                 self.properties["element_name"] = yaml_dict["name"]
             if "effects" in yaml_dict and len(yaml_dict["effects"]) > 0:
                 for eff_dic in yaml_dict["effects"]:
                     if "name" in eff_dic and hasattr(rc.__currsys__,
                                                      "ignore_effects"):
                         if eff_dic["name"] in rc.__currsys__.ignore_effects:
                             eff_dic["include"] = False
 
-                    self.effects += [make_effect(eff_dic, **self.properties)]
+                    self.effects.append(make_effect(eff_dic, **self.properties))
 
     def add_effect(self, effect):
         if isinstance(effect, efs.Effect):
-            self.effects += [effect]
+            self.effects.append(effect)
         else:
-            logging.warning("{} is not an Effect object and was not added"
-                          "".format(effect))
+            logging.warning("%s is not an Effect object and was not added", effect)
 
     def get_all(self, effect_class):
         return get_all_effects(self.effects, effect_class)
 
     def get_z_order_effects(self, z_level):
         if isinstance(z_level, int):
             zmin = z_level
@@ -98,19 +99,19 @@
             zmin, zmax = 0, 999
 
         effects = []
         for eff in self.effects:
             if eff.include and "z_order" in eff.meta:
                 z = eff.meta["z_order"]
                 if isinstance(z, (list, tuple)):
-                    if any([zmin <= zi <= zmax for zi in z]):
-                        effects += [eff]
+                    if any(zmin <= zi <= zmax for zi in z):
+                        effects.append(eff)
                 else:
                     if zmin <= z <= zmax:
-                        effects += [eff]
+                        effects.append(eff)
 
         return effects
 
     @property
     def surfaces_list(self):
         _ter_list = [effect for effect in self.effects
                      if isinstance(effect, (efs.SurfaceList, efs.FilterWheel,
@@ -171,93 +172,98 @@
         """
         obj = None
         if isclass(item):
             obj = self.get_all(item)
         elif isinstance(item, int):
             obj = self.effects[item]
         elif isinstance(item, str):
-            if item[0] == "#" and "." in item:
+            if item.startswith("#") and "." in item:
                 eff, meta = item.replace("#", "").split(".")
                 obj = self[eff][f"#{meta}"]
             else:
                 obj = [eff for eff in self.effects
                        if eff.meta["name"] == item]
 
         if isinstance(obj, list) and len(obj) == 1:
             obj = obj[0]
         # if obj is None or len(obj) == 0:
         #     logging.warning(f'No result for key: "{item}". '
         #                     f'Did you mean "#{item}"?')
 
         return obj
 
+    def write_string(self, stream: TextIO, list_effects: bool = True) -> None:
+        """Write formatted string representation to I/O stream"""
+        stream.write(f"{self!s} contains {len(self.effects)} Effects\n")
+        if list_effects:
+            for i_eff, eff in enumerate(self.effects):
+                stream.write(f"[{i_eff}] {eff!r}\n")
+
+    def pretty_str(self) -> str:
+        """Return formatted string representation as str"""
+        with StringIO() as str_stream:
+            self.write_string(str_stream)
+            output = str_stream.getvalue()
+        return output
+
+    @property
+    def display_name(self):
+        return self.meta.get("name", self.meta.get("filename", "<empty>"))
+
     def __repr__(self):
-        msg = '\nOpticalElement : "{}" contains {} Effects: \n' \
-              ''.format(self.meta["name"], len(self.effects))
-        eff_str = "\n".join(["[{}] {}".format(i, eff.__repr__())
-                             for i, eff in enumerate(self.effects)])
-        return msg + eff_str
+        return f"<{self.__class__.__name__}>"
 
     def __str__(self):
-        name = self.meta.get("name", self.meta.get("filename", "<empty>"))
-        return '{}: "{}"'.format(type(self).__name__, name)
+        return f"{self.__class__.__name__}: \"{self.display_name}\""
 
     @property
     def properties_str(self):
         prop_str = ""
-        max_key_len = max([len(key) for key in self.properties.keys()])
+        max_key_len = max(len(key) for key in self.properties.keys())
+        padlen = max_key_len + 4
         for key in self.properties:
-            if key not in ["comments", "changes", "description", "history",
-                           "report"]:
-                prop_str += "    {} : {}\n".format(key.rjust(max_key_len),
-                                                   self.properties[key])
+            if key not in {"comments", "changes", "description", "history",
+                           "report"}:
+                prop_str += f"{key:>{padlen}} : {self.properties[key]}\n"
 
         return prop_str
 
     def report(self, filename=None, output="rst", rst_title_chars="^#*+",
                **kwargs):
 
-        rst_str = """
-{}
-{}
+        rst_str = f"""
+{str(self)}
+{rst_title_chars[0] * len(str(self))}
 
-**Element**: {}
+**Element**: {self.meta.get("object", "<unknown optical element>")}
 
-**Alias**: {}
+**Alias**: {self.meta.get("alias", "<unknown alias>")}
         
-**Description**: {}
+**Description**: {self.meta.get("description", "<no description>")}
 
 Global properties
-{}
+{rst_title_chars[1] * 17}
 ::
 
-{}
-""".format(str(self),
-           rst_title_chars[0] * len(str(self)),
-           self.meta.get("object", "<unknown optical element>"),
-           self.meta.get("alias", "<unknown alias>"),
-           self.meta.get("description", "<no description>"),
-           rst_title_chars[1] * 17,
-           self.properties_str)
+{self.properties_str}
+"""
 
         if len(self.list_effects()) > 0:
-            rst_str += """        
+            rst_str += f"""
 Effects
-{}
+{rst_title_chars[1] * 7}
 
 Summary of Effects included in this optical element:
 
 .. table::
-    :name: {}
+    :name: {"tbl:" + self.meta.get("name", "<unknown OpticalElement>")}
    
-{}
+{table_to_rst(self.list_effects(), indent=4)}
  
-""".format(rst_title_chars[1] * 7,
-           "tbl:" + self.meta.get("name", "<unknown OpticalElement>"),
-           table_to_rst(self.list_effects(), indent=4))
+"""
 
         reports = [eff.report(rst_title_chars=rst_title_chars[-2:], **kwargs)
                    for eff in self.effects]
         rst_str += "\n\n" + "\n\n".join(reports)
 
         write_report(rst_str, filename, output)
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/optical_train.py` & `ScopeSim-0.6.0/scopesim/optics/optical_train.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
-import os
 import sys
 from copy import deepcopy
 from shutil import copyfileobj
+from pathlib import Path
 
 from datetime import datetime
 
 import numpy as np
 from scipy.interpolate import interp1d
 from astropy.io import fits
 from astropy.wcs import WCS
@@ -79,17 +79,16 @@
     or by passing a dictionary (with one or multiple entries) to the
     OpticalTrain object::
 
         >>> opt["dark_current"] = {"value": 0.75, "dit": 30}
 
     """
     def __init__(self, cmds=None):
-
-        self._description = self.__repr__()
         self.cmds = cmds
+        self._description = self.__repr__()
         self.optics_manager = None
         self.fov_manager = None
         self.image_planes = []
         self.detector_arrays = []
         self.yaml_dicts = None
         self._last_source = None
 
@@ -107,16 +106,16 @@
         """
 
         if isinstance(user_commands, str):
             user_commands = UserCommands(use_instrument=user_commands)
         elif isinstance(user_commands, UserCommands):
             user_commands = copy.deepcopy(user_commands)
         else:
-            raise ValueError("user_commands must be a UserCommands or str object: "
-                             "{}".format(type(user_commands)))
+            raise ValueError("user_commands must be a UserCommands or str object "
+                             f"but is {type(user_commands)}")
 
         self.cmds = user_commands
         rc.__currsys__ = user_commands
         self.yaml_dicts = rc.__currsys__.yaml_dicts
         self.optics_manager = OpticsManager(self.yaml_dicts)
         self.update()
 
@@ -195,16 +194,16 @@
 
             fov.flatten()
             self.image_planes[fov.image_plane_id].add(fov.hdu, wcs_suffix="D")
             # ..todo: finish off the multiple image plane stuff
 
         # [2D - Vibration, flat fielding, chopping+nodding]
         for effect in self.optics_manager.image_plane_effects:
-            for ii in range(len(self.image_planes)):
-                self.image_planes[ii] = effect.apply_to(self.image_planes[ii])
+            for ii, image_plane in enumerate(self.image_planes):
+                self.image_planes[ii] = effect.apply_to(image_plane)
 
         self._last_fovs = fovs
         self._last_source = source
 
 
     def prepare_source(self, source):
         """
@@ -223,46 +222,46 @@
         # Convert to PHOTLAM per arcsec2
         # ..todo: this is not sufficiently general
 
         for cube in source.cube_fields:
             header, data, wave = cube.header, cube.data, cube.wave
 
             # Need to check whether BUNIT is per arcsec2 or per pixel
-            inunit = u.Unit(header['BUNIT'])
+            inunit = u.Unit(header["BUNIT"])
             data = data.astype(np.float32) * inunit
             factor = 1
             for base, power in zip(inunit.bases, inunit.powers):
                 if (base**power).is_equivalent(u.arcsec**(-2)):
                     conversion =(base**power).to(u.arcsec**(-2)) / base**power
                     data *= conversion
                     factor = u.arcsec**(-2)
 
             data = data.to(PHOTLAM,
                            equivalencies=u.spectral_density(wave[:, None, None]))
 
             if factor == 1:    # Normalise to 1 arcsec2 if not a spatial density
                 # ..todo: lower needed because "DEG" is not understood, this is ugly
-                pixarea = (header['CDELT1'] * u.Unit(header['CUNIT1'].lower()) *
-                           header['CDELT2'] * u.Unit(header['CUNIT2'].lower())).to(u.arcsec**2)
+                pixarea = (header["CDELT1"] * u.Unit(header["CUNIT1"].lower()) *
+                           header["CDELT2"] * u.Unit(header["CUNIT2"].lower())).to(u.arcsec**2)
                 data = data / pixarea.value    # cube is per arcsec2
 
             data = (data * factor).value
 
-            cube.header['BUNIT'] = 'PHOTLAM/arcsec2'    # ..todo: make this more explicit?
+            cube.header["BUNIT"] = "PHOTLAM/arcsec2"    # ..todo: make this more explicit?
 
             # The imageplane_utils like to have the spatial WCS in units of "deg". Ensure
             # that the cube is passed on accordingly
-            cube.header['CDELT1'] = header['CDELT1'] * u.Unit(header['CUNIT1'].lower()).to(u.deg)
-            cube.header['CDELT2'] = header['CDELT2'] * u.Unit(header['CUNIT2'].lower()).to(u.deg)
-            cube.header['CUNIT1'] = 'deg'
-            cube.header['CUNIT2'] = 'deg'
+            cube.header["CDELT1"] = header["CDELT1"] * u.Unit(header["CUNIT1"].lower()).to(u.deg)
+            cube.header["CDELT2"] = header["CDELT2"] * u.Unit(header["CUNIT2"].lower()).to(u.deg)
+            cube.header["CUNIT1"] = "deg"
+            cube.header["CUNIT2"] = "deg"
 
             # Put on fov wavegrid
-            wave_min = min([fov.meta["wave_min"] for fov in self.fov_manager.fovs])
-            wave_max = max([fov.meta["wave_max"] for fov in self.fov_manager.fovs])
+            wave_min = min(fov.meta["wave_min"] for fov in self.fov_manager.fovs)
+            wave_max = max(fov.meta["wave_max"] for fov in self.fov_manager.fovs)
             wave_unit = u.Unit(from_currsys("!SIM.spectral.wave_unit"))
             dwave = from_currsys("!SIM.spectral.spectral_bin_width")  # Not a quantity
             fov_waveset = np.arange(wave_min.value, wave_max.value, dwave) * wave_unit
             fov_waveset = fov_waveset.to(u.um)
 
             # Interpolate into new data cube.
             # This is done layer by layer for memory reasons.
@@ -271,19 +270,19 @@
             for j in range(data.shape[1]):
                 cube_interp = interp1d(wave.to(u.um).value, data[:, j, :],
                                        axis=0, kind="linear",
                                        bounds_error=False, fill_value=0)
                 new_data[:, j, :] = cube_interp(fov_waveset.value)
 
             cube.data = new_data
-            cube.header['CTYPE3'] = 'WAVE'
-            cube.header['CRPIX3'] = 1
-            cube.header['CRVAL3'] = wave_min.value
-            cube.header['CDELT3'] = dwave
-            cube.header['CUNIT3'] = wave_unit.name
+            cube.header["CTYPE3"] = "WAVE"
+            cube.header["CRPIX3"] = 1
+            cube.header["CRVAL3"] = wave_min.value
+            cube.header["CDELT3"] = dwave
+            cube.header["CUNIT3"] = wave_unit.name
 
         return source
 
     def readout(self, filename=None, **kwargs):
         """
         Produces detector readouts for the observed image
 
@@ -315,157 +314,156 @@
                 for effect in fits_effects:
                     hdul = effect.apply_to(hdul, optical_train=self)
             else:
                 try:
                     hdul = self.write_header(hdul)
                 except Exception as error:
                     print("\nWarning: header update failed, data will be saved with incomplete header.")
-                    print("Reason: ", sys.exc_info()[0], error)
-                    print("")
+                    print(f"Reason: {sys.exc_info()[0]} {error}\n")
 
             if filename is not None and isinstance(filename, str):
                 fname = filename
                 if len(self.detector_arrays) > 1:
-                    fname = str(i) + "_" + filename
+                    fname = f"{i}_{filename}"
                 hdul.writeto(fname, overwrite=True)
 
-            hduls += [hdul]
+            hduls.append(hdul)
 
         return hduls
 
     def write_header(self, hdulist):
         """Writes meaningful header to simulation product"""
 
         # Primary hdu
         pheader = hdulist[0].header
-        pheader['DATE'] = datetime.now().isoformat(timespec='seconds')
-        pheader['ORIGIN'] = 'Scopesim ' + version
-        pheader['INSTRUME'] = from_currsys("!OBS.instrument")
-        pheader['INSTMODE'] = ", ".join(from_currsys("!OBS.modes"))
-        pheader['TELESCOP'] = from_currsys("!TEL.telescope")
-        pheader['LOCATION'] = from_currsys("!ATMO.location")
+        pheader["DATE"] = datetime.now().isoformat(timespec="seconds")
+        pheader["ORIGIN"] = "Scopesim " + version
+        pheader["INSTRUME"] = from_currsys("!OBS.instrument")
+        pheader["INSTMODE"] = ", ".join(from_currsys("!OBS.modes"))
+        pheader["TELESCOP"] = from_currsys("!TEL.telescope")
+        pheader["LOCATION"] = from_currsys("!ATMO.location")
 
         # Source information taken from first only.
         # ..todo: What if source is a composite?
         srcfield = self._last_source.fields[0]
         if type(srcfield).__name__ == "Table":
-            pheader['SOURCE'] = "Table"
+            pheader["SOURCE"] = "Table"
         elif type(srcfield).__name__ == "ImageHDU":
-            if 'BG_SURF' in srcfield.header:
-                pheader['SOURCE'] = srcfield.header['BG_SURF']
+            if "BG_SURF" in srcfield.header:
+                pheader["SOURCE"] = srcfield.header["BG_SURF"]
             else:
                 try:
-                    pheader['SOURCE'] = srcfield.header['FILENAME']
+                    pheader["SOURCE"] = srcfield.header["FILENAME"]
                 except KeyError:
-                    pheader['SOURCE'] = "ImageHDU"
+                    pheader["SOURCE"] = "ImageHDU"
 
         # Image hdul
         # ..todo: currently only one, update for detector arrays
-        # ..todo: normalise filenames - some need from_currsys, some need os.path.basename
+        # ..todo: normalise filenames - some need from_currsys, some need Path(...).name
         #         this should go into a function so as to reduce clutter here.
         iheader = hdulist[1].header
-        iheader['EXPTIME'] = from_currsys("!OBS.exptime"), "[s]"
-        iheader['DIT'] = from_currsys("!OBS.dit"), "[s]"
-        iheader['NDIT'] = from_currsys("!OBS.ndit")
-        iheader['BUNIT'] = 'e', 'per EXPTIME'
-        iheader['PIXSCALE'] = from_currsys("!INST.pixel_scale"), "[arcsec]"
+        iheader["EXPTIME"] = from_currsys("!OBS.exptime"), "[s]"
+        iheader["DIT"] = from_currsys("!OBS.dit"), "[s]"
+        iheader["NDIT"] = from_currsys("!OBS.ndit")
+        iheader["BUNIT"] = "e", "per EXPTIME"
+        iheader["PIXSCALE"] = from_currsys("!INST.pixel_scale"), "[arcsec]"
 
         # A simple WCS
-        iheader['CTYPE1'] = 'LINEAR'
-        iheader['CTYPE2'] = 'LINEAR'
-        iheader['CRPIX1'] = (iheader['NAXIS1'] + 1) / 2
-        iheader['CRPIX2'] = (iheader['NAXIS2'] + 1) / 2
-        iheader['CRVAL1'] = 0.
-        iheader['CRVAL2'] = 0.
-        iheader['CDELT1'] = iheader['PIXSCALE']
-        iheader['CDELT2'] = iheader['PIXSCALE']
-        iheader['CUNIT1'] = 'arcsec'
-        iheader['CUNIT2'] = 'arcsec'
+        iheader["CTYPE1"] = "LINEAR"
+        iheader["CTYPE2"] = "LINEAR"
+        iheader["CRPIX1"] = (iheader["NAXIS1"] + 1) / 2
+        iheader["CRPIX2"] = (iheader["NAXIS2"] + 1) / 2
+        iheader["CRVAL1"] = 0.
+        iheader["CRVAL2"] = 0.
+        iheader["CDELT1"] = iheader["PIXSCALE"]
+        iheader["CDELT2"] = iheader["PIXSCALE"]
+        iheader["CUNIT1"] = "arcsec"
+        iheader["CUNIT2"] = "arcsec"
 
         for eff in self.optics_manager.detector_setup_effects:
             efftype = type(eff).__name__
 
             if efftype == "DetectorList" and eff.include:
-                iheader['DETECTOR'] = eff.meta['detector']
+                iheader["DETECTOR"] = eff.meta["detector"]
 
         for eff in self.optics_manager.detector_array_effects:
             efftype = type(eff).__name__
 
             if (efftype == "DetectorModePropertiesSetter" and
                 eff.include):
                 # ..todo: can we write this into currsys?
-                iheader['DET_MODE'] = (eff.meta['detector_readout_mode'],
+                iheader["DET_MODE"] = (eff.meta["detector_readout_mode"],
                                        "detector readout mode")
-                iheader['MINDIT'] = from_currsys("!DET.mindit"), "[s]"
-                iheader['FULLWELL'] = from_currsys("!DET.full_well"), "[s]"
-                iheader['RON'] = from_currsys("!DET.readout_noise"), "[e]"
-                iheader['DARK'] = from_currsys("!DET.dark_current"), "[e/s]"
+                iheader["MINDIT"] = from_currsys("!DET.mindit"), "[s]"
+                iheader["FULLWELL"] = from_currsys("!DET.full_well"), "[s]"
+                iheader["RON"] = from_currsys("!DET.readout_noise"), "[e]"
+                iheader["DARK"] = from_currsys("!DET.dark_current"), "[e/s]"
 
         ifilter = 1   # Counts filter wheels
         isurface = 1  # Counts surface lists
         for eff in self.optics_manager.source_effects:
             efftype = type(eff).__name__
 
             if efftype == "ADCWheel" and eff.include:
-                iheader['ADC'] = eff.current_adc.meta['name']
+                iheader["ADC"] = eff.current_adc.meta["name"]
 
             if efftype == "FilterWheel" and eff.include:
-                iheader[f'FILTER{ifilter}'] = (eff.current_filter.meta['name'],
-                                               eff.meta['name'])
+                iheader[f"FILTER{ifilter}"] = (eff.current_filter.meta["name"],
+                                               eff.meta["name"])
                 ifilter += 1
 
             if efftype == "SlitWheel" and eff.include:
-                iheader['SLIT'] = (eff.current_slit.meta['name'],
-                                   eff.meta['name'])
+                iheader["SLIT"] = (eff.current_slit.meta["name"],
+                                   eff.meta["name"])
 
             if efftype == "PupilTransmission" and eff.include:
-                iheader['PUPTRANS'] = (from_currsys("!OBS.pupil_transmission"),
+                iheader["PUPTRANS"] = (from_currsys("!OBS.pupil_transmission"),
                                        "cold stop, pupil transmission")
 
             if efftype == "SkycalcTERCurve" and eff.include:
-                iheader['ATMOSPHE'] = "Skycalc", "atmosphere model"
-                iheader['LOCATION'] = eff.meta['location']
-                iheader['AIRMASS'] = eff.meta['airmass']
-                iheader['TEMPERAT'] = eff.meta['temperature'], '[degC]'
-                iheader['HUMIDITY'] = eff.meta['humidity']
-                iheader['PRESSURE'] = eff.meta['pressure'], '[hPa]'
-                iheader['PWV'] = eff.meta['pwv'], "precipitable water vapour"
+                iheader["ATMOSPHE"] = "Skycalc", "atmosphere model"
+                iheader["LOCATION"] = eff.meta["location"]
+                iheader["AIRMASS"] = eff.meta["airmass"]
+                iheader["TEMPERAT"] = eff.meta["temperature"], "[degC]"
+                iheader["HUMIDITY"] = eff.meta["humidity"]
+                iheader["PRESSURE"] = eff.meta["pressure"], "[hPa]"
+                iheader["PWV"] = eff.meta["pwv"], "precipitable water vapour"
 
             if efftype == "AtmosphericTERCurve" and eff.include:
-                iheader['ATMOSPHE'] = eff.meta['filename'], "atmosphere model"
+                iheader["ATMOSPHE"] = eff.meta["filename"], "atmosphere model"
                 # ..todo: expand if necessary
 
             if efftype == "SurfaceList" and eff.include:
-                iheader[f'SURFACE{isurface}'] = (eff.meta['filename'],
-                                                 eff.meta['name'])
+                iheader[f"SURFACE{isurface}"] = (eff.meta["filename"],
+                                                 eff.meta["name"])
                 isurface += 1
 
             if efftype == "QuantumEfficiencyCurve" and eff.include:
-                iheader['QE'] = os.path.basename(eff.meta['filename']), eff.meta['name']
+                iheader["QE"] = Path(eff.meta["filename"]).name, eff.meta["name"]
 
         for eff in self.optics_manager.fov_effects:
             efftype = type(eff).__name__
 
             # ..todo: needs to be handled with isinstance(eff, PSF)
             if efftype == "FieldConstantPSF" and eff.include:
-                iheader["PSF"] = eff.meta['filename'], "point spread function"
+                iheader["PSF"] = eff.meta["filename"], "point spread function"
 
             if efftype == "SpectralTraceList" and eff.include:
-                iheader["SPECTRAC"] = (from_currsys(eff.meta['filename']),
+                iheader["SPECTRAC"] = (from_currsys(eff.meta["filename"]),
                                        "spectral trace definition")
                 if "CTYPE1" in eff.meta:
-                    for key in ['WCSAXES', 'CTYPE1', 'CTYPE2', 'CRPIX1', 'CRPIX2', 'CRVAL1',
-                                'CRVAL2', 'CDELT1', 'CDELT2', 'CUNIT1', 'CUNIT2']:
+                    for key in {"WCSAXES", "CTYPE1", "CTYPE2", "CRPIX1", "CRPIX2", "CRVAL1",
+                                "CRVAL2", "CDELT1", "CDELT2", "CUNIT1", "CUNIT2"}:
                         iheader[key] = eff.meta[key]
 
         for eff in self.optics_manager.detector_effects:
             efftype = type(eff).__name__
 
             if efftype == "LinearityCurve" and eff.include:
-                iheader['DETLIN'] = from_currsys(eff.meta['filename'])
+                iheader["DETLIN"] = from_currsys(eff.meta["filename"])
 
         return hdulist
 
     def set_focus(self, **kwargs):
         self.cmds.update(**kwargs)
         dy = self.cmds.default_yamls
         if len(dy) > 0 and "packages" in dy:
@@ -476,27 +474,30 @@
     def shutdown(self):
         """
         Shut down the instrument.
 
         This method closes all open file handles and should be called when the optical train
         is no longer needed.
         """
-        for effect_name in self.effects['name']:
+        for effect_name in self.effects["name"]:
             try:
                 self[effect_name]._file.close()
             except AttributeError:
                 pass
 
         self._description = "The instrument has been shut down."
 
 
     @property
     def effects(self):
         return self.optics_manager.list_effects()
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}({self.cmds!r})"
+
     def __str__(self):
         return self._description
 
     def __getitem__(self, item):
         return self.optics_manager[item]
 
     def __setitem__(self, key, value):
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/optics_manager.py` & `ScopeSim-0.6.0/scopesim/optics/optics_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import logging
 from inspect import isclass
+from typing import TextIO
+from io import StringIO
+from collections.abc import Sequence
 
 import numpy as np
 from astropy import units as u
 from astropy.table import Table
 from synphot import SpectralElement, Empirical1D
 
 from .optical_element import OpticalElement
@@ -26,30 +29,30 @@
         which include ``effects`` and ``properties`` sub-dictionaries
 
     kwargs : expanded dict
         Any extra information not directly related to the optical elements
 
     """
 
-    def __init__(self, yaml_dicts=[], **kwargs):
+    def __init__(self, yaml_dicts=None, **kwargs):
         self.optical_elements = []
         self.meta = {}
         self.meta.update(kwargs)
         self._surfaces_table = None
         self._surface_like_effects = None
 
         if yaml_dicts is not None:
             self.load_effects(yaml_dicts, **self.meta)
 
         self.set_derived_parameters()
 
     def set_derived_parameters(self):
 
         if "!INST.pixel_scale" not in rc.__currsys__:
-            raise ValueError("!INST.pixel_scale is missing from the current"
+            raise ValueError("'!INST.pixel_scale' is missing from the current"
                              "system. Please add this to the instrument (INST)"
                              "properties dict for the system.")
         pixel_scale = rc.__currsys__["!INST.pixel_scale"] * u.arcsec
         area = self.area
         etendue = area * pixel_scale**2
         rc.__currsys__["!TEL.etendue"] = etendue
         rc.__currsys__["!TEL.area"] = area
@@ -78,18 +81,18 @@
         ----------
         yaml_dicts : list of dicts
             Each YAML dict should contain the descriptions of the Effects needed
             by each ``OpticalElement``
 
         """
 
-        if isinstance(yaml_dicts, dict):
+        if not isinstance(yaml_dicts, Sequence):
             yaml_dicts = [yaml_dicts]
-        self.optical_elements += [OpticalElement(dic, **kwargs)
-                                  for dic in yaml_dicts if "effects" in dic]
+        self.optical_elements.extend(OpticalElement(dic, **kwargs)
+                                     for dic in yaml_dicts if "effects" in dic)
 
     def add_effect(self, effect, ext=0):
         """
         Add an Effect object to an OpticalElement at index ``ext``
 
         Parameters
         ----------
@@ -172,17 +175,16 @@
         return is_spectroscope(self.all_effects)
 
     @property
     def image_plane_headers(self):
         detector_lists = self.detector_setup_effects
         headers = [det_list.image_plane_header for det_list in detector_lists]
 
-        if len(detector_lists) == 0:
-            raise ValueError("No DetectorList objects found. {}"
-                             "".format(detector_lists))
+        if not detector_lists:
+            raise ValueError(f"No DetectorList objects found. {detector_lists}")
 
         return headers
 
     @property
     def detector_array_effects(self):
         return self.get_z_order_effects(900)
 
@@ -279,28 +281,26 @@
         tbl = Table(names=colnames, data=data, copy=False)
 
         return tbl
 
     def report(self, filename=None, output="rst", rst_title_chars="_^#*+",
                **kwargs):
 
-        rst_str = """
+        rst_str = f"""
 List of Optical Elements
-{}
+{rst_title_chars[0] * 24}
 
 Summary of Effects in Optical Elements:
-{}
+{rst_title_chars[1] * 39}
 
 .. table::
     :name: tbl:effects_summary
 
-{}
-""".format(rst_title_chars[0] * 24,
-           rst_title_chars[1] * 39,
-           table_to_rst(self.list_effects(), indent=4))
+{table_to_rst(self.list_effects(), indent=4)}
+"""
 
         reports = [opt_el.report(rst_title_chars=rst_title_chars[-4:], **kwargs)
                    for opt_el in self.optical_elements]
         rst_str += "\n\n" + "\n\n".join(reports)
 
         write_report(rst_str, filename, output)
 
@@ -313,15 +313,15 @@
         obj = []
         if isclass(item):
             obj += [opt_el.get_all(item) for opt_el in self.optical_elements]
         elif isinstance(item, int):
             obj = self.optical_elements[item]
         elif isinstance(item, str):
             # check for hash-string for getting Effect.meta values
-            if item[0] == "#" and "." in item:
+            if item.startswith("#") and "." in item:
                 opt_el_name = item.replace("#", "").split(".")[0]
                 new_item = item.replace(f"{opt_el_name}.", "")
                 obj = self[opt_el_name][new_item]
             else:
                 # get all optical elements that match "item"
                 obj = [opt_el for opt_el in self.optical_elements
                        if opt_el.meta["name"] == item]
@@ -339,24 +339,34 @@
             raise ValueError(f"Cannot find object: {item}")
 
         return obj
 
     def __setitem__(self, key, value):
         obj = self.__getitem__(key)
         if isinstance(obj, list) and len(obj) > 1:
-            logging.warning("{} does not return a singular object:\n {}"
-                          "".format(key, obj))
+            logging.warning("%s does not return a singular object:\n %s", key, obj)
         elif isinstance(obj, efs.Effect) and isinstance(value, dict):
             obj.meta.update(value)
 
-    def __repr__(self):
-        msg = f"\nOpticsManager contains {len(self.optical_elements)} " \
-              f"OpticalElements \n"
-        for ii, opt_el in enumerate(self.optical_elements):
-            msg += f'[{ii}] "{opt_el.meta["name"]}" contains ' \
-                   f'{len(opt_el.effects)} effects \n'
+    def write_string(self, stream: TextIO) -> None:
+        """Write formatted string representation to I/O stream"""
+        stream.write(f"{self!s} contains {len(self.optical_elements)} "
+                     "OpticalElements\n")
+        for opt_elem in enumerate(self.optical_elements):
+            opt_elem.write_string(stream, list_effects=False)
+
+    def pretty_str(self) -> str:
+        """Return formatted string representation as str"""
+        with StringIO() as str_stream:
+            self.write_string(str_stream)
+            output = str_stream.getvalue()
+        return output
+
+    @property
+    def display_name(self):
+        return self.meta.get("name", self.meta.get("filename", "<empty>"))
 
-        return msg
+    def __repr__(self):
+        return f"<{self.__class__.__name__}>"
 
     def __str__(self):
-        name = self.meta.get("name", self.meta.get("filename", "<empty>"))
-        return f'{type(self).__name__}: "{name}"'
+        return f"{self.__class__.__name__}: \"{self.display_name}\""
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/radiometry.py` & `ScopeSim-0.6.0/scopesim/optics/radiometry.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,26 +71,24 @@
 
         return combine_emissions(self.table, self.surfaces, rows, etendue,
                                  use_area)
 
     @property
     def emission(self):
         if "etendue" not in self.meta:
-            raise ValueError("self.meta['etendue'] must be set")
+            raise ValueError("self.meta[\"etendue\"] must be set")
         etendue = quantify(self.meta["etendue"], "m2 arcsec2")
 
         return self.get_emission(etendue)
 
     @property
     def throughput(self):
         return self.get_throughput()
 
     def plot(self, what="all", rows=None):
-        raise NotImplemented
+        raise NotImplementedError()
 
     def __getitem__(self, item):
         return self.surfaces[item]
 
     def __repr__(self):
-        return self.table.__repr__()
-
-
+        return f"{self.__class__.__name__}({self.table!r}, **{self.meta})"
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/radiometry_utils.py` & `ScopeSim-0.6.0/scopesim/optics/radiometry_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from collections import OrderedDict
 from copy import deepcopy
 import logging
 
-import numpy as np
 from astropy import units as u
 from astropy.io import ascii as ioascii
 from astropy.table import Table, vstack
 
 from .surface import SpectralSurface
-from ..utils import real_colname, insert_into_ordereddict, quantify, \
+from ..utils import real_colname, insert_into_ordereddict, \
     change_table_entry, convert_table_comments_to_dict, from_currsys
 
 
 def combine_emissions(tbl, surfaces, row_indexes, etendue, use_area=False):
     """
     Combine thermal emission from a series of surfaces
 
@@ -72,15 +71,15 @@
     throughput = None
     for ii, row_num in enumerate(rows_indexes):
 
         row = tbl[row_num]
         surf = surfaces[row[r_name]]
         action_attr = row[r_action]
         if action_attr == "":
-            raise ValueError("No action in surf.meta: {}".format(surf.meta))
+            raise ValueError(f"No action in surf.meta: {surf.meta}")
 
         if isinstance(surf, SpectralSurface):
             surf_throughput = getattr(surf, action_attr)
 
             if ii == 0:
                 throughput = deepcopy(surf_throughput)
             else:
@@ -133,16 +132,16 @@
             surf_val = surf.meta[surf_col]
             if isinstance(surf_val, u.Quantity):
                 surf_val = surf_val.value
             new_tbl = change_table_entry(new_tbl, colname, surf_val,
                                          position=position)
         else:
             if not silent:
-                logging.warning("{} was not found in the meta dictionary of {}. "
-                              "This could cause problems".format(colname, name))
+                logging.warning(("%s was not found in the meta dictionary of %s. "
+                                 "This could cause problems"), colname, name)
 
     colname = real_colname("name", new_tbl.colnames)
     new_tbl = change_table_entry(new_tbl, colname, name, position=position)
 
     return new_tbl
 
 
@@ -153,16 +152,16 @@
     return dic
 
 
 def make_surface_dict_from_table(tbl):
     surf_dict = OrderedDict({})
     if tbl is not None and len(tbl) > 0:
         names = tbl[real_colname("name", tbl.colnames)]
-        for ii in range(len(tbl)):
-            surf_dict[names[ii]] = make_surface_from_row(tbl[ii], **tbl.meta)
+        for ii, row in enumerate(tbl):
+            surf_dict[names[ii]] = make_surface_from_row(row, **tbl.meta)
 
     return surf_dict
 
 
 def make_surface_from_row(row, **kwargs):
     row_dict = {colname.lower(): row[colname] for colname in row.colnames}
     kwargs.update(row_dict)
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/surface.py` & `ScopeSim-0.6.0/scopesim/optics/surface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import os
 import logging
+from pathlib import Path
+from dataclasses import dataclass
+from typing import Any
 
 import numpy as np
 
 from astropy import units as u
 from astropy.io import ascii as ioascii
 from astropy.table import Table
 
@@ -13,20 +15,21 @@
 from ..effects import ter_curves_utils as ter_utils
 from ..utils import get_meta_quantity, quantify, extract_type_from_unit
 from ..utils import from_currsys, convert_table_comments_to_dict, find_file
 from .surface_utils import make_emission_from_emissivity,\
     make_emission_from_array
 
 
+@dataclass
 class PoorMansSurface:
-    """ Solely used by SurfaceList """
-    def __init__(self, emission, throughput, meta):
-        self.emission = emission
-        self.throughput = throughput
-        self.meta = meta
+    """Solely used by SurfaceList """
+    # FIXME: Use correct types instead of Any
+    emission: Any
+    throughput: Any
+    meta: Any
 
 
 class SpectralSurface:
     """
     Initialised by a file containing one or more of the following columns:
     transmission, emissivity, reflection. The column wavelength must be given.
     Alternatively kwargs for the above mentioned quantities can be passed as
@@ -40,15 +43,15 @@
         filename = find_file(filename)
         self.meta = {"filename"         : filename,
                      "temperature"      : -270*u.deg_C,  # deg C
                      "emission_unit"    : "",
                      "wavelength_unit"  : u.um}
 
         self.table = Table()
-        if filename is not None and os.path.exists(filename):
+        if filename is not None and Path(filename).exists():
             self.table = ioascii.read(filename)
             tbl_meta = convert_table_comments_to_dict(self.table)
             if isinstance(tbl_meta, dict):
                 self.meta.update(tbl_meta)
 
         self.meta.update(kwargs)
 
@@ -123,16 +126,15 @@
 
         has_solid_angle = extract_type_from_unit(flux.meta["solid_angle"],
                                                  "solid angle")[1] != u.Unit("")
         if flux is not None and has_solid_angle:
             conversion_factor = flux.meta["solid_angle"].to(u.arcsec ** -2)
             flux = flux * conversion_factor
             flux.meta["solid_angle"] = u.arcsec**-2
-            flux.meta["history"] += ["Converted to arcsec-2: {}"
-                                     "".format(conversion_factor)]
+            flux.meta["history"].append(f"Converted to arcsec-2: {conversion_factor}")
 
         if flux is not None and "rescale_emission" in self.meta:
             dic = from_currsys(self.meta["rescale_emission"])
             amplitude = dic["value"] * u.Unit(dic["unit"])
             filter_name = dic["filter_name"]
             if "filename_format" in dic:
                 filter_name = dic["filename_format"].format(filter_name)
@@ -191,16 +193,15 @@
         if value_arr is not None and wave is not None and fmt == "synphot":
             response_curve = SpectralElement(Empirical1D, points=wave,
                                              lookup_table=value_arr)
         elif fmt == "array":
             response_curve = value_arr
         else:
             response_curve = None
-            logging.warning("Both wavelength and {} must be set"
-                          "".format(ter_property))
+            logging.warning("Both wavelength and %s must be set", ter_property)
 
         return response_curve
 
     def _compliment_array(self, colname_a, colname_b):
         """
         Returns an complimentary array using: ``a + b + c = 1``
 
@@ -252,16 +253,16 @@
         """
 
         if colname in self.meta:
             val = self.meta[colname]
         elif colname in self.table.colnames:
             val = self.table[colname].data
         else:
-            logging.debug(f"{colname} not found in either '.meta' or '.table': "
-                          f"[{self.meta.get('name', self.meta['filename'])}]")
+            logging.debug("%s not found in either '.meta' or '.table': [%s]",
+                          colname, self.meta.get("name", self.meta["filename"]))
             return None
 
         col_units = colname+"_unit"
         if isinstance(val, u.Quantity):
             units = val.unit
         elif col_units in self.meta:
             units = u.Unit(self.meta[col_units])
@@ -271,19 +272,24 @@
         if isinstance(val, u.Quantity):
             val_out = val.to(units)
         elif isinstance(val, (list, tuple, np.ndarray)):
             val_out = val * units
         elif val is None:
             val_out = None
         else:
-            raise ValueError("{} must be of type: Quantity, array, list, tuple"
-                             "".format(colname))
+            raise ValueError(f"{colname} must be of type: Quantity, array, "
+                             f"list, tuple, but is {type(colname)}")
 
         return val_out
 
     def __repr__(self):
+        msg = (f"{self.__class__.__name__}({self.meta['filename']}, "
+               f"**{self.meta!r})")
+        return msg
+
+    def __str__(self):
         meta = self.meta
         name = meta["name"] if "name" in meta else meta["filename"]
         cols = "".join([col[0].upper() for col in self.table.colnames])
-        msg = '<SpectralSurface> [{}] "{}"'.format(cols, name)
+        msg = "SpectralSurface [{cols}] \"{name}\""
 
         return msg
```

### Comparing `ScopeSim-0.5.6/scopesim/optics/surface_utils.py` & `ScopeSim-0.6.0/scopesim/optics/surface_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,33 +62,33 @@
     """
 
     if not isinstance(flux, u.Quantity):
         if "emission_unit" in meta:
             flux = quantify(flux, meta["emission_unit"])
         else:
             logging.warning("emission_unit must be set in self.meta, "
-                          "or emission must be an astropy.Quantity")
+                            "or emission must be an astropy.Quantity")
             flux = None
 
     if isinstance(wave, u.Quantity) and isinstance(flux, u.Quantity):
         flux_unit, angle = extract_type_from_unit(flux.unit, "solid angle")
         flux = flux / angle
 
         if is_flux_binned(flux.unit):
             flux = normalise_binned_flux(flux, wave)
 
         orig_unit = flux.unit
         flux = SourceSpectrum(Empirical1D, points=wave,
                               lookup_table=flux)
         flux.meta["solid_angle"] = angle
-        flux.meta["history"] = ["Created from emission array with units {}"
-                                "".format(orig_unit)]
+        flux.meta["history"] = [("Created from emission array with units "
+                                 f"{orig_unit}")]
     else:
         logging.warning("wavelength and emission must be "
-                      "astropy.Quantity py_objects")
+                        "astropy.Quantity py_objects")
         flux = None
 
     return flux
 
 
 def normalise_binned_flux(flux, wave):
     """
@@ -130,14 +130,10 @@
 
     Returns
     -------
     flag : bool
 
     """
     unit = unit**1
-    flag = False
     # unit.physical_type is a string in astropy<=4.2 and a PhysicalType
     # class in astropy==4.3 and thus has to be cast to a string first.
-    if u.bin in unit._bases or "flux density" not in str(unit.physical_type):
-        flag = True
-
-    return flag
+    return (u.bin in unit._bases or "flux density" not in str(unit.physical_type))
```

### Comparing `ScopeSim-0.5.6/scopesim/reports/report_generator.py` & `ScopeSim-0.6.0/scopesim/reports/report_generator.py`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/reports/rst_utils.py` & `ScopeSim-0.6.0/scopesim/reports/rst_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os
+from pathlib import Path
 
 from astropy.table import TableFormatter
 from docutils.core import publish_doctree, publish_parts
 from docutils.nodes import comment, literal_block
 import yaml
 
 from .. import rc
@@ -165,16 +165,16 @@
         img_path = options.get("path", rc.__config__["!SIM.reports.image_path"])
         formats = options.get("format", ["png"])
         formats = [formats] if isinstance(formats, str) else formats
         for fmt in formats:
 
             fname = options.get("name", "untitled").split(".")[0]
             fname = ".".join([fname, fmt])
-            fname = os.path.join(img_path, fname)
-            context_code += '\nplt.savefig("{}")'.format(fname)
+            fname = Path(img_path, fname)
+            context_code += f"\nplt.savefig(\"{fname}\")"
 
     return context_code
 
 
 def plotify_rst_text(rst_text):
     """
     Generates and saves plots from code blocks in an RST string
@@ -298,25 +298,24 @@
     if filename is None:
         filename = rst_text.split(title_char)[0].strip().replace(" ", "_")
 
     text = "Title\n<<<<<\nSubtitle\n>>>>>>>>\n\n"
     parts = publish_parts(text + rst_text, writer_name="latex")
 
     if not float_figures:
-        parts["body"] = parts["body"].replace('begin{figure}',
-                                              'begin{figure}[H]')
+        parts["body"] = parts["body"].replace("begin{figure}",
+                                              "begin{figure}[H]")
 
     if use_code_box:
-        parts["body"] = parts["body"].replace('begin{alltt}',
-                                              'begin{alltt}\n\\begin{lstlisting}[frame=single]')
-        parts["body"] = parts["body"].replace('end{alltt}',
-                                              'end{lstlisting}\n\\end{alltt}')
+        parts["body"] = parts["body"].replace("begin{alltt}",
+                                              "begin{alltt}\n\\begin{lstlisting}[frame=single]")
+        parts["body"] = parts["body"].replace("end{alltt}",
+                                              "end{lstlisting}\n\\end{alltt}")
 
-    filename = filename.split(".")[0] + ".tex"
-    file_path = os.path.join(path, filename)
+    file_path = Path(path, filename).with_suffix(".tex")
     with open(file_path, "w") as f:
         f.write(parts["body"])
 
     tex_str = parts["body"]
 
     return tex_str
 
@@ -325,27 +324,26 @@
     """ The same as ``latexify_rst_text```, but the output is in RST format """
     if path is None:
         path = from_currsys(rc.__config__["!SIM.reports.rst_path"])
 
     if filename is None:
         filename = rst_text.split(title_char)[0].strip().replace(" ", "_")
 
-    filename = filename.split(".")[0] + ".rst"
-    file_path = os.path.join(path, filename)
+    file_path = Path(path, filename).with_suffix(".rst")
     with open(file_path, "w") as f:
         f.write(rst_text)
 
     return rst_text
 
 
 def table_to_rst(tbl, indent=0, rounding=None):
     if isinstance(rounding, int):
         for col in tbl.itercols():
-            if col.info.dtype.kind == 'f':
-                col.info.format = '.{}f'.format(rounding)
+            if col.info.dtype.kind == "f":
+                col.info.format = f".{rounding}f"
     
     tbl_fmtr = TableFormatter()
     lines, outs = tbl_fmtr._pformat_table(tbl, max_width=-1, max_lines=-1,
                                           show_unit=False)
     i = outs["n_header"] - 1
     lines[i] = lines[i].replace("-", "=")
     lines = [lines[i]] + lines + [lines[i]]
```

### Comparing `ScopeSim-0.5.6/scopesim/server/OLD_database.py` & `ScopeSim-0.6.0/scopesim/server/OLD_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from scopesim.server.database import get_server_elements
 from urllib3.exceptions import HTTPError
 
 from astropy.utils.data import download_file
 
 from scopesim import rc
 
+from warnings import warn
 
 def get_local_packages(path):
     """
     List the packages that are available in the directory ``path``
 
     Parameters
     ----------
@@ -25,14 +26,16 @@
 
     Returns
     -------
     pkgs : list
         Names of packages on the local disk
 
     """
+    warn("Function Depreciated --> please use scopesim.download_package-s-()",
+         DeprecationWarning, stacklevel=2)
     dirnames = os.listdir(path)
     pkgs = []
 
     for dname in dirnames:
         if os.path.exists(os.path.join(path, dname, dname+".yaml")):
             pkgs += [dname]
 
@@ -162,8 +165,7 @@
 
         except HTTPError:
             raise ValueError(f"Unable to find file: {url + pkg_path}")
 
         save_path = os.path.abspath(save_path)
 
     return save_path
-
```

### Comparing `ScopeSim-0.5.6/scopesim/source/source.py` & `ScopeSim-0.6.0/scopesim/source/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 # table columns = x, y, spec_id, weight
 # table meta keywords = x_unit, y_unit
 #
 # image header keywords = WCS, SPEC_ID, WEIGHT
 # [WCS = CRPIXn, CRVALn = (0,0), CTYPEn, CDn_m, NAXISn, CUNITn
 """
 
-import os
 import pickle
 import logging
 from copy import deepcopy
+from pathlib import Path
 import numpy as np
 
 from astropy.table import Table, Column
 from astropy.io import ascii as ioascii
 from astropy.io import fits
 from astropy import units as u
 from astropy.wcs import WCS
@@ -177,31 +177,31 @@
         elif image_hdu is not None and flux is not None:
             self._from_imagehdu_and_flux(image_hdu, flux)
 
         elif image_hdu is not None and flux is None and spectra is None:
             if image_hdu.header.get("BUNIT") is not None:
                 self._from_imagehdu_only(image_hdu)
             else:
-                msg = f"image_hdu must be accompanied by either spectra or flux:\n" \
-                      f"spectra: {spectra}, flux: {flux}"
+                msg = ("image_hdu must be accompanied by either spectra or flux:\n"
+                       f"spectra: {spectra}, flux: {flux}")
                 logging.exception(msg)
                 raise ValueError(msg)
 
         elif x is not None and y is not None and \
                 ref is not None and spectra is not None:
             self._from_arrays(x, y, ref, weight, spectra)
 
     def _from_file(self, filename, spectra, flux):
         filename = utils.find_file(filename)
 
         if utils.is_fits(filename):
             fits_type = utils.get_fits_type(filename)
             data = fits.getdata(filename)
             hdr = fits.getheader(filename)
-            hdr['FILENAME'] = os.path.basename(filename)
+            hdr["FILENAME"] = Path(filename).name
             if fits_type == "image":
                 image = fits.ImageHDU(data=data, header=hdr)
                 if spectra is not None:
                     self._from_imagehdu_and_spectra(image, spectra)
                 elif flux is not None:
                     self._from_imagehdu_and_flux(image, flux)
                 else:
@@ -217,15 +217,15 @@
             tbl.meta.update(utils.convert_table_comments_to_dict(tbl))
             self._from_table(tbl, spectra)
 
     def _from_table(self, tbl, spectra):
         if "weight" not in tbl.colnames:
             tbl.add_column(Column(name="weight", data=np.ones(len(tbl))))
         tbl["ref"] += len(self.spectra)
-        self.fields += [tbl]
+        self.fields.append(tbl)
         self.spectra += spectra
 
     def _from_imagehdu_and_spectra(self, image_hdu, spectra):
         if not image_hdu.header.get("BG_SRC"):
             image_hdu.header["CRVAL1"] = 0
             image_hdu.header["CRVAL2"] = 0
             image_hdu.header["CRPIX1"] = image_hdu.header["NAXIS1"] / 2
@@ -257,15 +257,15 @@
         for i in [1, 2]:
             # Do not test for CUNIT or CDELT so that it throws an exception
             unit = u.Unit(image_hdu.header["CUNIT"+str(i)].lower())
             val = float(image_hdu.header["CDELT"+str(i)])
             image_hdu.header["CUNIT"+str(i)] = "DEG"
             image_hdu.header["CDELT"+str(i)] = val * unit.to(u.deg)
 
-        self.fields += [image_hdu]
+        self.fields.append(image_hdu)
 
     def _from_imagehdu_and_flux(self, image_hdu, flux):
         if isinstance(flux, u.Unit):
             flux = 1 * flux
 
         spec_template = src_tmp.vega_spectrum
         if isinstance(flux, u.Quantity):
@@ -277,17 +277,18 @@
         self._from_imagehdu_and_spectra(image_hdu, spectra)
 
     def _from_imagehdu_only(self, image_hdu):
         bunit = image_hdu.header.get("BUNIT")
         try:
             bunit = u.Unit(bunit)
         except ValueError:
-            f"Astropy cannot parse BUNIT [{bunit}].\n" \
-            f"You can bypass this check by passing an astropy Unit to the flux parameter:\n" \
-            f">>> Source(image_hdu=..., flux=u.Unit(bunit), ...)"
+            print(f"Astropy cannot parse BUNIT [{bunit}].\n"
+                  "You can bypass this check by passing an astropy Unit to "
+                  "the flux parameter:\n"
+                  ">>> Source(image_hdu=..., flux=u.Unit(bunit), ...)")
 
         value = 0 if bunit in [u.mag, u.ABmag] else 1
         self._from_imagehdu_and_flux(image_hdu, value * bunit)
 
     def _from_arrays(self, x, y, ref, weight, spectra):
         if weight is None:
             weight = np.ones(len(x))
@@ -295,15 +296,15 @@
         x = utils.quantify(x, u.arcsec)
         y = utils.quantify(y, u.arcsec)
         tbl = Table(names=["x", "y", "ref", "weight"],
                     data=[x, y, np.array(ref) + len(self.spectra), weight])
         tbl.meta["x_unit"] = "arcsec"
         tbl.meta["y_unit"] = "arcsec"
 
-        self.fields += [tbl]
+        self.fields.append(tbl)
         self.spectra += spectra
 
     def _from_cube(self, cube, ext=0):
         """
 
         Parameters
         ----------
@@ -320,30 +321,31 @@
             data = cube.data
             header = cube.header
             wcs = WCS(cube)
         else:
             with fits.open(cube) as hdul:
                 data = hdul[ext].data
                 header = hdul[ext].header
-                header['FILENAME'] = os.path.basename(cube)
+                header["FILENAME"] = Path(cube).name
                 wcs = WCS(cube)
 
         try:
-            bunit = header['BUNIT']
+            bunit = header["BUNIT"]
             u.Unit(bunit)
         except KeyError:
             bunit = "erg / (s cm2 arcsec2)"
-            logging.warning("Keyword 'BUNIT' not found, setting to %s by default", bunit)
+            logging.warning("Keyword \"BUNIT\" not found, setting to %s by default",
+                            bunit)
         except ValueError as errcode:
-            print("'BUNIT' keyword is malformed:", errcode)
+            print("\"BUNIT\" keyword is malformed:", errcode)
             raise
 
         # Compute the wavelength vector. This will be attached to the cube_hdu
         # as a new `wave` attribute.  This is not optimal coding practice.
-        wave = wcs.all_pix2world(header['CRPIX1'], header['CRPIX2'],
+        wave = wcs.all_pix2world(header["CRPIX1"], header["CRPIX2"],
                                  np.arange(data.shape[0]), 0)[-1]
 
         wave = (wave * u.Unit(wcs.wcs.cunit[-1])).to(u.um,
                                                      equivalencies=u.spectral())
 
         # WCS keywords must be updated because astropy.wcs converts wavelengths to 'm'
         header.update(wcs.to_header())
@@ -351,15 +353,15 @@
         target_cube = data
         target_hdr = header.copy()
         target_hdr["BUNIT"] = bunit
 
         cube_hdu = fits.ImageHDU(data=target_cube, header=target_hdr)
         cube_hdu.wave = wave          # ..todo: review wave attribute, bad practice
 
-        self.fields += [cube_hdu]
+        self.fields.append(cube_hdu)
 
     @property
     def table_fields(self):
         """List of fields that are defined through tables"""
         fields = [field for field in self.fields if isinstance(field, Table)]
         return fields
 
@@ -458,21 +460,21 @@
 
     def image(self, wave_min, wave_max, **kwargs):
         return self.image_in_range(wave_min, wave_max, **kwargs)
 
     @classmethod
     def load(cls, filename):
         """Load :class:'.Source' object from filename"""
-        with open(filename, 'rb') as fp1:
+        with open(filename, "rb") as fp1:
             src = pickle.load(fp1)
         return src
 
     def dump(self, filename):
         """Save to filename as a pickle"""
-        with open(filename, 'wb') as fp1:
+        with open(filename, "wb") as fp1:
             pickle.dump(self, fp1)
 
     # def collapse_spectra(self, wave_min=None, wave_max=None):
     #     for spec in self.spectra:
     #         waves = spec.waveset
     #         if wave_min is not None and wave_max is not None:
     #             mask = (waves >= wave_min) * (waves <= wave_max)
@@ -549,17 +551,17 @@
         new_source = Source()
         new_source.meta = deepcopy(self.meta)
         new_source._meta_dicts = deepcopy(self._meta_dicts)
         new_source.spectra = deepcopy(self.spectra)
         for field in self.fields:
             if isinstance(field, (fits.ImageHDU, fits.PrimaryHDU)) \
                     and field._file is not None:  # and field._data_loaded is False:
-                new_source.fields += [field]
+                new_source.fields.append(field)
             else:
-                new_source.fields += [deepcopy(field)]
+                new_source.fields.append(deepcopy(field))
 
         return new_source
 
     def append(self, source_to_add):
         new_source = source_to_add.make_copy()
         # If there is no field yet, then self._meta_dicts contains a
         # reference to self.meta, which is empty. This ensures that both are
@@ -568,27 +570,26 @@
         if len(self.fields) == 0:
             assert self._meta_dicts == [{}]
             self._meta_dicts = []
         if isinstance(source_to_add, Source):
             for field in new_source.fields:
                 if isinstance(field, Table):
                     field["ref"] += len(self.spectra)
-                    self.fields += [field]
+                    self.fields.append(field)
 
                 elif isinstance(field, (fits.ImageHDU, fits.PrimaryHDU)):
                     if ("SPEC_REF" in field.header and
                         isinstance(field.header["SPEC_REF"], int)):
                         field.header["SPEC_REF"] += len(self.spectra)
-                    self.fields += [field]
+                    self.fields.append(field)
                 self.spectra += new_source.spectra
 
                 self._meta_dicts += source_to_add._meta_dicts
         else:
-            raise ValueError("Cannot add {} object to Source object"
-                             "".format(type(new_source)))
+            raise ValueError(f"Cannot add {type(new_source)} object to Source object")
 
     def __add__(self, new_source):
         self_copy = self.make_copy()
         self_copy.append(new_source)
         return self_copy
 
     def __radd__(self, new_source):
@@ -606,8 +607,8 @@
                 num_spec = "-"
                 msg += f"[{ifld}]: ImageHDU with size {im_size}"
                 if "SPEC_REF" in self.fields[ifld].header:
                     num_spec = self.fields[ifld].header["SPEC_REF"]
                     msg += f", referencing spectrum {num_spec}"
                 msg += "\n"
 
-        return msg
+        return msg
```

### Comparing `ScopeSim-0.5.6/scopesim/source/source_templates.py` & `ScopeSim-0.6.0/scopesim/source/source_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from os import path as pth
+from pathlib import Path
 
 import numpy as np
 
 from astropy import units as u
 from astropy.table import Table
 from astropy.io import fits
 from astropy.utils.decorators import deprecated_renamed_argument
@@ -11,16 +11,14 @@
 from synphot.units import PHOTLAM
 
 from ..optics import image_plane_utils as ipu
 from .source_utils import make_img_wcs_header
 from .source import Source
 from .. import rc
 
-__all__ = ["empty_sky", "star", "star_field"]
-
 
 def empty_sky(flux=0):
     """
     Returns an empty source so that instrumental fluxes can be simulated
 
     Returns
     -------
@@ -28,15 +26,15 @@
 
     """
     sky = Source(lam=[0.3, 3.0]*u.um, spectra=[flux, flux]*PHOTLAM,
                  x=[0], y=[0], ref=[0], weight=[1])
     return sky
 
 
-@deprecated_renamed_argument('mag', 'flux', '0.1.5')
+@deprecated_renamed_argument("mag", "flux", "0.1.5")
 def star(x=0, y=0, flux=0):
     """
     Source object for a single star in either vega, AB magnitudes, or Jansky
 
     The star is associated with the reference spectrum for each photometric
     system, therefore a reference wavelength or filter does not need to be given
 
@@ -69,15 +67,15 @@
     ref = 0
 
     tbl = Table(data=[[x], [y], [w], [ref], [flux]],
                 names=["x", "y", "weight", "ref", "mag"],
                 units=[u.arcsec, u.arcsec, None, None, mag_unit])
     tbl.meta["photometric_system"] = "vega" if mag_unit == u.mag else "ab"
     src = Source(spectra=spec, table=tbl)
-    src.meta.update({"function_call": f"star(x={x}, y={y}, flux={flux})",
+    src.meta.update({"function_call": f"star({x=}, {y=}, {flux=})",
                      "module": "scopesim.source.source_templates",
                      "object": "star"})
 
     return src
 
 
 def star_field(n, mmin, mmax, width, height=None, use_grid=False):
@@ -269,15 +267,17 @@
 
     return src
 
 
 def vega_spectrum(mag=0):
     if isinstance(mag, u.Quantity):
         mag = mag.value
-    vega = SourceSpectrum.from_file(pth.join(rc.__pkg_dir__, "vega.fits"))
+    # HACK: Turn Path object back into string, because not everything
+    #       that depends on this function can handle Path objects (yet)
+    vega = SourceSpectrum.from_file(str(Path(rc.__pkg_dir__, "vega.fits")))
     vega = vega * 10 ** (-0.4 * mag)
     return vega
 
 
 def st_spectrum(mag=0):
     # ..todo: the waves vector is a bit random, in particular its length, but sets the resolution of
     #         the final spectrum in scopesim. Can this be make more general?
```

### Comparing `ScopeSim-0.5.6/scopesim/source/source_utils.py` & `ScopeSim-0.6.0/scopesim/source/source_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,35 +9,35 @@
 from .. import utils
 
 
 def validate_source_input(**kwargs):
     if "filename" in kwargs and kwargs["filename"] is not None:
         filename = kwargs["filename"]
         if utils.find_file(filename) is None:
-            logging.warning("filename was not found: {}".format(filename))
+            logging.warning("filename was not found: %s", filename)
 
     if "image" in kwargs and kwargs["image"] is not None:
         image_hdu = kwargs["image"]
         if not isinstance(image_hdu, (fits.PrimaryHDU, fits.ImageHDU)):
             raise ValueError("image must be fits.HDU object with a WCS."
-                             "type(image) == {}".format(type(image_hdu)))
+                             f"{type(image_hdu) = }")
 
         if len(wcs.find_all_wcs(image_hdu.header)) == 0:
-            logging.warning("image does not contain valid WCS. {}"
-                          "".format(wcs.WCS(image_hdu)))
+            logging.warning("image does not contain valid WCS. %s",
+                            wcs.WCS(image_hdu))
 
     if "table" in kwargs and kwargs["table"] is not None:
         tbl = kwargs["table"]
         if not isinstance(tbl, Table):
             raise ValueError("table must be an astropy.Table object:"
-                             "{}".format(type(tbl)))
+                             f"{type(tbl) = }")
 
         if not np.all([col in tbl.colnames for col in ["x", "y", "ref"]]):
             raise ValueError("table must contain at least column names: "
-                             "'x, y, ref': {}".format(tbl.colnames))
+                             f"'x, y, ref': {tbl.colnames}")
 
     return True
 
 
 def convert_to_list_of_spectra(spectra, lam):
     spectra_list = []
     if isinstance(spectra, SourceSpectrum):
@@ -255,9 +255,7 @@
 #         imagehdu.data = imagehdu.data.value
 #     else:
 #         unit = ""
 #         logging.warning("No flux unit found on ImageHDU. Please add BUNIT or "
 #                       "FLUXUNIT to the header.")
 #
 #     return unit
-
-
```

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/ATMO_default_NIR_IMG.dat` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/ATMO_default_NIR_IMG.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/INS_ifu_traces.fits` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/INS_ifu_traces.fits`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/INS_lss_traces.fits` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/INS_lss_traces.fits`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/YAML_atmosphere.yaml` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/YAML_atmosphere.yaml`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/YAML_basic_instrument.yaml` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/YAML_basic_instrument.yaml`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/YAML_detector.yaml` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/YAML_detector.yaml`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/YAML_mode_ifu.yaml` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/YAML_mode_ifu.yaml`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/YAML_mode_spectroscopy.yaml` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/YAML_mode_spectroscopy.yaml`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/YAML_telescope.yaml` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/YAML_telescope.yaml`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/code/make_spectral_trace.py` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/code/make_spectral_trace.py`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/default.yaml` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/default.yaml`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/filters/TC_filter_BrGamma.dat` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/filters/TC_filter_BrGamma.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/filters/TC_filter_CH4.dat` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/filters/TC_filter_CH4.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/filters/TC_filter_H.dat` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/filters/TC_filter_H.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/filters/TC_filter_J.dat` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/filters/TC_filter_J.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/basic_instrument/filters/TC_filter_Ks.dat` & `ScopeSim-0.6.0/scopesim/tests/mocks/basic_instrument/filters/TC_filter_Ks.dat`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/tests/mocks/load_basic_instrument.py` & `ScopeSim-0.6.0/scopesim/tests/mocks/load_basic_instrument.py`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/utils.py` & `ScopeSim-0.6.0/scopesim/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,28 @@
 """
 Helper functions for ScopeSim
 """
 import math
-import os
 from pathlib import Path
 import sys
 import logging
-import logging
 from collections import OrderedDict
 from docutils.core import publish_string
 from copy import deepcopy
 
 import requests
 import yaml
 import numpy as np
 from astropy import units as u
 from astropy.io import fits
-from astropy.io import ascii as ioascii
 from astropy.table import Column, Table
 
 from . import rc
 
 
-def msg(cmds, message, level=3):
-    """
-    Prints a message based on the level of verbosity given in cmds
-
-    Parameters
-    ----------
-    cmds : UserCommands
-        just for the SIM_VERBOSE and SIM_MESSAGE_LEVEL keywords
-    message : str
-        message to be printed
-    level : int, optional
-        all messages with level <= SIM_MESSAGE_LEVEL are printed. I.e. level=5
-        messages are not important, level=1 are very important
-    """
-    if cmds["SIM_VERBOSE"] == "yes" and level <= cmds["SIM_MESSAGE_LEVEL"]:
-        print(message)
-
-
 def unify(x, unit, length=1):
     """
     Convert all types of input to an astropy array/unit pair
 
     Parameters
     ----------
     x : int, float, np.ndarray, astropy.Quantity
@@ -107,15 +86,15 @@
     """
     # Convert angles to radians
     ha = ha / 12. * np.pi
     de = np.deg2rad(de)
     lat = np.deg2rad(lat)
 
     eta = np.arctan2(np.cos(lat) * np.sin(ha),
-                     np.sin(lat) * np.cos(de) - \
+                     np.sin(lat) * np.cos(de) -
                      np.cos(lat) * np.sin(de) * np.cos(ha))
 
     return np.rad2deg(eta)
 
 
 def moffat(r, alpha, beta):
     """
@@ -127,15 +106,15 @@
     alpha
     beta
 
     Returns
     -------
     eta
     """
-    return (beta - 1)/(np.pi * alpha**2) * (1 + (r/alpha)**2)**(-beta)
+    return (beta - 1) / (np.pi * alpha ** 2) * (1 + (r / alpha) ** 2) ** (-beta)
 
 
 def poissonify(arr):
     """
     Add a realisation of the poisson process to the array 'arr'.
 
     Parameters
@@ -170,46 +149,48 @@
     """
     if isinstance(val, (list, tuple, np.ndarray)):
         arr = np.array(arr)
         return [nearest(arr, i) for i in val]
 
     return np.argmin(abs(arr - val))
 
+
 def power_vector(val, degree):
     """Return the vector of powers of val up to a degree"""
     if degree < 0 or not isinstance(degree, int):
         raise ValueError("degree must be a positive integer")
 
-    return np.array([val**exp for exp in range(degree + 1)])
+    return np.array([val ** exp for exp in range(degree + 1)])
+
 
 def deriv_polynomial2d(poly):
     """Derivatives (gradient) of a Polynomial2D model
 
     Parameters
     ----------
     poly : astropy.modeling.models.Polynomial2D
 
-    Output
-    ------
+    Returns
+    -------
     gradient : tuple of Polynomial2d
     """
     import re
     from astropy.modeling.models import Polynomial2D
     degree = poly.degree
     dpoly_dx = Polynomial2D(degree=degree - 1)
     dpoly_dy = Polynomial2D(degree=degree - 1)
     regexp = re.compile(r'c(\d+)_(\d+)')
     for pname in poly.param_names:
         # analyse the name
         match = regexp.match(pname)
         i = int(match.group(1))
         j = int(match.group(2))
         cij = getattr(poly, pname)
-        pname_x = "c%d_%d" % (i-1, j)
-        pname_y = "c%d_%d" % (i, j-1)
+        pname_x = "c%d_%d" % (i - 1, j)
+        pname_y = "c%d_%d" % (i, j - 1)
         setattr(dpoly_dx, pname_x, i * cij)
         setattr(dpoly_dy, pname_y, j * cij)
 
     return dpoly_dx, dpoly_dy
 
 
 def add_keyword(filename, keyword, value, comment="", ext=0):
@@ -229,52 +210,14 @@
     """
     f = fits.open(filename, mode="update")
     f[ext].header[keyword] = (value, comment)
     f.flush()
     f.close()
 
 
-def add_SED_to_scopesim(file_in, file_out=None, wave_units="um"):
-    """
-    Adds the SED given in ``file_in`` to the ScopeSim data directory
-
-    Parameters
-    ----------
-    file_in : str
-        path to the SED file. Can be either FITS or ASCII format with 2 columns
-        Column 1 is the wavelength, column 2 is the flux
-    file_out : str, optional
-        Default is None. The file path to save the ASCII file. If ``None``, the SED
-        is saved to the ScopeSim data directory i.e. to ``rc.__data_dir__``
-    wave_units : str, astropy.Units
-        Units for the wavelength column, either as a string or as astropy units
-        Default is [um]
-
-    """
-
-    file_name, file_ext = os.path.basename(file_in).split(".")
-
-    if file_out is None:
-        if "SED_" not in file_name:
-            file_out = rc.__data_dir__ + "SED_" + file_name + ".dat"
-        else: file_out = rc.__data_dir__ + file_name + ".dat"
-
-    if file_ext.lower() in "fits":
-        data = fits.getdata(file_in)
-        lam, val = data[data.columns[0].name], data[data.columns[1].name]
-    else:
-        lam, val = ioascii.read(file_in)[:2]
-
-    lam = (lam * u.Unit(wave_units)).to(u.um)
-    mask = (lam > 0.3*u.um) * (lam < 5.0*u.um)
-
-    np.savetxt(file_out, np.array((lam[mask], val[mask]), dtype=np.float32).T,
-               header="wavelength    value \n [um]         [flux]")
-
-
 def airmass_to_zenith_dist(airmass):
     """
     returns zenith distance in degrees
 
     Z = arccos(1/X)
     """
     return np.rad2deg(np.arccos(1. / airmass))
@@ -304,15 +247,15 @@
     start, stop: [int, float]
         the starting and (maximal) end values of the sequence.
 
     step : [int, float]
         increment of the sequence, defaults to 1
 
     """
-    feps = 1e-10     # value used in R seq.default
+    feps = 1e-10  # value used in R seq.default
 
     delta = stop - start
     if delta == 0 and stop == 0:
         return stop
     try:
         npts = delta / step
     except ZeroDivisionError:
@@ -331,29 +274,29 @@
     if reldd < 100 * sys.float_info.epsilon:
         return start
 
     if isinstance(delta, int) and isinstance(step, int):
         # integer sequence
         npts = int(npts)
         return start + np.asarray(range(npts + 1)) * step
+
+    npts = int(npts + feps)
+    sequence = start + np.asarray(range(npts + 1)) * step
+    # correct for possible overshot because of fuzz (from seq.R)
+    if step > 0:
+        return np.minimum(sequence, stop)
     else:
-        npts = int(npts + feps)
-        sequence = start + np.asarray(range(npts + 1)) * step
-        # correct for possible overshot because of fuzz (from seq.R)
-        if step > 0:
-            return np.minimum(sequence, stop)
-        else:
-            return np.maximum(sequence, stop)
+        return np.maximum(sequence, stop)
 
 
 def add_mags(mags):
     """
     Returns a combined magnitude for a group of py_objects with ``mags``
     """
-    return -2.5*np.log10((10**(-0.4*np.array(mags))).sum())
+    return -2.5 * np.log10((10 ** (-0.4 * np.array(mags))).sum())
 
 
 def dist_mod_from_distance(d):
     """
     mu = 5 * np.log10(d) - 5
     """
 
@@ -362,15 +305,15 @@
 
 
 def distance_from_dist_mod(mu):
     """
     d = 10**(1 + mu / 5)
     """
 
-    d = 10**(1 + mu / 5)
+    d = 10 ** (1 + mu / 5)
     return d
 
 
 def telescope_diffraction_limit(aperture_size, wavelength, distance=None):
     """
     Returns the diffraction limit of a telescope
 
@@ -391,15 +334,15 @@
     -------
     diff_limit : float
         [arcsec] The angular diffraction limit.
         If distance is not None, diff_limit is in the same units as distance
 
     """
 
-    diff_limit = (((wavelength*u.um)/(aperture_size*u.m))*u.rad).to(u.arcsec).value
+    diff_limit = (((wavelength * u.um) / (aperture_size * u.m)) * u.rad).to(u.arcsec).value
 
     if distance is not None:
         diff_limit *= distance / u.pc.to(u.AU)
 
     return diff_limit
 
 
@@ -473,15 +416,14 @@
     which : str
         ["console", "file"]
     level : str
         ["ON", "OFF", "DEBUG", "INFO", "WARN", "ERROR", "CRITICAL"]
 
     """
 
-
     hdlr_name = f"scopesim_{which}_logger"
     level = {"ON": "INFO", "OFF": "CRITICAL"}.get(level.upper(), level)
     logger = logging.getLogger()
     logger.setLevel(level)
     for hdlr in logger.handlers:
         if hdlr.name == hdlr_name:
             hdlr.setLevel(level)
@@ -538,36 +480,41 @@
     -------
     Absolute path of the file
     """
 
     if filename is None or filename.lower() == "none":
         return None
 
-    if filename[0] == "!":
+    if filename.startswith("!"):
         filename = from_currsys(filename)
+    # Turn into pathlib.Path object for better manipulation afterwards
+    filename = Path(filename)
 
     if path is None:
         path = rc.__search_path__
 
-    if os.path.isabs(filename):
+    if filename.is_absolute():
         # absolute path: only path to try
         trynames = [filename]
     else:
         # try to find the file in a search path
-        trynames = [os.path.join(trydir, *os.path.split(filename))
+        trynames = [Path(trydir, filename)
                     for trydir in path if trydir is not None]
 
     for fname in trynames:
-        if os.path.exists(fname):   # success
+        if fname.exists():  # success
             # strip leading ./
-            while fname[:2] == './':
-                fname = fname[2:]
-            return fname
-        else:
-            continue
+            # Path should take care of this automatically!
+            # while fname[:2] == './':
+            #     fname = fname[2:]
+            # Nevertheless, make sure this is actually the case...
+            assert not str(fname).startswith("./")
+            # HACK: Turn Path object back into string, because not everything
+            #       that depends on this function can handle Path objects (yet)
+            return str(fname)
 
     # no file found
     msg = f"File cannot be found: {filename}"
     if not silent:
         logging.error(msg)
 
     if from_currsys("!SIM.file.error_on_missing_file") is True:
@@ -600,31 +547,31 @@
     airmass : float (>= 1)
 
     Returns
     -------
     zenith distance in degrees
     """
 
-    return np.rad2deg(np.arccos(1/airmass))
+    return np.rad2deg(np.arccos(1 / airmass))
 
 
 def convert_table_comments_to_dict(tbl):
 
     comments_dict = {}
     if "comments" in tbl.meta:
         try:
             comments_str = "\n".join(tbl.meta["comments"])
             comments_dict = yaml.full_load(comments_str)
-        except:
+        except yaml.error.YAMLError:
             logging.warning("Couldn't convert <table>.meta['comments'] to dict")
             comments_dict = tbl.meta["comments"]
     elif "COMMENT" in tbl.meta:
         try:
             comments_dict = yaml.full_load("\n".join(tbl.meta["COMMENT"]))
-        except:
+        except yaml.error.YAMLError:
             logging.warning("Couldn't convert <table>.meta['COMMENT'] to dict")
             comments_dict = tbl.meta["COMMENT"]
     else:
         logging.debug("No comments in table")
 
     return comments_dict
 
@@ -652,15 +599,15 @@
 
 def real_colname(name, colnames, silent=True):
     names = [name.lower(), name.upper(), name[0].upper() + name[1:].lower()]
     real_name = [name for name in names if name in colnames]
     if len(real_name) == 0:
         real_name = None
         if not silent:
-            logging.warning("None of {} were found in {}".format(names, colnames))
+            logging.warning("None of %s were found in %s", names, colnames)
     else:
         real_name = real_name[0]
 
     return real_name
 
 
 def insert_into_ordereddict(dic, new_entry, pos):
@@ -677,16 +624,18 @@
     new_dic = new_dic[:pos] + new_entry + new_dic[pos:]
     new_dic = OrderedDict(new_dic)
 
     return new_dic
 
 
 def empty_type(x):
-    type_dict = {int: 0, float: 0., bool: False, str: " ",
-                 list: [], tuple: (), dict: {}}
+    type_dict = {
+        int: 0, float: 0., bool: False, str: " ",
+        list: [], tuple: (), dict: {}
+    }
     if "<U" in str(x):
         x = str
 
     return type_dict[x]
 
 
 def get_meta_quantity(meta_dict, name, fallback_unit=""):
@@ -743,15 +692,14 @@
         if isinstance(item, (np.ndarray, list, tuple)) and np.size(item) > 1000:
             quant = item << u.Unit(unit)
         else:
             quant = item * u.Unit(unit)
     return quant
 
 
-
 def extract_type_from_unit(unit, unit_type):
     """
     Extract ``astropy`` physical type from a compound unit
 
     Parameters
     ----------
     unit : astropy.Unit
@@ -762,20 +710,18 @@
     -------
     new_unit : Unit
         The input unit minus any base units corresponding to ``unit_type``
     extracted_units : Unit
         Any base units corresponding to ``unit_type``
 
     """
-
-    unit = unit**1
     extracted_units = u.Unit("")
-    for base, power in zip(unit._bases, unit._powers):
-        if unit_type == (base**abs(power)).physical_type:
-            extracted_units *= base**power
+    for base, power in zip(unit.bases, unit.powers):
+        if unit_type == (base ** abs(power)).physical_type:
+            extracted_units *= base ** power
 
     new_unit = unit / extracted_units
 
     return new_unit, extracted_units
 
 
 def extract_base_from_unit(unit, base_unit):
@@ -792,21 +738,20 @@
     new_unit : Unit
         The input unit minus any base units corresponding to ``base_unit``
     extracted_units : Unit
         Any base units corresponding to ``base_unit``
 
     """
 
-    unit = unit**1
     extracted_units = u.Unit("")
-    for base, power in zip(unit._bases, unit._powers):
+    for base, power in zip(unit.bases, unit.powers):
         if base == base_unit:
-            extracted_units *= base**power
+            extracted_units *= base ** power
 
-    new_unit = unit * extracted_units**-1
+    new_unit = unit * extracted_units ** -1
 
     return new_unit, extracted_units
 
 
 def is_fits(filename):
     flag = False
     if filename is not None:
@@ -843,17 +788,16 @@
                 if len(col) < 1000:
                     col = col * u.Unit(com_tbl[colname_u])
                 else:
                     col = col << u.Unit(com_tbl[colname_u])
             else:
                 col = col * u.Unit(default_unit)
                 tbl_name = table.meta.get("name", table.meta.get("filename"))
-                logging.info("{}_unit was not found in table.meta: {}. "
-                             "Default to: {}"
-                             "".format(colname, tbl_name, default_unit))
+                logging.info(("%s_unit was not found in table.meta: %s. "
+                              "Default to: %s"), colname, tbl_name, default_unit)
 
     return col
 
 
 def unit_from_table(colname, table, default_unit=""):
     """
     Looks for the unit for a column based on the meta dict keyword "<col>_unit"
@@ -866,17 +810,16 @@
         unit = u.Unit(table.meta[colname_u])
     else:
         com_tbl = convert_table_comments_to_dict(table)
         if colname_u in com_tbl:
             unit = u.Unit(com_tbl[colname_u])
         else:
             tbl_name = table.meta.get("name", table.meta.get("filename"))
-            logging.info("{}_unit was not found in table.meta: {}. "
-                         "Default to: {}"
-                         "".format(colname, tbl_name, default_unit))
+            logging.info(("%s_unit was not found in table.meta: %s. "
+                          "Default to: %s"), colname, tbl_name, default_unit)
             unit = u.Unit(default_unit)
 
     return unit
 
 
 def deg2rad(theta):
     return theta * math.pi / 180
@@ -887,16 +830,16 @@
 
 
 def has_needed_keywords(header, suffix=""):
     """
     Check to see if the WCS keywords are in the header
     """
     keys = ["CDELT1", "CRVAL1", "CRPIX1"]
-    return sum([key + suffix in header.keys() for key in keys]) == 3 and \
-           "NAXIS1" in header.keys()
+    return (sum(key + suffix in header.keys() for key in keys) == 3 and
+            "NAXIS1" in header.keys())
 
 
 def stringify_dict(dic, ignore_types=(str, int, float)):
     """
     Turns a dict entries into strings for addition to FITS headers
     """
     from copy import deepcopy
@@ -922,15 +865,15 @@
     Returns
     -------
     orig_dict : dict
         Updated dict
 
     """
     for key in orig_dict:
-        if type(orig_dict[key]) is str and orig_dict[key] in new_entries:
+        if isinstance(orig_dict[key], str) and orig_dict[key] in new_entries:
             orig_dict[key] = new_entries[orig_dict[key]]
 
     return orig_dict
 
 
 def from_currsys(item):
     """
@@ -950,48 +893,47 @@
     if isinstance(item, list):
         item = [from_currsys(x) for x in item]
 
     if isinstance(item, dict):
         for key in item:
             item[key] = from_currsys(item[key])
 
-    if isinstance(item, str) and len(item) and item[0] == "!":
+    if isinstance(item, str) and len(item) and item.startswith("!"):
         if item in rc.__currsys__:
             item = rc.__currsys__[item]
         else:
-            raise ValueError("{} was not found in rc.__currsys__".format(item))
+            raise ValueError(f"{item} was not found in rc.__currsys__")
 
     if isinstance(item, str) and item.lower() == "none":
         item = None
 
     return item
 
 
 def check_keys(input_dict, required_keys, action="error", all_any="all"):
     """ Checks to see if all/any of the required keys are present in a dict """
 
     if isinstance(input_dict, (list, tuple)):
         input_dict = {key: None for key in input_dict}
 
     if all_any == "all":
-        keys_present = all([key in input_dict for key in required_keys])
+        keys_present = all(key in input_dict for key in required_keys)
     elif all_any == "any":
-        keys_present = any([key in input_dict for key in required_keys])
+        keys_present = any(key in input_dict for key in required_keys)
     else:
         raise ValueError("all_any must be either 'all' or 'any'")
 
     if not keys_present:
         if "error" in action:
-            raise ValueError("One or more of the following keys missing "
-                             "from input_dict: \n{} \n{}"
-                             "".format(required_keys, input_dict.keys()))
-        elif "warn" in action:
-            logging.warning("One or more of the following keys missing "
-                          "from input_dict: \n{} \n{}"
-                          "".format(required_keys, input_dict.keys()))
+            raise ValueError("One or more of the following keys missing from "
+                             f"input_dict: \n{required_keys} \n{input_dict.keys()}")
+        if "warn" in action:
+            logging.warning(("One or more of the following keys missing "
+                             "from input_dict: \n%s \n%s"), required_keys,
+                            input_dict.keys())
 
     return keys_present
 
 
 def interp2(x_new, x_orig, y_orig):
     """Checks and corrects for decreasing x_orig values"""
 
@@ -999,31 +941,31 @@
         y_new = np.interp(x_new, x_orig, y_orig)
     else:
         y_new = np.interp(x_new, x_orig[::-1], y_orig[::-1])
 
     return y_new
 
 
-def write_report(text, filename=None, output=["rst"]):
+def write_report(text, filename=None, output=None):
     """ Writes a report string to file in latex or rst format"""
-    if isinstance(output, str):
+    if output is None:
+        output = ["rst"]
+    elif isinstance(output, str):
         output = [output]
 
     if filename is not None:
         for fmt in output:
             out_text = deepcopy(text)
             if fmt.lower() == "latex":
                 out_text = publish_string(out_text, writer_name="latex")
                 out_text = out_text.decode("utf-8")
 
             suffix = {"rst": ".rst", "latex": ".tex"}[fmt]
-            fname = Path(filename)
-            fname = os.path.join(*fname.parts[:-1], fname.stem + suffix)
-            with open(fname, "w") as f:
-                f.write(out_text)
+            fname = Path(filename).with_suffix(suffix)
+            fname.write_text(out_text, encoding="utf-8")
 
 
 def pretty_print_dict(dic, indent=0):
     text = ""
     for key, value in dic.items():
         if isinstance(value, dict):
             text += " " * indent + f"{str(key)}:\n"
@@ -1044,23 +986,25 @@
     dic = response.json()
     run_id = dic["workflow_runs"][0]["id"]
 
     response = requests.get(f"https://api.github.com/repos/{owner_name}/{repo_name}/actions/runs/{run_id}/jobs")
     dic = response.json()
     params_list = []
     for job in dic["jobs"]:
-        params = {"name": job['name'],
-                  "status": job['status'],
-                  "conclusion": job['conclusion'],
-                  "started_at": job['started_at'],
-                  "completed_at": job['completed_at'],
-                  "url": job['html_url'],
-                  "badge_url": None}
+        params = {
+            "name": job['name'],
+            "status": job['status'],
+            "conclusion": job['conclusion'],
+            "started_at": job['started_at'],
+            "completed_at": job['completed_at'],
+            "url": job['html_url'],
+            "badge_url": None
+        }
 
         key = "Python_" + job['name'].split()[-1][:-1]
         value = "passing" if job['conclusion'] == "success" else "failing"
         colour = "brightgreen" if job['conclusion'] == "success" else "red"
         badge_url = f"https://img.shields.io/badge/{key}-{value}-{colour}"
         params["badge_url"] = badge_url
-        params_list += [params]
+        params_list.append(params)
 
     return params_list
```

### Comparing `ScopeSim-0.5.6/scopesim/vega.fits` & `ScopeSim-0.6.0/scopesim/vega.fits`

 * *Files identical despite different names*

### Comparing `ScopeSim-0.5.6/scopesim/version.py` & `ScopeSim-0.6.0/scopesim/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,23 @@
-version = '0.5.6'
-date    = '2023-03-13 16:00:00 GMT'
+from importlib import metadata
+version = metadata.version(__package__)
+date = '2023-07-10 10:00:00 GMT'
 yaml_descriptions = """
+- version : 0.6.0
+  date : 2023-07-10
+  comment : Summer 2023
+  changes :
+  - Rename MAORY to MORFEO #195
+  - Fix NCPA and PSF affecting spectroscopy #238
+  - Fix line widths bug #213
+  - Add rectification utilities #237
+  - Include grating efficiencies #215
+  - Improve downloading of IRDB #234
+  - Improve Windows support
+
 - version : 0.5.6
   date : 2023-03-13
   comment : Hotfix to include minimal set of SVO data
   changes :
   - Run notebooks in CI #183
   - Add SVO data because SVO is down #185
   - Fix OpticalTrain shared cmds attribute and fix docstring #186
```


# Comparing `tmp/vasprocar-1.1.15.6.tar.gz` & `tmp/vasprocar-1.1.15.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasprocar-1.1.15.6.tar", last modified: Fri May 19 16:09:06 2023, max compression
+gzip compressed data, was "vasprocar-1.1.15.7.tar", last modified: Mon Jul 10 21:49:23 2023, max compression
```

## Comparing `vasprocar-1.1.15.6.tar` & `vasprocar-1.1.15.7.tar`

### file list

```diff
@@ -1,95 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 16:09:06.784999 vasprocar-1.1.15.6/
--rw-rw-rw-   0        0        0    35822 2023-01-01 17:34:12.000000 vasprocar-1.1.15.6/LICENSE.txt
--rw-rw-rw-   0        0        0     2220 2023-05-19 16:09:06.784999 vasprocar-1.1.15.6/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2023-01-17 12:07:08.000000 vasprocar-1.1.15.6/README.md
--rw-rw-rw-   0        0        0      167 2023-05-19 16:09:06.784999 vasprocar-1.1.15.6/setup.cfg
--rw-rw-rw-   0        0        0     1234 2023-05-19 16:08:51.000000 vasprocar-1.1.15.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:09:05.999567 vasprocar-1.1.15.6/vasprocar/
--rw-rw-rw-   0        0        0      360 2023-04-28 15:54:36.000000 vasprocar-1.1.15.6/vasprocar/BibTeX.dat
--rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.15.6/vasprocar/DOI.png
--rw-rw-rw-   0        0        0     3673 2023-04-28 15:54:42.000000 vasprocar-1.1.15.6/vasprocar/VASProcar.py
--rw-rw-rw-   0        0        0      201 2023-03-10 21:53:46.000000 vasprocar-1.1.15.6/vasprocar/__init__.py
--rw-rw-rw-   0        0        0     3673 2023-04-28 15:54:15.000000 vasprocar-1.1.15.6/vasprocar/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:09:06.219321 vasprocar-1.1.15.6/vasprocar/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 16:09:06.407986 vasprocar-1.1.15.6/vasprocar/src/_VASP/
--rw-rw-rw-   0        0        0    18256 2023-04-26 12:33:54.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/_info.py
--rw-rw-rw-   0        0        0    13975 2023-02-01 18:32:31.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/_info_b.py
--rw-rw-rw-   0        0        0    15741 2023-02-05 19:46:41.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/_label.py
--rw-rw-rw-   0        0        0    31402 2023-04-16 15:59:10.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/_nscf.py
--rw-rw-rw-   0        0        0     9428 2023-02-07 22:29:38.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/_var_kpoints.py
--rw-rw-rw-   0        0        0    20816 2023-05-06 13:08:43.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/chgcar.py
--rw-rw-rw-   0        0        0    32155 2023-02-06 18:01:33.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/contribuicao.py
--rw-rw-rw-   0        0        0    14022 2023-02-07 16:02:48.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/dielectric_function.py
--rw-rw-rw-   0        0        0    26245 2023-02-07 16:02:09.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    28274 2023-02-07 16:01:48.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0    24344 2023-04-01 21:06:45.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/kpoints_2D_3D.py
--rw-rw-rw-   0        0        0    15068 2023-05-04 13:02:49.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/parchg.py
--rw-rw-rw-   0        0        0     8140 2023-04-27 16:07:00.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/poscar_replace.py
--rw-rw-rw-   0        0        0    14843 2023-05-04 13:03:13.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/potencial.py
--rw-rw-rw-   0        0        0    15029 2023-05-04 13:03:33.000000 vasprocar-1.1.15.6/vasprocar/src/_VASP/wave_function.py
--rw-rw-rw-   0        0        0      626 2023-02-07 16:00:07.000000 vasprocar-1.1.15.6/vasprocar/src/_loop.py
--rw-rw-rw-   0        0        0    16703 2023-05-04 12:41:29.000000 vasprocar-1.1.15.6/vasprocar/src/_settings.py
--rw-rw-rw-   0        0        0     2897 2023-03-23 12:12:59.000000 vasprocar-1.1.15.6/vasprocar/src/_update.py
--rw-rw-rw-   0        0        0    17291 2023-02-07 15:59:42.000000 vasprocar-1.1.15.6/vasprocar/src/bandas_2D.py
--rw-rw-rw-   0        0        0    16604 2023-02-07 22:46:17.000000 vasprocar-1.1.15.6/vasprocar/src/bandas_3D.py
--rw-rw-rw-   0        0        0    14962 2023-02-07 22:46:24.000000 vasprocar-1.1.15.6/vasprocar/src/bandas_4D.py
--rw-rw-rw-   0        0        0     2100 2023-02-06 17:36:59.000000 vasprocar-1.1.15.6/vasprocar/src/correction_file.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:09:06.424273 vasprocar-1.1.15.6/vasprocar/src/etc/
--rw-rw-rw-   0        0        0      360 2023-04-28 15:54:36.000000 vasprocar-1.1.15.6/vasprocar/src/etc/BibTeX.dat
--rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.15.6/vasprocar/src/etc/DOI.png
--rw-rw-rw-   0        0        0   374410 2022-06-01 18:31:32.000000 vasprocar-1.1.15.6/vasprocar/src/etc/Greek_alphabet.jpg
--rw-rw-rw-   0        0        0    20078 2023-02-07 22:46:33.000000 vasprocar-1.1.15.6/vasprocar/src/fermi_surface.py
--rw-rw-rw-   0        0        0    16978 2023-04-27 19:31:37.000000 vasprocar-1.1.15.6/vasprocar/src/level_countour.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:09:06.659315 vasprocar-1.1.15.6/vasprocar/src/plot/
-drwxrwxrwx   0        0        0        0 2023-05-19 16:09:06.784999 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/
--rw-rw-rw-   0        0        0     5204 2023-04-28 13:13:46.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_bandas_2D.py
--rw-rw-rw-   0        0        0     4322 2023-05-04 14:16:22.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_chgcar.py
--rw-rw-rw-   0        0        0     4960 2023-04-28 13:17:27.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_dielectric_function.py
--rw-rw-rw-   0        0        0    13180 2023-04-28 13:22:43.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    13278 2023-04-28 15:25:56.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0    11204 2023-04-28 15:27:51.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py
--rw-rw-rw-   0        0        0     3883 2023-05-03 16:43:07.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_parchg.py
--rw-rw-rw-   0        0        0     3807 2023-04-28 15:30:54.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_potencial.py
--rw-rw-rw-   0        0        0     6272 2023-04-28 15:35:06.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_projecao_localizacao.py
--rw-rw-rw-   0        0        0    11195 2023-04-28 15:41:27.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_projecao_orbitais.py
--rw-rw-rw-   0        0        0     6149 2023-04-28 15:45:01.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_projecao_psi.py
--rw-rw-rw-   0        0        0    10949 2023-04-28 15:49:29.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_projecao_spin.py
--rw-rw-rw-   0        0        0     4002 2023-04-28 15:51:35.000000 vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_wave_function.py
--rw-rw-rw-   0        0        0     6459 2023-04-26 19:46:07.000000 vasprocar-1.1.15.6/vasprocar/src/plot/_plot_settings.py
--rw-rw-rw-   0        0        0     5859 2023-04-26 19:52:01.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_bandas_2D.py
--rw-rw-rw-   0        0        0     5094 2023-04-27 16:26:15.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_bandas_3D_matplotlib.py
--rw-rw-rw-   0        0        0     5789 2023-04-27 16:25:56.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_bandas_3D_plotly.py
--rw-rw-rw-   0        0        0     5212 2023-04-27 16:30:27.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_bandas_4D_plotly.py
--rw-rw-rw-   0        0        0     5022 2023-05-04 14:15:37.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_chgcar.py
--rw-rw-rw-   0        0        0     4311 2023-04-27 16:32:25.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_dielectric_function.py
--rw-rw-rw-   0        0        0    12937 2023-04-27 16:41:40.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    34063 2023-04-27 16:53:46.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0     8368 2023-04-27 16:59:55.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_fermi_surface.py
--rw-rw-rw-   0        0        0     6527 2023-04-27 17:03:00.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_level_countour.py
--rw-rw-rw-   0        0        0     4693 2023-05-03 16:43:27.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_parchg.py
--rw-rw-rw-   0        0        0     4693 2023-04-27 17:09:05.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_potencial.py
--rw-rw-rw-   0        0        0    14161 2023-04-27 18:34:47.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_projecao_localizacao.py
--rw-rw-rw-   0        0        0    26915 2023-04-27 18:40:15.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_projecao_orbitais.py
--rw-rw-rw-   0        0        0    14283 2023-04-27 18:48:44.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_projecao_psi.py
--rw-rw-rw-   0        0        0     7782 2023-04-27 18:53:12.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_projecao_spin.py
--rw-rw-rw-   0        0        0    11866 2023-04-27 19:17:24.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_spin_texture_2D.py
--rw-rw-rw-   0        0        0     9865 2023-04-27 19:05:41.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_spin_texture_3D.py
--rw-rw-rw-   0        0        0     6287 2023-04-27 19:06:44.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_spin_texture_4D.py
--rw-rw-rw-   0        0        0     6345 2023-04-27 19:08:37.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_spin_texture_4D_[iso].py
--rw-rw-rw-   0        0        0    15772 2023-04-27 19:29:40.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_spin_texture_contour.py
--rw-rw-rw-   0        0        0    17321 2023-04-27 19:30:01.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_spin_texture_contour_video.py
--rw-rw-rw-   0        0        0     4600 2023-04-27 17:12:08.000000 vasprocar-1.1.15.6/vasprocar/src/plot/plot_wave_function.py
--rw-rw-rw-   0        0        0    26728 2023-02-09 23:53:36.000000 vasprocar-1.1.15.6/vasprocar/src/projecao_localizacao.py
--rw-rw-rw-   0        0        0    27714 2023-04-26 12:02:26.000000 vasprocar-1.1.15.6/vasprocar/src/projecao_orbitais.py
--rw-rw-rw-   0        0        0    33246 2023-02-14 20:05:13.000000 vasprocar-1.1.15.6/vasprocar/src/projecao_psi.py
--rw-rw-rw-   0        0        0    24325 2023-02-16 16:44:51.000000 vasprocar-1.1.15.6/vasprocar/src/projecao_spin.py
--rw-rw-rw-   0        0        0    22748 2023-02-14 20:11:56.000000 vasprocar-1.1.15.6/vasprocar/src/spin_texture.py
--rw-rw-rw-   0        0        0    22318 2023-04-27 19:32:03.000000 vasprocar-1.1.15.6/vasprocar/src/spin_texture_contour.py
--rw-rw-rw-   0        0        0    23728 2023-04-27 19:32:28.000000 vasprocar-1.1.15.6/vasprocar/src/spin_texture_contour_video.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:09:06.031450 vasprocar-1.1.15.6/vasprocar.egg-info/
--rw-rw-rw-   0        0        0     2220 2023-05-19 16:09:05.000000 vasprocar-1.1.15.6/vasprocar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3134 2023-05-19 16:09:05.000000 vasprocar-1.1.15.6/vasprocar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 16:09:05.000000 vasprocar-1.1.15.6/vasprocar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-19 16:09:05.000000 vasprocar-1.1.15.6/vasprocar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       91 2023-05-19 16:09:05.000000 vasprocar-1.1.15.6/vasprocar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 16:09:05.000000 vasprocar-1.1.15.6/vasprocar.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.491193 vasprocar-1.1.15.7/
+-rw-rw-rw-   0        0        0    35822 2023-01-01 17:34:12.000000 vasprocar-1.1.15.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     2220 2023-07-10 21:49:23.491193 vasprocar-1.1.15.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1589 2023-01-17 12:07:08.000000 vasprocar-1.1.15.7/README.md
+-rw-rw-rw-   0        0        0      167 2023-07-10 21:49:23.491193 vasprocar-1.1.15.7/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2023-07-10 21:49:06.000000 vasprocar-1.1.15.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.347075 vasprocar-1.1.15.7/vasprocar/
+-rw-rw-rw-   0        0        0      360 2023-04-28 15:54:36.000000 vasprocar-1.1.15.7/vasprocar/BibTeX.dat
+-rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.15.7/vasprocar/DOI.png
+-rw-rw-rw-   0        0        0     4569 2023-07-10 21:47:53.000000 vasprocar-1.1.15.7/vasprocar/VASProcar.py
+-rw-rw-rw-   0        0        0      201 2023-03-10 21:53:46.000000 vasprocar-1.1.15.7/vasprocar/__init__.py
+-rw-rw-rw-   0        0        0     4569 2023-07-10 21:47:53.000000 vasprocar-1.1.15.7/vasprocar/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.396126 vasprocar-1.1.15.7/vasprocar/src/
+drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.428205 vasprocar-1.1.15.7/vasprocar/src/_VASP/
+-rw-rw-rw-   0        0        0    18256 2023-04-26 12:33:54.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/_info.py
+-rw-rw-rw-   0        0        0    13975 2023-02-01 18:32:31.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/_info_b.py
+-rw-rw-rw-   0        0        0    15757 2023-07-10 18:09:15.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/_label.py
+-rw-rw-rw-   0        0        0    31402 2023-04-16 15:59:10.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/_nscf.py
+-rw-rw-rw-   0        0        0     9428 2023-02-07 22:29:38.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/_var_kpoints.py
+-rw-rw-rw-   0        0        0    20778 2023-07-03 13:16:41.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/chgcar.py
+-rw-rw-rw-   0        0        0    32155 2023-02-06 18:01:33.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/contribuicao.py
+-rw-rw-rw-   0        0        0    14022 2023-02-07 16:02:48.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/dielectric_function.py
+-rw-rw-rw-   0        0        0    26717 2023-07-10 19:38:20.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    28742 2023-07-10 19:40:51.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0    24344 2023-04-01 21:06:45.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/kpoints_2D_3D.py
+-rw-rw-rw-   0        0        0    15068 2023-05-04 13:02:49.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/parchg.py
+-rw-rw-rw-   0        0        0     8140 2023-04-27 16:07:00.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/poscar_replace.py
+-rw-rw-rw-   0        0        0     4159 2023-07-03 14:06:19.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/postar_combination.py
+-rw-rw-rw-   0        0        0    14843 2023-05-04 13:03:13.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/potencial.py
+-rw-rw-rw-   0        0        0    15029 2023-05-04 13:03:33.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/wave_function.py
+-rw-rw-rw-   0        0        0      626 2023-02-07 16:00:07.000000 vasprocar-1.1.15.7/vasprocar/src/_loop.py
+-rw-rw-rw-   0        0        0    17882 2023-07-10 21:37:23.000000 vasprocar-1.1.15.7/vasprocar/src/_settings.py
+-rw-rw-rw-   0        0        0     2897 2023-03-23 12:12:59.000000 vasprocar-1.1.15.7/vasprocar/src/_update.py
+-rw-rw-rw-   0        0        0    17818 2023-07-10 19:22:09.000000 vasprocar-1.1.15.7/vasprocar/src/bandas_2D.py
+-rw-rw-rw-   0        0        0    16604 2023-02-07 22:46:17.000000 vasprocar-1.1.15.7/vasprocar/src/bandas_3D.py
+-rw-rw-rw-   0        0        0    14962 2023-02-07 22:46:24.000000 vasprocar-1.1.15.7/vasprocar/src/bandas_4D.py
+-rw-rw-rw-   0        0        0     2100 2023-02-06 17:36:59.000000 vasprocar-1.1.15.7/vasprocar/src/correction_file.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.428205 vasprocar-1.1.15.7/vasprocar/src/etc/
+-rw-rw-rw-   0        0        0      360 2023-04-28 15:54:36.000000 vasprocar-1.1.15.7/vasprocar/src/etc/BibTeX.dat
+-rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.15.7/vasprocar/src/etc/DOI.png
+-rw-rw-rw-   0        0        0   374410 2022-06-01 18:31:32.000000 vasprocar-1.1.15.7/vasprocar/src/etc/Greek_alphabet.jpg
+-rw-rw-rw-   0        0        0    20078 2023-02-07 22:46:33.000000 vasprocar-1.1.15.7/vasprocar/src/fermi_surface.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.428205 vasprocar-1.1.15.7/vasprocar/src/inputs/
+-rw-rw-rw-   0        0        0     1010 2023-07-10 21:45:59.000000 vasprocar-1.1.15.7/vasprocar/src/inputs/inputs.py
+-rw-rw-rw-   0        0        0     3625 2023-07-10 21:43:57.000000 vasprocar-1.1.15.7/vasprocar/src/inputs/inputs_files.py
+-rw-rw-rw-   0        0        0    16978 2023-04-27 19:31:37.000000 vasprocar-1.1.15.7/vasprocar/src/level_countour.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.475081 vasprocar-1.1.15.7/vasprocar/src/plot/
+drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.491193 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/
+-rw-rw-rw-   0        0        0     5204 2023-04-28 13:13:46.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_bandas_2D.py
+-rw-rw-rw-   0        0        0     4322 2023-05-04 14:16:22.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_chgcar.py
+-rw-rw-rw-   0        0        0     4960 2023-04-28 13:17:27.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dielectric_function.py
+-rw-rw-rw-   0        0        0    13180 2023-04-28 13:22:43.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    13278 2023-04-28 15:25:56.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0    11204 2023-04-28 15:27:51.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py
+-rw-rw-rw-   0        0        0     3883 2023-05-03 16:43:07.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_parchg.py
+-rw-rw-rw-   0        0        0     3807 2023-04-28 15:30:54.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_potencial.py
+-rw-rw-rw-   0        0        0     6272 2023-04-28 15:35:06.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_localizacao.py
+-rw-rw-rw-   0        0        0    11195 2023-04-28 15:41:27.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_orbitais.py
+-rw-rw-rw-   0        0        0     6149 2023-04-28 15:45:01.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_psi.py
+-rw-rw-rw-   0        0        0    10949 2023-04-28 15:49:29.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_spin.py
+-rw-rw-rw-   0        0        0     4002 2023-04-28 15:51:35.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_wave_function.py
+-rw-rw-rw-   0        0        0     6459 2023-04-26 19:46:07.000000 vasprocar-1.1.15.7/vasprocar/src/plot/_plot_settings.py
+-rw-rw-rw-   0        0        0     5859 2023-04-26 19:52:01.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_2D.py
+-rw-rw-rw-   0        0        0     5094 2023-04-27 16:26:15.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_3D_matplotlib.py
+-rw-rw-rw-   0        0        0     5789 2023-04-27 16:25:56.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_3D_plotly.py
+-rw-rw-rw-   0        0        0     5212 2023-04-27 16:30:27.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_4D_plotly.py
+-rw-rw-rw-   0        0        0     5022 2023-05-04 14:15:37.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_chgcar.py
+-rw-rw-rw-   0        0        0     4311 2023-04-27 16:32:25.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_dielectric_function.py
+-rw-rw-rw-   0        0        0    12937 2023-04-27 16:41:40.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    34063 2023-04-27 16:53:46.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0     8368 2023-04-27 16:59:55.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_fermi_surface.py
+-rw-rw-rw-   0        0        0     6527 2023-04-27 17:03:00.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_level_countour.py
+-rw-rw-rw-   0        0        0     4693 2023-05-03 16:43:27.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_parchg.py
+-rw-rw-rw-   0        0        0     4693 2023-04-27 17:09:05.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_potencial.py
+-rw-rw-rw-   0        0        0    14161 2023-04-27 18:34:47.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_localizacao.py
+-rw-rw-rw-   0        0        0    26915 2023-04-27 18:40:15.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_orbitais.py
+-rw-rw-rw-   0        0        0    14283 2023-04-27 18:48:44.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_psi.py
+-rw-rw-rw-   0        0        0     7782 2023-04-27 18:53:12.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_spin.py
+-rw-rw-rw-   0        0        0    11866 2023-04-27 19:17:24.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_2D.py
+-rw-rw-rw-   0        0        0     9865 2023-04-27 19:05:41.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_3D.py
+-rw-rw-rw-   0        0        0     6287 2023-04-27 19:06:44.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_4D.py
+-rw-rw-rw-   0        0        0     6345 2023-04-27 19:08:37.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_4D_[iso].py
+-rw-rw-rw-   0        0        0    15772 2023-04-27 19:29:40.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_contour.py
+-rw-rw-rw-   0        0        0    17321 2023-04-27 19:30:01.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_contour_video.py
+-rw-rw-rw-   0        0        0     4600 2023-04-27 17:12:08.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_wave_function.py
+-rw-rw-rw-   0        0        0    26728 2023-02-09 23:53:36.000000 vasprocar-1.1.15.7/vasprocar/src/projecao_localizacao.py
+-rw-rw-rw-   0        0        0    28470 2023-07-10 19:37:56.000000 vasprocar-1.1.15.7/vasprocar/src/projecao_orbitais.py
+-rw-rw-rw-   0        0        0    33246 2023-02-14 20:05:13.000000 vasprocar-1.1.15.7/vasprocar/src/projecao_psi.py
+-rw-rw-rw-   0        0        0    25231 2023-07-10 19:36:12.000000 vasprocar-1.1.15.7/vasprocar/src/projecao_spin.py
+-rw-rw-rw-   0        0        0    22748 2023-02-14 20:11:56.000000 vasprocar-1.1.15.7/vasprocar/src/spin_texture.py
+-rw-rw-rw-   0        0        0    22318 2023-04-27 19:32:03.000000 vasprocar-1.1.15.7/vasprocar/src/spin_texture_contour.py
+-rw-rw-rw-   0        0        0    23728 2023-04-27 19:32:28.000000 vasprocar-1.1.15.7/vasprocar/src/spin_texture_contour_video.py
+drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.380541 vasprocar-1.1.15.7/vasprocar.egg-info/
+-rw-rw-rw-   0        0        0     2220 2023-07-10 21:49:23.000000 vasprocar-1.1.15.7/vasprocar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3244 2023-07-10 21:49:23.000000 vasprocar-1.1.15.7/vasprocar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 21:49:23.000000 vasprocar-1.1.15.7/vasprocar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-10 21:49:23.000000 vasprocar-1.1.15.7/vasprocar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       91 2023-07-10 21:49:23.000000 vasprocar-1.1.15.7/vasprocar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-10 21:49:23.000000 vasprocar-1.1.15.7/vasprocar.egg-info/top_level.txt
```

### Comparing `vasprocar-1.1.15.6/LICENSE.txt` & `vasprocar-1.1.15.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/PKG-INFO` & `vasprocar-1.1.15.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasprocar
-Version: 1.1.15.6
+Version: 1.1.15.7
 Summary: VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP code, through an interactive user interface.
 Home-page: https://doi.org/10.5281/zenodo.6343960
 Download-URL: https://doi.org/10.5281/zenodo.6343960
 Author: Augusto de Lelis Araujo and Renan da Paixao Maciel
 Author-email: augusto-lelis@outlook.com, renan.maciel@physics.uu.se
 License: GNU GPLv3
 Description-Content-Type: text/markdown
```

### Comparing `vasprocar-1.1.15.6/README.md` & `vasprocar-1.1.15.7/README.md`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/setup.py` & `vasprocar-1.1.15.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "vasprocar",
-    version = "1.1.15.6",
+    version = "1.1.15.7",
     entry_points={'console_scripts': ['vasprocar = vasprocar:main']},
     description = "VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP code, through an interactive user interface.",
     author = "Augusto de Lelis Araujo and Renan da Paixao Maciel", 
     author_email = "augusto-lelis@outlook.com, renan.maciel@physics.uu.se",
     url = "https://doi.org/10.5281/zenodo.6343960",
     download_url = "https://doi.org/10.5281/zenodo.6343960",
     license = "GNU GPLv3",
```

### Comparing `vasprocar-1.1.15.6/vasprocar/DOI.png` & `vasprocar-1.1.15.7/vasprocar/DOI.png`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/_info.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/_info.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/_info_b.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/_info_b.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/_label.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/_label.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,42 +70,41 @@
        confirmacao = input (" "); confirmacao = str(confirmacao)       
    #-----------------------------------   
 
    #============================================================================
    # Getting the number of k-points to be highlighted in the Bands structure ===
    #============================================================================
 
-   print("")
-   print ("=============================================================================================")
-   print ("Attention: Edit the KPOINTS file, inserting the desired label in the k-points of the file.   ")
-   print ("               !!!! All k-points present in the KPOINTS file, must be labeled !!!!           ")
-   print ("=============================================================================================")
-   print ("Example:                                                                                     ")
-   print ("         0.0 0.0 0.0 #1 (Gamma)                                                              ")
-   print ("         0.5 0.5 0.0 M                                                                       ")
-   print ("                                                                                             ")
-   print ("         0.5 0.5 0.0 M                                                                       ")
-   print ("         0.5 0.0 0.0 X                                                                       ")
-   print ("=============================================================================================")
-   print ("Use the following codes (#number) for using Greek symbols as labels:                         ")
-   print ("                                                                                             ")
-   print ("#1  = Gamma       |  #2  = gamma        |  #3  = Delta     |  #4  = delta       |               ")
-   print ("#5  = Lambda      |  #6  = lambda       |  #7  = Sigma     |  #8  = sigma       |               ")
-   print ("#9  = Theta       |  #10 = tetha        |  #11 = Omega     |  #12 = omega       |               ")
-   print ("#13 = Psi         |  #14 = psi          |  #15 = Phi       |  #16 = phi         |  #17 = varphi ")
-   print ("#18 = alfa        |  #19 = beta         |  #20 = pi        |  #21 = rho         |               ")
-   print ("#22 = tau         |  #23 = upsilon      |  #24 = mu        |  #25 = nu          |               ")
-   print ("#26 = epsilon     |  #27 = eta          |  #28 = kappa     |  #29 = xi          |  #30 = zeta   ")
-   print ("#31 = left_arrow  |  #32 = right_arrow  |  #33 = up_arrow  |  #34 = down_arrow  |               ")
-   print ("=============================================================================================")
-   print ("After editing the KPOINTS file, press [ENTER] to continue                                    ")
-   print ("=============================================================================================")
-   confirmacao = input (" "); confirmacao = str(confirmacao)       
-
-   #===================================================================================
+   if (len(inputs) == 0):
+      print("")
+      print ("=============================================================================================")
+      print ("Attention: Edit the KPOINTS file, inserting the desired label in the k-points of the file.   ")
+      print ("               !!!! All k-points present in the KPOINTS file, must be labeled !!!!           ") 
+      print ("=============================================================================================")
+      print ("Example:                                                                                     ")
+      print ("         0.0 0.0 0.0 #1 (Gamma)                                                              ")
+      print ("         0.5 0.5 0.0 M                                                                       ")
+      print ("                                                                                             ")
+      print ("         0.5 0.5 0.0 M                                                                       ")
+      print ("         0.5 0.0 0.0 X                                                                       ")
+      print ("=============================================================================================")
+      print ("Use the following codes (#number) for using Greek symbols as labels:                         ") 
+      print ("                                                                                             ")
+      print ("#1  = Gamma       |  #2  = gamma        |  #3  = Delta     |  #4  = delta       |               ")
+      print ("#5  = Lambda      |  #6  = lambda       |  #7  = Sigma     |  #8  = sigma       |               ")
+      print ("#9  = Theta       |  #10 = tetha        |  #11 = Omega     |  #12 = omega       |               ")
+      print ("#13 = Psi         |  #14 = psi          |  #15 = Phi       |  #16 = phi         |  #17 = varphi ")
+      print ("#18 = alfa        |  #19 = beta         |  #20 = pi        |  #21 = rho         |               ")
+      print ("#22 = tau         |  #23 = upsilon      |  #24 = mu        |  #25 = nu          |               ")
+      print ("#26 = epsilon     |  #27 = eta          |  #28 = kappa     |  #29 = xi          |  #30 = zeta   ")
+      print ("#31 = left_arrow  |  #32 = right_arrow  |  #33 = up_arrow  |  #34 = down_arrow  |               ")
+      print ("=============================================================================================")
+      print ("After editing the KPOINTS file, press [ENTER] to continue                                    ")
+      print ("=============================================================================================")
+      confirmacao = input (" "); confirmacao = str(confirmacao)       
 
    #------------------------------------------
    kpoints = open(dir_files + '/KPOINTS', "r")
    #------------------------------------------
 
    VTemp = kpoints.readline()
    VTemp = kpoints.readline()
```

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/_nscf.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/_nscf.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/_var_kpoints.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/_var_kpoints.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/chgcar.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/chgcar.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,46 +301,27 @@
         for j in range (Grid_y):  
             for k in range (Grid_z):                          
                 indice = i + (j + k*Grid_y)*Grid_x
                 Vx[i] = Vx[i] + V_local[indice]*escala_x*fator
                 Vy[j] = Vy[j] + V_local[indice]*escala_y*fator
                 Vz[k] = Vz[k] + V_local[indice]*escala_z*fator
 
-
-
-
-
-
-
-
-
 if (plot_type == 1): 
 
    for i in range (passo1):
 
        if (i < (passo1-1)):
           for j in range(5):
               new_chgcar.write(f'{new_V_local[((i)*5) + j]} ')
        if (i == (passo1-1)):
           for j in range(passo2):
               new_chgcar.write(f'{new_V_local[((i)*5) + j]} ')
        new_chgcar.write(f' \n')
    new_chgcar.close()
 
-
-
-
-
-
-
-
-
-
-
-
 #=======================================================================
 # Saving data to plot the Charge =======================================
 #=======================================================================            
 
 #---------------------------------------------------------------------------------
 densidade = open(dir_files + '/output/Charge/Charge_X.dat', "w")
 #---------------------------------------------------------------------------------
```

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/contribuicao.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/contribuicao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/dielectric_function.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/dos_pdos_ldos.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/dos_pdos_ldos.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,131 +77,136 @@
 print ("##############################################################")
 print ("##################### Density of States: #####################")
 print ("##############################################################") 
 print (" ")
 
 if (escolha == -1):
 
-   print ("##############################################################") 
-   print ("Do you want to change the DOS|lDOS|pDOS color default?        ")
-   print ("[0] NOT                                                       ")
-   print ("[1] YES                                                       ")
-   print ("##############################################################") 
-   esc_color = input (" "); esc_color = int(esc_color)
-   print (" ")  
-
-   if (esc_color == 1):
-
-      print ("##############################################################")
-      print ("Color code:                                                   ")
-      print ("0  White   | 1  Black | 2  Red    | 3  Green  | 4  Blue       ")
-      print ("5  Yellow  | 6  Borwn | 7  Grey   | 8  Violet | 9  Cyan       ")
-      print ("10 Magenta |11 Orange | 12 Indigo | 13 Maroon | 14 Turquesa   ")
-      print ("15 Dark_Green                                                 ")
-      print ("##############################################################")       
-      print ("VASProcar color pattern:                                      ")
-      print ("                                                              ")
-      print ("total_DOS|lDOS:  7 13  (Grey, Maroon)                         ")
-      print ("--------------------------------------------------------------") 
-      print ("pdOS S|P|D|F:  4 2 3 10 (Blue, Red, Green, Magenta)           ")
-      print ("--------------------------------------------------------------")      
-      print ("pdOS Px|Py|Pz: 4 2 3    (Blue, Red, Green)                    ")
-      print ("--------------------------------------------------------------") 
-      print ("pdOS Dxy|Dyz|Dz2|Dxz|Dx2: 4 2 3 10 9                          ")
-      print ("(Blue, Red, Green, Magenta, Cyan)                             ")
-      print ("--------------------------------------------------------------")
-      if (n_orb == 16): 
-         print ("pdOS Fyx2|Fxyz|Fyz2|Fzz2|Fxz2|Fzx2|Fxx2: 4 2 3 10 9 5 11      ")
-         print ("(Blue, Red, Green, Magenta, Cyan, Yellow, Orange)             ")
+   if (len(inputs) == 0):
       print ("##############################################################") 
-      print (" ")
+      print ("Do you want to change the DOS|lDOS|pDOS color default?        ")
+      print ("[0] NOT                                                       ")
+      print ("[1] YES                                                       ")
+      print ("##############################################################") 
+      esc_color = input (" "); esc_color = int(esc_color)
+      print (" ")  
 
-      print ("==============================================================") 
-      print ("Enter in sequence the colors of total_DOS and lDOS:           ")
-      cor_orb = input ("Colors_DOS|lDOS: ")
-      #---------------------
-      tcor = cor_orb.split()
-      c_DOS = int(tcor[0]); c_lDOS = int(tcor[1])
-      #---------------------
-      print (" ")
+   if (esc_color == 1):
 
-      print ("==============================================================") 
-      print ("Type in sequence the colors of pDOS S|P|D|F:                  ")
-      cor_orb = input ("Colors_of_Orbitals: ")
-      #---------------------
-      tcor = cor_orb.split()
-      c_S = int(tcor[0]); c_P = int(tcor[1]); c_D = int(tcor[2]); c_F = int(tcor[3])
-      #---------------------
-      print (" ")
-      
-      if (n_orb >= 9):
+      if (len(inputs) == 0):
+         print ("##############################################################")
+         print ("Color code:                                                   ")
+         print ("0  White   | 1  Black | 2  Red    | 3  Green  | 4  Blue       ")
+         print ("5  Yellow  | 6  Borwn | 7  Grey   | 8  Violet | 9  Cyan       ")
+         print ("10 Magenta |11 Orange | 12 Indigo | 13 Maroon | 14 Turquesa   ")
+         print ("15 Dark_Green                                                 ")
+         print ("##############################################################")       
+         print ("VASProcar color pattern:                                      ")
+         print ("                                                              ")
+         print ("total_DOS|lDOS:  7 13  (Grey, Maroon)                         ")
+         print ("--------------------------------------------------------------") 
+         print ("pdOS S|P|D|F:  4 2 3 10 (Blue, Red, Green, Magenta)           ")
+         print ("--------------------------------------------------------------")      
+         print ("pdOS Px|Py|Pz: 4 2 3    (Blue, Red, Green)                    ")
+         print ("--------------------------------------------------------------") 
+         print ("pdOS Dxy|Dyz|Dz2|Dxz|Dx2: 4 2 3 10 9                          ")
+         print ("(Blue, Red, Green, Magenta, Cyan)                             ")
+         print ("--------------------------------------------------------------") 
+         if (n_orb == 16): 
+            print ("pdOS Fyx2|Fxyz|Fyz2|Fzz2|Fxz2|Fzx2|Fxx2: 4 2 3 10 9 5 11      ")
+            print ("(Blue, Red, Green, Magenta, Cyan, Yellow, Orange)             ")
+         print ("##############################################################") 
+         print (" ")
 
          print ("==============================================================") 
-         print ("Type in sequence the colors of pDOS Px|Py|Pzs                 ")
-         cor_orb = input ("Colors_of_Orbitals: ")
+         print ("Enter in sequence the colors of total_DOS and lDOS:           ")
+         cor_orb = input ("Colors_DOS|lDOS: ")
          #---------------------
          tcor = cor_orb.split()
-         c_Px = int(tcor[0]); c_Py = int(tcor[1]); c_Pz = int(tcor[2])
+         c_DOS = int(tcor[0]); c_lDOS = int(tcor[1])
          #---------------------
          print (" ")
-         
+
          print ("==============================================================") 
-         print ("Type in sequence the colors of pDOS Dxy|Dyz|Dz2|Dxz|Dx2:      ")
+         print ("Type in sequence the colors of pDOS S|P|D|F:                  ")
          cor_orb = input ("Colors_of_Orbitals: ")
          #---------------------
          tcor = cor_orb.split()
-         c_Dxy = int(tcor[0]); c_Dyz = int(tcor[1]); c_Dz2 = int(tcor[2]); c_Dxz = int(tcor[3]); c_Dx2 = int(tcor[4])
+         c_S = int(tcor[0]); c_P = int(tcor[1]); c_D = int(tcor[2]); c_F = int(tcor[3])
          #---------------------
          print (" ")
+      
+         if (n_orb >= 9):
 
-         if (n_orb == 16):
-            print ("=============================================================================") 
-            print ("Type in sequence the colors of pDOS Fyx2|Fxyz|Fyz2|Fzz2|Fxz2|Fzx2|Fxx2:      ")
+            print ("==============================================================") 
+            print ("Type in sequence the colors of pDOS Px|Py|Pzs                 ")
+            cor_orb = input ("Colors_of_Orbitals: ")
+            #---------------------
+            tcor = cor_orb.split()
+            c_Px = int(tcor[0]); c_Py = int(tcor[1]); c_Pz = int(tcor[2])
+            #---------------------
+            print (" ")
+         
+            print ("==============================================================") 
+            print ("Type in sequence the colors of pDOS Dxy|Dyz|Dz2|Dxz|Dx2:      ")
             cor_orb = input ("Colors_of_Orbitals: ")
             #---------------------
             tcor = cor_orb.split()
-            c_Fyx2 = int(tcor[0]); c_Fxyz = int(tcor[1]); c_Fyz2 = int(tcor[2]); c_Fzz2 = int(tcor[3])
-            c_Fxz2 = int(tcor[4]); c_Fzx2 = int(tcor[5]); c_Fxx2 = int(tcor[6])
+            c_Dxy = int(tcor[0]); c_Dyz = int(tcor[1]); c_Dz2 = int(tcor[2]); c_Dxz = int(tcor[3]); c_Dx2 = int(tcor[4])
             #---------------------
-            print (" ")   
+            print (" ")
 
-   print ("##############################################################") 
-   print ("with respect to energy, would you like? ======================")
-   print ("[0] Use the default energy value from DFT output =============")
-   print ("[1] Shift the Fermi level to 0.0 eV  =========================")
-   print ("##############################################################")
-   esc_fermi = input (" "); esc_fermi = int(esc_fermi)
-   print (" ")    
-
-   print ("##############################################################")
-   print ("What do you want to Plot/Analyze? ============================")
-   print ("[0] to analyze all ions in the lattice =======================")
-   print ("[1] to analyze selected ions =================================")
-   print ("##############################################################")
-   esc = input (" "); esc = int(esc)
-   print(" ")
+            if (n_orb == 16):
+               print ("=============================================================================") 
+               print ("Type in sequence the colors of pDOS Fyx2|Fxyz|Fyz2|Fzz2|Fxz2|Fzx2|Fxx2:      ")
+               cor_orb = input ("Colors_of_Orbitals: ")
+               #---------------------
+               tcor = cor_orb.split()
+               c_Fyx2 = int(tcor[0]); c_Fxyz = int(tcor[1]); c_Fyz2 = int(tcor[2]); c_Fzz2 = int(tcor[3])
+               c_Fxz2 = int(tcor[4]); c_Fzx2 = int(tcor[5]); c_Fxx2 = int(tcor[6])
+               #---------------------
+               print (" ")   
+
+   if (len(inputs) == 0):
+      print ("##############################################################") 
+      print ("with respect to energy, would you like? ======================") 
+      print ("[0] Use the default energy value from DFT output =============")
+      print ("[1] Shift the Fermi level to 0.0 eV  =========================")
+      print ("##############################################################")
+      esc_fermi = input (" "); esc_fermi = int(esc_fermi)
+      print (" ")    
+
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("What do you want to Plot/Analyze? ============================")
+      print ("[0] to analyze all ions in the lattice =======================")
+      print ("[1] to analyze selected ions =================================")
+      print ("##############################################################")
+      esc = input (" "); esc = int(esc)
+      print(" ")
 
    if (esc == 1):
 
       #-------------------------
       sim_nao = ["nao"]*(ni + 1)
       #-------------------------
 
-      print ("##############################################################")
-      print ("Choose the ranges of ions to be analyzed: =================== ")
-      print ("Type as in the examples below =============================== ")
-      print ("--------------------------------------------------------------")
-      print ("The order in which ions are added does not change the result. ")
-      print ("--------------------------------------------------------------")
-      print ("ranges_of_ions: 1:5 7:7 11* 15:27                             ")          
-      print ("ranges_of_ions: 7:49 50:53                                    ")
-      print ("ranges_of_ions: 3* 8* 16:21                                   ")
-      print ("##############################################################")
-      ion_range = input ("ranges_of_ions: ")
-      print (" ")
+      if (len(inputs) == 0):
+         print ("##############################################################")
+         print ("Choose the ranges of ions to be analyzed: =================== ")
+         print ("Type as in the examples below =============================== ")
+         print ("--------------------------------------------------------------")
+         print ("The order in which ions are added does not change the result. ")
+         print ("--------------------------------------------------------------")
+         print ("ranges_of_ions: 1:5 7:7 11* 15:27                             ")          
+         print ("ranges_of_ions: 7:49 50:53                                    ")
+         print ("ranges_of_ions: 3* 8* 16:21                                   ")
+         print ("##############################################################")
+         ion_range = input ("ranges_of_ions: ")
+         print (" ")
       #---------------------------------------------------------------------------------------
       selected_ions = ion_range.replace(':', ' ').replace('-', ' ').replace('*', ' *').split()
       loop = int(len(selected_ions)/2)
       #---------------------------------------------------------------------------------------
       
       for i in range (1,(loop+1)):
           #------------------------------------------------------
@@ -519,13 +524,15 @@
 print("= Edit the DOS Plot through the DOS_pDOS_lDOS.py or .agr =======")
 print("= (via Grace) files generated in the output/DOS folder =========")   
 print("================================================================")
 
 #-----------------------------------------------------------------
 print(" ")
 print("======================= Completed =======================")
+print(" ")
 #-----------------------------------------------------------------
 
 #=======================================================================
 # User option to perform another calculation or finished the code ======
 #=======================================================================
-execute_python_file(filename = '_loop.py')
+if (len(inputs) == 0):
+   execute_python_file(filename = '_loop.py')
```

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py`

 * *Files 4% similar despite different names*

```diff
@@ -58,130 +58,136 @@
 print ("##############################################################")
 print ("############# Density of States (Polarized Spin) #############")
 print ("##############################################################") 
 print (" ")
 
 if (escolha == -1):
 
-   print ("##############################################################") 
-   print ("Do you want to change the DOS|lDOS|pDOS color default?        ")
-   print ("[0] NOT                                                       ")
-   print ("[1] YES                                                       ")
-   print ("##############################################################") 
-   esc_color = input (" "); esc_color = int(esc_color)
-   print (" ")  
-
-   if (esc_color == 1):
-      print ("##############################################################")
-      print ("Color code:                                                   ")
-      print ("0  White   | 1  Black | 2  Red    | 3  Green  | 4  Blue       ")
-      print ("5  Yellow  | 6  Borwn | 7  Grey   | 8  Violet | 9  Cyan       ")
-      print ("10 Magenta |11 Orange | 12 Indigo | 13 Maroon | 14 Turquesa   ")
-      print ("15 Dark_Green                                                 ")
-      print ("##############################################################")       
-      print ("VASProcar color pattern:                                      ")
-      print ("                                                              ")
-      print ("total_DOS|lDOS:  7 13  (Grey, Maroon)                         ")
-      print ("--------------------------------------------------------------")  
-      print ("pdOS S|P|D|F:  4 2 3 10 (Blue, Red, Green, Magenta)           ")
-      print ("--------------------------------------------------------------")      
-      print ("pDOS Px|Py|Pz:  4 2 3  (Blue, Red, Green)                     ")
-      print ("--------------------------------------------------------------") 
-      print ("pDOS Dxy|Dyz|Dz2|Dxz|Dx2: 4 2 3 10 9                          ")
-      print ("(Blue, Red, Green, Magenta, Cyan)                             ")
-      print ("--------------------------------------------------------------")
-      if (n_orb == 16): 
-         print ("pDOS Fyx2|Fxyz|Fyz2|Fzz2|Fxz2|Fzx2|Fxx2: 4 2 3 10 9 5 11      ")
-         print ("(Blue, Red, Green, Magenta, Cyan, Yellow, Orange)             ")
+   if (len(inputs) == 0):
       print ("##############################################################") 
-      print (" ")
+      print ("Do you want to change the DOS|lDOS|pDOS color default?        ")
+      print ("[0] NOT                                                       ")
+      print ("[1] YES                                                       ")
+      print ("##############################################################") 
+      esc_color = input (" "); esc_color = int(esc_color)
+      print (" ")  
 
-      print ("==============================================================") 
-      print ("Enter in sequence the colors of total_DOS and lDOS:           ")
-      cor_orb = input ("Colors_DOS|lDOS: ")
-      #---------------------
-      tcor = cor_orb.split()
-      c_DOS = int(tcor[0]); c_lDOS = int(tcor[1])
-      #---------------------
-      print (" ")
+   if (esc_color == 1):
 
-      print ("==============================================================") 
-      print ("Enter in sequence the colors of pdOS S|P|D:                   ")
-      cor_orb = input ("Colors_pdOS_S|P|D: ")
-      #---------------------
-      tcor = cor_orb.split()
-      c_S = int(tcor[0]); c_P = int(tcor[1]); c_D = int(tcor[2])
-      #---------------------
-      print (" ")
-      
-      if (n_orb >= 9):
+      if (len(inputs) == 0):
+         print ("##############################################################")
+         print ("Color code:                                                   ")
+         print ("0  White   | 1  Black | 2  Red    | 3  Green  | 4  Blue       ")
+         print ("5  Yellow  | 6  Borwn | 7  Grey   | 8  Violet | 9  Cyan       ")
+         print ("10 Magenta |11 Orange | 12 Indigo | 13 Maroon | 14 Turquesa   ")
+         print ("15 Dark_Green                                                 ")
+         print ("##############################################################")       
+         print ("VASProcar color pattern:                                      ")
+         print ("                                                              ")
+         print ("total_DOS|lDOS:  7 13  (Grey, Maroon)                         ")
+         print ("--------------------------------------------------------------") 
+         print ("pdOS S|P|D|F:  4 2 3 10 (Blue, Red, Green, Magenta)           ")
+         print ("--------------------------------------------------------------")      
+         print ("pdOS Px|Py|Pz: 4 2 3    (Blue, Red, Green)                    ")
+         print ("--------------------------------------------------------------") 
+         print ("pdOS Dxy|Dyz|Dz2|Dxz|Dx2: 4 2 3 10 9                          ")
+         print ("(Blue, Red, Green, Magenta, Cyan)                             ")
+         print ("--------------------------------------------------------------") 
+         if (n_orb == 16): 
+            print ("pdOS Fyx2|Fxyz|Fyz2|Fzz2|Fxz2|Fzx2|Fxx2: 4 2 3 10 9 5 11      ")
+            print ("(Blue, Red, Green, Magenta, Cyan, Yellow, Orange)             ")
+         print ("##############################################################") 
+         print (" ")
 
          print ("==============================================================") 
-         print ("Enter in sequence the colors of pdOS Px|Py|Pz:                ")
-         cor_orb = input ("Colors_pdOS_Px|Py|Pz: ")
+         print ("Enter in sequence the colors of total_DOS and lDOS:           ")
+         cor_orb = input ("Colors_DOS|lDOS: ")
          #---------------------
          tcor = cor_orb.split()
-         c_Px = int(tcor[0]); c_Py = int(tcor[1]); c_Pz = int(tcor[2])
+         c_DOS = int(tcor[0]); c_lDOS = int(tcor[1])
          #---------------------
          print (" ")
-         
+
          print ("==============================================================") 
-         print ("Enter in sequence the colors of pDOS Dxy|Dyz|Dz2|Dxz|Dx2:     ")
-         cor_orb = input ("Colors_pDOS_Dxy|Dyz|Dz2|Dxz|Dx2: ")
+         print ("Type in sequence the colors of pDOS S|P|D|F:                  ")
+         cor_orb = input ("Colors_of_Orbitals: ")
          #---------------------
          tcor = cor_orb.split()
-         c_Dxy = int(tcor[0]); c_Dyz = int(tcor[1]); c_Dz2 = int(tcor[2]); c_Dxz = int(tcor[3]); c_Dx2 = int(tcor[4])
+         c_S = int(tcor[0]); c_P = int(tcor[1]); c_D = int(tcor[2]); c_F = int(tcor[3])
          #---------------------
          print (" ")
+      
+         if (n_orb >= 9):
 
-         if (n_orb == 16):
-            print ("=============================================================================") 
-            print ("Enter in sequence the colors of pDOS Fyx2|Fxyz|Fyz2|Fzz2|Fxz2|Fzx2|Fxx2:     ")
-            cor_orb = input ("Colors_dos_Orbitais: ")
+            print ("==============================================================") 
+            print ("Type in sequence the colors of pDOS Px|Py|Pzs                 ")
+            cor_orb = input ("Colors_of_Orbitals: ")
             #---------------------
             tcor = cor_orb.split()
-            c_Fyx2 = int(tcor[0]); c_Fxyz = int(tcor[1]); c_Fyz2 = int(tcor[2]); c_Fzz2 = int(tcor[3])
-            c_Fxz2 = int(tcor[4]); c_Fzx2 = int(tcor[5]); c_Fxx2 = int(tcor[6])
+            c_Px = int(tcor[0]); c_Py = int(tcor[1]); c_Pz = int(tcor[2])
+            #---------------------
+            print (" ")
+         
+            print ("==============================================================") 
+            print ("Type in sequence the colors of pDOS Dxy|Dyz|Dz2|Dxz|Dx2:      ")
+            cor_orb = input ("Colors_of_Orbitals: ")
             #---------------------
-            print (" ")     
+            tcor = cor_orb.split()
+            c_Dxy = int(tcor[0]); c_Dyz = int(tcor[1]); c_Dz2 = int(tcor[2]); c_Dxz = int(tcor[3]); c_Dx2 = int(tcor[4])
+            #---------------------
+            print (" ")
 
-   print ("##############################################################") 
-   print ("with respect to energy, would you like? ======================")
-   print ("[0] Use the default energy value from DFT output =============")
-   print ("[1] Shift the Fermi level to 0.0 eV  =========================")
-   print ("##############################################################") 
-   esc_fermi = input (" "); esc_fermi = int(esc_fermi)
-   print (" ")    
-
-   print ("##############################################################")
-   print ("What do you want to Plot/Analyze? ============================")
-   print ("[0] to analyze all ions in the lattice =======================")
-   print ("[1] to analyze selected ions =================================")
-   print ("##############################################################")
-   esc = input (" "); esc = int(esc)
-   print(" ")
+            if (n_orb == 16):
+               print ("=============================================================================") 
+               print ("Type in sequence the colors of pDOS Fyx2|Fxyz|Fyz2|Fzz2|Fxz2|Fzx2|Fxx2:      ")
+               cor_orb = input ("Colors_of_Orbitals: ")
+               #---------------------
+               tcor = cor_orb.split()
+               c_Fyx2 = int(tcor[0]); c_Fxyz = int(tcor[1]); c_Fyz2 = int(tcor[2]); c_Fzz2 = int(tcor[3])
+               c_Fxz2 = int(tcor[4]); c_Fzx2 = int(tcor[5]); c_Fxx2 = int(tcor[6])
+               #---------------------
+               print (" ")   
+
+   if (len(inputs) == 0):
+      print ("##############################################################") 
+      print ("with respect to energy, would you like? ======================") 
+      print ("[0] Use the default energy value from DFT output =============")
+      print ("[1] Shift the Fermi level to 0.0 eV  =========================")
+      print ("##############################################################")
+      esc_fermi = input (" "); esc_fermi = int(esc_fermi)
+      print (" ")    
+
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("What do you want to Plot/Analyze? ============================")
+      print ("[0] to analyze all ions in the lattice =======================")
+      print ("[1] to analyze selected ions =================================")
+      print ("##############################################################")
+      esc = input (" "); esc = int(esc)
+      print(" ")
 
    if (esc == 1):
-      
+
       #-------------------------
       sim_nao = ["nao"]*(ni + 1)
       #-------------------------
 
-      print ("##############################################################")
-      print ("Choose the ranges of ions to be analyzed: =================== ")
-      print ("Type as in the examples below =============================== ")
-      print ("--------------------------------------------------------------")
-      print ("The order in which ions are added does not change the result. ")
-      print ("--------------------------------------------------------------")
-      print ("ranges_of_ions: 1:5 7:7 11* 15:27                             ")          
-      print ("ranges_of_ions: 7:49 50:53                                    ")
-      print ("ranges_of_ions: 3* 8* 16:21                                   ")
-      print ("##############################################################")
-      ion_range = input ("ranges_of_ions: ")
-      print (" ")
+      if (len(inputs) == 0):
+         print ("##############################################################")
+         print ("Choose the ranges of ions to be analyzed: =================== ")
+         print ("Type as in the examples below =============================== ")
+         print ("--------------------------------------------------------------")
+         print ("The order in which ions are added does not change the result. ")
+         print ("--------------------------------------------------------------")
+         print ("ranges_of_ions: 1:5 7:7 11* 15:27                             ")          
+         print ("ranges_of_ions: 7:49 50:53                                    ")
+         print ("ranges_of_ions: 3* 8* 16:21                                   ")
+         print ("##############################################################")
+         ion_range = input ("ranges_of_ions: ")
+         print (" ")
       #---------------------------------------------------------------------------------------
       selected_ions = ion_range.replace(':', ' ').replace('-', ' ').replace('*', ' *').split()
       loop = int(len(selected_ions)/2)
       #---------------------------------------------------------------------------------------
       
       for i in range (1,(loop+1)):
           #------------------------------------------------------
@@ -539,13 +545,15 @@
 print("= Edit the DOS Plot through the DOS_pDOS_lDOS.py or .agr =======")
 print("= (via Grace) files generated in the output/DOS folder =========")   
 print("================================================================")
 
 #-----------------------------------------------------------------
 print(" ")
 print("======================= Completed =======================")
+print(" ")
 #-----------------------------------------------------------------
 
 #=======================================================================
 # User option to perform another calculation or finished the code ======
 #=======================================================================
-execute_python_file(filename = '_loop.py')
+if (len(inputs) == 0):
+   execute_python_file(filename = '_loop.py')
```

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/kpoints_2D_3D.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/kpoints_2D_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/parchg.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/parchg.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/poscar_replace.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/poscar_replace.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/potencial.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/potencial.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_VASP/wave_function.py` & `vasprocar-1.1.15.7/vasprocar/src/_VASP/wave_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_loop.py` & `vasprocar-1.1.15.7/vasprocar/src/_loop.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_settings.py` & `vasprocar-1.1.15.7/vasprocar/src/_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def execute_python_file(filename: str):
     return exec(open(main_dir + str(filename)).read(), globals())
 
 # set GRACE variables
 execute_python_file(filename = "plot/_plot_settings.py")
 
 #------------------------------------------------ ------------------------------
-# Regarding the network parameter, choose: -------------------------------------
+# Regarding the lattice parameter, choose: -------------------------------------
 #------------------------------------------------ ------------------------------
 # [1] Use the parameter informed in the CONTCAR (VASP) or nscf.out (QE) file
 # [2] Adopt as a parameter the smallest value among the modules of the primitive
 #     vectors of the crystal lattice (A1, A2 and A3).
 #------------------------------------------------ ------------------------------
 param_estim = 1
 
@@ -25,136 +25,147 @@
     os.mkdir(dir_files + '/output')
 # ---------------------------------
 
 # ----------------------------------------------------------------------
 # Obtaining the code input parameters: ---------------------------------
 # ----------------------------------------------------------------------
 
-print("##############################################################")
-print("################ What do you want to Analyze? ################")
-print("##############################################################")
-print("## ======================================================== ##")
-print("## [1] Energy: 2D|3D|isosurface Plot, Fermi Surfaces,       ##")
-print("##             Contour levels                               ##")
-print("## ======================================================== ##")  
-print("## [2] Spin: 2D|3D|isosurface Plot,                         ##")
-print("##           Projection on Contour levels                   ##")
-print("## ======================================================== ##") 
-print("## [3] Projection Orbital and Spacial of the states,        ##")
-print("##     Density of States (DOS, p-DOs, l-DOS),               ##")
-print("##     Projection of Character of the states                ##")
-print("## ======================================================== ##") 
-print("## [4] Charge Density, Electrostatic Potential,             ##")
-print("##     Dielectric Function                                  ##")
-print("## ======================================================== ##")
-print("## [555] Generate KPOINTS file (2D Plane or 3D Mesh in ZB)  ##")
-print("## ======================================================== ##")
-print("## [665] POSCAR - Ion substitution in the lattice           ##")
-print("## ======================================================== ##")
-print("## [777] Tip: Using Multiple PROCAR Files                   ##")
-print("## ======================================================== ##")
-print("## [888] Check and fix VASP output files                    ##")
-print("## ======================================================== ##")
-print("## [999] Install/Update Python modules                      ##")
-print("## ======================================================== ##")
-print("##############################################################")
-opcao = input(" "); opcao = int(opcao)
-print(" ")
+if (len(inputs) == 0):
 
-# ======================================================================
-
-if (opcao > -10 and opcao < 10):
    print("##############################################################")
-   print("####################### Choose option: #######################")
+   print("################ What do you want to Analyze? ################")
    print("##############################################################")
-
-if (opcao == 1 or opcao == -1):
-   print("## ======================================================== ##")
-   print("## Band Structure - 2D Plot:  [k-path, E(eV)]               ##")
-   print("## [10] Default   --   [-10] Custom                         ##")
    print("## ======================================================== ##")
-   print("## Fermi surface - 2D projection:  [ki, kj, E(eV)]          ##")
-   print("## [11] Default   --   [-11] Custom                         ##")
+   print("## [1] Energy: 2D|3D|isosurface Plot, Fermi Surfaces,       ##")
+   print("##             Contour levels                               ##")
+   print("## ======================================================== ##")  
+   print("## [2] Spin: 2D|3D|isosurface Plot,                         ##")
+   print("##           Projection on Contour levels                   ##")
+   print("## ======================================================== ##") 
+   print("## [3] Projection Orbital and Spacial of the states,        ##")
+   print("##     Density of States (DOS, p-DOs, l-DOS),               ##")
+   print("##     Projection of Character of the states                ##")
+   print("## ======================================================== ##") 
+   print("## [4] Charge Density, Electrostatic Potential,             ##")
+   print("##     Dielectric Function                                  ##")
    print("## ======================================================== ##")
-   print("## Band Contour levels (2D Projection and 3D Plot):         ##")
-   print("## [12] Default   --   [-12] Custom                         ##")
+   print("## [5] Creation, correction and manipulation of VASP output ##")
+   print("##     files: KPOINTS|POSCAR|POTCAR|PROCAR|OUTCAR|CHGCAR    ##")
    print("## ======================================================== ##")
-   print("## Band Structure - 3D Plot: [ki, kj, E(eV)]                ##")
-   print("## [13] Default   --   [-13] Custom                         ##")
+   print("## [6] Input files (code automation)                        ##")
    print("## ======================================================== ##")
-   print("## Band isosurfaces:  [kx, ky, kz, E(eV) or dE(eV)]         ##")
-   print("## [14] Default   --   [-14] Custom                         ##")
+   print("## [999] Install/Update Python modules                      ##")
    print("## ======================================================== ##")
    print("##############################################################")
    opcao = input(" "); opcao = int(opcao)
    print(" ")
 
-if (opcao == 2 or opcao == -2):
-   print("## ======================================================== ##")
-   print("## 2D Projection of Components Sx|Sy|Sz:  [k-path, E(eV)]   ##")
-   print("## [20] Default   --   [-20] Custom                         ##")
-   print("## ======================================================== ##")
-   print("## Projections 2D|3D|Isosurface of Components Sx|Sy|Sz      ##")
-   print("## and of the vectors SiSj e SxSySz                         ##")
-   print("## [21] Default   --   [-21] Custom                         ##")
-   print("## ======================================================== ##")
-   print("## Plot of Components Sx|Sy|Sz and of the vectors SiSj      ##")
-   print("## along a given Band and Contour level (constant energy)   ##")
-   print("## [22] Default   --   [-22] Custom                         ##")
-   print("## ======================================================== ##")
-   print("## Video showing the evolution of Sx|Sy|Sz or SiSj vectors  ##")
-   print("## as a function of Energy (Contour level)                  ##")
-   print("## [23] Default   --   [-23] Custom                         ##")
-   print("## ======================================================== ##")
-   print("##############################################################")   
-   opcao = input(" "); opcao = int(opcao)
-   print(" ")
+   # ======================================================================
+
+   if (opcao > -10 and opcao < 10):
+      print("##############################################################")
+      print("####################### Choose option: #######################")
+      print("##############################################################")
+
+   if (opcao == 1 or opcao == -1):
+      print("## ======================================================== ##")
+      print("## Band Structure - 2D Plot:  [k-path, E(eV)]               ##")
+      print("## [10] Default   --   [-10] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## Fermi surface - 2D projection:  [ki, kj, E(eV)]          ##")
+      print("## [11] Default   --   [-11] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## Band Contour levels (2D Projection and 3D Plot):         ##")
+      print("## [12] Default   --   [-12] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## Band Structure - 3D Plot: [ki, kj, E(eV)]                ##")
+      print("## [13] Default   --   [-13] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## Band isosurfaces:  [kx, ky, kz, E(eV) or dE(eV)]         ##")
+      print("## [14] Default   --   [-14] Custom                         ##")
+      print("## ======================================================== ##")
+      print("##############################################################")
+      opcao = input(" "); opcao = int(opcao)
+      print(" ")
+
+   if (opcao == 2 or opcao == -2):
+      print("## ======================================================== ##")
+      print("## 2D Projection of Components Sx|Sy|Sz:  [k-path, E(eV)]   ##")
+      print("## [20] Default   --   [-20] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## Projections 2D|3D|Isosurface of Components Sx|Sy|Sz      ##")
+      print("## and of the vectors SiSj e SxSySz                         ##")
+      print("## [21] Default   --   [-21] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## Plot of Components Sx|Sy|Sz and of the vectors SiSj      ##")
+      print("## along a given Band and Contour level (constant energy)   ##")
+      print("## [22] Default   --   [-22] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## Video showing the evolution of Sx|Sy|Sz or SiSj vectors  ##")
+      print("## as a function of Energy (Contour level)                  ##")
+      print("## [23] Default   --   [-23] Custom                         ##")
+      print("## ======================================================== ##")
+      print("##############################################################")   
+      opcao = input(" "); opcao = int(opcao)
+      print(" ")
    
-if (opcao == 3 or opcao == -3):
-   print("## ======================================================== ##")
-   print("## 2D Projection of Orbitals S|P|D|F:  [k-path, E(eV)]      ##")       
-   print("## [30] Default   --   [-30] Custom                         ##")
-   print("## ======================================================== ##")
-   print("## DOS, p-DOS e l-DOS (Plot 2D)                             ##")
-   print("## [31] Default   --   [-31] Custom                         ##")
-   print("## ======================================================== ##")
-   print("## 2D projection of the spatial location of bands (regions) ##")
-   print("## [32] Default   --   [-32] Custom                         ##")
-   print("## ======================================================== ##")
-   print("## 2D projection of states Character:                       ##")
-   print("## [33] Default   --   [-33] Custom                         ##")
-   print("## ======================================================== ##")
-   print("## Contribution of Orbitals and ions on states: (Table)     ##")
-   print("## [34] Default   --   [-34] Custom                         ##")
-   print("## ======================================================== ##")
-   print("##############################################################") 
-   opcao = input(" "); opcao = int(opcao)
-   print(" ")
+   if (opcao == 3 or opcao == -3):
+      print("## ======================================================== ##")
+      print("## 2D Projection of Orbitals S|P|D|F:  [k-path, E(eV)]      ##")       
+      print("## [30] Default   --   [-30] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## DOS, p-DOS e l-DOS (Plot 2D)                             ##")
+      print("## [31] Default   --   [-31] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## 2D projection of the spatial location of bands (regions) ##")
+      print("## [32] Default   --   [-32] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## 2D projection of states Character:                       ##")
+      print("## [33] Default   --   [-33] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## Contribution of Orbitals and ions on states: (Table)     ##")
+      print("## [34] Default   --   [-34] Custom                         ##")
+      print("## ======================================================== ##")
+      print("##############################################################") 
+      opcao = input(" "); opcao = int(opcao)
+      print(" ")
    
-if (opcao == 4 or opcao == -4):
-   print("## ======================================================== ##")
-   print("## Electrostatic Potential in X,Y,Z direction - 2D Plot     ##")
-   print("## [40] Default   --   [-40] Custom                         ##")
-   print("## ======================================================== ##") 
-   print("## Charge Density in X,Y,Z direction - 2D Plot              ##")
-   print("## [41] Default   --   [-41] Custom                         ##")
-   print("## ======================================================== ##")
-   print("## Partial Charge Density in X,Y,Z direction - 2D Plot      ##")
-   print("## [42] Default   --   [-42] Custom                         ##")
-   print("## ======================================================== ##")
-   print("## Dielectric Function in X,Y,Z (Real|Imaginary) - 2D Plot  ##")
-   print("## [43] Default   --   [-43] Custom                         ##")
-   print("## ======================================================== ##")
-   # print("##         !!!!! UNDER TESTS - Non-Functional !!!!!         ##")
-   # print("## Wave Function in X,Y,Z (Real and Imaginary) - 2D Plot    ##")
-   # print("## [44] Default   --   [-44] Custom                         ##")
-   # print("## ======================================================== ##")
-   print("##############################################################")
-   opcao = input(" "); opcao = int(opcao)
-   print(" ")
+   if (opcao == 4 or opcao == -4):
+      print("## ======================================================== ##")
+      print("## Electrostatic Potential in X,Y,Z direction - 2D Plot     ##")
+      print("## [40] Default   --   [-40] Custom                         ##")
+      print("## ======================================================== ##") 
+      print("## Charge Density in X,Y,Z direction - 2D Plot              ##")
+      print("## [41] Default   --   [-41] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## Partial Charge Density in X,Y,Z direction - 2D Plot      ##")
+      print("## [42] Default   --   [-42] Custom                         ##")
+      print("## ======================================================== ##")
+      print("## Dielectric Function in X,Y,Z (Real|Imaginary) - 2D Plot  ##")
+      print("## [43] Default   --   [-43] Custom                         ##")
+      print("## ======================================================== ##")
+      # print("##         !!!!! UNDER TESTS - Non-Functional !!!!!         ##")
+      # print("## Wave Function in X,Y,Z (Real and Imaginary) - 2D Plot    ##")
+      # print("## [44] Default   --   [-44] Custom                         ##")
+      # print("## ======================================================== ##")
+      print("##############################################################")
+      opcao = input(" "); opcao = int(opcao)
+      print(" ")
+
+   if (opcao == 5 or opcao == -5):
+      print("## ======================================================== ##")
+      print("## [51] Generate KPOINTS file (2D Plane or 3D Mesh in ZB)   ##")
+      print("## [52] POSCAR - Ion substitution in the lattice            ##")
+      print("## [53] Combining/Merging different POTCAR files            ##")
+      print("## [54] Tip: Using Multiple PROCAR Files                    ##")
+      print("## [55] Check and fix VASP output files                     ##")
+      print("## ======================================================== ##")
+      print("##############################################################")
+      opcao = input(" "); opcao = int(opcao)
+      print(" ")
    
 # ----------------------------------------------------------------------
 # Copying file to "output" folder: -------------------------------------
 # ----------------------------------------------------------------------
 
 source = main_dir + '/etc/BibTeX.dat'
 destination = dir_files + '/output/BibTeX.dat'
@@ -164,15 +175,15 @@
 destination = dir_files + '/output/DOI.png'
 shutil.copyfile(source, destination)
 
 # ----------------------------------------------------------------------
 # Getting information from CONTCAR/OUTCAR/PROCAR files: ----------------
 # ----------------------------------------------------------------------
 
-if (opcao > -100 and opcao < 100 and opcao != 41 and opcao != -41):
+if (opcao > -100 and opcao < 100 and opcao != 41 and opcao != -41 and opcao != 52 and opcao != -52 and opcao != 53 and opcao != -53 and opcao != 6 and opcao != -6):
    execute_python_file(filename = DFT + '_info_b.py')
 
    print("#######################################################################")
    print("# Obtaining information from the lattice and the calculation performed:")
    print("#######################################################################")
 
    print(" ")
@@ -272,35 +283,41 @@
 
 if (opcao == 43 or opcao == -43):
    execute_python_file(filename = DFT + 'dielectric_function.py')
     
 # if (opcao == 44 or opcao == -44):
 #    execute_python_file(filename = DFT + 'wave_function.py')
 
-if (opcao == 555 or opcao == -555):
+if (opcao == 51 or opcao == -51):
    execute_python_file(filename = DFT + 'kpoints_2D_3D.py')
 
-if (opcao == 665 or opcao == -665):
+if (opcao == 52 or opcao == -52):
    execute_python_file(filename = DFT + 'poscar_replace.py')
 
-if (opcao == 777 or opcao == -777):
+if (opcao == 53 or opcao == -53):
+   execute_python_file(filename = DFT + 'postar_combination.py')
+
+if (opcao == 54 or opcao == -54):
    print("##############################################################")
    print("## ======================================================== ##")
    print("## ------------- Using Multiple PROCAR Files: ------------- ##")
    print("## ======================================================== ##")
    print("##                                                          ##")
    print("## For the use of Multiple PROCAR files, they must be       ##")
    print("## renamed sequentially, as below:                          ##")
    print("##                                                          ##")
    print("## PROCAR.1 PROCAR.2 PROCAR.3 PROCAR.4 PROCAR.5 ...         ##")
    print("##                                                          ##")
    print("## Note: All PROCAR files used must contain exactly the     ##") 
    print("##       same number of k-points                            ##")
    print("##############################################################")
    pausa = input (" ")
+   exit()
        
-if (opcao == 888 or opcao == -888):
+if (opcao == 55 or opcao == -55):
    execute_python_file(filename = 'correction_file.py')
 
+if (opcao == 6 or opcao == -6):
+   execute_python_file(filename = 'inputs/' + 'inputs_files.py')
+
 if (opcao == 999 or opcao == -999):
    execute_python_file(filename = '_update.py')
-
```

### Comparing `vasprocar-1.1.15.6/vasprocar/src/_update.py` & `vasprocar-1.1.15.7/vasprocar/src/_update.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/bandas_2D.py` & `vasprocar-1.1.15.7/vasprocar/src/bandas_2D.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,38 +25,40 @@
 print ("##############################################################")
 print ("##################### Band Structure Plot ####################")
 print ("##############################################################")
 print (" ")
 
 if (escolha == -1):
 
-   print ("##############################################################")
-   print ("Regarding the Plot of Bands, choose: =========================")
-   print ("[0] Plot all bands ===========================================")
-   print ("[1] Plot selected bands ======================================")
-   print ("##############################################################")
-   esc_bands = input (" "); esc_bands = int(esc_bands)
-   print(" ")
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Regarding the Plot of Bands, choose: =========================")
+      print ("[0] Plot all bands ===========================================")
+      print ("[1] Plot selected bands ======================================")
+      print ("##############################################################")
+      esc_bands = input (" "); esc_bands = int(esc_bands)
+      print(" ")
 
    if (esc_bands == 0):
       bands_range = '1:' + str(nb)
 
-   if (esc_bands == 1):     
-      print ("##############################################################")
-      print ("Choose the bands to be plotted through interval ============= ")
-      print ("Type as in the examples below =============================== ")
-      print ("------------------------------------------------------------- ")
-      print ("Bands can be added in any order ----------------------------- ")
-      print ("------------------------------------------------------------- ")
-      print ("bands_intervals  35:42                                        ")          
-      print ("bands_intervals  1:15 27:69 18:19 76*                         ")
-      print ("bands_intervals  7* 9* 11* 13*                                ")
-      print ("##############################################################")
-      bands_range = input ("bands_intervals  ")
-      print (" ")
+   if (esc_bands == 1):
+      if (len(inputs) == 0): 
+         print ("##############################################################")
+         print ("Choose the bands to be plotted through interval ============= ")
+         print ("Type as in the examples below =============================== ")
+         print ("------------------------------------------------------------- ")
+         print ("Bands can be added in any order ----------------------------- ")
+         print ("------------------------------------------------------------- ")
+         print ("bands_intervals  35:42                                        ")          
+         print ("bands_intervals  1:15 27:69 18:19 76*                         ")
+         print ("bands_intervals  7* 9* 11* 13*                                ")
+         print ("##############################################################")
+         bands_range = input ("bands_intervals  ")
+         print (" ")
       #------------------------------------------------------------------------------------------
       selected_bands = bands_range.replace(':', ' ').replace('-', ' ').replace('*', ' *').split()
       loop = int(len(selected_bands)/2)
       #------------------------------------------------------------------------------------------
 
       for i in range (1,(loop+1)):
           #--------------------------------------------------------
@@ -69,59 +71,64 @@
              print (" ")
              print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
              print ("ERROR: The values of the informed bands are incorrect %%%%")
              print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
              confirmation = input (" ")
              exit()
 
-   print ("##############################################################") 
-   print ("with respect to energy, would you like? ======================")
-   print ("[0] Use the default energy value from DFT output =============")
-   print ("[1] Shift the Fermi level to 0.0 eV  =========================")
-   print ("##############################################################")
-   esc_fermi = input (" "); esc_fermi = int(esc_fermi)
-   print (" ")   
-
-   print ("##############################################################") 
-   print ("Do you want to modify the energy range to be plotted? ========")
-   print ("[0] NOT                                                       ")
-   print ("[1] YES                                                       ")
-   print ("##############################################################")
-   esc_range_E = input (" "); esc_range_E = int(esc_range_E)
-   print (" ")
+   if (len(inputs) == 0):
+      print ("##############################################################") 
+      print ("with respect to energy, would you like? ======================")
+      print ("[0] Use the default energy value from DFT output =============")
+      print ("[1] Shift the Fermi level to 0.0 eV  =========================")
+      print ("##############################################################")
+      esc_fermi = input (" "); esc_fermi = int(esc_fermi)
+      print (" ")   
 
-   if (esc_range_E == 1):
+   if (len(inputs) == 0):
       print ("##############################################################") 
-      print ("Enter the energy range to be plotted: ========================")
-      print ("Note: Enter the lowest and highest energy value to be plotted ")
-      print ("      in relation to the Fermi Level                          ")
-      print ("Examples:                                                     ")
-      print ("--------------------------------------------------------------")
-      print ("E_min E_max: -3.0 15.0                                        ")
-      print ("E_min E_max: -5.1 5.0                                         ")
-      print ("##############################################################")      
-      range_E = input ("E_min E_max:  ")
+      print ("Do you want to modify the energy range to be plotted? ========")
+      print ("[0] NOT                                                       ")
+      print ("[1] YES                                                       ")
+      print ("##############################################################")
+      esc_range_E = input (" "); esc_range_E = int(esc_range_E)
       print (" ")
-      #--------------------------------------------------
+
+   if (esc_range_E == 1):
+      if (len(inputs) == 0):
+         print ("##############################################################") 
+         print ("Enter the energy range to be plotted: ========================")
+         print ("Note: Enter the lowest and highest energy value to be plotted ")
+         print ("      in relation to the Fermi Level                          ")
+         print ("Examples:                                                     ")
+         print ("--------------------------------------------------------------")
+         print ("E_min E_max: -3.0 15.0                                        ")
+         print ("E_min E_max: -5.1 5.0                                         ")
+         print ("##############################################################")      
+         range_E = input ("E_min E_max:  ")
+         print (" ")
+      #---------------------------------------------------------------------------------------
       selected_energ = range_E.replace('-', ' -').replace('+', ' +').replace(':', ' ').split()
+      #--------------------------------------------------------------------------------------- 
       E_min = float(selected_energ[0])
       E_max = float(selected_energ[1])
 
-   print ("##############################################################")
-   print ("Would you like to label the k-points?                         ")
-   print ("[0] DO NOT label the k-points  ===============================")
-   print ("[1] highlight k-points present in KPOINTS file ===============")
-   print ("[2] Customize: highlight and Label k-points   ================")
-   print ("##############################################################") 
-   dest_k = input (" "); dest_k = int(dest_k)
-   print (" ")
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Would you like to label the k-points?                         ")
+      print ("[0] DO NOT label the k-points  ===============================")
+      print ("[1] highlight k-points present in KPOINTS file ===============")
+      print ("[2] Customize: highlight and Label k-points   ================")
+      print ("##############################################################") 
+      dest_k = input (" "); dest_k = int(dest_k)
+      print (" ")
    #--------------
    l_symmetry = 0
    
-   if (DFT == '_QE/' and dest_k == 2):
+   if (DFT == '_QE/' and dest_k == 2 and len(inputs) == 0 ):
       print ("##############################################################")
       print ("Do you want to insert symmetries as k-point label?            ")
       print ("[0] NOT                                                       ")
       print ("[1] YES                                                       ")
       print ("##############################################################") 
       l_symmetry = input (" "); l_symmetry = int(l_symmetry)
       print (" ")       
@@ -131,15 +138,15 @@
       print ("label.TXT file should be found inside the 'output' folder ====")
       print ("after reading the PROCAR file ================================")
       print ("##############################################################") 
       print (" ")
       #-----------
       Dimensao = 1
 
-   if (dest_k != 2):
+   if (dest_k != 2 and len(inputs) == 0):
       print ("##############################################################")
       print ("Would you like to choose k-axis units?                        ")
       print ("[1] 2pi/Param. (Param. in Angs.) =============================")
       print ("[2] 1/Angs. ==================================================")
       print ("[3] 1/nm.   ==================================================")
       print ("##############################################################") 
       Dimensao = input (" "); Dimensao = int(Dimensao)
@@ -309,13 +316,15 @@
 print("= Bandas.py or Bandas.agr (via Grace) generated in the ====")   
 print("= output/Bandas folder ====================================") 
 print("===========================================================")
 
 #-----------------------------------------------------------------
 print(" ")
 print("======================= Completed =======================")
+print(" ")
 #-----------------------------------------------------------------
 
 #=======================================================================
 # User option to perform another calculation or finished the code ======
 #=======================================================================
-execute_python_file(filename = '_loop.py')
+if (len(inputs) == 0):
+   execute_python_file(filename = '_loop.py')
```

### Comparing `vasprocar-1.1.15.6/vasprocar/src/bandas_3D.py` & `vasprocar-1.1.15.7/vasprocar/src/bandas_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/bandas_4D.py` & `vasprocar-1.1.15.7/vasprocar/src/bandas_4D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/correction_file.py` & `vasprocar-1.1.15.7/vasprocar/src/correction_file.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/etc/DOI.png` & `vasprocar-1.1.15.7/vasprocar/src/etc/DOI.png`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/etc/Greek_alphabet.jpg` & `vasprocar-1.1.15.7/vasprocar/src/etc/Greek_alphabet.jpg`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/fermi_surface.py` & `vasprocar-1.1.15.7/vasprocar/src/fermi_surface.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/level_countour.py` & `vasprocar-1.1.15.7/vasprocar/src/level_countour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_bandas_2D.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_bandas_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_chgcar.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_chgcar.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_dielectric_function.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_parchg.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_parchg.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_potencial.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_potencial.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_projecao_localizacao.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_projecao_orbitais.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_projecao_psi.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_psi.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_projecao_spin.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_spin.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/Grace/plot_wave_function.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_wave_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/_plot_settings.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/_plot_settings.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_bandas_2D.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_bandas_3D_matplotlib.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_3D_matplotlib.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_bandas_3D_plotly.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_3D_plotly.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_bandas_4D_plotly.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_4D_plotly.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_chgcar.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_chgcar.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_dielectric_function.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_dos_pdos_ldos.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_fermi_surface.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_fermi_surface.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_level_countour.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_level_countour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_parchg.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_parchg.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_potencial.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_potencial.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_projecao_localizacao.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_projecao_orbitais.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_projecao_psi.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_psi.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_projecao_spin.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_spin.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_spin_texture_2D.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_spin_texture_3D.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_spin_texture_4D.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_4D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_spin_texture_4D_[iso].py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_4D_[iso].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_spin_texture_contour.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_contour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_spin_texture_contour_video.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_contour_video.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/plot/plot_wave_function.py` & `vasprocar-1.1.15.7/vasprocar/src/plot/plot_wave_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/projecao_localizacao.py` & `vasprocar-1.1.15.7/vasprocar/src/projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/projecao_orbitais.py` & `vasprocar-1.1.15.7/vasprocar/src/projecao_orbitais.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,33 +18,34 @@
 #======================================================================
 execute_python_file(filename = DFT + '_info.py')
 
 #======================================================================
 # Get the input from user =============================================
 #======================================================================
 
-if (n_orb == 3):
-   print ("#############################")
-   print ("Projection of Orbitals: S|P|D")
-   print ("#############################")
-
-if (n_orb == 4):
-   print ("###############################") 
-   print ("Projection of Orbitals: S|P|D|F")
-   print ("###############################") 
-
-if (n_orb >= 9):
-   print ("################################################################") 
-   print ("Projection of Orbitals: S, P (Px|Py|Pz), D (Dxy|Dyz|Dz2|Dxz|Dx2)")
-   if(n_orb == 16):
-     print ("                        F (Fyx2|Fxyz|Fyz2|Fzz2|Fxz2|Fzx2|Fxx2)")
-   print ("################################################################") 
-print(" ") 
+if (len(inputs) == 0):
+   if (n_orb == 3):
+      print ("#############################")
+      print ("Projection of Orbitals: S|P|D")
+      print ("#############################")
+
+   if (n_orb == 4):
+      print ("###############################") 
+      print ("Projection of Orbitals: S|P|D|F")
+      print ("###############################") 
+
+   if (n_orb >= 9):
+      print ("################################################################") 
+      print ("Projection of Orbitals: S, P (Px|Py|Pz), D (Dxy|Dyz|Dz2|Dxz|Dx2)")
+      if(n_orb == 16):
+        print ("                        F (Fyx2|Fxyz|Fyz2|Fzz2|Fxz2|Fzx2|Fxx2)")
+      print ("################################################################") 
+   print(" ") 
 
-if (escolha == -1):
+if (escolha == -1 and len(inputs) == 0):
 
    print ("###############################################################") 
    print ("Do you want to change the color pattern of Orbital projections?")
    print ("[0] NOT                                                        ")
    print ("[1] YES                                                        ")
    print ("###############################################################") 
    esc_color = input (" "); esc_color = int(esc_color)
@@ -110,38 +111,42 @@
             #---------------------
             tcor = cor_orb.split()
             c_Fyx2 = int(tcor[0]); c_Fxyz = int(tcor[1]); c_Fyz2 = int(tcor[2]); c_Fzz2 = int(tcor[3])
             c_Fxz2 = int(tcor[4]); c_Fzx2 = int(tcor[5]); c_Fxx2 = int(tcor[6])
             #---------------------
             print (" ")
 
-   print ("##############################################################")
-   print ("Regarding the Plot of Bands, choose ==========================")
-   print ("[0] Plot/Analyze all bands ===================================")
-   print ("[1] Plot/Analyze selected bands ==============================")
-   print ("##############################################################")
-   esc_bands = input (" "); esc_bands = int(esc_bands)
-   print(" ")
+if (escolha == -1):
+
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Regarding the Plot of Bands, choose ==========================")
+      print ("[0] Plot/Analyze all bands ===================================")
+      print ("[1] Plot/Analyze selected bands ==============================")
+      print ("##############################################################")
+      esc_bands = input (" "); esc_bands = int(esc_bands)
+      print(" ")
 
    if (esc_bands == 0):
       bands_range = '1:' + str(nb)
 
-   if (esc_bands == 1):     
-      print ("##############################################################")
-      print ("Select the bands to be analyzed using intervals:              ")
-      print ("Type as in the examples below =============================== ")
-      print ("------------------------------------------------------------- ")
-      print ("Bands can be added in any order ----------------------------- ")
-      print ("------------------------------------------------------------- ")
-      print ("bands_intervals  35:42                                        ")          
-      print ("bands_intervals  1:15 27:69 18:19 76*                         ")
-      print ("bands_intervals  7* 9* 11* 13* 14-15                          ")
-      print ("##############################################################")
-      bands_range = input ("bands_intervals  ")
-      print (" ")
+   if (esc_bands == 1):
+      if (len(inputs) == 0):    
+         print ("##############################################################")
+         print ("Select the bands to be analyzed using intervals:              ")
+         print ("Type as in the examples below =============================== ")
+         print ("------------------------------------------------------------- ")
+         print ("Bands can be added in any order ----------------------------- ")
+         print ("------------------------------------------------------------- ")
+         print ("bands_intervals  35:42                                        ")          
+         print ("bands_intervals  1:15 27:69 18:19 76*                         ")
+         print ("bands_intervals  7* 9* 11* 13* 14-15                          ")
+         print ("##############################################################")
+         bands_range = input ("bands_intervals  ")
+         print (" ")
       #------------------------------------------------------------------------------------------
       selected_bands = bands_range.replace(':', ' ').replace('-', ' ').replace('*', ' *').split()
       loop = int(len(selected_bands)/2)
       #------------------------------------------------------------------------------------------
       
       for i in range (1,(loop+1)):
           #--------------------------------------------------------
@@ -154,73 +159,78 @@
              print (" ")
              print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
              print ("ERROR: The values of the informed bands are incorrect %%%%")
              print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
              confirmation = input (" ")
              exit()       
 
-   print ("##############################################################") 
-   print ("with respect to energy, would you like? ======================")
-   print ("[0] Use the default energy value from DFT output =============")
-   print ("[1] Shift the Fermi level to 0.0 eV  =========================")
-   print ("##############################################################") 
-   esc_fermi = input (" "); esc_fermi = int(esc_fermi)
-   print (" ")   
-
-   print ("##############################################################") 
-   print ("Do you want to modify the energy range to be plotted? ========")
-   print ("[0] NOT                                                       ")
-   print ("[1] YES                                                       ")
-   print ("##############################################################")
-   esc_range_E = input (" "); esc_range_E = int(esc_range_E)
-   print (" ")
+   if (len(inputs) == 0):
+      print ("##############################################################") 
+      print ("with respect to energy, would you like? ======================") 
+      print ("[0] Use the default energy value from DFT output =============")
+      print ("[1] Shift the Fermi level to 0.0 eV  =========================")
+      print ("##############################################################") 
+      esc_fermi = input (" "); esc_fermi = int(esc_fermi)
+      print (" ")   
 
-   if (esc_range_E == 1):
+   if (len(inputs) == 0):
       print ("##############################################################") 
-      print ("Enter the energy range to be plotted: ========================")
-      print ("Note: Enter the lowest and highest energy value to be plotted ")
-      print ("            in relation to the Fermi Level                    ")
-      print ("Examples:                                                     ")
-      print ("--------------------------------------------------------------")
-      print ("E_min E_max: -3.0 15.0                                        ")
-      print ("E_min E_max: -5.1 5.0                                         ")
-      print ("##############################################################")      
-      range_E = input ("E_min E_max:  ")
+      print ("Do you want to modify the energy range to be plotted? ========")
+      print ("[0] NOT                                                       ")
+      print ("[1] YES                                                       ")
+      print ("##############################################################")
+      esc_range_E = input (" "); esc_range_E = int(esc_range_E)
       print (" ")
+
+   if (esc_range_E == 1):
+      if (len(inputs) == 0):
+         print ("##############################################################") 
+         print ("Enter the energy range to be plotted: ========================")
+         print ("Note: Enter the lowest and highest energy value to be plotted ")
+         print ("            in relation to the Fermi Level                    ")
+         print ("Examples:                                                     ")
+         print ("--------------------------------------------------------------")
+         print ("E_min E_max: -3.0 15.0                                        ")
+         print ("E_min E_max: -5.1 5.0                                         ")
+         print ("##############################################################")      
+         range_E = input ("E_min E_max:  ")
+         print (" ")
       #--------------------------------------------------
       selected_energ = range_E.replace('-', ' -').replace('+', ' +').replace(':', ' ').split()
       E_min = float(selected_energ[0])
       E_max = float(selected_energ[1])
 
-   print ("##############################################################")
-   print ("What do you want to analyze? =================================")
-   print ("[0] Analyze all ions in the lattice ==========================")
-   print ("[1] Analyze selected Ions ====================================")
-   print ("##############################################################")
-   esc_ions = input (" "); esc_ions = int(esc_ions)
-   print(" ")
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("What do you want to analyze? =================================")
+      print ("[0] Analyze all ions in the lattice ==========================")
+      print ("[1] Analyze selected Ions ====================================")
+      print ("##############################################################")
+      esc_ions = input (" "); esc_ions = int(esc_ions)
+      print(" ")
 
    if (esc_ions == 1):
       
       #-------------------------
       sim_nao = ["nao"]*(ni + 1)  #  sim_nao vector initialization
       #-------------------------
 
-      print ("################################################################")
-      print ("Choose the ions_ranges to be analyzed: ======================== ")
-      print ("Type as in the examples below ================================= ")
-      print ("----------------------------------------------------------------")
-      print ("The order in which the ions are added does not change the result")
-      print ("----------------------------------------------------------------")
-      print ("ions_ranges  1:5 3:9 11* 15:27                                  ")
-      print ("ions_ranges  7:49 50:53                                         ")
-      print ("ions_ranges  1* 3* 6:9                                          ")
-      print ("################################################################")
-      ion_range = input ("ions_ranges  ")
-      print (" ")
+      if (len(inputs) == 0):
+         print ("################################################################")
+         print ("Choose the ions_ranges to be analyzed: ======================== ")
+         print ("Type as in the examples below ================================= ")
+         print ("----------------------------------------------------------------")
+         print ("The order in which the ions are added does not change the result")
+         print ("----------------------------------------------------------------")
+         print ("ions_ranges  1:5 3:9 11* 15:27                                  ")
+         print ("ions_ranges  7:49 50:53                                         ")
+         print ("ions_ranges  1* 3* 6:9                                          ")
+         print ("################################################################")
+         ion_range = input ("ions_ranges  ")
+         print (" ")
       #---------------------------------------------------------------------------------------
       selected_ions = ion_range.replace(':', ' ').replace('-', ' ').replace('*', ' *').split()
       loop = int(len(selected_ions)/2)
       #---------------------------------------------------------------------------------------
       
       for i in range (1,(loop+1)):
           #------------------------------------------------------
@@ -236,69 +246,73 @@
              print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
              confirmation = input (" ")
              exit()
           #----------------------------------------------------------------------           
           for j in range(loop_i, (loop_f + 1)):
               sim_nao[j] = "sim"    
 
-   print (" ")
-   print ("##############################################################")
-   print ("Would you like to label the k-points?                         ")
-   print ("[0] DO NOT label the k-points  ===============================")
-   print ("[1] highlight k-points present in KPOINTS file ===============")
-   print ("[2] Customize: highlight and Label k-points   ================")
-   print ("##############################################################")  
-   dest_k = input (" "); dest_k = int(dest_k)
-   print (" ")
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Would you like to label the k-points?                         ")
+      print ("[0] DO NOT label the k-points  ===============================")
+      print ("[1] highlight k-points present in KPOINTS file ===============")
+      print ("[2] Customize: highlight and Label k-points   ================")
+      print ("##############################################################") 
+      dest_k = input (" "); dest_k = int(dest_k)
+      print (" ")
+   #--------------
+   l_symmetry = 0
 
-   if (DFT == '_QE/' and dest_k == 2):
+   if (DFT == '_QE/' and dest_k == 2 and len(inputs) == 0):
       print ("##############################################################")
-      print ("Do you want to insert the symmetries as label of the k-points?")
+      print ("Do you want to insert symmetries as k-point label?            ")
       print ("[0] NOT                                                       ")
       print ("[1] YES                                                       ")
       print ("##############################################################") 
       l_symmetry = input (" "); l_symmetry = int(l_symmetry)
       print (" ") 
 
    if (dest_k == 2):
       print ("##############################################################")
       print ("label.TXT file should be found inside the 'output' folder ====")
       print ("after reading the PROCAR file ================================")
       print ("##############################################################") 
       print (" ")
-
+      #-----------
       Dimensao = 1
 
-   if (dest_k != 2):   
+   if (dest_k != 2 and len(inputs) == 0):
       print ("##############################################################")
       print ("Would you like to choose k-axis units?                        ")
       print ("[1] 2pi/Param. (Param. in Angs.) =============================")
       print ("[2] 1/Angs. ==================================================")
       print ("[3] 1/nm.   ==================================================")
       print ("##############################################################")
       Dimensao = input (" "); Dimensao = int(Dimensao)
       print(" ")
 
-   print ("##############################################################")
-   print ("Enter the weight/size of the spheres in the projection: ======")
-   print ("Enter a value between 0.0 and 1.0 ============================")
-   print ("##############################################################")
-   peso_total = input (" "); peso_total = float(peso_total)
-   print(" ")
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Enter the weight/size of the spheres in the projection: ======")
+      print ("Enter a value between 0.0 and 1.0 ============================")
+      print ("##############################################################")
+      peso_total = input (" "); peso_total = float(peso_total)
+      print(" ")
 
-   print ("##############################################################")
-   print ("Enter the transparency value to apply to the projections:     ")
-   print ("This option is useful for checking the overlap of orbitals.   ")   
-   print ("Enter a value between 0.0 and 1.0 ============================")
-   print ("==============================================================")
-   print ("Hint: The higher the k-point density, the lower the ==========")
-   print ("      transparency value used, start with 0.5 ================")
-   print ("##############################################################")
-   transp = input (" "); transp = float(transp)
-   print(" ")         
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Enter the transparency value to apply to the projections:     ")
+      print ("This option is useful for checking the overlap of orbitals.   ")   
+      print ("Enter a value between 0.0 and 1.0 ============================")
+      print ("==============================================================")
+      print ("Hint: The higher the k-point density, the lower the ==========") 
+      print ("      transparency value used, start with 0.5 ================")
+      print ("##############################################################")
+      transp = input (" "); transp = float(transp)
+      print(" ")         
 
 if (escolha == 1):
    bands_range = '1:' + str(nb)
    esc_fermi = 1
    esc_range_E = 0  
    esc_ions = 0
    dest_k = 1
@@ -489,13 +503,15 @@
 print("= Edit the Plot of the projections through Orbitais.py files or ")
 print("= .agr files (Grace) generated in the output/Orbitais folder    ")
 print("================================================================")
    
 #-----------------------------------------------------------------------
 print(" ")
 print("-------------------------- Completed --------------------------")
+print(" ")
 #-----------------------------------------------------------------------
 
 #=======================================================================
 # User option to perform another calculation or finished the code ======
 #=======================================================================
-execute_python_file(filename = '_loop.py')
+if (len(inputs) == 0):
+   execute_python_file(filename = '_loop.py')
```

### Comparing `vasprocar-1.1.15.6/vasprocar/src/projecao_psi.py` & `vasprocar-1.1.15.7/vasprocar/src/projecao_psi.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/projecao_spin.py` & `vasprocar-1.1.15.7/vasprocar/src/projecao_spin.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,70 +25,73 @@
 print ("##############################################################")
 print ("########### 2D Plot of Spin Components (Sx|Sy|Sz): ###########")
 print ("##############################################################") 
 print (" ")
 
 if (escolha == -1):
 
-   print ("#######################################################################") 
-   print ("Do you want to change the color pattern of the Spin Up|Down Components ")
-   print ("[0] NOT                                                                ")
-   print ("[1] YES                                                                ")
-   print ("#######################################################################") 
-   esc_color = input (" "); esc_color = int(esc_color)
-   print (" ")  
+   if (len(inputs) == 0):
+      print ("#######################################################################") 
+      print ("Do you want to change the color pattern of the Spin Up|Down Components ")
+      print ("[0] NOT                                                                ")
+      print ("[1] YES                                                                ")
+      print ("#######################################################################") 
+      esc_color = input (" "); esc_color = int(esc_color)
+      print (" ")  
 
    if (esc_color == 1):
-      print ("##############################################################")
-      print ("color code:                                                   ")
-      print ("0  White   | 1  Black | 2  Red    | 3  Green  | 4  Blue       ")
-      print ("5  Yellow  | 6  Borwn | 7  Grey   | 8  Violet | 9  Cyan       ")
-      print ("10 Magenta |11 Orange | 12 Indigo | 13 Maroon | 14 Turquesa   ")
-      print ("15 Dark_Green                                                 ")
-      print ("##############################################################")       
-      print ("VASProcar color pattern:                                      ")
-      print ("                                                              ")
-      print ("Spin_Up | Spin_Down: 2 4 (Red, Blue)                          ")
-      print ("##############################################################") 
-      print (" ")
-
-      print ("==============================================================") 
-      print ("Enter the Spin Up and Spin Down colors in sequence:           ")
-      cor_spin = input ("Spin_Up | Spin_Down: ")
+      if (len(inputs) == 0):
+         print ("##############################################################")
+         print ("color code:                                                   ")
+         print ("0  White   | 1  Black | 2  Red    | 3  Green  | 4  Blue       ")
+         print ("5  Yellow  | 6  Borwn | 7  Grey   | 8  Violet | 9  Cyan       ")
+         print ("10 Magenta |11 Orange | 12 Indigo | 13 Maroon | 14 Turquesa   ")
+         print ("15 Dark_Green                                                 ")
+         print ("##############################################################")       
+         print ("VASProcar color pattern:                                      ")
+         print ("                                                              ")
+         print ("Spin_Up | Spin_Down: 2 4 (Red, Blue)                          ")
+         print ("##############################################################") 
+         print (" ")
+         print ("==============================================================") 
+         print ("Enter the Spin Up and Spin Down colors in sequence:           ")
+         cor_spin = input ("Spin_Up | Spin_Down: ")
+         print (" ")  
       #-------------------------
       tcor = cor_spin.split()
       c_spin_up = int(tcor[0])
       c_spin_down = int(tcor[1])
       #-------------------------
-      print (" ")     
-
-   print ("##############################################################")
-   print ("Regarding the Plot of Bands, choose ==========================")
-   print ("[0] Plot/Analyze all bands ===================================")
-   print ("[1] Plot/Analyze selected bands ==============================")
-   print ("##############################################################")
-   esc_bands = input (" "); esc_bands = int(esc_bands)
-   print(" ")
+   
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Regarding the Plot of Bands, choose ==========================")
+      print ("[0] Plot/Analyze all bands ===================================")
+      print ("[1] Plot/Analyze selected bands ==============================")
+      print ("##############################################################")
+      esc_bands = input (" "); esc_bands = int(esc_bands)
+      print(" ")
 
    if (esc_bands == 0):
       bands_range = '1:' + str(nb)
 
    if (esc_bands == 1):     
-      print ("##############################################################")
-      print ("Select the bands to be analyzed using intervals: =============")
-      print ("Type as in the examples below =============================== ")
-      print ("------------------------------------------------------------- ")
-      print ("Bands can be added in any order ----------------------------- ")
-      print ("------------------------------------------------------------- ")
-      print ("bands_intervals  35:42                                        ")          
-      print ("bands_intervals  1:15 27:69 18:19 76*                         ")
-      print ("bands_intervals  7* 9* 11* 13* 16:21                          ")
-      print ("##############################################################")
-      bands_range = input ("bands_intervals  ")
-      print (" ")
+      if (len(inputs) == 0): 
+         print ("##############################################################")
+         print ("Select the bands to be analyzed using intervals: =============")
+         print ("Type as in the examples below =============================== ")
+         print ("------------------------------------------------------------- ")
+         print ("Bands can be added in any order ----------------------------- ")
+         print ("------------------------------------------------------------- ")
+         print ("bands_intervals  35:42                                        ")          
+         print ("bands_intervals  1:15 27:69 18:19 76*                         ")
+         print ("bands_intervals  7* 9* 11* 13* 16:21                          ")
+         print ("##############################################################")
+         bands_range = input ("bands_intervals  ")
+         print (" ")
       #------------------------------------------------------------------------------------------
       selected_bands = bands_range.replace(':', ' ').replace('-', ' ').replace('*', ' *').split()
       loop = int(len(selected_bands)/2)
       #------------------------------------------------------------------------------------------
       
       for i in range (1,(loop+1)):
           #-----------------------------------------
@@ -101,73 +104,79 @@
              print (" ")
              print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
              print ("ERROR: The values of the informed bands are incorrect %%%%")
              print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
              confirmation = input (" ")
              exit()
 
-   print ("##############################################################") 
-   print ("with respect to energy, would you like? ======================")
-   print ("[0] Use the default energy value from DFT output =============")
-   print ("[1] Shift the Fermi level to 0.0 eV  =========================")
-   print ("##############################################################") 
-   esc_fermi = input (" "); esc_fermi = int(esc_fermi)
-   print (" ")   
-
-   print ("##############################################################") 
-   print ("Do you want to modify the energy range to be plotted? ========")
-   print ("[0] NOT                                                       ")
-   print ("[1] YES                                                       ")
-   print ("##############################################################")
-   esc_range_E = input (" "); esc_range_E = int(esc_range_E)
-   print (" ")
+   if (len(inputs) == 0):
+      print ("##############################################################") 
+      print ("with respect to energy, would you like? ======================")
+      print ("[0] Use the default energy value from DFT output =============")
+      print ("[1] Shift the Fermi level to 0.0 eV  =========================")
+      print ("##############################################################")
+      esc_fermi = input (" "); esc_fermi = int(esc_fermi)
+      print (" ")   
 
-   if (esc_range_E == 1):
+   if (len(inputs) == 0):
       print ("##############################################################") 
-      print ("Enter the energy range to be plotted: ========================")
-      print ("Note: Enter the lowest and highest energy value to be plotted ")
-      print ("            in relation to the Fermi Level.                   ")
-      print ("Examples:                                                     ")
-      print ("--------------------------------------------------------------")
-      print ("E_min E_max: -3.0 15.0                                        ")
-      print ("E_min E_max: -5.1 5.0                                         ")
-      print ("##############################################################")      
-      range_E = input ("E_min E_max:  ")
+      print ("Do you want to modify the energy range to be plotted? ========")
+      print ("[0] NOT                                                       ")
+      print ("[1] YES                                                       ")
+      print ("##############################################################")
+      esc_range_E = input (" "); esc_range_E = int(esc_range_E)
       print (" ")
-      #--------------------------------------------------
+
+   if (esc_range_E == 1):
+      if (len(inputs) == 0):
+         print ("##############################################################") 
+         print ("Enter the energy range to be plotted: ========================")
+         print ("Note: Enter the lowest and highest energy value to be plotted ")
+         print ("      in relation to the Fermi Level                          ")
+         print ("Examples:                                                     ")
+         print ("--------------------------------------------------------------")
+         print ("E_min E_max: -3.0 15.0                                        ")
+         print ("E_min E_max: -5.1 5.0                                         ")
+         print ("##############################################################")      
+         range_E = input ("E_min E_max:  ")
+         print (" ")
+      #---------------------------------------------------------------------------------------
       selected_energ = range_E.replace('-', ' -').replace('+', ' +').replace(':', ' ').split()
+      #--------------------------------------------------------------------------------------- 
       E_min = float(selected_energ[0])
       E_max = float(selected_energ[1])
 
-   print ("##############################################################")
-   print ("What do you want to Plot/Analyze? ============================")
-   print ("[0] to analyze all ions in the lattice =======================")
-   print ("[1] to analyze selected ions =================================")
-   print ("##############################################################")
-   esc_ions = input (" "); esc_ions = int(esc_ions)
-   print (" ")
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("What do you want to Plot/Analyze? ============================")
+      print ("[0] to analyze all ions in the lattice =======================")
+      print ("[1] to analyze selected ions =================================")
+      print ("##############################################################")
+      esc_ions = input (" "); esc_ions = int(esc_ions)
+      print (" ")
 
    if (esc_ions == 1):
 
       #-------------------------
       sim_nao = ["nao"]*(ni + 1)  
       #-------------------------
 
-      print ("################################################################")
-      print ("Choose the intervals_of_ions to be analyzed: ===================")
-      print ("Type as in the examples below ==================================")
-      print ("----------------------------------------------------------------")
-      print ("The order in which the ions are added does not change the result")
-      print ("----------------------------------------------------------------")
-      print ("intervals_of_ions  1:5 3:9 11* 15:27                            ")          
-      print ("intervals_of_ions  7:49 50:53                                   ")
-      print ("intervals_of_ions  3* 6* 8:11                                   ")        
-      print ("################################################################") 
-      ion_range = input ("intervals_of_ions  ")
-      print (" ")
+      if (len(inputs) == 0):
+         print ("################################################################")
+         print ("Choose the intervals_of_ions to be analyzed: ===================")
+         print ("Type as in the examples below ==================================")
+         print ("----------------------------------------------------------------")
+         print ("The order in which the ions are added does not change the result")
+         print ("----------------------------------------------------------------")
+         print ("intervals_of_ions  1:5 3:9 11* 15:27                            ")          
+         print ("intervals_of_ions  7:49 50:53                                   ")
+         print ("intervals_of_ions  3* 6* 8:11                                   ")        
+         print ("################################################################") 
+         ion_range = input ("intervals_of_ions  ")
+         print (" ")
       #-------------------------------------------------------------------------------
       selected_ions = ion_range.replace(':', ' ').replace('-', ' ').replace('*', ' *').split()
       loop = int(len(selected_ions)/2)
       #-------------------------------------------------------------------------------
       
       for i in range (1,(loop+1)):
           #--------------------------------------------------------
@@ -183,70 +192,73 @@
              print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
              confirmation = input (" ")
              exit()
           #----------------------------------------------------------------------           
           for j in range(loop_i, (loop_f + 1)):
               sim_nao[j] = "sim" 
    
-   print ("##############################################################")
-   print ("Would you like to label the k-points?                         ")
-   print ("[0] DO NOT label the k-points  ===============================")
-   print ("[1] highlight k-points present in KPOINTS file ===============")
-   print ("[2] Customize: highlight and Label k-points   ================")
-   print ("##############################################################") 
-   dest_k = input (" "); dest_k = int(dest_k)
-   print (" ")
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Would you like to label the k-points?                         ")
+      print ("[0] DO NOT label the k-points  ===============================")
+      print ("[1] highlight k-points present in KPOINTS file ===============")
+      print ("[2] Customize: highlight and Label k-points   ================")
+      print ("##############################################################") 
+      dest_k = input (" "); dest_k = int(dest_k)
+      print (" ")
 
-   if (DFT == '_QE/' and dest_k == 2):
+   if (DFT == '_QE/' and dest_k == 2 and len(inputs) == 0):
       print ("##############################################################")
       print ("Do you want to insert symmetries as k-point label?            ")
       print ("[0] NOT                                                       ")
       print ("[1] YES                                                       ")
       print ("##############################################################") 
       l_symmetry = input (" "); l_symmetry = int(l_symmetry)
       print (" ") 
 
    if (dest_k == 2):
       print ("##############################################################")
       print ("label.TXT file should be found inside the 'output' folder ====")
       print ("after reading the PROCAR file ================================")
       print ("##############################################################") 
       print (" ")
-
+      #-----------
       Dimensao = 1
 
-   if (dest_k != 2):
+   if (dest_k != 2 and len(inputs) == 0):
       print ("##############################################################")
       print ("Would you like to choose k-axis units?                        ")
       print ("[1] 2pi/Param. (Param. in Angs.) =============================")
       print ("[2] 1/Angs. ==================================================")
       print ("[3] 1/nm.   ==================================================")
       print ("##############################################################")
       Dimensao = input (" "); Dimensao = int(Dimensao)
       print(" ")
 
-   print ("##############################################################")
-   print ("Enter the weight/size of the spheres in the projection: ======")
-   print ("Enter a value between 0.0 and 1.0 ============================")
-   print ("##############################################################")
-   peso_total = input (" "); peso_total = float(peso_total)
-   print(" ")
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Enter the weight/size of the spheres in the projection: ======")
+      print ("Enter a value between 0.0 and 1.0 ============================")
+      print ("##############################################################")
+      peso_total = input (" "); peso_total = float(peso_total)
+      print(" ")
 
-   print ("################################################################")
-   print ("Enter the transparency value to apply to the projections:       ")
-   print ("This option is useful for checking for overlaps ================")   
-   print ("Enter a value between 0.0 and 1.0 ==============================")
-   print ("================================================================")
-   print ("Hint: The higher the k-point density, the lower the transparency")
-   print ("      value used, start with 0.5 ===============================")
-   print ("################################################################")
-   transp = input (" "); transp = float(transp)
-   print(" ")           
+   if (len(inputs) == 0):
+      print ("################################################################")
+      print ("Enter the transparency value to apply to the projections:       ") 
+      print ("This option is useful for checking for overlaps ================")   
+      print ("Enter a value between 0.0 and 1.0 ==============================")
+      print ("================================================================")
+      print ("Hint: The higher the k-point density, the lower the transparency")
+      print ("      value used, start with 0.5 ===============================")
+      print ("################################################################")
+      transp = input (" "); transp = float(transp)
+      print(" ")           
 
-if (escolha == 1):
+if (escolha == 1 and len(inputs) == 0):
    bands_range = '1:' + str(nb)
    esc_fermi = 1
    esc_range_E = 0  
    esc_ions = 0
    dest_k = 1
    Dimensao = 1
    l_symmetry = 0
@@ -428,13 +440,16 @@
 print("= Edit the Plot of projections using the following Spin.py or")
 print("= .agr files (via Grace) generated in the output/Spin folder.")   
 print("=============================================================")
 
 #-----------------------------------------------------------------
 print(" ")
 print("======================= Completed =======================")
+print(" ")
 #-----------------------------------------------------------------
 
+
 #=======================================================================
 # User option to perform another calculation or finished the code ======
 #=======================================================================
-execute_python_file(filename = '_loop.py')
+if (len(inputs) == 0):
+   execute_python_file(filename = '_loop.py')
```

### Comparing `vasprocar-1.1.15.6/vasprocar/src/spin_texture.py` & `vasprocar-1.1.15.7/vasprocar/src/spin_texture.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/spin_texture_contour.py` & `vasprocar-1.1.15.7/vasprocar/src/spin_texture_contour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar/src/spin_texture_contour_video.py` & `vasprocar-1.1.15.7/vasprocar/src/spin_texture_contour_video.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.6/vasprocar.egg-info/PKG-INFO` & `vasprocar-1.1.15.7/vasprocar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasprocar
-Version: 1.1.15.6
+Version: 1.1.15.7
 Summary: VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP code, through an interactive user interface.
 Home-page: https://doi.org/10.5281/zenodo.6343960
 Download-URL: https://doi.org/10.5281/zenodo.6343960
 Author: Augusto de Lelis Araujo and Renan da Paixao Maciel
 Author-email: augusto-lelis@outlook.com, renan.maciel@physics.uu.se
 License: GNU GPLv3
 Description-Content-Type: text/markdown
```

### Comparing `vasprocar-1.1.15.6/vasprocar.egg-info/SOURCES.txt` & `vasprocar-1.1.15.7/vasprocar.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,22 @@
 vasprocar/src/_VASP/contribuicao.py
 vasprocar/src/_VASP/dielectric_function.py
 vasprocar/src/_VASP/dos_pdos_ldos.py
 vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py
 vasprocar/src/_VASP/kpoints_2D_3D.py
 vasprocar/src/_VASP/parchg.py
 vasprocar/src/_VASP/poscar_replace.py
+vasprocar/src/_VASP/postar_combination.py
 vasprocar/src/_VASP/potencial.py
 vasprocar/src/_VASP/wave_function.py
 vasprocar/src/etc/BibTeX.dat
 vasprocar/src/etc/DOI.png
 vasprocar/src/etc/Greek_alphabet.jpg
+vasprocar/src/inputs/inputs.py
+vasprocar/src/inputs/inputs_files.py
 vasprocar/src/plot/_plot_settings.py
 vasprocar/src/plot/plot_bandas_2D.py
 vasprocar/src/plot/plot_bandas_3D_matplotlib.py
 vasprocar/src/plot/plot_bandas_3D_plotly.py
 vasprocar/src/plot/plot_bandas_4D_plotly.py
 vasprocar/src/plot/plot_chgcar.py
 vasprocar/src/plot/plot_dielectric_function.py
```


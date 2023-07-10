# Comparing `tmp/csp-cryspy-1.1.1.tar.gz` & `tmp/csp-cryspy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csp-cryspy-1.1.1.tar", last modified: Wed Jun 14 14:14:14 2023, max compression
+gzip compressed data, was "csp-cryspy-1.2.0.tar", last modified: Mon Jul 10 10:42:36 2023, max compression
```

## Comparing `csp-cryspy-1.1.1.tar` & `csp-cryspy-1.2.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.989115 csp-cryspy-1.1.1/
--rw-r--r--   0 yamashita06   (501) staff       (20)     1080 2018-02-20 06:34:19.000000 csp-cryspy-1.1.1/LICENSE
--rw-r--r--   0 yamashita06   (501) staff       (20)     5616 2023-06-14 14:14:14.988944 csp-cryspy-1.1.1/PKG-INFO
--rw-r--r--   0 yamashita06   (501) staff       (20)     3710 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/README.md
--rw-r--r--   0 yamashita06   (501) staff       (20)      991 2023-03-16 13:18:20.000000 csp-cryspy-1.1.1/pyproject.toml
--rw-r--r--   0 yamashita06   (501) staff       (20)       38 2023-06-14 14:14:14.989160 csp-cryspy-1.1.1/setup.cfg
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.959743 csp-cryspy-1.1.1/src/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.960466 csp-cryspy-1.1.1/src/cryspy/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.962583 csp-cryspy-1.1.1/src/cryspy/BO/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/BO/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2580 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/BO/bo_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6772 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/BO/bo_next_select.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      726 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/BO/bo_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4804 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/BO/combo_cryspy.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      688 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/BO/select_descriptor.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.964382 csp-cryspy-1.1.1/src/cryspy/EA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3995 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/ea_append.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4870 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/ea_child.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2262 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/ea_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4765 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/ea_next_gen.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.966935 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    29426 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/crossover.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     8526 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/ea_generation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     8533 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/permutation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2858 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/rotation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     9434 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/select_parents.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6434 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/strain.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.968855 csp-cryspy-1.1.1/src/cryspy/IO/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/IO/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      452 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/IO/change_input.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1888 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/IO/io_stat.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     5567 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/IO/out_results.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4842 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/IO/pkl_data.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    70148 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/IO/read_input.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.970708 csp-cryspy-1.1.1/src/cryspy/LAQA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/LAQA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      900 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/LAQA/calc_score.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1394 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/LAQA/laqa_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1872 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/LAQA/laqa_next_selection.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1049 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/LAQA/laqa_restart.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.972673 csp-cryspy-1.1.1/src/cryspy/RS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/RS/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.973703 csp-cryspy-1.1.1/src/cryspy/RS/gen_struc_RS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/RS/gen_struc_RS/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    28135 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    19060 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/RS/gen_struc_RS/random_generation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      437 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/RS/rs_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      669 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/RS/rs_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)       65 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.974197 csp-cryspy-1.1.1/src/cryspy/calc_dscrpt/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.974953 csp-cryspy-1.1.1/src/cryspy/calc_dscrpt/FP/
--rw-r--r--   0 yamashita06   (501) staff       (20)       22 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/calc_dscrpt/FP/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3401 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/calc_dscrpt/FP/calc_FP.py
--rw-r--r--   0 yamashita06   (501) staff       (20)       17 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/calc_dscrpt/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.975363 csp-cryspy-1.1.1/src/cryspy/interactive/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/interactive/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.975901 csp-cryspy-1.1.1/src/cryspy/interface/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.976673 csp-cryspy-1.1.1/src/cryspy/interface/ASE/
--rw-------   0 yamashita06   (501) staff       (20)      684 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/interface/ASE/calc_files_ase.py
--rw-------   0 yamashita06   (501) staff       (20)     1065 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/interface/ASE/collect_ase.py
--rw-------   0 yamashita06   (501) staff       (20)     1915 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/interface/ASE/ctrl_job_ase.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.978471 csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      855 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/calc_files_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1442 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/collect_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2112 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2859 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.979864 csp-cryspy-1.1.1/src/cryspy/interface/OMX/
--rw-r--r--   0 yamashita06   (501) staff       (20)      752 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/OMX/calc_files_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2679 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/OMX/collect_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3954 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/OMX/ctrl_job_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3119 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/OMX/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.981396 csp-cryspy-1.1.1/src/cryspy/interface/QE/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/QE/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      703 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/QE/calc_files_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    11215 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/QE/collect_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3856 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/QE/ctrl_job_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2884 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/QE/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.982743 csp-cryspy-1.1.1/src/cryspy/interface/VASP/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/VASP/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      661 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/VASP/calc_files_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     9063 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/interface/VASP/collect_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3603 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/VASP/ctrl_job_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.983417 csp-cryspy-1.1.1/src/cryspy/interface/ext/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/ext/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      428 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/ext/collect_ext.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     7127 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/interface/select_code.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.984951 csp-cryspy-1.1.1/src/cryspy/interface/soiap/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/soiap/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      705 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/soiap/calc_files_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     7477 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/soiap/collect_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2173 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/soiap/ctrl_job_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2415 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/interface/soiap/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.985802 csp-cryspy-1.1.1/src/cryspy/job/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/job/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    12290 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/job/ctrl_ext.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    30846 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/job/ctrl_job.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.986196 csp-cryspy-1.1.1/src/cryspy/scripts/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/scripts/__init__.py
--rwx------   0 yamashita06   (501) staff       (20)     4166 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/scripts/cryspy.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.987085 csp-cryspy-1.1.1/src/cryspy/start/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/start/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     5316 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/start/cryspy_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4565 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/start/cryspy_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6672 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/start/gen_init_struc.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.987862 csp-cryspy-1.1.1/src/cryspy/util/
--rw-r--r--   0 yamashita06   (501) staff       (20)      106 2023-03-16 12:21:45.000000 csp-cryspy-1.1.1/src/cryspy/util/constants.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    15584 2023-05-16 07:40:54.000000 csp-cryspy-1.1.1/src/cryspy/util/struc_util.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2581 2023-06-14 14:03:15.000000 csp-cryspy-1.1.1/src/cryspy/util/utility.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:14:14.988728 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/
--rw-------   0 yamashita06   (501) staff       (20)     5616 2023-06-14 14:14:14.000000 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/PKG-INFO
--rw-------   0 yamashita06   (501) staff       (20)     3141 2023-06-14 14:14:14.000000 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/SOURCES.txt
--rw-------   0 yamashita06   (501) staff       (20)        1 2023-06-14 14:14:14.000000 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/dependency_links.txt
--rw-------   0 yamashita06   (501) staff       (20)       54 2023-06-14 14:14:14.000000 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/entry_points.txt
--rw-------   0 yamashita06   (501) staff       (20)       14 2023-06-14 14:14:14.000000 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/requires.txt
--rw-------   0 yamashita06   (501) staff       (20)        7 2023-06-14 14:14:14.000000 csp-cryspy-1.1.1/src/csp_cryspy.egg-info/top_level.txt
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.732870 csp-cryspy-1.2.0/
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1080 2018-02-20 06:34:19.000000 csp-cryspy-1.2.0/LICENSE
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5869 2023-07-10 10:42:36.732419 csp-cryspy-1.2.0/PKG-INFO
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3963 2023-07-10 10:39:43.000000 csp-cryspy-1.2.0/README.md
+-rw-r--r--   0 yamashita06   (501) staff       (20)      991 2023-03-16 13:18:20.000000 csp-cryspy-1.2.0/pyproject.toml
+-rw-r--r--   0 yamashita06   (501) staff       (20)       38 2023-07-10 10:42:36.732993 csp-cryspy-1.2.0/setup.cfg
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.640432 csp-cryspy-1.2.0/src/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.641506 csp-cryspy-1.2.0/src/cryspy/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.643432 csp-cryspy-1.2.0/src/cryspy/BO/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/BO/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2651 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/BO/bo_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     7087 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/BO/bo_next_select.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      726 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/BO/bo_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4907 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/BO/combo_cryspy.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      757 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/BO/select_descriptor.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.645002 csp-cryspy-1.2.0/src/cryspy/EA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/EA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4042 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/EA/ea_append.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4943 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/EA/ea_child.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2329 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/EA/ea_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4830 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/EA/ea_next_gen.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.647754 csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    29393 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/crossover.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     8262 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/ea_generation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     8455 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/permutation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2849 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/rotation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     9388 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/select_parents.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6428 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/strain.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.649852 csp-cryspy-1.2.0/src/cryspy/IO/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/IO/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      452 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/IO/change_input.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1825 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/IO/io_stat.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5567 2023-07-09 14:20:12.000000 csp-cryspy-1.2.0/src/cryspy/IO/out_results.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4842 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/IO/pkl_data.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    72130 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/IO/read_input.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.651975 csp-cryspy-1.2.0/src/cryspy/LAQA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/LAQA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      900 2023-05-16 07:40:54.000000 csp-cryspy-1.2.0/src/cryspy/LAQA/calc_score.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1475 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/LAQA/laqa_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1929 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/LAQA/laqa_next_selection.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1116 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/LAQA/laqa_restart.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.653344 csp-cryspy-1.2.0/src/cryspy/RS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/RS/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.654554 csp-cryspy-1.2.0/src/cryspy/RS/gen_struc_RS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/RS/gen_struc_RS/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    27405 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    18977 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/RS/gen_struc_RS/random_generation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      437 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/RS/rs_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      669 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/RS/rs_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)       65 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.655008 csp-cryspy-1.2.0/src/cryspy/calc_dscrpt/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.656374 csp-cryspy-1.2.0/src/cryspy/calc_dscrpt/FP/
+-rw-r--r--   0 yamashita06   (501) staff       (20)       22 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/calc_dscrpt/FP/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2821 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/calc_dscrpt/FP/calc_FP.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)       17 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/calc_dscrpt/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.656803 csp-cryspy-1.2.0/src/cryspy/interactive/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:03:15.000000 csp-cryspy-1.2.0/src/cryspy/interactive/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.658429 csp-cryspy-1.2.0/src/cryspy/interface/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.679126 csp-cryspy-1.2.0/src/cryspy/interface/ASE/
+-rw-r--r--   0 yamashita06   (501) staff       (20)      818 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/ASE/calc_files_ase.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1116 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/ASE/collect_ase.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2027 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/ASE/ctrl_job_ase.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.682233 csp-cryspy-1.2.0/src/cryspy/interface/LAMMPS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/interface/LAMMPS/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      988 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/LAMMPS/calc_files_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1534 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/LAMMPS/collect_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2243 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2859 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/interface/LAMMPS/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.686109 csp-cryspy-1.2.0/src/cryspy/interface/OMX/
+-rw-r--r--   0 yamashita06   (501) staff       (20)      886 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/OMX/calc_files_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2784 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/OMX/collect_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4091 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/OMX/ctrl_job_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3119 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/interface/OMX/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.689943 csp-cryspy-1.2.0/src/cryspy/interface/QE/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/interface/QE/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      836 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/QE/calc_files_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    11099 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/QE/collect_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3993 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/QE/ctrl_job_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2919 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/QE/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.694821 csp-cryspy-1.2.0/src/cryspy/interface/VASP/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/interface/VASP/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      795 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/VASP/calc_files_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     9093 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/VASP/collect_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3767 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/VASP/ctrl_job_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/interface/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.696481 csp-cryspy-1.2.0/src/cryspy/interface/ext/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/interface/ext/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      513 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/ext/collect_ext.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     7854 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/select_code.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.700656 csp-cryspy-1.2.0/src/cryspy/interface/soiap/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/interface/soiap/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      839 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/soiap/calc_files_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     7460 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/soiap/collect_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2304 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/interface/soiap/ctrl_job_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2415 2023-07-09 12:00:10.000000 csp-cryspy-1.2.0/src/cryspy/interface/soiap/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.703693 csp-cryspy-1.2.0/src/cryspy/job/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/job/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    12494 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/job/ctrl_ext.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    30886 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/job/ctrl_job.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.704727 csp-cryspy-1.2.0/src/cryspy/scripts/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/scripts/__init__.py
+-rwxr-xr-x   0 yamashita06   (501) staff       (20)     4380 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/scripts/cryspy.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.706904 csp-cryspy-1.2.0/src/cryspy/start/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/start/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5475 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/start/cryspy_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4644 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/start/cryspy_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6457 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/start/gen_init_struc.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.728805 csp-cryspy-1.2.0/src/cryspy/util/
+-rw-r--r--   0 yamashita06   (501) staff       (20)      106 2023-03-16 12:21:45.000000 csp-cryspy-1.2.0/src/cryspy/util/constants.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    15732 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/util/struc_util.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3809 2023-07-10 10:34:05.000000 csp-cryspy-1.2.0/src/cryspy/util/utility.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-07-10 10:42:36.731840 csp-cryspy-1.2.0/src/csp_cryspy.egg-info/
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5869 2023-07-10 10:42:36.000000 csp-cryspy-1.2.0/src/csp_cryspy.egg-info/PKG-INFO
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3141 2023-07-10 10:42:36.000000 csp-cryspy-1.2.0/src/csp_cryspy.egg-info/SOURCES.txt
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-07-10 10:42:36.000000 csp-cryspy-1.2.0/src/csp_cryspy.egg-info/dependency_links.txt
+-rw-r--r--   0 yamashita06   (501) staff       (20)       54 2023-07-10 10:42:36.000000 csp-cryspy-1.2.0/src/csp_cryspy.egg-info/entry_points.txt
+-rw-r--r--   0 yamashita06   (501) staff       (20)       14 2023-07-10 10:42:36.000000 csp-cryspy-1.2.0/src/csp_cryspy.egg-info/requires.txt
+-rw-r--r--   0 yamashita06   (501) staff       (20)        7 2023-07-10 10:42:36.000000 csp-cryspy-1.2.0/src/csp_cryspy.egg-info/top_level.txt
```

### Comparing `csp-cryspy-1.1.1/LICENSE` & `csp-cryspy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.1/PKG-INFO` & `csp-cryspy-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csp-cryspy
-Version: 1.1.1
+Version: 1.2.0
 Summary: CrySPY is a crystal structure prediction tool written in Python.
 Author-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 Maintainer-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 License: MIT License
         
         Copyright (c) 2018 CrySPY Development Team
         
@@ -42,26 +42,30 @@
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
 Document: https://tomoki-yamashita.github.io/CrySPY_doc  
 Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.1.1 (2023 June 14)
+version 1.2.0 (2023 July 10)
 
 ## News
+- [2023 July 10] CrySPY 1.2.0 released. Version information/version 1.2.0
+    + Interface for ASE
+    + Adoption of logging
+    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [CHANGELOG](./CHANGELOG.md)
 - [2023 June 14] CrySPY 1.1.1 released
     + bug fix
 - [2023 May 16] CrySPY 1.1.0 released
     + MPI parallelization (optional)
     + New score of LAQA
-    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
+    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [CHANGELOG](./CHANGELOG.md)
 - [2023 March 16] CrySPY 1.0.0 released
     + CrySPY is available in PyPI, so you can install by pip (project name is csp-cryspy).
-    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
+    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [CHANGELOG](./CHANGELOG.md)
 
 
 ## System requirements
 ### Python
 - Python >= 3.8
 - [PyXtal >= 0.5.3](https://pyxtal.readthedocs.io/en/latest "PyXtal")
```

### Comparing `csp-cryspy-1.1.1/README.md` & `csp-cryspy-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,30 @@
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
 Document: https://tomoki-yamashita.github.io/CrySPY_doc  
 Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.1.1 (2023 June 14)
+version 1.2.0 (2023 July 10)
 
 ## News
+- [2023 July 10] CrySPY 1.2.0 released. Version information/version 1.2.0
+    + Interface for ASE
+    + Adoption of logging
+    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [CHANGELOG](./CHANGELOG.md)
 - [2023 June 14] CrySPY 1.1.1 released
     + bug fix
 - [2023 May 16] CrySPY 1.1.0 released
     + MPI parallelization (optional)
     + New score of LAQA
-    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
+    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [CHANGELOG](./CHANGELOG.md)
 - [2023 March 16] CrySPY 1.0.0 released
     + CrySPY is available in PyPI, so you can install by pip (project name is csp-cryspy).
-    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
+    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [CHANGELOG](./CHANGELOG.md)
 
 
 ## System requirements
 ### Python
 - Python >= 3.8
 - [PyXtal >= 0.5.3](https://pyxtal.readthedocs.io/en/latest "PyXtal")
```

### Comparing `csp-cryspy-1.1.1/pyproject.toml` & `csp-cryspy-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.1/src/cryspy/BO/bo_init.py` & `csp-cryspy-1.2.0/src/cryspy/BO/bo_init.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 '''
 Initialize Bayesian optimization
 '''
 
 import configparser
+from logging import getLogger
 import random
 
 import pandas as pd
 
 from .select_descriptor import select_descriptor
 from ..IO import io_stat, pkl_data
 from ..IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def initialize(stat, init_struc_data, rslt_data):
     # ---------- log
-    print('\n# ---------- Selection: 1')
+    logger.info('# ---------- Selection: 1')
 
     # ---------- check init_struc_data
     if None in init_struc_data.values():
         raise ValueError('init_struc_data includes None')
 
     # ---------- initialize
     n_selection = 1
@@ -35,16 +38,16 @@
                            'Spg_sym_opt', 'E_eV_atom', 'Magmom', 'Opt']]
     pkl_data.save_rslt(rslt_data)
 
     # ---------- random select
     all_id = [i for i in range(len(init_struc_data))]
     if rin.manual_select_bo:
         # ------ manual select bo
-        print('Manual select: {}'.format(
-            ' '.join(str(i) for i in rin.manual_select_bo)))
+        x = ' '.join(str(i) for i in rin.manual_select_bo)
+        logger.info(f'Manual select: {x}')
         nselect = rin.nselect_bo - len(rin.manual_select_bo)
         id_queueing = rin.manual_select_bo[:]    # shallow copy
         if 0 < nselect:
             diff_id = list(set(all_id) - set(id_queueing))
             id_queueing.extend(random.sample(diff_id, nselect))
         # ------ delete the value for manual_select_bo in cryspy.in
         config = configparser.ConfigParser()
@@ -71,9 +74,10 @@
     # ---------- status
     io_stat.set_common(stat, 'selection', n_selection)
     io_stat.set_id(stat, 'selected_id', id_queueing)
     io_stat.set_id(stat, 'id_queueing', id_queueing)
     io_stat.write_stat(stat)
 
     # ---------- out and log
-    print('selected_id: {}'.format(' '.join(str(a) for a in id_queueing)))
+    x = ' '.join(str(a) for a in id_queueing)
+    logger.info(f'selected_id: {x}')
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/BO/bo_next_select.py` & `csp-cryspy-1.2.0/src/cryspy/BO/bo_next_select.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 '''
 Selection in Bayesian optimization
 '''
 
 import configparser
+from contextlib import redirect_stdout
+from logging import getLogger
+import os
 
 import numpy as np
 
 from .combo_cryspy import Policy_cryspy
 from ..IO import io_stat, out_results, pkl_data
 from ..IO import read_input as rin
 
 
-def next_select(stat, rslt_data, bo_id_data, bo_data):
+logger = getLogger('cryspy')
+
+def next_select(stat, rslt_data, bo_id_data, bo_data, noprint=False):
     # ---------- log
-    print('# ------ Bayesian optimization')
+    logger.info('# ------ Bayesian optimization')
 
     # ---------- bo_id_data and bo_data
     n_selection, id_running, id_queueing, id_select_hist = bo_id_data
     init_dscrpt_data, opt_dscrpt_data, bo_mean, bo_var, bo_score = bo_data
 
     # ---------- n_selection
     n_selection += 1
 
     # ---------- manual select
     if rin.manual_select_bo:
-        print('Manual select: {}'.format(
-            ' '.join(str(i) for i in rin.manual_select_bo)))
+        x = ' '.join(str(i) for i in rin.manual_select_bo)
+        logger.info(f'Manual select: {x}')
         # ------ check already selected
         tmp_list = [i for i in rin.manual_select_bo if i in opt_dscrpt_data]
         for j in tmp_list:
             rin.manual_select_bo.remove(j)
-            print('ID {} was already selected. Remove it'.format(j))
+            logger.info(f'ID {j} was already selected. Remove it')
         # ------ number of structure to be selected
         nselect = rin.nselect_bo - len(rin.manual_select_bo)
         id_queueing = rin.manual_select_bo
         # ------ delete the value for manual_select_bo in cryspy.in
         config = configparser.ConfigParser()
         config.read('cryspy.in')
         config.set('BO', 'manual_select_bo', '')
@@ -55,25 +60,24 @@
         non_error_id = [i for i in range(len(init_dscrpt_data))]
         for i in range(len(init_dscrpt_data)):
             if i in opt_dscrpt_data:
                 # -- already done
                 if opt_dscrpt_data[i] is None:    # find error
                     non_error_id.remove(i)
                     continue
+                x = rslt_data.loc[i]['E_eV_atom']
                 if rin.emax_bo is not None:
-                    if rslt_data.loc[i]['E_eV_atom'] > rin.emax_bo:
+                    if x > rin.emax_bo:
                         non_error_id.remove(i)
-                        print('Eliminate ID {}: {} > emax_bo'.format(
-                              i, rslt_data.loc[i]['E_eV_atom']))
+                        logger.info(f'Eliminate ID {i}: {x} > emax_bo')
                         continue
                 if rin.emin_bo is not None:
-                    if rslt_data.loc[i]['E_eV_atom'] < rin.emin_bo:
+                    if x < rin.emin_bo:
                         non_error_id.remove(i)
-                        print('Eliminate ID {}: {} < emin_bo'.format(
-                              i, rslt_data.loc[i]['E_eV_atom']))
+                        logger.info(f'Eliminate ID {i}: {x} < emin_bo')
                         continue
                 s_act.append(len(descriptors))
                 done_id.append(i)
                 descriptors.append(opt_dscrpt_data[i])
             else:
                 # -- not yet
                 if i in rin.manual_select_bo:
@@ -85,15 +89,15 @@
         targets = [rslt_data.loc[cid]['E_eV_atom'] for cid in done_id]
         # ------ list --> numpy
         s_act = np.array(s_act, dtype=int)
         descriptors = np.array(descriptors)
         targets = np.array(targets, dtype=float)
         # ------ Bayesian optimization
         actions, cryspy_mean, cryspy_var, cryspy_score = bayes_opt(
-            s_act, descriptors, targets, nselect)
+            s_act, descriptors, targets, nselect, noprint)
         # ------ actions --> id_queueing
         for i in actions:
             id_queueing.append(non_error_id[i])
         # ------ bo_mean, bo_var, bo_score
         remaining_id = list(set(non_error_id) - set(done_id))
         bo_mean[n_selection] = dict(zip(remaining_id, cryspy_mean))
         bo_var[n_selection] = dict(zip(remaining_id, cryspy_var))
@@ -124,56 +128,63 @@
     # ---------- status
     io_stat.set_common(stat, 'selection', n_selection)
     io_stat.set_id(stat, 'selected_id', id_queueing)
     io_stat.set_id(stat, 'id_queueing', id_queueing)
     io_stat.write_stat(stat)
 
     # ---------- out and log
-    print('\n\n# ---------- Selection: {}'.format(n_selection))
-    print('selected_id: {}'.format(' '.join(str(a) for a in id_queueing)))
+    logger.info(f'# ---------- Selection: {n_selection}')
+    x = ' '.join(str(a) for a in id_queueing)
+    logger.info(f'selected_id: {x}')
 
     # ---------- ext
     if rin.calc_code == 'ext':
         with open('ext/stat_job', 'w') as fstat:
             fstat.write('out\n')
 
 
-def bayes_opt(s_act, descriptors, targets, nselect):
+def bayes_opt(s_act, descriptors, targets, nselect, noprint=False):
     # ---------- start COMBO part
     # ------ standardization
     # X = combo.misc.centering(descriptors)
     dev = np.std(descriptors, axis=0)
     nonzero_indx = np.where(dev > rin.cdev)[0]
     X = (descriptors[:, nonzero_indx] - np.mean(
         descriptors[:, nonzero_indx], axis=0)) / dev[nonzero_indx]
 
     # ------ Declaring the policy by
     pc = Policy_cryspy(test_X=X)
 
     # ------ pick up data, already optimized
-    actions = pc.specified_search(specified_actions=s_act,
-                                  max_num_probes=1)
+    actions = pc.specified_search(specified_actions=s_act, max_num_probes=1)
 
     # ------ write
     pc.write(actions, -targets)    # minus for minimum search
 
     # ------ log
     out_log(pc.history)
 
     # ------ Bayes_search
-    actions, cryspy_mean, cryspy_var, cryspy_score = pc.bayes_search_cryspy(
-        max_num_probes=1,
-        num_search_each_probe=nselect,
-        score=rin.score,
-        num_rand_basis=rin.num_rand_basis)
+    if noprint:
+        with redirect_stdout(open(os.devnull, 'w')):
+            actions, cryspy_mean, cryspy_var, cryspy_score = pc.bayes_search_cryspy(
+                max_num_probes=1,
+                num_search_each_probe=nselect,
+                score=rin.score,
+                num_rand_basis=rin.num_rand_basis)
+    else:
+        actions, cryspy_mean, cryspy_var, cryspy_score = pc.bayes_search_cryspy(
+            max_num_probes=1,
+            num_search_each_probe=nselect,
+            score=rin.score,
+            num_rand_basis=rin.num_rand_basis)
 
     # ------ return
     return actions, cryspy_mean, cryspy_var, cryspy_score
 
 
 # ---------- just for log
 def out_log(history):
     n = history.total_num_search
     index = np.argmax(history.fx[0:n])
 
-    print('current best E = {0}\n'.format(-history.fx[index]))
-    print('\n')
+    logger.info(f'current best E = {-history.fx[index]}')
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/BO/bo_restart.py` & `csp-cryspy-1.2.0/src/cryspy/BO/bo_restart.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.1/src/cryspy/BO/combo_cryspy.py` & `csp-cryspy-1.2.0/src/cryspy/BO/combo_cryspy.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,33 @@
 Modify Policy class in combo3 for CrySPY
 
  This code partly includes program codes in COMBO
  (https://github.com/tsudalab/combo)
  which is distributed under the MIT License.
 '''
 
+from logging import getLogger
+
 import combo
 import numpy as np
 
 
+logger = getLogger('cryspy')
+
 # ---------- inheritance
 class Policy_cryspy(combo.search.discrete.policy):
 
     def specified_search(self, specified_actions, max_num_probes,
                          num_search_each_probe=1,
                          simulator=None, is_disp=True):
         N = int(num_search_each_probe)
         if int(max_num_probes) * N > len(self.actions):
-            raise ValueError('max_num_probes * num_search_each_probe must'
-                             ' be smaller than the length of candidates')
+            logger.error('max_num_probes * num_search_each_probe must'
+                        ' be smaller than the length of candidates')
+            raise SystemExit(1)
         for n in range(0, max_num_probes):
             action = self.get_specified_action(N, specified_actions)
             return action
 
     def get_specified_action(self, N, specified_actions):
         action = specified_actions
         self.actions = self.delete_actions(action)
@@ -100,14 +105,15 @@
         if mode == 'EI':
             f = combo.search.score.EI(predictor, training, test)
         elif mode == 'PI':
             f = combo.search.score.PI(predictor, training, test)
         elif mode == 'TS':
             f = combo.search.score.TS(predictor, training, test, alpha)
         else:
-            raise NotImplementedError('mode must be EI, PI or TS.')
+            logger.error('mode must be EI, PI or TS.')
+            raise SystemExit(1)
         # ---------- start cryspy
         cryspy_mean = predictor.get_post_fmean(training, test)
         cryspy_var = predictor.get_post_fcov(training, test)
         return f, cryspy_mean, cryspy_var
         # ---------- end cryspy
 #        return f
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/BO/select_descriptor.py` & `csp-cryspy-1.2.0/src/cryspy/BO/select_descriptor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 '''
 Select descriptors
     - FP: FingerPrint
 '''
 
-from ..util.utility import check_fppath 
+from logging import getLogger
+
+from ..util.utility import check_fppath
 from ..calc_dscrpt.FP.calc_FP import Calc_FP
 from ..IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def select_descriptor(struc_data):
     # ---------- fingerprint
     if rin.dscrpt == 'FP':
-        print('Calculate descriptors: FingerPrint', flush=True)
+        logger.info('Calculate descriptors: FingerPrint')
         # ------ check cal_fingerprint executable file
         fppath = check_fppath(rin.fppath)
         # ------ calc fingerprint
         cfp = Calc_FP(struc_data, rin.fp_rmin, rin.fp_rmax,
                       rin.fp_npoints, rin.fp_sigma, fppath)
         cfp.calc()
         return cfp.descriptors
     else:
-        raise NotImplementedError('Now FP only')
+        logger.error('Now FP only')
+        raise SystemExit(1)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/EA/ea_append.py` & `csp-cryspy-1.2.0/src/cryspy/EA/ea_append.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 '''
 Append structures by evolutionary algorithm
 '''
 
+from logging import getLogger
 import os
 
 import pandas as pd
 
 from .ea_child import child_gen
 from .gen_struc_EA.select_parents import Select_parents
 from ..IO import change_input, io_stat, out_results, pkl_data
 from ..IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def append_struc(stat, init_struc_data):
     # ---------- append structures by EA
-    print('\n# ---------- Append structures by EA')
+    logger.info('# ---------- Append structures by EA')
 
     # ---------- load data
     opt_struc_data = pkl_data.load_opt_struc()
     rslt_data = pkl_data.load_rslt()
 
     # ---------- fitness
     fitness = rslt_data['E_eV_atom'].to_dict()    # {ID: energy, ..,}
 
     # ---------- instantiate Seclect_parents class
-    print('# ------ select parents')
+    logger.info('# ------ select parents')
     sp = Select_parents(opt_struc_data, fitness, None, None, rin.n_fittest)
     if rin.slct_func == 'TNM':
         sp.set_tournament()
     else:
         sp.set_roulette()
 
     # ---------- generate offspring by EA
-    print('# ------ Generate structures')
+    logger.info('# ------ Generate structures')
     init_struc_data, eagen = child_gen(sp, init_struc_data)
 
     # ----------  ea_info
     if os.path.isfile('./data/pkl_data/EA_data.pkl'):
         _, _, ea_info, ea_origin = pkl_data.load_ea_data()
     else:
         # ------ initialize
@@ -76,24 +79,22 @@
 
     # ---------- save ea_data
     ea_data = (None, None, ea_info, ea_origin)
     pkl_data.save_ea_data(ea_data)
 
     # ---------- change variables in cryspy.in
     config = change_input.config_read()
-    print('# -- Changed cryspy.in')
+    logger.info('# -- Changed cryspy.in')
     # ------ tot_struc
     change_input.change_basic(config, 'tot_struc', rin.tot_struc + rin.n_pop)
-    print('Changed tot_struc in cryspy.in from {} to {}'.format(
-          rin.tot_struc, rin.tot_struc + rin.n_pop))
+    logger.info(f'Changed tot_struc in cryspy.in from {rin.tot_struc} to {rin.tot_struc + rin.n_pop}')
     rin.tot_struc = rin.tot_struc + rin.n_pop
     # ------ append_struc_ea: True --> False
     change_input.change_option(config, 'append_struc_ea', False)
-    print('Changed append_struc_ea in cryspy.in from {} to {}'.format(
-          True, False))
+    logger.info('Changed append_struc_ea in cryspy.in from True to Flase')
     # ------ write
     change_input.write_config(config)
 
     # ---------- status
     io_stat.set_input_common(stat, 'basic', 'tot_struc', rin.tot_struc)
     io_stat.set_input_common(stat, 'option', 'append_struc_ea', False)
     io_stat.write_stat(stat)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/EA/ea_child.py` & `csp-cryspy-1.2.0/src/cryspy/EA/ea_child.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from logging import getLogger
+
 from .gen_struc_EA.crossover import Crossover
 from .gen_struc_EA.ea_generation import EA_generation
 from .gen_struc_EA.permutation import Permutation
 from .gen_struc_EA.rotation import Rotation
 from .gen_struc_EA.strain import Strain
 from ..IO import pkl_data
 from ..IO import read_input as rin
@@ -9,20 +11,22 @@
 from ..util.struc_util import set_mindist
 
 # ---------- import later
 #from ..RS.gen_struc_RS.gen_pyxtal import Rnd_struc_gen_pyxtal
 #from ..RS.gen_struc_RS.random_generation import Rnd_struc_gen
 
 
+logger = getLogger('cryspy')
+
 def child_gen(sp, init_struc_data, struc_mol_id=None):
     # ---------- instantiate EA_generation class
     eagen = EA_generation(sp=sp, id_start=rin.tot_struc,
                           init_pos_path='./data/init_POSCARS')
     # ---------- set mindist
-    print('# mindist')
+    logger.info('# mindist')
     mindist = set_mindist(rin.mindist, rin.mindist_factor)
     if rin.struc_mode == 'mol_bs':
         mindist_dummy = set_mindist(rin.mindist_mol_bs, rin.mindist_mol_bs_factor)
     # ------ Crossover
     if rin.n_crsov > 0:
         if rin.struc_mode not in ['mol', 'mol_bs']:
             co = Crossover(mindist)
@@ -73,15 +77,15 @@
             # -- molecular crystal
             elif rin.struc_mode == 'mol':
                 rsgx.set_mol()
                 rsgx.gen_struc_mol(nstruc=rin.n_rand, id_offset=eagen.cid,
                                    init_pos_path='./data/init_POSCARS')
             # ------ molecular crystal breaking symmetry
             elif rin.struc_mode == 'mol_bs':
-                print('# -- mindist_mol_bs')
+                logger.info('# -- mindist_mol_bs')
                 mindist_dummy = set_mindist(rin.mindist_mol_bs, rin.mindist_mol_bs_factor, dummy=True)
                 rsgx.set_mol()
                 rsgx.gen_struc_mol_break_sym(nstruc=rin.n_rand,
                                              mindist_dummy=mindist_dummy,
                                              id_offset=eagen.cid,
                                              init_pos_path='./data/init_POSCARS')
             # -- update
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/EA/ea_init.py` & `csp-cryspy-1.2.0/src/cryspy/EA/ea_init.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 '''
 Initialize evolutionary algorithm
 '''
 
+from logging import getLogger
+
 import pandas as pd
 
 from ..IO import out_results
 from ..IO import io_stat, pkl_data
 from ..IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def initialize(stat, rslt_data):
     # ---------- log
-    print('\n# ---------- Initialize evolutionary algorithm')
-    print('# ------ Generation 1')
-    print('{} structures by random\n'.format(rin.tot_struc))
+    logger.info('# ---------- Initialize evolutionary algorithm')
+    logger.info('# ------ Generation 1')
+    logger.info(f'{rin.tot_struc} structures by random')
 
     # ---------- initialize
     gen = 1
     id_queueing = [i for i in range(rin.tot_struc)]
     id_running = []
     # ------ ea_info
     ea_info = pd.DataFrame(columns=['Gen', 'Population',
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/EA/ea_next_gen.py` & `csp-cryspy-1.2.0/src/cryspy/EA/ea_next_gen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 '''
 Generational change in evolutionary algorithm
 '''
 
+from logging import getLogger
+
 import pandas as pd
 
 from .ea_child import child_gen
 from .gen_struc_EA.select_parents import Select_parents
 from ..IO import out_results
 from ..IO import change_input, io_stat, pkl_data
 from ..IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def next_gen(stat, init_struc_data, struc_mol_id, opt_struc_data, rslt_data, ea_id_data):
     # ---------- ea_id_data
     gen, id_queueing, id_running = ea_id_data
 
     # ---------- log
-    print('# ---------- Evolutionary algorithm\n')
-    print('# ------ Generation {}'.format(gen + 1))
+    logger.info('# ---------- Evolutionary algorithm')
+    logger.info(f'# ------ Generation {gen + 1}')
 
     # ---------- current generation
     c_rslt = rslt_data[rslt_data['Gen'] == gen]
     c_fitness = c_rslt['E_eV_atom'].to_dict()    # {ID: energy, ...}
 
     # ---------- load ea_data, ea_data is used only in this module
     elite_struc, elite_fitness, ea_info, ea_origin = pkl_data.load_ea_data()
 
     # ---------- instantiate Seclect_parents class
-    print('# -- select parents')
+    logger.info('# -- select parents')
     sp = Select_parents(opt_struc_data, c_fitness, elite_struc, elite_fitness, rin.n_fittest)
     if rin.slct_func == 'TNM':
         sp.set_tournament()
     else:
         sp.set_roulette()
 
     # ---------- generate offspring by EA
-    print('# -- Generate structures')
+    logger.info('# -- Generate structures')
     if rin.struc_mode not in ['mol', 'mol_bs']:
         _, eagen = child_gen(sp, init_struc_data, None)
     else:
         _, eagen, _ = child_gen(sp, init_struc_data, struc_mol_id)
 
     # ---------- select elite
     if rin.n_elite > 0:
-        print('# -- select elites')
+        logger.info('# -- select elites')
         # ------ init
         all_fitness = rslt_data['E_eV_atom'].to_dict()    # {ID: energy, ..,}
         elite_struc = {}
         elite_fitness = {}
         # ------ Select_parents class also works for selecting elite structures
         se = Select_parents(opt_struc_data, all_fitness, None, None, rin.n_elite)
         for cid in se.ranking_dedupe:
-            print('Structure ID {0:>6} keeps as the elite'.format(cid))
+            logger.info(f'Structure ID {cid:>6} keeps as the elite')
             elite_struc[cid] = opt_struc_data[cid]
             elite_fitness[cid] = all_fitness[cid]
     else:
         elite_struc = None
         elite_fitness = None
 
     # ---------- new generation
@@ -102,18 +106,17 @@
     ea_data = (elite_struc, elite_fitness, ea_info, ea_origin)
     pkl_data.save_ea_data(ea_data)
 
     # ---------- change the value of tot_struc
     config = change_input.config_read()
     change_input.change_basic(config, 'tot_struc', rin.tot_struc + rin.n_pop)
     change_input.write_config(config)
-    print('# -- changed cryspy.in')
-    print('Changed the value of tot_struc in cryspy.in'
-          ' from {} to {}'.format(
-              rin.tot_struc, rin.tot_struc + rin.n_pop))
+    logger.info('# -- changed cryspy.in')
+    logger.info('Changed the value of tot_struc in cryspy.in'
+          f' from {rin.tot_struc} to {rin.tot_struc + rin.n_pop}')
 
     # ---------- status
     io_stat.set_input_common(stat, 'basic', 'tot_struc', rin.tot_struc + rin.n_pop)
     io_stat.set_common(stat, 'generation', gen)
     io_stat.set_id(stat, 'id_queueing', id_queueing)
     io_stat.write_stat(stat)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/crossover.py` & `csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/crossover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 '''
 Crossover class
 '''
 
 from collections import Counter
+from logging import getLogger
 import random
-import sys
 
 import numpy as np
 from pymatgen.core import Structure, Lattice
 from pymatgen.core.periodic_table import DummySpecie
 
 from ...IO import read_input as rin
 from ...util.struc_util import origin_shift, sort_by_atype, check_distance, find_site, cal_g, sort_by_atype_mol
 
 
+logger = getLogger('cryspy')
+
 class Crossover:
     '''
     crossover
 
     # ---------- instance methods
     self.gen_child(struc_A, struc_B)
         if success, return self.child
@@ -30,15 +32,15 @@
 
         # ---------- weight of lattice
         if rin.crs_lat == 'equal':
             self.w_lat = np.array([1.0, 1.0])
         elif rin.crs_lat == 'random':
             self.w_lat = np.random.choice([0.0, 1.0], size=2, replace=False)
         else:
-            raise ValueError('crs_lat must be equal or random')
+            logger.error('crs_lat must be equal or random')
 
     def gen_child(self, struc_A, struc_B):
         '''
         generate child structure
 
         # ---------- return
         (if success) self.child:
@@ -203,15 +205,15 @@
                     self.child.remove_sites([rm_index])
                     self._nat_diff[itype] -= 1
         # ---------- final check
         dist_list = check_distance(self.child, rin.atype,
                                    self.mindist, check_all=True)
         if dist_list:    # still something within mindist
             self.child = None
-            print('some atoms within mindist. retry.', file=sys.stderr, flush=True)
+            logger.warning('some atoms within mindist. retry.')
 
     def _remove_border_line(self):
         # ---------- rank atoms from border line
         coords_axis = self.child.frac_coords[:, self._axis]
         # ------ one point crossover: boundary --> 0.0, slice_point, 1.0
         near_sp = (self._slice_point/2.0 < coords_axis) & \
             (coords_axis < (self._slice_point + 1.0)/2.0)
@@ -252,18 +254,17 @@
                 success, mindist_ij, dist = check_distance(self.child,
                                                            rin.atype,
                                                            self.mindist)
                 if success:
                     cnt = 0    # reset
                     self._nat_diff[i] += 1
                 else:
-                    print('mindist in _add_border_line: {} - {}, {}. retry.'.format(
-                        rin.atype[mindist_ij[0]],
-                        rin.atype[mindist_ij[1]],
-                        dist), file=sys.stderr, flush=True)
+                    type0 = rin.atype[mindist_ij[0]]
+                    type1 = rin.atype[mindist_ij[1]]
+                    logger.warning(f'mindist in _add_border_line: {type0} - {type1}, {dist}. retry.')
                     self.child.pop()    # cancel
                 # ------ fail
                 if cnt == rin.maxcnt_ea:
                     self.child = None
                     return
 
     def _mean_choice(self):
@@ -509,18 +510,17 @@
                 self._rm_dummy.append(DummySpecie("Xx{}".format(i)))
                 self.decide_mol_from_dummy(self.child)
                 success, mindist_ij, dist = self.check_distance_mol(self.child, rin.mindist_mol_ea)
                 if success:
                     cnt = 0    # reset
                     self._nmol_diff[i] += 1
                 else:
-                    sys.stderr.write('mindist in _add_border_line: {} - {}, {}. retry.\n'.format(
-                        rin.atype[mindist_ij[0]],
-                        rin.atype[mindist_ij[1]],
-                        dist))
+                    type0 = rin.atype[mindist_ij[0]]
+                    type1 = rin.atype[mindist_ij[1]]
+                    logger.warning(f'mindist in _add_border_line: {type0} - {type1}, {dist}. retry.')
                     self.child.pop()    # cancel
                 # ------ fail
                 if cnt == rin.maxcnt_ea:
                     self.child = None
                     return
 
     def replace_mol(self, struc):
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/ea_generation.py` & `csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/ea_generation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 '''
 Structure generation by evolutionary algorithm
 '''
 
+from logging import getLogger
+
 from ...IO import read_input as rin
 from ...util.struc_util import out_poscar
 
 
+logger = getLogger('cryspy')
+
 class EA_generation:
     '''
     generate structures by evolutionary algorithm
 
     # ---------- args
     sp: instance of Select_parents class
     id_start (int or None): starting id
@@ -29,26 +33,26 @@
         # ---------- check args
         self.sp = sp
         # ------ id_offset
         if id_start is None:
             self.cid = max(sp.fitness.keys()) + 1
         elif isinstance(id_start, int):
             if id_start < (max(sp.fitness.keys()) + 1):
-                raise ValueError('id_start is already included'
+                logger.error('id_start is already included'
                                  ' structure ID of the data')
             else:
                 self.cid = id_start
         else:
-            raise TypeError('id_start must be int or None')
+            logger.error('id_start must be int or None')
         # ------ init_pos_path
         if init_pos_path is not None:
             if isinstance(init_pos_path, str):
                 self.init_pos_path = init_pos_path
             else:
-                raise TypeError('init_pos_path must be str or None')
+                logger.error('init_pos_path must be str or None')
         # ---------- initialize data
         self.offspring = {}    # structure data
         self.offspring_mol_id = {}
         self.parents = {}    # tuple of parents ID
         self.operation = {}
 
     def gen_crossover(self, co, struc_mol_id, molecular=False):
@@ -79,18 +83,17 @@
                 self.operation[self.cid] = 'crossover'
                 try:
                     spg_sym, spg_num = child.get_space_group_info(
                         symprec=rin.symprec)
                 except TypeError:
                     spg_num = 0
                     spg_sym = None
-                print('Structure ID {0:>6} was generated'
-                      ' from {1:>6} and {2:>6} by crossover.'
-                      ' Space group: {3:>3} {4}'.format(self.cid, pid_A, pid_B,
-                                                        spg_num, spg_sym), flush=True)
+                logger.info(f'Structure ID {self.cid:>6} was generated'
+                      f' from {pid_A:>6} and {pid_B:>6} by crossover.'
+                      f' Space group: {spg_num:>3} {spg_sym}')
                 if self.init_pos_path is not None:
                     out_poscar(child, self.cid, self.init_pos_path)
                 self.cid += 1
                 struc_cnt += 1
 
     def gen_permutation(self, pm, struc_mol_id, molecular=False):
         '''
@@ -118,18 +121,17 @@
                 self.operation[self.cid] = 'permutation'
                 try:
                     spg_sym, spg_num = child.get_space_group_info(
                         symprec=rin.symprec)
                 except TypeError:
                     spg_num = 0
                     spg_sym = None
-                print('Structure ID {0:>6} was generated'
-                      ' from {1:>6} by permutation.'
-                      ' Space group: {2:>3} {3}'.format(self.cid, pid,
-                                                        spg_num, spg_sym), flush=True)
+                logger.info(f'Structure ID {self.cid:>6} was generated'
+                      f' from {pid:>6} by permutation.'
+                      f' Space group: {spg_num:>3} {spg_sym}')
                 if self.init_pos_path is not None:
                     out_poscar(child, self.cid, self.init_pos_path)
                 self.cid += 1
                 struc_cnt += 1
 
     def gen_strain(self, st, struc_mol_id, molecular=False, protect_mol_struc=True):
         '''
@@ -161,18 +163,17 @@
                 self.operation[self.cid] = 'strain'
                 try:
                     spg_sym, spg_num = child.get_space_group_info(
                         symprec=rin.symprec)
                 except TypeError:
                     spg_num = 0
                     spg_sym = None
-                print('Structure ID {0:>6} was generated'
-                      ' from {1:>6} by strain.'
-                      ' Space group: {2:>3} {3}'.format(self.cid, pid,
-                                                        spg_num, spg_sym), flush=True)
+                logger.info(f'Structure ID {self.cid:>6} was generated'
+                      f' from {pid:>6} by strain.'
+                      f' Space group: {spg_num:>3} {spg_sym}')
                 if self.init_pos_path is not None:
                     out_poscar(child, self.cid, self.init_pos_path)
                 self.cid += 1
                 struc_cnt += 1
 
     def gen_rotation(self, struc_mol_id, rot):
         '''
@@ -196,15 +197,14 @@
                 self.parents[self.cid] = (pid, )    # tuple
                 self.operation[self.cid] = 'rotation'
                 try:
                     spg_sym, spg_num = child.get_space_group_info(symprec=rin.symprec)
                 except TypeError:
                     spg_num = 0
                     spg_sym = None
-                print('Structure ID {0:>6} was generated'
-                      ' from {1:>6} by rotation.'
-                      ' Space group: {2:>3} {3}'.format(self.cid, pid,
-                                                        spg_num, spg_sym), flush=True)
+                logger.info(f'Structure ID {self.cid:>6} was generated'
+                      f' from {pid:>6} by rotation.'
+                      f' Space group: {spg_num:>3} {spg_sym}')
                 if self.init_pos_path is not None:
                     out_poscar(child, self.cid, self.init_pos_path)
                 self.cid += 1
                 struc_cnt += 1
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/permutation.py` & `csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/permutation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 '''
 Permutaion class
 '''
 
+from logging import getLogger
 import sys
 
 import numpy as np
 from pymatgen.analysis.structure_matcher import StructureMatcher
 from pymatgen.core import Structure
 
 from ...IO import read_input as rin
 from ...util.struc_util import sort_by_atype, check_distance, cal_g, sort_by_atype_mol, find_site
 
 
+logger = getLogger('cryspy')
+
 class Permutation:
     '''
     permutation
 
     # ---------- args
     ntimes (int): ntimes permutaion
 
@@ -74,23 +77,22 @@
             success, mindist_ij, dist = check_distance(self.child,
                                                        rin.atype,
                                                        self.mindist)
             if success:
                 self.child = sort_by_atype(self.child, rin.atype)
                 return self.child
             else:
-                print('mindist in permutation: {} - {}, {}. retry.'.format(
-                    rin.atype[mindist_ij[0]],
-                    rin.atype[mindist_ij[1]],
-                    dist), file=sys.stderr, flush=True)
+                type0 = rin.atype[mindist_ij[0]]
+                type1 = rin.atype[mindist_ij[1]]
+                logger.warning(f'mindist in permutation: {type0} - {type1}, {dist}. retry.')
                 cnt += 1
                 if cnt >= rin.maxcnt_ea:
-                    print('Permutatin: could not satisfy min_dist' +
-                          ' in {} times'.format(rin.maxcnt_ea), file=sys.stderr)
-                    print('Change parent', file=sys.stderr, flush=True)
+                    logger.warning('Permutatin: could not satisfy min_dist' +
+                          f' in {rin.maxcnt_ea} times')
+                    logger.warning('Change parent')
                     self.child = None
                     return None    # change parent
 
     def gen_child_mol(self, struc, mol_id):
         '''
         generate child structures for mol
 
@@ -164,23 +166,22 @@
             if success:
                 self.child, self.mol_id, self.group_id = sort_by_atype_mol(self.child,
                                                                            rin.atype,
                                                                            self.mol_id,
                                                                            self.group_id)
                 return self.child, [self.mol_id, self.group_id, self.true_dists]
             else:
-                print('mindist in permutation: {} - {}, {}. retry.'.format(
-                    rin.atype[mindist_ij[0]],
-                    rin.atype[mindist_ij[1]],
-                    dist), file=sys.stderr, flush=True)
+                type0 = rin.atype[mindist_ij[0]]
+                type1 = rin.atype[mindist_ij[1]]
+                logger.warning(f'mindist in permutation: {type0} - {type1}, {dist}. retry.')
                 cnt += 1
                 if cnt >= rin.maxcnt_ea:
-                    print('Permutatin: could not satisfy min_dist' +
-                          ' in {} times'.format(rin.maxcnt_ea), file=sys.stderr)
-                    print('Change parent', file=sys.stderr, flush=True)
+                    logger.warning('Permutatin: could not satisfy min_dist' +
+                          f' in {rin.maxcnt_ea} times')
+                    logger.warning('Change parent')
                     self.child = None
                     return None    # change parent
 
     def check_mol_diff(self, mol_choice, mol_id, group_id):
         # ---------- check_mol_choice[0] and the mol_id
         for i, gid in enumerate(group_id):
             if gid == mol_choice[0]:
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/rotation.py` & `csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/rotation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 '''
 Rotation class
 '''
 
+from logging import getLogger
 import sys
 
 import numpy as np
 from pymatgen.core import Structure
 
 from ...IO import read_input as rin
 from ...util.struc_util import check_distance, rot_mat, find_site, cal_g, sort_by_atype_mol
 
 
+logger = getLogger('cryspy')
+
 class Rotation:
     '''
     rotation
     '''
 
     def __init__(self, mindist):
         self.mindist = mindist
@@ -52,18 +55,17 @@
                                                        rin.atype,
                                                        self.mindist)
             if success:
                 self.child, self.mol_id, self.group_id = sort_by_atype_mol(self.child, rin.atype,
                                                                            mol_id[0], rotated_group_id)
                 return self.child, [self.mol_id, self.group_id, mol_id[2]]
             else:
-                print('mindist in rotation: {} - {}, {}. retry.'.format(
-                    rin.atype[mindist_ij[0]],
-                    rin.atype[mindist_ij[1]],
-                    dist), file=sys.stderr, flush=True)
+                type0 = rin.atype[mindist_ij[0]]
+                type1 = rin.atype[mindist_ij[1]]
+                logger.warning(f'mindist in rotation: {type0} - {type1}, {dist}. retry.')
                 cnt += 1
                 if cnt >= rin.maxcnt_ea:
-                    print('Rotation: could not satisfy min_dist' +
-                          ' in {} times'.format(rin.maxcnt_ea), file=sys.stderr)
-                    print('Change parent', file=sys.stderr, flush=True)
+                    logger.warning('Rotation: could not satisfy min_dist' +
+                          f' in {rin.maxcnt_ea} times')
+                    logger.warning('Change parent')
                     self.child = None
                     return None, None    # change parent
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/select_parents.py` & `csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/select_parents.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 '''
 Select parents in evolutionary algorithm
 '''
 
+from logging import getLogger
+
 import numpy as np
 from pymatgen.analysis.structure_matcher import StructureMatcher
 
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 class Select_parents:
     '''
     select parents
 
     # ---------- args
     struc_data (dict or list): structure data
         You may include None in struc_data
@@ -53,22 +57,20 @@
         for key, value in self.fitness.items():
             if value is None or np.isnan(value):
                 self.fitness[key] = -np.inf if rin.fit_reverse else np.inf
             # ---- emax_ea
             if rin.emax_ea is not None:
                 if value > rin.emax_ea:
                     self.fitness[key] = -np.inf if rin.fit_reverse else np.inf
-                    print('Eliminate ID {}: {} > emax_ea'.format(
-                          key, value))
+                    logger.info(f'Eliminate ID {key}: {value} > emax_ea')
             # ---- emin_ea
             if rin.emin_ea is not None:
                 if value < rin.emin_ea:
                     self.fitness[key] = -np.inf if rin.fit_reverse else np.inf
-                    print('Eliminate ID {}: {} < emin_ea'.format(
-                          key, value))
+                    logger.info(f'Eliminate ID {key}: {value} < emin_ea')
         # ------ self
         self.n_fittest = n_fittest
         # ---------- ranking of fitness: list of id
         self.ranking = sorted(self.fitness, key=self.fitness.get,
                               reverse=rin.fit_reverse)
         #print('ranking', self.ranking)
         # ---------- remove duplicated structures and
@@ -77,48 +79,48 @@
 
     def _check_data(self, struc_data, fitness, elite_struc, elite_fitness):
         # ---------- struc_data and fitness
         if isinstance(struc_data, dict) and isinstance(fitness, dict):
             pass    # if dict, allow len(struc_data) != len(fitness)
         elif isinstance(struc_data, dict) and (
                 isinstance(fitness, list) or isinstance(fitness, np.ndarray)):
-            raise TypeError('struc_data is dict,'
+            logger.error('struc_data is dict,'
                             ' so fitness should also be dict')
         elif isinstance(fitness, dict) and (
                 isinstance(struc_data, list)
                 or isinstance(struc_data, np.ndarray)):
-            raise TypeError('fitness is dict,'
+            logger.error('fitness is dict,'
                             ' so struc_data should also be dict')
         elif isinstance(struc_data, list) and (
                 isinstance(fitness, list) or isinstance(fitness, np.ndarray)):
             # ------ check number of data
             if not len(struc_data) == len(fitness):
-                raise ValueError('not len(struc_data) == len(fitness)')
+                logger.error('not len(struc_data) == len(fitness)')
             # ------ convert
             struc_data = {i: struc_data[i] for i in range(len(struc_data))}
             fitness = {i: fitness[i] for i in range(len(fitness))}
         else:
-            raise TypeError('Type of struc_data and fitness is wrong')
+            logger.error('Type of struc_data and fitness is wrong')
         # ---------- elite
         if isinstance(elite_struc, dict) and isinstance(elite_fitness, dict):
             # ------ check number of data
             if not len(elite_struc) == len(elite_fitness):
-                raise ValueError('not len(elite_struc) == len(elite_fitness)')
+                logger.error('not len(elite_struc) == len(elite_fitness)')
             if None in elite_struc.values():
-                raise ValueError('elite_struc includes None')
+                logger.error('elite_struc includes None')
             if (None in elite_fitness.values()) or (
                     np.nan in elite_fitness.values()):
-                raise ValueError('elite_fitness includes None or np.nan')
+                logger.error('elite_fitness includes None or np.nan')
             # ------ add elite to data
             struc_data.update(elite_struc)
             fitness.update(elite_fitness)
         elif elite_struc is elite_fitness is None:
             pass
         else:
-            raise TypeError('elite_struc and elite_fitness'
+            logger.error('elite_struc and elite_fitness'
                             ' must be dict or None')
         # ---------- return
         return struc_data, fitness
 
     def _dedupe(self):
         # ---------- remove duplicated structure data
         # ------ initialize
@@ -143,18 +145,17 @@
             else:
                 self.ranking_dedupe.append(i_id)
                 # n_fittest
                 if self.n_fittest > 0:
                     if len(self.ranking_dedupe) == self.n_fittest:
                         break
         # ---------- log
-        print('Remove duplicated data')
+        logger.info('Remove duplicated data')
         if self.n_fittest > 0:
-            print('Survival of the fittest: top {0} structures survive'.format(
-                self.n_fittest))
+            logger.info(f'Survival of the fittest: top {self.n_fittest} structures survive')
 
     def set_tournament(self):
         '''
         setting for tournament selection
         '''
         # ---------- set self.get_parents() <-- self._tournament or self._roulette
         self.get_parents = self._tournament
@@ -218,15 +219,15 @@
         # ---------- check args
         # ------ fitness
         if isinstance(fitness, np.ndarray):
             pass
         elif isinstance(fitness, list):
             fitness = np.array(fitness)
         else:
-            raise TypeError('fitness must be list or np.array')
+            logger.error('fitness must be list or np.array')
         # ------ in case of int
         a = float(rin.a_rlt)
         b = float(rin.b_rlt)
         # ---------- for fit_reverse
         if not rin.fit_reverse:
             fitness = -fitness
         # ---------- scaling
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/EA/gen_struc_EA/strain.py` & `csp-cryspy-1.2.0/src/cryspy/EA/gen_struc_EA/strain.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 '''
 Strain class
 '''
+from logging import getLogger
 import sys
 
 import numpy as np
 from pymatgen.core import Structure
 from pymatgen.core.periodic_table import DummySpecie
 
 from ...IO import read_input as rin
 from ...util.struc_util import sort_by_atype, sort_by_atype_mol, check_distance, cal_g, find_site
 
 
+logger = getLogger('cryspy')
+
 class Strain:
     '''
     strain
 
     # ---------- instance methods
     gen_child(self, struc)
     '''
@@ -58,18 +61,17 @@
             success, mindist_ij, dist = check_distance(self.child,
                                                        rin.atype,
                                                        self.mindist)
             if success:
                 self.child = sort_by_atype(self.child, rin.atype)
                 return self.child
             else:
-                print('mindist in strain: {} - {}, {}. retry.'.format(
-                    rin.atype[mindist_ij[0]],
-                    rin.atype[mindist_ij[1]],
-                    dist), file=sys.stderr, flush=True)
+                type0 = rin.atype[mindist_ij[0]]
+                type1 = rin.atype[mindist_ij[1]]
+                logger.warning(f'mindist in strain: {type0} - {type1}, {dist}. retry.')
                 cnt += 1
                 if cnt >= rin.maxcnt_ea:
                     self.child = None
                     return None    # change parent
 
     def gen_child_mol(self, struc, mol_id):
         '''
@@ -139,15 +141,14 @@
                                                        rin.atype,
                                                        self.mindist)
             if success:
                 self.child, self.mol_id, self.group_id = sort_by_atype_mol(self.child, rin.atype,
                                                                            strained_mol_id, strained_group_id)
                 return self.child, [self.mol_id, self.group_id, mol_id[2]]
             else:
-                print('mindist in permutation: {} - {}, {}. retry.'.format(
-                    rin.atype[mindist_ij[0]],
-                    rin.atype[mindist_ij[1]],
-                    dist), file=sys.stderr, flush=True)
+                type0 = rin.atype[mindist_ij[0]]
+                type1 = rin.atype[mindist_ij[1]]
+                logger.warning(f'mindist in permutation: {type0} - {type1}, {dist}. retry.')
                 cnt += 1
                 if cnt >= rin.maxcnt_ea:
                     self.child = None
                     return None    # change parent
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/IO/io_stat.py` & `csp-cryspy-1.2.0/src/cryspy/IO/io_stat.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,31 +45,30 @@
 def write_stat(stat):
     with open('cryspy.stat', 'w') as f:
         stat.write(f)
 
 
 # ---------- input section
 def set_input_common(stat, sec, var_str, var):
-    stat.set(sec, var_str, '{}'.format(var))
+    stat.set(sec, var_str, f'{var}')
 
 
 # ---------- status section
 def set_common(stat, var_str, var):
-    stat.set('status', var_str, '{}'.format(var))
+    stat.set('status', var_str, f'{var}')
 
 
 def set_id(stat, var_str, var_list):
     if len(var_list) > 30:
-        stat.set('status', var_str, '{0} ... total {1} IDs'.format(
-            ' '.join(str(a) for a in var_list[:5]), len(var_list)))
+        vl = ' '.join(str(a) for a in var_list[:5])
+        stat.set('status', var_str, f'{vl} ... total {len(var_list)} IDs')
     else:
-        stat.set('status', var_str, '{}'.format(
-            ' '.join(str(a) for a in var_list)))
+        vl = ' '.join(str(a) for a in var_list)
+        stat.set('status', var_str, f'{vl}')
 
 
 def set_stage(stat, current_id, current_stage):
-    stat.set('status', 'ID {:>6}'.format(current_id), 'Stage {}'.format(
-        current_stage))
+    stat.set('status', f'ID {current_id:>6}', f'Stage {current_stage}')
 
 
 def clean_id(stat, current_id):
-    stat.remove_option('status', 'ID {:>6}'.format(current_id))
+    stat.remove_option('status', f'ID {current_id:>6}')
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/IO/out_results.py` & `csp-cryspy-1.2.0/src/cryspy/IO/out_results.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.1/src/cryspy/IO/pkl_data.py` & `csp-cryspy-1.2.0/src/cryspy/IO/pkl_data.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.1/src/cryspy/IO/read_input.py` & `csp-cryspy-1.2.0/src/cryspy/IO/read_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,63 @@
 '''
 Read input from cryspy.in
 '''
 
 import configparser
+from logging import getLogger
 import os
 
 from . import io_stat
 from ..util import utility
 
 
+logger = getLogger('cryspy')
+
 def readin():
     # ---------- read cryspy.in
     if not os.path.isfile('cryspy.in'):
-        raise IOError('Could not find cryspy.in file')
+        logger.error('Could not find cryspy.in file')
+        raise SystemExit(1)
     config = configparser.ConfigParser()
     config.read('cryspy.in')
 
     # ---------- basic
     # ------ global declaration
     global algo, calc_code, tot_struc
     global nstage, njob, jobcmd, jobfile
     # ------ read intput variables
     calc_code = config.get('basic', 'calc_code')
     if calc_code not in ['VASP', 'QE', 'soiap', 'LAMMPS', 'OMX', 'ASE', 'ext']:
-        raise NotImplementedError(
-            'calc_code must be VASP, QE, OMX, soiap, LAMMPS, ASE, or ext')
+        logger.error('calc_code must be VASP, QE, OMX, soiap, LAMMPS, ASE, or ext')
+        raise SystemExit(1)
     algo = config.get('basic', 'algo')
     if algo not in ['RS', 'BO', 'LAQA', 'EA']:
-        raise NotImplementedError('algo must be RS, BO, LAQA, or EA')
+        logger.error('algo must be RS, BO, LAQA, or EA')
+        raise SystemExit(1)
     if algo == 'LAQA':
         if calc_code not in ['VASP', 'QE', 'soiap']:
-            raise NotImplementedError('LAQA: only VASP, QE, and soiap for now')
+            logger.error('LAQA: only VASP, QE, and soiap for now')
+            raise SystemExit(1)
     tot_struc = config.getint('basic', 'tot_struc')
     if tot_struc <= 0:
-        raise ValueError('tot_struc <= 0, check tot_struc')
+        logger.error('tot_struc <= 0, check tot_struc')
+        raise SystemExit(1)
     if not calc_code == 'ext':
         nstage = config.getint('basic', 'nstage')
         if nstage <= 0:
-            raise ValueError('nstage <= 0, check nstage')
+            logger.error('nstage <= 0, check nstage')
+            raise SystemExit(1)
         if algo == 'LAQA':
             if not nstage == 1:
-                raise ValueError('nstage shoud be 1 in LAQA')
+                logger.error('nstage shoud be 1 in LAQA')
+                raise SystemExit(1)
         njob = config.getint('basic', 'njob')
         if njob <= 0:
-            raise ValueError('njob <= 0, check njob')
+            logger.error('njob <= 0, check njob')
+            raise SystemExit(1)
         jobcmd = config.get('basic', 'jobcmd')
         jobfile = config.get('basic', 'jobfile')
 
     # ---------- structure
     # ------ global declaration
     global struc_mode, natot, atype, nat
     global mol_file, nmol, timeout_mol, rot_mol, nrot
@@ -58,58 +68,67 @@
 
     # ------ read intput variables
     try:
         struc_mode = config.get('structure', 'struc_mode')
     except (configparser.NoOptionError, configparser.NoSectionError):
         struc_mode = 'crystal'
     if struc_mode not in ['crystal', 'mol', 'mol_bs', 'host']:
-        raise ValueError('struc_mode is wrong')
+        logger.error('struc_mode is wrong')
+        raise SystemExit(1)
     if algo == 'EA' and struc_mode in ['mol', 'mol_bs']:
         if calc_code == 'ext':
-            raise NotImplementedError('EA, mol or mol_bs, ext, not yet')
+            logger.error('EA, mol or mol_bs, ext, not yet')
+            raise SystemExit(1)
     natot = config.getint('structure', 'natot')
     if natot <= 0:
-        raise ValueError('natot <= 0, check natot')
+        logger.error('natot <= 0, check natot')
+        raise SystemExit(1)
     atype = config.get('structure', 'atype')
     atype = [a for a in atype.split()]    # list
     nat = config.get('structure', 'nat')
     nat = [int(x) for x in nat.split()]    # character --> integer
     if not len(nat) == len(atype):
-        raise ValueError('not len(nat) == len(atype), check atype and nat')
+        logger.error('not len(nat) == len(atype), check atype and nat')
+        raise SystemExit(1)
     if not sum(nat) == natot:
-        raise ValueError('not sum(nat) == natot, check natot and nat')
+        logger.error('not sum(nat) == natot, check natot and nat')
+        raise SystemExit(1)
     # -- mol
     if struc_mode in ['mol', 'mol_bs']:
         mol_file = config.get('structure', 'mol_file')
         mol_file = [a for a in mol_file.split()]    # list
         nmol = config.get('structure', 'nmol')
         nmol = [int(x) for x in nmol.split()]    # character --> integer
         if not len(mol_file) == len(nmol):
-            raise ValueError('not len(mol_file) == len(nmol)')
+            logger.error('not len(mol_file) == len(nmol)')
+            raise SystemExit(1)
         try:
             timeout_mol = config.getfloat('structure', 'timeout_mol')
         except (configparser.NoOptionError, configparser.NoSectionError):
             timeout_mol = 120.0
         if timeout_mol <= 0:
-            raise ValueError('timeout_mol must be positive')
+            logger.error('timeout_mol must be positive')
+            raise SystemExit(1)
         if struc_mode == 'mol_bs':
             # rot_mol
             try:
                 rot_mol = config.get('structure', 'rot_mol')
             except (configparser.NoOptionError, configparser.NoSectionError):
                 rot_mol = 'random_wyckoff'
             if rot_mol not in ['random', 'random_mol', 'random_wyckoff']:
-                raise ValueError('rot_mol is wrong')
+                logger.error('rot_mol is wrong')
+                raise SystemExit(1)
             # nrot
             try:
                 nrot = config.getint('structure', 'nrot')
             except (configparser.NoOptionError, configparser.NoSectionError):
                 nrot = 20
             if nrot <= 0:
-                raise ValueError('nrot <=0, check nrot')
+                logger.error('nrot <=0, check nrot')
+                raise SystemExit(1)
         else:
             rot_mol = None
             nrot = None
     else:
         mol_file = None
         nmol = None
         timeout_mol = 120.0
@@ -118,128 +137,139 @@
     # -- volume
     try:
         vol_mu = config.getfloat('structure', 'vol_mu')
     except (configparser.NoOptionError, configparser.NoSectionError):
         vol_mu = None
     if vol_mu is not None:
         if vol_mu <= 0.0:
-            raise ValueError('vol_mu must be positive float')
+            logger.error('vol_mu must be positive float')
+            raise SystemExit(1)
     try:
         vol_sigma = config.getfloat('structure', 'vol_sigma')
     except (configparser.NoOptionError, configparser.NoSectionError):
         vol_sigma = None
     if vol_mu is not None:
         if vol_sigma is None:
-            raise ValueError("check vol_mu: {} and vol_sigma: {}".format(
-                vol_mu, vol_sigma))
+            logger.error(f'check vol_mu: {vol_mu} and vol_sigma: {vol_sigma}')
+            raise SystemExit(1)
     if vol_sigma is not None:
         if vol_sigma < 0.0:
-            raise ValueError('vol_sigma must not be negative')
+            logger.error('vol_sigma must not be negative')
+            raise SystemExit(1)
     try:
         vol_factor = config.get('structure', 'vol_factor')
         vol_factor = [float(x) for x in vol_factor.split()]    # char --> float
         if vol_factor[0] <= 0.0:
-            raise ValueError('vol_factor must be positive')
+            logger.error('vol_factor must be positive')
+            raise SystemExit(1)
         if len(vol_factor) == 1:
             vol_factor = vol_factor * 2    # [0.8] --> [0.8, 0.8]
         if len(vol_factor) == 2:
             if vol_factor[0] > vol_factor[1]:
-                raise ValueError('check: vol_factor[0] < vol_factor[1]')
+                logger.error('check: vol_factor[0] < vol_factor[1]')
+                raise SystemExit(1)
         else:
-            raise ValueError('len(vol_factor) must be 1 or 2')
+            logger.error('len(vol_factor) must be 1 or 2')
+            raise SystemExit(1)
     except (configparser.NoOptionError, configparser.NoSectionError):
         vol_factor = [1.1, 1.1]
     try:
         maxcnt = config.getint('structure', 'maxcnt')
     except (configparser.NoOptionError, configparser.NoSectionError):
         maxcnt = 50
     if maxcnt < 0:
-        raise ValueError('maxcnt must be positive int')
+        logger.error('maxcnt must be positive int')
+        raise SystemExit(1)
     try:
         symprec = config.getfloat('structure', 'symprec')
     except (configparser.NoOptionError, configparser.NoSectionError):
         symprec = 0.01
     if symprec < 0.0:
-        raise ValueError('symprec must be positive float')
+        logger.error('symprec must be positive float')
+        raise SystemExit(1)
     try:
         spgnum = config.get('structure', 'spgnum')
     except (configparser.NoOptionError, configparser.NoSectionError):
         spgnum = 'all'
     if spgnum == '0':
         if struc_mode in ['mol', 'mol_bs']:
-            raise ValueError('spgnum = 0 is not allow when struc_mode is mol or mol_bs')
+            logger.error('spgnum = 0 is not allow when struc_mode is mol or mol_bs')
+            raise SystemExit(1)
         spgnum = 0
     elif spgnum == 'all':
         pass
     else:
         spgnum = _spglist(spgnum)
     try:
         use_find_wy = config.getboolean('structure', 'use_find_wy')
     except (configparser.NoOptionError, configparser.NoSectionError):
         use_find_wy = False
     if use_find_wy:
         if not struc_mode == 'crystal':
-            raise ValueError('find_wy can be use if struc_mode is crystal')
+            logger.error('find_wy can be use if struc_mode is crystal')
+            raise SystemExit(1)
     try:
         fwpath = config.get('structure', 'fwpath')
     except (configparser.NoOptionError, configparser.NoSectionError):
         fwpath = None
     # ------ mindist
     try:
         mindist = []
         for i in range(len(atype)):
-            tmp = config.get('structure', 'mindist_{}'.format(i+1))
+            tmp = config.get('structure', f'mindist_{i+1}')
             tmp = [float(x) for x in tmp.split()]    # character --> float
             if not len(tmp) == len(atype):
-                raise ValueError('not len(mindist_{}) == len(atype)'.format(i+1))
+                logger.error(f'not len(mindist_{i+1}) == len(atype)')
+                raise SystemExit(1)
             mindist.append(tmp)
         # -- check symmetric matrix
         for i in range(len(mindist)):
             for j in range(len(mindist)):
                 if i < j:
                     if not mindist[i][j] == mindist[j][i]:
-                        raise ValueError('mindist is not symmetric. ({}, {}) -->'
-                                         ' {}, ({}, {}) --> {}'.format(
-                                             i, j, mindist[i][j],
-                                             j, i, mindist[j][i]))
+                        logger.error(f'mindist is not symmetric. ({i}, {j}) -->'
+                                         f' {mindist[i][j]}, ({j}, {i}) --> {mindist[j][i]}')
+                        raise SystemExit(1)
     except (configparser.NoOptionError, configparser.NoSectionError):
         mindist = None
     # ------ mindist_factor
     try:
         mindist_factor = config.getfloat('structure', 'mindist_factor')
         if mindist_factor <= 0.0:
-            raise ValueError('mindist_factor must be positive')
+            logger.error('mindist_factor must be positive')
+            raise SystemExit(1)
     except (configparser.NoOptionError, configparser.NoSectionError):
         mindist_factor = 1.0
     # ------ mindist_mol_bs
     if struc_mode == 'mol_bs':
         try:
             mindist_mol_bs = []
             for i in range(len(mol_file)):
-                tmp = config.get('structure', 'mindist_mol_bs_{}'.format(i+1))
+                tmp = config.get('structure', f'mindist_mol_bs_{i+1}')
                 tmp = [float(x) for x in tmp.split()]    # character --> float
                 if not len(tmp) == len(mol_file):
-                    raise ValueError('not len(mindist_mol_bs_{}) == len(mol_file)'.format(i+1))
+                    logger.error(f'not len(mindist_mol_bs_{i+1}) == len(mol_file)')
+                    raise SystemExit(1)
                 mindist_mol_bs.append(tmp)
             # -- check symmetric matrix
             for i in range(len(mindist_mol_bs)):
                 for j in range(len(mindist_mol_bs)):
                     if i < j:
                         if not mindist_mol_bs[i][j] == mindist_mol_bs[j][i]:
-                            raise ValueError('mindist_mol_bs is not symmetric. ({}, {}) -->'
-                                             ' {}, ({}, {}) --> {}'.format(
-                                                 i, j, mindist_mol_bs[i][j],
-                                                 j, i, mindist_mol_bs[j][i]))
+                            logger.error(f'mindist_mol_bs is not symmetric. ({i}, {j}) -->'
+                                             f' {mindist_mol_bs[i][j]}, ({j}, {i}) --> {mindist_mol_bs[j][i]}')
+                            raise SystemExit(1)
         except (configparser.NoOptionError, configparser.NoSectionError):
             mindist_mol_bs = None
         # ------ mindist_mol_bs_factor
         try:
             mindist_mol_bs_factor = config.getfloat('structure', 'mindist_mol_bs_factor')
             if mindist_mol_bs_factor <= 0.0:
-                raise ValueError('mindist_mol_bs_factor must be positive')
+                logger.error('mindist_mol_bs_factor must be positive')
+                raise SystemExit(1)
         except (configparser.NoOptionError, configparser.NoSectionError):
             mindist_mol_bs_factor = 1.0
     else:
         mindist_mol_bs = None
         mindist_mol_bs_factor = 1.0
     # ------ spgnum == 0 or use_find_wy
     minlen = None
@@ -247,19 +277,22 @@
     dangle = None
     if spgnum == 0 or use_find_wy:
         # -- read input variables
         minlen = config.getfloat('structure', 'minlen')
         maxlen = config.getfloat('structure', 'maxlen')
         dangle = config.getfloat('structure', 'dangle')
         if minlen <= 0.0:
-            raise ValueError('minlen must be positive')
+            logger.error('minlen must be positive')
+            raise SystemExit(1)
         if minlen > maxlen:
-            raise ValueError('minlen > maxlen')
+            logger.error('minlen > maxlen')
+            raise SystemExit(1)
         if dangle <= 0.0:
-            raise ValueError('dangle < 0.0, dangle must be positive')
+            logger.error('dangle < 0.0, dangle must be positive')
+            raise SystemExit(1)
 
     # ---------- option
     # ------ global declaration
     global stop_chkpt
     global load_struc_flag, stop_next_struc, recalc
     global append_struc_ea
     global energy_step_flag, struc_step_flag
@@ -282,66 +315,74 @@
         recalc = config.get('option', 'recalc')
         recalc = [int(x) for x in recalc.split()]    # character --> integer
     except (configparser.NoOptionError, configparser.NoSectionError):
         recalc = []
     if recalc:
         for i in recalc:
             if not 0 <= i < tot_struc:
-                raise ValueError('recalc must be non-negative int'
+                logger.error('recalc must be non-negative int'
                                  ' and less than tot_struc')
+                raise SystemExit(1)
     try:
         append_struc_ea = config.getboolean('option', 'append_struc_ea')
     except (configparser.NoOptionError, configparser.NoSectionError):
         append_struc_ea = False
     try:
         energy_step_flag = config.getboolean('option', 'energy_step_flag')
         if calc_code in ['LAMMPS', 'OMX', 'ASE', 'ext']:
-            raise NotImplementedError('energy_step_flag: only VASP, QE, and soiap for now')
+            logger.error('energy_step_flag: only VASP, QE, and soiap for now')
+            raise SystemExit(1)
     except (configparser.NoOptionError, configparser.NoSectionError):
         energy_step_flag = False
     try:
         struc_step_flag = config.getboolean('option', 'struc_step_flag')
         if calc_code in ['LAMMPS', 'OMX', 'ASE', 'ext']:
-            raise NotImplementedError('struc_step_flag: only VASP, QE, and soiap for now')
+            logger.error('struc_step_flag: only VASP, QE, and soiap for now')
+            raise SystemExit(1)
     except (configparser.NoOptionError, configparser.NoSectionError):
         struc_step_flag = False
     try:
         force_step_flag = config.getboolean('option', 'force_step_flag')
         if calc_code in ['LAMMPS', 'OMX', 'ASE', 'ext']:
-            raise NotImplementedError('force_step_flag: only VASP, QE, and soiap for now')
+            logger.error('force_step_flag: only VASP, QE, and soiap for now')
+            raise SystemExit(1)
     except (configparser.NoOptionError, configparser.NoSectionError):
         force_step_flag = False
     if algo == 'LAQA':
         force_step_flag = True
     try:
         stress_step_flag = config.getboolean('option', 'stress_step_flag')
         if calc_code in ['LAMMPS', 'OMX', 'ASE', 'ext']:
-            raise NotImplementedError('stress_step_flag: only VASP, QE, and soiap for now')
+            logger.error('stress_step_flag: only VASP, QE, and soiap for now')
+            raise SystemExit(1)
     except (configparser.NoOptionError, configparser.NoSectionError):
         stress_step_flag = False
     if algo == 'LAQA':
         stress_step_flag = True
 
     # ---------- BO
     if algo == 'BO':
         # ------ global declaration
         global nselect_bo, score, num_rand_basis, cdev, dscrpt
         global fppath, fp_rmin, fp_rmax, fp_npoints, fp_sigma
         global max_select_bo, manual_select_bo, emax_bo, emin_bo
         # ------ read intput variables
         nselect_bo = config.getint('BO', 'nselect_bo')
         if nselect_bo <= 0:
-            raise ValueError('nselect_bo <= 0, check nselect_bo')
+            logger.error('nselect_bo <= 0, check nselect_bo')
+            raise SystemExit(1)
         elif tot_struc < nselect_bo:
-            raise ValueError('tot_struc < nselect_bo, check nselect_bo')
+            logger.error('tot_struc < nselect_bo, check nselect_bo')
+            raise SystemExit(1)
         score = config.get('BO', 'score')
         if score == 'TS' or score == 'EI' or score == 'PI':
             pass
         else:
-            raise ValueError('score must be TS, EI, or PI, check score')
+            logger.error('score must be TS, EI, or PI, check score')
+            raise SystemExit(1)
         try:
             num_rand_basis = config.getint('BO', 'num_rand_basis')
         except configparser.NoOptionError:
             num_rand_basis = 0
         try:
             cdev = config.getfloat('BO', 'cdev')
         except configparser.NoOptionError:
@@ -351,69 +392,77 @@
             try:
                 fppath = config.get('BO', 'fppath')
             except (configparser.NoOptionError, configparser.NoSectionError):
                 fppath = None
             # -- check cal_fingerprint executable file
             fppath = utility.check_fppath(fppath)
         else:
-            raise NotImplementedError('Now FP only')
+            logger.error('Now FP only')
+            raise SystemExit(1)
         # -- parameters for f-fingerprint
         try:
             fp_rmin = config.getfloat('BO', 'fp_rmin')
         except configparser.NoOptionError:
             fp_rmin = 0.5
         try:
             fp_rmax = config.getfloat('BO', 'fp_rmax')
         except configparser.NoOptionError:
             fp_rmax = 5.0
         if fp_rmin < 0.0:
-            raise ValueError('fp_rmin < 0, check fp_rmin')
+            logger.error('fp_rmin < 0, check fp_rmin')
+            raise SystemExit(1)
         if fp_rmax < fp_rmin:
-            raise ValueError('fp_rmax < fp_rmin, check fp_rmin and fp_rmax')
+            logger.error('fp_rmax < fp_rmin, check fp_rmin and fp_rmax')
+            raise SystemExit(1)
         try:
             fp_npoints = config.getint('BO', 'fp_npoints')
         except configparser.NoOptionError:
             fp_npoints = 20
         if fp_npoints <= 0:
-            raise ValueError('fp_npoints <= 0, check fp_npoints')
+            logger.error('fp_npoints <= 0, check fp_npoints')
+            raise SystemExit(1)
         try:
             fp_sigma = config.getfloat('BO', 'fp_sigma')
         except configparser.NoOptionError:
             fp_sigma = 1.0
         if fp_sigma < 0:
-            raise ValueError('fp_sigma < 0, check fp_sigma')
+            logger.error('fp_sigma < 0, check fp_sigma')
+            raise SystemExit(1)
         # -- BO option
         try:
             max_select_bo = config.getint('BO', 'max_select_bo')
         except configparser.NoOptionError:
             max_select_bo = 0
         if max_select_bo < 0:
-            raise ValueError('max_select_bo must be non-negative int')
+            logger.error('max_select_bo must be non-negative int')
+            raise SystemExit(1)
         try:
             manual_select_bo = config.get('BO', 'manual_select_bo')
             manual_select_bo = [int(x) for x in manual_select_bo.split()]
         except configparser.NoOptionError:
             manual_select_bo = []
         if manual_select_bo:
             for i in manual_select_bo:
                 if not 0 <= i < tot_struc:
-                    raise ValueError('manual_select_bo must be'
+                    logger.error('manual_select_bo must be'
                                      ' non-negative int'
                                      ' and less than tot_struc')
+                    raise SystemExit(1)
         try:
             emax_bo = config.getfloat('BO', 'emax_bo')
         except (configparser.NoOptionError, configparser.NoSectionError):
             emax_bo = None
         try:
             emin_bo = config.getfloat('BO', 'emin_bo')
         except (configparser.NoOptionError, configparser.NoSectionError):
             emin_bo = None
         if emax_bo is not None and emin_bo is not None:
             if emin_bo > emax_bo:
-                raise ValueError('emax_bo < emin_bo, check emax_bo and emin_bo')
+                logger.error('emax_bo < emin_bo, check emax_bo and emin_bo')
+                raise SystemExit(1)
 
     # ---------- LAQA
     if algo == 'LAQA':
         # ------ global declaration
         global nselect_laqa, wf, ws
         # ------ read intput variables
         nselect_laqa = config.getint('LAQA', 'nselect_laqa')
@@ -437,145 +486,165 @@
         if struc_mode in ['mol', 'mol_bs']:
             global n_rotation, mindist_mol_ea, rot_max_angle, protect_mol_struc
         # global restart_gen
         # ------ read intput variables
         # -- number of structures
         n_pop = config.getint('EA', 'n_pop')
         if n_pop <= 0:
-            raise ValueError('n_pop must be positive int')
+            logger.error('n_pop must be positive int')
+            raise SystemExit(1)
         n_crsov = config.getint('EA', 'n_crsov')
         if n_crsov < 0:
-            raise ValueError('n_crsov must be zero or positive int')
+            logger.error('n_crsov must be zero or positive int')
+            raise SystemExit(1)
         n_perm = config.getint('EA', 'n_perm')
         if n_perm < 0:
-            raise ValueError('n_perm must be zero or positive int')
+            logger.error('n_perm must be zero or positive int')
+            raise SystemExit(1)
         if n_perm != 0 and len(atype) == 1:
-            raise ValueError('When the number of atom type is 1,'
+            logger.error('When the number of atom type is 1,'
                              ' n_perm must be 0')
+            raise SystemExit(1)
         n_strain = config.getint('EA', 'n_strain')
         if n_strain < 0:
-            raise ValueError('n_strain must be zero or positive int')
+            logger.error('n_strain must be zero or positive int')
+            raise SystemExit(1)
         n_rand = config.getint('EA', 'n_rand')
         if n_rand < 0:
-            raise ValueError('n_rand must be zero or positive int')
+            logger.error('n_rand must be zero or positive int')
+            raise SystemExit(1)
         if struc_mode not in ['mol', 'mol_bs']:
             if n_crsov + n_perm + n_strain + n_rand != n_pop:
-                raise ValueError('n_crsov + n_perm + n_strain + n_rand'
+                logger.error('n_crsov + n_perm + n_strain + n_rand'
                                  ' must be n_pop')
+                raise SystemExit(1)
         if struc_mode in ['mol', 'mol_bs']:
             n_rotation = config.getint('EA', 'n_rotation')
             if n_rotation < 0:
-                raise ValueError('n_rotation must be zero or positive int')
+                logger.error('n_rotation must be zero or positive int')
+                raise SystemExit(1)
             if n_crsov + n_perm + n_strain + n_rand + n_rotation != n_pop:
-                raise ValueError('n_crsov + n_perm + n_strain + n_rand + n_rotation'
+                logger.error('n_crsov + n_perm + n_strain + n_rand + n_rotation'
                                  ' must be n_pop')
+                raise SystemExit(1)
         n_elite = config.getint('EA', 'n_elite')
         if n_elite < 0:
-            raise ValueError('n_elite must be non-negative int')
+            logger.error('n_elite must be non-negative int')
+            raise SystemExit(1)
         # -- n_fittest
         try:
             fit_reverse = config.getboolean('EA', 'fit_reverse')
         except configparser.NoOptionError:
             fit_reverse = False
         try:
             n_fittest = config.getint('EA', 'n_fittest')
         except configparser.NoOptionError:
             n_fittest = 0
         if n_fittest < 0:
-            raise ValueError('n_fittest must be zero or positive int')
+            logger.error('n_fittest must be zero or positive int')
+            raise SystemExit(1)
         # -- select function
         slct_func = config.get('EA', 'slct_func')
         if slct_func not in ['TNM', 'RLT']:
-            raise ValueError('slct_func must be TNM or RLT')
+            logger.error('slct_func must be TNM or RLT')
+            raise SystemExit(1)
         if slct_func == 'TNM':
             try:
                 t_size = config.getint('EA', 't_size')
             except configparser.NoOptionError:
                 t_size = 3
             if t_size < 2:
-                raise ValueError('t_size must be greater than or equal to 2')
+                logger.error('t_size must be greater than or equal to 2')
+                raise SystemExit(1)
         elif slct_func == 'RLT':
             try:
                 a_rlt = config.getfloat('EA', 'a_rlt')
             except configparser.NoOptionError:
                 a_rlt = 10.0
             try:
                 b_rlt = config.getfloat('EA', 'b_rlt')
             except configparser.NoOptionError:
                 b_rlt = 1.0
             if not 0 < b_rlt < a_rlt:
-                raise ValueError('must be 0 < b_rlt < a_rlt')
+                logger.error('must be 0 < b_rlt < a_rlt')
+                raise SystemExit(1)
         # -- crossover
         try:
             crs_lat = config.get('EA', 'crs_lat')
         except configparser.NoOptionError:
             crs_lat = 'equal'
         if crs_lat not in ['equal', 'random']:
-            raise ValueError('crs_lat must be equal or random')
+            logger.error('crs_lat must be equal or random')
+            raise SystemExit(1)
         try:
             nat_diff_tole = config.getint('EA', 'nat_diff_tole')
         except configparser.NoOptionError:
             nat_diff_tole = 4
         if nat_diff_tole < 0:
-            raise ValueError('nat_diff_tole must be nen-negative int')
+            logger.error('nat_diff_tole must be nen-negative int')
+            raise SystemExit(1)
         # -- permutation
         try:
             ntimes = config.getint('EA', 'ntimes')
         except configparser.NoOptionError:
             ntimes = 1
         if ntimes <= 0:
-            raise ValueError('ntimes must be positive int')
+            logger.error('ntimes must be positive int')
+            raise SystemExit(1)
         try:
             sigma_st = config.getfloat('EA', 'sigma_st')
         except configparser.NoOptionError:
             sigma_st = 0.5
         if sigma_st <= 0:
-            raise ValueError('simga_st must be positive float')
+            logger.error('simga_st must be positive float')
+            raise SystemExit(1)
         if struc_mode in ['mol', 'mol_bs']:
             # -- strain
             try:
                 protect_mol_struc = config.getboolean('EA', 'protect_mol_struc')
             except configparser.NoOptionError:
                 protect_mol_struc = False
             # -- rotation
             try:
                 rot_max_angle = config.getint('EA', 'rot_max_angle')
             except configparser.NoOptionError:
                 rot_max_angle = 360
             if rot_max_angle <= 0:
-                raise ValueError('rot_max_angle must be positive int')
+                logger.error('rot_max_angle must be positive int')
+                raise SystemExit(1)
         # -- common
         if struc_mode in ['mol', 'mol_bs']:
             mindist_mol_ea = []
             for i in range(len(mol_file)):
-                tmp = config.get('EA', 'mindist_mol_ea_{}'.format(i+1))
+                tmp = config.get('EA', f'mindist_mol_ea_{i+1}')
                 tmp = [float(x) for x in tmp.split()]    # character --> float
                 if not len(tmp) == len(mol_file):
-                    raise ValueError('not len(mindist_mol_ea_{}) == len(mol_file)'.format(i+1))
+                    logger.error(f'not len(mindist_mol_ea_{i+1}) == len(mol_file)')
+                    raise SystemExit(1)
                 mindist_mol_ea.append(tmp)
             # check symmetric matrix
             for i in range(len(mindist_mol_ea)):
                 for j in range(len(mindist_mol_ea)):
                     if i < j:
                         if not mindist_mol_ea[i][j] == mindist_mol_ea[j][i]:
-                            raise ValueError('mindist_mol is not symmetric. ({}, {}) -->'
-                                             ' {}, ({}, {}) --> {}'.format(
-                                                 i, j, mindist_mol_ea[i][j],
-                                                 j, i, mindist_mol_ea[j][i]))
+                            logger.error(f'mindist_mol is not symmetric. ({i}, {j}) -->'
+                                             f' {mindist_mol_ea[i][j]}, ({j}, {i}) --> {mindist_mol_ea[j][i]}')
+                            raise SystemExit(1)
         try:
             maxcnt_ea = config.getint('EA', 'maxcnt_ea')
         except configparser.NoOptionError:
             maxcnt_ea = 50
         # -- EA option
         try:
             maxgen_ea = config.getint('EA', 'maxgen_ea')
         except configparser.NoOptionError:
             maxgen_ea = 0
         if maxgen_ea < 0:
-            raise ValueError('maxgen_ea must be non-negative int')
+            logger.error('maxgen_ea must be non-negative int')
+            raise SystemExit(1)
         # # -- restart option
         # try:
         #     restart_gen = config.getint('EA', 'restart_gen')
         # except configparser.NoOptionError:
         #     restart_gen = 0
         try:
             emax_ea = config.getfloat('EA', 'emax_ea')
@@ -583,28 +652,30 @@
             emax_ea = None
         try:
             emin_ea = config.getfloat('EA', 'emin_ea')
         except (configparser.NoOptionError, configparser.NoSectionError):
             emin_ea = None
         if emax_ea is not None and emin_ea is not None:
             if emin_ea > emax_ea:
-                raise ValueError('emax_ea < emin_ea, check emax_ea and emin_ea')
+                logger.error('emax_ea < emin_ea, check emax_ea and emin_ea')
+                raise SystemExit(1)
 
     # ---------- global declaration for comman part in calc_code
     global kppvol, kpt_flag, force_gamma
 
     # ---------- VASP
     if calc_code == 'VASP':
         # ------ read intput variables
         kpt_flag = True
         kppvol = config.get('VASP', 'kppvol')
         kppvol = [int(x) for x in kppvol.split()]    # character --> int
         if not len(kppvol) == nstage:
-            raise ValueError('not len(kppvol) == nstage,'
+            logger.error('not len(kppvol) == nstage,'
                              ' check kppvol and nstage')
+            raise SystemExit(1)
         try:
             force_gamma = config.getboolean('VASP', 'force_gamma')
         except configparser.NoOptionError:
             force_gamma = False
 
     # ---------- QE
     elif calc_code == 'QE':
@@ -613,16 +684,17 @@
         # ------ read intput variables
         kpt_flag = True
         qe_infile = config.get('QE', 'qe_infile')
         qe_outfile = config.get('QE', 'qe_outfile')
         kppvol = config.get('QE', 'kppvol')
         kppvol = [int(x) for x in kppvol.split()]    # character --> int
         if not len(kppvol) == nstage:
-            raise ValueError('not len(kppvol) == nstage,'
+            logger.error('not len(kppvol) == nstage,'
                              ' check kppvol and nstage')
+            raise SystemExit(1)
         try:
             force_gamma = config.getboolean('QE', 'force_gamma')
         except configparser.NoOptionError:
             force_gamma = False
 
     # ---------- OpenMX
     elif calc_code == 'OMX':
@@ -639,16 +711,17 @@
         ValElecIn = ValenceElec.split()
         for i in range(0, len(ValElecIn), 3):
             upSpin[ValElecIn[i]]   = ValElecIn[i+1]
             downSpin[ValElecIn[i]] = ValElecIn[i+2]
         kppvol = config.get('OMX', 'kppvol')
         kppvol = [int(x) for x in kppvol.split()]    # character --> int
         if not len(kppvol) == nstage:
-            raise ValueError('not len(kppvol) == nstage,'
+            logger.error('not len(kppvol) == nstage,'
                             ' check kppvol and nstage')
+            raise SystemExit(1)
         try:
             force_gamma = config.getboolean('OMX', 'force_gamma')
         except configparser.NoOptionError:
             force_gamma = False
 
     # ---------- soiap
     elif calc_code == 'soiap':
@@ -692,34 +765,38 @@
 
 
 def _spglist(spgnum):
     tmpspg = []
     for c in spgnum.split():
         if '-' in c:
             if not len(c.split('-')) == 2:
-                raise ValueError('Wrong input in spgnum. ')
+                logger.error('Wrong input in spgnum. ')
+                raise SystemExit(1)
             istart = int(c.split('-')[0])
             iend = int(c.split('-')[1])+1
             if istart < 0 or 230 < istart:
-                raise ValueError('spgnum must be 1 -- 230')
+                logger.error('spgnum must be 1 -- 230')
+                raise SystemExit(1)
             if iend < 0 or 231 < iend:
-                raise ValueError('spgnum must be 1 -- 230')
+                logger.error('spgnum must be 1 -- 230')
+                raise SystemExit(1)
             for i in range(istart, iend):
                 if i not in tmpspg:
                     tmpspg.append(i)
         else:
             if int(c) < 0 or 230 < int(c):
-                raise ValueError('spgnum must be 1 -- 230')
+                logger.error('spgnum must be 1 -- 230')
+                raise SystemExit(1)
             if not int(c) in tmpspg:
                 tmpspg += [int(c)]
     return tmpspg
 
 
 def save_stat(stat):    # only 1st run
-    print('Save input data in cryspy.stat')
+    logger.info('Save input data in cryspy.stat')
     # ---------- basic
     stat.set('basic', 'algo', '{}'.format(algo))
     stat.set('basic', 'calc_code', '{}'.format(calc_code))
     stat.set('basic', 'tot_struc', '{}'.format(tot_struc))
     if not calc_code == 'ext':
         stat.set('basic', 'nstage', '{}'.format(nstage))
         stat.set('basic', 'njob', '{}'.format(njob))
@@ -886,14 +963,17 @@
     stat.set('option', 'stress_step_flag', '{}'.format(stress_step_flag))
 
     # ---------- write stat
     io_stat.write_stat(stat)
 
 
 def diffinstat(stat):
+    #
+    # Do not use SystemExit in diffinstat!
+    #
     logic_change = False
 
     # ---------- old input
     # ------ basic
     old_algo = stat.get('basic', 'algo')
     old_calc_code = stat.get('basic', 'calc_code')
     old_tot_struc = stat.getint('basic', 'tot_struc')
@@ -944,26 +1024,26 @@
     try:    # case: None
         old_mindist = stat.get('structure', 'mindist')
         if old_mindist == 'None':
             old_mindist = None    # character --> None
     except (configparser.NoOptionError, configparser.NoSectionError):
         old_mindist = []
         for i in range(len(atype)):
-            tmp = stat.get('structure', 'mindist_{}'.format(i+1))
+            tmp = stat.get('structure', f'mindist_{i+1}')
             tmp = [float(x) for x in tmp.split()]    # character --> float
             old_mindist.append(tmp)
     old_mindist_factor = stat.getfloat('structure', 'mindist_factor')
     try:    # case: None
         old_mindist_mol_bs = stat.get('structure', 'mindist_mol_bs')
         if old_mindist_mol_bs == 'None':
             old_mindist_mol_bs = None    # character --> None
     except (configparser.NoOptionError, configparser.NoSectionError):
         old_mindist_mol_bs = []
         for i in range(len(mol_file)):
-            tmp = stat.get('structure', 'mindist_mol_bs_{}'.format(i+1))
+            tmp = stat.get('structure', f'mindist_mol_bs_{i+1}')
             tmp = [float(x) for x in tmp.split()]    # character --> float
             old_mindist_mol_bs.append(tmp)
     old_mindist_mol_bs_factor = stat.getfloat('structure', 'mindist_mol_bs_factor')
     old_maxcnt = stat.getint('structure', 'maxcnt')
     old_symprec = stat.getfloat('structure', 'symprec')
     old_spgnum = stat.get('structure', 'spgnum')
     if old_spgnum == '0':
@@ -1048,15 +1128,15 @@
         old_ntimes = stat.getint('EA', 'ntimes')
         old_sigma_st = stat.getfloat('EA', 'sigma_st')
         if struc_mode in ['mol', 'mol_bs']:
             old_protect_mol_struc = stat.getboolean('EA', 'protect_mol_struc')
             old_rot_max_angle = stat.getint('EA', 'rot_max_angle')
             old_mindist_mol_ea = []
             for i in range(len(mol_file)):
-                tmp = stat.get('EA', 'mindist_mol_ea_{}'.format(i+1))
+                tmp = stat.get('EA', f'mindist_mol_ea_{i+1}')
                 tmp = [float(x) for x in tmp.split()]    # character --> float
                 old_mindist_mol_ea.append(tmp)
         old_maxcnt_ea = stat.getint('EA', 'maxcnt_ea')
         old_maxgen_ea = stat.getint('EA', 'maxgen_ea')
         # old_restart_gen = stat.get('EA', 'restart_gen')
         old_emax_ea = stat.get('EA', 'emax_ea')
         if old_emax_ea == 'None':
@@ -1573,8 +1653,8 @@
 
     # ---------- save stat if necessary
     if logic_change:
         io_stat.write_stat(stat)
 
 
 def diff_out(var_str, old_var, var):
-    print('Changed {0} from {1} to {2}'.format(var_str, old_var, var))
+    logger.info(f'Changed {var_str} from {old_var} to {var}')
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/LAQA/calc_score.py` & `csp-cryspy-1.2.0/src/cryspy/LAQA/calc_score.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.1/src/cryspy/LAQA/laqa_init.py` & `csp-cryspy-1.2.0/src/cryspy/LAQA/laqa_init.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 '''
 Initialize LAQA
 '''
 
+from logging import getLogger
+
 from ..IO import io_stat, pkl_data
 from ..IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def initialize(stat):
-    print('\n# ---------- Initialize LAQA')
+    logger.info('# ---------- Initialize LAQA')
 
     # ---------- initialize
     tot_step_select = [0]
     laqa_step = {}
     laqa_struc = {}
     laqa_energy = {}
     laqa_bias = {}
@@ -37,12 +41,13 @@
     io_stat.set_common(stat, 'selection', 0)
     io_stat.set_common(stat, 'total_step', 0)
     io_stat.set_id(stat, 'selected_id', id_queueing)    # all IDs
     io_stat.set_id(stat, 'id_queueing', id_queueing)    # all IDs
     io_stat.write_stat(stat)
 
     # ---------- log
-    print('# ---------- Selection 0')
+    logger.info('# ---------- Selection 0')
     if len(id_queueing) > 30:
-        print('selected_id: {} IDs'.format(len(id_queueing)))
+        logger.info(f'selected_id: {len(id_queueing)} IDs')
     else:
-        print('selected_id: {}'.format(' '.join(str(a) for a in id_queueing)))
+        x = ' '.join(str(a) for a in id_queueing)
+        logger.info(f'selected_id: {x}')
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/LAQA/laqa_next_selection.py` & `csp-cryspy-1.2.0/src/cryspy/LAQA/laqa_next_selection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 '''
 Selection in LAQA
 '''
 
+from logging import getLogger
 import os
 
 from ..IO import io_stat, pkl_data
 from ..IO import read_input as rin
 from ..IO.out_results import out_laqa_id_hist
 
 
+logger = getLogger('cryspy')
+
 def next_selection(stat, laqa_id_data, laqa_data):
     # ---------- laqa_id_data and laqa_data
     (id_queueing, id_running, id_select_hist) = laqa_id_data
     (tot_step_select, laqa_step, laqa_struc,
      laqa_energy, laqa_bias, laqa_score) = laqa_data
 
     # ---------- LAQA selection
@@ -22,15 +25,15 @@
         else:
             id_queueing.append(k)
             if len(id_queueing) == rin.nselect_laqa:
                 break
 
     # ---------- done LAQA
     if len(id_queueing) == 0:
-        print('\nDone all structures!')
+        logger.info('\nDone all structures!')
         os.remove('lock_cryspy')
         raise SystemExit()
 
     # ---------- append id_select_hist and out
     id_select_hist.append(id_queueing[:])    # append shallow copy
     out_laqa_id_hist(id_select_hist)
 
@@ -47,13 +50,13 @@
     # ---------- status
     io_stat.set_common(stat, 'selection', len(id_select_hist))
     io_stat.set_id(stat, 'selected_id', id_queueing)
     io_stat.set_id(stat, 'id_queueing', id_queueing)
     io_stat.write_stat(stat)
 
     # ---------- out and log
-    print('\n# ---------- Selection {}'.format(len(id_select_hist)))
+    logger.info(f'# ---------- Selection {len(id_select_hist)}')
     if len(id_queueing) > 30:
-        print('selected_id: {} IDs'.format(len(id_queueing)))
+        logger.info(f'selected_id: {len(id_queueing)} IDs')
     else:
-        print('selected_id: {}\n'.format(
-            ' '.join(str(a) for a in id_queueing)))
+        x = ' '.join(str(a) for a in id_queueing)
+        logger.info(f'selected_id: {x}')
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/LAQA/laqa_restart.py` & `csp-cryspy-1.2.0/src/cryspy/LAQA/laqa_restart.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 '''
 Restart in LAQA
 '''
 
+from logging import getLogger
+
 from ..IO import io_stat, pkl_data
 from ..IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def restart(stat, prev_nstruc):
     # ---------- load laqa data
     id_queueing, id_running, id_select_hist = pkl_data.load_laqa_id()
     tot_step_select, laqa_step, laqa_struc, \
         laqa_energy, laqa_bias, laqa_score = pkl_data.load_laqa_data()
 
     # ---------- initialize for appended ID
     for i in range(prev_nstruc, rin.tot_struc):
         laqa_step[i] = []
         laqa_struc[i] = []
         laqa_energy[i] = []
         laqa_bias[i] = []
         laqa_score[i] = [float('inf')]
         id_queueing.append(i)
-    print('Append scores and id_queueing')
+    logger.info('Append scores and id_queueing')
 
     # ---------- status
     io_stat.set_id(stat, 'id_queueing', id_queueing)
     io_stat.write_stat(stat)
 
     # ---------- save for LAQA
     laqa_id_data = (id_queueing, id_running, id_select_hist)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py` & `csp-cryspy-1.2.0/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 '''
 Random structure generation using PyXtal (https://github.com/qzhu2017/PyXtal)
 '''
 
 import collections
 from contextlib import redirect_stdout, redirect_stderr
+from io import StringIO
+from logging import getLogger
 from multiprocessing import Process, Queue
 import os
 import random
 import sys
 
 import numpy as np
 from pymatgen.core import Structure, Molecule
@@ -17,14 +19,16 @@
 from pyxtal.tolerance import Tol_matrix
 
 from ...util.struc_util import check_distance, sort_by_atype, out_poscar
 from ...util.struc_util import get_atype_dummy, scale_cell_mol, rot_mat
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 class Rnd_struc_gen_pyxtal:
     '''
     Random structure generation using pyxtal
     '''
 
     def __init__(self, mindist):
         self.mindist = mindist
@@ -39,15 +43,16 @@
         pyxtal_mol_names = list(Collection('molecules'))
         for i, mf in enumerate(rin.mol_file):
             if os.path.isfile(mf):
                 mol = Molecule.from_file(mf)
             elif mf in pyxtal_mol_names:
                 mol = pyxtal_mol_data[mf]
             else:
-                raise ValueError('no molecular files')
+                logger.error('no molecular files')
+                raise SystemExit(1)
             mol_data.append(mol)
         # ---------- self.xxx
         self.mol_data = mol_data
 
     def gen_struc(self, nstruc, id_offset=0, init_pos_path=None):
         '''
         Generate random structures for given space groups
@@ -80,20 +85,24 @@
             else:
                 spg = random.choice(rin.spgnum)
             # ------ vol_factor
             rand_vol = random.uniform(rin.vol_factor[0], rin.vol_factor[1])
             # ------ generate structure
             tmp_crystal = pyxtal()
             try:
-                with redirect_stdout(sys.stderr):
+                f = StringIO()
+                with redirect_stdout(f):
                     tmp_crystal.from_random(dim=3, group=spg, species=rin.atype,
                                             numIons=rin.nat, factor=rand_vol,
                                             conventional=False, tm=tolmat)
+                s = f.getvalue().rstrip()    # to delete \n
+                if s:
+                    logger.warning(s)
             except Exception as e:
-                print(e, ':spg = {} retry.'.format(spg), file=sys.stderr, flush=True)
+                logger.warning(e.args[0] + f': spg = {spg} retry.')
                 continue
             if tmp_crystal.valid:
                 tmp_struc = tmp_crystal.to_pymatgen(resort=False)    # pymatgen Structure format
                 # -- check the number of atoms
                 if not self._check_nat(tmp_struc):
                     # (pyxtal 0.1.4) cryspy adopts "conventional=False",
                     #     which is better for DFT calculation
@@ -128,17 +137,16 @@
                         symprec=rin.symprec)
                 except TypeError:
                     spg_num = 0
                     spg_sym = None
                 # -- register the structure in pymatgen format
                 cid = len(self.init_struc_data) + id_offset
                 self.init_struc_data[cid] = tmp_struc
-                print('Structure ID {0:>6} was generated.'
-                      ' Space group: {1:>3} --> {2:>3} {3}'.format(
-                       cid, spg, spg_num, spg_sym), flush=True)
+                logger.info(f'Structure ID {cid:>6} was generated.'
+                      f' Space group: {spg:>3} --> {spg_num:>3} {spg_sym}')
                 # -- save init_POSCARS
                 if init_pos_path is not None:
                     out_poscar(tmp_struc, cid, init_pos_path)
 
     def gen_struc_mol(self, nstruc, id_offset=0, init_pos_path=None):
         '''
         Generate random molecular crystal structures for given space groups
@@ -155,24 +163,14 @@
                              specify a path of file
                              if you write POSCAR data of init_struc_data
                              ATTENSION: data are appended to the specified file
 
         # ---------- comment
         generated structure data are saved in self.init_struc_data
         '''
-        # ---------- check args
-        if not (type(nstruc) is int and nstruc > 0):
-            raise ValueError('nstruc must be positive int')
-        if type(id_offset) is not int:
-            raise TypeError('id_offset must be int')
-        if init_pos_path is None or type(init_pos_path) is str:
-            pass
-        else:
-            raise ValueError('init_pos_path is wrong.'
-                             ' init_pos_path = {}'.format(init_pos_path))
         # ---------- initialize
         self.init_struc_data = {}
         if rin.algo == 'EA' and rin.struc_mode in ['mol', 'mol_bs']:
             self.struc_mol_id = {}
         # ---------- Tol_matrix
         tolmat = self._set_tol_mat(rin.atype, self.mindist)
         # ---------- loop for structure generattion
@@ -192,48 +190,49 @@
             if p.is_alive():
                 p.terminate()
                 p.join()
             if sys.version_info.minor >= 7:
                 # Process.close() available from python 3.7
                 p.close()
             if q.empty():
-                print('timeout for molecular structure generation. retry.',
-                      file=sys.stderr, flush=True)
+                logger.warning('timeout for molecular structure generation. retry.')
                 continue
             else:
                 # -- get struc data from _mp_mc
                 if rin.algo == 'EA':
                     tmp_q = q.get()
                     tmp_struc = tmp_q[0]    # structure data
                     dums = tmp_q[1]         # dummy element
                     in_dists = tmp_q[2]     # interatomic distance in a molecule
                     mol_dists = tmp_q[3]    # distance between molecules
                 else:
                     tmp_struc = q.get()
                 tmp_valid = q.get()
                 if tmp_struc == 'error':
+                    # in case of 'error', tmp_valid <-- error message (Exception)
+                    logger.warning(tmp_valid.args[0] + f': spg = {spg} retry.')
                     continue
             if tmp_valid:
                 # -- scale volume
                 if rin.vol_mu is not None:
                     vol = random.gauss(mu=rin.vol_mu, sigma=rin.vol_sigma)
                     vol = vol * tmp_struc.num_sites / rin.natot    # for conv. cell
                     tmp_struc = scale_cell_mol(tmp_struc, self.mol_data, vol)
                     if not tmp_struc:    # case: scale_cell_mol returns False
-                        print('failed scale cell. retry.', file=sys.stderr, flush=True)
+                        logger.warning('failed scale cell. retry.')
                         continue
                 # -- check nat
                 if not self._check_nat(tmp_struc):
                     # cryspy adopts conventional=True
                     # pyxtal returns conventional cell,
                     # too many atoms if centering
                     tmp_struc = tmp_struc.get_primitive_structure()
                     # recheck nat
                     if not self._check_nat(tmp_struc):    # failure
-                        print('different num. of atoms. retry.', file=sys.stderr, flush=True)
+                        logger.warning('different num. of atoms. retry.')
                         continue
                 # -- grouping atoms for molecule using interatomic distance
                 if rin.algo == 'EA':
                     loopcnt = 0
                     while loopcnt < 10:
                         loopcnt += 1
                         mol_group = []
@@ -300,17 +299,16 @@
                     spg_num = 0
                     spg_sym = None
                 # -- register the structure in pymatgen format
                 cid = len(self.init_struc_data) + id_offset
                 self.init_struc_data[cid] = tmp_struc
                 if rin.algo == 'EA' and rin.struc_mode in ['mol', 'mol_bs']:
                     self.struc_mol_id.update({cid: [tmp_mol_indx, tmp_id, mol_dists]})
-                print('Structure ID {0:>6} was generated.'
-                      ' Space group: {1:>3} --> {2:>3} {3}'.format(
-                       cid, spg, spg_num, spg_sym), flush=True)
+                logger.info(f'Structure ID {cid:>6} was generated.'
+                      f' Space group: {spg:>3} --> {spg_num:>3} {spg_sym}')
                 # -- save init_POSCARS
                 if init_pos_path is not None:
                     out_poscar(tmp_struc, cid, init_pos_path)
 
     def gen_struc_mol_break_sym(self, nstruc, mindist_dummy,
                                 id_offset=0, init_pos_path=None):
         '''
@@ -332,24 +330,14 @@
                              specify a path of file
                              if you write POSCAR data of init_struc_data
                              ATTENSION: data are appended to the specified file
 
         # ---------- comment
         generated structure data are saved in self.init_struc_data
         '''
-        # ---------- check args
-        if not (type(nstruc) is int and nstruc > 0):
-            raise ValueError('nstruc must be positive int')
-        if type(id_offset) is not int:
-            raise TypeError('id_offset must be int')
-        if init_pos_path is None or type(init_pos_path) is str:
-            pass
-        else:
-            raise ValueError('init_pos_path is wrong.'
-                             ' init_pos_path = {}'.format(init_pos_path))
         # ---------- initialize
         self.init_struc_data = {}
         if rin.algo == 'EA' and rin.struc_mode in ['mol', 'mol_bs']:
             self.struc_mol_id = {}
         # ------ dummy atom type
         atype_dummy = get_atype_dummy()
         # ---------- Tol_matrix for dummy atoms
@@ -362,20 +350,24 @@
             else:
                 spg = random.choice(rin.spgnum)
             # ------ vol_factor
             rand_vol = random.uniform(rin.vol_factor[0], rin.vol_factor[1])
             # ------ generate structure
             tmp_crystal = pyxtal()
             try:
-                with redirect_stdout(sys.stderr):
+                f = StringIO()
+                with redirect_stdout(f):
                     tmp_crystal.from_random(dim=3, group=spg, species=atype_dummy,
                                             numIons=rin.nmol, factor=rand_vol,
                                             conventional=False, tm=tolmat)
+                s = f.getvalue().rstrip()    # to delete \n
+                if s:
+                    logger.warning(s)
             except Exception as e:
-                print(e, ':spg = {} retry.'.format(spg), file=sys.stderr, flush=True)
+                logger.warning(e.args[0] + f': spg = {spg} retry.')
                 continue
             if tmp_crystal.valid:
                 # -- each wyckoff position --> dummy atom
                 dums = []        # dummy atoms
                 dum_pos = []     # internal position of dummy
                 dum_type = {}    # type of dummy
                                  #  e.g. {DummySpecie X00+: 'Rn',
@@ -464,18 +456,17 @@
                     tmp_struc = sort_by_atype(tmp_struc, rin.atype)
                     # -- check minimum distance
                     if self.mindist is not None:
                         success, mindist_ij, dist = check_distance(tmp_struc,
                                                                    rin.atype,
                                                                    self.mindist)
                         if not success:
-                            print('mindist: {} - {}, {}. retry.'.format(
-                                rin.atype[mindist_ij[0]],
-                                rin.atype[mindist_ij[1]],
-                                dist), file=sys.stderr, flush=True)
+                            type0 = rin.atype[mindist_ij[0]]
+                            type1 = rin.atype[mindist_ij[1]]
+                            logger.warning(f'mindist: {type0} - {type1}, {dist}. retry.')
                             if rin.rot_mol is None:
                                 break    # go back to the while loop
                             continue    # failure
                     # -- check actual space group (success)
                     try:
                         spg_sym, spg_num = tmp_struc.get_space_group_info(
                             symprec=rin.symprec)
@@ -495,17 +486,16 @@
                     mol_dists = []
                     for j, mol in enumerate(self.mol_data):
                         tmp_dists = []
                         for n, m in enumerate(mol):
                             tmp_dists.append(mol.get_distance(0, n))
                         mol_dists.append(tmp_dists)
                     self.struc_mol_id.update({cid: [tmp_mol_indx, tmp_id, mol_dists]})
-                print('Structure ID {0:>6} was generated.'
-                      ' Space group: {1:>3} --> {2:>3} {3}'.format(
-                       cid, spg, spg_num, spg_sym), flush=True)
+                logger.info(f'Structure ID {cid:>6} was generated.'
+                      f' Space group: {spg:>3} --> {spg_num:>3} {spg_sym}')
                 # -- save init_POSCARS
                 if init_pos_path is not None:
                     out_poscar(tmp_struc, cid, init_pos_path)
 
     def _set_tol_mat(self, atype, mindist):
         tolmat = Tol_matrix()
         for i, itype in enumerate(atype):
@@ -521,25 +511,28 @@
             if species_list.count(rin.atype[i]) != rin.nat[i]:
                 return False    # failure
         return True
 
     def _mp_mc(self, tolmat, spg, nmol, rand_vol, q, algo):
         '''
         multiprocess part
-        here cannot use rin.xxx
+        here cannot use rin.xxx and logging
         '''
         try:
             np.random.seed(random.randint(0, 100000000))
             tmp_crystal = pyxtal(molecular=True)
-            with open('err_cryspy', 'a') as f:
-                with redirect_stdout(f):
-                    with redirect_stderr(f):
-                        tmp_crystal.from_random(dim=3, group=spg,
-                                                species=self.mol_data, numIons=nmol,
-                                                factor=rand_vol, conventional=False, tm=tolmat)
+            f = StringIO()
+            with redirect_stdout(f):
+                with redirect_stderr(f):
+                    tmp_crystal.from_random(dim=3, group=spg,
+                                            species=self.mol_data, numIons=nmol,
+                                            factor=rand_vol, conventional=False, tm=tolmat)
+            s = f.getvalue().rstrip()    # to delete \n
+            if s:
+                logger.warning(s)
             if algo == 'EA':
                 tmp_struc = tmp_crystal.to_pymatgen(resort=False)
                 tmp_lattice = tmp_struc.lattice
                 dums = []        # dummy atoms
                 dum_pos = []     # internal position of dummy
                 in_dists = []
                 mol_dists = []
@@ -569,12 +562,9 @@
                 else:
                     q.put(tmp_crystal.to_pymatgen(resort=False))
                 q.put(tmp_crystal.valid)
             else:
                 q.put(None)
                 q.put(tmp_crystal.valid)
         except Exception as e:
-            with open('err_cryspy', 'a') as f:
-                f.write(e.args[0])
-                f.write('    spg = {} retry.\n'.format(spg))
             q.put('error')
-            q.put(None)
+            q.put(e)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/RS/gen_struc_RS/random_generation.py` & `csp-cryspy-1.2.0/src/cryspy/RS/gen_struc_RS/random_generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 '''
 Random structure generation w/o pyxtal
 '''
 
 import json
+from logging import getLogger
 import math
 import os
 import random
 import subprocess
 import sys
 
 import numpy as np
 from pymatgen.core import Structure
 
 from ...IO import read_input as rin
 from ...util.struc_util import check_distance, out_poscar
 
 
+logger = getLogger('cryspy')
+
 class Rnd_struc_gen:
     '''
     Random structure generation w/o pyxtal
     '''
 
     def __init__(self, mindist):
         self.mindist = mindist
@@ -58,31 +61,30 @@
                 if rin.vol_mu is not None:
                     vol = random.gauss(mu=rin.vol_mu, sigma=rin.vol_sigma)
                     tmp_struc.scale_lattice(volume=vol)
                     success, mindist_ij, dist = check_distance(tmp_struc,
                                                                rin.atype,
                                                                self.mindist)
                     if not success:
-                        print('mindist in gen_wo_spg: {} - {}, {}. retry.'.format(
-                            rin.atype[mindist_ij[0]],
-                            rin.atype[mindist_ij[1]],
-                            dist), file=sys.stderr, flush=True)
+                        type0 = rin.atype[mindist_ij[0]]
+                        type1 = rin.atype[mindist_ij[1]]
+                        logger.warning(f'mindist in gen_wo_spg: {type0} - {type1}, {dist}. retry.')
                         continue    # failure
                 # ------ check actual space group using pymatgen
                 try:
                     spg_sym, spg_num = tmp_struc.get_space_group_info(
                         symprec=rin.symprec)
                 except TypeError:
                     spg_num = 0
                     spg_sym = None
                 # ------ register the structure in pymatgen format
                 cid = len(init_struc_data) + id_offset
                 init_struc_data[cid] = tmp_struc
-                print('Structure ID {0:>6} was generated.'
-                      ' Space group: {1:>3} {2}'.format(cid, spg_num, spg_sym), flush=True)
+                logger.info(f'Structure ID {cid:>6} was generated.'
+                      f' Space group: {spg_num:>3} {spg_sym}')
                 # ------ save poscar
                 if init_pos_path is not None:
                     out_poscar(tmp_struc, cid, init_pos_path)
         self.init_struc_data = init_struc_data
 
     def gen_with_find_wy(self, nstruc, id_offset=0,
                          init_pos_path=None, fwpath='find_wy', mpi_rank=0):
@@ -146,32 +148,30 @@
             if rin.vol_mu is not None:
                 vol = random.gauss(mu=rin.vol_mu, sigma=rin.vol_sigma)
                 tmp_struc.scale_lattice(volume=vol)
                 success, mindist_ij, dist = check_distance(tmp_struc,
                                                            rin.atype,
                                                            self.mindist)
                 if not success:
-                    print('mindist in gen_with_find_wy: {} - {}, {}. retry.'.format(
-                        rin.atype[mindist_ij[0]],
-                        rin.atype[mindist_ij[1]],
-                        dist), file=sys.stderr, flush=True)
+                    type0 = rin.atype[mindist_ij[0]]
+                    type1 = rin.atype[mindist_ij[1]]
+                    logger.warning(f'mindist in gen_with_find_wy: {type0} - {type1}, {dist}. retry.')
                     continue    # failure
             # ------ check actual space group using pymatgen
             try:
                 spg_sym, spg_num = tmp_struc.get_space_group_info(
                     symprec=rin.symprec)
             except TypeError:
                 spg_num = 0
                 spg_sym = None
             # ------ register the structure in pymatgen format
             cid = len(init_struc_data) + id_offset
             init_struc_data[cid] = tmp_struc
-            print('Structure ID {0:>6} was generated.'
-                  ' Space group: {1:>3} --> {2:>3} {3}'.format(
-                   cid, self.spg, spg_num, spg_sym), flush=True)
+            logger.info(f'Structure ID {cid:>6} was generated.'
+                  f' Space group: {self.spg:>3} --> {spg_num:>3} {spg_sym}')
             # ------ clean
             self._rm_files()
         # ---------- go back to ..
         os.chdir('../../')
         # ---------- init_struc_data
         self.init_struc_data = init_struc_data
 
@@ -216,15 +216,16 @@
                 # trigonal includes rhombohedral in find_wy
                 csys = 'Trigonal'
             elif 168 <= spg <= 194:
                 csys = 'Hexagonal'
             elif 195 <= spg <= 230:
                 csys = 'Cubic'
             else:
-                raise ValueError('spg is wrong')
+                logger.error('spg is wrong')
+                raise SystemExit(1)
         # ---------- generate lattice constants a, b, c, alpha, beta, gamma
         if csys == 'Triclinic':
             t1 = random.uniform(rin.minlen, rin.maxlen)
             t2 = random.uniform(rin.minlen, rin.maxlen)
             t3 = random.uniform(rin.minlen, rin.maxlen)
             t = [t1, t2, t3]
             t.sort()
@@ -324,18 +325,17 @@
             tmp_struc = Structure([self.va, self.vb, self.vc],
                                   self.atomlist[:len(incoord)],
                                   incoord)
             success, mindist_ij, dist = check_distance(tmp_struc,
                                                        rin.atype,
                                                        self.mindist)
             if not success:
-                print('mindist in _gen_struc_wo_spg: {} - {}, {}. retry.'.format(
-                    rin.atype[mindist_ij[0]],
-                    rin.atype[mindist_ij[1]],
-                    dist), file=sys.stderr, flush=True)
+                type0 = rin.atype[mindist_ij[0]]
+                type1 = rin.atype[mindist_ij[1]]
+                logger.warning(f'mindist in _gen_struc_wo_spg: {type0} - {type1}, {dist}. retry.')
                 incoord.pop(-1)    # cancel
                 cnt += 1
                 if rin.maxcnt < cnt:
                     return None
         return tmp_struc
 
     def _fw_input(self):
@@ -401,18 +401,17 @@
                 # -- check minimum distance
                 spgstruc = Structure(plat, atomnames, cart,
                                      coords_are_cartesian=True)
                 success, mindist_ij, dist = check_distance(spgstruc,
                                                            rin.atype,
                                                            self.mindist)
                 if not success:
-                    print('mindist in _gen_struc_with_spg: {} - {}, {}. retry.'.format(
-                        rin.atype[mindist_ij[0]],
-                        rin.atype[mindist_ij[1]],
-                        dist), file=sys.stderr, flush=True)
+                    type0 = rin.atype[mindist_ij[0]]
+                    type1 = rin.atype[mindist_ij[1]]
+                    logger.warning(f'mindist in _gen_struc_with_spg: {type0} - {type1}, {dist}. retry.')
                     # failure
                     # num_uniqvar = 0 --> value == 0
                     cnt = rin.maxcnt + 1 if value == 0 else cnt + 1
                     if rin.maxcnt < cnt:
                         return False, spgstruc    # spgstruc is dummy
                 else:
                     break    # break while loop --> next eq atoms
@@ -455,15 +454,16 @@
                 elif ch == 'z':
                     pos.append(rval[2])
                 elif ch == 'x-y':
                     pos.append(rval[0] - rval[1])
                 elif ch == '2x':
                     pos.append(2.0 * rval[0])
                 else:
-                    raise ValueError('unknown ch in conversion in gen_wycoord')
+                    logger.error('unknown ch in conversion in gen_wycoord')
+                    raise SystemExit(1)
             pos = np.array(pos)
             eq_positions.append(pos + each['add'])
             eq_atomnames.append(each['name'])
         return eq_atomnames, eq_positions
 
     def _rm_files(self, files=['input', 'POS_WY_SKEL_ALL.json']):
         for rfile in files:
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/RS/rs_restart.py` & `csp-cryspy-1.2.0/src/cryspy/RS/rs_restart.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.1/src/cryspy/calc_dscrpt/FP/calc_FP.py` & `csp-cryspy-1.2.0/src/cryspy/calc_dscrpt/FP/calc_FP.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 '''
 Calculate Fingerprint
 '''
 
+from logging import getLogger
 import os
 import subprocess
 
 import numpy as np
 
 
+logger = getLogger('cryspy')
+
 class Calc_FP:
     '''
     calculate fingerprint using cal_fingerprint program
 
     # ---------- args
     struc_data (dict or list): structure data
         You may include None in struc_data
@@ -32,38 +35,22 @@
         # ------ struc_data
         if type(struc_data) is dict:
             pass
         elif type(struc_data) is list:
             # -- convert to dict
             struc_data = {i: struc_data[i] for i in range(len(struc_data))}
         else:
-            raise TypeError('Type of struc_data is wrong')
+            logger.error('Type of struc_data is wrong')
+            raise SystemExit(1)
         self.struc_data = struc_data
-        # ------ fp_rmin, fp_rmax, fp_sigma
-        if fp_rmin >= fp_rmax:
-            raise ValueError('fprmin >= fp_rmax')
-        for x in [fp_rmin, fp_rmax, fp_sigma]:
-            if type(x) is float and x > 0:
-                pass
-            else:
-                raise ValueError('fp_rmin, fp_rmax, and fp_sigma'
-                                 ' msut be positive float')
+        # ------ fp
         self.fp_rmin = fp_rmin
         self.fp_rmax = fp_rmax
         self.fp_sigma = fp_sigma
-        # ------ fp_npoints
-        if type(fp_npoints) is int and fp_npoints > 0:
-            pass
-        else:
-            raise ValueError('fp_npoints must be positive int')
         self.fp_npoints = fp_npoints
-        # ------ fppath
-        if not os.path.isfile(fppath):
-            raise IOError('There is no cal_fingerprint program in {}'.format(
-                fppath))
         self.fppath = os.path.abspath(fppath)
 
     def calc(self):
         '''
         calculate fingerprint
 
         # ---------- return
@@ -75,15 +62,16 @@
         os.chdir('tmp_calc_FP')
         # ---------- calc fingerprint
         self.descriptors = {}
         for cid, struc in self.struc_data.items():
             # ------ output POSCAR
             struc.to(fmt='poscar', filename='POSCAR')
             if not os.path.isfile('POSCAR'):
-                raise IOError('No POSCAR file')
+                logger.error('No POSCAR file')
+                raise SystemExit(1)
             # ------ run cal_fingerprint
             with open('log_fingerprint', 'w') as logf:
                 subprocess.call([self.fppath, 'POSCAR',
                                  '-rmin', '{}'.format(self.fp_rmin),
                                  '-rmax', '{}'.format(self.fp_rmax),
                                  '-npoints', '{}'.format(self.fp_npoints),
                                  '-sigma', '{}'.format(self.fp_sigma)],
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/ASE/calc_files_ase.py` & `csp-cryspy-1.2.0/src/cryspy/interface/ASE/calc_files_ase.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 '''
 Calculation files in ASE
 '''
 
+from logging import getLogger
 import os
 
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def check_input_ase():
     # ---------- prepare rin.jobfile, POTCAR, INCAR
     calc_inputs = [rin.jobfile, rin.ase_python]
 
     # ----- check required files
     for f in calc_inputs:
         if f == rin.ase_python:
             finfiles = [rin.ase_python + '_{}'.format(i) for i in range(
                 1, rin.nstage+1)]
             for ff in finfiles:
                 if not os.path.isfile('./calc_in/'+ff):
-                    raise IOError('Could not find ./calc_in/'+ff)
+                    logger.error('Could not find ./calc_in/'+ff)
+                    raise SystemExit(1)
         else:
             if not os.path.isfile('./calc_in/'+f):
-                raise IOError('Could not find ./calc_in/'+f)
+                logger.error('Could not find ./calc_in/'+f)
+                raise SystemExit(1)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/ASE/collect_ase.py` & `csp-cryspy-1.2.0/src/cryspy/interface/ASE/collect_ase.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 '''
 Collect results in ASE
 '''
 
+from logging import getLogger
+
 import numpy as np
 from pymatgen.core import Structure
 
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def collect_ase(current_id, work_path):
     # ---------- etc
     magmom = np.nan
     check_opt = 'no_file'    # always no_file in ASE for now
     # ---------- collect energy
     try:
         with open(work_path+'log.tote') as f:
             lines = f.readlines()
         energy = float(lines[-1].split()[0])    # in eV/cell
         energy = energy/float(rin.natot)    # eV/cell --> eV/atom
     except Exception as e:
         energy = np.nan    # error
-        print(e, '    Structure ID {0}, could not obtain energy from {1}'.format(
-            current_id, 'log.tote'))
+        logger.warning(e.args[0] + f':    Structure ID {current_id}, could not obtain energy from log.tote')
     # ---------- collect CONTCAR
     try:
         opt_struc = Structure.from_file(work_path+'CONTCAR')
     except Exception:
         opt_struc = None
     # ---------- check
     if np.isnan(energy):
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/ASE/ctrl_job_ase.py` & `csp-cryspy-1.2.0/src/cryspy/interface/ASE/ctrl_job_ase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 '''
 Control jobs in ASE
 '''
 
+from logging import getLogger
 import os
 import shutil
 
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def next_stage_ase(stage, work_path):
     # ---------- skip_flag
     skip_flag = False
 
     # ---------- rename ASE files at the current stage
     ase_files = ['POSCAR', 'CONTCAR', 'log.tote']
-    for f in vasp_files:
+    for f in ase_files:
         if not os.path.isfile(work_path+f):
-            raise IOError('Not found '+work_path+f)
+            logger.error('Not found '+work_path+f)
+            raise SystemExit(1)
         os.rename(work_path+f, work_path+'stage{}_'.format(stage)+f)
 
     # ---------- cp CONTCAR POSCAR
     shutil.copyfile(work_path+'stage{}_CONTCAR'.format(stage),
                     work_path+'POSCAR')
 
     # ---------- copy the input file from ./calc_in for the next stage
@@ -37,22 +41,23 @@
 
 def next_struc_ase(structure, current_id, work_path):
     # ---------- copy files
     calc_inputs = [rin.ase_python]
     for f in calc_inputs:
         ff = f+'_1' if f == rin.ase_python else f
         if not os.path.isfile('./calc_in/' + ff):
-            raise IOError('Could not find ./calc_in/' + ff)
+            logger.error('Could not find ./calc_in/' + ff)
+            raise SystemExit(1)
         # ------ e.g. cp ./calc_in/INCAR_1 work0001/INCAR
         shutil.copyfile('./calc_in/'+ff, work_path+f)
 
     # ---------- generate POSCAR
     structure.to(fmt='poscar', filename=work_path+'POSCAR')
     if not os.path.isfile(work_path+'POSCAR'):
-        raise IOError('Could not find {}POSCAR'.format(work_path))
+        logger.error(f'Could not find {work_path}POSCAR')
 
     # ---------- Change the title of POSCAR
     with open(work_path+'POSCAR', 'r') as f:
         lines = f.readlines()
     lines[0] = 'ID_{}\n'.format(current_id)
     with open(work_path+'POSCAR', 'w') as f:
         for line in lines:
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/calc_files_lammps.py` & `csp-cryspy-1.2.0/src/cryspy/interface/soiap/calc_files_soiap.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 '''
-Calculation files in LAMMPS
+Calculation files in soiap
 '''
 
+from logging import getLogger
 import os
 
 from ...IO import read_input as rin
 
 
-def check_input_lammps():
-    # ---------- prepare rin.jobfile, rin.lammps_potential, rin.rammps_infile
-    if rin.lammps_potential is None:
-        calc_inputs = [rin.jobfile, rin.lammps_infile]
-    else:
-        calc_inputs = [rin.jobfile, rin.lammps_infile] + rin.lammps_potential
+logger = getLogger('cryspy')
+
+def check_input_soiap():
+    # ---------- prepare rin.jobfile, rin.soiap_infile
+    calc_inputs = [rin.jobfile, rin.soiap_infile]
 
     # ----- check required files
     for f in calc_inputs:
-        if f == rin.lammps_infile:
-            finfiles = [rin.lammps_infile + '_{}'.format(i) for i in range(
-                1, rin.nstage+1)]
+        if f == rin.soiap_infile:
+            finfiles = [rin.soiap_infile + '_{}'.format(i)
+                        for i in range(1, rin.nstage+1)]
             for ff in finfiles:
                 if not os.path.isfile('./calc_in/'+ff):
-                    raise IOError('Could not find ./calc_in/'+ff)
+                    logger.error('Could not find ./calc_in/'+ff)
+                    raise SystemExit(1)
         else:
             if not os.path.isfile('./calc_in/'+f):
-                raise IOError('Could not find ./calc_in/'+f)
+                logger.error('Could not find ./calc_in/'+f)
+                raise SystemExit(1)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/collect_lammps.py` & `csp-cryspy-1.2.0/src/cryspy/interface/LAMMPS/collect_lammps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 '''
 Collect results in LAMMPS
 '''
 
+from logging import getLogger
 import numpy as np
 
 from . import structure as lammps_structure
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def collect_lammps(current_id, work_path):
     # ---------- check optimization in current stage & obtain energy
     energy = np.nan
     check_opt = 'not_yet'
     try:
         with open(work_path+rin.lammps_outfile, 'r') as fout:
             lines = fout.readlines()
         for i, line in enumerate(lines):
             if 'ERROR:' in line:
-                print('    ' + line.rstrip())
+                logger.warning('    ' + line.rstrip())
                 energy = np.nan
                 check_opt = 'not_yet'
                 break
             elif 'Minimization stats:' in line:
                 energy = float(lines[i+3].split()[2])  # in eV (units is metal)
                 energy = energy/float(rin.natot)    # eV/cell --> eV/atom
                 check_opt = 'done'
     except Exception as e:
-        print(e)
-        print('    Structure ID {0}, could not obtain energy from {1}'.format(
-            current_id, rin.lammps_outfile))
+        logger.warning(e.args[0] + f':    Structure ID {current_id},'
+                       f'could not obtain energy from {rin.lammps_outfile}')
         energy = np.nan    # error
         check_opt = 'no_file'
 
     # ---------- obtain magmom
     magmom = np.nan    # magnetic moment is not calculated
 
     # ---------- collect the last structure
     try:
         opt_struc = lammps_structure.from_file(work_path+'log.struc')
     except Exception as e:
-        print(e)
+        logger.warning(e.args[0])
         opt_struc = None
 
     # ---------- return
     return opt_struc, energy, magmom, check_opt
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py` & `csp-cryspy-1.2.0/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 '''
 Control jobs in LAMMPS
 '''
 
+from logging import getLogger
 import os
 import shutil
 
 from . import structure as lammps_structure
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def next_stage_lammps(stage, work_path):
     # ---------- skip_flag
     skip_flag = False
 
     # ---------- rename lammps files at the current stage
     lammps_files = [rin.lammps_infile, rin.lammps_outfile,
                     rin.lammps_data, 'log.struc']
     for f in lammps_files:
         if not os.path.isfile(work_path+f):
-            raise IOError('Not found '+work_path+f)
+            logger.error('Not found '+work_path+f)
+            raise SystemExit(1)
         os.rename(work_path+f, work_path+'stage{}_'.format(stage)+f)
 
     # ---------- copy the input file from ./calc_in for the next stage
     finfile = './calc_in/'+rin.lammps_infile+'_{}'.format(stage + 1)
     shutil.copyfile(finfile, work_path+rin.lammps_infile)
 
     # ---------- generate the structure data file
     try:
         structure = lammps_structure.from_file(
             work_path+'stage{}_log.struc'.format(stage))
     except ValueError:
         skip_flag = True
-        print('    error in lammps,  skip this structure')
+        logger.warning('    error in lammps,  skip this structure')
         return skip_flag
     with open(work_path+'stage{}_'.format(stage)+rin.lammps_data, 'r') as f:
         lines = f.readlines()
     title = lines[0][7:]    # string following 'data_'
     lammps_structure.write(structure,
                            work_path+rin.lammps_data,
                            title=title)
@@ -49,14 +53,15 @@
     if rin.lammps_potential is None:
         calc_inputs = [rin.lammps_infile]
     else:
         calc_inputs = [rin.lammps_infile] + rin.lammps_potential
     for f in calc_inputs:
         ff = f+'_1' if f == rin.lammps_infile else f
         if not os.path.isfile('./calc_in/'+ff):
-            raise IOError('Could not find ./calc_in/'+ff)
+            logger.error('Could not find ./calc_in/'+ff)
+            raise SystemExit(1)
         shutil.copyfile('./calc_in/'+ff, work_path+f)
 
     # ---------- generate the structure data file
     lammps_structure.write(structure,
                            work_path+rin.lammps_data,
                            title='ID_{0:d}'.format(current_id))
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/LAMMPS/structure.py` & `csp-cryspy-1.2.0/src/cryspy/interface/LAMMPS/structure.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/OMX/calc_files_OMX.py` & `csp-cryspy-1.2.0/src/cryspy/interface/LAMMPS/calc_files_lammps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 '''
-Calculation files in OpenMX
-written by H. Sawahata 2020/03/09
-info at hikaruri.jp
+Calculation files in LAMMPS
 '''
 
+from logging import getLogger
 import os
 
 from ...IO import read_input as rin
 
 
-def check_input_OMX():
-    # ---------- prepare rin.jobfile, rin.OMX_infile
-    calc_inputs = [rin.jobfile, rin.OMX_infile]
+logger = getLogger('cryspy')
 
-    # ------ check required files
+def check_input_lammps():
+    # ---------- prepare rin.jobfile, rin.lammps_potential, rin.rammps_infile
+    if rin.lammps_potential is None:
+        calc_inputs = [rin.jobfile, rin.lammps_infile]
+    else:
+        calc_inputs = [rin.jobfile, rin.lammps_infile] + rin.lammps_potential
+
+    # ----- check required files
     for f in calc_inputs:
-        if f == rin.OMX_infile:
-            finfiles = [rin.OMX_infile + '_{}'.format(i) for i in range(
+        if f == rin.lammps_infile:
+            finfiles = [rin.lammps_infile + '_{}'.format(i) for i in range(
                 1, rin.nstage+1)]
             for ff in finfiles:
-                if not os.path.isfile('./calc_in/' + ff):
-                    raise IOError('Could not find ./calc_in/' + ff)
+                if not os.path.isfile('./calc_in/'+ff):
+                    logger.error('Could not find ./calc_in/'+ff)
+                    raise SystemExit(1)
         else:
-            if not os.path.isfile('./calc_in/' + f):
-                raise IOError('Could not find ./calc_in/' + f)
+            if not os.path.isfile('./calc_in/'+f):
+                logger.error('Could not find ./calc_in/'+f)
+                raise SystemExit(1)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/OMX/collect_OMX.py` & `csp-cryspy-1.2.0/src/cryspy/interface/OMX/collect_OMX.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 '''
 Collect results in OpenMX
 written  by  H. Sawahata 2020/03/09
 info at hikaruri.jp
 '''
 
+from logging import getLogger
+
 import numpy as np
 import re
 from pymatgen.core.units import Energy
 
 from . import structure as OMX_structure
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def collect_OMX(current_id, work_path):
     # ---------- check optimization in previous stage (done)
     # If *.out file exists, the calculation is done.
     try:
         with open(work_path+rin.OMX_outfile, 'r') as fpout:
             lines = fpout.readlines()
         check_opt = 'done'
     except Exception as e:
-        print(e)
+        logger.warning(e.args[0])
         check_opt = 'no_file'
 
     # ---------- obtain energy and magmom (done)
     try:
         with open(work_path+rin.OMX_outfile, 'r') as fpout:
             lines = fpout.readlines()
         energy = np.nan
@@ -39,17 +43,16 @@
             if line.find("muB") >= 0:
                 muB = line.split()
                 magmom = float(muB[4])
                 break
     except Exception as e:
         energy = np.nan    # error
         magmom = np.nan    # error
-        print(e)
-        print(' Structure ID {0}, could not obtain energy from {1}'.format(
-            current_id, rin.OMX_outfile))
+        logger.warning(e.args[0] + f':    Structure ID {current_id},'
+                       f' could not obtain energy from {rin.OMX_outfile}')
 
     # ---------- collect the last structure (yet)
     try:
         lines_cell = OMX_structure.extract_cell_parameters_from_outfile(
             work_path+rin.OMX_outfile)
         if lines_cell is None:
             lines_cell = OMX_structure.extract_cell_parameters_from_infile(
@@ -61,15 +64,15 @@
                 work_path+rin.OMX_infile)
         opt_struc = OMX_structure.from_lines(lines_cell, lines_atom)
         # ------ opt_OMX-structure
         with open('./data/opt_OMX-structure', 'a') as fstruc:
             fstruc.write('# ID {0:d}\n'.format(current_id))
         OMX_structure.write(opt_struc, './data/opt_OMX-structure', mode='a')
     except Exception as e:
-        print(e)
+        logger.warning(e.args[0])
         opt_struc = None
 
     # ---------- check
     if np.isnan(energy):
         opt_struc = None
     if opt_struc is None:
         energy = np.nan
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/OMX/ctrl_job_OMX.py` & `csp-cryspy-1.2.0/src/cryspy/interface/OMX/ctrl_job_OMX.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 '''
 Control jobs in OpenMX
 written by H. Sawahata 2020/03/09
 info at hikaruri.jp
 '''
 
+from logging import getLogger
 import os
 import shutil
 
 from pymatgen.io.vasp.sets import MITRelaxSet
 
 from . import structure as OMX_structure
 from ...IO.out_results import out_kpts
 from ...IO import pkl_data
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def next_stage_OMX(stage, work_path, kpt_data, current_id):
     # ---------- skip_flag
     skip_flag = False
 
     # ---------- rename OpenMX files at the current stage
     OMX_files = [rin.OMX_infile, rin.OMX_outfile]
     for f in OMX_files:
         if not os.path.isfile(work_path+f):
-            raise IOError('Not found '+work_path+f)
+            logger.error('Not found '+work_path+f)
+            raise SystemExit(1)
         os.rename(work_path+f, work_path+'stage{}_'.format(stage)+f)
 
     # ---------- next structure
     try:
         lines_cell = OMX_structure.extract_cell_parameters_from_outfile(
             work_path+'stage{}_'.format(stage)+rin.OMX_outfile)
         if lines_cell is None:
@@ -40,15 +44,15 @@
                 work_path+'stage{}_'.format(stage)+rin.OMX_infile)
         structure = OMX_structure.from_lines(lines_cell, lines_atom)
     except ValueError:
         skip_flag = True
         kpt_data[current_id].append(['skip'])
         pkl_data.save_kpt(kpt_data)
         out_kpts(kpt_data)
-        print('    error in OpenMX,  skip this structure')
+        logger.info(f'    error in OpenMX,  skip structure {current_id}')
         return skip_flag, kpt_data
 
     # ---------- copy the input file from ./calc_in for the next stage
     finput = './calc_in/'+rin.OMX_infile+'_{}'.format(stage + 1)
     shutil.copyfile(finput, work_path+rin.OMX_infile)
 
     # ---------- append structure info.
@@ -78,15 +82,16 @@
 
 def next_struc_OMX(structure, current_id, work_path, kpt_data):
     # ---------- copy files
     calc_inputs = [rin.OMX_infile]
     for f in calc_inputs:
         ff = f+'_1' if f == rin.OMX_infile else f
         if not os.path.isfile('./calc_in/' + ff):
-            raise IOError('Could not find ./calc_in/' + ff)
+            logger.error('Could not find ./calc_in/' + ff)
+            raise SystemExit(1)
         shutil.copyfile('./calc_in/'+ff, work_path+f)
 
     # ---------- append structure info. to the input file
     with open(work_path+rin.OMX_infile, 'a') as fin:
         fin.write('\n')
     OMX_structure.write(structure, work_path+rin.OMX_infile, mode='a')
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/OMX/structure.py` & `csp-cryspy-1.2.0/src/cryspy/interface/OMX/structure.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/QE/calc_files_qe.py` & `csp-cryspy-1.2.0/src/cryspy/interface/QE/calc_files_qe.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 '''
 Calculation files in Quantum ESPRESSO
 '''
 
+from logging import getLogger
 import os
 
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def check_input_qe():
     # ---------- prepare rin.jobfile, rin.qe_infile
     calc_inputs = [rin.jobfile, rin.qe_infile]
 
     # ------ check required files
     for f in calc_inputs:
         if f == rin.qe_infile:
             finfiles = [rin.qe_infile + '_{}'.format(i) for i in range(
                 1, rin.nstage+1)]
             for ff in finfiles:
                 if not os.path.isfile('./calc_in/' + ff):
-                    raise IOError('Could not find ./calc_in/' + ff)
+                    logger.error('Could not find ./calc_in/' + ff)
+                    raise SystemExit(1)
         else:
             if not os.path.isfile('./calc_in/' + f):
-                raise IOError('Could not find ./calc_in/' + f)
+                logger.error('Could not find ./calc_in/' + f)
+                raise SystemExit(1)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/QE/collect_qe.py` & `csp-cryspy-1.2.0/src/cryspy/interface/QE/collect_qe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 '''
 Collect results in Quantum ESPRESSO
 '''
 
+from logging import getLogger
 import sys
 
 import numpy as np
 from pymatgen.core import Structure
 
 from . import structure as qe_structure
 from ...util import constants
 from ...IO import pkl_data
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def collect_qe(current_id, work_path):
     # ---------- check optimization in previous stage
     try:
         with open(work_path+rin.qe_outfile, 'r') as fpout:
             lines = fpout.readlines()
         check_opt = 'not_yet'
         for line in lines:
             if 'End final coordinates' in line:
                 check_opt = 'done'
     except Exception as e:
-        print(e)
+        logger.warning(e.args[0])
         check_opt = 'no_file'
 
     # ---------- obtain energy and magmom
     try:
         with open(work_path+rin.qe_outfile, 'r') as fpout:
             lines = fpout.readlines()
         energy = np.nan
@@ -41,17 +44,16 @@
             if line.find("total magnetization") >= 0:
                 muB = line.split()
                 magmom = float(muB[3])
                 break
     except Exception as e:
         energy = np.nan    # error
         magmom = np.nan    # error
-        print(e)
-        print('    Structure ID {0}, could not obtain energy from {1}'.format(
-            current_id, rin.qe_outfile))
+        logger.warning(e.args[0] + f':    Structure ID {current_id},'
+                       f'could not obtain energy from {rin.qe_outfile}')
 
     # ---------- collect the last structure
     try:
         lines_cell = qe_structure.extract_cell_parameters(
             work_path+rin.qe_outfile)
         if lines_cell is None:
             lines_cell = qe_structure.extract_cell_parameters(
@@ -64,15 +66,15 @@
         opt_struc = qe_structure.from_lines(lines_cell, lines_atom)
 
         # ------ opt_qe-structure
         with open('./data/opt_qe-structure', 'a') as fstruc:
             fstruc.write('# ID {0:d}\n'.format(current_id))
         qe_structure.write(opt_struc, './data/opt_qe-structure', mode='a')
     except Exception as e:
-        print(e)
+        logger.warning(e.args[0])
         opt_struc = None
 
     # ---------- check
     if np.isnan(energy):
         opt_struc = None
     if opt_struc is None:
         energy = np.nan
@@ -108,23 +110,21 @@
                 vc_flag = True
         # ------ delete last energy (after End final coordinates)
         if final_flag and vc_flag:
             energy_step.pop(-1)
         # ------ list --> array, Ry/cell --> eV/atom
         if not energy_step:
             energy_step = None    # if empty
-            print('#### ID: {0}: failed to parse energy_step\n'.format(
-                current_id), file=sys.stderr)
+            logger.warning(f'#### ID: {current_id}: failed to parse energy_step')
         else:
             energy_step = constants.RY2EV / rin.natot * np.array(energy_step,
                                                                dtype='float')
     except Exception as e:
         energy_step = None
-        print(e, '#### ID: {0}: failed to parse energy_step\n'.format(
-            current_id), file=sys.stderr)
+        logger.warning(e.args[0] + f'#### ID: {current_id}: failed to parse energy_step')
 
     # ---------- append energy_step
     if energy_step_data.get(current_id) is None:
         energy_step_data[current_id] = []    # initialize
     energy_step_data[current_id].append(energy_step)
 
     # ---------- save energy_step_data
@@ -151,16 +151,15 @@
         _extract_struc_qe(work_path+rin.qe_infile, struc_step)
         # ------ struc step from pwscf.out
         _extract_struc_qe(work_path+rin.qe_outfile, struc_step)
         # ------ delete last structure due to duplication
         struc_step.pop(-1)
     except Exception as e:
         struc_step = None
-        print(e ,'#### ID: {0}: failed to parse in struc_step\n'.format(
-            current_id), file=sys.stderr)
+        logger.warning(e.args[0] + f'#### ID: {current_id}: failed to parse in struc_step')
 
     # ---------- append struc_step_data
     if struc_step_data.get(current_id) is None:
         struc_step_data[current_id] = []    # initialize
     struc_step_data[current_id].append(struc_step)
 
     # ---------- save struc_step_data
@@ -245,20 +244,18 @@
                 vc_flag = True
         # ------ delete last energy (after End final coordinates)
         if final_flag and vc_flag:
             force_step.pop(-1)
         # ------ if empty
         if len(force_step) == 0:
             force_step = None
-            print('#### ID: {0}: failed to parse force_step\n'.format(
-                current_id), file=sys.stderr)
+            logger.warning(f'#### ID: {current_id}: failed to parse force_step')
     except Exception as e:
         force_step = None
-        print(e, '#### ID: {0}: failed to parse in force_step\n'.format(
-            current_id), file=sys.stderr)
+        logger.warning(e + f'#### ID: {current_id}: failed to parse in force_step')
 
     # ---------- append force_step
     if force_step_data.get(current_id) is None:
         force_step_data[current_id] = []    # initialize
     force_step_data[current_id].append(force_step)
 
     # ---------- save force_step_data
@@ -305,20 +302,18 @@
                 vc_flag = True
         # ------ delete last energy (after End final coordinates)
         if final_flag and vc_flag:
             stress_step.pop(-1)
         # ------ if empty
         if len(stress_step) == 0:
             stress_step = None
-            print('#### ID: {0}: failed to parse stress_step\n'.format(
-                current_id), file=sys.stderr)
+            logger.warning(f'#### ID: {current_id}: failed to parse stress_step')
     except Exception as e:
         stress_step = None
-        print(e, '#### ID: {0}: failed to parse in stress_step\n'.format(
-            current_id), file=sys.stderr)
+        logger.warning(e + f'#### ID: {current_id}: failed to parse in stress_step')
 
     # ---------- append stress_step
     if stress_step_data.get(current_id) is None:
         stress_step_data[current_id] = []    # initialize
     stress_step_data[current_id].append(stress_step)
 
     # ---------- save stress_step_data
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/QE/ctrl_job_qe.py` & `csp-cryspy-1.2.0/src/cryspy/interface/QE/ctrl_job_qe.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 '''
 Control jobs in Quantum ESPRESSO
 '''
 
+from logging import getLogger
 import os
 import shutil
 
 from pymatgen.io.vasp.sets import MITRelaxSet
 
 from . import structure as qe_structure
 from ...IO.out_results import out_kpts
 from ...IO import pkl_data
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def next_stage_qe(stage, work_path, kpt_data, current_id):
     # ---------- skip_flag
     skip_flag = False
 
     # ---------- rename QE files at the current stage
     qe_files = [rin.qe_infile, rin.qe_outfile]
     for f in qe_files:
         if not os.path.isfile(work_path+f):
-            raise IOError('Not found '+work_path+f)
+            logger.error('Not found '+work_path+f)
+            raise SystemExit(1)
         os.rename(work_path+f, work_path+'stage{}_'.format(stage)+f)
 
     # ---------- next structure
     try:
         lines_cell = qe_structure.extract_cell_parameters(
             work_path+'stage{}_'.format(stage)+rin.qe_outfile)
         if lines_cell is None:
@@ -38,15 +42,15 @@
                 work_path+'stage{}_'.format(stage)+rin.qe_infile)
         structure = qe_structure.from_lines(lines_cell, lines_atom)
     except ValueError:
         skip_flag = True
         kpt_data[current_id].append(['skip'])
         pkl_data.save_kpt(kpt_data)
         out_kpts(kpt_data)
-        print('    error in QE,  skip this structure')
+        logger.info(f'    error in QE,  skip structure {current_id}')
         return skip_flag, kpt_data
 
     # ---------- copy the input file from ./calc_in for the next stage
     finput = './calc_in/'+rin.qe_infile+'_{}'.format(stage + 1)
     shutil.copyfile(finput, work_path+rin.qe_infile)
 
     # ---------- append structure info.
@@ -76,15 +80,16 @@
 
 def next_struc_qe(structure, current_id, work_path, kpt_data):
     # ---------- copy files
     calc_inputs = [rin.qe_infile]
     for f in calc_inputs:
         ff = f+'_1' if f == rin.qe_infile else f
         if not os.path.isfile('./calc_in/' + ff):
-            raise IOError('Could not find ./calc_in/' + ff)
+            logger.error('Could not find ./calc_in/' + ff)
+            raise SystemExit(1)
         shutil.copyfile('./calc_in/'+ff, work_path+f)
 
     # ---------- append structure info. to the input file
     with open(work_path+rin.qe_infile, 'a') as fin:
         fin.write('\n')
     qe_structure.write(structure, work_path+rin.qe_infile, mode='a')
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/QE/structure.py` & `csp-cryspy-1.2.0/src/cryspy/interface/QE/structure.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 '''
 Structure file for Quantum ESPRESSO
 '''
 
+from logging import getLogger
+
 from pymatgen.core import Structure
 from pymatgen.core.units import Length
 
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def extract_cell_parameters(filename):
     # ---------- last CELL_PARAMETERS
     with open(filename, 'r') as f:
         lines = f.readlines()
     lines_cell = None
     for i, line in enumerate(reversed(lines)):
         if 'CELL_PARAMETERS' in line:
@@ -45,16 +49,16 @@
         scale = float(unit[unit.index('=')+1:])    # in Bohr
         scale = float(Length(scale, 'bohr').to('ang'))    # in Ang
     elif unit == 'bohr':
         scale = float(Length(1.0, 'bohr').to('ang'))    # in Ang
     elif unit == 'angstrom':
         scale = 1.0    # in Ang
     else:
-        raise ValueError('unit "{0:s}" for CELL_PARAMETERS'
-                         ' is not supported'.format(unit))
+        logger.error(f'unit "{unit:s}" for CELL_PARAMETERS'
+                         ' is not supported')
     lattice = [[scale * float(x) for x in line.split()]
                for line in lines_cell[1:4]]
 
     # ---------- species & coordinates
     unit = lines_atom[0].split()[1]
     if unit[0] == '(' and unit[-1] == ')':
         unit = unit[1:-1]
@@ -63,16 +67,16 @@
     for line in lines_atom[1:]:
         fields = line.split()
         species.append(fields[0])
         coords.append([float(x) for x in fields[1:4]])
         if unit == 'crystal':
             pass    # 'coords' are already internal coordinates
         else:
-            raise ValueError('unit "{0:s}" for ATOMIC_POSITIONS'
-                             ' is not supported yet'.format(unit))
+            logger.error(f'unit "{unit:s}" for ATOMIC_POSITIONS'
+                             ' is not supported yet')
 
     structure = Structure(lattice, species, coords)
     return structure
 
 
 def write(structure, output, mode='w'):
     # ---------- get in POSCAR format
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/VASP/calc_files_vasp.py` & `csp-cryspy-1.2.0/src/cryspy/interface/VASP/calc_files_vasp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 '''
 Calculation files in VASP
 '''
 
+from logging import getLogger
 import os
 
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def check_input_vasp():
     # ---------- prepare rin.jobfile, POTCAR, INCAR
     calc_inputs = [rin.jobfile, 'POTCAR', 'INCAR']
 
     # ------ check required files
     for f in calc_inputs:
         if f == 'INCAR':
             fincars = ['INCAR_{}'.format(i) for i in range(1, rin.nstage+1)]
             for ff in fincars:
                 if not os.path.isfile('./calc_in/' + ff):
-                    raise IOError('Could not find ./calc_in/' + ff)
+                    logger.error('Could not find ./calc_in/' + ff)
+                    raise SystemExit(1)
         else:
             if not os.path.isfile('./calc_in/' + f):
-                raise IOError('Could not find ./calc_in/' + f)
+                logger.error('Could not find ./calc_in/' + f)
+                raise SystemExit(1)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/VASP/collect_vasp.py` & `csp-cryspy-1.2.0/src/cryspy/interface/VASP/collect_vasp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 '''
 Collect results in VASP
 '''
 
+from logging import getLogger
 import os
 import sys
 import xml.etree.ElementTree as ET
 
 import numpy as np
 from pymatgen.core import Structure
 
 from ...util import constants
 from ...IO import pkl_data
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def collect_vasp(current_id, work_path):
     # ---------- check optimization
     check_opt = check_opt_vasp(work_path+'OUTCAR')
     # ---------- obtain energy and magmom
     energy, magmom = get_energy_magmom_vasp(work_path)
     if np.isnan(energy):
-        print('    Structure ID {0},'
-              ' could not obtain energy from OSZICAR'.format(current_id))
+        logger.warning(f'    Structure ID {current_id},'
+              ' could not obtain energy from OSZICAR')
     # ---------- collect CONTCAR
     try:
         opt_struc = Structure.from_file(work_path+'CONTCAR')
     except Exception:
         opt_struc = None
     # ---------- check
     if np.isnan(energy):
@@ -92,21 +95,21 @@
         for cal in cals:
             eng = cal.find('energy')    # first 'energy' child node
             fr_eng = eng.find('i')    # first 'i' tag is free energy
 
             if fr_eng.attrib['name'] == 'e_fr_energy':
                 energy_step.append(fr_eng.text)
             else:
-                raise ValueError('bug')
+                logger.error('bug in get_energy_step_vasp')
+                raise SystemExit(1)
         # ------ list, str --> array
         energy_step = np.array(energy_step, dtype='float')/float(rin.natot)
     except Exception as e:
         energy_step = None
-        print(e, '#### ID: {0}: failed to parse in energy_step\n'.format(
-            current_id), file=sys.stderr)
+        logger.warning(e.args[0] + f': #### ID: {current_id}: failed to parse in energy_step')
 
     # ---------- append energy_step
     if energy_step_data.get(current_id) is None:
         energy_step_data[current_id] = []    # initialize
     energy_step_data[current_id].append(energy_step)
 
     # ---------- save energy_step_data
@@ -155,16 +158,15 @@
                 incoord.append([float(x) for x in a.text.split()])
             # -- structure in pymatgen format
             struc = Structure(lattice, atomlist, incoord)
             # -- append
             struc_step.append(struc)
     except Exception as e:
         struc_step = None
-        print(e, '#### ID: {0}: failed to parse in struc_step\n'.format(
-            current_id), file=sys.stderr)
+        logger.warning(e.args[0], f': #### ID: {current_id}: failed to parse in struc_step')
 
     # ---------- append struc_step
     if struc_step_data.get(current_id) is None:
         struc_step_data[current_id] = []    # initialize
     struc_step_data[current_id].append(struc_step)
 
     # ---------- save struc_step_data
@@ -208,16 +210,15 @@
                         force.append(v.text.split())
             # -- list, str --> array
             force = np.array(force, dtype='float')
             # -- appned force_step
             force_step.append(force)
     except Exception as e:
         force_step = None
-        print(e, '#### ID: {0}: failed to parse in force_step\n'.format(
-            current_id), file=sys.stderr)
+        logger.warning(e.args[0] + f': #### ID: {current_id}: failed to parse in force_step')
 
     # ---------- append force_step
     if force_step_data.get(current_id) is None:
         force_step_data[current_id] = []    # initialize
     force_step_data[current_id].append(force_step)
 
     # ---------- save force_step_data
@@ -263,16 +264,15 @@
             stress = np.array(stress, dtype='float')
             # -- kbar --> eV/ang**3
             stress = stress * constants.KBAR2eV_ANG3
             # -- appned stress_step
             stress_step.append(stress)
     except Exception as e:
         stress_step = None
-        print(e, '#### ID: {0}: failed to parse in stress_step\n'.format(
-            current_id), file=sys.stderr)
+        logger.warning(e.args[0], f': #### ID: {current_id}: failed to parse in stress_step')
 
     # ---------- append stress_step
     if stress_step_data.get(current_id) is None:
         stress_step_data[current_id] = []    # initialize
     stress_step_data[current_id].append(stress_step)
 
     # ---------- save stress_step_data
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/VASP/ctrl_job_vasp.py` & `csp-cryspy-1.2.0/src/cryspy/interface/VASP/ctrl_job_vasp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 '''
 Control jobs in VASP
 '''
 
+from logging import getLogger
 import os
 import shutil
 
 from pymatgen.core import Structure
 from pymatgen.io.vasp.sets import MITRelaxSet
 
 from ...IO.out_results import out_kpts
 from ...IO import pkl_data
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def next_stage_vasp(stage, work_path, kpt_data, current_id):
     # ---------- skip_flag
     skip_flag = False
 
     # ---------- rename VASP files at the current stage
     vasp_files = ['POSCAR', 'KPOINTS', 'CONTCAR',
                   'OUTCAR', 'OSZICAR', 'vasprun.xml']
     for f in vasp_files:
         if not os.path.isfile(work_path+f):
-            raise IOError('Not found '+work_path+f)
+            logger.error('Not found '+work_path+f)
+            raise SystemExit(1)
         os.rename(work_path+f, work_path+'stage{}_'.format(stage)+f)
 
     # ---------- cp CONTCAR POSCAR
     shutil.copyfile(work_path+'stage{}_CONTCAR'.format(stage),
                     work_path+'POSCAR')
 
     # ---------- remove STOPCAR
@@ -37,15 +41,15 @@
     try:
         structure = Structure.from_file(work_path+'POSCAR')
     except ValueError:
         skip_flag = True
         kpt_data[current_id].append(['skip'])
         pkl_data.save_kpt(kpt_data)
         out_kpts(kpt_data)
-        print('    error in VASP,  skip this structure')
+        logger.info(f'    error in VASP,  skip structure {current_id}')
         return skip_flag, kpt_data
     mitparamset = MITRelaxSet(structure)
     # kppvol[0]: <--> stage 1, kppvol[1] <--> stage2, ...
     #   so (stage - 1): current stage, stage: next stage in kppvol
     kpoints = mitparamset.kpoints.automatic_density_by_vol(structure,
                                                            rin.kppvol[stage],
                                                            rin.force_gamma)
@@ -66,22 +70,24 @@
 
 def next_struc_vasp(structure, current_id, work_path, kpt_data):
     # ---------- copy files
     calc_inputs = ['POTCAR', 'INCAR']
     for f in calc_inputs:
         ff = f+'_1' if f == 'INCAR' else f
         if not os.path.isfile('./calc_in/' + ff):
-            raise IOError('Could not find ./calc_in/' + ff)
+            logger.error('Could not find ./calc_in/' + ff)
+            raise SystemExit(1)
         # ------ e.g. cp ./calc_in/INCAR_1 work0001/INCAR
         shutil.copyfile('./calc_in/'+ff, work_path+f)
 
     # ---------- generate POSCAR
     structure.to(fmt='poscar', filename=work_path+'POSCAR')
     if not os.path.isfile(work_path+'POSCAR'):
-        raise IOError('Could not find {}POSCAR'.format(work_path))
+        logger.error('Could not find {}POSCAR'.format(work_path))
+        raise SystemExit(1)
 
     # ---------- Change the title of POSCAR
     with open(work_path+'POSCAR', 'r') as f:
         lines = f.readlines()
     lines[0] = 'ID_{}\n'.format(current_id)
     with open(work_path+'POSCAR', 'w') as f:
         for line in lines:
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/select_code.py` & `csp-cryspy-1.2.0/src/cryspy/interface/select_code.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,24 +4,35 @@
     - QE
     - OMX
     - soiap
     - LAMMPS
     - ASE
 '''
 
-from .VASP import calc_files_vasp, ctrl_job_vasp, collect_vasp
-from .QE import calc_files_qe, ctrl_job_qe, collect_qe
-from .soiap import calc_files_soiap, ctrl_job_soiap, collect_soiap
-from .LAMMPS import calc_files_lammps, ctrl_job_lammps, collect_lammps
-from .OMX import calc_files_OMX, ctrl_job_OMX, collect_OMX
-from .ASE import calc_files_ase, ctrl_job_ase, collect_ase
-from .ext import collect_ext
+from logging import getLogger
 
 from ..IO import read_input as rin
 
+if rin.calc_code == 'VASP':
+    from .VASP import calc_files_vasp, ctrl_job_vasp, collect_vasp
+elif rin.calc_code == 'QE':
+    from .QE import calc_files_qe, ctrl_job_qe, collect_qe
+elif rin.calc_code == 'OMX':
+    from .OMX import calc_files_OMX, ctrl_job_OMX, collect_OMX
+elif rin.calc_code == 'soiap':
+    from .soiap import calc_files_soiap, ctrl_job_soiap, collect_soiap
+elif rin.calc_code == 'LAMMPS':
+    from .LAMMPS import calc_files_lammps, ctrl_job_lammps, collect_lammps
+elif rin.calc_code == 'ASE':
+    from .ASE import calc_files_ase, ctrl_job_ase, collect_ase
+elif rin.calc_code == 'ext':
+    from .ext import collect_ext
+
+
+logger = getLogger('cryspy')
 
 def check_calc_files():
     if rin.calc_code == 'VASP':
         calc_files_vasp.check_input_vasp()
     elif rin.calc_code == 'QE':
         calc_files_qe.check_input_qe()
     elif rin.calc_code == 'OMX':
@@ -31,15 +42,16 @@
     elif rin.calc_code == 'LAMMPS':
         calc_files_lammps.check_input_lammps()
     elif rin.calc_code == 'ASE':
         calc_files_ase.check_input_ase()
     elif rin.calc_code == 'ext':
         pass
     else:
-        raise NotImplementedError()
+        logger.error(f'{rin.calc_code}: not implemented yet')
+        raise SystemExit(1)
 
 
 def next_stage(stage, work_path, *args):
     # args[0] <-- kpt_data
     # args[1] <-- current_id for kpt_data
     if rin.calc_code == 'VASP':
         skip_flag, kpt_data = ctrl_job_vasp.next_stage_vasp(stage, work_path,
@@ -59,15 +71,16 @@
     elif rin.calc_code == 'LAMMPS':
         skip_flag = ctrl_job_lammps.next_stage_lammps(stage, work_path)
         return skip_flag
     elif rin.calc_code == 'ASE':
         skip_flag = ctrl_job_ase.next_stage_ase(stage, work_path)
         return skip_flag
     else:
-        raise NotImplementedError()
+        logger.error(f'{rin.calc_code}: not implemented yet')
+        raise SystemExit(1)
 
 
 def collect(current_id, work_path):
     if rin.calc_code == 'VASP':
         opt_struc, energy, magmom, check_opt = \
             collect_vasp.collect_vasp(current_id, work_path)
     elif rin.calc_code == 'QE':
@@ -85,15 +98,16 @@
     elif rin.calc_code == 'ASE':
         opt_struc, energy, magmom, check_opt = \
             collect_ase.collect_ase(current_id, work_path)
     elif rin.calc_code == 'ext':
         ext_opt_struc_data, ext_energy_data = collect_ext.collect_ext()
         return ext_opt_struc_data, ext_energy_data
     else:
-        raise NotImplementedError()
+        logger.error(f'{rin.calc_code}: not implemented yet')
+        raise SystemExit(1)
 
     # ---------- return
     return opt_struc, energy, magmom, check_opt
 
 
 def next_struc(structure, current_id, work_path, *args):
     # args[0] <-- kpt_data
@@ -112,15 +126,16 @@
     elif rin.calc_code == 'soiap':
         ctrl_job_soiap.next_struc_soiap(structure, current_id, work_path)
     elif rin.calc_code == 'LAMMPS':
         ctrl_job_lammps.next_struc_lammps(structure, current_id, work_path)
     elif rin.calc_code == 'ASE':
         ctrl_job_ase.next_struc_ase(structure, current_id, work_path)
     else:
-        raise NotImplementedError()
+        logger.error(f'{rin.calc_code}: not implemented yet')
+        raise SystemExit(1)
 
 
 def get_energy_step(energy_step_data, current_id, work_path):
     if rin.calc_code == 'VASP':
         energy_step_data = collect_vasp.get_energy_step_vasp(
             energy_step_data, current_id, work_path)
         return energy_step_data
@@ -129,15 +144,16 @@
                                                          current_id, work_path)
         return energy_step_data
     elif rin.calc_code == 'soiap':
         energy_step_data = collect_soiap.get_energy_step_soiap(
             energy_step_data, current_id, work_path)
         return energy_step_data
     else:
-        raise NotImplementedError()
+        logger.error(f'{rin.calc_code}: not implemented yet')
+        raise SystemExit(1)
 
 
 def get_struc_step(struc_step_data, current_id, work_path):
     if rin.calc_code == 'VASP':
         struc_step_data = collect_vasp.get_struc_step_vasp(
             struc_step_data, current_id, work_path)
         return struc_step_data
@@ -146,15 +162,16 @@
             struc_step_data, current_id, work_path)
         return struc_step_data
     elif rin.calc_code == 'soiap':
         struc_step_data = collect_soiap.get_struc_step_soiap(
             struc_step_data, current_id, work_path)
         return struc_step_data
     else:
-        raise NotImplementedError()
+        logger.error(f'{rin.calc_code}: not implemented yet')
+        raise SystemExit(1)
 
 
 def get_force_step(force_step_data, current_id, work_path):
     if rin.calc_code == 'VASP':
         force_step_data = collect_vasp.get_force_step_vasp(
             force_step_data, current_id, work_path)
         return force_step_data
@@ -163,15 +180,16 @@
             force_step_data, current_id, work_path)
         return force_step_data
     elif rin.calc_code == 'soiap':
         force_step_data = collect_soiap.get_force_step_soiap(
             force_step_data, current_id, work_path)
         return force_step_data
     else:
-        raise NotImplementedError()
+        logger.error(f'{rin.calc_code}: not implemented yet')
+        raise SystemExit(1)
 
 
 def get_stress_step(stress_step_data, current_id, work_path):
     if rin.calc_code == 'VASP':
         stress_step_data = collect_vasp.get_stress_step_vasp(
             stress_step_data, current_id, work_path)
         return stress_step_data
@@ -180,8 +198,9 @@
             stress_step_data, current_id, work_path)
         return stress_step_data
     elif rin.calc_code == 'soiap':
         stress_step_data = collect_soiap.get_stress_step_soiap(
             stress_step_data, current_id, work_path)
         return stress_step_data
     else:
-        raise NotImplementedError()
+        logger.error(f'{rin.calc_code}: not implemented yet')
+        raise SystemExit(1)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/soiap/collect_soiap.py` & `csp-cryspy-1.2.0/src/cryspy/interface/soiap/collect_soiap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 '''
 Collect results in soiap
 '''
 
+from logging import getLogger
 import sys
 
 import numpy as np
 
 from . import structure as soiap_structure
 from ...util import constants
 from ...IO import pkl_data
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def collect_soiap(current_id, work_path):
     # ---------- check optimization in current stage
     try:
         with open(work_path+rin.soiap_outfile, 'r') as fout:
             lines = fout.readlines()
         check_opt = 'not_yet'
         for i, line in enumerate(lines):
@@ -32,16 +35,16 @@
     try:
         with open(work_path+'log.tote') as f:
             lines = f.readlines()
         energy = float(lines[-1].split()[4])    # in Hartree/atom
         energy = energy * constants.HRT2EV        # Hartree/atom to eV/atom
     except Exception as e:
         energy = np.nan    # error
-        print(e, '    Structure ID {0}, could not obtain energy from {1}'.format(
-            current_id, rin.soiap_outfile))
+        logger.warning(e.args[0] + f'    Structure ID {current_id},'
+                    f' could not obtain energy from {rin.soiap_outfile}')
 
     # ---------- collect the last structure
     try:
         with open(work_path+'log.struc', 'r') as f:
             lines = f.readlines()
             lines = lines[-(rin.natot+5):]
         opt_struc = soiap_structure.from_file(lines)
@@ -78,16 +81,15 @@
             lines = f.readlines()
         for line in lines:
             if line.split()[1] == '1':
                 energy_step.append(line.split()[4])    # collumn 4: Hartree/atom
         energy_step = np.array(energy_step, dtype='float') * constants.HRT2EV
     except Exception as e:
         energy_step = None
-        print(e, '#### ID: {0}: failed to parse log.tote\n'.format(
-            current_id), file=sys.stderr)
+        logger.warning(e.args[0] + f'#### ID: {current_id}: failed to parse log.tote')
 
     # ---------- append energy_step
     if energy_step_data.get(current_id) is None:
         energy_step_data[current_id] = []    # initialize
     energy_step_data[current_id].append(energy_step)
 
     # ---------- save energy_step_data
@@ -121,16 +123,15 @@
             tmp_lines.append(line)
             if len(tmp_lines) == rin.natot + 5:
                 struc = soiap_structure.from_file(tmp_lines)
                 struc_step.append(struc)
                 tmp_lines = []    # clear
     except Exception as e:
         struc_step = None
-        print(e, '#### ID: {0}: failed to parse log.struc\n'.format(
-            current_id), file=sys.stderr)
+        logger.warning(e.args[0], f'#### ID: {current_id}: failed to parse log.struc')
 
     # ---------- append struc_step
     if struc_step_data.get(current_id) is None:
         struc_step_data[current_id] = []    # initialize
     struc_step_data[current_id].append(struc_step)
 
     # ---------- save struc_step_data
@@ -167,16 +168,15 @@
                     tmp_lines = np.array(tmp_lines)
                     # Hartree/Bohr --> eV/ang
                     tmp_lines = tmp_lines * constants.HRT2EV / constants.BOHR2ANG
                     force_step.append(tmp_lines)
                     tmp_lines = []    # clear
     except Exception as e:
         force_step = None
-        print(e, '#### ID: {0}: failed to parse log.frc\n'.format(
-            current_id), file=sys.stderr)
+        logger.warning(e.args[0] + f'#### ID: {current_id}: failed to parse log.frc')
 
     # ---------- append force_step
     if force_step_data.get(current_id) is None:
         force_step_data[current_id] = []    # initialize
     force_step_data[current_id].append(force_step)
 
     # ---------- save force_step_data
@@ -213,16 +213,15 @@
                     tmp_lines = np.array(tmp_lines)
                     # Hartree/Bohr**3 --> eV/ang**3
                     tmp_lines = tmp_lines * constants.HRT2EV / constants.BOHR2ANG**3
                     stress_step.append(tmp_lines)
                     tmp_lines = []    # clear
     except Exception as e:
         stress_step = None
-        print(e, '#### ID: {0}: failed to parse log.strs\n'.format(
-            current_id), file=sys.stderr)
+        logger.warning(e.args[0], f'#### ID: {current_id}: failed to parse log.strs')
 
     # ---------- append stress_step
     if stress_step_data.get(current_id) is None:
         stress_step_data[current_id] = []    # initialize
     stress_step_data[current_id].append(stress_step)
 
     # ---------- save stress_step_data
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/soiap/ctrl_job_soiap.py` & `csp-cryspy-1.2.0/src/cryspy/interface/soiap/ctrl_job_soiap.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 '''
 Control jobs in soiap
 '''
 
+from logging import getLogger
 import os
 import shutil
 
 from . import structure as soiap_structure
 from ...IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def next_stage_soiap(stage, work_path):
     # ---------- skip_flag
     skip_flag = False
 
     # ---------- rename soiap files at the current stage
     soiap_files = [rin.soiap_infile, rin.soiap_outfile, rin.soiap_cif,
                    'log.struc', 'log.tote', 'log.frc', 'log.strs']
     for f in soiap_files:
         if not os.path.isfile(work_path+f):
-            raise IOError('Not found '+work_path+f)
+            logger.error('Not found '+work_path+f)
+            raise SystemExit(1)
         os.rename(work_path+f, work_path+'stage{}_'.format(stage)+f)
 
     # ---------- copy the input file from ./calc_in for the next stage
     finfile = './calc_in/'+rin.soiap_infile+'_{}'.format(stage + 1)
     shutil.copyfile(finfile, work_path+rin.soiap_infile)
 
     # ---------- generate the CIF file
     try:
         with open(work_path+'stage{}_log.struc'.format(stage), 'r') as f:
             lines = f.readlines()
             lines = lines[-(rin.natot+5):]
         structure = soiap_structure.from_file(lines)
     except ValueError:
         skip_flag = True
-        print('    error in soiap,  skip this structure')
+        logger.warning('    error in soiap,  skip this structure')
         return skip_flag
     with open(work_path+'stage{}_'.format(stage)+rin.soiap_cif, 'r') as f:
         lines = f.readlines()
     title = lines[0][5:]    # string following 'data_'
     soiap_structure.write(structure,
                           work_path+rin.soiap_cif,
                           symprec=rin.symprec,
@@ -49,15 +53,16 @@
 
 def next_struc_soiap(structure, current_id, work_path):
     # ---------- copy files
     calc_inputs = [rin.soiap_infile]
     for f in calc_inputs:
         ff = f+'_1' if f == rin.soiap_infile else f
         if not os.path.isfile('./calc_in/'+ff):
-            raise IOError('Could not find ./calc_in/'+ff)
+            logger.error('Could not find ./calc_in/'+ff)
+            raise SystemExit(1)
         shutil.copyfile('./calc_in/'+ff, work_path+f)
 
     # ---------- generate the CIF file
     soiap_structure.write(structure,
                           work_path+rin.soiap_cif,
                           symprec=rin.symprec,
                           title='ID_{0:d}'.format(current_id))
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/interface/soiap/structure.py` & `csp-cryspy-1.2.0/src/cryspy/interface/soiap/structure.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.1.1/src/cryspy/job/ctrl_ext.py` & `csp-cryspy-1.2.0/src/cryspy/job/ctrl_ext.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import shutil
 
+from logging import getLogger
 import numpy as np
 
 from ..interface import select_code
 from ..IO import read_input as rin
 from ..IO import io_stat, pkl_data
 from ..IO.out_results import out_rslt
 from ..util.struc_util import out_poscar, out_cif
@@ -12,14 +13,16 @@
 if rin.algo == 'BO':
     from ..BO.select_descriptor import select_descriptor
     from ..BO import bo_next_select
 if rin.algo == 'EA':
     from ..EA import ea_next_gen
 
 
+logger = getLogger('cryspy')
+
 class Ctrl_ext:
 
     def __init__(self, stat, init_struc_data):
         self.stat = stat
         self.init_struc_data = init_struc_data
         self.opt_struc_data = pkl_data.load_opt_struc()
         self.rslt_data = pkl_data.load_rslt()
@@ -58,31 +61,34 @@
                 self.job_stat = 'no queue'
             else:
                 self.job_stat = 'else'
         except IOError:
             self.job_stat = 'no_file'
 
     def handle_job(self):
-        print('\n# ---------- job status')
+        logger.info('# ---------- job status')
         if self.job_stat == 'submitted':
-            print('still queueing or running')
+            logger.info('still queueing or running')
         elif self.job_stat == 'done':
-            print('collect data')
+            logger.info('collect data')
             self.ctrl_done()
         elif self.job_stat == 'out':
-            print('write queueing structure data in ext/queue/')
+            logger.info('write queueing structure data in ext/queue/')
             self.out_queue()
         elif self.job_stat == 'no queue':
             pass
         elif self.job_stat == 'else':
-            raise ValueError('Wrong job_stat')
+            logger.error('Wrong job_stat')
+            raise SystemExit(1)
         elif self.job_stat == 'no_file':
-            raise ValueError('Wrong job_stat')
+            logger.error('Wrong job_stat')
+            raise SystemExit(1)
         else:
-            raise ValueError('Unexpected error')
+            logger.error('Unexpected error')
+            raise SystemExit(1)
 
     def out_queue(self):
         # ---------- out cifs
         os.makedirs('ext/queue', exist_ok=False)    # if dir exists, error --> stop
         for cid in self.id_queueing:
             self.init_struc_data[cid].to(fmt='cif', filename='ext/queue/{}.cif'.format(cid))
         # ---------- queue --> running
@@ -106,15 +112,16 @@
         if rin.algo == 'RS':
             self.ctrl_collect_rs()
         elif rin.algo == 'BO':
             self.ctrl_collect_bo()
         elif rin.algo == 'EA':
             self.ctrl_collect_ea()
         else:
-            raise ValueError('Error, algo')
+            logger.error('Error, algo')
+            raise SystemExit(1)
         # ---------- calc_data --> old_calc_data
         if os.path.isdir('ext/old_calc_data'):
             shutil.rmtree('ext/old_calc_data')
         shutil.move('ext/calc_data', 'ext/old_calc_data')
         # ---------- queue --> old_queue
         if os.path.isdir('ext/old_queue'):
             shutil.rmtree('ext/old_queue')
@@ -215,15 +222,15 @@
                     ext_spg_sym_opt[cid] = None
                 # -- out opt_struc
                 out_poscar(opt_struc, cid, './data/opt_POSCARS')
                 try:
                     out_cif(opt_struc, cid, './data/',
                             './data/opt_CIFS.cif', rin.symprec)
                 except TypeError:
-                    print('failed to write opt_CIF')
+                    logger.info('failed to write opt_CIF')
             # ------ error
             else:
                 ext_spg_num_opt[cid] = 0
                 ext_spg_sym_opt[cid] = None
         # ---------- save opt_struc_data
         self.opt_struc_data.update(ext_opt_struc_data)
         pkl_data.save_opt_struc(self.opt_struc_data)
@@ -237,49 +244,49 @@
         if rin.algo == 'BO':
             self.next_select_BO()
         if rin.algo == 'EA':
             self.next_gen_EA()
 
     def next_select_BO(self):
         # ---------- log
-        print('\nDone selection {}\n'.format(self.n_selection))
+        logger.info(f'\nDone selection {self.n_selection}')
         # ---------- done all structures
         if len(self.rslt_data) == rin.tot_struc:
-            print('Done all structures!')
+            logger.info('\nDone all structures!')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- check point 3
         if rin.stop_chkpt == 3:
-            print('Stop at check point 3: BO is ready\n')
+            logger.info('\nStop at check point 3: BO is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- max_select_bo
         if 0 < rin.max_select_bo <= self.n_selection:
-            print('Reached max_select_bo: {}\n'.format(rin.max_select_bo))
+            logger.info(f'\nReached max_select_bo: {rin.max_select_bo}')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- BO
         bo_data = (self.init_dscrpt_data, self.opt_dscrpt_data,
                    self.bo_mean, self.bo_var, self.bo_score)
         bo_id_data = (self.n_selection, self.id_queueing,
                       self.id_running, self.id_select_hist)
         bo_next_select.next_select(self.stat, self.rslt_data,
                                    bo_id_data, bo_data)
 
     def next_gen_EA(self):
         # ---------- log
-        print('\nDone generation {}\n'.format(self.gen))
+        logger.info(f'\nDone generation {self.gen}')
         # ---------- check point 3
         if rin.stop_chkpt == 3:
-            print('\nStop at check point 3: EA is ready\n')
+            logger.info('\nStop at check point 3: EA is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- maxgen_ea
         if 0 < rin.maxgen_ea <= self.gen:
-            print('\nReached maxgen_ea: {}\n'.format(rin.maxgen_ea))
+            logger.info(f'\nReached maxgen_ea: {rin.maxgen_ea}')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- EA
         ea_id_data = (self.gen, self.id_queueing, self.id_running)
         ea_next_gen.next_gen(self.stat, self.init_struc_data,
                              self.opt_struc_data, self.rslt_data, ea_id_data)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/job/ctrl_job.py` & `csp-cryspy-1.2.0/src/cryspy/job/ctrl_job.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 '''
 Control jobs
 '''
 
 import itertools
+from logging import getLogger
 import os
 import shutil
 import subprocess
 
 import numpy as np
 
 from ..interface import select_code
@@ -24,14 +25,16 @@
 if rin.algo == 'LAQA':
     from ..LAQA.calc_score import calc_laqa_bias
     from ..LAQA import laqa_next_selection
     from ..IO.out_results import out_laqa_status, out_laqa_step, out_laqa_score
     from ..IO.out_results import out_laqa_energy, out_laqa_bias
 
 
+logger = getLogger('cryspy')
+
 class Ctrl_job:
 
     def __init__(self, stat, init_struc_data):
         self.stat = stat
         self.init_struc_data = init_struc_data
         self.opt_struc_data = pkl_data.load_opt_struc()
         self.rslt_data = pkl_data.load_rslt()
@@ -89,26 +92,27 @@
                 self.tmp_running.append(self.tmp_queueing.pop(0))
         # ---------- initialize
         self.stage_stat = {}    # key: Structure ID
         self.job_stat = {}
         # ---------- check job status
         for cid in self.tmp_running:
             # ------ mkdir
-            if not os.path.isdir('work/{:06}'.format(cid)):
-                os.mkdir('work/{:06}'.format(cid))
+            if not os.path.isdir(f'work/{cid:06}'):
+                os.mkdir(f'work/{cid:06}')
             # ------ check stat_job file
-            stat_path = 'work/{:06}'.format(cid) + '/stat_job'
+            stat_path = f'work/{cid:06}' + '/stat_job'
             try:
                 with open(stat_path, 'r') as fstat:
                     istat = fstat.readline()    # id
                     sstat = fstat.readline()    # stage
                     jstat = fstat.readline()    # submitted or done or ...
                 self.stage_stat[cid] = int(sstat.split()[0])
                 if not cid == int(istat.split()[0]):
-                    raise SystemExit('ID is wrong in work/{:06}'.format(cid))
+                    logger.error(f'ID is wrong in work/{cid:06}')
+                    raise SystemExit(1)
                 self.stage_stat[cid] = int(sstat.split()[0])
                 if jstat[0:3] == 'sub':
                     self.job_stat[cid] = 'submitted'
                 elif jstat[0:4] == 'done':
                     self.job_stat[cid] = 'done'
                 elif jstat[0:4] == 'skip':
                     self.job_stat[cid] = 'skip'
@@ -118,68 +122,66 @@
                 self.stage_stat[cid] = 'no_file'
                 self.job_stat[cid] = 'no_file'
 
     def set_recalc(self):
         # ---------- check id
         for tid in rin.recalc:
             if tid not in self.opt_struc_data:
-                raise ValueError('ID {} has not yet been calculated'.format(
-                    tid))
+                logger.error(f'ID {tid} has not yet been calculated')
+                raise SystemExit(1)
         # ---------- append IDs to the head of id_queueing
         self.id_queueing = rin.recalc + self.id_queueing
         io_stat.set_id(self.stat, 'id_queueing', self.id_queueing)
         self.save_id_data()
         # ---------- log and out
-        print('# -- Recalc')
-        print('Append {} to the head of id_queueing'.format(rin.recalc))
+        logger.info('# -- Recalc')
+        logger.info(f'Append {rin.recalc} to the head of id_queueing')
         # ---------- clear recalc
         rin.recalc = []
         config = change_input.config_read()
         change_input.change_option(config, 'recalc', '')    # clear
         change_input.write_config(config)
-        print('Clear recalc in cryspy.in')
+        logger.info('Clear recalc in cryspy.in')
         io_stat.set_input_common(self.stat, 'option', 'recalc', '')
         io_stat.write_stat(self.stat)
 
     def handle_job(self):
-        print('\n# ---------- job status')
+        logger.info('# ---------- job status')
         for cid in self.tmp_running:
             # ---------- set work_path and current_id
-            self.work_path = './work/{:06}/'.format(cid)
+            self.work_path = f'./work/{cid:06}/'
             self.current_id = cid
             # ---------- handle job
             if self.job_stat[cid] == 'submitted':
-                print('ID {:>6}: still queueing or running'.format(cid))
+                logger.info(f'ID {cid:>6}: still queueing or running')
             elif self.job_stat[cid] == 'done':
                 self.ctrl_done()
             elif self.job_stat[cid] == 'skip':
                 self.ctrl_skip()
             elif self.job_stat[cid] == 'else':
-                raise ValueError('Wrong job_stat in {}. '.format(
-                    self.work_path))
+                logger.error(f'Wrong job_stat in {self.work_path}. ')
             elif self.job_stat[cid] == 'no_file':
                 self.ctrl_next_struc()
             else:
-                raise ValueError('Unexpected error in {}stat_job'.format(
-                    self.work_path))
+                logger.error(f'Unexpected error in {self.work_path}stat_job')
 
     def ctrl_done(self):
         self.current_stage = self.stage_stat[self.current_id]
         # ---------- log
-        print('ID {0:>6}: Stage {1} Done!'.format(
-            self.current_id, self.current_stage))
+        logger.info(f'ID {self.current_id:>6}: Stage {self.current_stage} Done!')
         # ---------- next stage
         if self.current_stage < rin.nstage:
             self.ctrl_next_stage()
         # ---------- collect result
         elif self.current_stage == rin.nstage:
             self.ctrl_collect()
         # ---------- error
         else:
-            raise ValueError('Wrong stage in '+self.work_path+'stat_job')
+            logger.error('Wrong stage in '+self.work_path+'stat_job')
+            raise SystemExit(1)
 
     def ctrl_next_stage(self):
         # ---------- energy step
         if rin.energy_step_flag:
             self.energy_step_data = select_code.get_energy_step(
                 self.energy_step_data, self.current_id, self.work_path)
         # ---------- struc step
@@ -211,27 +213,26 @@
         # ---------- submit
         self.submit_next_stage()
 
     def submit_next_stage(self):
         # ---------- submit job
         os.chdir(self.work_path)    # cd work_path
         with open('stat_job', 'w') as fwstat:
-            fwstat.write('{:<6}    # Structure ID\n'.format(self.current_id))
-            fwstat.write('{:<6}    # Stage\n'.format(self.current_stage + 1))
+            fwstat.write(f'{self.current_id:<6}    # Structure ID\n')
+            fwstat.write(f'{self.current_stage + 1:<6}    # Stage\n')
             fwstat.write('submitted\n')
         with open('sublog', 'w') as logf:
             subprocess.Popen([rin.jobcmd, rin.jobfile],
                              stdout=logf, stderr=logf)
         os.chdir('../../')    # go back to ..
         # ---------- save status
         io_stat.set_stage(self.stat, self.current_id, self.current_stage + 1)
         io_stat.write_stat(self.stat)
         # ---------- log
-        print('    submitted job, ID {0:>6} Stage {1}'.format(
-            self.current_id, self.current_stage + 1))
+        logger.info(f'    submitted job, ID {self.current_id:>6} Stage {self.current_stage + 1}')
 
     def ctrl_collect(self):
         # ---------- energy step
         if rin.energy_step_flag:
             self.energy_step_data = select_code.get_energy_step(
                 self.energy_step_data, self.current_id, self.work_path)
         # ---------- struc step
@@ -252,15 +253,16 @@
         elif rin.algo == 'BO':
             self.ctrl_collect_bo()
         elif rin.algo == 'LAQA':
             self.ctrl_collect_laqa()
         elif rin.algo == 'EA':
             self.ctrl_collect_ea()
         else:
-            raise ValueError('Error, algo')
+            logger.error('Error, algo')
+            raise SystemExit(1)
         # ---------- move to fin
         if rin.algo == 'LAQA':
             if self.fin_laqa:
                 self.mv_fin()
             else:
                 os.rename(self.work_path+'stat_job',
                           self.work_path+'prev_stat_job')
@@ -271,29 +273,29 @@
         # ---------- recheck
         self.recheck = True
 
     def ctrl_collect_rs(self):
         # ---------- get opt data
         opt_struc, energy, magmom, check_opt = \
             select_code.collect(self.current_id, self.work_path)
-        print('    collect results: E = {0} eV/atom'.format(energy))
+        logger.info(f'    collect results: E = {energy} eV/atom')
         # ---------- register opt_struc
         spg_sym, spg_num, spg_sym_opt, spg_num_opt = self.regist_opt(opt_struc)
         # ---------- save rslt
         self.rslt_data.loc[self.current_id] = [spg_num, spg_sym,
                                                spg_num_opt, spg_sym_opt,
                                                energy, magmom, check_opt]
         pkl_data.save_rslt(self.rslt_data)
         out_rslt(self.rslt_data)
 
     def ctrl_collect_bo(self):
         # ---------- get opt data
         opt_struc, energy, magmom, check_opt = \
             select_code.collect(self.current_id, self.work_path)
-        print('    collect results: E = {0} eV/atom'.format(energy))
+        logger.info(f'    collect results: E = {energy} eV/atom')
         # ---------- register opt_struc
         spg_sym, spg_num, spg_sym_opt, spg_num_opt = self.regist_opt(opt_struc)
         # ---------- save rslt
         self.rslt_data.loc[self.current_id] = [self.n_selection,
                                                spg_num, spg_sym,
                                                spg_num_opt, spg_sym_opt,
                                                energy, magmom, check_opt]
@@ -354,30 +356,30 @@
         out_laqa_step(self.laqa_step)
         out_laqa_score(self.laqa_score)
         out_laqa_energy(self.laqa_energy)
         out_laqa_bias(self.laqa_bias)
         # ---------- case of 'done' or error
         if check_opt == 'done' or np.isnan(energy) or np.isnan(tmp_laqa_bias):
             self.fin_laqa = True
-            print('    collect results: E = {0} eV/atom'.format(energy))
+            logger.info(f'    collect results: E = {energy} eV/atom')
             # ------ register opt_struc
             (spg_sym, spg_num,
              spg_sym_opt, spg_num_opt) = self.regist_opt(opt_struc)
             # ------ save rslt
             self.rslt_data.loc[self.current_id] = [spg_num, spg_sym,
                                                    spg_num_opt, spg_sym_opt,
                                                    energy, magmom, check_opt]
             pkl_data.save_rslt(self.rslt_data)
             out_rslt(self.rslt_data)
 
     def ctrl_collect_ea(self):
         # ---------- get opt data
         opt_struc, energy, magmom, check_opt = \
             select_code.collect(self.current_id, self.work_path)
-        print('    collect results: E = {0} eV/atom'.format(energy))
+        logger.info(f'    collect results: E = {energy} eV/atom')
         # ---------- register opt_struc
         spg_sym, spg_num, spg_sym_opt, spg_num_opt = self.regist_opt(opt_struc)
         # ---------- save rslt
         self.rslt_data.loc[self.current_id] = [self.gen,
                                                spg_num, spg_sym,
                                                spg_num_opt, spg_sym_opt,
                                                energy, magmom, check_opt]
@@ -409,15 +411,15 @@
                 spg_sym_opt = None
             # ------ out opt_struc
             out_poscar(opt_struc, self.current_id, './data/opt_POSCARS')
             try:
                 out_cif(opt_struc, self.current_id, self.work_path,
                         './data/opt_CIFS.cif', rin.symprec)
             except TypeError:
-                print('failed to write opt_CIF')
+                logger.warning('failed to write opt_CIF')
         # ---------- error
         else:
             spg_num_opt = 0
             spg_sym_opt = None
         # ---------- register opt_struc
         self.opt_struc_data[self.current_id] = opt_struc
         pkl_data.save_opt_struc(self.opt_struc_data)
@@ -438,20 +440,20 @@
             else:
                 next_struc_data = self.init_struc_data[self.current_id]
         # ---------- EA
         elif rin.algo == 'EA':
             next_struc_data = self.init_struc_data[self.current_id]
         # ---------- algo is wrong
         else:
-            raise ValueError('Error, algo')
+            logger.error('Error, algo in ctrl_next_struc')
+            raise SystemExit(1)
         # ---------- common part
         # ------ in case there is no initial strucure data
         if next_struc_data is None:
-            print('ID {:>6}: initial structure is None'.format(
-                self.current_id))
+            logger.info(f'ID {self.current_id:>6}: initial structure is None')
             self.ctrl_skip()
         # ------ normal initial structure data
         else:
             # -- prepare input files for structure optimization
             if rin.kpt_flag:
                 self.kpt_data = select_code.next_struc(next_struc_data,
                                                        self.current_id,
@@ -460,33 +462,33 @@
             else:
                 select_code.next_struc(next_struc_data, self.current_id,
                                        self.work_path)
             # -- prepare jobfile
             self.prepare_jobfile()
             # -- submit
             self.submit_next_struc()
-            print('ID {:>6}: submit job, Stage 1'.format(self.current_id))
+            logger.info(f'ID {self.current_id:>6}: submit job, Stage 1')
             # -- update status
             self.update_status(operation='submit')
 
     def submit_next_struc(self):
         # ---------- submit job
         os.chdir(self.work_path)    # cd work_path
         with open('stat_job', 'w') as fwstat:
-            fwstat.write('{:<6}    # Structure ID\n'.format(self.current_id))
-            fwstat.write('{:<6}    # Stage\n'.format(1))
+            fwstat.write(f'{self.current_id:<6}    # Structure ID\n')
+            fwstat.write(f'{1:<6}    # Stage\n')
             fwstat.write('submitted\n')
         with open('sublog', 'w') as logf:
             subprocess.Popen([rin.jobcmd, rin.jobfile],
                              stdout=logf, stderr=logf)
         os.chdir('../../')    # go back to csp root dir
 
     def ctrl_skip(self):
         # ---------- log
-        print('ID {:>6}: Skip'.format(self.current_id))
+        logger.info(f'ID {self.current_id:>6}: Skip')
         # ---------- get initial spg info
         if self.init_struc_data[self.current_id] is None:
             spg_sym = None
             spg_num = 0
         else:
             try:
                 spg_sym, spg_num = self.init_struc_data[
@@ -571,121 +573,121 @@
         elif operation == 'fin':
             if self.current_id in self.id_queueing:
                 self.id_queueing.remove(self.current_id)
             if self.current_id in self.id_running:
                 self.id_running.remove(self.current_id)
             io_stat.clean_id(self.stat, self.current_id)
         else:
-            raise ValueError('operation is wrong')
+            logger.error('operation is wrong')
+            raise SystemExit(1)
         io_stat.set_id(self.stat, 'id_queueing', self.id_queueing)
         io_stat.write_stat(self.stat)
         # ---------- save id_data
         self.save_id_data()
 
     def prepare_jobfile(self):
         if not os.path.isfile('./calc_in/' + rin.jobfile):
-            raise IOError('Could not find ./calc_in' + rin.jobfile)
+            logger.error('Could not find ./calc_in' + rin.jobfile)
+            raise SystemExit(1)
         with open('./calc_in/' + rin.jobfile, 'r') as f:
             lines = f.readlines()
         lines2 = []
         for line in lines:
             lines2.append(line.replace('CrySPY_ID', str(self.current_id)))
         with open(self.work_path + rin.jobfile, 'w') as f:
             f.writelines(lines2)
 
     def mv_fin(self):
-        if not os.path.isdir('work/fin/{0:06}'.format(self.current_id)):
-            shutil.move('work/{:06}'.format(self.current_id), 'work/fin/')
+        if not os.path.isdir(f'work/fin/{self.current_id:06}'):
+            shutil.move(f'work/{self.current_id:06}', 'work/fin/')
         else:    # rename for recalc
             for i in itertools.count(1):
-                if not os.path.isdir('work/fin/{0:06}_{1}'.format(
-                        self.current_id, i)):
-                    shutil.move('work/{:06}'.format(self.current_id),
-                                'work/fin/{0:06}_{1}'.format(
-                                    self.current_id, i))
+                if not os.path.isdir(f'work/fin/{self.current_id:06}_{i}'):
+                    shutil.move(f'work/{self.current_id:06}',
+                                f'work/fin/{self.current_id:06}_{i}')
                     break
 
-    def next_sg(self):
+    def next_sg(self, noprint=False):
         '''
         next selection or generation
         '''
         if rin.algo == 'BO':
-            self.next_select_BO()
+            self.next_select_BO(noprint)
         if rin.algo == 'LAQA':
             self.next_select_LAQA()
         if rin.algo == 'EA':
             self.next_gen_EA()
 
-    def next_select_BO(self):
+    def next_select_BO(self, noprint=False):
         # ---------- log
-        print('\nDone selection {}\n'.format(self.n_selection))
+        logger.info(f'\nDone selection {self.n_selection}')
         # ---------- done all structures
         if len(self.rslt_data) == rin.tot_struc:
-            print('Done all structures!')
+            logger.info('\nDone all structures!')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- flag for next selection or generation
         if not self.go_next_sg:
-            print('\nBO is ready')
+            logger.info('\nBO is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- check point 3
         if rin.stop_chkpt == 3:
-            print('Stop at check point 3: BO is ready')
+            logger.info('\nStop at check point 3: BO is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- max_select_bo
         if 0 < rin.max_select_bo <= self.n_selection:
-            print('Reached max_select_bo: {}'.format(rin.max_select_bo))
+            logger.info(f'\nReached max_select_bo: {rin.max_select_bo}')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- BO
         backup_cryspy()
         bo_data = (self.init_dscrpt_data, self.opt_dscrpt_data,
                    self.bo_mean, self.bo_var, self.bo_score)
         bo_id_data = (self.n_selection, self.id_queueing,
                       self.id_running, self.id_select_hist)
         bo_next_select.next_select(self.stat, self.rslt_data,
-                                   bo_id_data, bo_data)
+                                   bo_id_data, bo_data, noprint)
 
     def next_select_LAQA(self):
         # ---------- flag for next selection or generation
         if not self.go_next_sg:
-            print('\nLAQA is ready')
+            logger.info('\nLAQA is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- check point 3
         if rin.stop_chkpt == 3:
-            print('\nStop at check point 3: LAQA is ready')
+            logger.info('\nStop at check point 3: LAQA is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- selection of LAQA
         backup_cryspy()
         laqa_id_data = (self.id_queueing, self.id_running,
                         self.id_select_hist)
         laqa_data = (self.tot_step_select, self.laqa_step, self.laqa_struc,
                      self.laqa_energy, self.laqa_bias, self.laqa_score)
         laqa_next_selection.next_selection(self.stat, laqa_id_data, laqa_data)
 
     def next_gen_EA(self):
         # ---------- log
-        print('\nDone generation {}\n'.format(self.gen))
+        logger.info(f'\nDone generation {self.gen}')
         # ---------- flag for next selection or generation
         if not self.go_next_sg:
-            print('\nEA is ready')
+            logger.info('\nEA is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- check point 3
         if rin.stop_chkpt == 3:
-            print('\nStop at check point 3: EA is ready')
+            logger.info('\nStop at check point 3: EA is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- maxgen_ea
         if 0 < rin.maxgen_ea <= self.gen:
-            print('\nReached maxgen_ea: {}\n'.format(rin.maxgen_ea))
+            logger.info(f'\nReached maxgen_ea: {rin.maxgen_ea}')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- EA
         backup_cryspy()
         ea_id_data = (self.gen, self.id_queueing, self.id_running)
         if rin.struc_mode not in ['mol', 'mol_bs']:
             ea_next_gen.next_gen(self.stat, self.init_struc_data, None,
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/scripts/cryspy.py` & `csp-cryspy-1.2.0/src/cryspy/scripts/cryspy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python3
 '''
 Main script
 '''
 
 import argparse
+from logging import getLogger
 import os
-import sys
 
-from cryspy.interface import select_code
 from cryspy.IO import read_input as rin
 from cryspy.start import cryspy_init, cryspy_restart
-from cryspy.util.utility import backup_cryspy, clean_cryspy
+from cryspy.util.utility import set_logger, backup_cryspy, clean_cryspy
 
 # ---------- import later
+# from mpi4py import MPI
 # from cryspy.job.ctrl_ext import Ctrl_ext
 # from cryspy.job.ctrl_job import Ctrl_job
-# from mpi4py import MPI
-
+# from cryspy.interface import select_code
 
 def main():
     # ########## MPI start
     # ---------- MPI
     try:
         from mpi4py import MPI
         comm = MPI.COMM_WORLD
@@ -28,42 +27,43 @@
         mpi_size = comm.Get_size()
     except Exception as e:
         # ------ if mpi4py is not installed
         comm = None
         mpi_rank = 0
         mpi_size = 1
 
-    # ---------- stdout/stderr
-    sys.stdout = open('log_cryspy', 'a')
-    sys.stderr = open('err_cryspy', 'a')
-
     # ---------- argparse
     parser = argparse.ArgumentParser()
     parser.add_argument('-b', '--backup', help='backup data', action='store_true')
     parser.add_argument('-c', '--clean', help='clean data', action='store_true')
+    parser.add_argument('-g', '--debug', help='debug', action='store_true')
+    parser.add_argument('-n', '--noprint', help='not printing to the console', action='store_true')
     args = parser.parse_args()
 
+    # ---------- logger
+    set_logger(args.noprint, args.debug)
+    logger = getLogger('cryspy')
+    logger.debug('debug hogehoge')
+
     # ---------- backup option
     if args.backup:
         if mpi_rank == 0:
             backup_cryspy()
         raise SystemExit()
 
     # ---------- clean option
     if args.clean:
         if mpi_rank == 0:
-            sys.stdout = sys.__stdout__
-            sys.stderr = sys.__stderr__
             clean_cryspy()
         raise SystemExit()
 
     # ---------- lock
     if os.path.isfile('lock_cryspy'):
         if mpi_rank == 0:
-            print('lock_cryspy file exists', file=sys.stderr)
+            logger.error('lock_cryspy file exists')
         raise SystemExit(1)
     else:
         if mpi_size > 1:
             comm.barrier()
         if mpi_rank == 0:
             with open('lock_cryspy', 'w'):
                 pass    # create vacant file
@@ -81,20 +81,21 @@
         # only stat and init_struc_data in rank0 are important
         stat, init_struc_data = cryspy_restart.restart(comm, mpi_rank, mpi_size)
     # ########## MPI end
 
     if mpi_rank == 0:
         # ---------- check point 1
         if rin.stop_chkpt == 1:
-            print('Stop at check point 1')
+            logger.info('Stop at check point 1')
             os.remove('lock_cryspy')
             raise SystemExit()
 
         if not rin.calc_code == 'ext':
             # ---------- check calc files in ./calc_in
+            from cryspy.interface import select_code
             select_code.check_calc_files()
             # ---------- mkdir work/fin
             os.makedirs('work/fin', exist_ok=True)
 
         # ---------- Perform structure optimization externally
         if rin.calc_code == 'ext':
             # ------ instantiate Ctrl_job class
@@ -115,26 +116,26 @@
         # ---------- recheck for skip and done
         if not rin.calc_code == 'ext':
             if jobs.id_queueing:
                 cnt_recheck = 0
                 while jobs.recheck:
                     cnt_recheck += 1
                     jobs.recheck = False    # True --> False
-                    print('\n\n recheck {}\n'.format(cnt_recheck))
+                    logger.info(f'\n\nrecheck {cnt_recheck}\n')
                     jobs.check_job()
                     jobs.handle_job()
 
         # ---------- next selection or generation
         if not (jobs.id_queueing or jobs.id_running):
             # ---------- next selection or generation
             if rin.algo in ['BO', 'LAQA', 'EA']:
-                jobs.next_sg()
+                jobs.next_sg(args.noprint)
             # ---------- for RS
             else:
-                print('Done all structures!')
+                logger.info('\nDone all structures!')
 
         # ---------- unlock
         os.remove('lock_cryspy')
 
 
 if __name__ == '__main__':
     # ---------- main
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/start/cryspy_init.py` & `csp-cryspy-1.2.0/src/cryspy/start/cryspy_init.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 '''
 Initialize CrySPY
 '''
 
 from datetime import datetime
+from logging import getLogger
 import os
 
 import pandas as pd
 
 from .gen_init_struc import gen_init_struc
 from ..IO import pkl_data, io_stat
 from ..IO import read_input as rin
-from ..util.utility import get_date, get_version
+from ..util.utility import get_version
 from ..util.struc_util import out_poscar
 
 # ---------- import later
 #from ..RS import rs_init
 #from ..BO import bo_init
 #from ..LAQA import laqa_init
 #from ..EA import ea_init
 #from ..RS.gen_struc_RS.gen_pyxtal import Rnd_struc_gen_pyxtal
 #from ..RS.gen_struc_RS.random_generation import Rnd_struc_gen
 
 
+logger = getLogger('cryspy')
+
 def initialize(comm, mpi_rank, mpi_size):
+    # ---------- start
     if mpi_rank == 0:
-        # ---------- start
-        print(get_date())
-        print('CrySPY ' + get_version())
-        print('Start cryspy.py', flush=True)
-        print(f'Number of MPI processes: {mpi_size}\n')
+        logger.info('\n\n\nStart CrySPY ' + get_version() + '\n\n')
 
     # ---------- read input
     if mpi_rank == 0:
-        print('Read input file, cryspy.in')
+        logger.info('# ---------- Read input file, cryspy.in')
     # ########## MPI start
     if mpi_size > 1:
         comm.barrier()
-    rin.readin()          # read input data, cryspy,in
+    try:
+        rin.readin()          # read input data, cryspy,in
+    except Exception as e:
+        if mpi_rank == 0:
+            logger.error(e.args[0])
+        raise SystemExit(1)
     # ########## MPI end
     if mpi_rank == 0:
         stat = io_stat.stat_init()    # initialize stat
         rin.save_stat(stat)   # save input variables in cryspy.stat
 
         # ---------- make data directory
         os.makedirs('data/pkl_data', exist_ok=True)
 
     # ---------- generate initial structures
     if not rin.load_struc_flag:
         if mpi_rank == 0:
-            print('\n# --------- Generate initial structures')
+            logger.info('# ---------- Initial structure generation')
+            logger.info(f'Number of MPI processes: {mpi_size}')
         if mpi_size > 1:
             comm.barrier()
         if mpi_rank == 0:
             # ------ time
             time_start = datetime.today()
         # ########## MPI start
         # ------ from scratch
@@ -72,26 +78,26 @@
             # ------ save
             pkl_data.save_init_struc(init_struc_data)
             if rin.algo == 'EA' and rin.struc_mode in ['mol', 'mol_bs']:
                 pkl_data.save_struc_mol_id(struc_mol_id)
             # ------ time
             time_end = datetime.today()
             etime = time_end - time_start
-            print(f'\nElapsed time for structure generation: {etime}\n')
+            logger.info(f'Elapsed time for structure generation: {etime}')
     else:
         # ------ load initial structure
         if mpi_rank == 0:
-            print('\n# --------- Load initial structure data')
-            print('Load ./data/pkl_data/init_struc_data.pkl\n')
+            logger.info('# --------- Load initial structure data')
+            logger.info('Load ./data/pkl_data/init_struc_data.pkl')
             init_struc_data = pkl_data.load_init_struc()
             # -- check
             if not rin.tot_struc == len(init_struc_data):
-                raise ValueError('rin.tot_struc = {0},'
-                                ' len(init_struc_data) = {1}'.format(
-                                    rin.tot_struc, len(init_struc_data)))
+                logger.error(f'rin.tot_struc = {rin.tot_struc},'
+                                f' len(init_struc_data) = {len(init_struc_data)}')
+                raise SystemExit(1)
             # -- init_POSCARS
             for cid, struc in init_struc_data.items():
                 out_poscar(struc, cid, './data/init_POSCARS')
 
     if mpi_rank == 0:
         # ---------- initialize opt_struc_data
         opt_struc_data = {}
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/start/cryspy_restart.py` & `csp-cryspy-1.2.0/src/cryspy/start/cryspy_restart.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 '''
 Restart CrySPY
 '''
 
 from datetime import datetime
+from logging import getLogger
 import os
 import sys
 
 from .gen_init_struc import gen_init_struc
 from ..IO import io_stat, pkl_data
 from ..IO import read_input as rin
-from ..util.utility import get_date, get_version, backup_cryspy
+from ..util.utility import get_version, backup_cryspy
 
 # ---------- import later
 #from ..RS import rs_restart
 #from ..BO import bo_restart
 #from ..LAQA import laqa_restart
 #from ..EA import ea_append
 #from ..RS.gen_struc_RS.gen_pyxtal import Rnd_struc_gen_pyxtal
 #from ..RS.gen_struc_RS.random_generation import Rnd_struc_gen
 
 
+logger = getLogger('cryspy')
+
 def restart(comm, mpi_rank, mpi_size):
     if mpi_rank == 0:
-        print('\n\n')
-        print(get_date())
-        print('CrySPY ' + get_version())
-        print('Restart cryspy.py')
-        print(f'Number of MPI processes: {mpi_size}\n\n')
-
+        logger.info('\n\n\nRestart CrySPY ' + get_version() + '\n\n')
         # ---------- read stat
         stat = io_stat.stat_read()
     else:
         stat = None
 
     # ########## MPI start
     if mpi_size > 1:
         comm.barrier()
     # ---------- read input and check the change
-    rin.readin()
+    try:
+        rin.readin()
+    except Exception as e:
+        if mpi_rank == 0:
+            logger.error(e.args[0])
+        raise SystemExit(1)
     if mpi_rank == 0:
         try:
             rin.diffinstat(stat)
         except Exception as e:
             if mpi_size > 1:
-                print(e, file=sys.stderr, flush=True)
                 comm.Abort(1)
-            raise SystemExit(e)
+            logger.error(e.args[0])
+            raise SystemExit(1)
 
     # ------ load init_struc_data for appending structures
     # In EA, one can not change tot_struc, so struc_mol_id need not be considered here
     init_struc_data = pkl_data.load_init_struc()
 
     # ---------- append structures
     if len(init_struc_data) < rin.tot_struc:
@@ -76,15 +79,16 @@
             # -- LAQA
             if rin.algo == 'LAQA':
                 from ..LAQA import laqa_restart
                 laqa_restart.restart(stat, prev_nstruc)
             os.remove('lock_cryspy')
         raise SystemExit()
     elif rin.tot_struc < len(init_struc_data):
-        raise ValueError('tot_struc < len(init_struc_data)')
+        logger.error('tot_struc < len(init_struc_data)')
+        raise SystemExit(1)
 
     # ---------- append structures by EA (option)
     # not support MPI
     if rin.append_struc_ea:
         if mpi_rank == 0:
             # ------ backup
             backup_cryspy()
@@ -114,15 +118,15 @@
     # ---------- return
     return stat, init_struc_data
 
 
 def _append_struc(init_struc_data, comm, mpi_rank, mpi_size):
     # ---------- append initial structures
     if mpi_rank == 0:
-        print('\n# ---------- Append structures')
+        logger.info('# ---------- Append structures')
     if mpi_size > 1:
         comm.barrier()
     # ------ time
     if mpi_rank == 0:
         time_start = datetime.today()
 
     # ---------- gen_init_struc()
@@ -132,12 +136,12 @@
 
     if mpi_rank == 0:
         # ---------- save
         pkl_data.save_init_struc(init_struc_data)
         # ---------- time
         time_end = datetime.today()
         etime = time_end - time_start
-        print(f'\nElapsed time for structure generation: {etime}\n')
+        logger.info(f'Elapsed time for structure generation: {etime}')
 
     # ---------- return
     # only init_struc_data in rank0 is important
     return init_struc_data
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/start/gen_init_struc.py` & `csp-cryspy-1.2.0/src/cryspy/start/gen_init_struc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,48 @@
+from logging import getLogger
 import os
 import sys
 
 from ..IO import read_input as rin
 from ..util.utility import check_fwpath
 from ..util.struc_util import set_mindist, out_poscar
 
 
+logger = getLogger('cryspy')
+
 def gen_init_struc(init_struc_data, struc_mol_id, comm, mpi_rank, mpi_size):
     # ---------- mindist
     if mpi_rank == 0:
-        print('# ------ mindist', flush=True)
+        logger.info('# ------ mindist')
     if mpi_size > 1:
         comm.barrier()
     mindist = set_mindist(rin.mindist, rin.mindist_factor, False, mpi_rank)
 
     # ---------- nstruc, offset for MPI
     nstruc_list, offset_list = _divide_task(rin.tot_struc, mpi_size, len(init_struc_data))
 
+    # ---------- log
+    if mpi_rank == 0:
+        logger.info('# ------ generate structures')
+
     # ---------- pyxtal
     if not (rin.spgnum == 0 or rin.use_find_wy):
         from ..RS.gen_struc_RS.gen_pyxtal import Rnd_struc_gen_pyxtal
         rsgx = Rnd_struc_gen_pyxtal(mindist=mindist)
         # ------ crystal
         if rin.struc_mode == 'crystal':
             rsgx.gen_struc(nstruc=nstruc_list[mpi_rank], id_offset=offset_list[mpi_rank])
         # ------ molecular crystal
         elif rin.struc_mode == 'mol':
             rsgx.set_mol()
             rsgx.gen_struc_mol(nstruc=nstruc_list[mpi_rank], id_offset=offset_list[mpi_rank])
         # ------ molecular crystal breaking symmetry
         elif rin.struc_mode == 'mol_bs':
             if mpi_rank == 0:
-                print('# -- mindist_mol_bs')
+                logger.info('# -- mindist_mol_bs')
             mindist_dummy = set_mindist(rin.mindist_mol_bs, rin.mindist_mol_bs_factor,
                                         dummy=True, mpi_rank=mpi_rank)
             rsgx.set_mol()
             rsgx.gen_struc_mol_break_sym(nstruc=nstruc_list[mpi_rank],
                                             mindist_dummy=mindist_dummy,
                                             id_offset=offset_list[mpi_rank])
         # ------ init_struc_data
@@ -67,25 +74,15 @@
         from ..RS.gen_struc_RS.random_generation import Rnd_struc_gen
         rsg = Rnd_struc_gen(mindist=mindist)
         if rin.spgnum == 0:
             rsg.gen_wo_spg(nstruc=nstruc_list[mpi_rank], id_offset=offset_list[mpi_rank])
         else:
             # ---- findwy
             # -- check fwpath
-            if mpi_rank == 0:
-                try:
-                    fwpath = check_fwpath(rin.fwpath)
-                except Exception as e:
-                    if mpi_size > 1:
-                        print(e, file=sys.stderr, flush=True)
-                        comm.Abort(1)
-                    raise SystemExit(e)
-            else:
-                fwpath = None
-            fwpath = comm.bcast(fwpath, root=0)
+            fwpath = check_fwpath(rin.fwpath)
             if mpi_rank == 0:
                 os.makedirs('tmp_gen_struc', exist_ok=True)
             if mpi_size > 1:
                 comm.barrier()
             rsg.gen_with_find_wy(nstruc=nstruc_list[mpi_rank],
                                     id_offset=offset_list[mpi_rank], init_pos_path=None,
                                     fwpath=fwpath, mpi_rank=mpi_rank)
```

### Comparing `csp-cryspy-1.1.1/src/cryspy/util/struc_util.py` & `csp-cryspy-1.2.0/src/cryspy/util/struc_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 '''
 Utility for structures
 '''
 
+from logging import getLogger
 import os
 
 import numpy as np
 
 from pymatgen.core import Structure
 from pymatgen.io.cif import CifWriter
 from pyxtal.tolerance import Tol_matrix
 
 from ..IO import read_input as rin
 
 
+logger = getLogger('cryspy')
+
 def set_mindist(mindist_in, factor, dummy=False, mpi_rank=0):
     # ---------- dummy atom in mol_bs
     if dummy:
         atype = get_atype_dummy()
     else:
         atype = rin.atype
 
@@ -24,48 +27,50 @@
     if mindist_in is None:
         # ------ Tol matrix
         if rin.struc_mode in ['crystal']:
             tolmat = Tol_matrix(prototype='atomic', factor=factor)
         elif rin.struc_mode in ['mol', 'mol_bs']:
             tolmat = Tol_matrix(prototype='molecular', factor=factor)
         else:
-            raise ValueError('struc_mode')
+            logger.error('struc_mode is wrong')
+            raise SystemExit(1)
         # ------ set mindist
         mindist = []
         for i, itype in enumerate(atype):
             tmp = []
             for j, jtype in enumerate(atype):
                 tmp.append(tolmat.get_tol(itype, jtype))
             mindist.append(tmp)
     else:
         tmp_array = factor * np.array(mindist_in)
         mindist = tmp_array.tolist()
 
-    # ---------- print
+    # ---------- log
     if mpi_rank == 0:
         for i, itype in enumerate(atype):
             for j, jtype in enumerate(atype):
                 if i <= j:
                     if dummy:
-                        print(rin.mol_file[i], '-', rin.mol_file[j], mindist[i][j], flush=True)
+                        logger.info(f'{rin.mol_file[i]} - {rin.mol_file[j]}: {mindist[i][j]}')
                     else:
-                        print(itype, '-', jtype, mindist[i][j], flush=True)
+                        logger.info(f'{itype} - {jtype}: {mindist[i][j]}')
         if rin.struc_mode == 'mol':
-            print('When struc_mode is mol (only random structure, not EA part),')
-            print('- tolerance between monoatomic molecules is multiplied by 0.8 inside pyxtal (not printed above)')
-            print('- H-N, H-O, or H-F tolerance is multiplied by 0.9 inside pyxtal (not printed above)',  flush=True)
+            logger.info('When struc_mode is mol (only random structure, not EA part),\n'
+            '- tolerance between monoatomic molecules is multiplied by 0.8 inside pyxtal (not printed above)\n'
+            '- H-N, H-O, or H-F tolerance is multiplied by 0.9 inside pyxtal (not printed above)')
 
     # ---------- return
     return mindist
 
 
 def get_atype_dummy():
     noble_gas = ['Rn', 'Xe', 'Kr', 'Ar', 'Ne', 'He']
     if len(rin.nmol) > len(noble_gas):
-        raise ValueError('len(nmol) > len(noble_gas)')
+        logger.error('len(nmol) > len(noble_gas)')
+        raise SystemExit(1)
     atype = noble_gas[:len(rin.nmol)]
     return atype
 
 
 def out_poscar(struc, cid, fpath):
     # ---------- poscar format
     pos = struc.to(fmt='poscar')
@@ -90,16 +95,17 @@
     #                (need to delete '_chemical_formula_sum'. i don't know why)
     with open(tmp_path+'tmp.cif', 'r') as fcif:
         ciflines = fcif.readlines()
     ciflines[1] = 'data_ID_{}\n'.format(cid)
     if ciflines[11][:21] == '_chemical_formula_sum':
         ciflines.pop(11)
     else:
-        raise ValueError('ciflines[11] is not _chemical_formula_sum,'
+        logger.error('ciflines[11] is not _chemical_formula_sum,'
                          ' have to fix bag')
+        raise SystemExit(1)
 
     # ---------- cif --> opt_cifs
     with open(fpath, 'a') as foptcif:
         for line in ciflines:
             foptcif.write(line)
 
     # ---------- clean tmp.cif
@@ -303,15 +309,16 @@
 
     # ---------- input
     angles: in radian (degree=False)
     seq:
     degree:
     '''
     if not len(seq) == len(angles):
-        raise ValueError('not len(seq) == len(angles)')
+        logger.error('not len(seq) == len(angles)')
+        raise SystemExit(1)
 
     if degree:
         angles = np.deg2rad(angles)
 
     R = np.eye(3)
     angles = angles[::-1]
     seq = seq[::-1]
```

### Comparing `csp-cryspy-1.1.1/src/csp_cryspy.egg-info/PKG-INFO` & `csp-cryspy-1.2.0/src/csp_cryspy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csp-cryspy
-Version: 1.1.1
+Version: 1.2.0
 Summary: CrySPY is a crystal structure prediction tool written in Python.
 Author-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 Maintainer-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 License: MIT License
         
         Copyright (c) 2018 CrySPY Development Team
         
@@ -42,26 +42,30 @@
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
 Document: https://tomoki-yamashita.github.io/CrySPY_doc  
 Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.1.1 (2023 June 14)
+version 1.2.0 (2023 July 10)
 
 ## News
+- [2023 July 10] CrySPY 1.2.0 released. Version information/version 1.2.0
+    + Interface for ASE
+    + Adoption of logging
+    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [CHANGELOG](./CHANGELOG.md)
 - [2023 June 14] CrySPY 1.1.1 released
     + bug fix
 - [2023 May 16] CrySPY 1.1.0 released
     + MPI parallelization (optional)
     + New score of LAQA
-    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
+    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [CHANGELOG](./CHANGELOG.md)
 - [2023 March 16] CrySPY 1.0.0 released
     + CrySPY is available in PyPI, so you can install by pip (project name is csp-cryspy).
-    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
+    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [CHANGELOG](./CHANGELOG.md)
 
 
 ## System requirements
 ### Python
 - Python >= 3.8
 - [PyXtal >= 0.5.3](https://pyxtal.readthedocs.io/en/latest "PyXtal")
```

### Comparing `csp-cryspy-1.1.1/src/csp_cryspy.egg-info/SOURCES.txt` & `csp-cryspy-1.2.0/src/csp_cryspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


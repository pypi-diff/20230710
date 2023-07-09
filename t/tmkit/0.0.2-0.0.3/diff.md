# Comparing `tmp/tmkit-0.0.2.tar.gz` & `tmp/tmkit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmkit-0.0.2.tar", last modified: Thu Jul  6 18:43:43 2023, max compression
+gzip compressed data, was "tmkit-0.0.3.tar", last modified: Sun Jul  9 23:54:42 2023, max compression
```

## Comparing `tmkit-0.0.2.tar` & `tmkit-0.0.3.tar`

### file list

```diff
@@ -1,182 +1,197 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.233837 tmkit-0.0.2/
--rw-rw-rw-   0        0        0    35823 2022-10-06 19:26:08.000000 tmkit-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      300 2023-07-06 18:43:43.230837 tmkit-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1437 2023-07-06 18:01:52.000000 tmkit-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 18:43:43.233837 tmkit-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      712 2023-07-06 18:43:38.000000 tmkit-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.859837 tmkit-0.0.2/tmkit/
--rw-rw-rw-   0        0        0      458 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/Path.py
--rw-rw-rw-   0        0        0     1169 2023-07-03 17:00:04.000000 tmkit-0.0.2/tmkit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.889838 tmkit-0.0.2/tmkit/base/
--rw-rw-rw-   0        0        0     3169 2023-07-03 17:00:04.000000 tmkit-0.0.2/tmkit/base/PDB.py
--rw-rw-rw-   0        0        0      996 2023-06-29 20:03:03.000000 tmkit-0.0.2/tmkit/base/Position.py
--rw-rw-rw-   0        0        0       76 2019-09-15 16:59:06.000000 tmkit-0.0.2/tmkit/base/__init__.py
--rw-rw-rw-   0        0        0     1541 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/cath.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.904837 tmkit-0.0.2/tmkit/chain/
--rw-rw-rw-   0        0        0     4217 2023-07-06 12:47:01.000000 tmkit-0.0.2/tmkit/chain/Collate.py
--rw-rw-rw-   0        0        0     6767 2023-07-06 12:46:03.000000 tmkit-0.0.2/tmkit/chain/CollateBatch.py
--rw-rw-rw-   0        0        0      599 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/chain/PDB.py
--rw-rw-rw-   0        0        0        0 2022-08-06 11:29:10.000000 tmkit-0.0.2/tmkit/chain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.910837 tmkit-0.0.2/tmkit/channel/
--rw-rw-rw-   0        0        0     6299 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/channel/Workbench.py
--rw-rw-rw-   0        0        0        0 2019-08-11 19:08:40.000000 tmkit-0.0.2/tmkit/channel/__init__.py
--rw-rw-rw-   0        0        0     1807 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/collate.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.919836 tmkit-0.0.2/tmkit/contact/
--rw-rw-rw-   0        0        0     7748 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/contact/Evaluator.py
--rw-rw-rw-   0        0        0    24764 2023-07-02 17:52:28.000000 tmkit-0.0.2/tmkit/contact/Reader.py
--rw-rw-rw-   0        0        0        0 2019-08-11 18:38:08.000000 tmkit-0.0.2/tmkit/contact/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.927835 tmkit-0.0.2/tmkit/db/
--rw-rw-rw-   0        0        0     6480 2023-07-04 23:50:26.000000 tmkit-0.0.2/tmkit/db/Connectivity.py
--rw-rw-rw-   0        0        0     3438 2023-06-29 21:49:55.000000 tmkit-0.0.2/tmkit/db/Reader.py
--rw-rw-rw-   0        0        0        0 2019-05-10 13:10:28.000000 tmkit-0.0.2/tmkit/db/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.933869 tmkit-0.0.2/tmkit/db/biogrid/
--rw-rw-rw-   0        0        0     1902 2023-07-02 19:30:12.000000 tmkit-0.0.2/tmkit/db/biogrid/Reader.py
--rw-rw-rw-   0        0        0        0 2020-07-08 14:38:06.000000 tmkit-0.0.2/tmkit/db/biogrid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.940836 tmkit-0.0.2/tmkit/db/cath/
--rw-rw-rw-   0        0        0     4864 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/db/cath/Reader.py
--rw-rw-rw-   0        0        0        0 2022-08-11 11:28:12.000000 tmkit-0.0.2/tmkit/db/cath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.945836 tmkit-0.0.2/tmkit/db/construct/
--rw-rw-rw-   0        0        0     3077 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/db/construct/Network.py
--rw-rw-rw-   0        0        0        0 2020-08-28 22:57:35.000000 tmkit-0.0.2/tmkit/db/construct/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.950837 tmkit-0.0.2/tmkit/db/intact/
--rw-rw-rw-   0        0        0     2497 2023-07-02 19:38:00.000000 tmkit-0.0.2/tmkit/db/intact/Reader.py
--rw-rw-rw-   0        0        0        0 2020-07-11 22:05:59.000000 tmkit-0.0.2/tmkit/db/intact/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.956836 tmkit-0.0.2/tmkit/db/muthtp/
--rw-rw-rw-   0        0        0     4168 2023-07-02 19:38:00.000000 tmkit-0.0.2/tmkit/db/muthtp/Reader.py
--rw-rw-rw-   0        0        0        0 2022-08-07 05:11:20.000000 tmkit-0.0.2/tmkit/db/muthtp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.960836 tmkit-0.0.2/tmkit/db/predmuthtp/
--rw-rw-rw-   0        0        0     2911 2023-07-02 19:59:20.000000 tmkit-0.0.2/tmkit/db/predmuthtp/Reader.py
--rw-rw-rw-   0        0        0        0 2022-08-07 05:11:42.000000 tmkit-0.0.2/tmkit/db/predmuthtp/__init__.py
--rw-rw-rw-   0        0        0      979 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/edge.py
--rw-rw-rw-   0        0        0     3053 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/feature.py
--rw-rw-rw-   0        0        0      450 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/fetch.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.972836 tmkit-0.0.2/tmkit/id/
--rw-rw-rw-   0        0        0      525 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/id/Fasta.py
--rw-rw-rw-   0        0        0     2476 2023-07-05 23:15:24.000000 tmkit-0.0.2/tmkit/id/Mapping.py
--rw-rw-rw-   0        0        0     1035 2023-06-19 10:50:52.000000 tmkit-0.0.2/tmkit/id/PDB.py
--rw-rw-rw-   0        0        0        0 2020-04-26 23:07:36.000000 tmkit-0.0.2/tmkit/id/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.984839 tmkit-0.0.2/tmkit/interface/
--rw-rw-rw-   0        0        0      387 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/interface/Tool.py
--rw-rw-rw-   0        0        0      398 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/interface/Topology.py
--rw-rw-rw-   0        0        0        0 2020-07-09 17:22:43.000000 tmkit-0.0.2/tmkit/interface/__init__.py
--rw-rw-rw-   0        0        0      511 2023-06-29 21:39:11.000000 tmkit-0.0.2/tmkit/mapping.py
--rw-rw-rw-   0        0        0     3353 2023-07-02 17:26:33.000000 tmkit-0.0.2/tmkit/msa.py
--rw-rw-rw-   0        0        0     1817 2023-07-02 19:59:20.000000 tmkit-0.0.2/tmkit/mut.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.990838 tmkit-0.0.2/tmkit/name/
--rw-rw-rw-   0        0        0     3179 2023-07-04 23:49:09.000000 tmkit-0.0.2/tmkit/name/Mapping.py
--rw-rw-rw-   0        0        0        0 2022-08-06 12:13:25.000000 tmkit-0.0.2/tmkit/name/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.992835 tmkit-0.0.2/tmkit/position/
--rw-rw-rw-   0        0        0       16 2019-09-15 17:43:20.000000 tmkit-0.0.2/tmkit/position/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.002836 tmkit-0.0.2/tmkit/position/scenario/
--rw-rw-rw-   0        0        0     1724 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/position/scenario/Segment.py
--rw-rw-rw-   0        0        0     2421 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/position/scenario/Separation.py
--rw-rw-rw-   0        0        0        0 2019-09-21 21:40:26.000000 tmkit-0.0.2/tmkit/position/scenario/__init__.py
--rw-rw-rw-   0        0        0     3245 2023-07-02 18:50:26.000000 tmkit-0.0.2/tmkit/ppi.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.008869 tmkit-0.0.2/tmkit/property/
--rw-rw-rw-   0        0        0     7715 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/property/HelixSurface.py
--rw-rw-rw-   0        0        0        0 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/property/__init__.py
--rw-rw-rw-   0        0        0     1319 2023-06-29 21:41:10.000000 tmkit-0.0.2/tmkit/qc.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.021835 tmkit-0.0.2/tmkit/retrieve/
--rw-rw-rw-   0        0        0    11431 2023-07-02 17:14:47.000000 tmkit-0.0.2/tmkit/retrieve/MSA.py
--rw-rw-rw-   0        0        0     4362 2023-07-04 11:15:51.000000 tmkit-0.0.2/tmkit/retrieve/PDB.py
--rw-rw-rw-   0        0        0     1688 2023-07-04 11:15:51.000000 tmkit-0.0.2/tmkit/retrieve/XML.py
--rw-rw-rw-   0        0        0        0 2019-05-10 15:10:49.000000 tmkit-0.0.2/tmkit/retrieve/__init__.py
--rw-rw-rw-   0        0        0     4241 2023-07-05 23:13:50.000000 tmkit-0.0.2/tmkit/rrc.py
--rw-rw-rw-   0        0        0     3626 2023-07-04 10:19:01.000000 tmkit-0.0.2/tmkit/seq.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.033840 tmkit-0.0.2/tmkit/seqnetrr/
--rw-rw-rw-   0        0        0     7758 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/seqnetrr/Compare.py
--rw-rw-rw-   0        0        0     3507 2023-07-02 16:12:58.000000 tmkit-0.0.2/tmkit/seqnetrr/ComputLib.py
--rw-rw-rw-   0        0        0    11463 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/seqnetrr/Controller.py
--rw-rw-rw-   0        0        0        0 2022-05-17 20:55:49.000000 tmkit-0.0.2/tmkit/seqnetrr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.049836 tmkit-0.0.2/tmkit/seqnetrr/combo/
--rw-rw-rw-   0        0        0     1989 2023-07-02 17:02:29.000000 tmkit-0.0.2/tmkit/seqnetrr/combo/Length.py
--rw-rw-rw-   0        0        0      461 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/seqnetrr/combo/Param.py
--rw-rw-rw-   0        0        0     1674 2023-06-29 20:10:11.000000 tmkit-0.0.2/tmkit/seqnetrr/combo/Position.py
--rw-rw-rw-   0        0        0     2494 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/seqnetrr/combo/Separation.py
--rw-rw-rw-   0        0        0        0 2019-08-11 16:35:38.000000 tmkit-0.0.2/tmkit/seqnetrr/combo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.061838 tmkit-0.0.2/tmkit/seqnetrr/graph/
--rw-rw-rw-   0        0        0    16660 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/seqnetrr/graph/Bipartite.py
--rw-rw-rw-   0        0        0     2961 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/seqnetrr/graph/Cumulative.py
--rw-rw-rw-   0        0        0    19134 2023-07-02 17:04:50.000000 tmkit-0.0.2/tmkit/seqnetrr/graph/Unipartite.py
--rw-rw-rw-   0        0        0        0 2022-05-18 21:29:35.000000 tmkit-0.0.2/tmkit/seqnetrr/graph/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.066835 tmkit-0.0.2/tmkit/seqnetrr/net/
--rw-rw-rw-   0        0        0    25230 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/seqnetrr/net/Reader.py
--rw-rw-rw-   0        0        0        0 2022-06-12 23:19:50.000000 tmkit-0.0.2/tmkit/seqnetrr/net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.074835 tmkit-0.0.2/tmkit/seqnetrr/window/
--rw-rw-rw-   0        0        0     4902 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/seqnetrr/window/Pair.py
--rw-rw-rw-   0        0        0     4471 2023-07-02 15:47:51.000000 tmkit-0.0.2/tmkit/seqnetrr/window/Single.py
--rw-rw-rw-   0        0        0        0 2019-09-18 20:19:22.000000 tmkit-0.0.2/tmkit/seqnetrr/window/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.082840 tmkit-0.0.2/tmkit/seqnetrr/window/base/
--rw-rw-rw-   0        0        0     1309 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/seqnetrr/window/base/Pair.py
--rw-rw-rw-   0        0        0     1311 2023-07-02 16:10:15.000000 tmkit-0.0.2/tmkit/seqnetrr/window/base/Single.py
--rw-rw-rw-   0        0        0        0 2019-09-19 13:22:58.000000 tmkit-0.0.2/tmkit/seqnetrr/window/base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.099867 tmkit-0.0.2/tmkit/sequence/
--rw-rw-rw-   0        0        0      535 2023-07-05 23:14:23.000000 tmkit-0.0.2/tmkit/sequence/Fasta.py
--rw-rw-rw-   0        0        0      446 2023-06-29 20:03:03.000000 tmkit-0.0.2/tmkit/sequence/Index.py
--rw-rw-rw-   0        0        0     1881 2023-07-02 13:50:17.000000 tmkit-0.0.2/tmkit/sequence/PDB.py
--rw-rw-rw-   0        0        0     1640 2023-07-02 15:53:41.000000 tmkit-0.0.2/tmkit/sequence/XML.py
--rw-rw-rw-   0        0        0        0 2019-08-02 11:12:19.000000 tmkit-0.0.2/tmkit/sequence/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.106835 tmkit-0.0.2/tmkit/structure/
--rw-rw-rw-   0        0        0     3163 2023-07-03 17:00:04.000000 tmkit-0.0.2/tmkit/structure/PDB.py
--rw-rw-rw-   0        0        0        0 2019-08-02 11:11:48.000000 tmkit-0.0.2/tmkit/structure/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.111837 tmkit-0.0.2/tmkit/structure/ppi/
--rw-rw-rw-   0        0        0     1445 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/structure/ppi/Label.py
--rw-rw-rw-   0        0        0        0 2019-09-15 17:30:37.000000 tmkit-0.0.2/tmkit/structure/ppi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.116835 tmkit-0.0.2/tmkit/structure/rrc/
--rw-rw-rw-   0        0        0     1803 2023-06-29 20:03:03.000000 tmkit-0.0.2/tmkit/structure/rrc/Label.py
--rw-rw-rw-   0        0        0        0 2019-09-15 17:30:31.000000 tmkit-0.0.2/tmkit/structure/rrc/__init__.py
--rw-rw-rw-   0        0        0     4335 2023-07-04 17:11:34.000000 tmkit-0.0.2/tmkit/topo.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.124835 tmkit-0.0.2/tmkit/topology/
--rw-rw-rw-   0        0        0     4174 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/topology/Phobius.py
--rw-rw-rw-   0        0        0     7643 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/topology/TMHMM.py
--rw-rw-rw-   0        0        0        0 2019-05-10 13:11:26.000000 tmkit-0.0.2/tmkit/topology/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.129835 tmkit-0.0.2/tmkit/topology/lib/
--rw-rw-rw-   0        0        0    25043 2022-07-15 23:01:47.000000 tmkit-0.0.2/tmkit/topology/lib/Phobius.py
--rw-rw-rw-   0        0        0        0 2022-07-16 23:17:45.000000 tmkit-0.0.2/tmkit/topology/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.147835 tmkit-0.0.2/tmkit/topology/pdbtm/
--rw-rw-rw-   0        0        0     4882 2023-07-04 14:03:11.000000 tmkit-0.0.2/tmkit/topology/pdbtm/Component.py
--rw-rw-rw-   0        0        0     3246 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/topology/pdbtm/Determine.py
--rw-rw-rw-   0        0        0     3729 2023-06-29 20:03:03.000000 tmkit-0.0.2/tmkit/topology/pdbtm/Segment.py
--rw-rw-rw-   0        0        0     1486 2023-06-29 22:02:28.000000 tmkit-0.0.2/tmkit/topology/pdbtm/TMH.py
--rw-rw-rw-   0        0        0     2216 2023-06-29 20:03:03.000000 tmkit-0.0.2/tmkit/topology/pdbtm/ToFastaId.py
--rw-rw-rw-   0        0        0        0 2019-11-07 10:51:46.000000 tmkit-0.0.2/tmkit/topology/pdbtm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.160836 tmkit-0.0.2/tmkit/util/
--rw-rw-rw-   0        0        0      890 2023-06-19 10:50:53.000000 tmkit-0.0.2/tmkit/util/Console.py
--rw-rw-rw-   0        0        0     3398 2023-07-03 16:58:24.000000 tmkit-0.0.2/tmkit/util/Kit.py
--rw-rw-rw-   0        0        0     2782 2023-07-02 17:02:29.000000 tmkit-0.0.2/tmkit/util/Reader.py
--rw-rw-rw-   0        0        0     2525 2023-07-02 15:53:41.000000 tmkit-0.0.2/tmkit/util/Writer.py
--rw-rw-rw-   0        0        0        0 2022-07-15 19:58:41.000000 tmkit-0.0.2/tmkit/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.163835 tmkit-0.0.2/tmkit/visualize/
--rw-rw-rw-   0        0        0        0 2022-08-07 22:43:33.000000 tmkit-0.0.2/tmkit/visualize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.182836 tmkit-0.0.2/tmkit/visualize/component/
--rw-rw-rw-   0        0        0      398 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/Color.py
--rw-rw-rw-   0        0        0     3872 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/InterfaceResidues.py
--rw-rw-rw-   0        0        0      416 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/Select.py
--rw-rw-rw-   0        0        0        0 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/__init__.py
--rw-rw-rw-   0        0        0     2955 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/focal_blur.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.189868 tmkit-0.0.2/tmkit/visualize/component/palette/
--rw-rw-rw-   0        0        0        0 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/palette/__init__.py
--rw-rw-rw-   0        0        0     8639 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/palette/data2bfactor.py
--rw-rw-rw-   0        0        0     3699 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/palette/spectrumany.py
--rw-rw-rw-   0        0        0    14522 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/component/show_contacts.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.195837 tmkit-0.0.2/tmkit/visualize/func/
--rw-rw-rw-   0        0        0     2040 2023-07-02 13:29:15.000000 tmkit-0.0.2/tmkit/visualize/func/Coloring.py
--rw-rw-rw-   0        0        0        0 2022-08-11 11:29:35.000000 tmkit-0.0.2/tmkit/visualize/func/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.204839 tmkit-0.0.2/tmkit/visualize/isite/
--rw-rw-rw-   0        0        0     5478 2023-06-29 20:10:11.000000 tmkit-0.0.2/tmkit/visualize/isite/Labelling.py
--rw-rw-rw-   0        0        0     4010 2023-07-03 16:41:03.000000 tmkit-0.0.2/tmkit/visualize/isite/ProtocolDeepTMInter.py
--rw-rw-rw-   0        0        0        0 2020-12-31 08:21:51.000000 tmkit-0.0.2/tmkit/visualize/isite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:43.228837 tmkit-0.0.2/tmkit/visualize/small/
--rw-rw-rw-   0        0        0      640 2023-07-02 13:35:02.000000 tmkit-0.0.2/tmkit/visualize/small/Label.py
--rw-rw-rw-   0        0        0     2313 2023-07-02 13:29:15.000000 tmkit-0.0.2/tmkit/visualize/small/Local.py
--rw-rw-rw-   0        0        0      473 2023-07-02 13:33:44.000000 tmkit-0.0.2/tmkit/visualize/small/Palette.py
--rw-rw-rw-   0        0        0      664 2023-07-02 15:53:41.000000 tmkit-0.0.2/tmkit/visualize/small/Select.py
--rw-rw-rw-   0        0        0      405 2023-07-02 13:35:02.000000 tmkit-0.0.2/tmkit/visualize/small/Style.py
--rw-rw-rw-   0        0        0        0 2021-01-01 12:44:05.000000 tmkit-0.0.2/tmkit/visualize/small/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-06-29 21:36:51.000000 tmkit-0.0.2/tmkit/vs.py
-drwxrwxrwx   0        0        0        0 2023-07-06 18:43:42.877836 tmkit-0.0.2/tmkit.egg-info/
--rw-rw-rw-   0        0        0      300 2023-07-06 18:43:42.000000 tmkit-0.0.2/tmkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3766 2023-07-06 18:43:42.000000 tmkit-0.0.2/tmkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:43:42.000000 tmkit-0.0.2/tmkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-07-06 18:43:42.000000 tmkit-0.0.2/tmkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-06 18:43:42.000000 tmkit-0.0.2/tmkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:42.062923 tmkit-0.0.3/
+-rw-rw-rw-   0        0        0    33091 2023-07-06 20:59:29.000000 tmkit-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      300 2023-07-09 23:54:42.060921 tmkit-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6438 2023-07-09 23:30:12.000000 tmkit-0.0.3/README.md
+-rw-rw-rw-   0        0        0     4184 2023-07-09 13:37:54.000000 tmkit-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 23:54:42.062923 tmkit-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-07-09 23:54:34.000000 tmkit-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.673921 tmkit-0.0.3/tests/
+-rw-rw-rw-   0        0        0      490 2023-07-09 13:33:56.000000 tmkit-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      233 2023-07-09 13:33:56.000000 tmkit-0.0.3/tests/cath_test.py
+-rw-rw-rw-   0        0        0      322 2023-07-09 13:33:56.000000 tmkit-0.0.3/tests/collation_test.py
+-rw-rw-rw-   0        0        0      168 2023-07-06 20:59:29.000000 tmkit-0.0.3/tests/conftest.py
+-rw-rw-rw-   0        0        0      697 2023-07-09 13:33:56.000000 tmkit-0.0.3/tests/feature_test.py
+-rw-rw-rw-   0        0        0      260 2023-07-09 13:33:56.000000 tmkit-0.0.3/tests/mapping_test.py
+-rw-rw-rw-   0        0        0        0 2023-07-09 13:33:56.000000 tmkit-0.0.3/tests/mutation_test.py
+-rw-rw-rw-   0        0        0      572 2023-07-09 13:33:56.000000 tmkit-0.0.3/tests/residue_contact_test.py
+-rw-rw-rw-   0        0        0      556 2023-07-09 13:33:56.000000 tmkit-0.0.3/tests/sequence_test.py
+-rw-rw-rw-   0        0        0      619 2023-07-09 13:33:56.000000 tmkit-0.0.3/tests/topology_test.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.727924 tmkit-0.0.3/tmkit/
+-rw-rw-rw-   0        0        0       33 2023-07-09 17:40:04.000000 tmkit-0.0.3/tmkit/.env
+-rw-rw-rw-   0        0        0      753 2023-07-06 23:31:54.000000 tmkit-0.0.3/tmkit/Path.py
+-rw-rw-rw-   0        0        0     1360 2023-07-09 13:33:54.000000 tmkit-0.0.3/tmkit/__init__.py
+-rw-rw-rw-   0        0        0     1619 2023-07-06 20:59:29.000000 tmkit-0.0.3/tmkit/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.760927 tmkit-0.0.3/tmkit/base/
+-rw-rw-rw-   0        0        0     7086 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/base/PDB.py
+-rw-rw-rw-   0        0        0     1861 2023-07-09 21:09:07.000000 tmkit-0.0.3/tmkit/base/Position.py
+-rw-rw-rw-   0        0        0       78 2023-07-06 20:59:29.000000 tmkit-0.0.3/tmkit/base/__init__.py
+-rw-rw-rw-   0        0        0     3667 2023-07-09 16:19:45.000000 tmkit-0.0.3/tmkit/cath.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.773921 tmkit-0.0.3/tmkit/chain/
+-rw-rw-rw-   0        0        0     5363 2023-07-09 18:57:08.000000 tmkit-0.0.3/tmkit/chain/Collate.py
+-rw-rw-rw-   0        0        0     9360 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/chain/CollateBatch.py
+-rw-rw-rw-   0        0        0     1012 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/chain/PDB.py
+-rw-rw-rw-   0        0        0        0 2022-08-06 11:29:10.000000 tmkit-0.0.3/tmkit/chain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.778921 tmkit-0.0.3/tmkit/channel/
+-rw-rw-rw-   0        0        0     7510 2023-07-09 21:41:44.000000 tmkit-0.0.3/tmkit/channel/Workbench.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 19:08:40.000000 tmkit-0.0.3/tmkit/channel/__init__.py
+-rw-rw-rw-   0        0        0     5140 2023-07-09 19:00:20.000000 tmkit-0.0.3/tmkit/collate.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.785951 tmkit-0.0.3/tmkit/contact/
+-rw-rw-rw-   0        0        0    11083 2023-07-09 21:27:32.000000 tmkit-0.0.3/tmkit/contact/Evaluator.py
+-rw-rw-rw-   0        0        0    35763 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/contact/Reader.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 18:38:08.000000 tmkit-0.0.3/tmkit/contact/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.793952 tmkit-0.0.3/tmkit/db/
+-rw-rw-rw-   0        0        0     8365 2023-07-09 20:56:10.000000 tmkit-0.0.3/tmkit/db/Connectivity.py
+-rw-rw-rw-   0        0        0     7069 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/db/Reader.py
+-rw-rw-rw-   0        0        0        0 2019-05-10 13:10:28.000000 tmkit-0.0.3/tmkit/db/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.799921 tmkit-0.0.3/tmkit/db/biogrid/
+-rw-rw-rw-   0        0        0     3606 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/db/biogrid/Reader.py
+-rw-rw-rw-   0        0        0        0 2020-07-08 14:38:06.000000 tmkit-0.0.3/tmkit/db/biogrid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.805922 tmkit-0.0.3/tmkit/db/cath/
+-rw-rw-rw-   0        0        0     7723 2023-07-09 16:15:52.000000 tmkit-0.0.3/tmkit/db/cath/Reader.py
+-rw-rw-rw-   0        0        0        0 2022-08-11 11:28:12.000000 tmkit-0.0.3/tmkit/db/cath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.809952 tmkit-0.0.3/tmkit/db/construct/
+-rw-rw-rw-   0        0        0     4000 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/db/construct/Network.py
+-rw-rw-rw-   0        0        0        0 2020-08-28 22:57:35.000000 tmkit-0.0.3/tmkit/db/construct/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.814923 tmkit-0.0.3/tmkit/db/intact/
+-rw-rw-rw-   0        0        0     3772 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/db/intact/Reader.py
+-rw-rw-rw-   0        0        0        0 2020-07-11 22:05:59.000000 tmkit-0.0.3/tmkit/db/intact/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.820925 tmkit-0.0.3/tmkit/db/muthtp/
+-rw-rw-rw-   0        0        0     4959 2023-07-09 19:55:18.000000 tmkit-0.0.3/tmkit/db/muthtp/Reader.py
+-rw-rw-rw-   0        0        0        0 2022-08-07 05:11:20.000000 tmkit-0.0.3/tmkit/db/muthtp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.825921 tmkit-0.0.3/tmkit/db/predmuthtp/
+-rw-rw-rw-   0        0        0     4235 2023-07-09 19:55:18.000000 tmkit-0.0.3/tmkit/db/predmuthtp/Reader.py
+-rw-rw-rw-   0        0        0        0 2022-08-07 05:11:42.000000 tmkit-0.0.3/tmkit/db/predmuthtp/__init__.py
+-rw-rw-rw-   0        0        0     2198 2023-07-09 22:31:14.000000 tmkit-0.0.3/tmkit/edge.py
+-rw-rw-rw-   0        0        0     9190 2023-07-09 18:40:22.000000 tmkit-0.0.3/tmkit/feature.py
+-rw-rw-rw-   0        0        0     1139 2023-07-09 23:08:29.000000 tmkit-0.0.3/tmkit/fetch.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.834947 tmkit-0.0.3/tmkit/id/
+-rw-rw-rw-   0        0        0      974 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/id/Fasta.py
+-rw-rw-rw-   0        0        0     3205 2023-07-09 19:06:34.000000 tmkit-0.0.3/tmkit/id/Mapping.py
+-rw-rw-rw-   0        0        0     1275 2023-07-09 14:28:43.000000 tmkit-0.0.3/tmkit/id/PDB.py
+-rw-rw-rw-   0        0        0        0 2020-04-26 23:07:36.000000 tmkit-0.0.3/tmkit/id/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.841921 tmkit-0.0.3/tmkit/interface/
+-rw-rw-rw-   0        0        0     1023 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/interface/Tool.py
+-rw-rw-rw-   0        0        0      956 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/interface/Topology.py
+-rw-rw-rw-   0        0        0        0 2020-07-09 17:22:43.000000 tmkit-0.0.3/tmkit/interface/__init__.py
+-rw-rw-rw-   0        0        0     1260 2023-07-09 19:06:34.000000 tmkit-0.0.3/tmkit/mapping.py
+-rw-rw-rw-   0        0        0     6675 2023-07-09 19:35:43.000000 tmkit-0.0.3/tmkit/msa.py
+-rw-rw-rw-   0        0        0     2925 2023-07-09 19:55:18.000000 tmkit-0.0.3/tmkit/mut.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.846922 tmkit-0.0.3/tmkit/name/
+-rw-rw-rw-   0        0        0     4501 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/name/Mapping.py
+-rw-rw-rw-   0        0        0        0 2022-08-06 12:13:25.000000 tmkit-0.0.3/tmkit/name/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.848921 tmkit-0.0.3/tmkit/position/
+-rw-rw-rw-   0        0        0       14 2023-07-06 20:59:29.000000 tmkit-0.0.3/tmkit/position/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.857920 tmkit-0.0.3/tmkit/position/scenario/
+-rw-rw-rw-   0        0        0     1585 2023-07-09 21:14:59.000000 tmkit-0.0.3/tmkit/position/scenario/Segment.py
+-rw-rw-rw-   0        0        0     3397 2023-07-09 21:33:23.000000 tmkit-0.0.3/tmkit/position/scenario/Separation.py
+-rw-rw-rw-   0        0        0        0 2019-09-21 21:40:26.000000 tmkit-0.0.3/tmkit/position/scenario/__init__.py
+-rw-rw-rw-   0        0        0     5473 2023-07-09 21:05:05.000000 tmkit-0.0.3/tmkit/ppi.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.864921 tmkit-0.0.3/tmkit/property/
+-rw-rw-rw-   0        0        0     8055 2023-07-09 18:03:26.000000 tmkit-0.0.3/tmkit/property/HelixSurface.py
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:58:24.000000 tmkit-0.0.3/tmkit/property/__init__.py
+-rw-rw-rw-   0        0        0     8522 2023-07-02 22:18:52.000000 tmkit-0.0.3/tmkit/property/lips.pl
+-rw-rw-rw-   0        0        0     2336 2023-07-09 21:41:44.000000 tmkit-0.0.3/tmkit/qc.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.874922 tmkit-0.0.3/tmkit/retrieve/
+-rw-rw-rw-   0        0        0    15127 2023-07-09 19:41:45.000000 tmkit-0.0.3/tmkit/retrieve/MSA.py
+-rw-rw-rw-   0        0        0     4487 2023-07-09 14:21:14.000000 tmkit-0.0.3/tmkit/retrieve/PDB.py
+-rw-rw-rw-   0        0        0     2253 2023-07-09 14:21:14.000000 tmkit-0.0.3/tmkit/retrieve/XML.py
+-rw-rw-rw-   0        0        0        0 2019-05-10 15:10:49.000000 tmkit-0.0.3/tmkit/retrieve/__init__.py
+-rw-rw-rw-   0        0        0     6561 2023-07-09 21:30:40.000000 tmkit-0.0.3/tmkit/rrc.py
+-rw-rw-rw-   0        0        0     6082 2023-07-09 14:44:50.000000 tmkit-0.0.3/tmkit/seq.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.884952 tmkit-0.0.3/tmkit/seqnetrr/
+-rw-rw-rw-   0        0        0     7895 2023-07-09 21:27:32.000000 tmkit-0.0.3/tmkit/seqnetrr/Compare.py
+-rw-rw-rw-   0        0        0     3347 2023-07-06 22:57:46.000000 tmkit-0.0.3/tmkit/seqnetrr/ComputLib.py
+-rw-rw-rw-   0        0        0    12814 2023-07-09 22:30:50.000000 tmkit-0.0.3/tmkit/seqnetrr/Controller.py
+-rw-rw-rw-   0        0        0        0 2022-05-17 20:55:49.000000 tmkit-0.0.3/tmkit/seqnetrr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.898921 tmkit-0.0.3/tmkit/seqnetrr/combo/
+-rw-rw-rw-   0        0        0     2345 2023-07-09 22:47:53.000000 tmkit-0.0.3/tmkit/seqnetrr/combo/Length.py
+-rw-rw-rw-   0        0        0     1328 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/seqnetrr/combo/Param.py
+-rw-rw-rw-   0        0        0     2609 2023-07-09 22:47:53.000000 tmkit-0.0.3/tmkit/seqnetrr/combo/Position.py
+-rw-rw-rw-   0        0        0     4561 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/seqnetrr/combo/Separation.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 16:35:38.000000 tmkit-0.0.3/tmkit/seqnetrr/combo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.909961 tmkit-0.0.3/tmkit/seqnetrr/graph/
+-rw-rw-rw-   0        0        0    18542 2023-07-09 22:47:53.000000 tmkit-0.0.3/tmkit/seqnetrr/graph/Bipartite.py
+-rw-rw-rw-   0        0        0     4605 2023-07-09 22:47:53.000000 tmkit-0.0.3/tmkit/seqnetrr/graph/Cumulative.py
+-rw-rw-rw-   0        0        0    19498 2023-07-09 22:47:53.000000 tmkit-0.0.3/tmkit/seqnetrr/graph/Unipartite.py
+-rw-rw-rw-   0        0        0        0 2022-05-18 21:29:35.000000 tmkit-0.0.3/tmkit/seqnetrr/graph/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.914922 tmkit-0.0.3/tmkit/seqnetrr/net/
+-rw-rw-rw-   0        0        0    24193 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/seqnetrr/net/Reader.py
+-rw-rw-rw-   0        0        0        0 2022-06-12 23:19:50.000000 tmkit-0.0.3/tmkit/seqnetrr/net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.922922 tmkit-0.0.3/tmkit/seqnetrr/window/
+-rw-rw-rw-   0        0        0     4953 2023-07-09 22:47:53.000000 tmkit-0.0.3/tmkit/seqnetrr/window/Pair.py
+-rw-rw-rw-   0        0        0     3588 2023-07-09 22:47:53.000000 tmkit-0.0.3/tmkit/seqnetrr/window/Single.py
+-rw-rw-rw-   0        0        0        0 2019-09-18 20:19:22.000000 tmkit-0.0.3/tmkit/seqnetrr/window/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.929923 tmkit-0.0.3/tmkit/seqnetrr/window/base/
+-rw-rw-rw-   0        0        0     1291 2023-07-06 23:05:49.000000 tmkit-0.0.3/tmkit/seqnetrr/window/base/Pair.py
+-rw-rw-rw-   0        0        0     1293 2023-07-06 23:05:49.000000 tmkit-0.0.3/tmkit/seqnetrr/window/base/Single.py
+-rw-rw-rw-   0        0        0        0 2019-09-19 13:22:58.000000 tmkit-0.0.3/tmkit/seqnetrr/window/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.942959 tmkit-0.0.3/tmkit/sequence/
+-rw-rw-rw-   0        0        0      834 2023-07-09 14:08:51.000000 tmkit-0.0.3/tmkit/sequence/Fasta.py
+-rw-rw-rw-   0        0        0     1425 2023-07-06 20:59:29.000000 tmkit-0.0.3/tmkit/sequence/Index.py
+-rw-rw-rw-   0        0        0     2001 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/sequence/PDB.py
+-rw-rw-rw-   0        0        0     1344 2023-07-09 13:45:59.000000 tmkit-0.0.3/tmkit/sequence/XML.py
+-rw-rw-rw-   0        0        0        0 2019-08-02 11:12:19.000000 tmkit-0.0.3/tmkit/sequence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.947952 tmkit-0.0.3/tmkit/structure/
+-rw-rw-rw-   0        0        0     3854 2023-07-09 17:54:06.000000 tmkit-0.0.3/tmkit/structure/PDB.py
+-rw-rw-rw-   0        0        0        0 2019-08-02 11:11:48.000000 tmkit-0.0.3/tmkit/structure/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.952952 tmkit-0.0.3/tmkit/structure/ppi/
+-rw-rw-rw-   0        0        0     3180 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/structure/ppi/Label.py
+-rw-rw-rw-   0        0        0        0 2019-09-15 17:30:37.000000 tmkit-0.0.3/tmkit/structure/ppi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.956922 tmkit-0.0.3/tmkit/structure/rrc/
+-rw-rw-rw-   0        0        0     2811 2023-07-09 21:02:23.000000 tmkit-0.0.3/tmkit/structure/rrc/Label.py
+-rw-rw-rw-   0        0        0        0 2019-09-15 17:30:31.000000 tmkit-0.0.3/tmkit/structure/rrc/__init__.py
+-rw-rw-rw-   0        0        0     7318 2023-07-09 22:02:47.000000 tmkit-0.0.3/tmkit/topo.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.965923 tmkit-0.0.3/tmkit/topology/
+-rw-rw-rw-   0        0        0     6120 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/topology/Phobius.py
+-rw-rw-rw-   0        0        0     7750 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/topology/TMHMM.py
+-rw-rw-rw-   0        0        0        0 2019-05-10 13:11:26.000000 tmkit-0.0.3/tmkit/topology/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.970923 tmkit-0.0.3/tmkit/topology/lib/
+-rw-rw-rw-   0        0        0    25043 2022-07-15 23:01:47.000000 tmkit-0.0.3/tmkit/topology/lib/Phobius.py
+-rw-rw-rw-   0        0        0        0 2022-07-16 23:17:45.000000 tmkit-0.0.3/tmkit/topology/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.984922 tmkit-0.0.3/tmkit/topology/pdbtm/
+-rw-rw-rw-   0        0        0     5753 2023-07-06 23:17:47.000000 tmkit-0.0.3/tmkit/topology/pdbtm/Component.py
+-rw-rw-rw-   0        0        0     3843 2023-07-09 22:02:47.000000 tmkit-0.0.3/tmkit/topology/pdbtm/Determine.py
+-rw-rw-rw-   0        0        0     9926 2023-07-09 21:56:26.000000 tmkit-0.0.3/tmkit/topology/pdbtm/Segment.py
+-rw-rw-rw-   0        0        0     1324 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/topology/pdbtm/TMH.py
+-rw-rw-rw-   0        0        0     2940 2023-07-06 23:17:47.000000 tmkit-0.0.3/tmkit/topology/pdbtm/ToFastaId.py
+-rw-rw-rw-   0        0        0        0 2019-11-07 10:51:46.000000 tmkit-0.0.3/tmkit/topology/pdbtm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.996922 tmkit-0.0.3/tmkit/util/
+-rw-rw-rw-   0        0        0      934 2023-07-06 23:17:47.000000 tmkit-0.0.3/tmkit/util/Console.py
+-rw-rw-rw-   0        0        0    10911 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/util/Kit.py
+-rw-rw-rw-   0        0        0     5143 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/util/Reader.py
+-rw-rw-rw-   0        0        0     6845 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/util/Writer.py
+-rw-rw-rw-   0        0        0        0 2022-07-15 19:58:41.000000 tmkit-0.0.3/tmkit/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.998921 tmkit-0.0.3/tmkit/visualize/
+-rw-rw-rw-   0        0        0        0 2022-08-07 22:43:33.000000 tmkit-0.0.3/tmkit/visualize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:42.020921 tmkit-0.0.3/tmkit/visualize/component/
+-rw-rw-rw-   0        0        0      390 2023-07-09 22:23:17.000000 tmkit-0.0.3/tmkit/visualize/component/Color.py
+-rw-rw-rw-   0        0        0     4525 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/visualize/component/InterfaceResidues.py
+-rw-rw-rw-   0        0        0      402 2023-07-09 22:23:17.000000 tmkit-0.0.3/tmkit/visualize/component/Select.py
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:42:45.000000 tmkit-0.0.3/tmkit/visualize/component/__init__.py
+-rw-rw-rw-   0        0        0     2938 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/visualize/component/focal_blur.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:42.029923 tmkit-0.0.3/tmkit/visualize/component/palette/
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:42:45.000000 tmkit-0.0.3/tmkit/visualize/component/palette/__init__.py
+-rw-rw-rw-   0        0        0     9141 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/visualize/component/palette/data2bfactor.py
+-rw-rw-rw-   0        0        0     3956 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/visualize/component/palette/spectrumany.py
+-rw-rw-rw-   0        0        0    14198 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/visualize/component/show_contacts.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:42.034924 tmkit-0.0.3/tmkit/visualize/func/
+-rw-rw-rw-   0        0        0     2755 2023-07-09 22:17:28.000000 tmkit-0.0.3/tmkit/visualize/func/Coloring.py
+-rw-rw-rw-   0        0        0        0 2022-08-11 11:29:35.000000 tmkit-0.0.3/tmkit/visualize/func/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:42.042920 tmkit-0.0.3/tmkit/visualize/isite/
+-rw-rw-rw-   0        0        0     7220 2023-07-09 22:24:39.000000 tmkit-0.0.3/tmkit/visualize/isite/Labelling.py
+-rw-rw-rw-   0        0        0     5037 2023-07-09 22:23:17.000000 tmkit-0.0.3/tmkit/visualize/isite/ProtocolDeepTMInter.py
+-rw-rw-rw-   0        0        0        0 2020-12-31 08:21:51.000000 tmkit-0.0.3/tmkit/visualize/isite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:42.058922 tmkit-0.0.3/tmkit/visualize/small/
+-rw-rw-rw-   0        0        0     1169 2023-07-06 23:24:34.000000 tmkit-0.0.3/tmkit/visualize/small/Label.py
+-rw-rw-rw-   0        0        0     2595 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/visualize/small/Local.py
+-rw-rw-rw-   0        0        0      898 2023-07-07 14:29:23.000000 tmkit-0.0.3/tmkit/visualize/small/Palette.py
+-rw-rw-rw-   0        0        0     1259 2023-07-06 20:59:29.000000 tmkit-0.0.3/tmkit/visualize/small/Select.py
+-rw-rw-rw-   0        0        0      663 2023-07-06 23:24:34.000000 tmkit-0.0.3/tmkit/visualize/small/Style.py
+-rw-rw-rw-   0        0        0        0 2021-01-01 12:44:05.000000 tmkit-0.0.3/tmkit/visualize/small/__init__.py
+-rw-rw-rw-   0        0        0     5555 2023-07-09 22:13:29.000000 tmkit-0.0.3/tmkit/vs.py
+drwxrwxrwx   0        0        0        0 2023-07-09 23:54:41.750953 tmkit-0.0.3/tmkit.egg-info/
+-rw-rw-rw-   0        0        0      300 2023-07-09 23:54:41.000000 tmkit-0.0.3/tmkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4055 2023-07-09 23:54:41.000000 tmkit-0.0.3/tmkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 23:54:41.000000 tmkit-0.0.3/tmkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-07-09 23:54:41.000000 tmkit-0.0.3/tmkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-09 23:54:41.000000 tmkit-0.0.3/tmkit.egg-info/top_level.txt
```

### Comparing `tmkit-0.0.2/LICENSE` & `tmkit-0.0.3/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
                     GNU GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
   The GNU General Public License is a free, copyleft license for
 software and other kinds of works.
@@ -614,61 +614,8 @@
   If the disclaimer of warranty and limitation of liability provided
 above cannot be given local legal effect according to their terms,
 reviewing courts shall apply local law that most closely approximates
 an absolute waiver of all civil liability in connection with the
 Program, unless a warranty or assumption of liability accompanies a
 copy of the Program in return for a fee.
 
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                     END OF TERMS AND CONDITIONS
```

### Comparing `tmkit-0.0.2/tmkit/cath.py` & `tmkit-0.0.3/tmkit/topology/pdbtm/TMH.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,48 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
-__maintainer__ = "Jianfeng Sun"
 
-from tmkit.db.cath.Reader import reader as cathreader
+from typing import List, Tuple
 
+from tmkit.topology.pdbtm.Segment import Segment
 
-def summary_by_id(
-        id,
-):
-    """
-
-    Parameters
-    ----------
-    id
-
-    Returns
-    -------
-
-    """
-    return cathreader().api(identifier=id)
-
-
-def fetch_by_id(
-        id,
-):
-    """
-
-    Parameters
-    ----------
-    id
-
-    Returns
-    -------
-
-    """
-    return cathreader().fetch(domain_id=id, sort='domain')
-
-
-def download(
-        sv_fp,
-        version='newest',
-):
-    return cathreader().download(
-        version=version,
-        sv_fp=sv_fp,
-    )
-
-
-def read(
-        cath_fpn,
-        groupby,
-        group,
-):
-    """
-
-    Parameters
-    ----------
-    cath_fpn
-    groupby
-    group
-
-    Returns
-    -------
-
-    """
-    return cathreader().domain(
-        cath_fpn, groupby=groupby, group=group
-    )
-
-
-def fftojson(
-        df_prot,
-        df_cath_domain,
-        sv_fpn,
-        targets=[
-            'funfam_number',
-            'superfamily_id',
-            'pdb_segments',
-        ],
-):
-    """
-
-    Parameters
-    ----------
-    df_prot
-    df_cath_domain
-    sv_fpn
-    targets
-
-    Returns
-    -------
-
-    """
-    return cathreader().funfamsToJson(
-        df_prot=df_prot,
-        df_domain=df_cath_domain,
-        sv_fpn=sv_fpn,
-        targets=targets,
-    )
+
+class TMH:
+    def __init__(self, xml_fp: str, prot_name: str, seq_chain: str) -> None:
+        """
+        Initialize a TMH object.
+
+        Parameters
+        ----------
+        xml_fp : str
+            The filepath of the XML file.
+        prot_name : str
+            The name of the protein.
+        seq_chain : str
+            The sequence chain of the protein.
+
+        Returns
+        -------
+        None
+        """
+        self.xml_fp = xml_fp
+        self.prot_name = prot_name
+        self.seq_chain = seq_chain
+
+    def get(self) -> Tuple[List[int], List[int]]:
+        """
+        Get the start and end positions of the transmembrane helices.
+
+        Returns
+        -------
+        Tuple[List[int], List[int]]
+            A tuple containing two lists: the start positions and the end positions of the transmembrane helices.
+        """
+        start_id, last_id = Segment().tmh(
+            xml_fp=self.xml_fp,
+            prot_name=self.prot_name,
+            seq_chain=self.seq_chain,
+        )
+        return start_id, last_id
```

### Comparing `tmkit-0.0.2/tmkit/chain/CollateBatch.py` & `tmkit-0.0.3/tmkit/chain/CollateBatch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,82 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-from tmkit.util.Kit import tactic5
-from tmkit.sequence.PDB import pdb as spdb
-from tmkit.util.Kit import seqchainid
-from Bio import BiopythonWarning
+from typing import Dict, List, Union
+
 import warnings
 
+import pandas as pd
+from Bio import BiopythonWarning
+
+from tmkit.sequence.PDB import PDB as spdb
+from tmkit.util.Kit import seqchainid, tactic5
+
 
-class collateBatch:
+class CollateBatch:
+    """
+    Class for collating protein data from PDBTM and RCSB databases.
+
+    Parameters
+    ----------
+    prot_df : pd.DataFrame
+        DataFrame containing protein data.
+    pdb_rcsb_fp : str
+        Filepath for RCSB PDB file.
+    pdb_pdbtm_fp : str
+        Filepath for PDBTM PDB file.
+    prot_pdbtm_df : pd.DataFrame
+        DataFrame containing PDBTM protein data.
+    prot_rcsb_df : pd.DataFrame
+        DataFrame containing RCSB protein data.
+    strategy : str, optional
+        Strategy for collating data. Default is "diff".
+
+    Attributes
+    ----------
+    prot_df : pd.DataFrame
+        DataFrame containing protein data.
+    pdb_rcsb_fp : str
+        Filepath for RCSB PDB file.
+    pdb_pdbtm_fp : str
+        Filepath for PDBTM PDB file.
+    prot_collated_df : pd.DataFrame
+        DataFrame containing collated protein data.
+    """
 
     def __init__(
-            self,
-            prot_df,
-            pdb_rcsb_fp,
-            pdb_pdbtm_fp,
-            prot_pdbtm_df,
-            prot_rcsb_df,
-            strategy='diff',
-    ):
+        self,
+        prot_df: pd.DataFrame,
+        pdb_rcsb_fp: str,
+        pdb_pdbtm_fp: str,
+        prot_pdbtm_df: pd.DataFrame,
+        prot_rcsb_df: pd.DataFrame,
+        strategy: str = "diff",
+    ) -> None:
         self.prot_df = prot_df
         self.pdb_rcsb_fp = pdb_rcsb_fp
         self.pdb_pdbtm_fp = pdb_pdbtm_fp
 
         self.prot_collated_df = self.rcsb(
             prot_pdbtm_df=prot_pdbtm_df,
             prot_rcsb_df=prot_rcsb_df,
             strategy=strategy,
         )
 
-        # print('======>basic info: \n{}'.format(self.prot_collated_df))
+        print(f"======>basic info: \n{self.prot_collated_df}")
 
-    def rcsb(self, prot_pdbtm_df, prot_rcsb_df, strategy):
+    def rcsb(
+        self, prot_pdbtm_df: pd.DataFrame, prot_rcsb_df: pd.DataFrame, strategy: str
+    ) -> pd.DataFrame:
         """
+        Collates protein data from PDBTM and RCSB databases.
 
         Notes
         -----
             It contains 6 columns:
                 1> 0
                 2> 1
                 3> pdbtm
@@ -61,128 +97,165 @@
             shown 'rcsb', which means all chains of a self.prot_df in PDBTM
             can be found in RCSB.
 
             strategy_dict stores the same or different chains between PDBTM and RCSB.
 
         Parameters
         ----------
-        self.prot_df
-        prot_pdbtm_df
-        prot_rcsb_df
-        strategy
+        prot_pdbtm_df : pd.DataFrame
+            DataFrame containing PDBTM protein data.
+        prot_rcsb_df : pd.DataFrame
+            DataFrame containing RCSB protein data.
+        strategy : str
+            Strategy for collating data.
 
         Returns
         -------
-
+        pd.DataFrame
+            DataFrame containing collated protein data.
         """
-        prot_pdbtm_dict = tactic5(prot_pdbtm_df.values)
-        prot_rcsb_dict = tactic5(prot_rcsb_df.values)
-        strategy_dict = {}
+        prot_pdbtm_dict: Dict[str, List[str]] = tactic5(prot_pdbtm_df.values)
+        prot_rcsb_dict: Dict[str, List[str]] = tactic5(prot_rcsb_df.values)
+        strategy_dict: Dict[str, List[str]] = {}
         for prot_name in prot_pdbtm_dict.keys():
             A = prot_pdbtm_dict[prot_name]
             B = prot_rcsb_dict[prot_name]
-            if strategy == 'diff':
+            if strategy == "diff":
                 strategy_dict[prot_name] = list(set(A).difference(set(B)))
             else:
                 strategy_dict[prot_name] = list(set(A).intersection(set(B)))
-        self.prot_df['pdbtm'] = 'NaN'
-        self.prot_df['rcsb'] = 'NaN'
-        if strategy == 'diff':
-            self.prot_df['diff'] = 'NaN'
+        self.prot_df["pdbtm"] = "NaN"
+        self.prot_df["rcsb"] = "NaN"
+        if strategy == "diff":
+            self.prot_df["diff"] = "NaN"
         else:
-            self.prot_df['same'] = 'NaN'
-        self.prot_df['source'] = 'NaN'
+            self.prot_df["same"] = "NaN"
+        self.prot_df["source"] = "NaN"
         # print(strategy_dict)
         for i in self.prot_df.index:
-            self.prot_df.loc[i, 'pdbtm'] = ''.join(prot_pdbtm_dict[self.prot_df.iloc[i, 0]])
-            self.prot_df.loc[i, 'rcsb'] = ''.join(prot_rcsb_dict[self.prot_df.iloc[i, 0]])
-            if strategy == 'diff':
-                self.prot_df.loc[i, 'diff'] = ''.join(strategy_dict[self.prot_df.iloc[i, 0]])
+            self.prot_df.loc[i, "pdbtm"] = "".join(
+                prot_pdbtm_dict[self.prot_df.iloc[i, 0]]
+            )
+            self.prot_df.loc[i, "rcsb"] = "".join(
+                prot_rcsb_dict[self.prot_df.iloc[i, 0]]
+            )
+            if strategy == "diff":
+                self.prot_df.loc[i, "diff"] = "".join(
+                    strategy_dict[self.prot_df.iloc[i, 0]]
+                )
             else:
-                self.prot_df.loc[i, 'same'] = ''.join(strategy_dict[self.prot_df.iloc[i, 0]])
+                self.prot_df.loc[i, "same"] = "".join(
+                    strategy_dict[self.prot_df.iloc[i, 0]]
+                )
             if self.prot_df.iloc[i, 1] not in prot_rcsb_dict[self.prot_df.iloc[i, 0]]:
-                self.prot_df.loc[i, 'source'] = 'pdbtm'
+                self.prot_df.loc[i, "source"] = "pdbtm"
             else:
-                self.prot_df.loc[i, 'source'] = 'rcsb'
+                self.prot_df.loc[i, "source"] = "rcsb"
         # print(self.prot_df)
         return self.prot_df
 
-    def throwback(self, prot_collated_df, symbol='.'):
+    def throwback(
+        self, prot_collated_df: pd.DataFrame, symbol: str = "."
+    ) -> Dict[str, str]:
         """
+        Throws back collated protein data.
 
         Notes
         -----
             throw_backs is a dict with keys being the collated protein chains
             corresponding to the chains in RCSB mapped from PDBTM, with the
             values 'untransformed' or 'collated' being whether protein chains
-             are untransformed or collated, respectively.
+            are untransformed or collated, respectively.
 
         Parameters
         ----------
-        prot_df
-        prot_collated_df
-        pdb_chain_path
-        symbol
+        prot_collated_df : pd.DataFrame
+            DataFrame containing collated protein data.
+        symbol : str, optional
+            Symbol to use for chain ID. Default is ".".
 
         Returns
         -------
-            dict - throw_backs
-
+        Dict[str, str]
+            Dictionary containing throwback data.
         """
-        throw_backs = {}
+        throw_backs: Dict[str, str] = {}
         for id in self.prot_df.index:
             prot_name = self.prot_df.loc[id, 0]
             prot_chain = self.prot_df.loc[id, 1]
-            if prot_collated_df.loc[id, 'source'] == 'rcsb':
-                throw_backs[prot_name + symbol + prot_chain] = 'untransformed'
+            if prot_collated_df.loc[id, "source"] == "rcsb":
+                throw_backs[prot_name + symbol + prot_chain] = "untransformed"
             else:
-                chain_collated_dict = self.areSameSeqs(
+                chain_collated_dict = self.are_same_seqs(
                     prot_name=prot_name,
                     chain_to_be_collated=[prot_chain],
-                    rcsb_chains=list(prot_collated_df['rcsb'][id]),
-                    symbol='.',
+                    rcsb_chains=list(prot_collated_df["rcsb"][id]),
+                    symbol=".",
                 )
                 if len([*chain_collated_dict.values()]) > 0:
-                    print('======>master is collated: {} '.format([*chain_collated_dict.values()][0]))
-                    throw_backs[[*chain_collated_dict.values()][0]] = 'collated'
+                    print(
+                        "======>master is collated: {} ".format(
+                            [*chain_collated_dict.values()][0]
+                        )
+                    )
+                    throw_backs[[*chain_collated_dict.values()][0]] = "collated"
                 else:
-                    throw_backs[[*chain_collated_dict]] = 'transformed'
+                    throw_backs[[*chain_collated_dict]] = "transformed"
         return throw_backs
 
-    def areSameSeqs(self, prot_name, chain_to_be_collated=[], rcsb_chains=[], symbol='.'):
+    def are_same_seqs(
+        self,
+        prot_name: str,
+        chain_to_be_collated: List[str],
+        rcsb_chains: List[str],
+        symbol: str = ".",
+    ) -> Dict[str, List[str]]:
         """
+        Checks if protein sequences are the same.
 
         Parameters
         ----------
-        prot_name
-        chain_to_be_collated
-        rcsb_chains
-        symbol
+        prot_name : str
+            Name of protein.
+        chain_to_be_collated : List[str]
+            List of chains to be collated.
+        rcsb_chains : List[str]
+            List of RCSB chains.
+        symbol : str, optional
+            Symbol to use for chain ID. Default is ".".
 
         Returns
         -------
-
+        Dict[str, List[str]]
+            Dictionary containing chain collation data.
         """
-        chain_collated_dict = {}
+        chain_collated_dict: Dict[str, List[str]] = {}
         with warnings.catch_warnings():
-            warnings.simplefilter('ignore', BiopythonWarning)
+            warnings.simplefilter("ignore", BiopythonWarning)
             for chain_pdbtm in chain_to_be_collated:
                 chain_collated_dict[prot_name + symbol + seqchainid(chain_pdbtm)] = []
                 seq_pdbtm = spdb(
                     pdb_fp=self.pdb_pdbtm_fp,
                     prot_name=prot_name,
                     seq_chain=seqchainid(chain_pdbtm),
-                    file_chain='',
+                    file_chain="",
                 ).chain()
                 for chain_rcsb in rcsb_chains:
                     seq_rcsb = spdb(
                         pdb_fp=self.pdb_rcsb_fp,
                         prot_name=prot_name,
                         seq_chain=seqchainid(chain_rcsb),
-                        file_chain='',
+                        file_chain="",
                     ).chain()
                     if seq_pdbtm == seq_rcsb:
-                        print('=========>{}.{} in PDBTM corresponds to {}.{} in RCSB.'.format(
-                            prot_name, seqchainid(chain_pdbtm), prot_name, seqchainid(chain_rcsb))
+                        print(
+                            "=========>{}.{} in PDBTM corresponds to {}.{} in RCSB.".format(
+                                prot_name,
+                                seqchainid(chain_pdbtm),
+                                prot_name,
+                                seqchainid(chain_rcsb),
+                            )
                         )
-                        chain_collated_dict[prot_name + symbol + seqchainid(chain_pdbtm)].append(prot_name + symbol + seqchainid(chain_rcsb))
-        return chain_collated_dict
+                        chain_collated_dict[
+                            prot_name + symbol + seqchainid(chain_pdbtm)
+                        ].append(prot_name + symbol + seqchainid(chain_rcsb))
+        return chain_collated_dict
```

### Comparing `tmkit-0.0.2/tmkit/contact/Evaluator.py` & `tmkit-0.0.3/tmkit/seqnetrr/Compare.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,219 +1,224 @@
-__author__ = "Jianfeng Sun"
-__version__ = "v1.0"
-__copyright__ = "Copyright 2023"
-__license__ = "GPL v3.0"
-__email__ = "jianfeng.sunmt@gmail.com"
-__maintainer__ = "Jianfeng Sun"
-
-import numpy as np
-import pandas as pd
-from sklearn import metrics
-from tmkit.contact.Reader import reader as rrcreader
-
-
-class evaluator:
-
-    def __init__(
-            self,
-            prot_name,
-            file_chain,
-            dist_df,
-            pair_list,
-            dist_limit=None,
-            tool=None,
-            tool_fp=None,
-            sort_=None,
-            seq_sep_inferior=None,
-            seq_sep_superior=None,
-    ):
-        self.tool_fp = tool_fp
-        self.prot_name = prot_name
-        self.file_chain = file_chain
-        self.dist_limit = dist_limit
-        self.pair_list = pair_list
-        self.tool = tool
-        self.sort_ = sort_
-        self.seq_sep_inferior = seq_sep_inferior
-        self.seq_sep_superior = seq_sep_superior
-        self.rrcreader = rrcreader(
-            seq_sep_inferior=self.seq_sep_inferior,
-            seq_sep_superior=self.seq_sep_superior
-        )
-        self.dist_df = dist_df
-        self.dist_df.columns = [
-            'fasta_id_1',
-            'aa_1',
-            'pdb_id_1',
-            'fasta_id_2',
-            'aa_2',
-            'pdb_id_2',
-            'dist',
-            'is_contact'
-        ]
-        self.row_real_dist = self.dist_df.shape[0]
-
-        print('======>Evaluating protein {}'.format(prot_name + file_chain))
-
-    def fetch(self):
-        switch = {
-            'psicov': self.psicov,
-            'freecontact': self.freecontact,
-            'ccmpred': self.ccmpred,
-            'gremlin': self.gremlin,
-            'gdca': self.gdca,
-            'plmc': self.plmc,
-            'memconp':self.memconp,
-            'membrain2':self.membrain2,
-            'tma165': self.tma165,
-        }
-        return switch[self.tool]()
-
-    def compare(self, target, cut_off):
-        # #/*** block fetch target results ***/
-        res_sorted = target.sort_values(['score'], ascending=False)
-        # self.pfwwriter.generic(res_sorted, sv_fpn='./cheers')
-        res_cutoff = res_sorted.iloc[0:cut_off, :]
-        new_index = np.arange(res_cutoff.shape[0])
-        res_cutoff = res_cutoff.set_index(new_index, inplace=False, drop=True)
-        # print(res_cutoff)
-        row_cutoff = res_cutoff.shape[0]
-        row_offset = target.shape[0] - row_cutoff
-        # #/*** block y_true_cutoff ***/
-        y_true_cutoff = []
-        for i in range(row_cutoff):
-            conid1 = self.dist_df['fasta_id_1'] == res_cutoff['fasta_id_1'][i]
-            conid2 = self.dist_df['fasta_id_2'] == res_cutoff['fasta_id_2'][i]
-            juery = (conid1) & (conid2)
-            tmp = self.dist_df.loc[juery]
-            y_true_cutoff.append(tmp['is_contact'].sum())
-        # #/*** block y_true_all ***/
-        y_true_all = list(res_sorted['is_contact'])
-        # #/*** block y_pred_all ***/
-        y_pred_all = list(
-            np.concatenate(
-                [np.zeros([row_cutoff]) + 1, np.zeros([row_offset])],
-                axis=0
-            ).astype(np.int64)
-        )
-        # #/*** block precision ***/
-        precision = metrics.precision_score(y_true=y_true_all, y_pred=y_pred_all)
-        print('=========>precision: {}'.format(precision))
-        # #/*** block recall ***/
-        recall = metrics.recall_score(y_true=y_true_all, y_pred=y_pred_all)
-        print('=========>recall: {}'.format(recall))
-        # #/*** block mcc ***/
-        mcc = metrics.matthews_corrcoef(y_true=y_true_all, y_pred=y_pred_all)
-        print('=========>mcc: {}'.format(mcc))
-        # #/*** block f1score ***/
-        f1score = metrics.f1_score(y_true=y_true_all, y_pred=y_pred_all)
-        print('=========>f1score: {}'.format(f1score))
-        # #/*** block accuracy ***/
-        accuracy = metrics.accuracy_score(y_true=y_true_all, y_pred=y_pred_all)
-        print('=========>accuracy: {}'.format(accuracy))
-        metrics_summary = {
-            'precision': precision,
-            'recall': recall,
-            'f1score': f1score,
-            'mcc': mcc,
-            'accuracy': accuracy,
-        }
-        return metrics_summary
-
-    def psicov(self):
-        pcv_dist, chain_dist_all = self.rrcreader.psicov(
-            pcv_path=self.tool_fp,
-            file_name=self.prot_name,
-            file_chain=self.file_chain,
-            pair_list=self.pair_list,
-            dist_df=self.dist_df,
-            sort_=self.sort_
-        )
-        return pd.concat([pcv_dist, chain_dist_all], axis=1)
-
-    def freecontact(self):
-        fc_dist, chain_dist_all = self.rrcreader.freecontact(
-            fc_path=self.tool_fp,
-            file_name=self.prot_name,
-            file_chain=self.file_chain,
-            pair_list=self.pair_list,
-            dist_df=self.dist_df,
-            sort_=self.sort_
-        )
-        return pd.concat([fc_dist, chain_dist_all], axis=1)
-
-    def ccmpred(self):
-        cp_dist, chain_dist_all = self.rrcreader.ccmpred(
-            cp_path=self.tool_fp,
-            file_name=self.prot_name,
-            file_chain=self.file_chain,
-            pair_list=self.pair_list,
-            dist_df=self.dist_df,
-            sort_=self.sort_
-        )
-        return pd.concat([cp_dist, chain_dist_all], axis=1)
-
-    def gremlin(self):
-        gl_dist, chain_dist_all = self.rrcreader.gremlin(
-            gl_path=self.tool_fp,
-            file_name=self.prot_name,
-            file_chain=self.file_chain,
-            pair_list=self.pair_list,
-            dist_df=self.dist_df,
-            sort_=self.sort_
-        )
-        return pd.concat([gl_dist, chain_dist_all], axis=1)
-
-    def gdca(self):
-        gdca_dist, chain_dist_all = self.rrcreader.gdca(
-            gdca_path=self.tool_fp,
-            file_name=self.prot_name,
-            file_chain=self.file_chain,
-            pair_list=self.pair_list,
-            dist_df=self.dist_df,
-            sort_=self.sort_
-        )
-        return pd.concat([gdca_dist, chain_dist_all], axis=1)
-
-    def plmc(self):
-        plmc_dist, chain_dist_all = self.rrcreader.plmc(
-            plmc_path=self.tool_fp,
-            file_name=self.prot_name,
-            file_chain=self.file_chain,
-            pair_list=self.pair_list,
-            dist_df=self.dist_df,
-            sort_=self.sort_
-        )
-        return pd.concat([plmc_dist, chain_dist_all], axis=1)
-
-    def memconp(self):
-        memconp_dist, chain_dist_all = self.rrcreader.memconp(
-            mcp_path=self.tool_fp,
-            file_name=self.prot_name,
-            file_chain=self.file_chain,
-            pair_list=self.pair_list,
-            dist_df=self.dist_df,
-            sort_=self.sort_
-        )
-        return pd.concat([memconp_dist, chain_dist_all], axis=1)
-
-    def membrain2(self):
-        membrain2_dist, chain_dist_all = self.rrcreader.membrain2(
-            mb_path=self.tool_fp,
-            file_name=self.prot_name,
-            file_chain=self.file_chain,
-            pair_list=self.pair_list,
-            dist_df=self.dist_df,
-            sort_=self.sort_
-        )
-        return pd.concat([membrain2_dist, chain_dist_all], axis=1)
-
-    def tma165(self):
-        tma165_dist, chain_dist_all = self.rrcreader.tma165(
-            tma165_path=self.tool_fp,
-            file_name=self.prot_name,
-            file_chain=self.file_chain,
-            pair_list=self.pair_list,
-            dist_df=self.dist_df,
-            sort_=self.sort_
-        )
-        return pd.concat([tma165_dist, chain_dist_all], axis=1)
+__author__ = "Jianfeng Sun"
+__version__ = "v1.0"
+__copyright__ = "Copyright 2023"
+__license__ = "GPL v3.0"
+__email__ = "jianfeng.sunmt@gmail.com"
+__maintainer__ = "Jianfeng Sun"
+
+import time
+from tmkit.seqnetrr.window.Pair import Pair
+from tmkit.seqnetrr.window.Single import Single
+from tmkit.seqnetrr.combo.Length import length as plength
+from tmkit.sequence import Fasta as sfasta
+from tmkit.seqnetrr.combo.Position import Position as pfasta
+from tmkit.seqnetrr.graph.Bipartite import Bipartite as bigraph
+from tmkit.seqnetrr.graph.Unipartite import Unipartite as unigraph
+from tmkit.seqnetrr.graph.Cumulative import Cumulative as cumugraph
+from tmkit.util.Reader import Reader as prrcreader
+from tmkit.util.Writer import Writer as pfwriter
+
+
+class Compare:
+
+    def __init__(
+            self,
+            fasta_path,
+            window_size,
+            seq_sep_inferior,
+            pair_mode='patch',
+            mode='hash',
+            input_kind='general',
+            list_fpn=None,
+            fc_path=None,
+            sv_fpn=None,
+            is_sv=False,
+            len_thres=500,
+    ):
+        """
+
+        Parameters
+        ----------
+        fasta_path
+        window_size
+        seq_sep_inferior
+        pair_mode
+        mode
+        input_kind
+        list_fpn
+        fc_path
+        sv_fpn
+        is_sv
+        len_thres
+        """
+        self.sv_fpn = sv_fpn
+        self.pfreader = prrcreader()
+        self.pfwriter = pfwriter()
+        self.is_sv = is_sv
+        self.fc_path = fc_path
+        self.seq_sep_inferior = seq_sep_inferior
+        self.pair_mode = pair_mode
+        self.mode = mode
+        self.len_thres = len_thres
+        self.input_kind = input_kind
+        self.window_size = window_size
+        self.prot_df = self.pfreader.generic(list_fpn)
+        self.prot_df['len_seq'] = -1
+        for i in self.prot_df.index:
+            prot_name = self.prot_df.iloc[i, 0]
+            file_chain = self.chain(self.prot_df.iloc[i, 1])
+            sequence = sfasta.get(
+                fasta_fpn=fasta_path + prot_name + file_chain + '.fasta',
+            )
+            # print(sequence)
+            self.prot_df.loc[i, 'seq'] = sequence
+            self.prot_df.loc[i, 'len_seq'] = len(sequence)
+        self.prot_df = self.prot_df.loc[self.prot_df['len_seq'] < len_thres].reset_index(drop=True)
+        print('Sequence separation inf: {}'.format(self.seq_sep_inferior))
+        print('Length thres: {}'.format(self.len_thres))
+        print('Window size: {}'.format(self.window_size))
+        print('Input kind: {}'.format(self.input_kind))
+        print('\n{}'.format(self.prot_df))
+        print(self.prot_df.shape)
+
+    def chain(self, prot_chain):
+        """
+        Chain name modification.
+
+        Parameters
+        ----------
+        prot_chain
+            chain of a protein in the prefix of a FASTA file name
+
+        Returns
+        -------
+        str
+            chain name
+
+        """
+        return str(prot_chain) + 'l' if str(prot_chain).islower() else str(prot_chain)
+
+    def unipartite(self, mode):
+        print('Mode: {}'.format(mode))
+        for i in self.prot_df.index:
+            stime = time.time()
+            sequence = self.prot_df.loc[i, 'seq']
+            prot_name = self.prot_df.iloc[i, 0]
+            file_chain = self.chain(self.prot_df.iloc[i, 1])
+            print('===>ID.{}'.format(i))
+            print('===>protein: {}'.format(prot_name + file_chain))
+            print('===>protein length: {}'.format(self.prot_df.loc[i, 'len_seq']))
+            # /* scenario of position */
+            pos_list = plength(seq_sep_inferior=self.seq_sep_inferior).to_pair(len(sequence))
+            print('===>pair number: {}'.format(len(pos_list)))
+
+            # /* position */
+            position = pfasta(sequence).pair(pos_list=pos_list)
+
+            # /* window */
+            window_m_ids = Pair(
+                sequence=sequence,
+                position=position,
+                window_size=self.window_size,
+            ).mid()
+
+            p = unigraph(
+                sequence=sequence,
+                window_size=self.window_size,
+                window_m_ids=window_m_ids,
+                input_kind=self.input_kind,
+            )
+            # /* local ec scores */
+            list_2d = position
+            p.assign(
+                fpn=self.fc_path + prot_name + file_chain + '.evfold',
+                list_2d=list_2d,
+                mode=mode,
+            )
+            print('===>total time: {time}s.'.format(time=time.time() - stime))
+            # print(vec)
+            return 'Finished'
+
+    def bipartite(self, pair_mode, mode):
+        print('Pair mode: {}'.format(pair_mode))
+        print('Mode: {}'.format(mode))
+        for i in self.prot_df.index:
+            stime = time.time()
+            sequence = self.prot_df.loc[i, 'seq']
+            prot_name = self.prot_df.iloc[i, 0]
+            file_chain = self.chain(self.prot_df.iloc[i, 1])
+            print('===>ID.{}'.format(i))
+            print('===>protein: {}'.format(prot_name + file_chain))
+            print('===>protein length: {}'.format(self.prot_df.loc[i, 'len_seq']))
+            # /* scenario of position */
+            pos_list = plength(seq_sep_inferior=self.seq_sep_inferior).to_pair(len(sequence))
+            print('===>pair number: {}'.format(len(pos_list)))
+
+            # /* position */
+            position = pfasta(sequence).pair(pos_list=pos_list)
+
+            # /* window */
+            window_m_ids = Pair(
+                sequence=sequence,
+                position=position,
+                window_size=self.window_size,
+            ).mid()
+
+            p = bigraph(
+                sequence=sequence,
+                window_size=self.window_size,
+                window_m_ids=window_m_ids,
+                kind=pair_mode,
+                patch_size=2,
+                input_kind=self.input_kind,
+            )
+            # /* global ec scores */
+            list_2d = position
+            p.assign(
+                fpn=self.fc_path + prot_name + file_chain + '.evfold',
+                list_2d=list_2d,
+                mode=mode,
+            )
+            print('===>total time: {time}s.'.format(time=time.time() - stime))
+            # print(vec)
+            return 'Finished'
+
+    def cumulative(self, cumu_ratio=0.5):
+        print('cumulative ratio: {}'.format(cumu_ratio))
+        for i in self.prot_df.index:
+            stime = time.time()
+            sequence = self.prot_df.loc[i, 'seq']
+            prot_name = self.prot_df.iloc[i, 0]
+            file_chain = self.chain(self.prot_df.iloc[i, 1])
+            print('===>ID.{}'.format(i))
+            print('===>protein: {}'.format(prot_name + file_chain))
+            print('===>protein length: {}'.format(self.prot_df.loc[i, 'len_seq']))
+            # /* scenario of position */
+            pos_list = plength(seq_sep_inferior=self.seq_sep_inferior).tosgl(len(sequence))
+            print('===>pair number: {}'.format(len(pos_list)))
+
+            # /* position */
+            position = pfasta(sequence).single(pos_list=pos_list)
+
+            # /* window */
+            window_m_ids = Single(
+                sequence=sequence,
+                position=position,
+                window_size=self.window_size,
+            ).mid()
+
+            p = cumugraph(
+                sequence=sequence,
+                window_size=self.window_size,
+                window_m_ids=window_m_ids,
+                input_kind=self.input_kind,
+            )
+            # /* global ec scores */
+            list_2d = position
+            p.assign(
+                list_2d=list_2d,
+                fpn=self.fc_path + prot_name + file_chain + '.evfold',
+                L=int(len(sequence) * cumu_ratio),
+                simu_seq_len=None,
+            )
+            print('===>total time: {time}s.'.format(time=time.time() - stime))
+            return 'Finished'
```

### Comparing `tmkit-0.0.2/tmkit/db/construct/Network.py` & `tmkit-0.0.3/tmkit/db/construct/Network.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,111 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-import numpy as np
+from typing import List, Tuple
 
+import numpy as np
+import pandas as pd
 
-class network:
 
-    def single(self, interacting_df, uniprot_id, by=[], is_del_reflexive=False, is_del_repeated=False):
+class Network:
+    def single(
+        self,
+        interacting_df: pd.DataFrame,
+        uniprot_id: str,
+        by: List[str] = [],
+        is_del_reflexive: bool = False,
+        is_del_repeated: bool = False,
+    ) -> np.ndarray:
         """
+        Construct a single network for a given uniprot_id.
 
         Parameters
         ----------
-        interacting_df
-        uniprot_id
-        by
-            respective identifiers of interaction A nad interaction B
-        is_del_reflexive
-            delete those interacting with itself
-        is_del_repeated
-            delete interacting pairs occurring repeatedly
+        interacting_df : np.ndarray
+            The input interaction dataframe.
+        uniprot_id : str
+            The uniprot_id for which to construct the network.
+        by : List[str], optional
+            The respective identifiers of interaction A and interaction B, by default [].
+        is_del_reflexive : bool, optional
+            Whether to delete interactions with itself, by default False.
+        is_del_repeated : bool, optional
+            Whether to delete interacting pairs occurring repeatedly, by default False.
 
         Returns
         -------
-
+        np.ndarray
+            The constructed network.
         """
         interacting_left = interacting_df.groupby(by=[by[0]])
         interacting_right = interacting_df.groupby(by=[by[1]])
         # print(interacting_left.groups.keys())
         if uniprot_id in interacting_left.groups.keys():
             interacting_left_grouped = np.array(interacting_left.get_group(uniprot_id))
             # print(interacting_left_grouped)
-            print('=========>Record(s) for {} found in the left column.'.format(uniprot_id))
+            print(
+                "=========>Record(s) for {} found in the left column.".format(
+                    uniprot_id
+                )
+            )
         else:
-            print('=========>No record(s) for {} found in the left column.'.format(uniprot_id))
+            print(
+                "=========>No record(s) for {} found in the left column.".format(
+                    uniprot_id
+                )
+            )
             interacting_left_grouped = np.empty(shape=[0, 2])
         if uniprot_id in interacting_right.groups.keys():
-            interacting_right_grouped = np.array(interacting_right.get_group(uniprot_id))[:, [1, 0]]  # exchange the order of the two
+            interacting_right_grouped = np.array(
+                interacting_right.get_group(uniprot_id)
+            )[
+                :, [1, 0]
+            ]  # exchange the order of the two
             # print(interacting_right_grouped)
-            print('=========>Record(s) for {} found in the left column.'.format(uniprot_id))
+            print(
+                "=========>Record(s) for {} found in the left column.".format(
+                    uniprot_id
+                )
+            )
         else:
-            print('=========>No record(s) for {} found on the right column.'.format(uniprot_id))
+            print(
+                "=========>No record(s) for {} found on the right column.".format(
+                    uniprot_id
+                )
+            )
             interacting_right_grouped = np.empty(shape=[0, 2])
         if is_del_reflexive:
             A_row_marker = np.where(
                 interacting_left_grouped[:, 0] == interacting_left_grouped[:, 1]
             )
             B_row_marker = np.where(
                 interacting_right_grouped[:, 0] == interacting_right_grouped[:, 1]
             )
             interacting_left_grouped = np.delete(
-                interacting_left_grouped,
-                A_row_marker,
-                axis=0
+                interacting_left_grouped, A_row_marker, axis=0
             )
             interacting_right_grouped = np.delete(
                 interacting_right_grouped,
                 B_row_marker,
                 axis=0,
             )
         single_network = np.concatenate(
-            (interacting_left_grouped, interacting_right_grouped),
-            axis=0
+            (interacting_left_grouped, interacting_right_grouped), axis=0
         )
         if is_del_repeated:
             single_network_B = np.unique(single_network[:, 1])
             single_network = np.concatenate(
-                (np.array([uniprot_id] * single_network_B.shape[0])[:, np.newaxis], single_network_B[:, np.newaxis]),
-                axis=1
+                (
+                    np.array([uniprot_id] * single_network_B.shape[0])[:, np.newaxis],
+                    single_network_B[:, np.newaxis],
+                ),
+                axis=1,
             )
         if len(single_network) > 0:
             return single_network
         else:
-            return np.empty(shape=[0, 2])
+            return np.empty(shape=[0, 2])
```

### Comparing `tmkit-0.0.2/tmkit/id/PDB.py` & `tmkit-0.0.3/tmkit/chain/PDB.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-from tmkit.base import PDB
-from Bio.PDB.Polypeptide import three_to_one
+from typing import List
 
+from tmkit.base import PDB as bpdb
 
-class pdb(PDB.id):
 
-    def __init__(self, pdb_fp, prot_name, seq_chain, file_chain=''):
-        """
+class PDB(bpdb.Chain):
+    """
+    A class representing a Protein Data Bank (PDB) file.
 
-        Parameters
-        ----------
-        pdb_fp
-            structure path
-        prot_name
-            structure name
-        file_chain
-            file chain
-        seq_chain
-            sequence chain
-        """
-        super(pdb, self).__init__(pdb_fp, prot_name, seq_chain, file_chain)
+    Parameters
+    ----------
+    pdb_fp : str
+        The file path to the PDB file.
+    prot_name : str
+        The name of the protein.
+
+    Attributes
+    ----------
+    structure : Bio.PDB.Structure.Structure
+        The structure object of the PDB file.
+    """
 
-    def chain(self):
+    def __init__(self, pdb_fp: str, prot_name: str) -> None:
+        super().__init__(pdb_fp, prot_name)
+
+    def chains(self) -> List[str]:
         """
+        Get a list of chain IDs in the PDB file.
 
         Returns
         -------
-            dict: pdb id -> aa symbol
-
+        List[str]
+            A list of chain IDs.
         """
-        ids = {}
-        for i, residue in enumerate(self.pdb_chain):
-            res_name = three_to_one(residue.get_resname())
-            ids[residue.id[1]] = res_name
-        # print([*ids.keys()])
-        return ids
+        return [chain.get_id() for chain in self.structure.get_chains()]
```

### Comparing `tmkit-0.0.2/tmkit/position/scenario/Segment.py` & `tmkit-0.0.3/tmkit/base/Position.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,57 @@
-__author__ = "Jianfeng Sun"
-__version__ = "v1.0"
-__copyright__ = "Copyright 2023"
-__license__ = "GPL v3.0"
-__email__ = "jianfeng.sunmt@gmail.com"
-__maintainer__ = "Jianfeng Sun"
-
-import pandas as pd
-from tmkit.base.Position import position
-from tmkit.position.scenario.Separation import separation
-
-
-class segment(position):
-
-    def __init__(self, seq_sep_inferior=None, seq_sep_superior=None):
-        super(segment, self).__init__(seq_sep_inferior, seq_sep_superior)
-
-    def toPair(self, fas_lower, fas_upper):
-        """
-        ..  summary:
-            --------
-            get fasta ids of residue pairs of a protein regulated
-            by seq_sep_inferior and (or) seq_sep_superior
-
-        :param fas_lower: fasta 1d list
-        :param fas_upper: fasta 1d list
-        :return:
-        """
-        if fas_lower == [] and fas_upper == []:
-            return []
-        else:
-            df_ = pd.DataFrame(self.interv2combi(fas_lower, fas_upper))
-            pairs = separation(
-                df=df_,
-                first=0,
-                second=1,
-                is_sort=False,
-                seq_sep_inferior=self.seq_sep_inferior,
-                seq_sep_superior=self.seq_sep_superior
-            ).extract().values.tolist()
-            return pairs
-
-    def toSingle(self, fas_lower, fas_upper):
-        """
-        ..  summary:
-            --------
-            get fasta ids of residue pairs of a protein regulated
-            by seq_sep_inferior and (or) seq_sep_superior
-
-        :param fas_lower: fasta 1d list
-        :param fas_upper: fasta 1d list
-        :return:
-        """
-        return self.asp.interv2single(fas_lower, fas_upper)
-
+__author__ = "Jianfeng Sun"
+__version__ = "v1.0"
+__copyright__ = "Copyright 2023"
+__license__ = "GPL v3.0"
+__email__ = "jianfeng.sunmt@gmail.com"
+__maintainer__ = "Jianfeng Sun"
+
+from typing import List, Tuple, Union
+
+import numpy as np
+
+
+class Position:
+    def __init__(
+        self, seq_sep_inferior: Union[int, float] = None, seq_sep_superior: Union[int, float] = None
+    ) -> None:
+        """
+        Parameters
+        ----------
+        seq_sep_inferior : int or None, optional
+            The inferior sequence separation, by default None.
+        seq_sep_superior : int or None, optional
+            The superior sequence separation, by default None.
+        """
+        self.seq_sep_inferior = seq_sep_inferior
+        self.seq_sep_superior = seq_sep_superior
+
+    def interv2combi(
+        self, inf_arr: List[int], sup_arr: List[int]
+    ) -> List[Tuple[int, int]]:
+        """
+        Convert two arrays of inferior and superior sequence separations into a list of tuples representing all possible combinations.
+
+        Parameters
+        ----------
+        inf_arr : List[int]
+            The array of inferior sequence separations.
+        sup_arr : List[int]
+            The array of superior sequence separations.
+
+        Returns
+        -------
+        List[Tuple[int, int]]
+            A list of tuples representing all possible combinations.
+        """
+        tmp_2d = []
+        num_interv = len(inf_arr)
+        for i in range(num_interv):
+            tmp_2d.append(list(np.arange(inf_arr[i], sup_arr[i] + 1)))
+        combi = []
+        for i in range(num_interv):
+            for j in range(num_interv):
+                if i < j:
+                    for p in range(len(tmp_2d[i])):
+                        for q in range(len(tmp_2d[j])):
+                            combi.append((tmp_2d[i][p], tmp_2d[j][q]))
+        return combi
```

### Comparing `tmkit-0.0.2/tmkit/retrieve/PDB.py` & `tmkit-0.0.3/tmkit/retrieve/PDB.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,138 +1,150 @@
-__author__ = "Jianfeng Sun"
-__version__ = "v1.0"
-__copyright__ = "Copyright 2023"
-__license__ = "GPL v3.0"
-__email__ = "jianfeng.sunmt@gmail.com"
-__maintainer__ = "Jianfeng Sun"
-
-from Bio.PDB import PDBList
-from tmkit.util.Kit import ungz
-from tmkit.util.Kit import urlliby
-from tmkit.util.Kit import delete
-from tmkit.util.Kit import batchRename
-
-
-class pdb:
-
-    def __init__(
-            self,
-            prot_series,
-    ):
-        self.prot_dedup = prot_series.unique()
-
-    def rcsb(self, sv_fp, route='biopython'):
-        """
-
-        Notes
-        -----
-            Downloading a PDB file from RCSB PDB.
-
-            file_format is specified with 'structure' to download a file
-            with suffix of 'ent', which is totally the same with original
-            format of file with suffix of 'structure', 'pdb'.
-
-        See Also
-        --------
-            https://biopython.org/DIST/docs/api/Bio.PDB.PDBList%27-pysrc.html
-
-        Parameters
-        ----------
-        sv_fp
-            path to save files
-        route
-            'biopython' or 'external'
-
-        Returns
-        -------
-
-        """
-        pdb_list = PDBList()
-        if route == 'biopython':
-            for i, prot_name in enumerate(self.prot_dedup):
-                print('===>No.{} protein name: {}'.format(i + 1, prot_name))
-                pdb_list.retrieve_pdb_file(
-                    pdb_code=str(prot_name),
-                    file_format='pdb',
-                    pdir=sv_fp,
-                )
-                print("======>successfully downloaded!")
-            batchRename(
-                file_path=sv_fp,
-                old_suffix='ent',
-                new_suffix='pdb',
-                flag=0,
-            )
-        else:
-            for i, prot_name in enumerate(self.prot_dedup):
-                print('===>No.{} protein name: {}'.format(i + 1, prot_name))
-                url = 'https://files.rcsb.org/download/' + prot_name + '.pdb'
-                urlliby(
-                    url=url,
-                    fpn=sv_fp + str(prot_name) + '.pdb',
-                )
-        return 0
-
-    def pdbtm(self, sv_fp, kind='tr'):
-        """
-
-        Notes
-        -----
-            Downloading a PDB file from PDBTM.
-
-        Parameters
-        ----------
-        sv_fp
-            path to save files
-        kind
-            'tr' for 'transformed proteins'
-            '' for 'rcsb'
-
-        Returns
-        -------
-
-        """
-        count = 0
-        for i, prot_name in enumerate(self.prot_dedup):
-            mark = str(prot_name[1] + prot_name[2])
-            url = 'http://pdbtm.enzim.hu/data/database/' + mark + '/' + str(prot_name) + '.' + kind + 'pdb.gz'
-            print('===>No.{} protein name: {}'.format(i + 1, prot_name))
-            try:
-                urlliby(
-                    url=url,
-                    fpn=sv_fp + str(prot_name) + '.gz'
-                )
-                ungz(
-                    file_path=sv_fp,
-                    file_name=prot_name,
-                    sv_fp=sv_fp,
-                    new_suffix='.pdb'
-                )
-                delete(sv_fp + str(prot_name) + '.gz')
-                print("======>successfully downloaded!")
-            except:
-                count = count + 1
-                # print(count)
-                continue
-        return 0
-
-    def alphafold(self, sv_fp: str) -> None:
-        """
-        Download a PDB file of a protein from the AlphaFold database.
-
-        Args:
-            sv_fp (str): The path to save the downloaded PDB file.
-
-        Examples:
-            >>> alphafold("Q5VSL9", "Q5VSL9.pdb")
-        """
-        import requests
-        for i, uniprot_acc in enumerate(self.prot_dedup):
-            print("===>No.{} protein name: {}".format(i + 1, uniprot_acc))
-            url = f"https://alphafold.ebi.ac.uk/files/AF-{uniprot_acc}-F1-model_v4.pdb"
-            result = requests.get(url, allow_redirects=True)
-            if result.status_code == 200:
-                with open(sv_fp + uniprot_acc + '.pdb', 'wb') as f:
-                    f.write(result.content)
-                print("======>successfully downloaded!")
-            else:
-                print(f"Failed to download. HTTP status code: {result.status_code}")
+__author__ = "Jianfeng Sun"
+__version__ = "v1.0"
+__copyright__ = "Copyright 2023"
+__license__ = "GPL v3.0"
+__email__ = "jianfeng.sunmt@gmail.com"
+__maintainer__ = "Jianfeng Sun"
+
+import pandas as pd
+
+from Bio.PDB import PDBList
+
+from tmkit.util.Kit import batchRename, delete, ungz, urlliby
+
+
+class PDB:
+    def __init__(
+        self,
+        prot_series: pd.Series,
+    ) -> None:
+        """
+        Parameters
+        ----------
+        prot_series : pd.Series
+            A Pandas series of protein names.
+        """
+        self.prot_dedup = prot_series.unique()
+
+    def rcsb(self, sv_fp: str, route: str = "biopython") -> str:
+        """
+        Downloading a PDB file from RCSB PDB.
+
+        file_format is specified with 'structure' to download a file
+        with suffix of 'ent', which is totally the same with original
+        format of file with suffix of 'structure', 'pdb'.
+
+        See Also
+        --------
+        https://biopython.org/DIST/docs/api/Bio.PDB.PDBList%27-pysrc.html
+
+        Parameters
+        ----------
+        sv_fp : str
+            Path to save files.
+        route : str, optional
+            'biopython' or 'external', by default 'biopython'
+
+        Returns
+        -------
+        str
+            'Finished' if a PDB file is downloaded
+        """
+        pdb_list = PDBList()
+        if route == "biopython":
+            for i, prot_name in enumerate(self.prot_dedup):
+                print(f"===>No.{i + 1} protein name: {prot_name}")
+                pdb_list.retrieve_pdb_file(
+                    pdb_code=str(prot_name),
+                    file_format="pdb",
+                    pdir=sv_fp,
+                )
+            batchRename(
+                file_path=sv_fp,
+                old_suffix="ent",
+                new_suffix="pdb",
+                flag=0,
+            )
+        else:
+            for i, prot_name in enumerate(self.prot_dedup):
+                print(f"===>No.{i + 1} protein name: {prot_name}")
+                url = "https://files.rcsb.org/download/" + prot_name + ".pdb"
+                urlliby(
+                    url=url,
+                    fpn=sv_fp + str(prot_name) + ".pdb",
+                )
+        return 'Finished'
+
+    def pdbtm(self, sv_fp: str, kind: str = "tr") -> str:
+        """
+        Download PDB files from PDBTM.
+
+        Parameters
+        ----------
+        sv_fp : str
+            Path to save files.
+        kind : str, optional
+            'tr' for 'transformed proteins', '' for 'rcsb', by default 'tr'
+
+        Notes
+        -----
+        Downloading a PDB file from PDBTM.
+
+        Returns
+        -------
+        str
+            'Finished' if a PDB file is successfully retrieved.
+        """
+        count = 0
+        for i, prot_name in enumerate(self.prot_dedup):
+            mark = str(prot_name[1] + prot_name[2])
+            url = (
+                "http://pdbtm.enzim.hu/data/database/"
+                + mark
+                + "/"
+                + str(prot_name)
+                + "."
+                + kind
+                + "pdb.gz"
+            )
+            print(f"===>No.{i + 1} protein name: {prot_name}")
+            try:
+                urlliby(url=url, fpn=sv_fp + str(prot_name) + ".gz")
+                ungz(
+                    file_path=sv_fp, file_name=prot_name, sv_fp=sv_fp, new_suffix=".pdb"
+                )
+                delete(sv_fp + str(prot_name) + ".gz")
+            except:
+                count = count + 1
+                # print(count)
+                continue
+        return 'Finished'
+
+    def alphafold(self, sv_fp: str) -> str:
+        """
+        Download a PDB file of a protein from the AlphaFold database.
+
+        Parameters
+        ----------
+        sv_fp : str
+            The path to save the downloaded PDB file.
+
+        Examples
+        --------
+        >>> alphafold("Q5VSL9", "Q5VSL9.pdb")
+
+        Returns
+        -------
+        str
+            'Finished' if a PDB file is successfully retrieved.
+        """
+        import requests
+
+        for i, uniprot_acc in enumerate(self.prot_dedup):
+            url = f"https://alphafold.ebi.ac.uk/files/AF-{uniprot_acc}-F1-model_v4.pdb"
+            result = requests.get(url, allow_redirects=True)
+            if result.status_code == 200:
+                with open(sv_fp + uniprot_acc + ".pdb", "wb") as f:
+                    f.write(result.content)
+            else:
+                print(f"Failed to download. HTTP status code: {result.status_code}")
+        return 'Finished'
```

### Comparing `tmkit-0.0.2/tmkit/seqnetrr/ComputLib.py` & `tmkit-0.0.3/tmkit/seqnetrr/ComputLib.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,165 +1,164 @@
-__author__ = "Jianfeng Sun"
-__version__ = "v1.0"
-__copyright__ = "Copyright 2023"
-__license__ = "GPL v3.0"
-__email__ = "jianfeng.sunmt@gmail.com"
-__maintainer__ = "Jianfeng Sun"
-
-
-class computLib:
-
-    def interv2single(self, inf_arr, sup_arr):
-        """
-
-        Methods
-        -------
-                        1   2   3
-            inf_arr = [15, 48, 78]
-            sup_arr = [30, 53, 99]
-            element in interval No.1 matches elements in No.2,
-            No.3 one by one. and then, element in interval No.2
-            matches elements in interval No.3 until finished.
-
-        Parameters
-        ----------
-        inf_arr
-            1d list
-        sup_arr
-            1d list
-
-        Returns
-        -------
-
-        """
-        single = []
-        num_interv = len(inf_arr)
-        for i in range(num_interv):
-            segment = self.num2arr2d(inf_arr[i], sup_arr[i])
-            for j in segment:
-                single.append(j)
-        return single
-
-    def num2arr(self, length):
-        """
-
-        Notes
-        -----
-            generate a 2x2 array by given an number from 1.
-
-        Parameters
-        ----------
-        length
-
-        Returns
-        -------
-
-        """
-        arr = []
-        for i in range(length):
-            for j in range(length):
-                if i < j:
-                    arr.append([i + 1, j + 1])
-        return arr
-
-    def numTo3cols(self, length):
-        """
-
-        Notes
-        -----
-            generate a 2x2 array by given an number from 1.
-
-        Parameters
-        ----------
-        length
-
-        Returns
-        -------
-
-        """
-        arr = []
-        for i in range(length):
-            for j in range(length):
-                if i < j:
-                    arr.append([i+1, j+1, 1])
-        return arr
-
-    def tactic1(self, arr_2d):
-        """
-
-        Parameters
-        ----------
-        arr_2d
-
-        Returns
-        -------
-
-        """
-        result = {}
-        len_arr = len(arr_2d[0])
-        if len_arr == 3:
-            for item in arr_2d:
-                result.setdefault(item[0], {}).update({item[1]: item[2]})
-        else:
-            for item in arr_2d:
-                result.setdefault(item[0], {}).update({item[1]: item[2:]})
-        return result
-
-    def num2triangular(self, length):
-        """
-
-        Notes
-        -----
-            generate a 2x2 array by given an number from 1.
-
-        Parameters
-        ----------
-        length
-
-        Returns
-        -------
-
-        """
-        arr = []
-        for i in range(length):
-            for j in range(i, length):
-                arr.append([i + 1, j + 1])
-        return arr
-
-    def num2arr2d(self, inf, sup):
-        """
-
-        Notes
-        -----
-            generate a 1d array by given an inf and sup.
-
-        Parameters
-        ----------
-        inf
-        sup
-
-        Returns
-        -------
-
-        """
-        arr = []
-        for i in range(inf, sup + 1):
-            arr.append([i])
-        return arr
-
-    def patch(self, length, step=1):
-        """
-
-        Parameters
-        ----------
-        length
-        step
-
-        Returns
-        -------
-
-        """
-        arr = []
-        for i in range(-length, length + 1, step):
-            for j in range(-length, length + 1, step):
-                arr.append([i, j])
-        return arr
+__author__ = "Jianfeng Sun"
+__version__ = "v1.0"
+__copyright__ = "Copyright 2023"
+__license__ = "GPL v3.0"
+__email__ = "jianfeng.sunmt@gmail.com"
+__maintainer__ = "Jianfeng Sun"
+
+
+class ComputLib:
+    def interv2single(self, inf_arr, sup_arr):
+        """
+
+        Methods
+        -------
+                        1   2   3
+            inf_arr = [15, 48, 78]
+            sup_arr = [30, 53, 99]
+            element in interval No.1 matches elements in No.2,
+            No.3 one by one. and then, element in interval No.2
+            matches elements in interval No.3 until finished.
+
+        Parameters
+        ----------
+        inf_arr
+            1d list
+        sup_arr
+            1d list
+
+        Returns
+        -------
+
+        """
+        single = []
+        num_interv = len(inf_arr)
+        for i in range(num_interv):
+            segment = self.num2arr2d(inf_arr[i], sup_arr[i])
+            for j in segment:
+                single.append(j)
+        return single
+
+    def num2arr(self, length):
+        """
+
+        Notes
+        -----
+            generate a 2x2 array by given an number from 1.
+
+        Parameters
+        ----------
+        length
+
+        Returns
+        -------
+
+        """
+        arr = []
+        for i in range(length):
+            for j in range(length):
+                if i < j:
+                    arr.append([i + 1, j + 1])
+        return arr
+
+    def numTo3cols(self, length):
+        """
+
+        Notes
+        -----
+            generate a 2x2 array by given an number from 1.
+
+        Parameters
+        ----------
+        length
+
+        Returns
+        -------
+
+        """
+        arr = []
+        for i in range(length):
+            for j in range(length):
+                if i < j:
+                    arr.append([i + 1, j + 1, 1])
+        return arr
+
+    def tactic1(self, arr_2d):
+        """
+
+        Parameters
+        ----------
+        arr_2d
+
+        Returns
+        -------
+
+        """
+        result = {}
+        len_arr = len(arr_2d[0])
+        if len_arr == 3:
+            for item in arr_2d:
+                result.setdefault(item[0], {}).update({item[1]: item[2]})
+        else:
+            for item in arr_2d:
+                result.setdefault(item[0], {}).update({item[1]: item[2:]})
+        return result
+
+    def num2triangular(self, length):
+        """
+
+        Notes
+        -----
+            generate a 2x2 array by given an number from 1.
+
+        Parameters
+        ----------
+        length
+
+        Returns
+        -------
+
+        """
+        arr = []
+        for i in range(length):
+            for j in range(i, length):
+                arr.append([i + 1, j + 1])
+        return arr
+
+    def num2arr2d(self, inf, sup):
+        """
+
+        Notes
+        -----
+            generate a 1d array by given an inf and sup.
+
+        Parameters
+        ----------
+        inf
+        sup
+
+        Returns
+        -------
+
+        """
+        arr = []
+        for i in range(inf, sup + 1):
+            arr.append([i])
+        return arr
+
+    def patch(self, length, step=1):
+        """
+
+        Parameters
+        ----------
+        length
+        step
+
+        Returns
+        -------
+
+        """
+        arr = []
+        for i in range(-length, length + 1, step):
+            for j in range(-length, length + 1, step):
+                arr.append([i, j])
+        return arr
```

### Comparing `tmkit-0.0.2/tmkit/seqnetrr/combo/Length.py` & `tmkit-0.0.3/tmkit/structure/rrc/Label.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,90 @@
-__author__ = "Jianfeng Sun"
-__version__ = "v1.0"
-__copyright__ = "Copyright 2023"
-__license__ = "GPL v3.0"
-__email__ = "jianfeng.sunmt@gmail.com"
-__maintainer__ = "Jianfeng Sun"
-
-import pandas as pd
-from tmkit.seqnetrr.combo.Param import param
-from tmkit.seqnetrr.combo.Separation import separation
-
-
-class length(param):
-
-    def __init__(self, seq_sep_inferior=None, seq_sep_superior=None):
-        super(length, self).__init__(seq_sep_inferior, seq_sep_superior)
-
-    def topair(self, length, kind='standard'):
-        """
-        Notes
-        -----
-            Given length of a protein sequence, it gets fasta
-            ids of residue pairs of a protein regulated by
-            seq_sep_inferior and (or) seq_sep_superior.
-
-        Parameters
-        ----------
-        length
-            the length of a molecular sequence
-
-        Returns
-        -------
-        2d array
-
-        """
-        df_ = pd.DataFrame(self.computlib.num2arr(length))
-        if kind == 'standard':
-            return separation(
-                df=df_,
-                first=0,
-                second=1,
-                is_sort=False,
-                seq_sep_inferior=self.seq_sep_inferior,
-                seq_sep_superior=self.seq_sep_superior
-            ).extract().values.tolist()
-        elif kind == 'triangular':
-            return self.computlib.num2triangular(length)
-        elif kind == 'under_triangular':
-            return self.computlib.num2arr(length)
-
-    def tosgl(self, length):
-        """
-        Notes
-        -----
-            Given length of a protein sequence, it gets fasta
-            ids of residue pairs of a protein regulated by
-            seq_sep_inferior and (or) seq_sep_superior.
-
-        Parameters
-        ----------
-        length
-            the length of a molecular sequence
-
-        Returns
-        -------
-            2d array
-
-        """
-        return self.computlib.num2arr2d(1, length)
+__author__ = "Jianfeng Sun"
+__version__ = "v1.0"
+__copyright__ = "Copyright 2023"
+__license__ = "GPL v3.0"
+__email__ = "jianfeng.sunmt@gmail.com"
+__maintainer__ = "Jianfeng Sun"
+
+import numpy as np
+import pandas as pd
+
+from tmkit.position.scenario.Separation import Separation
+from tmkit.util.Reader import Reader
+
+
+class Label:
+    def __init__(
+        self,
+        dist_path,
+        prot_name,
+        file_chain,
+        cutoff=5.5,
+        seq_sep_inferior=None,
+        seq_sep_superior=None,
+    ):
+        """
+        Parameters
+        ----------
+        dist_path
+            path where a file containing real distances between residues is placed
+            (please check the file at ./data/rrc in the example dataset).
+        prot_name
+            Name of a protein in the prefix of a PDB file name (e.g., 1xqf in 1xqfA.pdb).
+        file_chain
+            Chain of a protein in the prefix of a PDB file name (e.g., A in 1xqfA.pdb).
+             Parameter file_chain will be converted within the function.
+        cutoff
+            distance cutoff to see whether two residues are in spatial contact (e.g., 5.5 angstrom).
+        seq_sep_inferior
+            The lower bounds of how far any two residues are in pairs.
+        seq_sep_superior
+            The upper bounds of how far any two residues are in pairs.
+        """
+        self.prot_name = prot_name
+        self.file_chain = file_chain
+        self.dist_fpn = dist_path + self.prot_name + self.file_chain + ".dist"
+        self.cutoff = cutoff
+        self.seq_sep_inferior = seq_sep_inferior
+        self.seq_sep_superior = seq_sep_superior
+
+    def attach(self) -> pd.DataFrame:
+        """
+        Attach distance between residues.
+
+        Returns
+        -------
+        pd.DataFrame
+            A Pandas DataFrame.
+
+        """
+        dist_df = Reader().generic(self.dist_fpn)
+        dist_np = np.array(dist_df)
+        row = dist_np.shape[0]
+        new_col = np.array([np.ones(row) * -1])
+        dist_np = np.column_stack((dist_np, new_col.T))
+        for i in range(row):
+            if dist_np[i][6] < self.cutoff:
+                dist_np[i][7] = 1
+            else:
+                dist_np[i][7] = 0
+        dist_df = pd.DataFrame(dist_np)
+        dist_df.columns = [
+            "fasta_id_1",
+            "aa_1",
+            "pdb_id_1",
+            "fasta_id_2",
+            "aa_2",
+            "pdb_id_2",
+            "dist",
+            "is_contact",
+        ]
+        dist_df = Separation(
+            df=dist_df,
+            first="fasta_id_1",
+            second="fasta_id_2",
+            target=None,
+            seq_sep_inferior=self.seq_sep_inferior,
+            seq_sep_superior=self.seq_sep_superior,
+            is_sort=False,
+        ).extract()
+        return dist_df.reset_index(inplace=False, drop=True)
```

### Comparing `tmkit-0.0.2/tmkit/seqnetrr/graph/Bipartite.py` & `tmkit-0.0.3/tmkit/seqnetrr/graph/Bipartite.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,353 +1,438 @@
-__author__ = "Jianfeng Sun"
-__version__ = "v1.0"
-__copyright__ = "Copyright 2023"
-__license__ = "GPL v3.0"
-__email__ = "jianfeng.sunmt@gmail.com"
-__maintainer__ = "Jianfeng Sun"
-
-import time
-import numpy as np
-from tmkit.seqnetrr.window.base import Pair as ecabPair
-from tmkit.seqnetrr.net.Reader import reader as prrcreader
-
-
-class bipartite(ecabPair.pair):
-    """
-    Methods
-    -------
-        pairids(), assign()
-
-    Notes
-    -----
-        bipartite class offers methods to assign ECA to global pairs.
-
-    """
-
-    def __init__(
-            self,
-            sequence,
-            window_size,
-            window_m_ids,
-            kind='memconp',
-            patch_size=None,
-            input_kind='general',
-    ):
-        """
-
-        Parameters
-        ----------
-        sequence
-        window_size
-        window_m_ids
-        kind
-        patch_size
-        """
-        super(bipartite, self).__init__(sequence, window_size, window_m_ids)
-        self.prrcreader = prrcreader(
-            seq_sep_inferior=None,
-            seq_sep_superior=None
-        )
-        if kind == 'memconp':
-            self.bigraph = [
-                # self.num_to_dos types in MemConP
-                [4, -4], [4, 4], [3, -4], [-4, 3], [3, 4],
-                [4, 3], [0, -4], [0, 4], [0, -3], [0, 3],
-                [-1, 0], [1, 0], [0, 0], [0, -1], [0, 1],
-                [3, 0], [-3, 0], [4, 0], [-4, 0], [-3, -4],
-                [-4, -3], [-3, 4], [4, -3], [-4, -4], [-4, 4],
-            ]
-        if kind == 'patch':
-            self.bigraph = self.computlib.patch(length=patch_size)
-            # print(self.bigraph)
-        if kind == 'cross':
-            self.bigraph = [
-                [-1, 0], [1, 0], [0, 0], [0, 1], [0, -1],
-            ]
-        if kind == 'unchanged':
-            self.bigraph = [
-                [0, 0],
-            ]
-        self.num_to_dos = len(self.bigraph)
-        self.num_to_dos_in_window = self.num_to_dos * self.aa_in_window_size
-        self.input_kind = input_kind
-        if self.input_kind == 'general':
-            self.file_initiator = self.prrcreader.general
-        elif self.input_kind == 'freecontact':
-            self.file_initiator = self.prrcreader.freecontact
-        elif self.input_kind == 'mutual information':
-            self.file_initiator = self.prrcreader.mi
-        elif self.input_kind == 'gdca':
-            self.file_initiator = self.prrcreader.gdca
-        elif self.input_kind == 'ccmpred':
-            self.file_initiator = self.prrcreader.ccmpred
-        elif self.input_kind == 'plmc':
-            self.file_initiator = self.prrcreader.plmc
-        elif self.input_kind == 'simulate':
-            self.file_initiator = self.prrcreader.simulate
-        else:
-            self.file_initiator = self.prrcreader.general
-
-    def pairids(self):
-        """
-        Notes
-        -----
-            pairids() constitutes all global pairs.
-
-        Methods
-        -------
-            1>. pairids
-                1st dimension: all pairs number
-                2nd dimension: (2 * window_size + 1) * length of bigraph list
-                3rd dimension: 2 (a pair)
-            1>. block 1:    traversing all pairs to be processed.
-                |--->block 1.1: traversing all amino acids in a window.
-                    |--->block 1.1.1:
-                        assigning None to those amino acids whose index
-                        beyond sequence length.
-                    |--->block 1.1.2:
-                        assigning calc results to rest of amino acids.
-                            |--->block 1.1.2.1:
-                                assigning None to those indices (original
-                                amino acid index minus number in bigraph
-                                list) beyond sequence length.
-                            |--->block 1.1.2.2:
-                                assigning results to array global_pair_ids.
-            block 2: assign ECA from ccmpred file
-                |--->block 2.1: read ccmpred file
-                |--->block 2.2: assign ECA from ccmpred file
-            block 3: assign ECA from plmc file
-                |--->block 3.1: read plmc file
-                |--->block 3.2: assign ECA from plmc file
-            block 4: assign ECA from gdca file
-                |--->block 4.1: read gdca file
-                |--->block 4.2: assign ECA from gdca file
-
-        Returns
-        -------
-        3d array,list
-
-        """
-        start_time = time.time()
-        n = len(self.sequence)
-        num_pending = len(self.bigraph)
-        num_aa_in_window = len(self.window_m_ids[0][0])
-        global_pair_ids = [[] for _ in range(self.num_pairs)]
-        # #/*** block 1 ***/
-        for i in range(self.num_pairs):
-            # #/*** block 1.1 ***/
-            for j in range(num_aa_in_window):
-                # #/*** block 1.1.1 ***/
-                if self.window_m_ids[i][0][j] is None or self.window_m_ids[i][1][j] is None:
-                    for k in range(num_pending):
-                        global_pair_ids[i].append([None, None])
-                # #/*** block 1.1.2 ***/
-                else:
-                    for k in range(num_pending):
-                        # #/*** block 1.1.2.1 ***/
-                        left = self.window_m_ids[i][0][j] - self.bigraph[k][0]
-                        right = self.window_m_ids[i][1][j] - self.bigraph[k][1]
-                        left_inf = left < 1
-                        left_sup = left > n
-                        right_inf = right < 1
-                        right_sup = right > n
-                        reflexive = left == right
-                        if left_inf or left_sup or right_inf or right_sup or reflexive:
-                            global_pair_ids[i].append([None, None])
-                        # #/*** block 1.1.2.2 ***/
-                        else:
-                            if left < right:
-                                global_pair_ids[i].append([left, right])
-                            else:
-                                global_pair_ids[i].append([right, left])
-        end_time = time.time()
-        print('======>bipartite pair generation: {time}s.'.format(time=end_time - start_time))
-        # print(global_pair_ids)
-        # print(len(global_pair_ids))
-        # print(len(global_pair_ids[0]))
-        # print(global_pair_ids[0])
-        # print(len(global_pair_ids[0][0]))
-        # print(global_pair_ids[0][0])
-        return global_pair_ids
-
-    def assign(self, list_2d, fpn=None, simu_seq_len=100, mode='hash'):
-        start_time = time.time()
-        list_2d_ = list_2d
-        if mode == 'hash_rl':
-            global_pair_ids = self.pairids()
-            pairs_left = []
-            pairs_right = []
-            for i in range(self.num_pairs):
-                for j in range(self.num_to_dos * (2 * self.window_size + 1)):
-                    pairs_left.append(global_pair_ids[i][j][0])
-                    pairs_right.append(global_pair_ids[i][j][1])
-            # print('Left pairs {}: {}'.format(len(pairs_right), len(pairs_left)))
-            # print('Right pairs {}: {}'.format(len(pairs_left), len(pairs_right)))
-            mark = len(pairs_left)
-            # #/*** block 1 ***/
-            # #/*** block 1.1 ***/
-            evfold_dict = self.file_initiator(
-                fpn=simu_seq_len if self.input_kind == 'simulate' else fpn,
-                sort_=5,
-            )
-            # print(evfold_dict)
-            # #/*** block 1.2 ***/
-            FCj = 0
-            for i in range(mark):
-                if i % (self.num_to_dos * (2 * self.window_size + 1)) == 0:
-                    FCj += 1
-                if pairs_left[i] is None or pairs_right[i] is None:
-                    list_2d_[FCj - 1].append(0)
-                else:
-                    inf = pairs_left[i]
-                    sup = pairs_right[i]
-                    # print([inf, sup])
-                    list_2d_[FCj - 1].append(evfold_dict[inf][sup])
-        elif mode == 'hash_ori':
-            evfold_dict = self.file_initiator(
-                fpn=simu_seq_len if self.input_kind == 'simulate' else fpn,
-                sort_=5,
-            )
-            global_pair_ids = self.pairids()
-            # #/*** block 1 ***/
-            for i in range(self.num_pairs):
-                # #/*** block 1.1 ***/
-                for j in range(self.num_to_dos_in_window):
-                    inf = global_pair_ids[i][j][0]
-                    sup = global_pair_ids[i][j][1]
-                    if inf is None or sup is None:
-                        list_2d_[i].append(0)
-                    else:
-                        list_2d_[i].append(evfold_dict[inf][sup])
-        elif mode == 'hash':
-            n = len(self.sequence)
-            num_pending = len(self.bigraph)
-            num_aa_in_window = len(self.window_m_ids[0][0])
-            evfold_dict = self.file_initiator(
-                fpn=simu_seq_len if self.input_kind == 'simulate' else fpn,
-                sort_=5,
-            )
-            # #/*** block 1 ***/
-            for i in range(self.num_pairs):
-                # #/*** block 1.1 ***/
-                for j in range(num_aa_in_window):
-                    # #/*** block 1.1.1 ***/
-                    if self.window_m_ids[i][0][j] is None or self.window_m_ids[i][1][j] is None:
-                        for k in range(num_pending):
-                            # global_pair_ids[i].append([None, None])
-                            list_2d_[i].append(0)
-                    # #/*** block 1.1.2 ***/
-                    else:
-                        for k in range(num_pending):
-                            # #/*** block 1.1.2.1 ***/
-                            left = self.window_m_ids[i][0][j] - self.bigraph[k][0]
-                            right = self.window_m_ids[i][1][j] - self.bigraph[k][1]
-                            left_inf = left < 1
-                            left_sup = left > n
-                            right_inf = right < 1
-                            right_sup = right > n
-                            reflexive = left == right
-                            if left_inf or left_sup or right_inf or right_sup or reflexive:
-                                # global_pair_ids[i].append([None, None])
-                                list_2d_[i].append(0)
-                            # #/*** block 1.1.2.2 ***/
-                            else:
-                                if left < right:
-                                    list_2d_[i].append(evfold_dict[left][right])
-                                else:
-                                    list_2d_[i].append(evfold_dict[right][left])
-        elif mode == 'pandas':
-            n = len(self.sequence)
-            num_pending = len(self.bigraph)
-            num_aa_in_window = len(self.window_m_ids[0][0])
-            evfold_df = self.file_initiator(
-                fpn=simu_seq_len if self.input_kind == 'simulate' else fpn,
-                is_sort=True,
-                sort_=3,
-            )
-            evfold_df = evfold_df.set_index(['id_1', 'id_2'])
-            # print(evfold_df)
-            # evfold_df_gp = evfold_df.groupby(by=['id_1', 'id_2'])
-            # evfold_df_gp_keys = evfold_df_gp.groups.keys()
-            # print(evfold_df_gp_keys)
-            # #/*** block 1 ***/
-            for i in range(self.num_pairs):
-                # #/*** block 1.1 ***/
-                for j in range(num_aa_in_window):
-                    # #/*** block 1.1.1 ***/
-                    if self.window_m_ids[i][0][j] is None or self.window_m_ids[i][1][j] is None:
-                        for k in range(num_pending):
-                            # global_pair_ids[i].append([None, None])
-                            list_2d_[i].append(0)
-                    # #/*** block 1.1.2 ***/
-                    else:
-                        for k in range(num_pending):
-                            # #/*** block 1.1.2.1 ***/
-                            left = self.window_m_ids[i][0][j] - self.bigraph[k][0]
-                            right = self.window_m_ids[i][1][j] - self.bigraph[k][1]
-                            left_inf = left < 1
-                            left_sup = left > n
-                            right_inf = right < 1
-                            right_sup = right > n
-                            reflexive = left == right
-                            if left_inf or left_sup or right_inf or right_sup or reflexive:
-                                # global_pair_ids[i].append([None, None])
-                                list_2d_[i].append(0)
-                            # #/*** block 1.1.2.2 ***/
-                            else:
-                                if left < right:
-                                    # print(evfold_df.at[(left, right), 'score'])
-                                    list_2d_[i].append(evfold_df.at[(left, right), 'score'])
-                                    # list_2d_[i].append(evfold_df.loc[(evfold_df['id_1'] == left) & (evfold_df['id_2'] == right)])
-                                    # list_2d_[i].append(evfold_df.ix[(left, right), 'score'])
-                                    # list_2d_[i].append(evfold_df_gp.get_group((left, right))['score'].values[0])
-                                else:
-                                    # print(evfold_df.at[(right, left), 'score'])
-                                    list_2d_[i].append(evfold_df.at[(right, left), 'score'])
-                                    # list_2d_[i].append(evfold_df.loc[(evfold_df['id_1'] == right) & (evfold_df['id_2'] == left)])
-                                    # list_2d_[i].append(evfold_np[2][(evfold_np[0] == right) & (evfold_np[1] == left)])
-                                    # list_2d_[i].append(evfold_df.ix[(right, left), 'score'])
-                                    # list_2d_[i].append(evfold_df_gp.get_group((right, left))['score'].values[0])
-        elif mode == 'numpy':
-            n = len(self.sequence)
-            num_pending = len(self.bigraph)
-            num_aa_in_window = len(self.window_m_ids[0][0])
-            evfold_df = self.file_initiator(
-                fpn=simu_seq_len if self.input_kind == 'simulate' else fpn,
-                is_sort=True,
-                sort_=3,
-            )
-            evfold_np = np.array(evfold_df).T
-            # print(evfold_np)
-            # #/*** block 1 ***/
-            for i in range(self.num_pairs):
-                # #/*** block 1.1 ***/
-                for j in range(num_aa_in_window):
-                    # #/*** block 1.1.1 ***/
-                    if self.window_m_ids[i][0][j] is None or self.window_m_ids[i][1][j] is None:
-                        for k in range(num_pending):
-                            # global_pair_ids[i].append([None, None])
-                            list_2d_[i].append(0)
-                    # #/*** block 1.1.2 ***/
-                    else:
-                        for k in range(num_pending):
-                            # #/*** block 1.1.2.1 ***/
-                            left = self.window_m_ids[i][0][j] - self.bigraph[k][0]
-                            right = self.window_m_ids[i][1][j] - self.bigraph[k][1]
-                            left_inf = left < 1
-                            left_sup = left > n
-                            right_inf = right < 1
-                            right_sup = right > n
-                            reflexive = left == right
-                            if left_inf or left_sup or right_inf or right_sup or reflexive:
-                                # global_pair_ids[i].append([None, None])
-                                list_2d_[i].append(0)
-                            # #/*** block 1.1.2.2 ***/
-                            else:
-                                if left < right:
-                                    # print(evfold_np[2][(evfold_np[0] == left) & (evfold_np[1] == right)][0])
-                                    list_2d_[i].append(evfold_np[2][(evfold_np[0] == left) & (evfold_np[1] == right)][0])
-                                else:
-                                    list_2d_[i].append(evfold_np[2][(evfold_np[0] == right) & (evfold_np[1] == left)][0])
-        end_time = time.time()
-        print('======>bipartite pair assignment: {time}s.'.format(time=end_time - start_time))
-        return list_2d_
+__author__ = "Jianfeng Sun"
+__version__ = "v1.0"
+__copyright__ = "Copyright 2023"
+__license__ = "GPL v3.0"
+__email__ = "jianfeng.sunmt@gmail.com"
+__maintainer__ = "Jianfeng Sun"
+
+import time
+
+import numpy as np
+
+from tmkit.seqnetrr.net.Reader import Reader as prrcreader
+from tmkit.seqnetrr.window.base import Pair as ecabPair
+
+
+class Bipartite(ecabPair.Pair):
+    """Bipartite class offers methods to assign ECA to global pairs."""
+
+    def __init__(
+        self,
+        sequence,
+        window_size,
+        window_m_ids,
+        kind="memconp",
+        patch_size=None,
+        input_kind="general",
+    ):
+        """
+
+        Parameters
+        ----------
+        sequence
+            a protein sequence
+        window_size
+            window size
+        window_m_ids
+            list contains ids of residues in windows
+        input_kind
+            residue contact prediction method
+        """
+        super().__init__(sequence, window_size, window_m_ids)
+        self.prrcreader = prrcreader(seq_sep_inferior=None, seq_sep_superior=None)
+        if kind == "memconp":
+            self.bigraph = [
+                # self.num_to_dos types in MemConP
+                [4, -4],
+                [4, 4],
+                [3, -4],
+                [-4, 3],
+                [3, 4],
+                [4, 3],
+                [0, -4],
+                [0, 4],
+                [0, -3],
+                [0, 3],
+                [-1, 0],
+                [1, 0],
+                [0, 0],
+                [0, -1],
+                [0, 1],
+                [3, 0],
+                [-3, 0],
+                [4, 0],
+                [-4, 0],
+                [-3, -4],
+                [-4, -3],
+                [-3, 4],
+                [4, -3],
+                [-4, -4],
+                [-4, 4],
+            ]
+        if kind == "patch":
+            self.bigraph = self.computlib.patch(length=patch_size)
+            # print(self.bigraph)
+        if kind == "cross":
+            self.bigraph = [
+                [-1, 0],
+                [1, 0],
+                [0, 0],
+                [0, 1],
+                [0, -1],
+            ]
+        if kind == "unchanged":
+            self.bigraph = [
+                [0, 0],
+            ]
+        self.num_to_dos = len(self.bigraph)
+        self.num_to_dos_in_window = self.num_to_dos * self.aa_in_window_size
+        self.input_kind = input_kind
+        if self.input_kind == "general":
+            self.file_initiator = self.prrcreader.general
+        elif self.input_kind == "freecontact":
+            self.file_initiator = self.prrcreader.freecontact
+        elif self.input_kind == "mutual information":
+            self.file_initiator = self.prrcreader.mi
+        elif self.input_kind == "gdca":
+            self.file_initiator = self.prrcreader.gdca
+        elif self.input_kind == "ccmpred":
+            self.file_initiator = self.prrcreader.ccmpred
+        elif self.input_kind == "plmc":
+            self.file_initiator = self.prrcreader.plmc
+        elif self.input_kind == "simulate":
+            self.file_initiator = self.prrcreader.simulate
+        else:
+            self.file_initiator = self.prrcreader.general
+
+    def pairids(self):
+        """
+        Constitutes all global pairs.
+
+        Methods
+        -------
+            1>. pairids
+                1st dimension: all pairs number
+                2nd dimension: (2 * window_size + 1) * length of bigraph list
+                3rd dimension: 2 (a pair)
+            1>. block 1:    traversing all pairs to be processed.
+                |--->block 1.1: traversing all amino acids in a window.
+                    |--->block 1.1.1:
+                        assigning None to those amino acids whose index
+                        beyond sequence length.
+                    |--->block 1.1.2:
+                        assigning calc results to rest of amino acids.
+                            |--->block 1.1.2.1:
+                                assigning None to those indices (original
+                                amino acid index minus number in bigraph
+                                list) beyond sequence length.
+                            |--->block 1.1.2.2:
+                                assigning results to array global_pair_ids.
+            block 2: assign ECA from ccmpred file
+                |--->block 2.1: read ccmpred file
+                |--->block 2.2: assign ECA from ccmpred file
+            block 3: assign ECA from plmc file
+                |--->block 3.1: read plmc file
+                |--->block 3.2: assign ECA from plmc file
+            block 4: assign ECA from gdca file
+                |--->block 4.1: read gdca file
+                |--->block 4.2: assign ECA from gdca file
+
+        Returns
+        -------
+        3d array,list
+
+        """
+        start_time = time.time()
+        n = len(self.sequence)
+        num_pending = len(self.bigraph)
+        num_aa_in_window = len(self.window_m_ids[0][0])
+        global_pair_ids = [[] for _ in range(self.num_pairs)]
+        # #/*** block 1 ***/
+        for i in range(self.num_pairs):
+            # #/*** block 1.1 ***/
+            for j in range(num_aa_in_window):
+                # #/*** block 1.1.1 ***/
+                if (
+                    self.window_m_ids[i][0][j] is None
+                    or self.window_m_ids[i][1][j] is None
+                ):
+                    for k in range(num_pending):
+                        global_pair_ids[i].append([None, None])
+                # #/*** block 1.1.2 ***/
+                else:
+                    for k in range(num_pending):
+                        # #/*** block 1.1.2.1 ***/
+                        left = self.window_m_ids[i][0][j] - self.bigraph[k][0]
+                        right = self.window_m_ids[i][1][j] - self.bigraph[k][1]
+                        left_inf = left < 1
+                        left_sup = left > n
+                        right_inf = right < 1
+                        right_sup = right > n
+                        reflexive = left == right
+                        if left_inf or left_sup or right_inf or right_sup or reflexive:
+                            global_pair_ids[i].append([None, None])
+                        # #/*** block 1.1.2.2 ***/
+                        else:
+                            if left < right:
+                                global_pair_ids[i].append([left, right])
+                            else:
+                                global_pair_ids[i].append([right, left])
+        end_time = time.time()
+        print(
+            "======>bipartite pair generation: {time}s.".format(
+                time=end_time - start_time
+            )
+        )
+        # print(global_pair_ids)
+        # print(len(global_pair_ids))
+        # print(len(global_pair_ids[0]))
+        # print(global_pair_ids[0])
+        # print(len(global_pair_ids[0][0]))
+        # print(global_pair_ids[0][0])
+        return global_pair_ids
+
+    def assign(self, list_2d, fpn=None, simu_seq_len=100, mode="hash"):
+        """
+
+        Parameters
+        ----------
+        list_2d
+            2dlist
+        fpn
+            path to a protein residue contact map file
+        simu_seq_len
+            length of a simulated FASTA sequence
+        mode
+            mode of assignment: hash | hash_ori | hash_rl | pandas | numpy
+
+        Returns
+        -------
+            2d array - list
+
+        """
+        start_time = time.time()
+        list_2d_ = list_2d
+        if mode == "hash_rl":
+            global_pair_ids = self.pairids()
+            pairs_left = []
+            pairs_right = []
+            for i in range(self.num_pairs):
+                for j in range(self.num_to_dos * (2 * self.window_size + 1)):
+                    pairs_left.append(global_pair_ids[i][j][0])
+                    pairs_right.append(global_pair_ids[i][j][1])
+            # print('Left pairs {}: {}'.format(len(pairs_right), len(pairs_left)))
+            # print('Right pairs {}: {}'.format(len(pairs_left), len(pairs_right)))
+            mark = len(pairs_left)
+            # #/*** block 1 ***/
+            # #/*** block 1.1 ***/
+            evfold_dict = self.file_initiator(
+                fpn=simu_seq_len if self.input_kind == "simulate" else fpn,
+                sort_=5,
+            )
+            # print(evfold_dict)
+            # #/*** block 1.2 ***/
+            FCj = 0
+            for i in range(mark):
+                if i % (self.num_to_dos * (2 * self.window_size + 1)) == 0:
+                    FCj += 1
+                if pairs_left[i] is None or pairs_right[i] is None:
+                    list_2d_[FCj - 1].append(0)
+                else:
+                    inf = pairs_left[i]
+                    sup = pairs_right[i]
+                    # print([inf, sup])
+                    list_2d_[FCj - 1].append(evfold_dict[inf][sup])
+        elif mode == "hash_ori":
+            evfold_dict = self.file_initiator(
+                fpn=simu_seq_len if self.input_kind == "simulate" else fpn,
+                sort_=5,
+            )
+            global_pair_ids = self.pairids()
+            # #/*** block 1 ***/
+            for i in range(self.num_pairs):
+                # #/*** block 1.1 ***/
+                for j in range(self.num_to_dos_in_window):
+                    inf = global_pair_ids[i][j][0]
+                    sup = global_pair_ids[i][j][1]
+                    if inf is None or sup is None:
+                        list_2d_[i].append(0)
+                    else:
+                        list_2d_[i].append(evfold_dict[inf][sup])
+        elif mode == "hash":
+            n = len(self.sequence)
+            num_pending = len(self.bigraph)
+            num_aa_in_window = len(self.window_m_ids[0][0])
+            evfold_dict = self.file_initiator(
+                fpn=simu_seq_len if self.input_kind == "simulate" else fpn,
+                sort_=5,
+            )
+            # #/*** block 1 ***/
+            for i in range(self.num_pairs):
+                # #/*** block 1.1 ***/
+                for j in range(num_aa_in_window):
+                    # #/*** block 1.1.1 ***/
+                    if (
+                        self.window_m_ids[i][0][j] is None
+                        or self.window_m_ids[i][1][j] is None
+                    ):
+                        for k in range(num_pending):
+                            # global_pair_ids[i].append([None, None])
+                            list_2d_[i].append(0)
+                    # #/*** block 1.1.2 ***/
+                    else:
+                        for k in range(num_pending):
+                            # #/*** block 1.1.2.1 ***/
+                            left = self.window_m_ids[i][0][j] - self.bigraph[k][0]
+                            right = self.window_m_ids[i][1][j] - self.bigraph[k][1]
+                            left_inf = left < 1
+                            left_sup = left > n
+                            right_inf = right < 1
+                            right_sup = right > n
+                            reflexive = left == right
+                            if (
+                                left_inf
+                                or left_sup
+                                or right_inf
+                                or right_sup
+                                or reflexive
+                            ):
+                                # global_pair_ids[i].append([None, None])
+                                list_2d_[i].append(0)
+                            # #/*** block 1.1.2.2 ***/
+                            else:
+                                if left < right:
+                                    list_2d_[i].append(evfold_dict[left][right])
+                                else:
+                                    list_2d_[i].append(evfold_dict[right][left])
+        elif mode == "pandas":
+            n = len(self.sequence)
+            num_pending = len(self.bigraph)
+            num_aa_in_window = len(self.window_m_ids[0][0])
+            evfold_df = self.file_initiator(
+                fpn=simu_seq_len if self.input_kind == "simulate" else fpn,
+                is_sort=True,
+                sort_=3,
+            )
+            evfold_df = evfold_df.set_index(["id_1", "id_2"])
+            # print(evfold_df)
+            # evfold_df_gp = evfold_df.groupby(by=['id_1', 'id_2'])
+            # evfold_df_gp_keys = evfold_df_gp.groups.keys()
+            # print(evfold_df_gp_keys)
+            # #/*** block 1 ***/
+            for i in range(self.num_pairs):
+                # #/*** block 1.1 ***/
+                for j in range(num_aa_in_window):
+                    # #/*** block 1.1.1 ***/
+                    if (
+                        self.window_m_ids[i][0][j] is None
+                        or self.window_m_ids[i][1][j] is None
+                    ):
+                        for k in range(num_pending):
+                            # global_pair_ids[i].append([None, None])
+                            list_2d_[i].append(0)
+                    # #/*** block 1.1.2 ***/
+                    else:
+                        for k in range(num_pending):
+                            # #/*** block 1.1.2.1 ***/
+                            left = self.window_m_ids[i][0][j] - self.bigraph[k][0]
+                            right = self.window_m_ids[i][1][j] - self.bigraph[k][1]
+                            left_inf = left < 1
+                            left_sup = left > n
+                            right_inf = right < 1
+                            right_sup = right > n
+                            reflexive = left == right
+                            if (
+                                left_inf
+                                or left_sup
+                                or right_inf
+                                or right_sup
+                                or reflexive
+                            ):
+                                # global_pair_ids[i].append([None, None])
+                                list_2d_[i].append(0)
+                            # #/*** block 1.1.2.2 ***/
+                            else:
+                                if left < right:
+                                    # print(evfold_df.at[(left, right), 'score'])
+                                    list_2d_[i].append(
+                                        evfold_df.at[(left, right), "score"]
+                                    )
+                                    # list_2d_[i].append(evfold_df.loc[(evfold_df['id_1'] == left) & (evfold_df['id_2'] == right)])
+                                    # list_2d_[i].append(evfold_df.ix[(left, right), 'score'])
+                                    # list_2d_[i].append(evfold_df_gp.get_group((left, right))['score'].values[0])
+                                else:
+                                    # print(evfold_df.at[(right, left), 'score'])
+                                    list_2d_[i].append(
+                                        evfold_df.at[(right, left), "score"]
+                                    )
+                                    # list_2d_[i].append(evfold_df.loc[(evfold_df['id_1'] == right) & (evfold_df['id_2'] == left)])
+                                    # list_2d_[i].append(evfold_np[2][(evfold_np[0] == right) & (evfold_np[1] == left)])
+                                    # list_2d_[i].append(evfold_df.ix[(right, left), 'score'])
+                                    # list_2d_[i].append(evfold_df_gp.get_group((right, left))['score'].values[0])
+        elif mode == "numpy":
+            n = len(self.sequence)
+            num_pending = len(self.bigraph)
+            num_aa_in_window = len(self.window_m_ids[0][0])
+            evfold_df = self.file_initiator(
+                fpn=simu_seq_len if self.input_kind == "simulate" else fpn,
+                is_sort=True,
+                sort_=3,
+            )
+            evfold_np = np.array(evfold_df).T
+            # print(evfold_np)
+            # #/*** block 1 ***/
+            for i in range(self.num_pairs):
+                # #/*** block 1.1 ***/
+                for j in range(num_aa_in_window):
+                    # #/*** block 1.1.1 ***/
+                    if (
+                        self.window_m_ids[i][0][j] is None
+                        or self.window_m_ids[i][1][j] is None
+                    ):
+                        for k in range(num_pending):
+                            # global_pair_ids[i].append([None, None])
+                            list_2d_[i].append(0)
+                    # #/*** block 1.1.2 ***/
+                    else:
+                        for k in range(num_pending):
+                            # #/*** block 1.1.2.1 ***/
+                            left = self.window_m_ids[i][0][j] - self.bigraph[k][0]
+                            right = self.window_m_ids[i][1][j] - self.bigraph[k][1]
+                            left_inf = left < 1
+                            left_sup = left > n
+                            right_inf = right < 1
+                            right_sup = right > n
+                            reflexive = left == right
+                            if (
+                                left_inf
+                                or left_sup
+                                or right_inf
+                                or right_sup
+                                or reflexive
+                            ):
+                                # global_pair_ids[i].append([None, None])
+                                list_2d_[i].append(0)
+                            # #/*** block 1.1.2.2 ***/
+                            else:
+                                if left < right:
+                                    # print(evfold_np[2][(evfold_np[0] == left) & (evfold_np[1] == right)][0])
+                                    list_2d_[i].append(
+                                        evfold_np[2][
+                                            (evfold_np[0] == left)
+                                            & (evfold_np[1] == right)
+                                        ][0]
+                                    )
+                                else:
+                                    list_2d_[i].append(
+                                        evfold_np[2][
+                                            (evfold_np[0] == right)
+                                            & (evfold_np[1] == left)
+                                        ][0]
+                                    )
+        end_time = time.time()
+        print(
+            "======>bipartite pair assignment: {time}s.".format(
+                time=end_time - start_time
+            )
+        )
+        return list_2d_
```

### Comparing `tmkit-0.0.2/tmkit/seqnetrr/graph/Unipartite.py` & `tmkit-0.0.3/tmkit/seqnetrr/graph/Unipartite.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,415 +1,438 @@
-__author__ = "Jianfeng Sun"
-__version__ = "v1.0"
-__copyright__ = "Copyright 2023"
-__license__ = "GPL v3.0"
-__email__ = "jianfeng.sunmt@gmail.com"
-__maintainer__ = "Jianfeng Sun"
-
-import time
-import itertools
-import numpy as np
-from tmkit.seqnetrr.window.base import Pair as ecabPair
-from tmkit.seqnetrr.net.Reader import reader as prrcreader
-
-
-class unipartite(ecabPair.pair):
-    """
-
-    Notes
-    -----
-       make(), assign().
-    reflexive class offers methods to assign CI to reflexive pairs.
-
-    References
-    ----------
-       It has been built since April, 2018.
-       Change Log:
-       1>. It has been revised since the end of June, 2018.
-       2>. It has been revised since Oct. 11th, 2018.
-
-    """
-
-    def __init__(
-            self,
-            sequence,
-            window_size,
-            window_m_ids,
-            input_kind='general',
-    ):
-        super(unipartite, self).__init__(sequence, window_size, window_m_ids)
-        self.prrcreader = prrcreader(
-            seq_sep_inferior=None,
-            seq_sep_superior=None
-        )
-        self.input_kind = input_kind
-        if self.input_kind == 'general':
-            self.file_initiator = self.prrcreader.general
-        elif self.input_kind == 'freecontact':
-            self.file_initiator = self.prrcreader.freecontact
-        elif self.input_kind == 'mutual information':
-            self.file_initiator = self.prrcreader.mi
-        elif self.input_kind == 'gdca':
-            self.file_initiator = self.prrcreader.gdca
-        elif self.input_kind == 'ccmpred':
-            self.file_initiator = self.prrcreader.ccmpred
-        elif self.input_kind == 'plmc':
-            self.file_initiator = self.prrcreader.plmc
-        elif self.input_kind == 'simulate':
-            self.file_initiator = self.prrcreader.simulate
-        else:
-            self.file_initiator = self.prrcreader.general
-
-    def pairids(self):
-        """
-
-        Methods
-        -------
-            1>. In this method, we constituted all reflexive pairs commbinations complying
-               with the concept of localEVfold, which means we eliminate all symmetric pairs,
-               like [a, b] or [b, a]. Because those two values equal with each other.
-               It is noted that the action below we haven't done yet: let a be first and b
-               be second if a < b.
-            2>. a. 1st dimension is also an ensemble of all pairs being in contact or not.
-               Length of first dimension is, for example, 119 (or first 800 that we specify)
-               for contact pairs in protein sequence 1atz A chain.
-               b. 2nd dimension includes the combinations of all pairs regularized by windows.
-               An example is that window size is 5, the length of second dimension is
-               [(5*2+1)(5*2)/2]*2 = 110. The correct understanding of number 2 outside square
-               bracket is that we have two residues, so we have to multipy 2 outside the
-               square bracket.
-               c. 3rd dimension is two residues serving as a pair.
-            3>. block 1: pairs[i][0] (e.g. [1, 2, 5]) is a residues ensemble that has been windowed by left
-                        residue of a pair. pairs[i][1] is a residues ensemble that has been
-                        windowed by right residue of a pair. itertools.combinations() perfroms
-                        any two residues combination from pairs[i][0] or pairs[i][1].
-               |------- block 1.1: l1 is any two residues combination from side_of_pair1, e.g.
-                                   [1, 2], [2, 5], [1, 5].
-               |------- block 1.2: l2 is any two residues combination from side_of_pair2.
-
-        Raises
-        ------
-            1>. It has been revised since the end of June, 2018.
-            2>. It has been revised since Oct. 10th, 2018.
-            3>. It has been revised since Sep. 19th, 2019.
-
-        Returns
-        -------
-            3d array
-
-        """
-        start_time = time.time()
-        local_pairs = [[] for _ in range(self.num_pairs)]
-        # #/*** block 1 ***/
-        for i in range(self.num_pairs):
-            # #/*** block 1.1 ***/
-            t1 = self.combo2x2(self.window_m_ids[i][0])
-            # print('win',self.window_m_ids[i][0])
-            # print(t1)
-            # for l1 in t1:
-            #     if l1[0] is not None and l1[1] is not None and l1[0] < l1[1]:
-            #         local_pairs[i].append([l1[0], l1[1]])
-            #     else:
-            #         local_pairs[i].append([l1[1], l1[0]])
-            for l1 in t1:
-                if l1[0] is not None and l1[1] is None:
-                    local_pairs[i].append([l1[0], None])
-                elif l1[0] is None and l1[1] is not None:
-                    local_pairs[i].append([None, l1[1]])
-                elif l1[0] is not None and l1[1] is not None:
-                    if l1[0] < l1[1]:
-                        local_pairs[i].append([l1[0], l1[1]])
-                    else:
-                        local_pairs[i].append([l1[1], l1[0]])
-                else:
-                    local_pairs[i].append([None, None])
-            # #/*** block 1.2 ***/
-            t2 = self.combo2x2(self.window_m_ids[i][1])
-            # for l2 in t2:
-            #     if l2[0] is not None and l2[1] is not None and l2[0] < l2[1]:
-            #         local_pairs[i].append([l2[0], l2[1]])
-            #     else:
-            #         local_pairs[i].append([l2[1], l2[0]])
-            for l2 in t2:
-                if l2[0] is not None and l2[1] is None:
-                    local_pairs[i].append([l2[0], None])
-                elif l2[0] is None and l2[1] is not None:
-                    local_pairs[i].append([None, l2[1]])
-                elif l2[0] is not None and l2[1] is not None:
-                    if l2[0] < l2[1]:
-                        local_pairs[i].append([l2[0], l2[1]])
-                    else:
-                        local_pairs[i].append([l2[1], l2[0]])
-                else:
-                    local_pairs[i].append([None, None])
-        end_time = time.time()
-        print('======>unipartite pair generation: {time}s.'.format(time=end_time - start_time))
-        return local_pairs
-
-    def combo2x2(self, array):
-        """
-
-        Notes
-        -----
-            nonrepeated 2x2 combination of elements of an array.
-
-        Parameters
-        ----------
-        array
-            amount of combo2x2: L*(L-1)/2.
-
-        Returns
-        -------
-
-        """
-        combo = []
-        ob = itertools.combinations(array, 2)
-        for i in ob:
-            combo.append(list(i))
-        return combo
-
-    def assign(self, list_2d, fpn=None, simu_seq_len=100, mode='hash'):
-        """
-
-        Notes
-        -----
-            assign() uses a fast algorithm to generate CI features for given reflexive pairs.
-
-        Methods
-        -------
-            1>. We provide a very fast data generation method for CIs. Typically this algorithm
-            can speed up around 5-10 times than the general method shown in the example below.
-            2>. The input dataset is a 2d dataset, like a stack, because we will do a stack op
-            later on. Data will be constantly fed into this stack.
-            The length of each contact pair or noncontact pair is [(5*2+1)(5*2)/2]*2 = 110
-            if we specify for a window size 5. Let's say:
-                          number: [(window_size * 2 + 1)(window_size * 2)/2]*2.
-            supp: Another fast retrieval way:
-            >>># list_2d[j-1].append(
-            >>># np.array(ccmpred.loc[(ccmpred['id_1'] == inf) &
-            >>># (ccmpred['id_2'] == sup)]['score'])[0])
-            3>. :arg [a, b] or [inf, sup]: the inferior(inf) and superior(sup) in a protein
-                                      sequence, separately.
-            :arg k: k = (a - 1) * length_sequence - {[a * (a + 1)] / 2} + b can be an index
-                   of pairwise residue in any CI file.
-            4>. block 1: assign CIs and FCj is a vernier of residue pairs to mark which pair we reach.
-            |------- block 1.1: read freecontact file
-            |------- block 1.2: assign CI from freecontact file
-                    |--------- block 1.2.1: i % (2 * self.stretch_window) means the completion
-                                            of all pairs in a window for first central pair,
-                                            where i is current residue in pair_left. This
-                                            sub-block means that assigning CIs will be finished
-                                            for each central pair until all residue pairs
-                                            combination in this window have been traversed
-                                            only once. And then it is next turn (execute
-                                            FCj + 1 op) for second central pair and so on.
-            block 2: assign CI from ccmpred file
-            |------- block 2.1: read ccmpred file
-            |------- block 2.2: assign CI from ccmpred file
-            block 3: assign CI from plmc file
-            |------- block 3.1: read plmc file
-            |------- block 3.2: assign CI from plmc file
-            block 4: assign CI from gdca file
-            |------- block 4.1: read gdca file
-            |------- block 4.2: assign CI from gdca file
-
-        Examples
-        --------
-            The time complexity of an example below is o(n^3)'''
-            >>># for i in range(len(local_pair_ids)):
-            >>>#     for j in range(len(local_pair_ids[0])):
-            >>>#         if local_pair_ids[i][j][0] is None or local_pair_ids[i][j][1] is None:
-            >>>#             trainning_data[i].append(0)
-            >>>#         else:
-            >>>#             for k in range(len(ccmpred_np)):
-            >>>#                 if ccmpred_np[k][0] == local_pair_ids[i][j][0] \
-            >>>#                         and ccmpred_np[k][1] == local_pair_ids[i][j][1] \
-            >>>#                         or ccmpred_np[k][0] == local_pair_ids[i][j][1] \
-            >>>#                         and ccmpred_np[k][1] == local_pair_ids[i][j][0]:
-            >>>#                     trainning_data[i].append(ccmpred_np[k][2])
-
-        Raises
-        ------
-            It has been built since April, 2018.
-            1>. It has been revised since the end of June, 2018.
-            2>. It has been revised since Oct. 10th, 2018.
-            3>. It has been revised since Sep. 19th, 2019.
-            3>. It has been revised since Sep. 23th, 2019.
-
-        Parameters
-        ----------
-        list_2d
-        fpn
-        simu_seq_len
-        mode
-
-        Returns
-        -------
-            2d array - list
-
-        """
-        start_time = time.time()
-        list_2d_ = list_2d
-        if mode == 'hash_rl':
-            local_pair_ids = self.pairids()
-            # print(local_pair_ids[0])
-            # print(len(local_pair_ids))
-            # print(len(local_pair_ids[0]))
-            # print(len(local_pair_ids[0][0]))
-            pairs_left = []
-            pairs_right = []
-            for i in range(self.num_pairs):
-                for j in range(2 * self.stretch_window):
-                    pairs_left.append(local_pair_ids[i][j][0])
-                    pairs_right.append(local_pair_ids[i][j][1])
-            # print('Left Pairs: {}'.format(pairs_left))
-            # print('Right Pairs: {}'.format(pairs_right))
-            # #/*** block 1 ***/
-            FCj = 0
-            # #/*** block 1.1 ***/
-            evfold_dict = self.file_initiator(
-                fpn=simu_seq_len if self.input_kind == 'simulate' else fpn,
-                sort_=5,
-            )
-            # #/*** block 1.2 ***/
-            for i in range(len(pairs_left)):
-                # #/*** block 1.2.1 ***/
-                if i % (2 * self.stretch_window) == 0:
-                    FCj += 1
-                if pairs_left[i] is None or pairs_right[i] is None:
-                    list_2d_[FCj - 1].append(0)
-                else:
-                    inf = pairs_left[i]
-                    sup = pairs_right[i]
-                    # print([inf, sup])
-                    list_2d_[FCj-1].append(evfold_dict[inf][sup])
-        elif mode == 'hash_ori':
-            evfold_dict = self.file_initiator(
-                fpn=simu_seq_len if self.input_kind == 'simulate' else fpn,
-                sort_=5,
-            )
-            local_pair_ids = self.pairids()
-            # #/*** block 1 ***/
-            for i in range(self.num_pairs):
-                # #/*** block 1.1 ***/
-                for j in range(2 * self.stretch_window):
-                    inf = local_pair_ids[i][j][0]
-                    sup = local_pair_ids[i][j][1]
-                    if inf is None or sup is None:
-                        list_2d_[i].append(0)
-                    else:
-                        list_2d_[i].append(evfold_dict[inf][sup])
-        elif mode == 'hash':
-            evfold_dict = self.file_initiator(
-                fpn=simu_seq_len if self.input_kind == 'simulate' else fpn,
-                sort_=5,
-            )
-            # #/*** block 1 ***/
-            for i in range(self.num_pairs):
-                # #/*** block 1.1 ***/
-                t1 = self.combo2x2(self.window_m_ids[i][0])
-                # print(self.window_m_ids[i][0])
-                # print(self.combo2x2(self.window_m_ids[i][0]))
-                for l1 in t1:
-                    if l1[0] is not None and l1[1] is None:
-                        list_2d_[i].append(0)
-                    elif l1[0] is None and l1[1] is not None:
-                        list_2d_[i].append(0)
-                    elif l1[0] is not None and l1[1] is not None:
-                        if l1[0] < l1[1]:
-                            list_2d_[i].append(evfold_dict[l1[0]][l1[1]])
-                        else:
-                            list_2d_[i].append(evfold_dict[l1[1]][l1[0]])
-                    else:
-                        list_2d_[i].append(0)
-                # #/*** block 1.2 ***/
-                t2 = self.combo2x2(self.window_m_ids[i][1])
-                for l2 in t2:
-                    if l2[0] is not None and l2[1] is None:
-                        list_2d_[i].append(0)
-                    elif l2[0] is None and l2[1] is not None:
-                        list_2d_[i].append(0)
-                    elif l2[0] is not None and l2[1] is not None:
-                        if l2[0] < l2[1]:
-                            list_2d_[i].append(evfold_dict[l2[0]][l2[1]])
-                        else:
-                            list_2d_[i].append(evfold_dict[l2[1]][l2[0]])
-                    else:
-                        list_2d_[i].append(0)
-        elif mode == 'pandas':
-            evfold_df = self.file_initiator(
-                fpn=simu_seq_len if self.input_kind == 'simulate' else fpn,
-                is_sort=True,
-                sort_=3,
-            )
-            evfold_df = evfold_df.set_index(['id_1', 'id_2'])
-            # #/*** block 1 ***/
-            for i in range(self.num_pairs):
-                # #/*** block 1.1 ***/
-                t1 = self.combo2x2(self.window_m_ids[i][0])
-                for l1 in t1:
-                    if l1[0] is not None and l1[1] is None:
-                        list_2d_[i].append(0)
-                    elif l1[0] is None and l1[1] is not None:
-                        list_2d_[i].append(0)
-                    elif l1[0] is not None and l1[1] is not None:
-                        if l1[0] < l1[1]:
-                            # print(evfold_df.at[(l1[0], l1[1]), 'score'])
-                            list_2d_[i].append(evfold_df.at[(l1[0], l1[1]), 'score'])
-                        else:
-                            # print(evfold_df.at[(l1[1], l1[0]), 'score'])
-                            list_2d_[i].append(evfold_df.at[(l1[1], l1[0]), 'score'])
-                    else:
-                        list_2d_[i].append(0)
-                # #/*** block 1.2 ***/
-                t2 = self.combo2x2(self.window_m_ids[i][1])
-                for l2 in t2:
-                    if l2[0] is not None and l2[1] is None:
-                        list_2d_[i].append(0)
-                    elif l2[0] is None and l2[1] is not None:
-                        list_2d_[i].append(0)
-                    elif l2[0] is not None and l2[1] is not None:
-                        if l2[0] < l2[1]:
-                            list_2d_[i].append(evfold_df.at[(l2[0], l2[1]), 'score'])
-                        else:
-                            list_2d_[i].append(evfold_df.at[(l2[1], l2[0]), 'score'])
-                    else:
-                        list_2d_[i].append(0)
-        elif mode == 'numpy':
-            evfold_df = self.file_initiator(
-                fpn=simu_seq_len if self.input_kind == 'simulate' else fpn,
-                is_sort=True,
-                sort_=3,
-            )
-            evfold_np = np.array(evfold_df).T
-            # #/*** block 1 ***/
-            for i in range(self.num_pairs):
-                # #/*** block 1.1 ***/
-                t1 = self.combo2x2(self.window_m_ids[i][0])
-                for l1 in t1:
-                    if l1[0] is not None and l1[1] is None:
-                        list_2d_[i].append(0)
-                    elif l1[0] is None and l1[1] is not None:
-                        list_2d_[i].append(0)
-                    elif l1[0] is not None and l1[1] is not None:
-                        if l1[0] < l1[1]:
-                            list_2d_[i].append(evfold_np[2][(evfold_np[0] == l1[0]) & (evfold_np[1] == l1[1])][0])
-                        else:
-                            list_2d_[i].append(evfold_np[2][(evfold_np[0] == l1[1]) & (evfold_np[1] == l1[0])][0])
-                    else:
-                        list_2d_[i].append(0)
-                # #/*** block 1.2 ***/
-                t2 = self.combo2x2(self.window_m_ids[i][1])
-                for l2 in t2:
-                    if l2[0] is not None and l2[1] is None:
-                        list_2d_[i].append(0)
-                    elif l2[0] is None and l2[1] is not None:
-                        list_2d_[i].append(0)
-                    elif l2[0] is not None and l2[1] is not None:
-                        if l2[0] < l2[1]:
-                            list_2d_[i].append(evfold_np[2][(evfold_np[0] == l2[0]) & (evfold_np[1] == l2[1])][0])
-                        else:
-                            list_2d_[i].append(evfold_np[2][(evfold_np[0] == l2[1]) & (evfold_np[1] == l2[0])][0])
-                    else:
-                        list_2d_[i].append(0)
-        print('======>unipartite pair assignment: {time}s.'.format(time=time.time() - start_time))
-        return list_2d_
+__author__ = "Jianfeng Sun"
+__version__ = "v1.0"
+__copyright__ = "Copyright 2023"
+__license__ = "GPL v3.0"
+__email__ = "jianfeng.sunmt@gmail.com"
+__maintainer__ = "Jianfeng Sun"
+
+import itertools
+import time
+
+import numpy as np
+
+from tmkit.seqnetrr.net.Reader import Reader as prrcreader
+from tmkit.seqnetrr.window.base import Pair as ecabPair
+
+
+class Unipartite(ecabPair.Pair):
+    """Reflexive class offers methods to assign CI to reflexive pairs."""
+
+    def __init__(
+        self,
+        sequence: str,
+        window_size: int,
+        window_m_ids: list,
+        input_kind: str="general",
+    ):
+        """
+
+        Parameters
+        ----------
+
+        sequence
+            a protein sequence
+        window_size
+            window size
+        window_m_ids
+            list contains ids of residues in windows
+        input_kind
+            residue contact prediction method
+        """
+        super().__init__(sequence, window_size, window_m_ids)
+        self.prrcreader = prrcreader(seq_sep_inferior=None, seq_sep_superior=None)
+        self.input_kind = input_kind
+        if self.input_kind == "general":
+            self.file_initiator = self.prrcreader.general
+        elif self.input_kind == "freecontact":
+            self.file_initiator = self.prrcreader.freecontact
+        elif self.input_kind == "mutual information":
+            self.file_initiator = self.prrcreader.mi
+        elif self.input_kind == "gdca":
+            self.file_initiator = self.prrcreader.gdca
+        elif self.input_kind == "ccmpred":
+            self.file_initiator = self.prrcreader.ccmpred
+        elif self.input_kind == "plmc":
+            self.file_initiator = self.prrcreader.plmc
+        elif self.input_kind == "simulate":
+            self.file_initiator = self.prrcreader.simulate
+        else:
+            self.file_initiator = self.prrcreader.general
+
+    def pairids(self):
+        """
+
+        Methods
+        -------
+            1>. In this method, we constituted all reflexive pairs commbinations complying
+               with the concept of localEVfold, which means we eliminate all symmetric pairs,
+               like [a, b] or [b, a]. Because those two values equal with each other.
+               It is noted that the action below we haven't done yet: let a be first and b
+               be second if a < b.
+            2>. a. 1st dimension is also an ensemble of all pairs being in contact or not.
+               Length of first dimension is, for example, 119 (or first 800 that we specify)
+               for contact pairs in protein sequence 1atz A chain.
+               b. 2nd dimension includes the combinations of all pairs regularized by windows.
+               An example is that window size is 5, the length of second dimension is
+               [(5*2+1)(5*2)/2]*2 = 110. The correct understanding of number 2 outside square
+               bracket is that we have two residues, so we have to multipy 2 outside the
+               square bracket.
+               c. 3rd dimension is two residues serving as a pair.
+            3>. block 1: pairs[i][0] (e.g. [1, 2, 5]) is a residues ensemble that has been windowed by left
+                        residue of a pair. pairs[i][1] is a residues ensemble that has been
+                        windowed by right residue of a pair. itertools.combinations() perfroms
+                        any two residues combination from pairs[i][0] or pairs[i][1].
+               |------- block 1.1: l1 is any two residues combination from side_of_pair1, e.g.
+                                   [1, 2], [2, 5], [1, 5].
+               |------- block 1.2: l2 is any two residues combination from side_of_pair2.
+
+        Raises
+        ------
+            1>. It has been revised since the end of June, 2018.
+            2>. It has been revised since Oct. 10th, 2018.
+            3>. It has been revised since Sep. 19th, 2019.
+
+        Returns
+        -------
+            3d array
+
+        """
+        start_time = time.time()
+        local_pairs = [[] for _ in range(self.num_pairs)]
+        # #/*** block 1 ***/
+        for i in range(self.num_pairs):
+            # #/*** block 1.1 ***/
+            t1 = self.combo2x2(self.window_m_ids[i][0])
+            # print('win',self.window_m_ids[i][0])
+            # print(t1)
+            # for l1 in t1:
+            #     if l1[0] is not None and l1[1] is not None and l1[0] < l1[1]:
+            #         local_pairs[i].append([l1[0], l1[1]])
+            #     else:
+            #         local_pairs[i].append([l1[1], l1[0]])
+            for l1 in t1:
+                if l1[0] is not None and l1[1] is None:
+                    local_pairs[i].append([l1[0], None])
+                elif l1[0] is None and l1[1] is not None:
+                    local_pairs[i].append([None, l1[1]])
+                elif l1[0] is not None and l1[1] is not None:
+                    if l1[0] < l1[1]:
+                        local_pairs[i].append([l1[0], l1[1]])
+                    else:
+                        local_pairs[i].append([l1[1], l1[0]])
+                else:
+                    local_pairs[i].append([None, None])
+            # #/*** block 1.2 ***/
+            t2 = self.combo2x2(self.window_m_ids[i][1])
+            # for l2 in t2:
+            #     if l2[0] is not None and l2[1] is not None and l2[0] < l2[1]:
+            #         local_pairs[i].append([l2[0], l2[1]])
+            #     else:
+            #         local_pairs[i].append([l2[1], l2[0]])
+            for l2 in t2:
+                if l2[0] is not None and l2[1] is None:
+                    local_pairs[i].append([l2[0], None])
+                elif l2[0] is None and l2[1] is not None:
+                    local_pairs[i].append([None, l2[1]])
+                elif l2[0] is not None and l2[1] is not None:
+                    if l2[0] < l2[1]:
+                        local_pairs[i].append([l2[0], l2[1]])
+                    else:
+                        local_pairs[i].append([l2[1], l2[0]])
+                else:
+                    local_pairs[i].append([None, None])
+        end_time = time.time()
+        print(
+            "======>unipartite pair generation: {time}s.".format(
+                time=end_time - start_time
+            )
+        )
+        return local_pairs
+
+    def combo2x2(self, array):
+        """
+        Non-repeated 2x2 combination of elements of an array.
+
+        Parameters
+        ----------
+        array
+            amount of combo2x2: L*(L-1)/2.
+
+        Returns
+        -------
+        List
+            2D list
+
+        """
+        combo = []
+        ob = itertools.combinations(array, 2)
+        for i in ob:
+            combo.append(list(i))
+        return combo
+
+    def assign(self, list_2d, fpn=None, simu_seq_len=100, mode="hash"):
+        """
+        It uses a fast algorithm to generate CI features for given reflexive pairs.
+
+        Methods
+        -------
+            1>. We provide a very fast data generation method for CIs. Typically this algorithm
+            can speed up around 5-10 times than the general method shown in the example below.
+            2>. The input dataset is a 2d dataset, like a stack, because we will do a stack op
+            later on. Data will be constantly fed into this stack.
+            The length of each contact pair or noncontact pair is [(5*2+1)(5*2)/2]*2 = 110
+            if we specify for a window size 5. Let's say:
+                          number: [(window_size * 2 + 1)(window_size * 2)/2]*2.
+            supp: Another fast retrieval way:
+            >>># list_2d[j-1].append(
+            >>># np.array(ccmpred.loc[(ccmpred['id_1'] == inf) &
+            >>># (ccmpred['id_2'] == sup)]['score'])[0])
+            3>. :arg [a, b] or [inf, sup]: the inferior(inf) and superior(sup) in a protein
+                                      sequence, separately.
+            :arg k: k = (a - 1) * length_sequence - {[a * (a + 1)] / 2} + b can be an index
+                   of pairwise residue in any CI file.
+            4>. block 1: assign CIs and FCj is a vernier of residue pairs to mark which pair we reach.
+            |------- block 1.1: read freecontact file
+            |------- block 1.2: assign CI from freecontact file
+                    |--------- block 1.2.1: i % (2 * self.stretch_window) means the completion
+                                            of all pairs in a window for first central pair,
+                                            where i is current residue in pair_left. This
+                                            sub-block means that assigning CIs will be finished
+                                            for each central pair until all residue pairs
+                                            combination in this window have been traversed
+                                            only once. And then it is next turn (execute
+                                            FCj + 1 op) for second central pair and so on.
+            block 2: assign CI from ccmpred file
+            |------- block 2.1: read ccmpred file
+            |------- block 2.2: assign CI from ccmpred file
+            block 3: assign CI from plmc file
+            |------- block 3.1: read plmc file
+            |------- block 3.2: assign CI from plmc file
+            block 4: assign CI from gdca file
+            |------- block 4.1: read gdca file
+            |------- block 4.2: assign CI from gdca file
+
+        Examples
+        --------
+            The time complexity of an example below is o(n^3)'''
+            >>># for i in range(len(local_pair_ids)):
+            >>>#     for j in range(len(local_pair_ids[0])):
+            >>>#         if local_pair_ids[i][j][0] is None or local_pair_ids[i][j][1] is None:
+            >>>#             trainning_data[i].append(0)
+            >>>#         else:
+            >>>#             for k in range(len(ccmpred_np)):
+            >>>#                 if ccmpred_np[k][0] == local_pair_ids[i][j][0] \
+            >>>#                         and ccmpred_np[k][1] == local_pair_ids[i][j][1] \
+            >>>#                         or ccmpred_np[k][0] == local_pair_ids[i][j][1] \
+            >>>#                         and ccmpred_np[k][1] == local_pair_ids[i][j][0]:
+            >>>#                     trainning_data[i].append(ccmpred_np[k][2])
+
+        Raises
+        ------
+            It has been built since April, 2018.
+            1>. It has been revised since the end of June, 2018.
+            2>. It has been revised since Oct. 10th, 2018.
+            3>. It has been revised since Sep. 19th, 2019.
+            3>. It has been revised since Sep. 23th, 2019.
+
+        Parameters
+        ----------
+        list_2d
+            2dlist
+        fpn
+            path to a protein residue contact map file
+        simu_seq_len
+            length of a simulated FASTA sequence
+        mode
+            mode of assignment: hash | hash_ori | hash_rl | pandas | numpy
+
+        Returns
+        -------
+            2d array - list
+
+        """
+        start_time = time.time()
+        list_2d_ = list_2d
+        if mode == "hash_rl":
+            local_pair_ids = self.pairids()
+            # print(local_pair_ids[0])
+            # print(len(local_pair_ids))
+            # print(len(local_pair_ids[0]))
+            # print(len(local_pair_ids[0][0]))
+            pairs_left = []
+            pairs_right = []
+            for i in range(self.num_pairs):
+                for j in range(2 * self.stretch_window):
+                    pairs_left.append(local_pair_ids[i][j][0])
+                    pairs_right.append(local_pair_ids[i][j][1])
+            # print('Left Pairs: {}'.format(pairs_left))
+            # print('Right Pairs: {}'.format(pairs_right))
+            # #/*** block 1 ***/
+            FCj = 0
+            # #/*** block 1.1 ***/
+            evfold_dict = self.file_initiator(
+                fpn=simu_seq_len if self.input_kind == "simulate" else fpn,
+                sort_=5,
+            )
+            # #/*** block 1.2 ***/
+            for i in range(len(pairs_left)):
+                # #/*** block 1.2.1 ***/
+                if i % (2 * self.stretch_window) == 0:
+                    FCj += 1
+                if pairs_left[i] is None or pairs_right[i] is None:
+                    list_2d_[FCj - 1].append(0)
+                else:
+                    inf = pairs_left[i]
+                    sup = pairs_right[i]
+                    # print([inf, sup])
+                    list_2d_[FCj - 1].append(evfold_dict[inf][sup])
+        elif mode == "hash_ori":
+            evfold_dict = self.file_initiator(
+                fpn=simu_seq_len if self.input_kind == "simulate" else fpn,
+                sort_=5,
+            )
+            local_pair_ids = self.pairids()
+            # #/*** block 1 ***/
+            for i in range(self.num_pairs):
+                # #/*** block 1.1 ***/
+                for j in range(2 * self.stretch_window):
+                    inf = local_pair_ids[i][j][0]
+                    sup = local_pair_ids[i][j][1]
+                    if inf is None or sup is None:
+                        list_2d_[i].append(0)
+                    else:
+                        list_2d_[i].append(evfold_dict[inf][sup])
+        elif mode == "hash":
+            evfold_dict = self.file_initiator(
+                fpn=simu_seq_len if self.input_kind == "simulate" else fpn,
+                sort_=5,
+            )
+            # #/*** block 1 ***/
+            for i in range(self.num_pairs):
+                # #/*** block 1.1 ***/
+                t1 = self.combo2x2(self.window_m_ids[i][0])
+                # print(self.window_m_ids[i][0])
+                # print(self.combo2x2(self.window_m_ids[i][0]))
+                for l1 in t1:
+                    if l1[0] is not None and l1[1] is None:
+                        list_2d_[i].append(0)
+                    elif l1[0] is None and l1[1] is not None:
+                        list_2d_[i].append(0)
+                    elif l1[0] is not None and l1[1] is not None:
+                        if l1[0] < l1[1]:
+                            list_2d_[i].append(evfold_dict[l1[0]][l1[1]])
+                        else:
+                            list_2d_[i].append(evfold_dict[l1[1]][l1[0]])
+                    else:
+                        list_2d_[i].append(0)
+                # #/*** block 1.2 ***/
+                t2 = self.combo2x2(self.window_m_ids[i][1])
+                for l2 in t2:
+                    if l2[0] is not None and l2[1] is None:
+                        list_2d_[i].append(0)
+                    elif l2[0] is None and l2[1] is not None:
+                        list_2d_[i].append(0)
+                    elif l2[0] is not None and l2[1] is not None:
+                        if l2[0] < l2[1]:
+                            list_2d_[i].append(evfold_dict[l2[0]][l2[1]])
+                        else:
+                            list_2d_[i].append(evfold_dict[l2[1]][l2[0]])
+                    else:
+                        list_2d_[i].append(0)
+        elif mode == "pandas":
+            evfold_df = self.file_initiator(
+                fpn=simu_seq_len if self.input_kind == "simulate" else fpn,
+                is_sort=True,
+                sort_=3,
+            )
+            evfold_df = evfold_df.set_index(["id_1", "id_2"])
+            # #/*** block 1 ***/
+            for i in range(self.num_pairs):
+                # #/*** block 1.1 ***/
+                t1 = self.combo2x2(self.window_m_ids[i][0])
+                for l1 in t1:
+                    if l1[0] is not None and l1[1] is None:
+                        list_2d_[i].append(0)
+                    elif l1[0] is None and l1[1] is not None:
+                        list_2d_[i].append(0)
+                    elif l1[0] is not None and l1[1] is not None:
+                        if l1[0] < l1[1]:
+                            # print(evfold_df.at[(l1[0], l1[1]), 'score'])
+                            list_2d_[i].append(evfold_df.at[(l1[0], l1[1]), "score"])
+                        else:
+                            # print(evfold_df.at[(l1[1], l1[0]), 'score'])
+                            list_2d_[i].append(evfold_df.at[(l1[1], l1[0]), "score"])
+                    else:
+                        list_2d_[i].append(0)
+                # #/*** block 1.2 ***/
+                t2 = self.combo2x2(self.window_m_ids[i][1])
+                for l2 in t2:
+                    if l2[0] is not None and l2[1] is None:
+                        list_2d_[i].append(0)
+                    elif l2[0] is None and l2[1] is not None:
+                        list_2d_[i].append(0)
+                    elif l2[0] is not None and l2[1] is not None:
+                        if l2[0] < l2[1]:
+                            list_2d_[i].append(evfold_df.at[(l2[0], l2[1]), "score"])
+                        else:
+                            list_2d_[i].append(evfold_df.at[(l2[1], l2[0]), "score"])
+                    else:
+                        list_2d_[i].append(0)
+        elif mode == "numpy":
+            evfold_df = self.file_initiator(
+                fpn=simu_seq_len if self.input_kind == "simulate" else fpn,
+                is_sort=True,
+                sort_=3,
+            )
+            evfold_np = np.array(evfold_df).T
+            # #/*** block 1 ***/
+            for i in range(self.num_pairs):
+                # #/*** block 1.1 ***/
+                t1 = self.combo2x2(self.window_m_ids[i][0])
+                for l1 in t1:
+                    if l1[0] is not None and l1[1] is None:
+                        list_2d_[i].append(0)
+                    elif l1[0] is None and l1[1] is not None:
+                        list_2d_[i].append(0)
+                    elif l1[0] is not None and l1[1] is not None:
+                        if l1[0] < l1[1]:
+                            list_2d_[i].append(
+                                evfold_np[2][
+                                    (evfold_np[0] == l1[0]) & (evfold_np[1] == l1[1])
+                                ][0]
+                            )
+                        else:
+                            list_2d_[i].append(
+                                evfold_np[2][
+                                    (evfold_np[0] == l1[1]) & (evfold_np[1] == l1[0])
+                                ][0]
+                            )
+                    else:
+                        list_2d_[i].append(0)
+                # #/*** block 1.2 ***/
+                t2 = self.combo2x2(self.window_m_ids[i][1])
+                for l2 in t2:
+                    if l2[0] is not None and l2[1] is None:
+                        list_2d_[i].append(0)
+                    elif l2[0] is None and l2[1] is not None:
+                        list_2d_[i].append(0)
+                    elif l2[0] is not None and l2[1] is not None:
+                        if l2[0] < l2[1]:
+                            list_2d_[i].append(
+                                evfold_np[2][
+                                    (evfold_np[0] == l2[0]) & (evfold_np[1] == l2[1])
+                                ][0]
+                            )
+                        else:
+                            list_2d_[i].append(
+                                evfold_np[2][
+                                    (evfold_np[0] == l2[1]) & (evfold_np[1] == l2[0])
+                                ][0]
+                            )
+                    else:
+                        list_2d_[i].append(0)
+        print(
+            "======>unipartite pair assignment: {time}s.".format(
+                time=time.time() - start_time
+            )
+        )
+        return list_2d_
```

### Comparing `tmkit-0.0.2/tmkit/seqnetrr/net/Reader.py` & `tmkit-0.0.3/tmkit/seqnetrr/net/Reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,49 +3,49 @@
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
 import numpy as np
 import pandas as pd
-from tmkit.util.Reader import reader as pfrreader
-from tmkit.util.Writer import writer as pfwwriter
-from tmkit.seqnetrr.combo.Separation import separation as ppssep
-from tmkit.seqnetrr.ComputLib import computLib
 
+from tmkit.seqnetrr.combo.Separation import Separation as ppssep
+from tmkit.seqnetrr.ComputLib import ComputLib
+from tmkit.util.Reader import Reader as pfrreader
+from tmkit.util.Writer import Writer as pfwwriter
 
-class reader:
 
+class Reader:
     def __init__(self, seq_sep_inferior=None, seq_sep_superior=None):
         self.__sort_ = -1
         self.seq_sep_inferior = seq_sep_inferior
         self.seq_sep_superior = seq_sep_superior
         self.pfrreader = pfrreader()
         self.pfwwriter = pfwwriter()
-        self.computlib = computLib()
+        self.computlib = ComputLib()
 
     @property
     def sort_(self):
         return self.__sort_
 
     @sort_.setter
     def sort_(self, value):
-        print('Please note that you are attempting externally.')
+        print("Please note that you are attempting externally.")
         if value > 7 or value < 0:
             raise ValueError(
-                '`sort_` has yet to reach there.',
-                '| 1: return results for entire-chain residue contacts.',
-                '| 2: return results of residue contacts by given pairs of interest.',
-                '| 3: return sorted results by `score`',
-                '| 4: return sorted results by `id_1` and `id_2`',
-                '| 5: return dict results of a predictor',
-                '| 6: return results of a residue of a predictor',
-                '| 7: return cumulative dict results of a predictor',
-                '| else: return raw results of a predictor',
-                '| beyond: you need to choose one of opts above.',
+                "`sort_` has yet to reach there.",
+                "| 1: return results for entire-chain residue contacts.",
+                "| 2: return results of residue contacts by given pairs of interest.",
+                "| 3: return sorted results by `score`",
+                "| 4: return sorted results by `id_1` and `id_2`",
+                "| 5: return dict results of a predictor",
+                "| 6: return results of a residue of a predictor",
+                "| 7: return cumulative dict results of a predictor",
+                "| else: return raw results of a predictor",
+                "| beyond: you need to choose one of opts above.",
             )
         else:
             self.__sort_ = value
 
     def sort_1(self, recombine, dist_df):
         """
         ..  @description
@@ -61,39 +61,39 @@
         :param dist_df: a df of distances of residue pairs
         :param is_sort: False or True
         :return:
         """
         dists_ = dist_df
         recombine_ = recombine
         len_recombine_ = recombine_.shape[0]
-        dists_['fasta_id_1'] = dists_['fasta_id_1'].astype(np.int)
-        dists_['fasta_id_2'] = dists_['fasta_id_2'].astype(np.int)
+        dists_["fasta_id_1"] = dists_["fasta_id_1"].astype(np.int)
+        dists_["fasta_id_2"] = dists_["fasta_id_2"].astype(np.int)
         dists__ = pd.DataFrame()
-        dists__[0] = dists_['fasta_id_1']
-        dists__[1] = dists_['fasta_id_2']
+        dists__[0] = dists_["fasta_id_1"]
+        dists__[1] = dists_["fasta_id_2"]
         dists__[2] = dists_.index.values
         dist_dict = self.todict(dists__)
         dist_ids = []
         for i in range(len_recombine_):
-            id_1 = recombine_['id_1'][i]
-            id_2 = recombine_['id_2'][i]
+            id_1 = recombine_["id_1"][i]
+            id_2 = recombine_["id_2"][i]
             # print(id_1, id_2)
             # ### /* block 3.2 */ ###
             dist_id = dist_dict[id_1][id_2]
             dist_ids.append(dist_id)
         recombine_dist = dists_.iloc[dist_ids]
         recombine_dist.columns = [
-            'fasta_id_1',
-            'aa_1',
-            'pdb_id_1',
-            'fasta_id_2',
-            'aa_2',
-            'pdb_id_2',
-            'dist',
-            'is_contact'
+            "fasta_id_1",
+            "aa_1",
+            "pdb_id_1",
+            "fasta_id_2",
+            "aa_2",
+            "pdb_id_2",
+            "dist",
+            "is_contact",
         ]
         recombine_dist = recombine_dist.reset_index(inplace=False, drop=True)
         return recombine_, recombine_dist
 
     def sort_2(self, recombine, dist_df, pair_df):
         """
         ..  @description
@@ -130,23 +130,23 @@
         dists_ = dist_df
         pair_df_ = pair_df
         pair_df_[2] = 0
         # print(pair_df_)
         # #/*** block 2 ***/
         # #/*** block 2.1 ***/
         predicts__ = pd.DataFrame()
-        predicts__[0] = predicts_['id_1']
-        predicts__[1] = predicts_['id_2']
+        predicts__[0] = predicts_["id_1"]
+        predicts__[1] = predicts_["id_2"]
         predicts__[2] = predicts_.index.values
         predict_dict = self.todict(predicts__)
         # print(predict_dict)
         # #/*** block 2.2 ***/
         dists__ = pd.DataFrame()
-        dists__[0] = dists_['fasta_id_1']
-        dists__[1] = dists_['fasta_id_2']
+        dists__[0] = dists_["fasta_id_1"]
+        dists__[1] = dists_["fasta_id_2"]
         dists__[2] = dists_.index.values
         dist_dict = self.todict(dists__)
         # print(dist_dict)
         # #/*** block 3 ***/
         pred_ids = []
         dist_ids = []
         len_pairs = pair_df_.shape[0]
@@ -160,36 +160,34 @@
                 # #/*** block 3.2 ***/
                 dist_id = dist_dict[id_1][id_2]
                 dist_ids.append(dist_id)
             except KeyError:
                 continue
         # #/*** block 4 ***/
         recombine_pred = predicts_.iloc[pred_ids]
-        recombine_pred.columns = [
-            'id_1',
-            'id_2',
-            'score'
-        ]
+        recombine_pred.columns = ["id_1", "id_2", "score"]
         recombine_pred = recombine_pred.reset_index(inplace=False, drop=True)
         # #/*** block 5 ***/
         recombine_dist = dists_.iloc[dist_ids]
         recombine_dist.columns = [
-            'fasta_id_1',
-            'aa_1',
-            'pdb_id_1',
-            'fasta_id_2',
-            'aa_2',
-            'pdb_id_2',
-            'dist',
-            'is_contact',
+            "fasta_id_1",
+            "aa_1",
+            "pdb_id_1",
+            "fasta_id_2",
+            "aa_2",
+            "pdb_id_2",
+            "dist",
+            "is_contact",
         ]
         recombine_dist = recombine_dist.reset_index(inplace=False, drop=True)
         return recombine_pred, recombine_dist
 
-    def sort_3(self, recombine, is_sort=False, is_uniform=False, uniform_df=None, indicator=0):
+    def sort_3(
+        self, recombine, is_sort=False, is_uniform=False, uniform_df=None, indicator=0
+    ):
         """
         ..  @description:
             -------------
             select data by specifying seq_sep_inferior and seq_sep_superior.
             The select data can be sorted by two ways:
             1.  'score'
             2.  'id_1' and 'id_2'
@@ -211,42 +209,35 @@
                 id_1 = uniform_list[i][0]
                 id_2 = uniform_list[i][1]
                 try:
                     uniform_list[i][2] = predict_dict[id_1][id_2]
                 except KeyError:
                     continue
             recombine_ = pd.DataFrame(uniform_list)
-            recombine_.columns = [
-                'id_1',
-                'id_2',
-                'score'
-            ]
+            recombine_.columns = ["id_1", "id_2", "score"]
             # print(recombine_)
             # self.pfwwriter.generic(recombine_, sv_fpn='./cheer')
         # # /*** block 2 ***/
         recombine_ = ppssep(
             df=recombine_,
-            first='id_1',
-            second='id_2',
-            target='score',
+            first="id_1",
+            second="id_2",
+            target="score",
             seq_sep_inferior=self.seq_sep_inferior,
             seq_sep_superior=self.seq_sep_superior,
-            is_sort=is_sort
+            is_sort=is_sort,
         ).extract()
         return recombine_
 
     def sort_6(self, recombine, id, L):
         recombine_ = recombine
-        constraint_1 = (recombine_['id_1'] == id)
+        constraint_1 = recombine_["id_1"] == id
         query = constraint_1
         recombine_ = recombine_.loc[query]
-        recombine_ = recombine_.sort_values(
-            by=['score'],
-            ascending=False
-        ).iloc[0: L, :]
+        recombine_ = recombine_.sort_values(by=["score"], ascending=False).iloc[0:L, :]
         return recombine_
 
     def cumulative(self, recombine, L, len_seq):
         """
         ..  @summary:
             ---------
             sort_6 calculates cummulative eca values.
@@ -255,68 +246,57 @@
         :param num:
         :param L:
         :return:
         """
         recombine_ = recombine
         cumu_dict = dict()
         for i in range(len_seq):
-            recombine_cumu = self.sort_6(recombine_, id=i+1, L=L)
-            cumu_dict[i+1] = self.addition(recombine_cumu)
+            recombine_cumu = self.sort_6(recombine_, id=i + 1, L=L)
+            cumu_dict[i + 1] = self.addition(recombine_cumu)
         return cumu_dict
 
     def addition(self, recombine):
         recombine_ = recombine
-        cumu = recombine_['score'].sum()
+        cumu = recombine_["score"].sum()
         return cumu
 
     def todict(self, recombine):
         arr_2d = recombine.values.tolist()
         # print(arr_2d)
         dicts = self.computlib.tactic1(arr_2d)
         return dicts
 
-    def mi(self, fpn, dist_df=None, pair_list=None, sort_=0, is_sort=False, id=0, L=50, len_seq=50):
+    def mi(
+        self,
+        fpn,
+        dist_df=None,
+        pair_list=None,
+        sort_=0,
+        is_sort=False,
+        id=0,
+        L=50,
+        len_seq=50,
+    ):
         self.__sort_ = sort_
-        results = self.pfrreader.generic(
-            fpn,
-            df_sep='\s+',
-            is_utf8=True
-        )
-        results.columns = [
-            'id_1',
-            'aa_1',
-            'id_2',
-            'aa_2',
-            'score',
-            'FC_score'
-        ]
-        recombine = results[[
-            'id_1',
-            'id_2',
-            'score'
-        ]]
+        results = self.pfrreader.generic(fpn, df_sep=r"\s+", is_utf8=True)
+        results.columns = ["id_1", "aa_1", "id_2", "aa_2", "score", "FC_score"]
+        recombine = results[["id_1", "id_2", "score"]]
         if self.__sort_ == 1:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             recombine = self.sort_3(
-                recombine,
-                is_sort=is_sort,
-                is_uniform=True,
-                uniform_df=pair_df
+                recombine, is_sort=is_sort, is_uniform=True, uniform_df=pair_df
             )
             dist_mi, dist_true = self.sort_1(recombine, dist_df)
             return dist_mi, dist_true
         elif self.__sort_ == 2:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             recombine = self.sort_3(
-                recombine,
-                is_sort=is_sort,
-                is_uniform=True,
-                uniform_df=pair_df
+                recombine, is_sort=is_sort, is_uniform=True, uniform_df=pair_df
             )
             dist_mi, dist_true = self.sort_2(recombine, dist_df, pair_df)
             # dist_mi.to_csv('3rvy_helices.txt', sep='\t', header=None, index=False)
             # print(len(dist_mi), len(dist_true))
             return dist_mi, dist_true
         elif self.__sort_ == 3:
             recombine = self.sort_3(recombine, is_sort=is_sort)
@@ -334,53 +314,42 @@
             cumu_dict = self.cumulative(recombine, L=L, len_seq=len_seq)
             return cumu_dict
         elif self.__sort_ == 8:
             pass
         else:
             return recombine
 
-    def freecontact(self, fpn, dist_df=None, pair_list=None, sort_=0, is_sort=False, id=0, L=50, len_seq=50):
+    def freecontact(
+        self,
+        fpn,
+        dist_df=None,
+        pair_list=None,
+        sort_=0,
+        is_sort=False,
+        id=0,
+        L=50,
+        len_seq=50,
+    ):
         self.__sort_ = sort_
-        results = self.pfrreader.generic(
-            fpn,
-            df_sep='\s+',
-            is_utf8=True
-        )
-        results.columns = [
-            'id_1',
-            'aa_1',
-            'id_2',
-            'aa_2',
-            'MI_score',
-            'score'
-        ]
-        recombine = results[[
-            'id_1',
-            'id_2',
-            'score'
-        ]]
+        results = self.pfrreader.generic(fpn, df_sep=r"\s+", is_utf8=True)
+        results.columns = ["id_1", "aa_1", "id_2", "aa_2", "MI_score", "score"]
+        recombine = results[["id_1", "id_2", "score"]]
         if self.__sort_ == 1:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             recombine = self.sort_3(
-                recombine,
-                is_sort=is_sort,
-                is_uniform=True,
-                uniform_df=pair_df
+                recombine, is_sort=is_sort, is_uniform=True, uniform_df=pair_df
             )
             dist_fc, dist_true = self.sort_1(recombine, dist_df)
             return dist_fc, dist_true
         elif self.__sort_ == 2:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             recombine = self.sort_3(
-                recombine,
-                is_sort=is_sort,
-                is_uniform=True,
-                uniform_df=pair_df
+                recombine, is_sort=is_sort, is_uniform=True, uniform_df=pair_df
             )
             dist_fc, dist_true = self.sort_2(recombine, dist_df, pair_df)
             # dist_fc.to_csv('3rvy_helices.txt', sep='\t', header=None, index=False)
             # print(len(dist_fc), len(dist_true))
             return dist_fc, dist_true
         elif self.__sort_ == 3:
             recombine = self.sort_3(recombine, is_sort=is_sort)
@@ -398,46 +367,41 @@
             cumu_dict = self.cumulative(recombine, L=L, len_seq=len_seq)
             return cumu_dict
         elif self.__sort_ == 8:
             pass
         else:
             return recombine
 
-    def ccmpred(self, fpn, dist_df=None, pair_list=None, sort_=0, is_sort=False, id=0, L=50, len_seq=50):
+    def ccmpred(
+        self,
+        fpn,
+        dist_df=None,
+        pair_list=None,
+        sort_=0,
+        is_sort=False,
+        id=0,
+        L=50,
+        len_seq=50,
+    ):
         self.__sort_ = sort_
-        file_results = self.pfrreader.generic(
-            fpn,
-            df_sep='\s+',
-            is_utf8=True
-        )
+        file_results = self.pfrreader.generic(fpn, df_sep=r"\s+", is_utf8=True)
         results = []
         for i, row in file_results.iterrows():
             for j in range(file_results.shape[1]):
                 if i < j:
                     # print(i+1, j+1, row[j])
-                    results.append([i+1, j+1, row[j]])
+                    results.append([i + 1, j + 1, row[j]])
         results = pd.DataFrame(results)
-        results.columns = [
-            'id_1',
-            'id_2',
-            'score'
-        ]
-        recombine = results[[
-            'id_1',
-            'id_2',
-            'score'
-        ]]
+        results.columns = ["id_1", "id_2", "score"]
+        recombine = results[["id_1", "id_2", "score"]]
         if self.__sort_ == 1:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             recombine = self.sort_3(
-                recombine,
-                is_sort=is_sort,
-                is_uniform=True,
-                uniform_df=pair_df
+                recombine, is_sort=is_sort, is_uniform=True, uniform_df=pair_df
             )
             dist_cp, dist_true = self.sort_1(recombine, dist_df)
             return dist_cp, dist_true
         elif self.__sort_ == 2:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             print(recombine.shape)
@@ -463,50 +427,42 @@
             cumu_dict = self.cumulative(recombine, L=L, len_seq=len_seq)
             return cumu_dict
         elif self.__sort_ == 8:
             pass
         else:
             return recombine
 
-    def gdca(self, fpn, dist_df=None, pair_list=None, sort_=0, is_sort=False, id=0, L=50, len_seq=50):
+    def gdca(
+        self,
+        fpn,
+        dist_df=None,
+        pair_list=None,
+        sort_=0,
+        is_sort=False,
+        id=0,
+        L=50,
+        len_seq=50,
+    ):
         self.__sort_ = sort_
-        results = self.pfrreader.generic(
-            fpn,
-            df_sep='\s+',
-            is_utf8=True
-        )
-        results.columns = [
-            'id_1',
-            'id_2',
-            'score'
-        ]
-        recombine = results[[
-            'id_1',
-            'id_2',
-            'score'
-        ]]
+        results = self.pfrreader.generic(fpn, df_sep=r"\s+", is_utf8=True)
+        results.columns = ["id_1", "id_2", "score"]
+        recombine = results[["id_1", "id_2", "score"]]
         if self.__sort_ == 1:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             recombine = self.sort_3(
-                recombine,
-                is_sort=is_sort,
-                is_uniform=True,
-                uniform_df=pair_df
+                recombine, is_sort=is_sort, is_uniform=True, uniform_df=pair_df
             )
             dist_gdca, dist_true = self.sort_1(recombine, dist_df)
             return dist_gdca, dist_true
         elif self.__sort_ == 2:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             recombine = self.sort_3(
-                recombine,
-                is_sort=is_sort,
-                is_uniform=True,
-                uniform_df=pair_df
+                recombine, is_sort=is_sort, is_uniform=True, uniform_df=pair_df
             )
             dist_gdca, dist_true = self.sort_2(recombine, dist_df, pair_df)
             # dist_gdca.to_csv('3rvy_helices.txt', sep='\t', header=None, index=False)
             # print(len(dist_gdca), len(dist_true))
             return dist_gdca, dist_true
         elif self.__sort_ == 3:
             recombine = self.sort_3(recombine, is_sort=is_sort)
@@ -524,53 +480,42 @@
             cumu_dict = self.cumulative(recombine, L=L, len_seq=len_seq)
             return cumu_dict
         elif self.__sort_ == 8:
             pass
         else:
             return recombine
 
-    def plmc(self, fpn, dist_df=None, pair_list=None, sort_=0, is_sort=False, id=0, L=50, len_seq=50):
+    def plmc(
+        self,
+        fpn,
+        dist_df=None,
+        pair_list=None,
+        sort_=0,
+        is_sort=False,
+        id=0,
+        L=50,
+        len_seq=50,
+    ):
         self.__sort_ = sort_
-        results = self.pfrreader.generic(
-            fpn,
-            df_sep='\s+',
-            is_utf8=True
-        )
-        results.columns = [
-            'id_1',
-            'aa_1',
-            'id_2',
-            'aa_2',
-            'placeholder',
-            'score'
-        ]
-        recombine = results[[
-            'id_1',
-            'id_2',
-            'score'
-        ]]
+        results = self.pfrreader.generic(fpn, df_sep=r"\s+", is_utf8=True)
+        results.columns = ["id_1", "aa_1", "id_2", "aa_2", "placeholder", "score"]
+        recombine = results[["id_1", "id_2", "score"]]
         if self.__sort_ == 1:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             recombine = self.sort_3(
-                recombine,
-                is_sort=is_sort,
-                is_uniform=True,
-                uniform_df=pair_df
+                recombine, is_sort=is_sort, is_uniform=True, uniform_df=pair_df
             )
             dist_plmc, dist_true = self.sort_1(recombine, dist_df)
             return dist_plmc, dist_true
         elif self.__sort_ == 2:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             recombine = self.sort_3(
-                recombine,
-                is_sort=is_sort,
-                is_uniform=True,
-                uniform_df=pair_df
+                recombine, is_sort=is_sort, is_uniform=True, uniform_df=pair_df
             )
             dist_plmc, dist_true = self.sort_2(recombine, dist_df, pair_df)
             # dist_plmc.to_csv('3rvy_helices.txt', sep='\t', header=None, index=False)
             # print(len(dist_plmc), len(dist_true))
             return dist_plmc, dist_true
         elif self.__sort_ == 3:
             recombine = self.sort_3(recombine, is_sort=is_sort)
@@ -588,50 +533,42 @@
             cumu_dict = self.cumulative(recombine, L=L, len_seq=len_seq)
             return cumu_dict
         elif self.__sort_ == 8:
             pass
         else:
             return recombine
 
-    def general(self, fpn, dist_df=None, pair_list=None, sort_=0, is_sort=False, id=0, L=50, len_seq=50):
+    def general(
+        self,
+        fpn,
+        dist_df=None,
+        pair_list=None,
+        sort_=0,
+        is_sort=False,
+        id=0,
+        L=50,
+        len_seq=50,
+    ):
         self.__sort_ = sort_
-        results = self.pfrreader.generic(
-            fpn,
-            df_sep='\s+',
-            is_utf8=True
-        )
-        results.columns = [
-            'id_1',
-            'id_2',
-            'score'
-        ]
-        recombine = results[[
-            'id_1',
-            'id_2',
-            'score'
-        ]]
+        results = self.pfrreader.generic(fpn, df_sep=r"\s+", is_utf8=True)
+        results.columns = ["id_1", "id_2", "score"]
+        recombine = results[["id_1", "id_2", "score"]]
         if self.__sort_ == 1:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             recombine = self.sort_3(
-                recombine,
-                is_sort=is_sort,
-                is_uniform=True,
-                uniform_df=pair_df
+                recombine, is_sort=is_sort, is_uniform=True, uniform_df=pair_df
             )
             dist_gdca, dist_true = self.sort_1(recombine, dist_df)
             return dist_gdca, dist_true
         elif self.__sort_ == 2:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             recombine = self.sort_3(
-                recombine,
-                is_sort=is_sort,
-                is_uniform=True,
-                uniform_df=pair_df
+                recombine, is_sort=is_sort, is_uniform=True, uniform_df=pair_df
             )
             dist_gdca, dist_true = self.sort_2(recombine, dist_df, pair_df)
             # dist_gdca.to_csv('3rvy_helices.txt', sep='\t', header=None, index=False)
             # print(len(dist_gdca), len(dist_true))
             return dist_gdca, dist_true
         elif self.__sort_ == 3:
             recombine = self.sort_3(recombine, is_sort=is_sort)
@@ -649,29 +586,41 @@
             cumu_dict = self.cumulative(recombine, L=L, len_seq=len_seq)
             return cumu_dict
         elif self.__sort_ == 8:
             pass
         else:
             return recombine
 
-    def simulate(self, fpn, dist_df=None, pair_list=None, sort_=0, is_sort=False, id=0, L=50, len_seq=50):
+    def simulate(
+        self,
+        fpn,
+        dist_df=None,
+        pair_list=None,
+        sort_=0,
+        is_sort=False,
+        id=0,
+        L=50,
+        len_seq=50,
+    ):
         self.__sort_ = sort_
         simu_seq_len = fpn
         results = pd.DataFrame(self.computlib.numTo3cols(length=simu_seq_len))
         print(results)
         results.columns = [
-            'id_1',
-            'id_2',
-            'score',
+            "id_1",
+            "id_2",
+            "score",
+        ]
+        recombine = results[
+            [
+                "id_1",
+                "id_2",
+                "score",
+            ]
         ]
-        recombine = results[[
-            'id_1',
-            'id_2',
-            'score',
-        ]]
         if self.__sort_ == 1:
             pair_df = pd.DataFrame(pair_list)
             # print(pair_df)
             recombine = self.sort_3(
                 recombine,
                 is_sort=is_sort,
                 is_uniform=True,
@@ -706,8 +655,8 @@
             return recombine
         elif self.__sort_ == 7:
             cumu_dict = self.cumulative(recombine, L=L, len_seq=len_seq)
             return cumu_dict
         elif self.__sort_ == 8:
             pass
         else:
-            return recombine
+            return recombine
```

### Comparing `tmkit-0.0.2/tmkit/seqnetrr/window/Pair.py` & `tmkit-0.0.3/tmkit/seqnetrr/window/Pair.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,130 +1,145 @@
-__author__ = "Jianfeng Sun"
-__version__ = "v1.0"
-__copyright__ = "Copyright 2023"
-__license__ = "GPL v3.0"
-__email__ = "jianfeng.sunmt@gmail.com"
-__maintainer__ = "Jianfeng Sun"
-
-import time
-
-
-class pair:
-    """
-    Methods
-    -------
-        mid(), mname(), bipartite(), make().
-
-    Notes
-    -----
-        window.pair class offers methods to perform a sliding
-        window op for each of central residue pairs for a
-        given sequence.
-
-    """
-
-    def __init__(
-            self,
-            sequence,
-            position,
-            window_size,
-    ):
-        self.sequence = sequence
-        self.m_pairs = position
-        self.window_size = window_size
-        self.len_seq = len(self.sequence)
-        self.num_pairs = len(self.m_pairs)
-
-    def mid(self):
-        """
-        Notes
-        -----
-            mid() gets all of residues around central residues with
-            a window size.
-
-        Methods
-        -------
-            1>. This function generates all residues with a sliding
-                window for m pairs.
-                self.window_size * 4 means all amino acids except for
-                two central amino acids.
-            2>. block 1:
-                --------
-                return [al1, al2, al3, ar1, ar2, ar3, bl1, bl2, bl3,
-                br1, br2, br3] for one pair a and b. Each of 2 central
-                residues is added to the end in each sub-array,
-                respectively.
-                block 2:
-                --------
-                assign None to window_m_ids.
-            3>. array specification:
-                i.  1st dimension includes all pairs being in contact
-                    or not in a protein sequence.
-                ii. 2nd dimension represents one pair, say 2 central
-                    residues, and consists of 2-sub array, each of
-                    which stores all residues windowed by one of 2
-                    residues.
-                iii.3rd dimension will store all residues regulated in
-                    a given window size.
-
-        Returns
-        -------
-            oder number of pairs and name of pairs
-
-        """
-        start_time = time.time()
-        window_m_ids = [[[] for _ in range(2)] for _ in range(self.num_pairs)]
-        # ###/*** block 1 ***/ ###
-        # ###/*** block 1.1 ***/ ###
-        for i in range(self.num_pairs):
-            left = [self.m_pairs[i][0] - (m1_left_id + 1) for m1_left_id in range(self.window_size)]
-            left.reverse()
-            right = [self.m_pairs[i][0] + (m1_right_id + 1) for m1_right_id in range(self.window_size)]
-            window_m_ids[i][0] = window_m_ids[i][0] + left + [self.m_pairs[i][0]] + right
-        # print(window_m_ids)
-        # ###/*** block 1.2 ***/ ###
-        for i in range(self.num_pairs):
-            left = [self.m_pairs[i][3] - (m2_left_id + 1) for m2_left_id in range(self.window_size)]
-            left.reverse()
-            right = [self.m_pairs[i][3] + (m2_right_id + 1) for m2_right_id in range(self.window_size)]
-            window_m_ids[i][1] = window_m_ids[i][1] + left + [self.m_pairs[i][3]] + right
-        # print(window_m_ids)
-        # #/*** block 2 ***/
-        for i in range(self.num_pairs):
-            for j in range(self.window_size * 2 + 1):
-                if window_m_ids[i][0][j] < 1 or window_m_ids[i][0][j] > self.len_seq:
-                    window_m_ids[i][0][j] = None
-                if window_m_ids[i][1][j] < 1 or window_m_ids[i][1][j] > self.len_seq:
-                    window_m_ids[i][1][j] = None
-        end_time = time.time()
-        print('=========>Window molecule generation: {time}s.'.format(time=end_time - start_time))
-        return window_m_ids
-
-    def mname(self, window_m_ids):
-        """
-        Notes
-        -----
-            mname() gets all residues names corresponding to mid().
-
-        Methods
-        -------
-            It will assgin residues in the window with amino acids
-            name and assign residues in the window but beyond the
-            sequence boundary with None.
-
-            What kind of residues and how many residues the window
-            includes, see method mid().
-
-        """
-        num_pairs = len(window_m_ids)
-        window_m_names = [[] for _ in range(num_pairs)]
-        for i in range(self.num_pairs):
-            for j in range(self.window_size * 4):
-                if window_m_ids[i][j] is None:
-                    window_m_names[i].append(None)
-                # print(window_m_names)
-                else:
-                    for k, character in enumerate(self.sequence):
-                        if window_m_ids[i][j] == k + 1:
-                            # print(character)
-                            window_m_names[i].append(character)
-        return window_m_names
+__author__ = "Jianfeng Sun"
+__version__ = "v1.0"
+__copyright__ = "Copyright 2023"
+__license__ = "GPL v3.0"
+__email__ = "jianfeng.sunmt@gmail.com"
+__maintainer__ = "Jianfeng Sun"
+
+import time
+
+
+class Pair:
+    """
+    window.pair class offers methods to perform a sliding
+    window op for each of central residue pairs for a
+    given sequence.
+
+    """
+
+    def __init__(
+        self,
+        sequence,
+        position,
+        window_size,
+    ):
+        self.sequence = sequence
+        self.m_pairs = position
+        self.window_size = window_size
+        self.len_seq = len(self.sequence)
+        self.num_pairs = len(self.m_pairs)
+
+    def mid(self):
+        """
+        Gets all of residues around central residues with a window size.
+
+        Methods
+        -------
+            1>. This function generates all residues with a sliding
+                window for m pairs.
+                self.window_size * 4 means all amino acids except for
+                two central amino acids.
+            2>. block 1:
+                --------
+                return [al1, al2, al3, ar1, ar2, ar3, bl1, bl2, bl3,
+                br1, br2, br3] for one pair a and b. Each of 2 central
+                residues is added to the end in each sub-array,
+                respectively.
+                block 2:
+                --------
+                assign None to window_m_ids.
+            3>. array specification:
+                i.  1st dimension includes all pairs being in contact
+                    or not in a protein sequence.
+                ii. 2nd dimension represents one pair, say 2 central
+                    residues, and consists of 2-sub array, each of
+                    which stores all residues windowed by one of 2
+                    residues.
+                iii.3rd dimension will store all residues regulated in
+                    a given window size.
+
+        Returns
+        -------
+        List
+            oder number of pairs and name of pairs.
+
+        """
+        start_time = time.time()
+        window_m_ids = [[[] for _ in range(2)] for _ in range(self.num_pairs)]
+        # ###/*** block 1 ***/ ###
+        # ###/*** block 1.1 ***/ ###
+        for i in range(self.num_pairs):
+            left = [
+                self.m_pairs[i][0] - (m1_left_id + 1)
+                for m1_left_id in range(self.window_size)
+            ]
+            left.reverse()
+            right = [
+                self.m_pairs[i][0] + (m1_right_id + 1)
+                for m1_right_id in range(self.window_size)
+            ]
+            window_m_ids[i][0] = (
+                window_m_ids[i][0] + left + [self.m_pairs[i][0]] + right
+            )
+        # print(window_m_ids)
+        # ###/*** block 1.2 ***/ ###
+        for i in range(self.num_pairs):
+            left = [
+                self.m_pairs[i][3] - (m2_left_id + 1)
+                for m2_left_id in range(self.window_size)
+            ]
+            left.reverse()
+            right = [
+                self.m_pairs[i][3] + (m2_right_id + 1)
+                for m2_right_id in range(self.window_size)
+            ]
+            window_m_ids[i][1] = (
+                window_m_ids[i][1] + left + [self.m_pairs[i][3]] + right
+            )
+        # print(window_m_ids)
+        # #/*** block 2 ***/
+        for i in range(self.num_pairs):
+            for j in range(self.window_size * 2 + 1):
+                if window_m_ids[i][0][j] < 1 or window_m_ids[i][0][j] > self.len_seq:
+                    window_m_ids[i][0][j] = None
+                if window_m_ids[i][1][j] < 1 or window_m_ids[i][1][j] > self.len_seq:
+                    window_m_ids[i][1][j] = None
+        end_time = time.time()
+        print(
+            "=========>Window molecule generation: {time}s.".format(
+                time=end_time - start_time
+            )
+        )
+        return window_m_ids
+
+    def mname(self, window_m_ids):
+        """
+        Gets all residues names corresponding to mid().
+
+        Methods
+        -------
+            It will assgin residues in the window with amino acids
+            name and assign residues in the window but beyond the
+            sequence boundary with None.
+
+            What kind of residues and how many residues the window
+            includes, see method mid().
+
+        Returns
+        -------
+        List
+            name of pairs.
+
+        """
+        num_pairs = len(window_m_ids)
+        window_m_names = [[] for _ in range(num_pairs)]
+        for i in range(self.num_pairs):
+            for j in range(self.window_size * 4):
+                if window_m_ids[i][j] is None:
+                    window_m_names[i].append(None)
+                # print(window_m_names)
+                else:
+                    for k, character in enumerate(self.sequence):
+                        if window_m_ids[i][j] == k + 1:
+                            # print(character)
+                            window_m_names[i].append(character)
+        return window_m_names
```

### Comparing `tmkit-0.0.2/tmkit/sequence/PDB.py` & `tmkit-0.0.3/tmkit/sequence/PDB.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-from tmkit.base import PDB
+from typing import List
 
+from tmkit.base import PDB as bpdb
 
-class pdb(PDB.sequence):
 
-    def __init__(self, pdb_fp, prot_name, seq_chain, file_chain=''):
+class PDB(bpdb.Sequence):
+    def __init__(
+        self, pdb_fp: str, prot_name: str, seq_chain: str, file_chain: str = ""
+    ) -> None:
         """
-
         Parameters
         ----------
-        pdb_fp
+        pdb_fp : str
             structure path
-        prot_name
+        prot_name : str
             structure name
-        file_chain
-            file chain
-        seq_chain
+        file_chain : str, optional
+            file chain, by default ""
+        seq_chain : str
             sequence chain
         """
-        super(pdb, self).__init__(pdb_fp, prot_name, seq_chain, file_chain)
+        super().__init__(pdb_fp, prot_name, seq_chain, file_chain)
 
-    def chain(self):
+    def chain(self) -> str:
         """
+        Get whole protein sequence from a PDB file.
 
         Notes
         -----
-            chain() can function in getting whole protein
-            sequence from a PDB file given. (1). For a PDB
-            file which contains many chains like A, B and C,
-            you can specify a specific chain through parameter
-            seq_chain. (2). For a PDB file which contains only
-            one chain like A, you can specify this chain 'A'
-            through parameter seq_chain. (3). For a PDB file
-            which doesn't contain any chain but the fact that
-            you know it contains A chain in truth, you can
-            specify '' chain through parameter seq_chain. It
-            is worth to mention that this function can also be
-            functional in the case where in each chain you specify
-            the residues are discontinuous, this function can
-            also find all discontinuous residues by a for-loop.
+        chain() can function in getting whole protein
+        sequence from a PDB file given. (1). For a PDB
+        file which contains many chains like A, B and C,
+        you can specify a specific chain through parameter
+        seq_chain. (2). For a PDB file which contains only
+        one chain like A, you can specify this chain 'A'
+        through parameter seq_chain. (3). For a PDB file
+        which doesn't contain any chain but the fact that
+        you know it contains A chain in truth, you can
+        specify '' chain through parameter seq_chain. It
+        is worth to mention that this function can also be
+        functional in the case where in each chain you specify
+        the residues are discontinuous, this function can
+        also find all discontinuous residues by a for-loop.
 
         Returns
         -------
-            a sequence
-
+        str
+            A sequence.
         """
-        seq=[]
+        seq: List[str] = []
         for pp in self.ppb.build_peptides(self.pdb_chain):
-            seq_tmp = str(pp.get_sequence())
-            # print(seq_tmp)
+            seq_tmp: str = str(pp.get_sequence())
             seq.append(seq_tmp)
-        return ''.join(seq)
-
+        return "".join(seq)
```

### Comparing `tmkit-0.0.2/tmkit/topology/TMHMM.py` & `tmkit-0.0.3/tmkit/topology/TMHMM.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
+import linecache
 import os
 import re
 import subprocess
-import linecache
+
 import numpy as np
-from tmkit.sequence import Fasta as sfasta
-from tmkit.util.Reader import reader
-from tmkit.util.Writer import writer
-from tmkit.interface import Topology
 
+from tmkit.interface import Topology
+from tmkit.sequence import Fasta as sfasta
+from tmkit.util.Reader import Reader
+from tmkit.util.Writer import Writer
 
-class tmhmm(Topology.topology):
 
+class TMHMM(Topology.Topology):
     def __init__(
-            self,
+        self,
     ):
-        self.reader = reader()
-        self.writer = writer()
+        self.reader = Reader()
+        self.writer = Writer()
 
     def run(
-            self,
-            fasta_fpn,
-            tmhmm_model_fpn,
-            tag,
-            sv_fpn,
+        self,
+        fasta_fpn,
+        tmhmm_model_fpn,
+        tag,
+        sv_fpn,
     ):
         """
         Notes
         -----
         This is running python inline by installing pip install tmhmm.py.
 
         See Also
@@ -48,34 +49,35 @@
         tag
         sv_fpn
 
         Returns
         -------
 
         """
-        print('===>TMHMM is running python inline...')
+        print("===>TMHMM is running python inline...")
         if sv_fpn is None:
-            raise 'sv_fpn has to be specified'
+            raise "sv_fpn has to be specified"
         import tmhmm as tmhmmpy
+
         annotation, posterior = tmhmmpy.predict(
             sequence=sfasta.get(fasta_fpn=fasta_fpn),
             header=None,
-            model_or_filelike=os.path.dirname(__file__) + '/lib/TMHMM2.0.model',
+            model_or_filelike=os.path.dirname(__file__) + "/lib/TMHMM2.0.model",
             # model_or_filelike=tmhmm_model_fpn,
         )
-        self.writer.save([[tag + '_tmhmm', annotation]], sv_fp=sv_fpn)
+        self.writer.save([[tag + "_tmhmm", annotation]], sv_fp=sv_fpn)
         return annotation
 
     def runLinux(
-            self,
-            fasta_fpn,
-            decodeanhmm,
-            options,
-            modelfile,
-            sv_fpn,
+        self,
+        fasta_fpn,
+        decodeanhmm,
+        options,
+        modelfile,
+        sv_fpn,
     ):
         """
         Notes
         -----
             This is running on Linux using the raw tmhmm executable.
 
         Parameters
@@ -92,24 +94,35 @@
             path to save files
 
         Returns
         -------
             A message string
 
         """
-        print('===>TMHMM is running on Linux...')
-        order = 'cat ' + fasta_fpn + '.fasta | ' + decodeanhmm + ' -f ' + options + ' -modelfile ' + modelfile + ' -noPrintSeq -noPrintScores -noPrintID -noPrintStat > ' + sv_fpn
+        print("===>TMHMM is running on Linux...")
+        order = (
+            "cat "
+            + fasta_fpn
+            + ".fasta | "
+            + decodeanhmm
+            + " -f "
+            + options
+            + " -modelfile "
+            + modelfile
+            + " -noPrintSeq -noPrintScores -noPrintID -noPrintStat > "
+            + sv_fpn
+        )
         # print(order)
         subprocess.Popen(
             order,
             stderr=subprocess.PIPE,
             stdout=subprocess.PIPE,
             shell=True,
         ).communicate()
-        return 'finished.'
+        return "finished."
 
     def extract(self, arr_2d):
         """
         Notes
         -----
         Extract topologies.
 
@@ -144,35 +157,35 @@
         """
         length = len(arr_2d)
         tm_lower, tm_upper = [], []
         cyto_lower, cyto_upper = [], []
         extra_lower, extra_upper = [], []
         rest_lower, rest_upper = [], []
         for i in range(length):
-            if arr_2d[i][0] == 'M':
+            if arr_2d[i][0] == "M":
                 tm_lower.append(arr_2d[i][1])
                 tm_upper.append(arr_2d[i][2])
-            elif arr_2d[i][0] == 'i':
+            elif arr_2d[i][0] == "i":
                 cyto_lower.append(arr_2d[i][1])
                 cyto_upper.append(arr_2d[i][2])
-            elif arr_2d[i][0] == 'o':
+            elif arr_2d[i][0] == "o":
                 extra_lower.append(arr_2d[i][1])
                 extra_upper.append(arr_2d[i][2])
             else:
                 rest_lower.append(arr_2d[i][1])
                 rest_upper.append(arr_2d[i][2])
         tmhmm_dict = {
-            'cyto_lower': cyto_lower,
-            'cyto_upper': cyto_upper,
-            'tmh_lower': tm_lower,
-            'tmh_upper': tm_upper,
-            'extra_lower': extra_lower,
-            'extra_upper': extra_upper,
-            'rest_lower': rest_lower,
-            'rest_upper': rest_upper,
+            "cyto_lower": cyto_lower,
+            "cyto_upper": cyto_upper,
+            "tmh_lower": tm_lower,
+            "tmh_upper": tm_upper,
+            "extra_lower": extra_lower,
+            "extra_upper": extra_upper,
+            "rest_lower": rest_lower,
+            "rest_upper": rest_upper,
         }
         return tmhmm_dict
 
     @classmethod
     def formatFromLinux(cls, tmhmm_fpn):
         """
         Notes
@@ -190,24 +203,24 @@
 
         """
         if not os.path.exists(tmhmm_fpn):
             raise FileNotFoundError
         # lines = linecache.getlines(tmhmm_fpn)
         line = linecache.getline(tmhmm_fpn, 1)
         # print(line)
-        block1 = re.split(r': ', line)
+        block1 = re.split(r": ", line)
         # print(block1)
-        block2 = block1[1].split(', ')
+        block2 = block1[1].split(", ")
         # print(block2)
         length = len(block2)
         arr = []
         for i in range(length):
-            tag = block2[i].split(' ')[0]
-            beg = block2[i].split(' ')[1]
-            end = block2[i].split(' ')[2]
+            tag = block2[i].split(" ")[0]
+            beg = block2[i].split(" ")[1]
+            end = block2[i].split(" ")[2]
             arr.append([tag, int(beg), int(end)])
         return arr
 
     @classmethod
     def formatFromInline(cls, tmhmm_fpn):
         """
         Notes
@@ -227,19 +240,19 @@
         if not os.path.exists(tmhmm_fpn):
             raise FileNotFoundError
         annot = sfasta.get(tmhmm_fpn)
         arr = []
         flag = 1
         for i in range(len(annot)):
             if i + 1 != len(annot):
-                if annot[i] == annot[i+1]:
+                if annot[i] == annot[i + 1]:
                     continue
                 else:
-                    arr.append([annot[i], flag, i+1])
-                    flag = i+2
+                    arr.append([annot[i], flag, i + 1])
+                    flag = i + 2
         arr.append([annot[-1], flag, len(annot)])
         # print(arr)
         return arr
 
     def totmhhcp(self, arr, sv_fpn=None):
         """
         Notes
@@ -258,20 +271,20 @@
             str
 
         """
         helix_orien = []
         for i in arr:
             sub = np.arange(i[1], i[2] + 1)
             for j in range(len(sub)):
-                if i[0] == 'o' or i[0] == 'O':
-                    helix_orien.append('O')
-                elif i[0] == 'i':
-                    helix_orien.append('I')
-                elif i[0] == 'M':
-                    helix_orien.append('H')
+                if i[0] == "o" or i[0] == "O":
+                    helix_orien.append("O")
+                elif i[0] == "i":
+                    helix_orien.append("I")
+                elif i[0] == "M":
+                    helix_orien.append("H")
                 else:
-                    helix_orien.append('U')
+                    helix_orien.append("U")
         trans_helix = "".join(helix_orien)
         if sv_fpn:
-            with open(sv_fpn, 'w') as f:
+            with open(sv_fpn, "w") as f:
                 f.write(trans_helix)
-        return trans_helix
+        return trans_helix
```

### Comparing `tmkit-0.0.2/tmkit/topology/lib/Phobius.py` & `tmkit-0.0.3/tmkit/topology/lib/Phobius.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.2/tmkit/util/Console.py` & `tmkit-0.0.3/tmkit/util/Console.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-__version__ = "v1.0"
-__copyright__ = "Copyright 2023"
-__license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
-
-from datetime import datetime
-from pyfiglet import Figlet
-
-
-class console:
-
-    def __init__(self, placeholder='logger: ', verbose=False):
-        self._verbose = verbose
-        self.placeholder = placeholder
-        self.vignette1 = Figlet(font='standard')
-        print(self.vignette1.renderText('TMKit'))
-
-    @property
-    def verbose(self, ):
-        return self._verbose
-
-    @verbose.setter
-    def verbose(self, value):
-        self._verbose = value
-
-    def print(self, content):
-        if self._verbose:
-            now = datetime.now()
-            dt_format = now.strftime("%d/%m/%Y %H:%M:%S ")
-            print(dt_format + self.placeholder + str(content))
-
-    def check(self, content):
-        if self._verbose:
-            print(content)
+__author__ = "Jianfeng Sun"
+__version__ = "v1.0"
+__copyright__ = "Copyright 2023"
+__license__ = "GPL v3.0"
+__email__ = "jianfeng.sunmt@gmail.com"
+__maintainer__ = "Jianfeng Sun"
+
+from datetime import datetime
+from pyfiglet import Figlet
+
+
+class console:
+
+    def __init__(self, placeholder='logger: ', verbose=False):
+        self._verbose = verbose
+        self.placeholder = placeholder
+        self.vignette1 = Figlet(font='standard')
+        print(self.vignette1.renderText('TMKit'))
+
+    @property
+    def verbose(self, ):
+        return self._verbose
+
+    @verbose.setter
+    def verbose(self, value):
+        self._verbose = value
+
+    def print(self, content):
+        if self._verbose:
+            now = datetime.now()
+            dt_format = now.strftime("%d/%m/%Y %H:%M:%S ")
+            print(dt_format + self.placeholder + str(content))
+
+    def check(self, content):
+        if self._verbose:
+            print(content)
```

### Comparing `tmkit-0.0.2/tmkit/visualize/component/focal_blur.py` & `tmkit-0.0.3/tmkit/visualize/component/focal_blur.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from __future__ import print_function
-from pymol import cmd
-from tempfile import mkdtemp
+from math import cos, pi, sin, sqrt
 from shutil import rmtree
-from math import sin, cos, pi, sqrt
+from tempfile import mkdtemp
+
 from PIL import Image
+from pymol import cmd
 
 
-def FocalBlur(
-        tmpdir,
-        aperture=2.0, samples=10, ray=0, width=0, height=0):
-    '''
+def FocalBlur(tmpdir, aperture=2.0, samples=10, ray=0, width=0, height=0):
+    """
     DESCRIPTION
 
         Creates fancy figures by introducing a focal blur to the image. The object
         at the origin will be in focus.
 
     AUTHOR
 
@@ -27,55 +25,58 @@
 
         FocalBlur aperture=float, samples=int, ray=0/1, width=int, height=int
 
     EXAMPELS
 
         FocalBlur aperture=1, samples=100
         FocalBlur aperture=2, samples=100, ray=1, width=600, height=400
-    '''
+    """
 
     # Formalize the parameter types
-    ray = (ray in ("True", "true", 1, "1"))
+    ray = ray in ("True", "true", 1, "1")
     aperture, samples = float(aperture), int(samples)
     width, height = int(width), int(height)
 
     # Create a temporary directory
     # tmpdir = mkdtemp()
     tmpdir = "./"
     print(tmpdir)
 
     # Get the orientation of the protein and the light
-    light = cmd.get('light')[1:-1]
-    light = [float(s) for s in light.split(',')]
+    light = cmd.get("light")[1:-1]
+    light = [float(s) for s in light.split(",")]
     view = cmd.get_view()
 
     # Rotate the protein and the light in order to create the blur
     for frame in range(samples):
         # Angles to rotate protein and light
         # Populate angles as Fermat's spiral
         theta = frame * pi * 110.0 / 144.0
         radius = 0.5 * aperture * sqrt(frame / float(samples - 1))
         x = cos(theta) * radius
         y = sin(theta) * radius
         xr = x / 180.0 * pi
         yr = y / 180.0 * pi
 
         # Rotate the protein
-        cmd.turn('x', x)
-        cmd.turn('y', y)
+        cmd.turn("x", x)
+        cmd.turn("y", y)
 
         # Rotate the light
         ly = light[1] * cos(xr) - light[2] * sin(xr)
         lz = light[2] * cos(xr) + light[1] * sin(xr)
         lx = light[0] * cos(yr) + lz * sin(yr)
         lz = lz * cos(yr) - lx * sin(yr)
-        cmd.set('light', [lx, ly, lz])
+        cmd.set("light", [lx, ly, lz])
 
         curFile = "%s/frame-%04d.png" % (tmpdir, frame)
-        print("Created frame %i/%i (%0.0f%%)" % (frame + 1, samples, 100 * (frame + 1) / samples))
+        print(
+            "Created frame %i/%i (%0.0f%%)"
+            % (frame + 1, samples, 100 * (frame + 1) / samples)
+        )
 
         # Save the image to temporary directory
         if ray:
             cmd.ray(width, height)
             cmd.png(curFile)
         else:
             cmd.png(curFile, quiet=1)
@@ -83,18 +84,19 @@
         # Create the average/blured image
         try:
             avg = Image.blend(avg, Image.open(curFile), 1.0 / (frame + 1))
         except:
             avg = Image.open(curFile)
 
         # Return the protein and the light to the original orientation
-        cmd.set('light', light)
+        cmd.set("light", light)
         cmd.set_view(view)
 
     # Load the blured image
-    avg.save('%s/avg.png' % (tmpdir))
-    cmd.load('%s/avg.png' % (tmpdir))
+    avg.save("%s/avg.png" % (tmpdir))
+    cmd.load("%s/avg.png" % (tmpdir))
 
     # Delete the temporary files
     # rmtree(tmpdir)
 
-cmd.extend('FocalBlur', FocalBlur)
+
+cmd.extend("FocalBlur", FocalBlur)
```

### Comparing `tmkit-0.0.2/tmkit/visualize/component/palette/data2bfactor.py` & `tmkit-0.0.3/tmkit/visualize/component/palette/data2bfactor.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,31 +12,34 @@
 contains the functions
    data2b_atom(mol='',data_file='')
    data2b_res(mol='',data_file='')
    data2q_atom(mol='',data_file='')
    data2q_res(mol='',data_file='')
 """
 
-import sys, re
+import re
+import sys
+
 from pymol import stored
 
-comment = re.compile('^\s*$|^\s*#')
+comment = re.compile(r"^\s*$|^\s*#")
+
 
 def atom_data_extract(data_file):
     """
     Read the specified 'by-atom' data file and extract the data from it
     and store it in parallel dictionaries specifying the data
     and residue names (both with keys of chain and residue number and atom name).
     The data file can contain comment lines starting with "#" (on lines by themselves).
     These comment lines are ignored.
     """
     bdat = {}
-    chain = ''
+    chain = ""
 
-    data_lines = open(data_file, 'r')
+    data_lines = open(data_file)
     # data_lines = open(data_file, 'rU')
     count = 0
 
     for line in data_lines:
         # ignore comment lines (beginning with a '#') or blank lines
         if not comment.match(line):
             words = line.split()
@@ -44,16 +47,16 @@
 
             # check number of columns of data
             if len(words) >= 5:
                 chain = words[0]
                 resi = words[1]
                 resn = words[2]
                 name = words[3]
-                if chain == '-':
-                    chain = ''
+                if chain == "-":
+                    chain = ""
                 ID = None
                 data = float(words[4])
             elif len(words) == 4:
                 resi = words[0]
                 resn = words[1]
                 name = words[2]
                 ID = None
@@ -62,231 +65,255 @@
                 # ptraj `atominfluct` output use ID and data
                 resi = None
                 resn = None
                 name = None
                 ID = int(words[0])
                 data = float(words[1])
             else:
-                sys.stderr.write("\nError in reading data files -- check number of columns.\n")
-                sys.stderr.write("Number of columns: %d  on line number %d\n" % (len(words),count))
+                sys.stderr.write(
+                    "\nError in reading data files -- check number of columns.\n"
+                )
+                sys.stderr.write(
+                    "Number of columns: %d  on line number %d\n" % (len(words), count)
+                )
                 sys.exit(1)
 
             if ID is None:
                 bdat.setdefault(chain, {}).setdefault(resi, {})[name] = (data, resn)
             else:
                 # it seem `resn` is not used in anywhere
-                bdat.setdefault(chain, {})[ID] = (data, '')
+                bdat.setdefault(chain, {})[ID] = (data, "")
 
     return bdat
 
+
 def residue_data_extract(data_file):
     """
     Read the specified 'by-residue' data file and extract the data from it
     and store it in parallel dictionaries specifying the data
     and residue names (both with keys of chain and residue number).
     The data file can contain comment lines starting with "#" (on lines by themselves).
     These comment lines are ignored.
     """
     bdat = {}
-    chain = ''
+    chain = ""
 
-    data_lines = open(data_file, 'r')
+    data_lines = open(data_file)
     # data_lines = open(data_file, 'rU')
     count = 0
 
     for line in data_lines:
         # ignore comment lines (beginning with a '#') or blank lines
         if not comment.match(line):
             words = line.split()
             count += 1
 
             # check number of columns of data
             if len(words) >= 4:
                 chain = words[0]
                 resi = words[1]
                 resn = words[2]
-                if chain == '-':
-                    chain = ''
+                if chain == "-":
+                    chain = ""
                 data = float(words[3])
             elif len(words) == 3:
                 resi = words[0]
                 resn = words[1]
                 data = float(words[2])
             elif len(words) == 2:
                 resi = words[0]
                 data = float(words[1])
-                resn = ''
+                resn = ""
             else:
-                sys.stderr.write("\nError in reading data files -- check number of columns.\n")
-                sys.stderr.write("Number of columns: %d  on line number %d\n" % (len(words),count))
+                sys.stderr.write(
+                    "\nError in reading data files -- check number of columns.\n"
+                )
+                sys.stderr.write(
+                    "Number of columns: %d  on line number %d\n" % (len(words), count)
+                )
                 sys.exit(1)
 
             bdat.setdefault(chain, {})[resi] = (data, resn)
 
     return bdat
 
+
 ###########################################################################################
 # for testing purposes:
 # if calling this as a program on its own, read the data_file name from
 # the command line and run residue_data_extract on it. (does not require
 # importing cmd from pymol
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     data_file_name = sys.argv[1]
     b_dict = residue_data_extract(data_file_name)
     for chain in sorted(b_dict):
         for resi in sorted(b_dict[chain]):
             b, resn = b_dict[chain][resi]
-            print("b-factors %s %s %s %s  new B='%s'" % (pdb_file, chain, resn, resi, b))
+            print(
+                "b-factors %s %s %s %s  new B='%s'" % (pdb_file, chain, resn, resi, b)
+            )
     sys.exit()
 
 
 ###########################################################################################
 # PyMOL stuff
 
 from pymol import cmd
 
-def data2b_atom(mol='', data_file='', property='b', quiet=0):
+
+def data2b_atom(mol="", data_file="", property="b", quiet=0):
     """
-DESCRIPTION
+    DESCRIPTION
 
-    Alters the B-factor data by atom.
+        Alters the B-factor data by atom.
 
-USAGE
+    USAGE
 
-    data2b_atom <mol>, <data_file>
+        data2b_atom <mol>, <data_file>
 
-    where <mol> is the molecular object whose B-factor data you wish to modify
-    and <data_file> is a file contain the data (one value for each atom)
-    The format of <data_file> should be:
+        where <mol> is the molecular object whose B-factor data you wish to modify
+        and <data_file> is a file contain the data (one value for each atom)
+        The format of <data_file> should be:
 
-         chain resi resn name data
-    or
-         resi resn name data
+             chain resi resn name data
+        or
+             resi resn name data
 
-    or
-         ID data
+        or
+             ID data
 
-    (i.e. "chain" is optional if all atoms are in one chain).
-    Lines beginning with '#' are ignored as comments.
+        (i.e. "chain" is optional if all atoms are in one chain).
+        Lines beginning with '#' are ignored as comments.
 
-    Example data lines:
+        Example data lines:
 
-      A ALA 1 N 3.5
-      A ALA 1 CA 3.0
-      A ALA 1 CB 3.14159
-      A ALA 1 C  6.23
-      A ALA 1 O    5.1
-      A GLY 2 N 10.3
-      A GLY 2 CA 1.714
-      A GLY 2 C -0.05
-      A GLY 2 O -3.12
+          A ALA 1 N 3.5
+          A ALA 1 CA 3.0
+          A ALA 1 CB 3.14159
+          A ALA 1 C  6.23
+          A ALA 1 O    5.1
+          A GLY 2 N 10.3
+          A GLY 2 CA 1.714
+          A GLY 2 C -0.05
+          A GLY 2 O -3.12
 
-SEE ALSO
+    SEE ALSO
 
-    data2b_res, data2q_atom, data2q_res
+        data2b_res, data2q_atom, data2q_res
     """
 
     b_dict = atom_data_extract(data_file)
     quiet = int(quiet) == 1
 
     def b_lookup(chain, resi, name, ID, b):
         def _lookup(chain, resi, name, ID):
             if resi in b_dict[chain] and isinstance(b_dict[chain][resi], dict):
                 return b_dict[chain][resi][name][0]
             else:
                 # find data by ID
                 return b_dict[chain][int(ID)][0]
+
         try:
             if not chain in b_dict:
-                chain = ''
+                chain = ""
             b = _lookup(chain, resi, name, ID)
-            if not quiet: print('///%s/%s/%s new: %f' % (chain, resi, name, b))
+            if not quiet:
+                print("///%s/%s/%s new: %f" % (chain, resi, name, b))
         except KeyError:
-            if not quiet: print('///%s/%s/%s keeping: %f' % (chain, resi, name, b))
+            if not quiet:
+                print("///%s/%s/%s keeping: %f" % (chain, resi, name, b))
         return b
+
     stored.b = b_lookup
 
-    cmd.alter(mol, '%s=stored.b(chain, resi, name, ID, %s)' % (property, property))
+    cmd.alter(mol, "%s=stored.b(chain, resi, name, ID, %s)" % (property, property))
     cmd.rebuild()
 
-def data2b_res(mol='', data_file='', property='b', quiet=0):
+
+def data2b_res(mol="", data_file="", property="b", quiet=0):
     """
-DESCRIPTION
+    DESCRIPTION
 
-    Alters the B-factor data by residue.
+        Alters the B-factor data by residue.
 
-USAGE
+    USAGE
 
-    data2b_res <mol>, <data_file>
+        data2b_res <mol>, <data_file>
 
-    where <mol> is the molecular object whose B-factor data you wish to modify
-    and <data_file> is a file contain the data (one value for each residue)
-    The format of <data_file> should be:
+        where <mol> is the molecular object whose B-factor data you wish to modify
+        and <data_file> is a file contain the data (one value for each residue)
+        The format of <data_file> should be:
 
-         chain resi resn data
-    or
-         resi resn data
-    or
-         resi data
+             chain resi resn data
+        or
+             resi resn data
+        or
+             resi data
 
-    (i.e. "chain" is optional). Lines beginning with '#' are ignored as comments.
+        (i.e. "chain" is optional). Lines beginning with '#' are ignored as comments.
 
-SEE ALSO
+    SEE ALSO
 
-    data2b_atom, data2q_atom, data2q_res
+        data2b_atom, data2q_atom, data2q_res
     """
 
     b_dict = residue_data_extract(data_file)
     quiet = int(quiet) == 1
 
     def b_lookup(chain, resi, name, b):
         try:
             if chain in b_dict:
                 b = b_dict[chain][resi][0]
             else:
-                b = b_dict[''][resi][0]
-            if not quiet: print('///%s/%s/%s new: %f' % (chain, resi, name, b))
+                b = b_dict[""][resi][0]
+            if not quiet:
+                print("///%s/%s/%s new: %f" % (chain, resi, name, b))
         except KeyError:
-            if not quiet: print('///%s/%s/%s keeping: %f' % (chain, resi, name, b))
+            if not quiet:
+                print("///%s/%s/%s keeping: %f" % (chain, resi, name, b))
         return b
+
     stored.b = b_lookup
 
-    cmd.alter(mol, '%s=stored.b(chain, resi, name, %s)' % (property, property))
+    cmd.alter(mol, "%s=stored.b(chain, resi, name, %s)" % (property, property))
     cmd.rebuild()
 
-def data2q_atom(mol='',data_file=''):
+
+def data2q_atom(mol="", data_file=""):
     """
-DESCRIPTION
+    DESCRIPTION
 
-    Alters the occupancy data by atom.
+        Alters the occupancy data by atom.
 
-USAGE
+    USAGE
 
-    See data2b_atom
+        See data2b_atom
 
-SEE ALSO
+    SEE ALSO
 
-    data2q_res, data2b_atom, data2b_res
+        data2q_res, data2b_atom, data2b_res
     """
-    data2b_atom(mol, data_file, property='q')
+    data2b_atom(mol, data_file, property="q")
+
 
-def data2q_res(mol='',data_file=''):
+def data2q_res(mol="", data_file=""):
     """
-DESCRIPTION
+    DESCRIPTION
 
-    Alters the occupancy data by residue.
+        Alters the occupancy data by residue.
 
-USAGE
+    USAGE
 
-    See data2b_res
+        See data2b_res
 
-SEE ALSO
+    SEE ALSO
 
-    data2q_atom, data2b_atom, data2b_res
+        data2q_atom, data2b_atom, data2b_res
     """
-    data2b_res(mol, data_file, property='q')
+    data2b_res(mol, data_file, property="q")
+
 
-cmd.extend('data2b_res',data2b_res)
-cmd.extend('data2b_atom',data2b_atom)
-cmd.extend('data2q_res',data2q_res)
-cmd.extend('data2q_atom',data2q_atom)
+cmd.extend("data2b_res", data2b_res)
+cmd.extend("data2b_atom", data2b_atom)
+cmd.extend("data2q_res", data2q_res)
+cmd.extend("data2q_atom", data2q_atom)
```

### Comparing `tmkit-0.0.2/tmkit/visualize/component/palette/spectrumany.py` & `tmkit-0.0.3/tmkit/visualize/component/palette/spectrumany.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,88 +1,92 @@
-'''
+"""
 http://pymolwiki.org/index.php/spectrumany
 
 (c) 2010 Thomas Holder
 
 License: BSD-2-Clause
-'''
+"""
 
-from __future__ import print_function
 
 from pymol import cmd, stored
 
-expression_sc = cmd.Shortcut([
-    'count',
-    'resi',
-    'b',
-    'q',
-    'pc',
-])
+expression_sc = cmd.Shortcut(
+    [
+        "count",
+        "resi",
+        "b",
+        "q",
+        "pc",
+    ]
+)
 
 
-def spectrumany(expression, color_list, selection='(all)', minimum=None, maximum=None, quiet=1):
-    '''
-DESCRIPTION
+def spectrumany(
+    expression, color_list, selection="(all)", minimum=None, maximum=None, quiet=1
+):
+    """
+    DESCRIPTION
 
-    Define a color spectrum with as many color-stops as you like (at least 2).
+        Define a color spectrum with as many color-stops as you like (at least 2).
 
-USAGE
+    USAGE
 
-    spectrumany expression, color_list [, selection [, minimum [, maximum ]]]
+        spectrumany expression, color_list [, selection [, minimum [, maximum ]]]
 
-ARGUMENTS
+    ARGUMENTS
 
-    expression = count, resi, b, q, or pc: respectively, atom count, residue
-    index, temperature factor, occupancy, or partial charge {default: count}
+        expression = count, resi, b, q, or pc: respectively, atom count, residue
+        index, temperature factor, occupancy, or partial charge {default: count}
 
-    color_list = string: Space separated list of colors
+        color_list = string: Space separated list of colors
 
-    ... all other arguments like with `spectrum` command
+        ... all other arguments like with `spectrum` command
 
-EXAMPLE
+    EXAMPLE
 
-    spectrumany count, forest green yellow white
-    spectrumany b, red yellow white, (polymer), maximum=100.0
+        spectrumany count, forest green yellow white
+        spectrumany b, red yellow white, (polymer), maximum=100.0
 
-SEE ALSO
+    SEE ALSO
 
-    spectrum
-    '''
+        spectrum
+    """
     quiet = int(quiet)
     colors = color_list.split()
     if len(colors) < 2:
-        print('failed! please provide at least 2 colors')
+        print("failed! please provide at least 2 colors")
         return
 
     colvec = [cmd.get_color_tuple(i) for i in colors]
     print(colvec)
     parts = len(colvec) - 1
 
-    expression = {'pc': 'partial_charge', 'fc': 'formal_charge',
-                  'count': 'index'}.get(expression, expression)
-    minmax_expr = {'resi': 'resv'}.get(expression, expression)
-    discrete_expr = ['index', 'resi']
+    expression = {"pc": "partial_charge", "fc": "formal_charge", "count": "index"}.get(
+        expression, expression
+    )
+    minmax_expr = {"resi": "resv"}.get(expression, expression)
+    discrete_expr = ["index", "resi"]
 
     if cmd.count_atoms(selection) == 0:
-        print('empty selection')
+        print("empty selection")
         return
 
     if None in [minimum, maximum]:
         stored.e = list()
-        cmd.iterate(selection, 'stored.e.append(%s)' % (minmax_expr))
+        cmd.iterate(selection, "stored.e.append(%s)" % (minmax_expr))
         if minimum is None:
             minimum = min(stored.e)
         if maximum is None:
             maximum = max(stored.e)
     minimum, maximum = float(minimum), float(maximum)
     if not quiet:
-        print(' Spectrum: range (%.5f to %.5f)' % (minimum, maximum))
+        print(" Spectrum: range (%.5f to %.5f)" % (minimum, maximum))
 
     if maximum == minimum:
-        print('no spectrum possible, only equal %s values' % (expression))
+        print("no spectrum possible, only equal %s values" % (expression))
         return
 
     if expression in discrete_expr:
         val_range = int(maximum - minimum + 1)
     else:
         val_range = maximum - minimum
         cmd.color(colors[0], selection)
@@ -91,27 +95,39 @@
     steps = 60 // parts
     steps_total = steps * parts
 
     val_start = minimum
     for p in range(parts):
         for i in range(steps):
             ii = float(i) / steps
-            col_list = [colvec[p + 1][j] * ii + colvec[p][j] * (1.0 - ii) for j in range(3)]
+            col_list = [
+                colvec[p + 1][j] * ii + colvec[p][j] * (1.0 - ii) for j in range(3)
+            ]
             # print(col_list)
             # ### /*** the line below is where I modified sth. ***/
-            col_name = '0x%02x%02x%02x' % (int(col_list[0] * 255), int(col_list[1] * 255), int(col_list[2] * 255))
+            col_name = "0x%02x%02x%02x" % (
+                int(col_list[0] * 255),
+                int(col_list[1] * 255),
+                int(col_list[2] * 255),
+            )
             # col_name = '0x%02x%02x%02x' % (col_list[0] * 255, col_list[1] * 255, col_list[2] * 255)
             val_end = val_range * (i + 1 + p * steps) / steps_total + minimum
             if expression in discrete_expr:
-                cmd.color(col_name, '(%s) and %s %d-%d' % (selection, expression, val_start, val_end))
+                cmd.color(
+                    col_name,
+                    "(%s) and %s %d-%d" % (selection, expression, val_start, val_end),
+                )
             else:
-                cmd.color(col_name, '(%s) and %s > %f' % (selection, expression, val_start))
+                cmd.color(
+                    col_name, "(%s) and %s > %f" % (selection, expression, val_start)
+                )
             val_start = val_end
 
-cmd.extend('spectrumany', spectrumany)
+
+cmd.extend("spectrumany", spectrumany)
 
 # tab-completion of arguments
-cmd.auto_arg[0]['spectrumany'] = [expression_sc, 'expression', ', ']
-cmd.auto_arg[1]['spectrumany'] = [cmd.auto_arg[0]['color'][0], 'color', ' ']
-cmd.auto_arg[2]['spectrumany'] = cmd.auto_arg[2]['spectrum']
+cmd.auto_arg[0]["spectrumany"] = [expression_sc, "expression", ", "]
+cmd.auto_arg[1]["spectrumany"] = [cmd.auto_arg[0]["color"][0], "color", " "]
+cmd.auto_arg[2]["spectrumany"] = cmd.auto_arg[2]["spectrum"]
 
 # vi:expandtab:smarttab
```

### Comparing `tmkit-0.0.2/tmkit/visualize/component/show_contacts.py` & `tmkit-0.0.3/tmkit/visualize/component/show_contacts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,297 +1,333 @@
 #!/usr/bin/python
 
-'''PyMOL plugin that provides show_contacts command and GUI
+"""PyMOL plugin that provides show_contacts command and GUI
 for highlighting good and bad polar contacts. Factored out of 
 clustermols by Matthew Baumgartner.
 The advantage of this package is it requires many fewer dependencies.
-'''
-from __future__ import print_function
+"""
+
+import os
+import sys
 
-import sys, os
 from pymol import cmd
 
-DEBUG=1
+DEBUG = 1
 
 
-def show_contacts(selection, selection2, result="contacts", cutoff=3.6, bigcutoff=4.0, SC_DEBUG = DEBUG):
+def show_contacts(
+    selection, selection2, result="contacts", cutoff=3.6, bigcutoff=4.0, SC_DEBUG=DEBUG
+):
     """
     USAGE
 
     show_contacts selection, selection2, [result=contacts],[cutoff=3.6],[bigcutoff=4.0]
 
     Show various polar contacts, the good, the bad, and the ugly.
 
     Edit MPB 6-26-14: The distances are heavy atom distances, so I upped the default cutoff to 4.0
-    
+
     Returns:
     True/False -  if False, something went wrong
     """
     if SC_DEBUG > 4:
-        print('Starting show_contacts')
+        print("Starting show_contacts")
         print('selection = "' + selection + '"')
         print('selection2 = "' + selection2 + '"')
-            
+
     result = cmd.get_legal_name(result)
 
-    #if the group of contacts already exist, delete them
+    # if the group of contacts already exist, delete them
     cmd.delete(result)
 
     # ensure only N and O atoms are in the selection
     all_don_acc1 = selection + " and (donor or acceptor)"
     all_don_acc2 = selection2 + " and  (donor or acceptor)"
-    
+
     if SC_DEBUG > 4:
         print('all_don_acc1 = "' + all_don_acc1 + '"')
         print('all_don_acc2 = "' + all_don_acc2 + '"')
-    
-    #if theses selections turn out not to have any atoms in them, pymol throws cryptic errors when calling the dist function like:
+
+    # if theses selections turn out not to have any atoms in them, pymol throws cryptic errors when calling the dist function like:
     #'Selector-Error: Invalid selection name'
-    #So for each one, manually perform the selection and then pass the reference to the distance command and at the end, clean up the selections
-    #the return values are the count of the number of atoms
-    all1_sele_count = cmd.select('all_don_acc1_sele', all_don_acc1)
-    all2_sele_count = cmd.select('all_don_acc2_sele', all_don_acc2)
-    
-    #print out some warnings
+    # So for each one, manually perform the selection and then pass the reference to the distance command and at the end, clean up the selections
+    # the return values are the count of the number of atoms
+    all1_sele_count = cmd.select("all_don_acc1_sele", all_don_acc1)
+    all2_sele_count = cmd.select("all_don_acc2_sele", all_don_acc2)
+
+    # print out some warnings
     if DEBUG > 3:
         if not all1_sele_count:
-            print('Warning: all_don_acc1 selection empty!')
+            print("Warning: all_don_acc1 selection empty!")
         if not all2_sele_count:
-            print('Warning: all_don_acc2 selection empty!')
-    
+            print("Warning: all_don_acc2 selection empty!")
+
     ########################################
     allres = result + "_all"
     if all1_sele_count and all2_sele_count:
-        cmd.distance(allres, 'all_don_acc1_sele', 'all_don_acc2_sele', bigcutoff, mode = 0)
+        cmd.distance(
+            allres, "all_don_acc1_sele", "all_don_acc2_sele", bigcutoff, mode=0
+        )
         cmd.set("dash_radius", "0.05", allres)
         cmd.set("dash_color", "purple", allres)
         cmd.hide("labels", allres)
-    
+
     ########################################
-    #compute good polar interactions according to pymol
+    # compute good polar interactions according to pymol
     polres = result + "_polar"
     if all1_sele_count and all2_sele_count:
-        cmd.distance(polres, 'all_don_acc1_sele', 'all_don_acc2_sele', cutoff, mode = 2) #hopefully this checks angles? Yes
-        cmd.set("dash_radius","0.126",polres)
-    
+        cmd.distance(
+            polres, "all_don_acc1_sele", "all_don_acc2_sele", cutoff, mode=2
+        )  # hopefully this checks angles? Yes
+        cmd.set("dash_radius", "0.126", polres)
+
     ########################################
-    #When running distance in mode=2, the cutoff parameter is ignored if set higher then the default of 3.6
-    #so set it to the passed in cutoff and change it back when you are done.
-    old_h_bond_cutoff_center = cmd.get('h_bond_cutoff_center') # ideal geometry
-    old_h_bond_cutoff_edge = cmd.get('h_bond_cutoff_edge') # minimally acceptable geometry
-    cmd.set('h_bond_cutoff_center', bigcutoff)
-    cmd.set('h_bond_cutoff_edge', bigcutoff)
-        
-    #compute possibly suboptimal polar interactions using the user specified distance
+    # When running distance in mode=2, the cutoff parameter is ignored if set higher then the default of 3.6
+    # so set it to the passed in cutoff and change it back when you are done.
+    old_h_bond_cutoff_center = cmd.get("h_bond_cutoff_center")  # ideal geometry
+    old_h_bond_cutoff_edge = cmd.get(
+        "h_bond_cutoff_edge"
+    )  # minimally acceptable geometry
+    cmd.set("h_bond_cutoff_center", bigcutoff)
+    cmd.set("h_bond_cutoff_edge", bigcutoff)
+
+    # compute possibly suboptimal polar interactions using the user specified distance
     pol_ok_res = result + "_polar_ok"
     if all1_sele_count and all2_sele_count:
-        cmd.distance(pol_ok_res, 'all_don_acc1_sele', 'all_don_acc2_sele', bigcutoff, mode = 2) 
+        cmd.distance(
+            pol_ok_res, "all_don_acc1_sele", "all_don_acc2_sele", bigcutoff, mode=2
+        )
         cmd.set("dash_radius", "0.06", pol_ok_res)
 
-    #now reset the h_bond cutoffs
-    cmd.set('h_bond_cutoff_center', old_h_bond_cutoff_center)
-    cmd.set('h_bond_cutoff_edge', old_h_bond_cutoff_edge) 
-    
-    
+    # now reset the h_bond cutoffs
+    cmd.set("h_bond_cutoff_center", old_h_bond_cutoff_center)
+    cmd.set("h_bond_cutoff_edge", old_h_bond_cutoff_edge)
+
     ########################################
-    
+
     onlyacceptors1 = selection + " and (acceptor and !donor)"
     onlyacceptors2 = selection2 + " and (acceptor and !donor)"
     onlydonors1 = selection + " and (!acceptor and donor)"
-    onlydonors2 = selection2 + " and (!acceptor and donor)"  
-    
-    #perform the selections
-    onlyacceptors1_sele_count = cmd.select('onlyacceptors1_sele', onlyacceptors1)
-    onlyacceptors2_sele_count = cmd.select('onlyacceptors2_sele', onlyacceptors2)
-    onlydonors1_sele_count = cmd.select('onlydonors1_sele', onlydonors1)
-    onlydonors2_sele_count = cmd.select('onlydonors2_sele', onlydonors2)    
-    
-    #print out some warnings
+    onlydonors2 = selection2 + " and (!acceptor and donor)"
+
+    # perform the selections
+    onlyacceptors1_sele_count = cmd.select("onlyacceptors1_sele", onlyacceptors1)
+    onlyacceptors2_sele_count = cmd.select("onlyacceptors2_sele", onlyacceptors2)
+    onlydonors1_sele_count = cmd.select("onlydonors1_sele", onlydonors1)
+    onlydonors2_sele_count = cmd.select("onlydonors2_sele", onlydonors2)
+
+    # print out some warnings
     if SC_DEBUG > 2:
         if not onlyacceptors1_sele_count:
-            print('Warning: onlyacceptors1 selection empty!')
+            print("Warning: onlyacceptors1 selection empty!")
         if not onlyacceptors2_sele_count:
-            print('Warning: onlyacceptors2 selection empty!')
+            print("Warning: onlyacceptors2 selection empty!")
         if not onlydonors1_sele_count:
-            print('Warning: onlydonors1 selection empty!')
+            print("Warning: onlydonors1 selection empty!")
         if not onlydonors2_sele_count:
-            print('Warning: onlydonors2 selection empty!')    
-            
-    
-    accres = result+"_aa"
+            print("Warning: onlydonors2 selection empty!")
+
+    accres = result + "_aa"
     if onlyacceptors1_sele_count and onlyacceptors2_sele_count:
-        aa_dist_out = cmd.distance(accres, 'onlyacceptors1_sele', 'onlyacceptors2_sele', cutoff, 0)
+        aa_dist_out = cmd.distance(
+            accres, "onlyacceptors1_sele", "onlyacceptors2_sele", cutoff, 0
+        )
 
         if aa_dist_out < 0:
-            print('\n\nCaught a pymol selection error in acceptor-acceptor selection of show_contacts')
-            print('accres:', accres)
-            print('onlyacceptors1', onlyacceptors1)
-            print('onlyacceptors2', onlyacceptors2)
+            print(
+                "\n\nCaught a pymol selection error in acceptor-acceptor selection of show_contacts"
+            )
+            print("accres:", accres)
+            print("onlyacceptors1", onlyacceptors1)
+            print("onlyacceptors2", onlyacceptors2)
             return False
-    
-        cmd.set("dash_color","red",accres)
-        cmd.set("dash_radius","0.125",accres)
-    
+
+        cmd.set("dash_color", "red", accres)
+        cmd.set("dash_radius", "0.125", accres)
+
     ########################################
-    
-    donres = result+"_dd"
+
+    donres = result + "_dd"
     if onlydonors1_sele_count and onlydonors2_sele_count:
-        dd_dist_out = cmd.distance(donres, 'onlydonors1_sele', 'onlydonors2_sele', cutoff, 0)
-        
-        #try to catch the error state 
+        dd_dist_out = cmd.distance(
+            donres, "onlydonors1_sele", "onlydonors2_sele", cutoff, 0
+        )
+
+        # try to catch the error state
         if dd_dist_out < 0:
-            print('\n\nCaught a pymol selection error in dd selection of show_contacts')
-            print('donres:', donres)
-            print('onlydonors1', onlydonors1)
-            print('onlydonors2', onlydonors2)
-            print("cmd.distance('" + donres + "', '" + onlydonors1 + "', '" + onlydonors2 + "', " + str(cutoff) + ", 0)")  
+            print("\n\nCaught a pymol selection error in dd selection of show_contacts")
+            print("donres:", donres)
+            print("onlydonors1", onlydonors1)
+            print("onlydonors2", onlydonors2)
+            print(
+                "cmd.distance('"
+                + donres
+                + "', '"
+                + onlydonors1
+                + "', '"
+                + onlydonors2
+                + "', "
+                + str(cutoff)
+                + ", 0)"
+            )
             return False
-        
-        cmd.set("dash_color","red",donres)  
-        cmd.set("dash_radius","0.125",donres)
-    
+
+        cmd.set("dash_color", "red", donres)
+        cmd.set("dash_radius", "0.125", donres)
+
     ##########################################################
     ##### find the buried unpaired atoms of the receptor #####
     ##########################################################
-    
-    #initialize the variable for when CALC_SASA is False
-    unpaired_atoms = ''
-    
-        
+
+    # initialize the variable for when CALC_SASA is False
+    unpaired_atoms = ""
+
     ## Group
-    cmd.group(result,"%s %s %s %s %s %s" % (polres, allres, accres, donres, pol_ok_res, unpaired_atoms))
-    
+    cmd.group(
+        result,
+        "%s %s %s %s %s %s"
+        % (polres, allres, accres, donres, pol_ok_res, unpaired_atoms),
+    )
+
     ## Clean up the selection objects
-    #if the show_contacts debug level is high enough, don't delete them.
+    # if the show_contacts debug level is high enough, don't delete them.
     if SC_DEBUG < 5:
-        cmd.delete('all_don_acc1_sele')
-        cmd.delete('all_don_acc2_sele')
-        cmd.delete('onlyacceptors1_sele')
-        cmd.delete('onlyacceptors2_sele')
-        cmd.delete('onlydonors1_sele')
-        cmd.delete('onlydonors2_sele')
-    
-    
+        cmd.delete("all_don_acc1_sele")
+        cmd.delete("all_don_acc2_sele")
+        cmd.delete("onlyacceptors1_sele")
+        cmd.delete("onlyacceptors2_sele")
+        cmd.delete("onlydonors1_sele")
+        cmd.delete("onlydonors2_sele")
+
     return True
-cmd.extend('contacts', show_contacts) #contacts to avoid clashing with cluster_mols version
 
 
+cmd.extend(
+    "contacts", show_contacts
+)  # contacts to avoid clashing with cluster_mols version
+
 
-    
-    
 #################################################################################
 ########################### Start of pymol plugin code ##########################
 #################################################################################
 
 
-about_text = '''show_contacts was factored out of the much more full-featured cluster_mols
+about_text = """show_contacts was factored out of the much more full-featured cluster_mols
 by Dr. Matt Baumgartner (https://pymolwiki.org/index.php/Cluster_mols).  It provides
 an easy way to highlight polar contacts (and clashes) between two selections without
 requiring the installation of additional dependencies.
-'''
+"""
+
 
 class Show_Contacts:
-    ''' Tk version of the Plugin GUI '''
+    """Tk version of the Plugin GUI"""
+
     def __init__(self, app):
         parent = app.root
         self.parent = parent
-        
+
         self.app = app
-        
+
         import Pmw
 
         ############################################################################################
         ### Open a window with options to select to loaded objects ###
         ############################################################################################
 
-        self.select_dialog = Pmw.Dialog(parent, 
-                         buttons = ('Ok','Cancel'), 
-                         title = 'Show Contacts Plugin',
-                         command = self.button_pressed )
-    
+        self.select_dialog = Pmw.Dialog(
+            parent,
+            buttons=("Ok", "Cancel"),
+            title="Show Contacts Plugin",
+            command=self.button_pressed,
+        )
+
         self.select_dialog.withdraw()
-    
 
-        #allow the user to select from objects already loaded in pymol
-        self.select_object_combo_box = Pmw.ComboBox(self.select_dialog.interior(),
-                                                               scrolledlist_items=[],
-                                                               labelpos='w',
-                                                               label_text='Select loaded object:',
-                                                               listbox_height = 2,
-                                                               dropdown=True)
-        self.select_object_combo_box2 = Pmw.ComboBox(self.select_dialog.interior(),
-                                                               scrolledlist_items=[],
-                                                               labelpos='w',
-                                                               label_text='Select loaded object:',
-                                                               listbox_height = 2,
-                                                               dropdown=True)                                                               
+        # allow the user to select from objects already loaded in pymol
+        self.select_object_combo_box = Pmw.ComboBox(
+            self.select_dialog.interior(),
+            scrolledlist_items=[],
+            labelpos="w",
+            label_text="Select loaded object:",
+            listbox_height=2,
+            dropdown=True,
+        )
+        self.select_object_combo_box2 = Pmw.ComboBox(
+            self.select_dialog.interior(),
+            scrolledlist_items=[],
+            labelpos="w",
+            label_text="Select loaded object:",
+            listbox_height=2,
+            dropdown=True,
+        )
         self.select_object_combo_box.grid(column=1, row=0)
         self.select_object_combo_box2.grid(column=2, row=0)
         self.populate_ligand_select_list()
         self.select_dialog.show()
-        
 
-      
     def button_pressed(self, result):
-        if hasattr(result,'keycode'):
+        if hasattr(result, "keycode"):
             if result.keycode == 36:
-                print('keycode:', result.keycode)
-        elif result == 'Ok' or result == 'Exit' or result == None:
+                print("keycode:", result.keycode)
+        elif result == "Ok" or result == "Exit" or result == None:
             s1 = self.select_object_combo_box.get()
             s2 = self.select_object_combo_box2.get()
-            show_contacts(s1,s2,'%s_%s'%(s1,s2))
-            self.select_dialog.withdraw()            
-        elif result == 'Cancel' or result == None:
+            show_contacts(s1, s2, f"{s1}_{s2}")
+            self.select_dialog.withdraw()
+        elif result == "Cancel" or result == None:
             self.select_dialog.withdraw()
 
-            
-
-    
     def populate_ligand_select_list(self):
-        ''' Go thourgh the loaded objects in PyMOL and add them to the selected list. '''
-        #get the loaded objects
+        """Go thourgh the loaded objects in PyMOL and add them to the selected list."""
+        # get the loaded objects
         loaded_objects = _get_select_list()
-         
+
         self.select_object_combo_box.clear()
         self.select_object_combo_box2.clear()
-        
+
         for ob in loaded_objects:
-            self.select_object_combo_box.insert('end', ob)
-            self.select_object_combo_box2.insert('end', ob)
-        
+            self.select_object_combo_box.insert("end", ob)
+            self.select_object_combo_box2.insert("end", ob)
+
 
 def _get_select_list():
-    '''
+    """
     Get either a list of object names, or a list of chain selections
-    '''
-    loaded_objects = [name for name in cmd.get_names('all', 1) if '_cluster_' not in name]
+    """
+    loaded_objects = [
+        name for name in cmd.get_names("all", 1) if "_cluster_" not in name
+    ]
 
     # if single object, try chain selections
     if len(loaded_objects) == 1:
         chains = cmd.get_chains(loaded_objects[0])
         if len(chains) > 1:
-            loaded_objects = ['{} & chain {}'.format(loaded_objects[0], chain) for chain in chains]
+            loaded_objects = [
+                f"{loaded_objects[0]} & chain {chain}" for chain in chains
+            ]
 
     return loaded_objects
 
 
 class Show_Contacts_Qt_Dialog:
-    ''' Qt version of the Plugin GUI '''
+    """Qt version of the Plugin GUI"""
+
     def __init__(self):
         from pymol.Qt import QtWidgets
+
         dialog = QtWidgets.QDialog()
         self.setupUi(dialog)
         self.populate_ligand_select_list()
         dialog.accepted.connect(self.accept)
         dialog.exec_()
 
     def accept(self):
         s1 = self.select_object_combo_box.currentText()
         s2 = self.select_object_combo_box2.currentText()
-        show_contacts(s1, s2, '%s_%s' % (s1, s2))
+        show_contacts(s1, s2, f"{s1}_{s2}")
 
     def populate_ligand_select_list(self):
         loaded_objects = _get_select_list()
 
         self.select_object_combo_box.clear()
         self.select_object_combo_box2.clear()
 
@@ -300,40 +336,50 @@
 
         if len(loaded_objects) > 1:
             self.select_object_combo_box2.setCurrentIndex(1)
 
     def setupUi(self, Dialog):
         # Based on auto-generated code from ui file
         from pymol.Qt import QtCore, QtWidgets
+
         Dialog.resize(400, 50)
         self.gridLayout = QtWidgets.QGridLayout(Dialog)
         label = QtWidgets.QLabel("Select loaded object:", Dialog)
         self.gridLayout.addWidget(label, 0, 0, 1, 1)
         self.select_object_combo_box = QtWidgets.QComboBox(Dialog)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
+        sizePolicy = QtWidgets.QSizePolicy(
+            QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed
+        )
         self.select_object_combo_box.setSizePolicy(sizePolicy)
         self.select_object_combo_box.setEditable(True)
         self.gridLayout.addWidget(self.select_object_combo_box, 0, 1, 1, 1)
         label = QtWidgets.QLabel("Select loaded object:", Dialog)
         self.gridLayout.addWidget(label, 1, 0, 1, 1)
         self.select_object_combo_box2 = QtWidgets.QComboBox(Dialog)
         self.select_object_combo_box2.setSizePolicy(sizePolicy)
         self.select_object_combo_box2.setEditable(True)
         self.gridLayout.addWidget(self.select_object_combo_box2, 1, 1, 1, 1)
         self.buttonBox = QtWidgets.QDialogButtonBox(Dialog)
         self.buttonBox.setOrientation(QtCore.Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.Cancel|QtWidgets.QDialogButtonBox.Ok)
+        self.buttonBox.setStandardButtons(
+            QtWidgets.QDialogButtonBox.Cancel | QtWidgets.QDialogButtonBox.Ok
+        )
         self.gridLayout.addWidget(self.buttonBox, 2, 0, 1, 2)
         self.buttonBox.accepted.connect(Dialog.accept)
         self.buttonBox.rejected.connect(Dialog.reject)
 
-    
+
 def __init__(self):
     try:
         from pymol.plugins import addmenuitemqt
-        addmenuitemqt('Show Contacts', Show_Contacts_Qt_Dialog)
+
+        addmenuitemqt("Show Contacts", Show_Contacts_Qt_Dialog)
         return
     except Exception as e:
         print(e)
-    self.menuBar.addmenuitem('Plugin', 'command', 'Show Contacts', label = 'Show Contacts', command = lambda s=self : Show_Contacts(s))  
-        
-
+    self.menuBar.addmenuitem(
+        "Plugin",
+        "command",
+        "Show Contacts",
+        label="Show Contacts",
+        command=lambda s=self: Show_Contacts(s),
+    )
```

### Comparing `tmkit-0.0.2/tmkit/visualize/small/Local.py` & `tmkit-0.0.3/tmkit/visualize/small/Local.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,95 @@
 __author__ = "Jianfeng Sun"
 __version__ = "v1.0"
 __copyright__ = "Copyright 2023"
 __license__ = "GPL v3.0"
 __email__ = "jianfeng.sunmt@gmail.com"
 __maintainer__ = "Jianfeng Sun"
 
-from tmkit.visualize.small.Palette import palette as pppmpalette
-from tmkit.visualize.small.Select import select as pppmselect
-from tmkit.visualize.small.Style import style as pppmstyle
-from tmkit.visualize.small.Label import label as pppmlabel
-from tmkit.chain.PDB import pdb as cpdb
+from typing import List, Tuple
 
 
-class local:
-
+class Local:
     def __init__(
-            self,
-            prot_name,
-            pdb_complex_fp,
-            prot_c,
-            sm_c,
-            sm_rep,
-            nby_rep,
-            pocket_rep='surface',
-    ):
+        self,
+        prot_name: str,
+        pdb_complex_fp: str,
+        prot_c: str,
+        sm_c: str,
+        sm_rep: str,
+        nby_rep: str,
+        pocket_rep: str = "surface",
+    ) -> None:
         """
+        Initialize a local object.
 
         Parameters
         ----------
-        prot_name
-            '6feq',
-        pdb_complex_fp
-            to('data/example/pymol/'),
-        sm_rep
-            "sticks",
-        nby_rep
-            'spheres',
-        prot_c
-            'blue_white_magenta', # 'blue_magenta' rainbow
-        sm_c
-            'blue_green',
+        prot_name : str
+            The name of the protein.
+        pdb_complex_fp : str
+            The filepath of the pdb complex.
+        prot_c : str
+            The color of the protein.
+        sm_c : str
+            The color of the small molecule.
+        sm_rep : str
+            The representation of the small molecule.
+        nby_rep : str
+            The representation of the nearby atoms.
+        pocket_rep : str, optional
+            The representation of the pocket, by default "surface".
         """
-        from pymol import cmd
-        from pymol import finish_launching
-        from pymol import preset
+        from pymol import cmd, finish_launching, preset
+
+        from tmkit.chain.PDB import PDB as cpdb
+        from tmkit.visualize.small.Label import Label as pppmlabel
+        from tmkit.visualize.small.Palette import Palette as pppmpalette
+        from tmkit.visualize.small.Select import Select as pppmselect
+        from tmkit.visualize.small.Style import Style as pppmstyle
+
         finish_launching()
 
         cmd.bg_color(
             color="black"
             # color="white"
         )
 
         chains = cpdb(
             pdb_fp=pdb_complex_fp,
             prot_name=prot_name,
         ).chains()
 
         cmd.load(
-            filename=pdb_complex_fp + prot_name + '.pdb',
+            filename=pdb_complex_fp + prot_name + ".pdb",
         )
 
         sel_op = pppmselect()
         sel_op.chain(chains)
         sel_op.pocket()
 
         pppmpalette(
             chains,
             prot_c=prot_c,
             sm_c=sm_c,
         )
         pppmstyle(
             sm_style=sm_rep,
         )
-        preset.ball_and_stick(selection='sm', mode=1)
-        preset.ligand_sites_mesh(selection='sm')
+        preset.ball_and_stick(selection="sm", mode=1)
+        preset.ligand_sites_mesh(selection="sm")
 
-        cmd.select(
-            name='nby',
-            selection='n. CA and br. all within 5 of organic'
-        )
+        cmd.select(name="nby", selection="n. CA and br. all within 5 of organic")
 
         cmd.show(
-            selection='nby',
+            selection="nby",
             representation=nby_rep,
         )
         cmd.show(
-            selection='pocket',
+            selection="pocket",
             representation=pocket_rep,
         )
-        pppmlabel().putup(select='nby', )
+        pppmlabel().putup(
+            select="nby",
+        )
 
-        cmd.set(name='sphere_scale', value=1.5, selection='nby')
+        cmd.set(name="sphere_scale", value=1.5, selection="nby")
```

### Comparing `tmkit-0.0.2/tmkit.egg-info/SOURCES.txt` & `tmkit-0.0.3/tmkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
+tests/__init__.py
+tests/cath_test.py
+tests/collation_test.py
+tests/conftest.py
+tests/feature_test.py
+tests/mapping_test.py
+tests/mutation_test.py
+tests/residue_contact_test.py
+tests/sequence_test.py
+tests/topology_test.py
+tmkit/.env
 tmkit/Path.py
 tmkit/__init__.py
+tmkit/__main__.py
 tmkit/cath.py
 tmkit/collate.py
 tmkit/edge.py
 tmkit/feature.py
 tmkit/fetch.py
 tmkit/mapping.py
 tmkit/msa.py
@@ -60,14 +73,15 @@
 tmkit/name/__init__.py
 tmkit/position/__init__.py
 tmkit/position/scenario/Segment.py
 tmkit/position/scenario/Separation.py
 tmkit/position/scenario/__init__.py
 tmkit/property/HelixSurface.py
 tmkit/property/__init__.py
+tmkit/property/lips.pl
 tmkit/retrieve/MSA.py
 tmkit/retrieve/PDB.py
 tmkit/retrieve/XML.py
 tmkit/retrieve/__init__.py
 tmkit/seqnetrr/Compare.py
 tmkit/seqnetrr/ComputLib.py
 tmkit/seqnetrr/Controller.py
```


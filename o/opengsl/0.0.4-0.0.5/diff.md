# Comparing `tmp/opengsl-0.0.4.tar.gz` & `tmp/opengsl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengsl-0.0.4.tar", last modified: Wed Jun 14 12:25:16 2023, max compression
+gzip compressed data, was "opengsl-0.0.5.tar", last modified: Mon Jul 10 12:18:27 2023, max compression
```

## Comparing `opengsl-0.0.4.tar` & `opengsl-0.0.5.tar`

### file list

```diff
@@ -1,238 +1,246 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.337691 opengsl-0.0.4/
--rw-rw-rw-   0        0        0     1085 2023-06-14 05:42:30.000000 opengsl-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       32 2023-06-14 11:34:51.000000 opengsl-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2481 2023-06-14 12:25:16.337691 opengsl-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1774 2023-06-14 12:23:14.000000 opengsl-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.166057 opengsl-0.0.4/opengsl/
--rw-rw-rw-   0        0        0     4090 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/ExpManager.py
--rw-rw-rw-   0        0        0      198 2023-06-14 11:34:51.000000 opengsl-0.0.4/opengsl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.161044 opengsl-0.0.4/opengsl/configs/
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.219105 opengsl-0.0.4/opengsl/configs/appnp/
--rw-rw-rw-   0        0        0      508 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/appnp/appnp_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      431 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/appnp/appnp_blogcatalog.yaml
--rw-rw-rw-   0        0        0      439 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/appnp/appnp_citeseer.yaml
--rw-rw-rw-   0        0        0      436 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/appnp/appnp_cora.yaml
--rw-rw-rw-   0        0        0      437 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/appnp/appnp_flickr.yaml
--rw-rw-rw-   0        0        0      355 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/appnp/appnp_hetero.yaml
--rw-rw-rw-   0        0        0      469 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/appnp/appnp_minesweeper.yaml
--rw-rw-rw-   0        0        0      439 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/appnp/appnp_pubmed.yaml
--rw-rw-rw-   0        0        0      466 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/appnp/appnp_questions.yaml
--rw-rw-rw-   0        0        0      468 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/appnp/appnp_roman-empire.yaml
--rw-rw-rw-   0        0        0      502 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/appnp/appnp_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.220123 opengsl-0.0.4/opengsl/configs/cogsl/
--rw-rw-rw-   0        0        0     1274 2023-06-14 10:44:54.000000 opengsl-0.0.4/opengsl/configs/cogsl/cogsl_citeseer.yaml
--rw-rw-rw-   0        0        0     1127 2023-06-14 10:44:54.000000 opengsl-0.0.4/opengsl/configs/cogsl/cogsl_cora.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.225104 opengsl-0.0.4/opengsl/configs/gat/
--rw-rw-rw-   0        0        0      540 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gat/gat_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      471 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gat/gat_blogcatalog.yaml
--rw-rw-rw-   0        0        0      401 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gat/gat_citeseer.yaml
--rw-rw-rw-   0        0        0      401 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gat/gat_cora.yaml
--rw-rw-rw-   0        0        0      471 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gat/gat_flickr.yaml
--rw-rw-rw-   0        0        0      543 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gat/gat_minesweeper.yaml
--rw-rw-rw-   0        0        0      401 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gat/gat_pubmed.yaml
--rw-rw-rw-   0        0        0      543 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gat/gat_questions.yaml
--rw-rw-rw-   0        0        0      541 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gat/gat_roman-empire.yaml
--rw-rw-rw-   0        0        0      542 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gat/gat_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.232071 opengsl-0.0.4/opengsl/configs/gaug/
--rw-rw-rw-   0        0        0     1238 2023-06-14 11:23:13.000000 opengsl-0.0.4/opengsl/configs/gaug/gaug_amazon-ratings.yaml
--rw-rw-rw-   0        0        0     1238 2023-06-14 11:13:54.000000 opengsl-0.0.4/opengsl/configs/gaug/gaug_blogcatalog.yaml
--rw-rw-rw-   0        0        0     1240 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/gaug/gaug_citeseer.yaml
--rw-rw-rw-   0        0        0     1235 2023-06-14 11:13:54.000000 opengsl-0.0.4/opengsl/configs/gaug/gaug_cora.yaml
--rw-rw-rw-   0        0        0     1239 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/gaug/gaug_flickr.yaml
--rw-rw-rw-   0        0        0     1233 2023-06-14 11:20:27.000000 opengsl-0.0.4/opengsl/configs/gaug/gaug_minesweeper.yaml
--rw-rw-rw-   0        0        0     1235 2023-06-14 11:13:54.000000 opengsl-0.0.4/opengsl/configs/gaug/gaug_pubmed.yaml
--rw-rw-rw-   0        0        0     1259 2023-06-14 11:19:40.000000 opengsl-0.0.4/opengsl/configs/gaug/gaug_roman-empire.yaml
--rw-rw-rw-   0        0        0     1231 2023-06-14 11:15:25.000000 opengsl-0.0.4/opengsl/configs/gaug/gaug_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.238072 opengsl-0.0.4/opengsl/configs/gcn/
--rw-rw-rw-   0        0        0      849 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gcn/gcn_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      872 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/gcn/gcn_blogcatalog.yaml
--rw-rw-rw-   0        0        0      851 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/gcn/gcn_citeseer.yaml
--rw-rw-rw-   0        0        0      870 2023-06-14 11:25:20.000000 opengsl-0.0.4/opengsl/configs/gcn/gcn_cora.yaml
--rw-rw-rw-   0        0        0      877 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/gcn/gcn_flickr.yaml
--rw-rw-rw-   0        0        0      849 2023-06-14 08:38:21.000000 opengsl-0.0.4/opengsl/configs/gcn/gcn_minesweeper.yaml
--rw-rw-rw-   0        0        0      851 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/gcn/gcn_pubmed.yaml
--rw-rw-rw-   0        0        0      847 2023-06-14 08:38:21.000000 opengsl-0.0.4/opengsl/configs/gcn/gcn_questions.yaml
--rw-rw-rw-   0        0        0      845 2023-06-14 08:37:12.000000 opengsl-0.0.4/opengsl/configs/gcn/gcn_roman-empire.yaml
--rw-rw-rw-   0        0        0      846 2023-06-14 08:43:47.000000 opengsl-0.0.4/opengsl/configs/gcn/gcn_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.242068 opengsl-0.0.4/opengsl/configs/gen/
--rw-rw-rw-   0        0        0      836 2023-06-14 10:03:38.000000 opengsl-0.0.4/opengsl/configs/gen/gen_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      835 2023-06-14 10:01:50.000000 opengsl-0.0.4/opengsl/configs/gen/gen_blogcatalog.yaml
--rw-rw-rw-   0        0        0      835 2023-06-14 09:59:56.000000 opengsl-0.0.4/opengsl/configs/gen/gen_citeseer.yaml
--rw-rw-rw-   0        0        0      835 2023-06-14 09:59:56.000000 opengsl-0.0.4/opengsl/configs/gen/gen_cora.yaml
--rw-rw-rw-   0        0        0      835 2023-06-14 10:01:50.000000 opengsl-0.0.4/opengsl/configs/gen/gen_flickr.yaml
--rw-rw-rw-   0        0        0      839 2023-06-14 10:04:58.000000 opengsl-0.0.4/opengsl/configs/gen/gen_minesweeper.yaml
--rw-rw-rw-   0        0        0      835 2023-06-14 09:59:56.000000 opengsl-0.0.4/opengsl/configs/gen/gen_pubmed.yaml
--rw-rw-rw-   0        0        0      836 2023-06-14 10:04:58.000000 opengsl-0.0.4/opengsl/configs/gen/gen_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.248583 opengsl-0.0.4/opengsl/configs/gprgnn/
--rw-rw-rw-   0        0        0      430 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gprgnn/gprgnn_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      435 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/gprgnn/gprgnn_blogcatalog.yaml
--rw-rw-rw-   0        0        0      439 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/gprgnn/gprgnn_citeseer.yaml
--rw-rw-rw-   0        0        0      436 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gprgnn/gprgnn_cora.yaml
--rw-rw-rw-   0        0        0      440 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/gprgnn/gprgnn_flickr.yaml
--rw-rw-rw-   0        0        0      398 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gprgnn/gprgnn_minesweeper.yaml
--rw-rw-rw-   0        0        0      439 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/gprgnn/gprgnn_pubmed.yaml
--rw-rw-rw-   0        0        0      395 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gprgnn/gprgnn_questions.yaml
--rw-rw-rw-   0        0        0      397 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gprgnn/gprgnn_roman-empire.yaml
--rw-rw-rw-   0        0        0      398 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/gprgnn/gprgnn_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.255580 opengsl-0.0.4/opengsl/configs/grcn/
--rw-rw-rw-   0        0        0      866 2023-06-14 09:06:14.000000 opengsl-0.0.4/opengsl/configs/grcn/grcn_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      864 2023-06-14 09:03:17.000000 opengsl-0.0.4/opengsl/configs/grcn/grcn_blogcatalog.yaml
--rw-rw-rw-   0        0        0      788 2023-06-14 09:03:17.000000 opengsl-0.0.4/opengsl/configs/grcn/grcn_citeseer.yaml
--rw-rw-rw-   0        0        0      814 2023-06-14 09:03:17.000000 opengsl-0.0.4/opengsl/configs/grcn/grcn_cora.yaml
--rw-rw-rw-   0        0        0      864 2023-06-14 09:03:17.000000 opengsl-0.0.4/opengsl/configs/grcn/grcn_flickr.yaml
--rw-rw-rw-   0        0        0      867 2023-06-14 09:06:14.000000 opengsl-0.0.4/opengsl/configs/grcn/grcn_minesweeper.yaml
--rw-rw-rw-   0        0        0     1233 2023-06-14 09:03:17.000000 opengsl-0.0.4/opengsl/configs/grcn/grcn_pubmed.yaml
--rw-rw-rw-   0        0        0      833 2023-06-14 09:06:14.000000 opengsl-0.0.4/opengsl/configs/grcn/grcn_questions.yaml
--rw-rw-rw-   0        0        0      834 2023-06-14 09:06:15.000000 opengsl-0.0.4/opengsl/configs/grcn/grcn_roman-empire.yaml
--rw-rw-rw-   0        0        0      832 2023-06-14 09:06:14.000000 opengsl-0.0.4/opengsl/configs/grcn/grcn_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.262589 opengsl-0.0.4/opengsl/configs/gt/
--rw-rw-rw-   0        0        0      678 2023-06-14 10:36:05.000000 opengsl-0.0.4/opengsl/configs/gt/gt_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      675 2023-06-14 10:36:05.000000 opengsl-0.0.4/opengsl/configs/gt/gt_blogcatalog.yaml
--rw-rw-rw-   0        0        0      676 2023-06-14 10:30:46.000000 opengsl-0.0.4/opengsl/configs/gt/gt_citeseer.yaml
--rw-rw-rw-   0        0        0      676 2023-06-14 10:30:46.000000 opengsl-0.0.4/opengsl/configs/gt/gt_cora.yaml
--rw-rw-rw-   0        0        0      675 2023-06-14 10:36:05.000000 opengsl-0.0.4/opengsl/configs/gt/gt_flickr.yaml
--rw-rw-rw-   0        0        0      677 2023-06-14 10:36:05.000000 opengsl-0.0.4/opengsl/configs/gt/gt_minesweeper.yaml
--rw-rw-rw-   0        0        0      676 2023-06-14 10:30:46.000000 opengsl-0.0.4/opengsl/configs/gt/gt_pubmed.yaml
--rw-rw-rw-   0        0        0      676 2023-06-14 10:36:05.000000 opengsl-0.0.4/opengsl/configs/gt/gt_questions.yaml
--rw-rw-rw-   0        0        0      677 2023-06-14 10:36:05.000000 opengsl-0.0.4/opengsl/configs/gt/gt_roman-empire.yaml
--rw-rw-rw-   0        0        0      678 2023-06-14 10:36:05.000000 opengsl-0.0.4/opengsl/configs/gt/gt_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.268587 opengsl-0.0.4/opengsl/configs/idgl/
--rw-rw-rw-   0        0        0      761 2023-06-14 11:26:41.000000 opengsl-0.0.4/opengsl/configs/idgl/idgl_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      760 2023-06-14 11:25:20.000000 opengsl-0.0.4/opengsl/configs/idgl/idgl_blogcatalog.yaml
--rw-rw-rw-   0        0        0      728 2023-06-14 11:25:20.000000 opengsl-0.0.4/opengsl/configs/idgl/idgl_citeseer.yaml
--rw-rw-rw-   0        0        0      726 2023-06-14 11:25:20.000000 opengsl-0.0.4/opengsl/configs/idgl/idgl_cora.yaml
--rw-rw-rw-   0        0        0      760 2023-06-14 11:25:20.000000 opengsl-0.0.4/opengsl/configs/idgl/idgl_flickr.yaml
--rw-rw-rw-   0        0        0      783 2023-06-14 11:27:45.000000 opengsl-0.0.4/opengsl/configs/idgl/idgl_minesweeper.yaml
--rw-rw-rw-   0        0        0      726 2023-06-14 11:25:20.000000 opengsl-0.0.4/opengsl/configs/idgl/idgl_pubmed.yaml
--rw-rw-rw-   0        0        0      747 2023-06-14 11:27:45.000000 opengsl-0.0.4/opengsl/configs/idgl/idgl_questions.yaml
--rw-rw-rw-   0        0        0      782 2023-06-14 11:27:02.000000 opengsl-0.0.4/opengsl/configs/idgl/idgl_roman-empire.yaml
--rw-rw-rw-   0        0        0      708 2023-06-14 11:34:05.000000 opengsl-0.0.4/opengsl/configs/idgl/idgl_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.274581 opengsl-0.0.4/opengsl/configs/jknet/
--rw-rw-rw-   0        0        0      851 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/jknet/jknet_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      854 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/jknet/jknet_blogcatalog.yaml
--rw-rw-rw-   0        0        0      859 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/jknet/jknet_citeseer.yaml
--rw-rw-rw-   0        0        0      854 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/jknet/jknet_cora.yaml
--rw-rw-rw-   0        0        0      859 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/jknet/jknet_flickr.yaml
--rw-rw-rw-   0        0        0      820 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/jknet/jknet_minesweeper.yaml
--rw-rw-rw-   0        0        0      860 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/jknet/jknet_pubmed.yaml
--rw-rw-rw-   0        0        0      818 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/jknet/jknet_questions.yaml
--rw-rw-rw-   0        0        0      819 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/jknet/jknet_roman-empire.yaml
--rw-rw-rw-   0        0        0      848 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/jknet/jknet_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.274581 opengsl-0.0.4/opengsl/configs/link/
--rw-rw-rw-   0        0        0      506 2023-06-14 11:23:13.000000 opengsl-0.0.4/opengsl/configs/link/link.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.275579 opengsl-0.0.4/opengsl/configs/lpa/
--rw-rw-rw-   0        0        0      459 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/lpa/lpa.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.281589 opengsl-0.0.4/opengsl/configs/nodeformer/
--rw-rw-rw-   0        0        0      607 2023-06-14 10:37:19.000000 opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      624 2023-06-14 10:36:05.000000 opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_blogcatalog.yaml
--rw-rw-rw-   0        0        0      608 2023-06-14 10:36:05.000000 opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_citeseer.yaml
--rw-rw-rw-   0        0        0      623 2023-06-14 10:36:05.000000 opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_cora.yaml
--rw-rw-rw-   0        0        0      600 2023-06-14 10:37:19.000000 opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_flickr.yaml
--rw-rw-rw-   0        0        0      606 2023-06-14 10:37:19.000000 opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_minesweeper.yaml
--rw-rw-rw-   0        0        0      624 2023-06-14 10:36:05.000000 opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_pubmed.yaml
--rw-rw-rw-   0        0        0      600 2023-06-14 10:37:19.000000 opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_questions.yaml
--rw-rw-rw-   0        0        0      625 2023-06-14 10:37:19.000000 opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_roman-empire.yaml
--rw-rw-rw-   0        0        0      607 2023-06-14 10:37:19.000000 opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.287588 opengsl-0.0.4/opengsl/configs/prognn/
--rw-rw-rw-   0        0        0      818 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/prognn/prognn_blogcatalog.yaml
--rw-rw-rw-   0        0        0      875 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/prognn/prognn_citeseer.yaml
--rw-rw-rw-   0        0        0      853 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/prognn/prognn_cora.yaml
--rw-rw-rw-   0        0        0      818 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/prognn/prognn_flickr.yaml
--rw-rw-rw-   0        0        0      813 2023-06-14 08:50:23.000000 opengsl-0.0.4/opengsl/configs/prognn/prognn_minesweeper.yaml
--rw-rw-rw-   0        0        0      873 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/prognn/prognn_pubmed.yaml
--rw-rw-rw-   0        0        0      796 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/prognn/prognn_questions.yaml
--rw-rw-rw-   0        0        0      797 2023-06-14 08:49:58.000000 opengsl-0.0.4/opengsl/configs/prognn/prognn_roman-empire.yaml
--rw-rw-rw-   0        0        0      910 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/prognn/prognn_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.290588 opengsl-0.0.4/opengsl/configs/segsl/
--rw-rw-rw-   0        0        0      804 2023-06-14 11:11:55.000000 opengsl-0.0.4/opengsl/configs/segsl/segsl_blogcatalog.yaml
--rw-rw-rw-   0        0        0      804 2023-06-14 11:10:05.000000 opengsl-0.0.4/opengsl/configs/segsl/segsl_citeseer.yaml
--rw-rw-rw-   0        0        0      820 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/segsl/segsl_cora.yaml
--rw-rw-rw-   0        0        0      773 2023-06-14 11:11:55.000000 opengsl-0.0.4/opengsl/configs/segsl/segsl_flickr.yaml
--rw-rw-rw-   0        0        0      818 2023-06-14 11:11:55.000000 opengsl-0.0.4/opengsl/configs/segsl/segsl_pubmed.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.296243 opengsl-0.0.4/opengsl/configs/sgc/
--rw-rw-rw-   0        0        0      353 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/sgc/sgc_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      413 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/sgc/sgc_blogcatalog.yaml
--rw-rw-rw-   0        0        0      432 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/sgc/sgc_citeseer.yaml
--rw-rw-rw-   0        0        0      464 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/sgc/sgc_cora.yaml
--rw-rw-rw-   0        0        0      418 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/sgc/sgc_flickr.yaml
--rw-rw-rw-   0        0        0      353 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/sgc/sgc_minesweeper.yaml
--rw-rw-rw-   0        0        0      431 2023-06-14 07:15:00.000000 opengsl-0.0.4/opengsl/configs/sgc/sgc_pubmed.yaml
--rw-rw-rw-   0        0        0      353 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/sgc/sgc_questions.yaml
--rw-rw-rw-   0        0        0      353 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/sgc/sgc_roman-empire.yaml
--rw-rw-rw-   0        0        0      353 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/configs/sgc/sgc_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.303243 opengsl-0.0.4/opengsl/configs/slaps/
--rw-rw-rw-   0        0        0      871 2023-06-14 09:55:08.000000 opengsl-0.0.4/opengsl/configs/slaps/slaps_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      904 2023-06-14 09:52:58.000000 opengsl-0.0.4/opengsl/configs/slaps/slaps_blogcatalog.yaml
--rw-rw-rw-   0        0        0      869 2023-06-14 09:06:15.000000 opengsl-0.0.4/opengsl/configs/slaps/slaps_citeseer.yaml
--rw-rw-rw-   0        0        0      931 2023-06-14 09:06:14.000000 opengsl-0.0.4/opengsl/configs/slaps/slaps_cora.yaml
--rw-rw-rw-   0        0        0      904 2023-06-14 09:52:58.000000 opengsl-0.0.4/opengsl/configs/slaps/slaps_flickr.yaml
--rw-rw-rw-   0        0        0      871 2023-06-14 09:55:08.000000 opengsl-0.0.4/opengsl/configs/slaps/slaps_minesweeper.yaml
--rw-rw-rw-   0        0        0      869 2023-06-14 09:53:04.000000 opengsl-0.0.4/opengsl/configs/slaps/slaps_pubmed.yaml
--rw-rw-rw-   0        0        0      871 2023-06-14 09:55:08.000000 opengsl-0.0.4/opengsl/configs/slaps/slaps_questions.yaml
--rw-rw-rw-   0        0        0      871 2023-06-14 09:55:08.000000 opengsl-0.0.4/opengsl/configs/slaps/slaps_roman-empire.yaml
--rw-rw-rw-   0        0        0      871 2023-06-14 09:55:08.000000 opengsl-0.0.4/opengsl/configs/slaps/slaps_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.308249 opengsl-0.0.4/opengsl/configs/stable/
--rw-rw-rw-   0        0        0      666 2023-06-14 11:08:51.000000 opengsl-0.0.4/opengsl/configs/stable/stable_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      661 2023-06-14 11:07:36.000000 opengsl-0.0.4/opengsl/configs/stable/stable_blogcatalog.yaml
--rw-rw-rw-   0        0        0      661 2023-06-14 11:05:19.000000 opengsl-0.0.4/opengsl/configs/stable/stable_citeseer.yaml
--rw-rw-rw-   0        0        0      661 2023-06-14 11:05:19.000000 opengsl-0.0.4/opengsl/configs/stable/stable_cora.yaml
--rw-rw-rw-   0        0        0      661 2023-06-14 11:07:36.000000 opengsl-0.0.4/opengsl/configs/stable/stable_flickr.yaml
--rw-rw-rw-   0        0        0      633 2023-06-14 11:08:51.000000 opengsl-0.0.4/opengsl/configs/stable/stable_minesweeper.yaml
--rw-rw-rw-   0        0        0      661 2023-06-14 11:06:52.000000 opengsl-0.0.4/opengsl/configs/stable/stable_pubmed.yaml
--rw-rw-rw-   0        0        0      632 2023-06-14 11:08:51.000000 opengsl-0.0.4/opengsl/configs/stable/stable_roman-empire.yaml
--rw-rw-rw-   0        0        0      630 2023-06-14 11:08:51.000000 opengsl-0.0.4/opengsl/configs/stable/stable_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.315442 opengsl-0.0.4/opengsl/configs/sublime/
--rw-rw-rw-   0        0        0      761 2023-06-14 11:02:01.000000 opengsl-0.0.4/opengsl/configs/sublime/sublime_amazon-ratings.yaml
--rw-rw-rw-   0        0        0      779 2023-06-14 10:44:54.000000 opengsl-0.0.4/opengsl/configs/sublime/sublime_blogcatalog.yaml
--rw-rw-rw-   0        0        0      754 2023-06-14 10:44:54.000000 opengsl-0.0.4/opengsl/configs/sublime/sublime_citeseer.yaml
--rw-rw-rw-   0        0        0      740 2023-06-14 10:44:54.000000 opengsl-0.0.4/opengsl/configs/sublime/sublime_cora.yaml
--rw-rw-rw-   0        0        0      758 2023-06-14 10:44:54.000000 opengsl-0.0.4/opengsl/configs/sublime/sublime_flickr.yaml
--rw-rw-rw-   0        0        0      759 2023-06-14 11:02:39.000000 opengsl-0.0.4/opengsl/configs/sublime/sublime_minesweeper.yaml
--rw-rw-rw-   0        0        0      755 2023-06-14 10:44:54.000000 opengsl-0.0.4/opengsl/configs/sublime/sublime_pubmed.yaml
--rw-rw-rw-   0        0        0      756 2023-06-14 11:00:53.000000 opengsl-0.0.4/opengsl/configs/sublime/sublime_questions.yaml
--rw-rw-rw-   0        0        0      759 2023-06-14 11:02:17.000000 opengsl-0.0.4/opengsl/configs/sublime/sublime_roman-empire.yaml
--rw-rw-rw-   0        0        0      758 2023-06-14 11:05:19.000000 opengsl-0.0.4/opengsl/configs/sublime/sublime_wiki-cooc.yaml
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.318443 opengsl-0.0.4/opengsl/data/
--rw-rw-rw-   0        0        0       28 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/data/__init__.py
--rw-rw-rw-   0        0        0     7559 2023-06-14 07:36:43.000000 opengsl-0.0.4/opengsl/data/dataset.py
--rw-rw-rw-   0        0        0     1845 2023-06-14 07:15:01.000000 opengsl-0.0.4/opengsl/data/hetero_load.py
--rw-rw-rw-   0        0        0     1242 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/data/homophily_control.py
--rw-rw-rw-   0        0        0     1743 2023-06-14 07:38:00.000000 opengsl-0.0.4/opengsl/data/pyg_load.py
--rw-rw-rw-   0        0        0     3116 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/data/split.py
--rw-rw-rw-   0        0        0     1028 2023-06-14 12:04:56.000000 opengsl-0.0.4/opengsl/load_conf.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.321505 opengsl-0.0.4/opengsl/method/
--rw-rw-rw-   0        0        0     1069 2023-06-14 11:34:51.000000 opengsl-0.0.4/opengsl/method/__init__.py
--rw-rw-rw-   0        0        0     9235 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/gnnsolver.py
--rw-rw-rw-   0        0        0    86508 2023-06-14 11:34:06.000000 opengsl-0.0.4/opengsl/method/gslsolver.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.334669 opengsl-0.0.4/opengsl/method/models/
--rw-rw-rw-   0        0        0        0 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/__init__.py
--rw-rw-rw-   0        0        0    13055 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/cogsl.py
--rw-rw-rw-   0        0        0     5535 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/gaug.py
--rw-rw-rw-   0        0        0     4584 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/gcn.py
--rw-rw-rw-   0        0        0     3470 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/gcn_idgl.py
--rw-rw-rw-   0        0        0     5153 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/gen.py
--rw-rw-rw-   0        0        0     9332 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/gnn_modules.py
--rw-rw-rw-   0        0        0     5704 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/grcn.py
--rw-rw-rw-   0        0        0    11587 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/gt.py
--rw-rw-rw-   0        0        0    10579 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/idgl.py
--rw-rw-rw-   0        0        0     4696 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/jknet.py
--rw-rw-rw-   0        0        0    14225 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/nodeformer.py
--rw-rw-rw-   0        0        0     6836 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/prognn.py
--rw-rw-rw-   0        0        0    31469 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/segsl.py
--rw-rw-rw-   0        0        0    11028 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/slaps.py
--rw-rw-rw-   0        0        0     6613 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/stable.py
--rw-rw-rw-   0        0        0    15908 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/method/models/sublime.py
--rw-rw-rw-   0        0        0     5067 2023-06-14 11:34:06.000000 opengsl-0.0.4/opengsl/method/solver.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.336636 opengsl-0.0.4/opengsl/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 11:34:51.000000 opengsl-0.0.4/opengsl/utils/__init__.py
--rw-rw-rw-   0        0        0     1392 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/utils/logger.py
--rw-rw-rw-   0        0        0     1107 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/utils/recorder.py
--rw-rw-rw-   0        0        0     6901 2023-06-14 05:42:30.000000 opengsl-0.0.4/opengsl/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:25:16.213096 opengsl-0.0.4/opengsl.egg-info/
--rw-rw-rw-   0        0        0     2481 2023-06-14 12:25:16.000000 opengsl-0.0.4/opengsl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8126 2023-06-14 12:25:16.000000 opengsl-0.0.4/opengsl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 12:25:16.000000 opengsl-0.0.4/opengsl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-06-14 12:25:16.000000 opengsl-0.0.4/opengsl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 12:25:16.000000 opengsl-0.0.4/opengsl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 12:25:16.337691 opengsl-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1409 2023-06-14 12:25:09.000000 opengsl-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:27.191271 opengsl-0.0.5/
+-rw-rw-rw-   0        0        0     1085 2023-06-29 07:24:59.000000 opengsl-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       31 2023-06-29 07:24:59.000000 opengsl-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    10647 2023-07-10 12:18:27.191271 opengsl-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9986 2023-06-29 07:24:59.000000 opengsl-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.328521 opengsl-0.0.5/opengsl/
+-rw-rw-rw-   0        0        0      167 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.359905 opengsl-0.0.5/opengsl/config/
+-rw-rw-rw-   0        0        0       52 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.391660 opengsl-0.0.5/opengsl/config/appnp/
+-rw-rw-rw-   0        0        0      508 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/appnp/appnp_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      431 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/appnp/appnp_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      439 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/appnp/appnp_citeseer.yaml
+-rw-rw-rw-   0        0        0      436 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/appnp/appnp_cora.yaml
+-rw-rw-rw-   0        0        0      437 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/appnp/appnp_flickr.yaml
+-rw-rw-rw-   0        0        0      355 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/appnp/appnp_hetero.yaml
+-rw-rw-rw-   0        0        0      469 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/appnp/appnp_minesweeper.yaml
+-rw-rw-rw-   0        0        0      439 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/appnp/appnp_pubmed.yaml
+-rw-rw-rw-   0        0        0      466 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/appnp/appnp_questions.yaml
+-rw-rw-rw-   0        0        0      468 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/appnp/appnp_roman-empire.yaml
+-rw-rw-rw-   0        0        0      502 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/appnp/appnp_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.391660 opengsl-0.0.5/opengsl/config/cogsl/
+-rw-rw-rw-   0        0        0     1274 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/cogsl/cogsl_citeseer.yaml
+-rw-rw-rw-   0        0        0     1127 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/cogsl/cogsl_cora.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.423023 opengsl-0.0.5/opengsl/config/gat/
+-rw-rw-rw-   0        0        0      540 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gat/gat_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      471 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gat/gat_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      401 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gat/gat_citeseer.yaml
+-rw-rw-rw-   0        0        0      401 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gat/gat_cora.yaml
+-rw-rw-rw-   0        0        0      471 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gat/gat_flickr.yaml
+-rw-rw-rw-   0        0        0      543 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gat/gat_minesweeper.yaml
+-rw-rw-rw-   0        0        0      401 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gat/gat_pubmed.yaml
+-rw-rw-rw-   0        0        0      543 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gat/gat_questions.yaml
+-rw-rw-rw-   0        0        0      541 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gat/gat_roman-empire.yaml
+-rw-rw-rw-   0        0        0      542 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gat/gat_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.454278 opengsl-0.0.5/opengsl/config/gaug/
+-rw-rw-rw-   0        0        0     1238 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gaug/gaug_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0     1238 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gaug/gaug_blogcatalog.yaml
+-rw-rw-rw-   0        0        0     1240 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gaug/gaug_citeseer.yaml
+-rw-rw-rw-   0        0        0     1235 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gaug/gaug_cora.yaml
+-rw-rw-rw-   0        0        0     1239 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gaug/gaug_flickr.yaml
+-rw-rw-rw-   0        0        0     1233 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gaug/gaug_minesweeper.yaml
+-rw-rw-rw-   0        0        0     1235 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gaug/gaug_pubmed.yaml
+-rw-rw-rw-   0        0        0     1259 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gaug/gaug_roman-empire.yaml
+-rw-rw-rw-   0        0        0     1231 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gaug/gaug_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.500957 opengsl-0.0.5/opengsl/config/gcn/
+-rw-rw-rw-   0        0        0      849 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gcn/gcn_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      872 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gcn/gcn_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      851 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gcn/gcn_citeseer.yaml
+-rw-rw-rw-   0        0        0      870 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gcn/gcn_cora.yaml
+-rw-rw-rw-   0        0        0      877 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gcn/gcn_flickr.yaml
+-rw-rw-rw-   0        0        0      849 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gcn/gcn_minesweeper.yaml
+-rw-rw-rw-   0        0        0      851 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gcn/gcn_pubmed.yaml
+-rw-rw-rw-   0        0        0      847 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gcn/gcn_questions.yaml
+-rw-rw-rw-   0        0        0      845 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gcn/gcn_roman-empire.yaml
+-rw-rw-rw-   0        0        0      846 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gcn/gcn_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.532212 opengsl-0.0.5/opengsl/config/gen/
+-rw-rw-rw-   0        0        0      836 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gen/gen_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      835 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gen/gen_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      835 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gen/gen_citeseer.yaml
+-rw-rw-rw-   0        0        0      835 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gen/gen_cora.yaml
+-rw-rw-rw-   0        0        0      835 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gen/gen_flickr.yaml
+-rw-rw-rw-   0        0        0      839 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gen/gen_minesweeper.yaml
+-rw-rw-rw-   0        0        0      835 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gen/gen_pubmed.yaml
+-rw-rw-rw-   0        0        0      836 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gen/gen_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.547837 opengsl-0.0.5/opengsl/config/gprgnn/
+-rw-rw-rw-   0        0        0      430 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gprgnn/gprgnn_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      435 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gprgnn/gprgnn_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      439 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gprgnn/gprgnn_citeseer.yaml
+-rw-rw-rw-   0        0        0      436 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gprgnn/gprgnn_cora.yaml
+-rw-rw-rw-   0        0        0      440 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gprgnn/gprgnn_flickr.yaml
+-rw-rw-rw-   0        0        0      398 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gprgnn/gprgnn_minesweeper.yaml
+-rw-rw-rw-   0        0        0      439 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gprgnn/gprgnn_pubmed.yaml
+-rw-rw-rw-   0        0        0      395 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gprgnn/gprgnn_questions.yaml
+-rw-rw-rw-   0        0        0      397 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gprgnn/gprgnn_roman-empire.yaml
+-rw-rw-rw-   0        0        0      398 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gprgnn/gprgnn_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.595119 opengsl-0.0.5/opengsl/config/grcn/
+-rw-rw-rw-   0        0        0      866 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/grcn/grcn_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      864 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/grcn/grcn_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      788 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/grcn/grcn_citeseer.yaml
+-rw-rw-rw-   0        0        0      814 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/grcn/grcn_cora.yaml
+-rw-rw-rw-   0        0        0      864 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/grcn/grcn_flickr.yaml
+-rw-rw-rw-   0        0        0      867 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/grcn/grcn_minesweeper.yaml
+-rw-rw-rw-   0        0        0     1233 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/grcn/grcn_pubmed.yaml
+-rw-rw-rw-   0        0        0      833 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/grcn/grcn_questions.yaml
+-rw-rw-rw-   0        0        0      834 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/grcn/grcn_roman-empire.yaml
+-rw-rw-rw-   0        0        0      832 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/grcn/grcn_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.610739 opengsl-0.0.5/opengsl/config/gt/
+-rw-rw-rw-   0        0        0      678 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gt/gt_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      675 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gt/gt_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      676 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gt/gt_citeseer.yaml
+-rw-rw-rw-   0        0        0      676 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gt/gt_cora.yaml
+-rw-rw-rw-   0        0        0      675 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gt/gt_flickr.yaml
+-rw-rw-rw-   0        0        0      677 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gt/gt_minesweeper.yaml
+-rw-rw-rw-   0        0        0      676 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gt/gt_pubmed.yaml
+-rw-rw-rw-   0        0        0      676 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gt/gt_questions.yaml
+-rw-rw-rw-   0        0        0      677 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gt/gt_roman-empire.yaml
+-rw-rw-rw-   0        0        0      678 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/gt/gt_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.671177 opengsl-0.0.5/opengsl/config/idgl/
+-rw-rw-rw-   0        0        0      761 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/idgl/idgl_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      760 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/idgl/idgl_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      728 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/idgl/idgl_citeseer.yaml
+-rw-rw-rw-   0        0        0      726 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/idgl/idgl_cora.yaml
+-rw-rw-rw-   0        0        0      760 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/idgl/idgl_flickr.yaml
+-rw-rw-rw-   0        0        0      783 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/idgl/idgl_minesweeper.yaml
+-rw-rw-rw-   0        0        0      726 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/idgl/idgl_pubmed.yaml
+-rw-rw-rw-   0        0        0      747 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/idgl/idgl_questions.yaml
+-rw-rw-rw-   0        0        0      782 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/idgl/idgl_roman-empire.yaml
+-rw-rw-rw-   0        0        0      708 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/idgl/idgl_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.751819 opengsl-0.0.5/opengsl/config/jknet/
+-rw-rw-rw-   0        0        0      851 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/jknet/jknet_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      854 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/jknet/jknet_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      859 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/jknet/jknet_citeseer.yaml
+-rw-rw-rw-   0        0        0      854 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/jknet/jknet_cora.yaml
+-rw-rw-rw-   0        0        0      859 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/jknet/jknet_flickr.yaml
+-rw-rw-rw-   0        0        0      820 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/jknet/jknet_minesweeper.yaml
+-rw-rw-rw-   0        0        0      860 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/jknet/jknet_pubmed.yaml
+-rw-rw-rw-   0        0        0      818 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/jknet/jknet_questions.yaml
+-rw-rw-rw-   0        0        0      819 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/jknet/jknet_roman-empire.yaml
+-rw-rw-rw-   0        0        0      848 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/jknet/jknet_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.751819 opengsl-0.0.5/opengsl/config/link/
+-rw-rw-rw-   0        0        0      505 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/link/link.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.751819 opengsl-0.0.5/opengsl/config/lpa/
+-rw-rw-rw-   0        0        0      458 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/lpa/lpa.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.799212 opengsl-0.0.5/opengsl/config/nodeformer/
+-rw-rw-rw-   0        0        0      607 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      624 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      608 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_citeseer.yaml
+-rw-rw-rw-   0        0        0      623 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_cora.yaml
+-rw-rw-rw-   0        0        0      600 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_flickr.yaml
+-rw-rw-rw-   0        0        0      606 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_minesweeper.yaml
+-rw-rw-rw-   0        0        0      624 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_pubmed.yaml
+-rw-rw-rw-   0        0        0      600 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_questions.yaml
+-rw-rw-rw-   0        0        0      625 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_roman-empire.yaml
+-rw-rw-rw-   0        0        0      607 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.830362 opengsl-0.0.5/opengsl/config/prognn/
+-rw-rw-rw-   0        0        0      818 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/prognn/prognn_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      875 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/prognn/prognn_citeseer.yaml
+-rw-rw-rw-   0        0        0      853 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/prognn/prognn_cora.yaml
+-rw-rw-rw-   0        0        0      818 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/prognn/prognn_flickr.yaml
+-rw-rw-rw-   0        0        0      813 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/prognn/prognn_minesweeper.yaml
+-rw-rw-rw-   0        0        0      873 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/prognn/prognn_pubmed.yaml
+-rw-rw-rw-   0        0        0      796 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/prognn/prognn_questions.yaml
+-rw-rw-rw-   0        0        0      797 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/prognn/prognn_roman-empire.yaml
+-rw-rw-rw-   0        0        0      910 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/prognn/prognn_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.845986 opengsl-0.0.5/opengsl/config/segsl/
+-rw-rw-rw-   0        0        0      804 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/segsl/segsl_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      804 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/segsl/segsl_citeseer.yaml
+-rw-rw-rw-   0        0        0      820 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/segsl/segsl_cora.yaml
+-rw-rw-rw-   0        0        0      773 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/segsl/segsl_flickr.yaml
+-rw-rw-rw-   0        0        0      818 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/segsl/segsl_pubmed.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.877670 opengsl-0.0.5/opengsl/config/sgc/
+-rw-rw-rw-   0        0        0      353 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sgc/sgc_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      413 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sgc/sgc_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      432 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sgc/sgc_citeseer.yaml
+-rw-rw-rw-   0        0        0      464 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sgc/sgc_cora.yaml
+-rw-rw-rw-   0        0        0      418 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sgc/sgc_flickr.yaml
+-rw-rw-rw-   0        0        0      353 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sgc/sgc_minesweeper.yaml
+-rw-rw-rw-   0        0        0      431 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sgc/sgc_pubmed.yaml
+-rw-rw-rw-   0        0        0      353 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sgc/sgc_questions.yaml
+-rw-rw-rw-   0        0        0      353 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sgc/sgc_roman-empire.yaml
+-rw-rw-rw-   0        0        0      353 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sgc/sgc_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.940182 opengsl-0.0.5/opengsl/config/slaps/
+-rw-rw-rw-   0        0        0      871 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/slaps/slaps_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      904 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/slaps/slaps_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      869 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/slaps/slaps_citeseer.yaml
+-rw-rw-rw-   0        0        0      931 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/slaps/slaps_cora.yaml
+-rw-rw-rw-   0        0        0      904 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/slaps/slaps_flickr.yaml
+-rw-rw-rw-   0        0        0      871 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/slaps/slaps_minesweeper.yaml
+-rw-rw-rw-   0        0        0      869 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/slaps/slaps_pubmed.yaml
+-rw-rw-rw-   0        0        0      871 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/slaps/slaps_questions.yaml
+-rw-rw-rw-   0        0        0      871 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/slaps/slaps_roman-empire.yaml
+-rw-rw-rw-   0        0        0      871 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/slaps/slaps_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.955805 opengsl-0.0.5/opengsl/config/stable/
+-rw-rw-rw-   0        0        0      666 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/stable/stable_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      661 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/stable/stable_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      661 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/stable/stable_citeseer.yaml
+-rw-rw-rw-   0        0        0      661 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/stable/stable_cora.yaml
+-rw-rw-rw-   0        0        0      661 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/stable/stable_flickr.yaml
+-rw-rw-rw-   0        0        0      633 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/stable/stable_minesweeper.yaml
+-rw-rw-rw-   0        0        0      661 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/stable/stable_pubmed.yaml
+-rw-rw-rw-   0        0        0      632 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/stable/stable_roman-empire.yaml
+-rw-rw-rw-   0        0        0      630 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/stable/stable_wiki-cooc.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:27.003117 opengsl-0.0.5/opengsl/config/sublime/
+-rw-rw-rw-   0        0        0      761 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sublime/sublime_amazon-ratings.yaml
+-rw-rw-rw-   0        0        0      779 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sublime/sublime_blogcatalog.yaml
+-rw-rw-rw-   0        0        0      754 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sublime/sublime_citeseer.yaml
+-rw-rw-rw-   0        0        0      740 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sublime/sublime_cora.yaml
+-rw-rw-rw-   0        0        0      758 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sublime/sublime_flickr.yaml
+-rw-rw-rw-   0        0        0      759 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sublime/sublime_minesweeper.yaml
+-rw-rw-rw-   0        0        0      755 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sublime/sublime_pubmed.yaml
+-rw-rw-rw-   0        0        0      756 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sublime/sublime_questions.yaml
+-rw-rw-rw-   0        0        0      759 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sublime/sublime_roman-empire.yaml
+-rw-rw-rw-   0        0        0      758 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/sublime/sublime_wiki-cooc.yaml
+-rw-rw-rw-   0        0        0     2060 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/config/util.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:27.003117 opengsl-0.0.5/opengsl/data/
+-rw-rw-rw-   0        0        0       76 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:27.003117 opengsl-0.0.5/opengsl/data/dataset/
+-rw-rw-rw-   0        0        0       48 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/data/dataset/__init__.py
+-rw-rw-rw-   0        0        0     8047 2023-07-10 12:02:35.000000 opengsl-0.0.5/opengsl/data/dataset/dataset.py
+-rw-rw-rw-   0        0        0     1900 2023-07-10 12:02:35.000000 opengsl-0.0.5/opengsl/data/dataset/hetero_load.py
+-rw-rw-rw-   0        0        0     1743 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/data/dataset/pyg_load.py
+-rw-rw-rw-   0        0        0     3116 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/data/dataset/split.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:27.018705 opengsl-0.0.5/opengsl/data/preprocess/
+-rw-rw-rw-   0        0        0      128 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/data/preprocess/__init__.py
+-rw-rw-rw-   0        0        0     1719 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/data/preprocess/control_homophily.py
+-rw-rw-rw-   0        0        0     2353 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/data/preprocess/normalize.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:27.018705 opengsl-0.0.5/opengsl/expmanager/
+-rw-rw-rw-   0        0        0     4618 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/expmanager/ExpManager.py
+-rw-rw-rw-   0        0        0        0 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/expmanager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:27.049959 opengsl-0.0.5/opengsl/method/
+-rw-rw-rw-   0        0        0     1218 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/__init__.py
+-rw-rw-rw-   0        0        0    19142 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/gnnsolver.py
+-rw-rw-rw-   0        0        0   102542 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/gslsolver.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:27.175634 opengsl-0.0.5/opengsl/method/models/
+-rw-rw-rw-   0        0        0        0 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/__init__.py
+-rw-rw-rw-   0        0        0    13055 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/cogsl.py
+-rw-rw-rw-   0        0        0     6065 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/gaug.py
+-rw-rw-rw-   0        0        0     4584 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/gcn.py
+-rw-rw-rw-   0        0        0     3470 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/gcn_idgl.py
+-rw-rw-rw-   0        0        0     5153 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/gen.py
+-rw-rw-rw-   0        0        0     9332 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/gnn_modules.py
+-rw-rw-rw-   0        0        0     5704 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/grcn.py
+-rw-rw-rw-   0        0        0    11738 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/gt.py
+-rw-rw-rw-   0        0        0    10579 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/idgl.py
+-rw-rw-rw-   0        0        0     4696 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/jknet.py
+-rw-rw-rw-   0        0        0    14225 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/nodeformer.py
+-rw-rw-rw-   0        0        0     6836 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/prognn.py
+-rw-rw-rw-   0        0        0    31469 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/segsl.py
+-rw-rw-rw-   0        0        0    11028 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/slaps.py
+-rw-rw-rw-   0        0        0     6613 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/stable.py
+-rw-rw-rw-   0        0        0    15908 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/models/sublime.py
+-rw-rw-rw-   0        0        0     7323 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/method/solver.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:27.191271 opengsl-0.0.5/opengsl/utils/
+-rw-rw-rw-   0        0        0      474 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/utils/__init__.py
+-rw-rw-rw-   0        0        0     2038 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/utils/logger.py
+-rw-rw-rw-   0        0        0     2433 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/utils/recorder.py
+-rw-rw-rw-   0        0        0     6032 2023-06-29 07:24:59.000000 opengsl-0.0.5/opengsl/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 12:18:26.344152 opengsl-0.0.5/opengsl.egg-info/
+-rw-rw-rw-   0        0        0    10647 2023-07-10 12:18:26.000000 opengsl-0.0.5/opengsl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8181 2023-07-10 12:18:26.000000 opengsl-0.0.5/opengsl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 12:18:26.000000 opengsl-0.0.5/opengsl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-07-10 12:18:26.000000 opengsl-0.0.5/opengsl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-10 12:18:26.000000 opengsl-0.0.5/opengsl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 12:18:27.191271 opengsl-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-07-10 12:16:42.000000 opengsl-0.0.5/setup.py
```

### Comparing `opengsl-0.0.4/LICENSE` & `opengsl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/cogsl/cogsl_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/cogsl/cogsl_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/cogsl/cogsl_cora.yaml` & `opengsl-0.0.5/opengsl/config/cogsl/cogsl_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gat/gat_amazon-ratings.yaml` & `opengsl-0.0.5/opengsl/config/gat/gat_amazon-ratings.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gat/gat_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/gat/gat_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gat/gat_questions.yaml` & `opengsl-0.0.5/opengsl/config/gat/gat_questions.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gat/gat_roman-empire.yaml` & `opengsl-0.0.5/opengsl/config/gat/gat_roman-empire.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gat/gat_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/gat/gat_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gaug/gaug_amazon-ratings.yaml` & `opengsl-0.0.5/opengsl/config/gaug/gaug_amazon-ratings.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gaug/gaug_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/gaug/gaug_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gaug/gaug_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/gaug/gaug_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gaug/gaug_cora.yaml` & `opengsl-0.0.5/opengsl/config/gaug/gaug_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gaug/gaug_flickr.yaml` & `opengsl-0.0.5/opengsl/config/gaug/gaug_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gaug/gaug_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/gaug/gaug_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gaug/gaug_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/gaug/gaug_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gaug/gaug_roman-empire.yaml` & `opengsl-0.0.5/opengsl/config/gaug/gaug_roman-empire.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gaug/gaug_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/gaug/gaug_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gcn/gcn_amazon-ratings.yaml` & `opengsl-0.0.5/opengsl/config/gcn/gcn_amazon-ratings.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gcn/gcn_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/gcn/gcn_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gcn/gcn_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/gcn/gcn_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gcn/gcn_cora.yaml` & `opengsl-0.0.5/opengsl/config/gcn/gcn_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gcn/gcn_flickr.yaml` & `opengsl-0.0.5/opengsl/config/gcn/gcn_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gcn/gcn_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/gcn/gcn_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gcn/gcn_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/gcn/gcn_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gcn/gcn_questions.yaml` & `opengsl-0.0.5/opengsl/config/gcn/gcn_questions.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gcn/gcn_roman-empire.yaml` & `opengsl-0.0.5/opengsl/config/gcn/gcn_roman-empire.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gcn/gcn_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/gcn/gcn_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gen/gen_amazon-ratings.yaml` & `opengsl-0.0.5/opengsl/config/gen/gen_amazon-ratings.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gen/gen_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/gen/gen_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gen/gen_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/gen/gen_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gen/gen_cora.yaml` & `opengsl-0.0.5/opengsl/config/gen/gen_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gen/gen_flickr.yaml` & `opengsl-0.0.5/opengsl/config/gen/gen_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gen/gen_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/gen/gen_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gen/gen_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/gen/gen_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gen/gen_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/gen/gen_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/grcn/grcn_amazon-ratings.yaml` & `opengsl-0.0.5/opengsl/config/grcn/grcn_amazon-ratings.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/grcn/grcn_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/grcn/grcn_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/grcn/grcn_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/grcn/grcn_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/grcn/grcn_cora.yaml` & `opengsl-0.0.5/opengsl/config/grcn/grcn_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/grcn/grcn_flickr.yaml` & `opengsl-0.0.5/opengsl/config/grcn/grcn_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/grcn/grcn_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/grcn/grcn_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/grcn/grcn_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/grcn/grcn_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/grcn/grcn_questions.yaml` & `opengsl-0.0.5/opengsl/config/grcn/grcn_questions.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/grcn/grcn_roman-empire.yaml` & `opengsl-0.0.5/opengsl/config/grcn/grcn_roman-empire.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/grcn/grcn_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/grcn/grcn_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gt/gt_amazon-ratings.yaml` & `opengsl-0.0.5/opengsl/config/gt/gt_amazon-ratings.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gt/gt_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/gt/gt_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gt/gt_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/gt/gt_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gt/gt_cora.yaml` & `opengsl-0.0.5/opengsl/config/gt/gt_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gt/gt_flickr.yaml` & `opengsl-0.0.5/opengsl/config/gt/gt_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gt/gt_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/gt/gt_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gt/gt_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/gt/gt_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gt/gt_questions.yaml` & `opengsl-0.0.5/opengsl/config/gt/gt_questions.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gt/gt_roman-empire.yaml` & `opengsl-0.0.5/opengsl/config/gt/gt_roman-empire.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/gt/gt_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/gt/gt_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/idgl/idgl_amazon-ratings.yaml` & `opengsl-0.0.5/opengsl/config/idgl/idgl_amazon-ratings.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/idgl/idgl_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/idgl/idgl_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/idgl/idgl_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/idgl/idgl_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/idgl/idgl_cora.yaml` & `opengsl-0.0.5/opengsl/config/idgl/idgl_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/idgl/idgl_flickr.yaml` & `opengsl-0.0.5/opengsl/config/idgl/idgl_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/idgl/idgl_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/idgl/idgl_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/idgl/idgl_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/idgl/idgl_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/idgl/idgl_questions.yaml` & `opengsl-0.0.5/opengsl/config/idgl/idgl_questions.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/idgl/idgl_roman-empire.yaml` & `opengsl-0.0.5/opengsl/config/idgl/idgl_roman-empire.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/idgl/idgl_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/idgl/idgl_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/jknet/jknet_amazon-ratings.yaml` & `opengsl-0.0.5/opengsl/config/jknet/jknet_amazon-ratings.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/jknet/jknet_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/jknet/jknet_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/jknet/jknet_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/jknet/jknet_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/jknet/jknet_cora.yaml` & `opengsl-0.0.5/opengsl/config/jknet/jknet_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/jknet/jknet_flickr.yaml` & `opengsl-0.0.5/opengsl/config/jknet/jknet_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/jknet/jknet_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/jknet/jknet_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/jknet/jknet_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/jknet/jknet_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/jknet/jknet_questions.yaml` & `opengsl-0.0.5/opengsl/config/jknet/jknet_questions.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/jknet/jknet_roman-empire.yaml` & `opengsl-0.0.5/opengsl/config/jknet/jknet_roman-empire.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/jknet/jknet_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/jknet/jknet_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_amazon-ratings.yaml` & `opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_amazon-ratings.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_cora.yaml` & `opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_flickr.yaml` & `opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_questions.yaml` & `opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_questions.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_roman-empire.yaml` & `opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_roman-empire.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/nodeformer/nodeformer_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/nodeformer/nodeformer_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/prognn/prognn_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/prognn/prognn_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/prognn/prognn_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/prognn/prognn_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/prognn/prognn_cora.yaml` & `opengsl-0.0.5/opengsl/config/prognn/prognn_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/prognn/prognn_flickr.yaml` & `opengsl-0.0.5/opengsl/config/prognn/prognn_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/prognn/prognn_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/prognn/prognn_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/prognn/prognn_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/prognn/prognn_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/prognn/prognn_questions.yaml` & `opengsl-0.0.5/opengsl/config/prognn/prognn_questions.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/prognn/prognn_roman-empire.yaml` & `opengsl-0.0.5/opengsl/config/prognn/prognn_roman-empire.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/prognn/prognn_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/prognn/prognn_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/segsl/segsl_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/segsl/segsl_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/segsl/segsl_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/segsl/segsl_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/segsl/segsl_cora.yaml` & `opengsl-0.0.5/opengsl/config/segsl/segsl_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/segsl/segsl_flickr.yaml` & `opengsl-0.0.5/opengsl/config/segsl/segsl_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/segsl/segsl_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/segsl/segsl_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/slaps/slaps_amazon-ratings.yaml` & `opengsl-0.0.5/opengsl/config/slaps/slaps_amazon-ratings.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/slaps/slaps_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/slaps/slaps_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/slaps/slaps_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/slaps/slaps_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/slaps/slaps_cora.yaml` & `opengsl-0.0.5/opengsl/config/slaps/slaps_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/slaps/slaps_flickr.yaml` & `opengsl-0.0.5/opengsl/config/slaps/slaps_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/slaps/slaps_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/slaps/slaps_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/slaps/slaps_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/slaps/slaps_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/slaps/slaps_questions.yaml` & `opengsl-0.0.5/opengsl/config/slaps/slaps_questions.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/slaps/slaps_roman-empire.yaml` & `opengsl-0.0.5/opengsl/config/slaps/slaps_roman-empire.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/slaps/slaps_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/slaps/slaps_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/stable/stable_amazon-ratings.yaml` & `opengsl-0.0.5/opengsl/config/stable/stable_amazon-ratings.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/stable/stable_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/stable/stable_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/stable/stable_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/stable/stable_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/stable/stable_cora.yaml` & `opengsl-0.0.5/opengsl/config/stable/stable_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/stable/stable_flickr.yaml` & `opengsl-0.0.5/opengsl/config/stable/stable_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/stable/stable_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/stable/stable_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/stable/stable_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/stable/stable_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/stable/stable_roman-empire.yaml` & `opengsl-0.0.5/opengsl/config/stable/stable_roman-empire.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/stable/stable_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/stable/stable_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/sublime/sublime_amazon-ratings.yaml` & `opengsl-0.0.5/opengsl/config/sublime/sublime_amazon-ratings.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/sublime/sublime_blogcatalog.yaml` & `opengsl-0.0.5/opengsl/config/sublime/sublime_blogcatalog.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/sublime/sublime_citeseer.yaml` & `opengsl-0.0.5/opengsl/config/sublime/sublime_citeseer.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/sublime/sublime_cora.yaml` & `opengsl-0.0.5/opengsl/config/sublime/sublime_cora.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/sublime/sublime_flickr.yaml` & `opengsl-0.0.5/opengsl/config/sublime/sublime_flickr.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/sublime/sublime_minesweeper.yaml` & `opengsl-0.0.5/opengsl/config/sublime/sublime_minesweeper.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/sublime/sublime_pubmed.yaml` & `opengsl-0.0.5/opengsl/config/sublime/sublime_pubmed.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/sublime/sublime_questions.yaml` & `opengsl-0.0.5/opengsl/config/sublime/sublime_questions.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/sublime/sublime_roman-empire.yaml` & `opengsl-0.0.5/opengsl/config/sublime/sublime_roman-empire.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/configs/sublime/sublime_wiki-cooc.yaml` & `opengsl-0.0.5/opengsl/config/sublime/sublime_wiki-cooc.yaml`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/data/dataset.py` & `opengsl-0.0.5/opengsl/data/dataset/dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,100 @@
 import torch
 from .pyg_load import pyg_load_dataset
 from .hetero_load import hetero_load
 from .split import get_split
-from ..utils.utils import normalize_feats
+from opengsl.data.preprocess.normalize import normalize
 import numpy as np
-from .homophily_control import get_new_adj
+from opengsl.data.preprocess.control_homophily import control_homophily
 import pickle
 import os
 import urllib.request
 
 
 class Dataset:
+    '''
+    Dataset Class.
+    This class loads, preprocesses and splits various datasets.
+
+    Parameters
+    ----------
+    data : str
+        The name of dataset.
+    feat_norm : bool
+        Whether to normalize the features.
+    verbose : bool
+        Whether to print statistics.
+    n_splits : int
+        Number of data splits.
+    homophily_control : float
+        The homophily ratio `control homophily` receives. If set to `None`, the original adj will be kept unchanged.
+    path : str
+        Path to save dataset files.
+    '''
 
     def __init__(self, data, feat_norm=False, verbose=True, n_splits=1, homophily_control=None, path='./data/'):
-        '''
-        This class loads, preprocessed and splits data. The results are saved as "self.feats, self.adj, self.labels, self.train_masks, self.val_masks, self.test_masks".
-        Noth that self.adj is undirected and has no self loops.
-
-        Parameters
-        ----------
-        data : the name of dataset
-        feat_norm : whether to normalize the features
-        verbose : whether to print statistics
-        n_splits : number of data splits
-        '''
         self.name = data
         self.path = path
         self.device = torch.device('cuda')
         self.prepare_data(data, feat_norm, verbose)
         self.split_data(n_splits, verbose)
         if homophily_control:
-            self.adj = get_new_adj(self.adj, self.labels.cpu().numpy(), homophily_control)
+            self.adj = control_homophily(self.adj, self.labels.cpu().numpy(), homophily_control)
 
     def prepare_data(self, ds_name, feat_norm=False, verbose=True):
         '''
-        Parameters
-        Load data. Homophilious data are loaded via pyg, while heterophilous data are loaded with "hetero_load".
+        Function to Load various datasets.
+        Homophilous datasets are loaded via pyg, while heterophilous datasets are loaded with `hetero_load`.
+        The results are saved as `self.feats, self.adj, self.labels, self.train_masks, self.val_masks, self.test_masks`.
+        Noth that `self.adj` is undirected and has no self loops.
 
+        Parameters
         ----------
-        ds_name : the name of dataset
-        feat_norm : whether to normalize the features
-        verbose : whether to print statistics
-
-        Returns
-        -------
+        ds_name : str
+            The name of dataset.
+        feat_norm : bool
+            Whether to normalize the features.
+        verbose : bool
+            Whether to print statistics.
 
         '''
         if ds_name in ['cora', 'pubmed', 'citeseer', 'amazoncom', 'amazonpho', 'coauthorcs', 'coauthorph', 'blogcatalog',
                        'flickr']:
             self.data_raw = pyg_load_dataset(ds_name, path=self.path)
             self.g = self.data_raw[0]
             self.feats = self.g.x  # unnormalized
             if ds_name == 'flickr':
                 self.feats = self.feats.to_dense()
             self.n_nodes = self.feats.shape[0]
             self.dim_feats = self.feats.shape[1]
             self.labels = self.g.y
             self.adj = torch.sparse.FloatTensor(self.g.edge_index, torch.ones(self.g.edge_index.shape[1]),
                                                 [self.n_nodes, self.n_nodes])
-            self.n_edges = self.g.num_edges
+            self.n_edges = self.g.num_edges/2
             self.n_classes = self.data_raw.num_classes
 
             self.feats = self.feats.to(self.device)
             self.labels = self.labels.to(self.device)
             self.adj = self.adj.to(self.device)
             # normalize features
             if feat_norm:
-                self.feats = normalize_feats(self.feats)
+                self.feats = normalize(self.feats, style='row')
 
         elif ds_name in ['amazon-ratings', 'questions', 'chameleon-filtered', 'squirrel-filtered', 'minesweeper', 'roman-empire', 'wiki-cooc']:
             self.feats, self.adj, self.labels, self.splits = hetero_load(ds_name, path=self.path)
 
             self.feats = self.feats.to(self.device)
             self.labels = self.labels.to(self.device)
             self.adj = self.adj.to(self.device)
             self.n_nodes = self.feats.shape[0]
             self.dim_feats = self.feats.shape[1]
             self.n_edges = len(self.adj.coalesce().values())/2
             if feat_norm:
-                self.feats = normalize_feats(self.feats)
+                self.feats = normalize(self.feats, style='row')
+                # exit(0)
             self.n_classes = len(self.labels.unique())
 
         else:
             print('dataset not implemented')
             exit(0)
 
         if verbose:
@@ -94,21 +106,22 @@
 
         self.num_targets = self.n_classes
         if self.num_targets == 2:
             self.num_targets = 1
 
     def split_data(self, n_splits, verbose=True):
         '''
+        Function to conduct data splitting for various datasets.
+
         Parameters
         ----------
-        n_splits : number of data splits
-        verbose : whether to print statistics
-
-        Returns
-        -------
+        n_splits : int
+            Number of data splits.
+        verbose : bool
+            Whether to print statistics.
 
         '''
         self.train_masks = []
         self.val_masks = []
         self.test_masks = []
         if self.name in ['blogcatalog', 'flickr']:
             def load_obj(file_name):
```

### Comparing `opengsl-0.0.4/opengsl/data/hetero_load.py` & `opengsl-0.0.5/opengsl/data/dataset/hetero_load.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import os
 import torch
 import dgl
 import urllib.request
 
 def hetero_load(name, path='./data/hetero_data'):
     file_name = f'{name.replace("-", "_")}.npz'
+    if not os.path.exists(path):
+        os.makedirs(path)
     if not os.path.exists(os.path.join(path, file_name)):
         download(file_name, path)
     data = np.load(os.path.join(path, f'{name.replace("-", "_")}.npz'))
     node_features = torch.tensor(data['node_features'])
     labels = torch.tensor(data['node_labels'])
     edges = torch.tensor(data['edges'])
     train_masks = torch.tensor(data['train_masks'])
@@ -18,28 +20,28 @@
 
     train_indices = [torch.nonzero(x, as_tuple=False).squeeze().numpy() for x in train_masks]
     val_indices = [torch.nonzero(x, as_tuple=False).squeeze().numpy() for x in val_masks]
     test_indices = [torch.nonzero(x, as_tuple=False).squeeze().numpy() for x in test_masks]
 
 
     n_nodes = node_features.shape[0]
-    graph = dgl.graph((edges[:, 0], edges[:, 1]), num_nodes=len(node_features), idtype=torch.int)
+    graph = dgl.graph((edges[:, 0], edges[:, 1]), num_nodes=len(node_features), idtype=torch.long)
     graph = dgl.to_bidirected(graph)
     adj = graph.adj()
 
     num_classes = len(labels.unique())
     num_targets = 1 if num_classes == 2 else num_classes
     if num_targets == 1:
         labels = labels.float()
 
 
     return node_features, adj, labels, (train_indices, val_indices, test_indices)
 
 def download(name, path):
-    url = 'https://github.com/yandex-research/heterophilous-graphs/raw/main/data/'
+    url = 'https://github.com/OpenGSL/HeterophilousDatasets/raw/main/data/'
     try:
         print('Downloading', url+name)
         urllib.request.urlretrieve(url + name, os.path.join(path, name))
         print('Done!')
     except:
         raise Exception('''Download failed! Make sure you have stable Internet connection and enter the right name''')
```

### Comparing `opengsl-0.0.4/opengsl/data/pyg_load.py` & `opengsl-0.0.5/opengsl/data/dataset/pyg_load.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/data/split.py` & `opengsl-0.0.5/opengsl/data/dataset/split.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/gslsolver.py` & `opengsl-0.0.5/opengsl/method/gslsolver.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,68 +2,93 @@
 from sklearn.metrics.pairwise import cosine_similarity as cos
 import numpy as np
 import random
 from copy import deepcopy
 from .models.gcn import GCN
 from .models.gnn_modules import APPNP
 from .models.grcn import GRCN
-from .models.gaug import GAug, eval_edge_pred, MultipleOptimizer
+from .models.gaug import GAug, eval_edge_pred, MultipleOptimizer, get_lr_schedule_by_sigmoid
 from .models.gen import EstimateAdj as GENEstimateAdj, prob_to_adj
 from .models.idgl import IDGL, sample_anchors, diff, compute_anchor_adj
 from .models.prognn import PGD, prox_operators, EstimateAdj, feature_smoothing
 from .models.gt import GT
 from .models.slaps import SLAPS
 from .models.nodeformer import NodeFormer, adj_mul
 from .models.segsl import knn_maxE1, add_knn, get_weight, get_adj_matrix, PartitionTree, get_community, reshape
 from .models.sublime import torch_sparse_to_dgl_graph, FGP_learner, ATT_learner, GNN_learner, MLP_learner, GCL, get_feat_mask, split_batch, dgl_graph_to_torch_sparse, GCN_SUB
 from .models.stable import DGI, preprocess_adj, aug_random_edge, get_reliable_neighbors
 from .models.cogsl import CoGSL
 import torch
 import torch.nn.functional as F
 import time
 from .solver import Solver
-from ..utils.utils import normalize, get_lr_schedule_by_sigmoid, get_homophily, normalize_sp_tensor, sparse_tensor_to_scipy_sparse, sparse_normalize, sparse_mx_to_torch_sparse_tensor
+from ..utils.utils import get_homophily, sparse_tensor_to_scipy_sparse, scipy_sparse_to_sparse_tensor
+from opengsl.data.preprocess.normalize import normalize, normalize_sp_matrix
 from ..utils.recorder import Recorder
 import dgl
 import copy
 import os
 from os.path import dirname
 
 
 class GRCNSolver(Solver):
-    def __init__(self, conf, dataset):
-        '''
-        Create a solver for grcn to train, evaluate, test in a run. Some operations are conducted during initialization instead of "set_method" to avoid repetitive computations.
+    '''
+        A solver to train, evaluate, test GRCN in a run.
+
         Parameters
         ----------
-        conf : config file
-        dataset: dataset object containing all things about dataset
+        conf : argparse.Namespace
+            Config file.
+        dataset : opengsl.data.Dataset
+            The dataset.
+
+        Attributes
+        ----------
+        method_name : str
+            The name of the method.
+
+        Examples
+        --------
+        >>> # load dataset
+        >>> import opengsl.dataset
+        >>> dataset = opengsl.data.Dataset('cora', feat_norm=True)
+        >>> # load config file
+        >>> import opengsl.config.load_conf
+        >>> conf = opengsl.config.load_conf('grcn', 'cora')
+        >>>
+        >>> solver = GRCNSolver(conf, dataset)
+        >>> # Conduct a experiment run.
+        >>> acc, new_structure = solver.run_exp(split=0, debug=True)
         '''
+    def __init__(self, conf, dataset):
         super().__init__(conf, dataset)
         self.method_name = "grcn"
         print("Solver Version : [{}]".format("grcn"))
         edge_index = self.adj.coalesce().indices().cpu()
         loop_edge_index = torch.stack([torch.arange(self.n_nodes), torch.arange(self.n_nodes)])
         edges = torch.cat([edge_index, loop_edge_index], dim=1)
         self.adj = torch.sparse.FloatTensor(edges, torch.ones(edges.shape[1]), [self.n_nodes, self.n_nodes]).to(self.device).coalesce()
 
 
     def learn(self, debug=False):
         '''
         Learning process of GRCN.
+
         Parameters
         ----------
-        debug
+        debug : bool
+            Whether to print statistics during training.
 
         Returns
         -------
-
+        result : dict
+            A dict containing train, valid and test metrics.
+        graph : torch.tensor
+            The learned structure.
         '''
-
-
         for epoch in range(self.conf.training['n_epochs']):
             improve = ''
             t0 = time.time()
             self.model.train()
             self.optim1.zero_grad()
             self.optim2.zero_grad()
 
@@ -100,42 +125,84 @@
         print('Time(s): {:.4f}'.format(self.total_time))
         loss_test, acc_test, _ = self.test()
         self.result['test'] = acc_test
         print("Loss(test) {:.4f} | Acc(test) {:.4f}".format(loss_test.item(), acc_test))
         return self.result, self.best_graph
 
     def evaluate(self, test_mask):
+        '''
+        Evaluation procedure of GRCN.
+
+        Parameters
+        ----------
+        test_mask : torch.tensor
+            A boolean tensor indicating whether the node is in the data set.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        adj : torch.tensor        
+            The learned structure.
+        '''
         self.model.eval()
         with torch.no_grad():
             output, adj = self.model(self.feats, self.adj)
         logits = output[test_mask]
         labels = self.labels[test_mask]
         loss=self.loss_fn(logits, labels)
         return loss, self.metric(labels.cpu().numpy(), logits.detach().cpu().numpy()), adj
 
     def set_method(self):
+        '''
+        Function to set the model and necessary variables for each run, automatically called in function `set`.
+
+        '''
         self.model = GRCN(self.n_nodes, self.dim_feats, self.num_targets, self.device, self.conf).to(self.device)
         self.optim1 = torch.optim.Adam(self.model.base_parameters(), lr=self.conf.training['lr'],
                                        weight_decay=self.conf.training['weight_decay'])
         self.optim2 = torch.optim.Adam(self.model.graph_parameters(), lr=self.conf.training['lr_graph'])
 
 
 class GAUGSolver(Solver):
+    '''
+    A solver to train, evaluate, test GAug in a run.
+
+    Parameters
+    ----------
+    conf : argparse.Namespace
+        Config file.
+    dataset : opengsl.data.Dataset
+        The dataset.
+
+    Attributes
+    ----------
+    method_name : str
+        The name of the method.
+
+    Examples
+    --------
+    >>> # load dataset
+    >>> import opengsl.dataset
+    >>> dataset = opengsl.data.Dataset('cora', feat_norm=True)
+    >>> # load config file
+    >>> import opengsl.config.load_conf
+    >>> conf = opengsl.config.load_conf('gaug', 'cora')
+    >>>
+    >>> solver = GAUGSolver(conf, dataset)
+    >>> # Conduct a experiment run.
+    >>> acc, new_strcuture = solver.run_exp(split=0, debug=True)
+    '''
     def __init__(self, conf, dataset):
-        '''
-        Create a solver for gaug to train, evaluate, test in a run. Some operations are conducted during initialization instead of "set_method" to avoid repetitive computations.
-        Parameters
-        ----------
-        conf : config file
-        dataset: dataset object containing all things about dataset
-        '''
         super().__init__(conf, dataset)
         self.method_name = "gaug"
         print("Solver Version : [{}]".format("gaug"))
-        self.normalized_adj = normalize_sp_tensor(self.adj).to(self.device)
+        self.normalized_adj = normalize(self.adj, sparse=True).to(self.device)
         self.adj_orig = (self.adj.to_dense() + torch.eye(self.n_nodes).to(self.device))  # adj with self loop
         self.conf = conf
 
     def pretrain_ep_net(self, norm_w, pos_weight, n_epochs, debug=False):
         """ pretrain the edge prediction network """
         optimizer = torch.optim.Adam(self.model.ep_net.parameters(), lr=self.conf.training['lr'])
         self.model.train()
@@ -193,14 +260,29 @@
 
             # print
             if debug:
                 print("NCNet pretrain, Epoch {:05d} | Time(s) {:.4f} | Loss(train) {:.4f} | Acc(train) {:.4f} | Loss(val) {:.4f} | Acc(val) {:.4f} | {}".format(
                     epoch+1, time.time() -t, loss_train.item(), acc_train, loss_val, acc_val, improve))
 
     def learn(self, debug=False):
+        '''
+        Learning process of GAUG.
+
+        Parameters
+        ----------
+        debug : bool
+            Whether to print statistics during training.
+
+        Returns
+        -------
+        result : dict
+            A dict containing train, valid and test metrics.
+        graph : torch.tensor
+            The learned structure.
+        '''
         patience_step = 0
 
         # prepare
         adj_t = self.adj_orig
         norm_w = adj_t.shape[0]**2 / float((adj_t.shape[0]**2 - adj_t.sum()) * 2)
         pos_weight = torch.FloatTensor([float(adj_t.shape[0]**2 - adj_t.sum()) / adj_t.sum()]).to(self.device)
 
@@ -278,14 +360,18 @@
         acc_test = self.metric(self.labels[self.test_mask].cpu().numpy(), output[self.test_mask].detach().cpu().numpy())
         self.result['test'] = acc_test
         print("Loss(test) {:.4f} | Acc(test) {:.4f}".format(loss_test.item(), acc_test))
 
         return self.result, self.best_graph
 
     def set_method(self):
+        '''
+        Function to set the model and necessary variables for each run, automatically called in function `set`.
+
+        '''
         # sample edges
         if self.labels.size(0) > 5000:
             edge_frac = 0.01
         else:
             edge_frac = 0.1
         adj_matrix = sp.csr_matrix(self.adj.to_dense().cpu().numpy())
         adj_matrix.setdiag(1)  # the original code samples 10%(1%) of the total edges(with self loop)
@@ -313,26 +399,47 @@
         self.val_edges = np.concatenate((pos_edges, neg_edges), axis=0)
         self.edge_labels = np.array([1] * n_edges_sample + [0] * n_edges_sample)
 
         self.model = GAug(self.dim_feats, self.num_targets, self.conf).to(self.device)
 
 
 class GENSolver(Solver):
+    '''
+    A solver to train, evaluate, test GEN in a run.
+
+    Parameters
+    ----------
+    conf : argparse.Namespace
+        Config file.
+    dataset : opengsl.data.Dataset
+        The dataset.
+
+    Attributes
+    ----------
+    method_name : str
+        The name of the method.
+
+    Examples
+    --------
+    >>> # load dataset
+    >>> import opengsl.dataset
+    >>> dataset = opengsl.data.Dataset('cora', feat_norm=True)
+    >>> # load config file
+    >>> import opengsl.config.load_conf
+    >>> conf = opengsl.config.load_conf('gen', 'cora')
+    >>>
+    >>> solver = GENSolver(conf, dataset)
+    >>> # Conduct a experiment run.
+    >>> acc, new_structure = solver.run_exp(split=0, debug=True)
+    '''
     def __init__(self, conf, dataset):
-        '''
-        Create a solver for gen to train, evaluate, test in a run. Some operations are conducted during initialization instead of "set_method" to avoid repetitive computations.
-        Parameters
-        ----------
-        conf : config file
-        dataset: dataset object containing all things about dataset
-        '''
         super().__init__(conf, dataset)
         self.method_name = "gen"
         print("Solver Version : [{}]".format("gen"))
-        self.homophily = get_homophily(self.labels.cpu().numpy(), self.adj.to_dense().cpu().numpy())
+        self.homophily = get_homophily(self.labels.cpu(), self.adj.to_dense().cpu(), type='node')
 
     def knn(self, feature):
         # Generate a knn graph for input feature matrix. Note that the graph contains self loop.
         adj = np.zeros((self.n_nodes, self.n_nodes), dtype=np.int64)
         dist = cos(feature.detach().cpu().numpy())
         col = np.argpartition(dist, -(self.conf.gsl['k'] + 1), axis=1)[:, -(self.conf.gsl['k'] + 1):].flatten()
         adj[np.arange(self.n_nodes).repeat(self.conf.gsl['k'] + 1), col] = 1
@@ -341,15 +448,15 @@
     def train_gcn(self, iter, adj, debug=False):
         if debug:
             print('==== Iteration {:04d} ===='.format(iter+1))
         t = time.time()
         improve_1 = ''
         best_loss_val = 10
         best_acc_val = 0
-        normalized_adj = normalize_sp_tensor(adj)
+        normalized_adj = normalize(adj, sparse=True)
         for epoch in range(self.conf.training['n_epochs']):
             improve_2 = ''
             t0 = time.time()
             self.model.train()
             self.optim.zero_grad()
 
             # forward and backward
@@ -395,43 +502,96 @@
         self.estimator.update_obs(self.knn(self.output))   # 4
         alpha, beta, O, Q, iterations = self.estimator.EM(self.output.max(1)[1].detach().cpu().numpy(), self.conf.gsl['tolerance'])
         adj = torch.tensor(prob_to_adj(Q, self.conf.gsl['threshold']),dtype=torch.float32, device=self.device).to_sparse()
         print('Iteration {:04d} | Time(s) {:.4f} | EM step {:04d}'.format(iter+1,time.time()-t,self.estimator.count))
         return adj
 
     def learn(self, debug=False):
+        '''
+        Learning process of GEN.
+
+        Parameters
+        ----------
+        debug : bool
+            Whether to print statistics during training.
 
+        Returns
+        -------
+        result : dict
+            A dict containing train, valid and test metrics.
+        graph : torch.tensor
+            The learned structure.
+        '''
         adj = self.adj
 
         for iter in range(self.conf.training['n_iters']):
             self.train_gcn(iter, adj, debug)
             adj = self.structure_learning(iter)
 
         print('Optimization Finished!')
         print('Time(s): {:.4f}'.format(self.total_time))
         loss_test, acc_test, _, _ = self.test()
         self.result['test'] = acc_test
         print("Loss(test) {:.4f} | Acc(test) {:.4f}".format(loss_test.item(), acc_test))
         return self.result, self.best_graph
 
     def evaluate(self, test_mask, normalized_adj):
+        '''
+        Evaluation procedure of GEN.
+
+        Parameters
+        ----------
+        test_mask : torch.tensor
+            A boolean tensor indicating whether the node is in the data set.
+        normalized_adj : torch.tensor
+            Adjacency matrix.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        hidden_output : torch.tensor        
+            Hidden output of the model.
+        output : torch.tensor        
+            Output of the model.
+        '''
         self.model.eval()
         with torch.no_grad():
             hidden_output, output = self.model((self.feats, normalized_adj, False))
         logits = output[test_mask]
         labels = self.labels[test_mask]
         loss=self.loss_fn(logits, labels)
         return loss, self.metric(labels.cpu().numpy(), logits.detach().cpu().numpy()), hidden_output, output
 
     def test(self):
+        '''
+        Test procedure of GEN.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        hidden_output : torch.tensor        
+            Hidden output of the model.
+        output : torch.tensor        
+            Output of the model.
+        '''
         self.model.load_state_dict(self.weights)
-        normalized_adj = normalize_sp_tensor(self.best_graph)
+        normalized_adj = normalize(self.best_graph, sparse=True)
         return self.evaluate(self.test_mask, normalized_adj)
 
     def set_method(self):
+        '''
+        Function to set the model and necessary variables for each run, automatically called in function `set`.
+
+        '''
         if self.conf.model['type']=='gcn':
             self.model = GCN(self.dim_feats, self.conf.model['n_hidden'], self.num_targets, self.conf.model['n_layers'],
                              self.conf.model['dropout'], self.conf.model['input_dropout'], self.conf.model['norm'],
                              self.conf.model['n_linear'], self.conf.model['spmm_type'], self.conf.model['act'],
                              self.conf.model['input_layer'], self.conf.model['output_layer'], weight_initializer='glorot',
                              bias_initializer='zeros').to(self.device)
         elif self.conf.model['type']=='appnp':
@@ -444,33 +604,53 @@
                                       weight_decay=self.conf.training['weight_decay'])
         self.best_iter = 0
         self.hidden_output = None
         self.output = None
 
 
 class IDGLSolver(Solver):
+    '''
+    A solver to train, evaluate, test IDGL in a run.
+
+    Parameters
+    ----------
+    conf : argparse.Namespace
+        Config file.
+    dataset : opengsl.data.Dataset
+        The dataset.
+
+    Attributes
+    ----------
+    method_name : str
+        The name of the method.
+
+    Examples
+    --------
+    >>> # load dataset
+    >>> import opengsl.dataset
+    >>> dataset = opengsl.data.Dataset('cora', feat_norm=True)
+    >>> # load config file
+    >>> import opengsl.config.load_conf
+    >>> conf = opengsl.config.load_conf('idgl', 'cora')
+    >>>
+    >>> solver = IDGLSolver(conf, dataset)
+    >>> # Conduct a experiment run.
+    >>> acc, new_structure = solver.run_exp(split=0, debug=True)
+    '''
     def __init__(self, conf, dataset):
-        '''
-        Create a solver for digl to train, evaluate, test in a run. Some operations are conducted during initialization instead of "set_method" to avoid repetitive computations.
-        Parameters
-        ----------
-        conf : config file
-        dataset: dataset object containing all things about dataset
-        '''
         super().__init__(conf, dataset)
         self.method_name = "idgl"
         print("Solver Version : [{}]".format("idgl"))
         self.conf = conf
-        self.normalize = normalize_sp_tensor if self.conf.model['scalable_run'] else normalize
         self.run_epoch = self._scalable_run_whole_epoch if self.conf.model['scalable_run'] else self._run_whole_epoch
         if self.conf.model['scalable_run']:
-            self.normalized_adj = self.normalize(self.adj)
+            self.normalized_adj = normalize(self.adj, sparse=True)
         else:
             self.adj = self.adj.to_dense()
-            self.normalized_adj = normalize(self.adj)
+            self.normalized_adj = normalize(self.adj, sparse=False)
 
     def _run_whole_epoch(self, mode='train', debug=False):
 
         # prepare
         training = mode == 'train'
         if mode == 'train':
             idx = self.train_mask
@@ -608,15 +788,29 @@
         graph_loss += self.conf.training['smoothness_ratio'] * torch.trace(torch.mm(features.transpose(-1, -2), torch.mm(L, features))) / int(np.prod(out_adj.shape))
         ones_vec = torch.ones(out_adj.size(-1)).to(self.device)
         graph_loss += -self.conf.training['degree_ratio'] * torch.mm(ones_vec.unsqueeze(0), torch.log(torch.mm(out_adj, ones_vec.unsqueeze(-1)) + 1e-12)).squeeze() / out_adj.shape[-1]
         graph_loss += self.conf.training['sparsity_ratio'] * torch.sum(torch.pow(out_adj, 2)) / int(np.prod(out_adj.shape))
         return graph_loss
 
     def learn(self, debug=False):
+        '''
+        Learning process of IDGL.
 
+        Parameters
+        ----------
+        debug : bool
+            Whether to print statistics during training.
+
+        Returns
+        -------
+        result : dict
+            A dict containing train, valid and test metrics.
+        graph : torch.tensor
+            The learned structure.
+        '''
         wait = 0
 
         for epoch in range(self.conf.training['max_epochs']):
             t = time.time()
             improve = ''
 
             # training phase
@@ -653,27 +847,52 @@
         with torch.no_grad():
             loss_test, acc_test, _ = self.run_epoch(mode='test', debug=debug)
         self.result['test']=acc_test
         print(acc_test)
         return self.result, self.best_graph
 
     def set_method(self):
+        '''
+        Function to set the model and necessary variables for each run, automatically called in function `set`.
+
+        '''
         self.model = IDGL(self.conf, self.dim_feats, self.num_targets).to(self.device)
         self.optimizer = torch.optim.Adam(self.model.parameters(), lr=self.conf.training['lr'], weight_decay=self.conf.training['weight_decay'])
 
 
 class PROGNNSolver(Solver):
+    '''
+    A solver to train, evaluate, test ProGNN in a run.
+
+    Parameters
+    ----------
+    conf : argparse.Namespace
+        Config file.
+    dataset : opengsl.data.Dataset
+        The dataset.
+
+    Attributes
+    ----------
+    method_name : str
+        The name of the method.
+
+    Examples
+    --------
+    >>> # load dataset
+    >>> import opengsl.dataset
+    >>> dataset = opengsl.data.Dataset('cora', feat_norm=True)
+    >>> # load config file
+    >>> import opengsl.config.load_conf
+    >>> conf = opengsl.config.load_conf('prognn', 'cora')
+    >>>
+    >>> solver = PROGNNSolver(conf, dataset)
+    >>> # Conduct a experiment run.
+    >>> acc, new_structure = solver.run_exp(split=0, debug=True)
+    '''
     def __init__(self, conf, dataset):
-        '''
-        Create a solver for prognn to train, evaluate, test in a run. Some operations are conducted during initialization instead of "set_method" to avoid repetitive computations.
-        Parameters
-        ----------
-        conf : config file
-        dataset: dataset object containing all things about dataset
-        '''
         super().__init__(conf, dataset)
         self.method_name = "prognn"
         print("Solver Version : [{}]".format("prognn"))
         self.adj = self.adj.to_dense()
 
     def train_gcn(self, epoch, debug=False):
         normalized_adj = self.estimator.normalize()
@@ -773,15 +992,29 @@
 
         #print
         if debug:
             print("Epoch {:05d} | Time(s) {:.4f} | Loss(adj) {:.4f} | Loss(val) {:.4f} | Acc(val) {:.4f} | {}".format(
                 epoch+1, time.time() - t, total_loss.item(), loss_val, acc_val, improve))
 
     def learn(self, debug=False):
+        '''
+        Learning process of PROGNN.
 
+        Parameters
+        ----------
+        debug : bool
+            Whether to print statistics during training.
+
+        Returns
+        -------
+        result : dict
+            A dict containing train, valid and test metrics.
+        graph : torch.tensor
+            The learned structure.
+        '''
         for epoch in range(self.conf.training['n_epochs']):
             for i in range(int(self.conf.training['outer_steps'])):
                 self.train_adj(epoch, debug=debug)
 
             for i in range(int(self.conf.training['inner_steps'])):
                 self.train_gcn(epoch, debug=debug)
 
@@ -799,30 +1032,61 @@
         print('Time(s): {:.4f}'.format(self.total_time))
         loss_test, acc_test = self.test()
         self.result['test'] = acc_test
         print("Loss(test) {:.4f} | Acc(test) {:.4f}".format(loss_test.item(), acc_test))
         return self.result, self.best_graph
 
     def evaluate(self, test_mask, normalized_adj):
+        '''
+        Evaluation procedure of PROGNN.
+
+        Parameters
+        ----------
+        test_mask : torch.tensor
+            A boolean tensor indicating whether the node is in the data set.
+        normalized_adj : torch.tensor
+            Adjacency matrix.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        '''
         self.model.eval()
         self.estimator.eval()
         with torch.no_grad():
             logits = self.model((self.feats, normalized_adj, False))[-1]
         logits = logits[test_mask]
         labels = self.labels[test_mask]
         loss=self.loss_fn(logits, labels)
         return loss, self.metric(labels.cpu().numpy(), logits.detach().cpu().numpy())
 
     def test(self):
+        '''
+        Test procedure of PROGNN.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        '''
         self.model.load_state_dict(self.weights)
         self.estimator.estimated_adj.data.copy_(self.best_graph)
         normalized_adj = self.estimator.normalize()
         return self.evaluate(self.test_mask, normalized_adj)
 
     def set_method(self):
+        '''
+        Function to set the model and necessary variables for each run, automatically called in function `set`.
+
+        '''
         if self.conf.model['type'] == 'gcn':
             self.model = GCN(self.dim_feats, self.conf.model['n_hidden'], self.num_targets, self.conf.model['n_layers'],
                              self.conf.model['dropout'], self.conf.model['input_dropout'], self.conf.model['norm'],
                              self.conf.model['n_linear'], self.conf.model['spmm_type'], self.conf.model['act'],
                              self.conf.model['input_layer'], self.conf.model['output_layer'],
                              weight_initializer='uniform').to(self.device)
         else:
@@ -839,41 +1103,75 @@
         self.optimizer_nuclear = PGD(self.estimator.parameters(), proxs=[prox_operators.prox_nuclear_cuda],
                                      lr=self.conf.training['lr_adj'], alphas=[self.conf.gsl['beta']])
 
         self.wait = 0
 
 
 class GTSolver(Solver):
+    '''
+    A solver to train, evaluate, test GT in a run.
+
+    Parameters
+    ----------
+    conf : argparse.Namespace
+        Config file.
+    dataset : opengsl.data.Dataset
+        The dataset.
+
+    Attributes
+    ----------
+    method_name : str
+        The name of the method.
+
+    Examples
+    --------
+    >>> # load dataset
+    >>> import opengsl.dataset
+    >>> dataset = opengsl.data.Dataset('cora', feat_norm=True)
+    >>> # load config file
+    >>> import opengsl.config.load_conf
+    >>> conf = opengsl.config.load_conf('gt', 'cora')
+    >>>
+    >>> solver = GTSolver(conf, dataset)
+    >>> # Conduct a experiment run.
+    >>> acc, _ = solver.run_exp(split=0, debug=True)
+    '''
     def __init__(self, conf, dataset):
-        '''
-        Create a solver for gt to train, evaluate, test in a run. Some operations are conducted during initialization instead of "set_method" to avoid repetitive computations.
-        Parameters
-        ----------
-        conf : config file
-        dataset: dataset object containing all things about dataset
-        '''
         super().__init__(conf, dataset)
         self.method_name = "gt"
         print("Solver Version : [{}]".format("gt"))
         # prepare dgl graph
         edges = self.adj.coalesce().indices().cpu()
         self.graph = dgl.graph((edges[0], edges[1]), num_nodes=self.n_nodes, idtype=torch.int)
         self.graph = dgl.add_self_loop(self.graph).to(self.device)
 
 
     def learn(self, debug=False):
+        '''
+        Learning process of GRCN.
 
+        Parameters
+        ----------
+        debug : bool
+            Whether to print statistics during training.
+
+        Returns
+        -------
+        result : dict
+            A dict containing train, valid and test metrics.
+        0 : constant
+        '''
         for epoch in range(self.conf.training['n_epochs']):
             improve = ''
             t0 = time.time()
             self.model.train()
             self.optim.zero_grad()
 
             # forward and backward
-            x, output, _ = self.model(self.feats, self.graph, self.labels.cpu().numpy())
+            x, output, _ = self.model(self.feats, self.graph, self.labels.cpu())
 
             loss_train = self.loss_fn(output[self.train_mask], self.labels[self.train_mask])
             acc_train = self.metric(self.labels[self.train_mask].cpu().numpy(), output[self.train_mask].detach().cpu().numpy())
             loss_train.backward()
             self.optim.step()
 
             # Evaluate
@@ -898,51 +1196,120 @@
         print('Time(s): {:.4f}'.format(self.total_time))
         loss_test, acc_test, homo_heads = self.test()
         self.result['test'] = acc_test
         print("Loss(test) {:.4f} | Acc(test) {:.4f}".format(loss_test.item(), acc_test))
         return self.result, 0
 
     def evaluate(self, test_mask, graph_analysis=False):
+        '''
+        Evaluation procedure of GT.
+
+        Parameters
+        ----------
+        test_mask : torch.tensor
+            A boolean tensor indicating whether the node is in the data set.
+        graph_analysis : bool
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        homo_heads
+
+        '''
         self.model.eval()
         with torch.no_grad():
-            x, output, homo_heads = self.model(self.feats, self.graph, self.labels.cpu().numpy(), graph_analysis)
+            x, output, homo_heads = self.model(self.feats, self.graph, self.labels.cpu(), graph_analysis)
         logits = output[test_mask]
         labels = self.labels[test_mask]
         loss = self.loss_fn(logits, labels)
         return loss, self.metric(labels.cpu().numpy(), logits.detach().cpu().numpy()), homo_heads
 
     def test(self):
+        '''
+        Test procedure of GT.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        homo_heads
+        '''
         self.model.load_state_dict(self.weights)
         return self.evaluate(self.test_mask, graph_analysis=self.conf.analysis['graph_analysis'])
 
     def set_method(self):
+        '''
+        Function to set the model and necessary variables for each run, automatically called in function `set`.
+
+        '''
         self.model = GT(self.dim_feats, self.conf.model['n_hidden'], self.num_targets, self.conf.model['n_layers'],
                    self.conf.model['dropout'], self.conf.model['input_dropout'], self.conf.model['norm_type'],
                    self.conf.model['n_heads'], self.conf.model['act'], input_layer=self.conf.model['input_layer'],
                         ff=self.conf.model['ff'], output_layer=self.conf.model['output_layer'],
                         use_norm=self.conf.model['use_norm'], use_redisual=self.conf.model['use_residual'],
                         hidden_dim_multiplier=self.conf.model['hidden_dim_multiplier']).to(self.device)
         self.optim = torch.optim.Adam(self.model.parameters(), lr=self.conf.training['lr'],
                                  weight_decay=self.conf.training['weight_decay'])
 
 
 class SLAPSSolver(Solver):
-    def __init__(self, conf, dataset):
-        '''
-        Create a solver for slaps to train, evaluate, test in a run. SLAPS don't use the origin edges from the dataset.
+    '''
+        A solver to train, evaluate, test SLAPS in a run.
+
         Parameters
         ----------
-        conf : config file
-        dataset: dataset object containing all things about dataset
+        conf : argparse.Namespace
+            Config file.
+        dataset : opengsl.data.Dataset
+            The dataset.
+
+        Attributes
+        ----------
+        method_name : str
+            The name of the method.
+
+        Examples
+        --------
+        >>> # load dataset
+        >>> import opengsl.dataset
+        >>> dataset = opengsl.data.Dataset('cora', feat_norm=True)
+        >>> # load config file
+        >>> import opengsl.config.load_conf
+        >>> conf = opengsl.config.load_conf('slaps', 'cora')
+        >>>
+        >>> solver = SLAPSSolver(conf, dataset)
+        >>> # Conduct a experiment run.
+        >>> acc, new_structure = solver.run_exp(split=0, debug=True)
         '''
+    def __init__(self, conf, dataset):
         super().__init__(conf, dataset)
         self.method_name = "slaps"
         print("Solver Version : [{}]".format("slaps"))
 
     def learn(self, debug=False):
+        '''
+        Learning process of SLAPS.
+
+        Parameters
+        ----------
+        debug : bool
+            Whether to print statistics during training.
+
+        Returns
+        -------
+        result : dict
+            A dict containing train, valid and test metrics.
+        graph : torch.tensor
+            The learned structure.
+        '''
         for epoch in range(self.conf.training['n_epochs']):
             improve = ''
             t0 = time.time()
             self.model.train()
             self.optim.zero_grad()
             
             # forward and backward
@@ -979,61 +1346,119 @@
         print('Time(s): {:.4f}'.format(self.total_time))
         loss_test, acc_test = self.test()
         self.result['test'] = acc_test
         print("Loss(test) {:.4f} | Acc(test) {:.4f}".format(loss_test.item(), acc_test))
         return self.result, self.best_graph
     
     def evaluate(self, test_mask):
+        '''
+        Evaluation procedure of SLAPS.
+
+        Parameters
+        ----------
+        test_mask : torch.tensor
+            A boolean tensor indicating whether the node is in the data set.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        '''
         self.model.eval()
         with torch.no_grad():
             output, _, _ = self.model(self.feats)
         logits = output[test_mask]
         labels = self.labels[test_mask]
         loss = self.loss_fn(logits, labels)
         return loss, self.metric(labels.cpu().numpy(), logits.detach().cpu().numpy())
 
     def set_method(self):
+        '''
+        Function to set the model and necessary variables for each run, automatically called in function `set`.
+
+        '''
         self.model = SLAPS(self.n_nodes, self.dim_feats, self.num_targets, self.feats, self.device, self.conf).to(self.device)
         self.optim = torch.optim.Adam([
             {'params': self.model.gcn_c.parameters(), 'lr': self.conf.training['lr'], 'weight_decay': self.conf.training['weight_decay']},
             {'params': self.model.gcn_dae.parameters(), 'lr': self.conf.training['lr_dae'], 'weight_decay': self.conf.training['weight_decay_dae']}
         ])
 
 
 class NODEFORMERSolver(Solver):
+    '''
+    A solver to train, evaluate, test Nodeformer in a run.
+
+    Parameters
+    ----------
+    conf : argparse.Namespace
+        Config file.
+    dataset : opengsl.data.Dataset
+        The dataset.
+
+    Attributes
+    ----------
+    method_name : str
+        The name of the method.
+
+    Examples
+    --------
+    >>> # load dataset
+    >>> import opengsl.dataset
+    >>> dataset = opengsl.data.Dataset('cora', feat_norm=True)
+    >>> # load config file
+    >>> import opengsl.config.load_conf
+    >>> conf = opengsl.config.load_conf('nodeoformer', 'cora')
+    >>>
+    >>> solver = NODEFORMERSolverSolver(conf, dataset)
+    >>> # Conduct a experiment run.
+    >>> acc, _ = solver.run_exp(split=0, debug=True)
+    '''
     def __init__(self, conf, dataset):
-        '''
-        Create a solver for grcn to train, evaluate, test in a run. Some operations are conducted during initialization instead of "set_method" to avoid repetitive computations.
-        Parameters
-        ----------
-        conf : config file
-        dataset: dataset object containing all things about dataset
-        '''
         super().__init__(conf, dataset)
         self.method_name = "nodeformer"
         print("Solver Version : [{}]".format("nodeformer"))
         edge_index = self.adj.coalesce().indices().cpu()
         loop_edge_index = torch.stack([torch.arange(self.n_nodes), torch.arange(self.n_nodes)])
         adj = torch.cat([edge_index, loop_edge_index], dim=1).to(self.device)
         self.adjs = []
         self.adjs.append(adj)
         for i in range(conf.model['rb_order'] - 1):  # edge_index of high order adjacency
             adj = adj_mul(adj, adj, self.n_nodes)
             self.adjs.append(adj)
 
     def set_method(self):
+        '''
+        Function to set the model and necessary variables for each run, automatically called in function `set`.
+
+        '''
         self.model = NodeFormer(self.dim_feats, self.conf.model['n_hidden'], self.num_targets, num_layers=self.conf.model['n_layers'], dropout=self.conf.model['dropout'],
                            num_heads=self.conf.model['n_heads'], use_bn=self.conf.model['use_bn'], nb_random_features=self.conf.model['M'],
                            use_gumbel=self.conf.model['use_gumbel'], use_residual=self.conf.model['use_residual'], use_act=self.conf.model['use_act'],
                            use_jk=self.conf.model['use_jk'],
                            nb_gumbel_sample=self.conf.model['K'], rb_order=self.conf.model['rb_order'], rb_trans=self.conf.model['rb_trans']).to(self.device)
         self.model.reset_parameters()
         self.optim = torch.optim.Adam(self.model.parameters(), weight_decay=self.conf.training['weight_decay'], lr=self.conf.training['lr'])
 
     def learn(self, debug=False):
+        '''
+        Learning process of Nodeformer.
+
+        Parameters
+        ----------
+        debug : bool
+            Whether to print statistics during training.
+
+        Returns
+        -------
+        result : dict
+            A dict containing train, valid and test metrics.
+        0 : constant
+        '''
 
         for epoch in range(self.conf.training['n_epochs']):
             improve = ''
             t0 = time.time()
             self.model.train()
             self.optim.zero_grad()
 
@@ -1069,39 +1494,88 @@
         print('Time(s): {:.4f}'.format(self.total_time))
         loss_test, acc_test = self.test()
         self.result['test'] = acc_test
         print("Loss(test) {:.4f} | Acc(test) {:.4f}".format(loss_test.item(), acc_test))
         return self.result, 0
 
     def evaluate(self, test_mask):
+        '''
+        Evaluation procedure of NODEFORMER.
+
+        Parameters
+        ----------
+        test_mask : torch.tensor
+            A boolean tensor indicating whether the node is in the data set.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        '''
         self.model.eval()
         with torch.no_grad():
             output, _ = self.model(self.feats, self.adjs, self.conf.model['tau'])
         logits = output[test_mask]
         labels = self.labels[test_mask]
         loss=self.loss_fn(logits, labels)
         return loss, self.metric(labels.cpu().numpy(), logits.detach().cpu().numpy())
 
 
 class SEGSLSolver(Solver):
+    '''
+    A solver to train, evaluate, test SEGSL in a run.
+
+    Parameters
+    ----------
+    conf : argparse.Namespace
+        Config file.
+    dataset : opengsl.data.Dataset
+        The dataset.
+
+    Attributes
+    ----------
+    method_name : str
+        The name of the method.
+
+    Examples
+    --------
+    >>> # load dataset
+    >>> import opengsl.dataset
+    >>> dataset = opengsl.data.Dataset('cora', feat_norm=True)
+    >>> # load config file
+    >>> import opengsl.config.load_conf
+    >>> conf = opengsl.config.load_conf('segsl', 'cora')
+    >>>
+    >>> solver = SEGSLSolver(conf, dataset)
+    >>> # Conduct a experiment run.
+    >>> acc, new_structure = solver.run_exp(split=0, debug=True)
+    '''
     def __init__(self, conf, dataset):
-        '''
-        Create a solver for segsl to train, evaluate, test in a run. Some operations are conducted during initialization instead of "set_method" to avoid repetitive computations.
-        Parameters
-        ----------
-        conf : config file
-        dataset: dataset object containing all things about dataset
-        '''
         super().__init__(conf, dataset)
         self.method_name = "segsl"
         print("Solver Version : [{}]".format("segsl"))
-        self.normalize = normalize_sp_tensor if self.conf.dataset['sparse'] else normalize
 
     def learn(self, debug=False):
+        '''
+        Learning process of SEGSL.
 
+        Parameters
+        ----------
+        debug : bool
+            Whether to print statistics during training.
+
+        Returns
+        -------
+        result : dict
+            A dict containing train, valid and test metrics.
+        graph : torch.tensor
+            The learned structure.
+        '''
         adj = self.adj.to_dense()
         adj.fill_diagonal_(1)
         adj = adj.to_sparse()
 
         for iter in range(self.conf.training['n_iters']):
             logits = self.train_gcn(iter, adj, debug)
             adj = self.structure_learning(logits, adj)
@@ -1122,15 +1596,15 @@
 
         if debug:
             print('==== Iteration {:04d} ===='.format(iter+1))
         t = time.time()
         improve_1 = ''
         best_loss_val = 10
         best_acc_val = 0
-        normalized_adj = self.normalize(adj, add_loop=False)
+        normalized_adj = normalize(adj, add_loop=False, sparse=True)
         for epoch in range(self.conf.training['n_epochs']):
             improve_2 = ''
             t0 = time.time()
             self.model.train()
             self.optim.zero_grad()
 
             # forward and backward
@@ -1166,16 +1640,16 @@
         print('Iteration {:04d} | Time(s) {:.4f} | Loss(val):{:.4f} | Acc(val):{:.4f} | {}'.format(iter+1,time.time()-t, best_loss_val, best_acc_val, improve_1))
 
         return output
 
     def structure_learning(self, logits, adj):
         edge_index = adj.coalesce().indices().t()
 
-        k = knn_maxE1(edge_index, logits.unsqueeze(1))  # edge index对称有自环
-        edge_index_2 = add_knn(k, logits.unsqueeze(1), edge_index)
+        k = knn_maxE1(edge_index, logits)  # edge index对称有自环
+        edge_index_2 = add_knn(k, logits, edge_index)
         weight = get_weight(logits, edge_index_2)
         adj_matrix = get_adj_matrix(self.n_nodes, edge_index_2, weight)
 
         code_tree = PartitionTree(adj_matrix=np.array(adj_matrix))
         code_tree.build_coding_tree(self.conf.gsl['se'])
 
         community, isleaf = get_community(code_tree)
@@ -1207,44 +1681,103 @@
                           num_nodes=self.n_nodes).to(self.device)
         graph = dgl.remove_self_loop(graph)
         graph = dgl.add_self_loop(graph)
         adj = graph.adj().to(self.device)
         return adj
 
     def evaluate(self, test_mask, normalized_adj):
+        '''
+        Evaluation procedure of SEGSL.
+
+        Parameters
+        ----------
+        test_mask : torch.tensor
+            A boolean tensor indicating whether the node is in the data set.
+        normalized_adj : torch.tensor
+            Adjacency matrix.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        hidden_output : torch.tensor        
+            Hidden output of the model.
+        output : torch.tensor        
+           Output of the model.
+        '''
         self.model.eval()
         with torch.no_grad():
             hidden_output, output = self.model((self.feats, normalized_adj, False))
         logits = output[test_mask]
         labels = self.labels[test_mask]
         loss=self.loss_fn(logits, labels)
         return loss, self.metric(labels.cpu().numpy(), logits.detach().cpu().numpy()), hidden_output, output
 
     def set_method(self):
+        '''
+        Function to set the model and necessary variables for each run, automatically called in function `set`.
+
+        '''
         self.best_iter = 0
 
     def test(self):
+        '''
+        Test procedure of SEGSL.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        hidden_output : torch.tensor        
+            Hidden output of the model.
+        output : torch.tensor        
+           Output of the model.
+        '''
         self.model.load_state_dict(self.weights)
-        normalized_adj = self.normalize(self.best_graph, add_loop=False)
+        normalized_adj = normalize(self.best_graph, add_loop=False, sparse=True)
         return self.evaluate(self.test_mask, normalized_adj)
 
 
 class SUBLIMESolver(Solver):
+    '''
+    A solver to train, evaluate, test SUBLIME in a run.
+
+    Parameters
+    ----------
+    conf : argparse.Namespace
+        Config file.
+    dataset : opengsl.data.Dataset
+        The dataset.
+
+    Attributes
+    ----------
+    method_name : str
+        The name of the method.
+
+    Examples
+    --------
+    >>> # load dataset
+    >>> import opengsl.dataset
+    >>> dataset = opengsl.data.Dataset('cora', feat_norm=True)
+    >>> # load config file
+    >>> import opengsl.config.load_conf
+    >>> conf = opengsl.config.load_conf('sublime', 'cora')
+    >>>
+    >>> solver = SUBLIMESolver(conf, dataset)
+    >>> # Conduct a experiment run.
+    >>> acc, new_structure = solver.run_exp(split=0, debug=True)
+    '''
     def __init__(self, conf, dataset):
-        '''
-        Create a solver for sublime to train, evaluate, test in a run. Some operations are conducted during initialization instead of "set_method" to avoid repetitive computations.
-        Parameters
-        ----------
-        conf : config file
-        dataset: dataset object containing all things about dataset
-        '''
         super().__init__(conf, dataset)
         self.method_name = "sublime"
         print("Solver Version : [{}]".format("sublime"))
-        self.normalize = normalize_sp_tensor if self.conf.sparse else normalize
 
     def loss_gcl(self, model, graph_learner, features, anchor_adj):
 
         # view 1: anchor graph
         if self.conf.maskfeat_rate_anchor:
             mask_v1, _ = get_feat_mask(features, self.conf.maskfeat_rate_anchor)
             features_v1 = features * (1 - mask_v1)
@@ -1259,15 +1792,15 @@
             features_v2 = features * (1 - mask)
         else:
             features_v2 = copy.deepcopy(features)
 
         learned_adj = graph_learner(features)   # 这个learned adj是有自环的
         if not self.conf.sparse:
             learned_adj = (learned_adj + learned_adj.T) / 2
-            learned_adj = self.normalize(learned_adj, add_loop=False)
+            learned_adj = normalize(learned_adj, add_loop=False, sparse=False)
 
         z2, _ = model(features_v2, learned_adj, 'learner')
 
         # compute loss
         if self.conf.contrast_batch_size:
             node_idxs = list(range(features.shape[0]))
             batches = split_batch(node_idxs, self.conf.contrast_batch_size)
@@ -1325,33 +1858,76 @@
                 print("Epoch {:05d} | Time(s) {:.4f} | Loss(train) {:.4f} | Acc(train) {:.4f} | Loss(val) {:.4f} | Acc(val) {:.4f} | {}".format(
                     epoch+1, time.time() -t0, loss_train.item(), acc_train, loss_val, acc_val, improve_2))
 
 
         print('Time(s) {:.4f} | Loss(val):{:.4f} | Acc(val):{:.4f} | {}'.format(time.time()-t, best_loss_val, best_acc_val, improve_1))
 
     def evaluate(self, model, test_mask, adj):
+        '''
+        Evaluation procedure of GRCN.
+
+        Parameters
+        ----------
+        model : torch.nn.Module
+            model.
+        test_mask : torch.tensor
+            A boolean tensor indicating whether the node is in the data set.
+        adj : torch.tensor
+            Adjacency matrix.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        '''
         model.eval()
         with torch.no_grad():
             output = model(self.feats, adj)
         logits = output[test_mask]
         labels = self.labels[test_mask]
         loss=self.loss_fn(logits, labels)
         return loss, self.metric(labels.cpu().numpy(), logits.detach().cpu().numpy())
 
     def test(self):
+        '''
+        Test procedure of SUBLIME.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        metric : float
+            Evaluation metric.
+        '''
         model = GCN_SUB(nfeat=self.dim_feats, nhid=self.conf.hidden_dim_cls, nclass=self.num_targets,
                         n_layers=self.conf.n_layers_cls, dropout=self.conf.dropout_cls,
                         dropout_adj=self.conf.dropedge_cls, sparse=self.conf.sparse).to(self.device)
         model.load_state_dict(self.weights)
         adj = self.best_graph_test
         return self.evaluate(model, self.test_mask, adj)
 
     def learn(self, debug=False):
+        '''
+        Learning process of SUBLIME.
 
-        anchor_adj = self.normalize(self.anchor_adj_raw, add_loop=False)
+        Parameters
+        ----------
+        debug : bool
+            Whether to print statistics during training.
+
+        Returns
+        -------
+        result : dict
+            A dict containing train, valid and test metrics.
+        graph : torch.tensor
+            The learned structure.
+        '''
+        anchor_adj = normalize(self.anchor_adj_raw, add_loop=False, sparse=self.conf.sparse)
 
         if self.conf.sparse:
             anchor_adj_torch_sparse = copy.deepcopy(anchor_adj)
             anchor_adj = torch_sparse_to_dgl_graph(anchor_adj)
 
         for epoch in range(1, self.conf.epochs + 1):
 
@@ -1397,19 +1973,23 @@
         print('Time(s): {:.4f}'.format(self.total_time))
         loss_test, acc_test = self.test()
         self.result['test'] = acc_test
         print("Loss(test) {:.4f} | Acc(test) {:.4f}".format(loss_test.item(), acc_test))
         return self.result, self.best_graph
 
     def set_method(self):
+        '''
+        Function to set the model and necessary variables for each run, automatically called in function `set`.
+
+        '''
         if self.conf.sparse:
             self.anchor_adj_raw = self.adj
         else:
             self.anchor_adj_raw = self.adj.to_dense()
-        anchor_adj = self.normalize(self.anchor_adj_raw, add_loop=False)
+        anchor_adj = normalize(self.anchor_adj_raw, add_loop=False, sparse=self.conf.sparse)
         if self.conf.type_learner == 'fgp':
             self.graph_learner = FGP_learner(self.feats.cpu(), self.conf.k, self.conf.sim_function, 6, self.conf.sparse)
         elif self.conf.type_learner == 'mlp':
             self.graph_learner = MLP_learner(2, self.feats.shape[1], self.conf.k, self.conf.sim_function, 6, self.conf.sparse,
                                  self.conf.activation_learner)
         elif self.conf.type_learner == 'att':
             self.graph_learner = ATT_learner(2, self.feats.shape[1], self.conf.k, self.conf.sim_function, 6, self.conf.sparse,
@@ -1424,43 +2004,64 @@
                          conf=self.conf).to(self.device)
         self.optimizer_cl = torch.optim.Adam(self.model.parameters(), lr=self.conf.lr, weight_decay=self.conf.wd)
         self.optimizer_learner = torch.optim.Adam(self.graph_learner.parameters(), lr=self.conf.lr,
                                              weight_decay=self.conf.wd)
 
 
 class STABLESolver(Solver):
+    '''
+    A solver to train, evaluate, test Stable in a run.
+
+    Parameters
+    ----------
+    conf : argparse.Namespace
+        Config file.
+    dataset : opengsl.data.Dataset
+        The dataset.
+
+    Attributes
+    ----------
+    method_name : str
+        The name of the method.
+
+    Examples
+    --------
+    >>> # load dataset
+    >>> import opengsl.dataset
+    >>> dataset = opengsl.data.Dataset('cora', feat_norm=True)
+    >>> # load config file
+    >>> import opengsl.config.load_conf
+    >>> conf = opengsl.config.load_conf('stable', 'cora')
+    >>>
+    >>> solver = STABLESolver(conf, dataset)
+    >>> # Conduct a experiment run.
+    >>> acc, new_structure = solver.run_exp(split=0, debug=True)
+    '''
     def __init__(self, conf, dataset):
-        '''
-        Create a solver for stable to train, evaluate, test in a run. Some operations are conducted during initialization instead of "set_method" to avoid repetitive computations.
-        Parameters
-        ----------
-        conf : config file
-        dataset: dataset object containing all things about dataset
-        '''
         super().__init__(conf, dataset)
         self.method_name = "stable"
         print("Solver Version : [{}]".format("stable"))
         self.adj = sparse_tensor_to_scipy_sparse(self.adj)
         self.processed_adj = preprocess_adj(self.feats.cpu().numpy(), self.adj, threshold=self.conf.jt)
 
     def pretrain(self, debug=False):
 
         # generate 2 augment views
         adj_delete = self.adj - self.processed_adj
         aug_adj1 = aug_random_edge(self.processed_adj, adj_delete=adj_delete, recover_percent=self.conf.recover_percent)  # random drop edges
         aug_adj2 = aug_random_edge(self.processed_adj, adj_delete=adj_delete, recover_percent=self.conf.recover_percent)  # random drop edges
-        sp_adj = sparse_normalize(self.processed_adj+(sp.eye(self.n_nodes) * self.conf.beta),
+        sp_adj = normalize_sp_matrix(self.processed_adj+(sp.eye(self.n_nodes) * self.conf.beta),
                                   add_loop=False)
-        sp_aug_adj1 = sparse_normalize(aug_adj1 + (sp.eye(self.n_nodes) * self.conf.beta),
+        sp_aug_adj1 = normalize_sp_matrix(aug_adj1 + (sp.eye(self.n_nodes) * self.conf.beta),
                                   add_loop=False)
-        sp_aug_adj2 = sparse_normalize(aug_adj2 + (sp.eye(self.n_nodes) * self.conf.beta),
+        sp_aug_adj2 = normalize_sp_matrix(aug_adj2 + (sp.eye(self.n_nodes) * self.conf.beta),
                                   add_loop=False)
-        sp_adj = sparse_mx_to_torch_sparse_tensor(sp_adj).to(self.device)
-        sp_aug_adj1 = sparse_mx_to_torch_sparse_tensor(sp_aug_adj1).to(self.device)
-        sp_aug_adj2 = sparse_mx_to_torch_sparse_tensor(sp_aug_adj2).to(self.device)
+        sp_adj = scipy_sparse_to_sparse_tensor(sp_adj).to(self.device)
+        sp_aug_adj1 = scipy_sparse_to_sparse_tensor(sp_aug_adj1).to(self.device)
+        sp_aug_adj2 = scipy_sparse_to_sparse_tensor(sp_aug_adj2).to(self.device)
 
         # contrastive learning
         weights = None
         wait = 0
         best = 1e9
         best_t = 0
         b_xent = torch.nn.BCEWithLogitsLoss()
@@ -1550,59 +2151,98 @@
         model.load_state_dict(weights)
         loss_test, acc_test = test(model)
         self.result['test'] = acc_test
         print("Loss(test) {:.4f} | Acc(test) {:.4f}".format(loss_test.item(), acc_test))
         return self.result
 
     def learn(self, debug=False):
+        '''
+        Learning process of STABLE.
+
+        Parameters
+        ----------
+        debug : bool
+            Whether to print statistics during training.
+
+        Returns
+        -------
+        result : dict
+            A dict containing train, valid and test metrics.
+        graph : torch.tensor
+            The learned structure.
+        '''
         embeds = self.pretrain(debug)
         embeds = embeds.squeeze(dim=0)
 
         # prunue the graph
         adj_clean = preprocess_adj(embeds.cpu().numpy(), self.adj, jaccard=False, threshold=self.conf.cos)
-        adj_clean = sparse_mx_to_torch_sparse_tensor(adj_clean).to(self.device).to_dense()
+        adj_clean = scipy_sparse_to_sparse_tensor(adj_clean).to(self.device).to_dense()
         # add k neighbors
         get_reliable_neighbors(adj_clean, embeds, k=self.conf.k, degree_threshold=self.conf.threshold)
         # 得到的是0-1 无自环的图
 
-        normalized_adj_clean = normalize(adj_clean)   # 未使用论文中对归一化的改进
+        normalized_adj_clean = normalize(adj_clean, sparse=False)   # 未使用论文中对归一化的改进
         result = self.train_gcn(embeds, normalized_adj_clean, debug)
         return result, adj_clean
 
     def set_method(self):
+        '''
+        Function to set the model and necessary variables for each run, automatically called in function `set`.
+
+        '''
         self.model = DGI(self.dim_feats, self.conf.n_embed, 'prelu').to(self.device)
         self.optim = torch.optim.Adam(self.model.parameters(), lr=self.conf.pretrain['lr'], weight_decay=self.conf.pretrain['weight_decay'])
         
         
 class CoGSLSolver(Solver):
+    '''
+    A solver to train, evaluate, test CoGSL in a run.
 
+    Parameters
+    ----------
+    conf : argparse.Namespace
+        Config file.
+    dataset : opengsl.data.Dataset
+        The dataset.
+
+    Attributes
+    ----------
+    method_name : str
+        The name of the method.
+
+    Examples
+    --------
+    >>> # load dataset
+    >>> import opengsl.dataset
+    >>> dataset = opengsl.data.Dataset('cora', feat_norm=True)
+    >>> # load config file
+    >>> import opengsl.config.load_conf
+    >>> conf = opengsl.config.load_conf('cogsl', 'cora')
+    >>>
+    >>> solver = CoGSLSolver(conf, dataset)
+    >>> # Conduct a experiment run.
+    >>> acc, new_structure = solver.run_exp(split=0, debug=True)
+    '''
     def __init__(self, conf, dataset):
-        '''
-        Create a solver for CoGSL to train, evaluate, test in a run.
-        Parameters
-        ----------
-        conf : config file
-        dataset: dataset object containing all things about dataset
-        '''
         super().__init__(conf, dataset)
         self.method_name = "cogsl"
         print("Solver Version : [{}]".format("CoGSL"))
         self.adj = (torch.eye(self.adj.shape[0]).to(self.device) + self.adj.to_dense()).to_sparse()
         if self.conf.dataset['init'] :
             _view1 = eval("self."+self.conf.dataset["name_view1"]+"()")
             self.view1_indices = self.get_indices(self.conf.dataset["view1_indices"], _view1, self.conf.dataset["view1_k"])
             _view2 = eval("self."+self.conf.dataset["name_view2"]+"()")
             self.view2_indices = self.get_indices(self.conf.dataset["view2_indices"], _view2, self.conf.dataset["view2_k"])
         else:
             _view1 = sp.load_npz(self.conf.dataset['view1_path'])
             _view2 = sp.load_npz(self.conf.dataset['view2_path'])
             self.view1_indices = torch.load(self.conf.dataset['view1_indices_path'])
             self.view2_indices = torch.load(self.conf.dataset['view2_indices_path'])
-        self.view1 = sparse_mx_to_torch_sparse_tensor( sparse_normalize(_view1,False) )
-        self.view2 = sparse_mx_to_torch_sparse_tensor( sparse_normalize(_view2,False) )
+        self.view1 = scipy_sparse_to_sparse_tensor(normalize_sp_matrix(_view1, False))
+        self.view2 = scipy_sparse_to_sparse_tensor(normalize_sp_matrix(_view2, False))
         self.loss_fn = F.binary_cross_entropy if self.num_targets == 1 else F.nll_loss
         #self.train_mask = np.load('/root/dataset/citeseer/train.npy')
         #self.valid_mask = np.load('/root/dataset/citeseer/val.npy')
         #self.test_mask = np.load('/root/dataset/citeseer/test.npy')
         #print(self.view1_indices.shape)
         #print(self.view1.shape)
         #print(self.view2_indices.shape)
@@ -1616,15 +2256,15 @@
         return sp.coo_matrix(adj)
 
     def view_adj(self):
         return sparse_tensor_to_scipy_sparse(self.adj)
 
     def view_diff(self):
         adj = sparse_tensor_to_scipy_sparse(self.adj)
-        at = sparse_normalize(adj,False)
+        at = normalize_sp_matrix(adj,False)
         result = self.conf.dataset['diff_alpha'] * sp.linalg.inv(sp.eye(adj.shape[0]) - (1 - self.conf.dataset['diff_alpha']) * at)
         return result
 
     def view_sub(self):
         adj = (self.adj.to_dense() - torch.eye(self.adj.shape[0]).to(self.device)).to_sparse()
         index = []
         for i in range(self.adj.indices().shape[1]):
@@ -1690,24 +2330,27 @@
         loss_v, _ = self.loss_acc(logits_v[self.train_mask], self.labels[self.train_mask])
         return self.conf.model['cls_coe'] * loss_v + (loss_v1 + loss_v2) * (1 - self.conf.model['cls_coe']) / 2, views
 
 
     def learn(self, debug=False):
         '''
         Learning process of CoGSL.
+
         Parameters
         ----------
-        debug
+        debug : bool
+            Whether to print statistics during training.
 
         Returns
         -------
-
+        result : dict
+            A dict containing train, valid and test metrics.
+        graph : torch.tensor
+            The learned structure.
         '''
-
-
         self.best_acc_val = 0
         self.best_loss_val = 1e9
         self.best_test = 0
         self.best_v_cls_weight = None
         torch.autograd.set_detect_anomaly(True)
 
         for epoch in range(self.conf.training['main_epoch']):
@@ -1763,15 +2406,27 @@
         self.result['test'] = acc_test
         #print("Test_Macro: ", test_f1_macro, "\tTest_Micro: ", test_f1_micro, "\tAUC: ", auc)
         print("Loss(test) {:.4f} | Acc(test) {:.4f}".format(loss_test.item(), acc_test))
         return self.result, self.best_graph.to_dense()
 
 
     def evaluate(self, test_mask):
+        '''
+        Evaluation procedure of CoGSL.
+
+        Parameters
+        ----------
+        test_mask : torch.tensor
+            A boolean tensor indicating whether the node is in the data set.
 
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        '''
         logits = self.model.get_v_cls_loss(self.view, self.feats)
 
         return self.loss_acc(logits[test_mask], self.labels[test_mask])
 
     def set_method(self):
         self.model = CoGSL(self.dim_feats, self.conf.model['cls_hid_1'], self.n_classes, self.conf.model['gen_hid'],
                            self.conf.model['mi_hid_1'], self.conf.model['com_lambda_v1'], self.conf.model['com_lambda_v2'],
@@ -1803,13 +2458,21 @@
     #        else:
     #            auc = roc_auc_score(y_true=label.detach().cpu().numpy(),
     #                                                    y_score=best_proba[:,1].detach().cpu().numpy()
     #                                                    )
     #        return test_f1_macro, test_f1_micro, auc
 
     def test(self):
+        '''
+        Test procedure of CoGSL.
+
+        Returns
+        -------
+        loss : float
+            Evaluation loss.
+        '''
         self.model.cls.encoder_v.load_state_dict(self.weights)
         self.model.eval()
         self.view = self.best_graph
 
         return self.evaluate(self.test_mask)
```

### Comparing `opengsl-0.0.4/opengsl/method/models/cogsl.py` & `opengsl-0.0.5/opengsl/method/models/cogsl.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/gaug.py` & `opengsl-0.0.5/opengsl/method/models/gaug.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .gcn import GCN
 from .gnn_modules import APPNP
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import pyro as pyro
-from ...utils.utils import normalize
+from opengsl.data.preprocess.normalize import normalize
 import numpy as np
 from sklearn.metrics import roc_auc_score, average_precision_score
 
 
 class VGAE(nn.Module):
     """ GAE/VGAE as edge prediction model """
     def __init__(self, dim_feats, conf):
@@ -123,8 +123,20 @@
             op.step()
 
     def update_lr(self, op_index, new_lr):
         """ update the learning rate of one optimizer
         Parameters: op_index: the index of the optimizer to update
                     new_lr:   new learning rate for that optimizer """
         for param_group in self.optimizers[op_index].param_groups:
-            param_group['lr'] = new_lr
+            param_group['lr'] = new_lr
+
+
+def get_lr_schedule_by_sigmoid(n_epochs, lr, warmup):
+    """ schedule the learning rate with the sigmoid function.
+    The learning rate will start with near zero and end with near lr """
+    factors = torch.FloatTensor(np.arange(n_epochs))
+    factors = ((factors / factors[-1]) * (warmup * 2)) - warmup
+    factors = torch.sigmoid(factors)
+    # range the factors to [0, 1]
+    factors = (factors - factors[0]) / (factors[-1] - factors[0])
+    lr_schedule = factors * lr
+    return lr_schedule
```

### Comparing `opengsl-0.0.4/opengsl/method/models/gcn.py` & `opengsl-0.0.5/opengsl/method/models/gcn.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/gcn_idgl.py` & `opengsl-0.0.5/opengsl/method/models/gcn_idgl.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/gen.py` & `opengsl-0.0.5/opengsl/method/models/gen.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/gnn_modules.py` & `opengsl-0.0.5/opengsl/method/models/gnn_modules.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/grcn.py` & `opengsl-0.0.5/opengsl/method/models/grcn.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/gt.py` & `opengsl-0.0.5/opengsl/method/models/gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import torch
 from torch import nn
 from dgl import ops
 from dgl.nn.functional import edge_softmax
 import torch.nn.functional as F
 import scipy.sparse as sp
 from ...utils.utils import get_homophily
+from opengsl.utils.utils import scipy_sparse_to_sparse_tensor
 
 
 class TransformerAttentionModule(nn.Module):
     def __init__(self, dim, dim_out, num_heads, dropout):
         super().__init__()
 
         assert dim % num_heads == 0, 'Dimension mismatch: hidden_dim should be a multiple of num_heads.'
@@ -68,15 +69,16 @@
         edges = graph.edges()
         row = edges[0].cpu().numpy()
         col = edges[1].cpu().numpy()
         # values = adj.coalesce().values().numpy()
         # return sp.coo_matrix((values, (row, col)), shape=adj.shape)
         for i in range(n_heads):
             values = attn_weights.squeeze()[:, i].cpu().detach().numpy()
-            adj = sp.coo_matrix((values, (row, col)), shape=(n_nodes, n_nodes)).todense()
+            adj = sp.coo_matrix((values, (row, col)), shape=(n_nodes, n_nodes))
+            adj = scipy_sparse_to_sparse_tensor(adj)
             homophily[i] = get_homophily(labels, adj)
         return homophily
 
 
 class FeedForwardModule(nn.Module):
     def __init__(self, dim, hidden_dim_multiplier, dropout, act):
         super().__init__()
@@ -229,15 +231,16 @@
         edges = graph.edges()
         row = edges[0].cpu().numpy()
         col = edges[1].cpu().numpy()
         # values = adj.coalesce().values().numpy()
         # return sp.coo_matrix((values, (row, col)), shape=adj.shape)
         for i in range(n_heads):
             values = attn_weights.squeeze()[:, i].cpu().detach().numpy()
-            adj = sp.coo_matrix((values, (row, col)), shape=(n_nodes, n_nodes)).todense()
+            adj = sp.coo_matrix((values, (row, col)), shape=(n_nodes, n_nodes))
+            adj = scipy_sparse_to_sparse_tensor(adj)
             homophily[i] = get_homophily(labels, adj)
         return homophily
 
 
 class GatedResidual(nn.Module):
     """ This is the implementation of Eq (5), i.e., gated residual connection between block.
     """
```

### Comparing `opengsl-0.0.4/opengsl/method/models/idgl.py` & `opengsl-0.0.5/opengsl/method/models/idgl.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/jknet.py` & `opengsl-0.0.5/opengsl/method/models/jknet.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/nodeformer.py` & `opengsl-0.0.5/opengsl/method/models/nodeformer.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/prognn.py` & `opengsl-0.0.5/opengsl/method/models/prognn.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/segsl.py` & `opengsl-0.0.5/opengsl/method/models/segsl.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/slaps.py` & `opengsl-0.0.5/opengsl/method/models/slaps.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/stable.py` & `opengsl-0.0.5/opengsl/method/models/stable.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl/method/models/sublime.py` & `opengsl-0.0.5/opengsl/method/models/sublime.py`

 * *Files identical despite different names*

### Comparing `opengsl-0.0.4/opengsl.egg-info/SOURCES.txt` & `opengsl-0.0.5/opengsl.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,190 +1,195 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-opengsl/ExpManager.py
 opengsl/__init__.py
-opengsl/load_conf.py
 opengsl.egg-info/PKG-INFO
 opengsl.egg-info/SOURCES.txt
 opengsl.egg-info/dependency_links.txt
 opengsl.egg-info/requires.txt
 opengsl.egg-info/top_level.txt
-opengsl/configs/appnp/appnp_amazon-ratings.yaml
-opengsl/configs/appnp/appnp_blogcatalog.yaml
-opengsl/configs/appnp/appnp_citeseer.yaml
-opengsl/configs/appnp/appnp_cora.yaml
-opengsl/configs/appnp/appnp_flickr.yaml
-opengsl/configs/appnp/appnp_hetero.yaml
-opengsl/configs/appnp/appnp_minesweeper.yaml
-opengsl/configs/appnp/appnp_pubmed.yaml
-opengsl/configs/appnp/appnp_questions.yaml
-opengsl/configs/appnp/appnp_roman-empire.yaml
-opengsl/configs/appnp/appnp_wiki-cooc.yaml
-opengsl/configs/cogsl/cogsl_citeseer.yaml
-opengsl/configs/cogsl/cogsl_cora.yaml
-opengsl/configs/gat/gat_amazon-ratings.yaml
-opengsl/configs/gat/gat_blogcatalog.yaml
-opengsl/configs/gat/gat_citeseer.yaml
-opengsl/configs/gat/gat_cora.yaml
-opengsl/configs/gat/gat_flickr.yaml
-opengsl/configs/gat/gat_minesweeper.yaml
-opengsl/configs/gat/gat_pubmed.yaml
-opengsl/configs/gat/gat_questions.yaml
-opengsl/configs/gat/gat_roman-empire.yaml
-opengsl/configs/gat/gat_wiki-cooc.yaml
-opengsl/configs/gaug/gaug_amazon-ratings.yaml
-opengsl/configs/gaug/gaug_blogcatalog.yaml
-opengsl/configs/gaug/gaug_citeseer.yaml
-opengsl/configs/gaug/gaug_cora.yaml
-opengsl/configs/gaug/gaug_flickr.yaml
-opengsl/configs/gaug/gaug_minesweeper.yaml
-opengsl/configs/gaug/gaug_pubmed.yaml
-opengsl/configs/gaug/gaug_roman-empire.yaml
-opengsl/configs/gaug/gaug_wiki-cooc.yaml
-opengsl/configs/gcn/gcn_amazon-ratings.yaml
-opengsl/configs/gcn/gcn_blogcatalog.yaml
-opengsl/configs/gcn/gcn_citeseer.yaml
-opengsl/configs/gcn/gcn_cora.yaml
-opengsl/configs/gcn/gcn_flickr.yaml
-opengsl/configs/gcn/gcn_minesweeper.yaml
-opengsl/configs/gcn/gcn_pubmed.yaml
-opengsl/configs/gcn/gcn_questions.yaml
-opengsl/configs/gcn/gcn_roman-empire.yaml
-opengsl/configs/gcn/gcn_wiki-cooc.yaml
-opengsl/configs/gen/gen_amazon-ratings.yaml
-opengsl/configs/gen/gen_blogcatalog.yaml
-opengsl/configs/gen/gen_citeseer.yaml
-opengsl/configs/gen/gen_cora.yaml
-opengsl/configs/gen/gen_flickr.yaml
-opengsl/configs/gen/gen_minesweeper.yaml
-opengsl/configs/gen/gen_pubmed.yaml
-opengsl/configs/gen/gen_wiki-cooc.yaml
-opengsl/configs/gprgnn/gprgnn_amazon-ratings.yaml
-opengsl/configs/gprgnn/gprgnn_blogcatalog.yaml
-opengsl/configs/gprgnn/gprgnn_citeseer.yaml
-opengsl/configs/gprgnn/gprgnn_cora.yaml
-opengsl/configs/gprgnn/gprgnn_flickr.yaml
-opengsl/configs/gprgnn/gprgnn_minesweeper.yaml
-opengsl/configs/gprgnn/gprgnn_pubmed.yaml
-opengsl/configs/gprgnn/gprgnn_questions.yaml
-opengsl/configs/gprgnn/gprgnn_roman-empire.yaml
-opengsl/configs/gprgnn/gprgnn_wiki-cooc.yaml
-opengsl/configs/grcn/grcn_amazon-ratings.yaml
-opengsl/configs/grcn/grcn_blogcatalog.yaml
-opengsl/configs/grcn/grcn_citeseer.yaml
-opengsl/configs/grcn/grcn_cora.yaml
-opengsl/configs/grcn/grcn_flickr.yaml
-opengsl/configs/grcn/grcn_minesweeper.yaml
-opengsl/configs/grcn/grcn_pubmed.yaml
-opengsl/configs/grcn/grcn_questions.yaml
-opengsl/configs/grcn/grcn_roman-empire.yaml
-opengsl/configs/grcn/grcn_wiki-cooc.yaml
-opengsl/configs/gt/gt_amazon-ratings.yaml
-opengsl/configs/gt/gt_blogcatalog.yaml
-opengsl/configs/gt/gt_citeseer.yaml
-opengsl/configs/gt/gt_cora.yaml
-opengsl/configs/gt/gt_flickr.yaml
-opengsl/configs/gt/gt_minesweeper.yaml
-opengsl/configs/gt/gt_pubmed.yaml
-opengsl/configs/gt/gt_questions.yaml
-opengsl/configs/gt/gt_roman-empire.yaml
-opengsl/configs/gt/gt_wiki-cooc.yaml
-opengsl/configs/idgl/idgl_amazon-ratings.yaml
-opengsl/configs/idgl/idgl_blogcatalog.yaml
-opengsl/configs/idgl/idgl_citeseer.yaml
-opengsl/configs/idgl/idgl_cora.yaml
-opengsl/configs/idgl/idgl_flickr.yaml
-opengsl/configs/idgl/idgl_minesweeper.yaml
-opengsl/configs/idgl/idgl_pubmed.yaml
-opengsl/configs/idgl/idgl_questions.yaml
-opengsl/configs/idgl/idgl_roman-empire.yaml
-opengsl/configs/idgl/idgl_wiki-cooc.yaml
-opengsl/configs/jknet/jknet_amazon-ratings.yaml
-opengsl/configs/jknet/jknet_blogcatalog.yaml
-opengsl/configs/jknet/jknet_citeseer.yaml
-opengsl/configs/jknet/jknet_cora.yaml
-opengsl/configs/jknet/jknet_flickr.yaml
-opengsl/configs/jknet/jknet_minesweeper.yaml
-opengsl/configs/jknet/jknet_pubmed.yaml
-opengsl/configs/jknet/jknet_questions.yaml
-opengsl/configs/jknet/jknet_roman-empire.yaml
-opengsl/configs/jknet/jknet_wiki-cooc.yaml
-opengsl/configs/link/link.yaml
-opengsl/configs/lpa/lpa.yaml
-opengsl/configs/nodeformer/nodeformer_amazon-ratings.yaml
-opengsl/configs/nodeformer/nodeformer_blogcatalog.yaml
-opengsl/configs/nodeformer/nodeformer_citeseer.yaml
-opengsl/configs/nodeformer/nodeformer_cora.yaml
-opengsl/configs/nodeformer/nodeformer_flickr.yaml
-opengsl/configs/nodeformer/nodeformer_minesweeper.yaml
-opengsl/configs/nodeformer/nodeformer_pubmed.yaml
-opengsl/configs/nodeformer/nodeformer_questions.yaml
-opengsl/configs/nodeformer/nodeformer_roman-empire.yaml
-opengsl/configs/nodeformer/nodeformer_wiki-cooc.yaml
-opengsl/configs/prognn/prognn_blogcatalog.yaml
-opengsl/configs/prognn/prognn_citeseer.yaml
-opengsl/configs/prognn/prognn_cora.yaml
-opengsl/configs/prognn/prognn_flickr.yaml
-opengsl/configs/prognn/prognn_minesweeper.yaml
-opengsl/configs/prognn/prognn_pubmed.yaml
-opengsl/configs/prognn/prognn_questions.yaml
-opengsl/configs/prognn/prognn_roman-empire.yaml
-opengsl/configs/prognn/prognn_wiki-cooc.yaml
-opengsl/configs/segsl/segsl_blogcatalog.yaml
-opengsl/configs/segsl/segsl_citeseer.yaml
-opengsl/configs/segsl/segsl_cora.yaml
-opengsl/configs/segsl/segsl_flickr.yaml
-opengsl/configs/segsl/segsl_pubmed.yaml
-opengsl/configs/sgc/sgc_amazon-ratings.yaml
-opengsl/configs/sgc/sgc_blogcatalog.yaml
-opengsl/configs/sgc/sgc_citeseer.yaml
-opengsl/configs/sgc/sgc_cora.yaml
-opengsl/configs/sgc/sgc_flickr.yaml
-opengsl/configs/sgc/sgc_minesweeper.yaml
-opengsl/configs/sgc/sgc_pubmed.yaml
-opengsl/configs/sgc/sgc_questions.yaml
-opengsl/configs/sgc/sgc_roman-empire.yaml
-opengsl/configs/sgc/sgc_wiki-cooc.yaml
-opengsl/configs/slaps/slaps_amazon-ratings.yaml
-opengsl/configs/slaps/slaps_blogcatalog.yaml
-opengsl/configs/slaps/slaps_citeseer.yaml
-opengsl/configs/slaps/slaps_cora.yaml
-opengsl/configs/slaps/slaps_flickr.yaml
-opengsl/configs/slaps/slaps_minesweeper.yaml
-opengsl/configs/slaps/slaps_pubmed.yaml
-opengsl/configs/slaps/slaps_questions.yaml
-opengsl/configs/slaps/slaps_roman-empire.yaml
-opengsl/configs/slaps/slaps_wiki-cooc.yaml
-opengsl/configs/stable/stable_amazon-ratings.yaml
-opengsl/configs/stable/stable_blogcatalog.yaml
-opengsl/configs/stable/stable_citeseer.yaml
-opengsl/configs/stable/stable_cora.yaml
-opengsl/configs/stable/stable_flickr.yaml
-opengsl/configs/stable/stable_minesweeper.yaml
-opengsl/configs/stable/stable_pubmed.yaml
-opengsl/configs/stable/stable_roman-empire.yaml
-opengsl/configs/stable/stable_wiki-cooc.yaml
-opengsl/configs/sublime/sublime_amazon-ratings.yaml
-opengsl/configs/sublime/sublime_blogcatalog.yaml
-opengsl/configs/sublime/sublime_citeseer.yaml
-opengsl/configs/sublime/sublime_cora.yaml
-opengsl/configs/sublime/sublime_flickr.yaml
-opengsl/configs/sublime/sublime_minesweeper.yaml
-opengsl/configs/sublime/sublime_pubmed.yaml
-opengsl/configs/sublime/sublime_questions.yaml
-opengsl/configs/sublime/sublime_roman-empire.yaml
-opengsl/configs/sublime/sublime_wiki-cooc.yaml
+opengsl/config/__init__.py
+opengsl/config/util.py
+opengsl/config/appnp/appnp_amazon-ratings.yaml
+opengsl/config/appnp/appnp_blogcatalog.yaml
+opengsl/config/appnp/appnp_citeseer.yaml
+opengsl/config/appnp/appnp_cora.yaml
+opengsl/config/appnp/appnp_flickr.yaml
+opengsl/config/appnp/appnp_hetero.yaml
+opengsl/config/appnp/appnp_minesweeper.yaml
+opengsl/config/appnp/appnp_pubmed.yaml
+opengsl/config/appnp/appnp_questions.yaml
+opengsl/config/appnp/appnp_roman-empire.yaml
+opengsl/config/appnp/appnp_wiki-cooc.yaml
+opengsl/config/cogsl/cogsl_citeseer.yaml
+opengsl/config/cogsl/cogsl_cora.yaml
+opengsl/config/gat/gat_amazon-ratings.yaml
+opengsl/config/gat/gat_blogcatalog.yaml
+opengsl/config/gat/gat_citeseer.yaml
+opengsl/config/gat/gat_cora.yaml
+opengsl/config/gat/gat_flickr.yaml
+opengsl/config/gat/gat_minesweeper.yaml
+opengsl/config/gat/gat_pubmed.yaml
+opengsl/config/gat/gat_questions.yaml
+opengsl/config/gat/gat_roman-empire.yaml
+opengsl/config/gat/gat_wiki-cooc.yaml
+opengsl/config/gaug/gaug_amazon-ratings.yaml
+opengsl/config/gaug/gaug_blogcatalog.yaml
+opengsl/config/gaug/gaug_citeseer.yaml
+opengsl/config/gaug/gaug_cora.yaml
+opengsl/config/gaug/gaug_flickr.yaml
+opengsl/config/gaug/gaug_minesweeper.yaml
+opengsl/config/gaug/gaug_pubmed.yaml
+opengsl/config/gaug/gaug_roman-empire.yaml
+opengsl/config/gaug/gaug_wiki-cooc.yaml
+opengsl/config/gcn/gcn_amazon-ratings.yaml
+opengsl/config/gcn/gcn_blogcatalog.yaml
+opengsl/config/gcn/gcn_citeseer.yaml
+opengsl/config/gcn/gcn_cora.yaml
+opengsl/config/gcn/gcn_flickr.yaml
+opengsl/config/gcn/gcn_minesweeper.yaml
+opengsl/config/gcn/gcn_pubmed.yaml
+opengsl/config/gcn/gcn_questions.yaml
+opengsl/config/gcn/gcn_roman-empire.yaml
+opengsl/config/gcn/gcn_wiki-cooc.yaml
+opengsl/config/gen/gen_amazon-ratings.yaml
+opengsl/config/gen/gen_blogcatalog.yaml
+opengsl/config/gen/gen_citeseer.yaml
+opengsl/config/gen/gen_cora.yaml
+opengsl/config/gen/gen_flickr.yaml
+opengsl/config/gen/gen_minesweeper.yaml
+opengsl/config/gen/gen_pubmed.yaml
+opengsl/config/gen/gen_wiki-cooc.yaml
+opengsl/config/gprgnn/gprgnn_amazon-ratings.yaml
+opengsl/config/gprgnn/gprgnn_blogcatalog.yaml
+opengsl/config/gprgnn/gprgnn_citeseer.yaml
+opengsl/config/gprgnn/gprgnn_cora.yaml
+opengsl/config/gprgnn/gprgnn_flickr.yaml
+opengsl/config/gprgnn/gprgnn_minesweeper.yaml
+opengsl/config/gprgnn/gprgnn_pubmed.yaml
+opengsl/config/gprgnn/gprgnn_questions.yaml
+opengsl/config/gprgnn/gprgnn_roman-empire.yaml
+opengsl/config/gprgnn/gprgnn_wiki-cooc.yaml
+opengsl/config/grcn/grcn_amazon-ratings.yaml
+opengsl/config/grcn/grcn_blogcatalog.yaml
+opengsl/config/grcn/grcn_citeseer.yaml
+opengsl/config/grcn/grcn_cora.yaml
+opengsl/config/grcn/grcn_flickr.yaml
+opengsl/config/grcn/grcn_minesweeper.yaml
+opengsl/config/grcn/grcn_pubmed.yaml
+opengsl/config/grcn/grcn_questions.yaml
+opengsl/config/grcn/grcn_roman-empire.yaml
+opengsl/config/grcn/grcn_wiki-cooc.yaml
+opengsl/config/gt/gt_amazon-ratings.yaml
+opengsl/config/gt/gt_blogcatalog.yaml
+opengsl/config/gt/gt_citeseer.yaml
+opengsl/config/gt/gt_cora.yaml
+opengsl/config/gt/gt_flickr.yaml
+opengsl/config/gt/gt_minesweeper.yaml
+opengsl/config/gt/gt_pubmed.yaml
+opengsl/config/gt/gt_questions.yaml
+opengsl/config/gt/gt_roman-empire.yaml
+opengsl/config/gt/gt_wiki-cooc.yaml
+opengsl/config/idgl/idgl_amazon-ratings.yaml
+opengsl/config/idgl/idgl_blogcatalog.yaml
+opengsl/config/idgl/idgl_citeseer.yaml
+opengsl/config/idgl/idgl_cora.yaml
+opengsl/config/idgl/idgl_flickr.yaml
+opengsl/config/idgl/idgl_minesweeper.yaml
+opengsl/config/idgl/idgl_pubmed.yaml
+opengsl/config/idgl/idgl_questions.yaml
+opengsl/config/idgl/idgl_roman-empire.yaml
+opengsl/config/idgl/idgl_wiki-cooc.yaml
+opengsl/config/jknet/jknet_amazon-ratings.yaml
+opengsl/config/jknet/jknet_blogcatalog.yaml
+opengsl/config/jknet/jknet_citeseer.yaml
+opengsl/config/jknet/jknet_cora.yaml
+opengsl/config/jknet/jknet_flickr.yaml
+opengsl/config/jknet/jknet_minesweeper.yaml
+opengsl/config/jknet/jknet_pubmed.yaml
+opengsl/config/jknet/jknet_questions.yaml
+opengsl/config/jknet/jknet_roman-empire.yaml
+opengsl/config/jknet/jknet_wiki-cooc.yaml
+opengsl/config/link/link.yaml
+opengsl/config/lpa/lpa.yaml
+opengsl/config/nodeformer/nodeformer_amazon-ratings.yaml
+opengsl/config/nodeformer/nodeformer_blogcatalog.yaml
+opengsl/config/nodeformer/nodeformer_citeseer.yaml
+opengsl/config/nodeformer/nodeformer_cora.yaml
+opengsl/config/nodeformer/nodeformer_flickr.yaml
+opengsl/config/nodeformer/nodeformer_minesweeper.yaml
+opengsl/config/nodeformer/nodeformer_pubmed.yaml
+opengsl/config/nodeformer/nodeformer_questions.yaml
+opengsl/config/nodeformer/nodeformer_roman-empire.yaml
+opengsl/config/nodeformer/nodeformer_wiki-cooc.yaml
+opengsl/config/prognn/prognn_blogcatalog.yaml
+opengsl/config/prognn/prognn_citeseer.yaml
+opengsl/config/prognn/prognn_cora.yaml
+opengsl/config/prognn/prognn_flickr.yaml
+opengsl/config/prognn/prognn_minesweeper.yaml
+opengsl/config/prognn/prognn_pubmed.yaml
+opengsl/config/prognn/prognn_questions.yaml
+opengsl/config/prognn/prognn_roman-empire.yaml
+opengsl/config/prognn/prognn_wiki-cooc.yaml
+opengsl/config/segsl/segsl_blogcatalog.yaml
+opengsl/config/segsl/segsl_citeseer.yaml
+opengsl/config/segsl/segsl_cora.yaml
+opengsl/config/segsl/segsl_flickr.yaml
+opengsl/config/segsl/segsl_pubmed.yaml
+opengsl/config/sgc/sgc_amazon-ratings.yaml
+opengsl/config/sgc/sgc_blogcatalog.yaml
+opengsl/config/sgc/sgc_citeseer.yaml
+opengsl/config/sgc/sgc_cora.yaml
+opengsl/config/sgc/sgc_flickr.yaml
+opengsl/config/sgc/sgc_minesweeper.yaml
+opengsl/config/sgc/sgc_pubmed.yaml
+opengsl/config/sgc/sgc_questions.yaml
+opengsl/config/sgc/sgc_roman-empire.yaml
+opengsl/config/sgc/sgc_wiki-cooc.yaml
+opengsl/config/slaps/slaps_amazon-ratings.yaml
+opengsl/config/slaps/slaps_blogcatalog.yaml
+opengsl/config/slaps/slaps_citeseer.yaml
+opengsl/config/slaps/slaps_cora.yaml
+opengsl/config/slaps/slaps_flickr.yaml
+opengsl/config/slaps/slaps_minesweeper.yaml
+opengsl/config/slaps/slaps_pubmed.yaml
+opengsl/config/slaps/slaps_questions.yaml
+opengsl/config/slaps/slaps_roman-empire.yaml
+opengsl/config/slaps/slaps_wiki-cooc.yaml
+opengsl/config/stable/stable_amazon-ratings.yaml
+opengsl/config/stable/stable_blogcatalog.yaml
+opengsl/config/stable/stable_citeseer.yaml
+opengsl/config/stable/stable_cora.yaml
+opengsl/config/stable/stable_flickr.yaml
+opengsl/config/stable/stable_minesweeper.yaml
+opengsl/config/stable/stable_pubmed.yaml
+opengsl/config/stable/stable_roman-empire.yaml
+opengsl/config/stable/stable_wiki-cooc.yaml
+opengsl/config/sublime/sublime_amazon-ratings.yaml
+opengsl/config/sublime/sublime_blogcatalog.yaml
+opengsl/config/sublime/sublime_citeseer.yaml
+opengsl/config/sublime/sublime_cora.yaml
+opengsl/config/sublime/sublime_flickr.yaml
+opengsl/config/sublime/sublime_minesweeper.yaml
+opengsl/config/sublime/sublime_pubmed.yaml
+opengsl/config/sublime/sublime_questions.yaml
+opengsl/config/sublime/sublime_roman-empire.yaml
+opengsl/config/sublime/sublime_wiki-cooc.yaml
 opengsl/data/__init__.py
-opengsl/data/dataset.py
-opengsl/data/hetero_load.py
-opengsl/data/homophily_control.py
-opengsl/data/pyg_load.py
-opengsl/data/split.py
+opengsl/data/dataset/__init__.py
+opengsl/data/dataset/dataset.py
+opengsl/data/dataset/hetero_load.py
+opengsl/data/dataset/pyg_load.py
+opengsl/data/dataset/split.py
+opengsl/data/preprocess/__init__.py
+opengsl/data/preprocess/control_homophily.py
+opengsl/data/preprocess/normalize.py
+opengsl/expmanager/ExpManager.py
+opengsl/expmanager/__init__.py
 opengsl/method/__init__.py
 opengsl/method/gnnsolver.py
 opengsl/method/gslsolver.py
 opengsl/method/solver.py
 opengsl/method/models/__init__.py
 opengsl/method/models/cogsl.py
 opengsl/method/models/gaug.py
```

### Comparing `opengsl-0.0.4/setup.py` & `opengsl-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 from setuptools import setup, find_packages
 
 REQUIRES = """
 ruamel.yaml
 pandas
 scipy
 scikit-learn
-wandb
-pyro-api
-pyro-ppl
-numpy
+pyro-api==0.1.2
+pyro-ppl==1.8.0
 numba
-torch
-torch_geometric
-torch_sparse
-dgl
 """
 
 def get_install_requires():
     reqs = [req for req in REQUIRES.split("\n") if len(req) > 0]
     return reqs
 
 
-with open("README.md") as f:
+with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 
 def do_setup():
     setup(
         name="opengsl",
-        version="0.0.4",
+        version="0.0.5",
         description="A comprehensive benchmark for Graph Structure Learning.",
         url="https://github.com/OpenGSL/OpenGSL",
         author='Zhiyao Zhou, Sheng Zhou, Bochao Mao, Xuanyi Zhou',
         long_description=readme,
         long_description_content_type="text/markdown",
         install_requires=get_install_requires(),
         python_requires=">=3.7.0",
@@ -41,15 +35,14 @@
         keywords=["AI", "GNN", "graph structure learning"],
         classifiers=[
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Intended Audience :: Developers",
-            "Intended Audience :: Education",
             "Intended Audience :: Science/Research",
         ]
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

